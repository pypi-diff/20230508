# Comparing `tmp/checkpoint_tool-0.6.0.tar.gz` & `tmp/checkpoint_tool-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.6.0.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.0.tar", max compression
```

## Comparing `checkpoint_tool-0.6.0.tar` & `checkpoint_tool-0.7.0.tar`

### file list

```diff
@@ -1,4 +1,10 @@
--rw-r--r--   0        0        0     5113 2023-05-02 05:40:25.984486 checkpoint_tool-0.6.0/README.md
--rw-r--r--   0        0        0    23405 2023-05-02 05:49:00.896816 checkpoint_tool-0.6.0/checkpoint.py
--rw-r--r--   0        0        0      679 2023-05-02 05:53:00.536869 checkpoint_tool-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 checkpoint_tool-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     6998 2023-05-08 16:31:17.720383 checkpoint_tool-0.7.0/README.md
+-rw-r--r--   0        0        0      628 2023-05-08 15:48:28.630434 checkpoint_tool-0.7.0/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2327 2023-05-08 16:29:05.083367 checkpoint_tool-0.7.0/checkpoint/app.py
+-rw-r--r--   0        0        0    23235 2023-05-03 09:41:14.000902 checkpoint_tool-0.7.0/checkpoint/checkpoint_legacy.py
+-rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.0/checkpoint/database.py
+-rw-r--r--   0        0        0     6933 2023-05-04 14:52:06.276241 checkpoint_tool-0.7.0/checkpoint/graph.py
+-rw-r--r--   0        0        0    10381 2023-05-08 16:25:46.529256 checkpoint_tool-0.7.0/checkpoint/task.py
+-rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.0/checkpoint/types.py
+-rw-r--r--   0        0        0      676 2023-05-08 16:30:02.134130 checkpoint_tool-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.0/PKG-INFO
```

### Comparing `checkpoint_tool-0.6.0/README.md` & `checkpoint_tool-0.7.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,212 +1,238 @@
 # Checkpoint-tool
 
-A lightweight workflow management tool written in pure Python.
+A lightweight workflow building/execution/management tool written in pure Python.
 
 Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
 
 
 ## Installation
 
 ```
 pip install checkpoint-tool
 ```
 
 ## Usage
 
 ### Basic usage
 
-Create task with decorators:
+Workflow is a directed acyclic graph (DAG) of tasks, and task is a unit of work represented with a class.
+Here is an example.
 ```python
-from checkpoint import task, requires
+from checkpoint import Task, Req, Requires, Const
 
-# Mark a function as task
-@task
-def choose(n: int, k: int):
-    if 0 < k < n:
-        # Mark dependencies on other tasks;
-        # The return values of these tasks are passed as the arguments.
-        @requires(choose(n - 1, k - 1))
-        @requires(choose(n - 1, k)) 
-        def __(prev1: int, prev2: int) -> int:
-            # Main computation
-            return prev1 + prev2
-    elif k == 0 or k == n:
-        # Dependency can change according to the task parameters (`n` and `k`).
-        # Here, we need no dependency to compute `choose(n, 1)` or `choose(n, n)`.
-        def __() -> int:
-            return 1
-    else:
-        raise ValueError(f'{(n, k)}')
-
-    # Return function that produces a value instead of the value itself.
-    return __
-
-# Build the task graph to compute `choose(6, 3)`
-# and greedily consume it with `concurrent.futures.ProcessPoolExecutor`
-# (i.e., as parallel as possible).
-# The cache is stored at `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/...`
-# and reused whenever available.
-ans = choose(6, 3).run()
+# Define a task and **its entire upstream workflow** with a class definition.
+# Inheriting `Task` is necesary, as it takes care of all the work storing and reusing the result and tracking the dependencies.
+# `infer_task_type` decorator helps the type checker to infer the types of the task class. (optional)
+@infer_task_type
+class Choose(Task):
+    """ Compute the binomial coefficient. """
+    # Inside a task, we first declare the values that must be computed upstream with the descriptor `Req`.
+    # In this example, `Choose(n, k)` depends on `Choose(n - 1, k - 1)` and `Choose(n - 1, k)`,
+    # so it requires two `int` values.
+    # Either the type annotation `Requires[...]` or the assignment `= Req()` may be omitted.
+    prev1: Requires[int] = Req()
+    prev2: Requires[int] = Req()
+
+    def init(self, n: int, k: int):
+        # The prerequisite tasks and the other instance attributes are prepared here.
+        # It thus recursively defines all the tasks we need to run this task,
+        # i.e., the entire upstream workflow.
+
+        if 0 < k < n:
+            self.prev1 = Choose(n - 1, k - 1)
+            self.prev2 = Choose(n - 1, k)
+        elif k == 0 or k == n:
+            # We can just pass a value to a requirement slot directly without running tasks.
+            self.prev1 = Const(0)
+            self.prev2 = Const(1)
+        else:
+            raise ValueError(f'{(n, k)}')
+
+    def main(self) -> int:
+        # Here we define the main computation of the task,
+        # which is delayed until it is necessary.
+
+        # The return values of the prerequisite tasks are accessible via the descriptors:
+        return self.prev1 + self.prev2
+
+# To run tasks, use the `run_task()` method.
+ans = Choose(6, 3).worker.run_task()  # `ans` should be 6 Choose 3, which is 20.
+
+# It greedily executes all the necessary tasks as parallel as possible
+# and then spits out the return value of the task on which we call `run_task()`.
+# The return values of the intermediate tasks are cached at
+# `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/...`
+# and reused on the fly whenever possible.
 ```
 
 ### Deleting cache
 
 It is possible to selectively discard cache: 
 ```python
-# After some modificaiton of `choose(3, 3)`,
+# After some modificaiton of `Choose(3, 3)`,
 # selectively discard the cache corresponding to the modification.
-choose(3, 3).clear()
+Choose(3, 3).clear_task()
 
-# `ans` is recomputed tracing back to the computation of `choose(3, 3)`.
-ans = choose(6, 3).run()
+# `ans` is recomputed tracing back to the computation of `Choose(3, 3)`.
+ans = Choose(6, 3).run_task()
 
-# Delete all the cache associated with `choose`,
-# equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.choose`.
-choose.clear()            
+# Delete all the cache associated with `Choose`,
+# equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.Choose`.
+Choose.clear_all_tasks()            
 ```
 
-### Advanced IO
+### Limitations of Task I/O
 
-More complex inputs can be passed as long as it is JSON serializable:
+The arguments of the `init` method can be anything JSON serializable:
 ```python
-@task
-def f1(**param1):
+class T1(Task):
+    def init(self, **param1):
+        ...
     ...
 
-@task
-def f2(**param2):
+class T2(Task):
+    def init(self, **param2):
+        ...
     ...
 
-@task
-def f3(json_params):
-    @requires(f1(**json_params['param1']))
-    @requires(f2(**json_params['param2']))
-    def __(obj1, obj2):
+class T3(Task):
+    x1 = Req()
+    x2 = Req()
+
+    def init(self, json_params):
+        self.x1 = T1(**json_params['param1'])
+        self.x2 = T2(**json_params['param2'])
+
+    def main(self):
         ...
-    return __
 
-result = f3({'param1': { ... }, 'param2': { ... }}).run()
+result = T3({'param1': { ... }, 'param2': { ... }}).run_task()
 ```
 
-Even more complex inputs can be passed as `task`s:
+Otherwise they can be passed via `Task` and `Req`:
 ```python
-from checkpoint import Task
-
 Dataset = ...  # Some complex data structure
 Model = ...    # Some complex data structure
 
-@task
-def load_dataset():
-    def __() -> Dataset:
-        ...
-    return __
-
-@task
-def train_model(dataset_task: Task[Dataset]):
-    @requires(dataset_task)
-    def __(dataset) -> Model:
+class LoadDataset(Task):
+    def init(self):
+        pass
+
+    def main(self) -> Dataset:
+        ...
+
+class TrainModel(Task):
+    dataset: Requires[Datset]
+
+    def init(self, dataset_task: Task[Dataset]):
+        self.dataset = dataset_task
+
+    def main(self) -> Model:
         ...
-    return __
     
-@task
-def score_model(dataset_task: Task[Dataset], model_task: Task[Model]):
-    @requires(dataset_task)
-    @requires(model_task)
-    def __(dataset, model) -> float:
+class ScoreModel(Task):
+    dataset: Requires[Datset]
+    model: Requires[Model]
+
+    def init(self, dataset_task: Task[Dataset], model_task: Task[Model]):
+        self.dataset = dataset_task
+        self.model = model_task
+
+    def main(self) -> float:
         ...
-    return __
 
 
-dataset_task = load_dataset()
-model_task = train_model(dataset)
-score_task = score_model(dataset, model)
-print(score_task.run())
+dataset_task = LoadDataset()
+model_task = TrainModel(dataset)
+score_task = ScoreModel(dataset, model)
+print(score_task.run_task()
 ```
 
-Task dependencies can be specified with lists and dicts:
+`Req` accepts a list/dict of tasks and automatically unfolds it.
 ```python
-@task
-def summarize_scores(scores_tasks: dict[str, Task[float]]):
+from checkpoint import RequiresDict
 
-    @requires(score_tasks)
-    def __(score_dict):
-        ...
-    return __
+
+class SummarizeScores(Task):
+    scores: RequiresDict[str, float] = Req()  # Again, type annotation or assignment may be omitted.
+
+    def init(self, task_dict: dict[str, Task[float]]):
+        self.scores = task_dict
+
+    def main(self) -> float:
+        return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
 
+The output of the `main` method should be serializable with `cloudpickle`.
 Large outputs can be stored with compression via `zlib`:
 ```python
-@task(compress_level=-1)
-def large_output_task():
+class LargeOutputTask(Task, compress_level=-1):
     ...
 ```
 
 ### Data directories
 
-Use `TaskDirectory` to create a fresh directory dedicated to each task. The contents of the directory are cleared at each task call and persist until the task is `clear`ed.
+Use `DataPath(name)` to get a fresh path dedicated to each task.
+The parent directory is automatically created at
+`{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{cryptic_task_id}`
+and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
-from pathlib import Path
-from checkpoint import TaskDirectory
+from checkpoint import DataPath
 
-@task
-def train_model(...):
+class TrainModel(Task):
+    model_path = DataPath('model.bin')
+    ...
 
-    # Passing a new directory at
-    # `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/data/{cryptic_task_id}`
-    @requires(TaskDirectory())
-    def __(path: Path) -> str:
+    def main(self) -> str:
         ...
-        model_path = str(path / 'model.bin')
-        model.save(model_path)
-        return model_path
-
-    return __
+        model.save(self.model_path)  # Gives `Path('.../model.bin')`
+        return self.model_path
 ```
 
 ### Execution policy configuration
 
 One can control the task execution with `concurrent.futures.Executor` class:
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
-@task
-def my_task():
+class MyTask(Task):
     ...
 
 # Limit the number of parallel workers
-my_task().run(executor=ProcessPoolExecutor(max_workers=2))
+MyTask().run(executor=ProcessPoolExecutor(max_workers=2))
 
 # Thread-based parallelism
-my_task().run(executor=ThreadPoolExecutor())
+MyTask().run(executor=ThreadPoolExecutor())
 ```
 
 One can also control the concurrency at a task/queue level:
 ```python
-# Task-level concurrency limit
-my_task().run(rate_limit={my_task.queue: 2})
-
-# Queue-level concurrency limit
-@task(queue='gpu')
-def task_using_gpu():
+class TaskUsingGPU(Task, queue='gpu'):
     ...
 
-@task(queue='gpu')
-def another_task_using_gpu():
+class AnotherTaskUsingGPU(Task, queue='gpu'):
     ...
 
-# ...
-some_downstream_task.run(rate_limit={'gpu': 1})
+SomeDownstreamTask().run(rate_limits={'gpu': 1})  # Queue-level concurrency control
+SomeDownstreamTask().run(rate_limits={MemoryIntensiveTask.queue: 1})  # Task-level concurrency control
 
 ```
 
 ### Commandline tool
 We can use checkpoint-tool from commandline like `python -m checkpoint path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
 ```python
 # taskfile.py
 
-@task
-def main():
+class Main(Task):
     ...
 ```
-The command runs the `main` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
-Please refer to `python -m checkpoint --help` for more info.
+The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
+Please refer to `python -m checkpoint.app --help` for more info.
+
+
+
+## TODO
+ - [ ] Loader-based serialization
+ - [ ] Simple visualizers
+    - [ ] Task-wise progressbar
+    - [ ] Graph visualizer
```

### Comparing `checkpoint_tool-0.6.0/checkpoint.py` & `checkpoint_tool-0.7.0/checkpoint/checkpoint_legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,17 +523,14 @@
         self.G.remove_nodes_from(to_remove)
 
     def _transitive_reduction(self) -> None:
         TR = nx.transitive_reduction(self.G)
         TR.add_nodes_from(self.G.nodes(data=True))
         self.G = TR
 
-    def get_task_factories(self) -> dict[str, TaskFactory[..., Any]]:
-        return dict((path, attr['task'].task_factory) for (path, _), attr in self.G.nodes.items())
-
     def get_initial_tasks(self) -> dict[str, list[TaskKey]]:
         leaves = [x for x in self.G if self.G.in_degree(x) == 0]
         return self._group_by_queue(leaves)
 
     def _group_by_queue(self, nodes: list[TaskKey]) -> dict[str, list[TaskKey]]:
         out = defaultdict(list)
         for x in nodes:
```

### Comparing `checkpoint_tool-0.6.0/pyproject.toml` & `checkpoint_tool-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.6.0"
+version = "0.7.0"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
-packages = [{include = "checkpoint.py"}]
+packages = [{include = "checkpoint"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.5.0"
 diskcache = "^5.6.1"
 cloudpickle = "^2.2.1"
 networkx = "^3.1"
```


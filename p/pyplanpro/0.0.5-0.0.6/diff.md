# Comparing `tmp/pyplanpro-0.0.5.tar.gz` & `tmp/pyplanpro-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplanpro-0.0.5.tar", last modified: Mon May  1 14:44:17 2023, max compression
+gzip compressed data, was "pyplanpro-0.0.6.tar", last modified: Mon May  8 09:41:01 2023, max compression
```

## Comparing `pyplanpro-0.0.5.tar` & `pyplanpro-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/PyPlanPro/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/PyPlanPro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/PyPlanPro/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/heuristic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/scheduler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/pyplanpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/tests/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/scheduler/test_heuristic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/tests/stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/stress/test_stress_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PyPlanPro/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PyPlanPro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/PyPlanPro/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/heuristic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/scheduler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/PyPlanPro/scheduler/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/pyplanpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 09:41:01.000000 pyplanpro-0.0.6/pyplanpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:41:01.595040 pyplanpro-0.0.6/tests/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/scheduler/test_heuristic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:40:49.000000 pyplanpro-0.0.6/tests/scheduler/test_scheduler.py
```

### Comparing `pyplanpro-0.0.5/LICENSE` & `pyplanpro-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.5/PKG-INFO` & `pyplanpro-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.5
+Version: 0.0.6
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.5/PyPlanPro/models/resource.py` & `pyplanpro-0.0.6/PyPlanPro/models/resource.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.5/PyPlanPro/models/resource_group.py` & `pyplanpro-0.0.6/PyPlanPro/models/resource_group.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.5/PyPlanPro/models/task.py` & `pyplanpro-0.0.6/PyPlanPro/models/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @dataclass
 class Task:
     id: int
     duration: int
     priority: int
     resource_group: ResourceGroup
     predecessors: Optional[List['Task']] = field(default_factory=list)
+    predecessor_delay: int = 0
 
     def __eq__(self, other):
         if isinstance(other, Task):
             return self.id == other.id
         return NotImplemented
 
     def __hash__(self):
```

### Comparing `pyplanpro-0.0.5/PyPlanPro/scheduler/heuristic_solver.py` & `pyplanpro-0.0.6/PyPlanPro/scheduler/heuristic_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         task_dict = {task.id: task for task in self.tasks}
         task_vars = {task.id: {} for task in self.tasks}
         resource_interval_trees = self._get_resource_interval_trees(self.resources)
 
         unscheduled_tasks = []
         for i, task_id in enumerate(task_ids_ordered):
             task = task_dict[task_id]
-            # get max_start_time from max predecessors end
-            max_start_time = max((task_vars[pred.id].get('task_end',0) for pred in task.predecessors), default=0)
-            
+            # get earliest start from max predecessors end
+            task_earliest_start = self._get_task_earliest_start(task_vars, task)
+
             # find the resource who completes the task first
-            fastest_resource = self._get_fastest_resource(task,resource_interval_trees, max_start_time)
+            fastest_resource = self._get_fastest_resource(task,resource_interval_trees, task_earliest_start)
             if fastest_resource is None:
                 unscheduled_tasks.append(task.id)
                 self._update_task_vars_unscheduled(task_vars, task)
                 continue
 
             self._update_task_vars_scheduled(task_vars, task, fastest_resource)
 
@@ -54,14 +54,18 @@
             "assigned_resource_id": fastest_resource["resource"].id,
             "task_start": fastest_resource["task_start"],
             "task_end": fastest_resource["task_end"],
             "task_intervals": [(interval.begin, interval.end) for interval in sorted(fastest_resource["task_interval_tree"])]
         }
         task_vars[task.id] = task_values
 
+    def _get_task_earliest_start(self, task_vars, task):
+        predecessor_max_end = max((task_vars[pred.id].get('task_end',0) for pred in task.predecessors), default=0)
+        return predecessor_max_end + task.predecessor_delay
+
     def _get_task_order(self, tasks):
         """
         Returns a list of task IDs in the order required to complete them as quickly as possible while considering task priorities.
 
         :param tasks: List of tasks with durations, predecessors, and priorities.
         :return: List of task IDs in the order required to complete them as quickly as possible while considering task priorities.
         """
```

### Comparing `pyplanpro-0.0.5/PyPlanPro/scheduler/optimizer.py` & `pyplanpro-0.0.6/PyPlanPro/scheduler/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.5/PyPlanPro/scheduler/scheduler_result.py` & `pyplanpro-0.0.6/PyPlanPro/scheduler/scheduler_result.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.5/README.md` & `pyplanpro-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.5/pyplanpro.egg-info/PKG-INFO` & `pyplanpro-0.0.6/pyplanpro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.5
+Version: 0.0.6
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.5/pyplanpro.egg-info/SOURCES.txt` & `pyplanpro-0.0.6/pyplanpro.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -16,10 +16,8 @@
 pyplanpro.egg-info/SOURCES.txt
 pyplanpro.egg-info/dependency_links.txt
 pyplanpro.egg-info/requires.txt
 pyplanpro.egg-info/top_level.txt
 tests/__init__.py
 tests/scheduler/__init__.py
 tests/scheduler/test_heuristic_solver.py
-tests/scheduler/test_scheduler.py
-tests/stress/__init__.py
-tests/stress/test_stress_scheduler.py
+tests/scheduler/test_scheduler.py
```

### Comparing `pyplanpro-0.0.5/setup.py` & `pyplanpro-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 setup(
     name='pyplanpro',
-    version='0.0.5',
+    version='0.0.6',
     author='Jacob Østergaard Nielsen',
     author_email='jaoe@oestergaard-as.dk',
     description='Task scheduler for python',
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     url='https://github.com/Oestergaard-A-S/PyPlanPro',
     install_requires= read_requirements("requirements.txt"),
```

### Comparing `pyplanpro-0.0.5/tests/scheduler/test_heuristic_solver.py` & `pyplanpro-0.0.6/tests/scheduler/test_heuristic_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pyplanpro import Resource, Task, ResourceGroup
-from pyplanpro.scheduler.heuristic_solver import HeuristicSolver
+from PyPlanPro import Resource, Task, ResourceGroup
+from PyPlanPro.scheduler.heuristic_solver import HeuristicSolver
 from intervaltree import IntervalTree, Interval
 import pytest
 import copy
 
 # Sample data for testing
 resources = [
     Resource(id=0, availability_slots=[(0,10),(20,30)]),
     Resource(id=1, availability_slots=[(2,10), (12,20)])
 ]
 
 rg = ResourceGroup(id=1, resources=resources)
 tasks = [
     Task(id=0, duration=10, priority=1, resource_group=rg),
-    Task(id=1, duration=5, priority=2, resource_group=rg),
+    Task(id=1, duration=5, priority=2, resource_group=rg, predecessor_delay=5),
     Task(id=2, duration=10, priority=2, resource_group=rg),
     Task(id=3, duration=5, priority=3, resource_group=rg),
     Task(id=4, duration=1, priority=4, resource_group=rg)
 ]
 tasks[0].predecessors = [tasks[3]]
 tasks[1].predecessors = [tasks[4]]
 tasks[2].predecessors = [tasks[4]]
@@ -66,8 +66,8 @@
     rits, resource_id, interval_tree_index, task_start, task_end)
 
     assert rits[resource_id] != rits_old[resource_id] ,"Updated does not equal original"
     assert len(rits[resource_id]) == (len(rits_old[resource_id]) + 1), "Update adds 1 more slot"
     # check no other resource intervals are modified
     del rits_old[resource_id]
     del rits[resource_id]
-    assert rits == rits_old, "Are identical if change is deleted"
+    assert rits == rits_old, "Are identical if change is deleted"
```


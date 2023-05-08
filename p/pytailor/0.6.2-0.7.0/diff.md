# Comparing `tmp/pytailor-0.6.2.tar.gz` & `tmp/pytailor-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytailor-0.6.2.tar", max compression
+gzip compressed data, was "pytailor-0.7.0.tar", max compression
```

## Comparing `pytailor-0.6.2.tar` & `pytailor-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1517 2023-05-01 17:52:28.244821 pytailor-0.6.2/LICENSE
--rw-r--r--   0        0        0      884 2023-05-01 17:52:28.252822 pytailor-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       68 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/__init__.py
--rw-r--r--   0        0        0      314 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/__init__.py
--rw-r--r--   0        0        0     1000 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/account.py
--rw-r--r--   0        0        0      104 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/base.py
--rw-r--r--   0        0        0    22572 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/dag.py
--rw-r--r--   0        0        0     2688 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/fileset.py
--rw-r--r--   0        0        0      844 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/local_files.py
--rw-r--r--   0        0        0     4260 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/parameterization.py
--rw-r--r--   0        0        0     3182 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/project.py
--rw-r--r--   0        0        0      173 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/__init__.py
--rw-r--r--   0        0        0     5744 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/description.py
--rw-r--r--   0        0        0     6199 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/files_schema.py
--rw-r--r--   0        0        0     6976 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/inputs_schema.py
--rw-r--r--   0        0        0        0 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/strategies/__init__.py
--rw-r--r--   0        0        0     1080 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/strategies/additionalProperties.py
--rw-r--r--   0        0        0      427 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/strategies/tailorschemabuilder.py
--rw-r--r--   0        0        0    10825 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/workflow.py
--rw-r--r--   0        0        0     5221 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/workflow_definition.py
--rw-r--r--   0        0        0        0 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/cli/__init__.py
--rw-r--r--   0        0        0     3585 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/cli/main.py
--rw-r--r--   0        0        0      119 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/__init__.py
--rw-r--r--   0        0        0     4141 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/async_rest_client.py
--rw-r--r--   0        0        0     4303 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/auth.py
--rw-r--r--   0        0        0     3025 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/file_client.py
--rw-r--r--   0        0        0     3812 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/handling.py
--rw-r--r--   0        0        0    10560 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/rest_client.py
--rw-r--r--   0        0        0     1971 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/config.py
--rw-r--r--   0        0        0      371 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/exceptions.py
--rw-r--r--   0        0        0       74 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/__init__.py
--rw-r--r--   0        0        0     1398 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/serialrunner.py
--rw-r--r--   0        0        0    18262 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/taskrunner.py
--rw-r--r--   0        0        0     3631 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/worker.py
--rw-r--r--   0        0        0     3503 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/worker_checks.py
--rw-r--r--   0        0        0    19407 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/models.py
--rw-r--r--   0        0        0     7873 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/utils.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 pytailor-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-05-08 07:32:22.416754 pytailor-0.7.0/LICENSE
+-rw-r--r--   0        0        0      884 2023-05-08 07:32:22.428753 pytailor-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/__init__.py
+-rw-r--r--   0        0        0     1000 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/account.py
+-rw-r--r--   0        0        0      104 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/base.py
+-rw-r--r--   0        0        0    22572 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/dag.py
+-rw-r--r--   0        0        0     2688 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/fileset.py
+-rw-r--r--   0        0        0      844 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/local_files.py
+-rw-r--r--   0        0        0     4260 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/parameterization.py
+-rw-r--r--   0        0        0     3182 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/project.py
+-rw-r--r--   0        0        0      173 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/schema/__init__.py
+-rw-r--r--   0        0        0     5744 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/schema/description.py
+-rw-r--r--   0        0        0     6199 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/schema/files_schema.py
+-rw-r--r--   0        0        0     6976 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/schema/inputs_schema.py
+-rw-r--r--   0        0        0        0 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/schema/strategies/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/schema/strategies/additionalProperties.py
+-rw-r--r--   0        0        0      427 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/schema/strategies/tailorschemabuilder.py
+-rw-r--r--   0        0        0    10825 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/workflow.py
+-rw-r--r--   0        0        0     5221 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/api/workflow_definition.py
+-rw-r--r--   0        0        0        0 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/cli/__init__.py
+-rw-r--r--   0        0        0     3585 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/cli/main.py
+-rw-r--r--   0        0        0      119 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/clients/__init__.py
+-rw-r--r--   0        0        0     4141 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/clients/async_rest_client.py
+-rw-r--r--   0        0        0     4303 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/clients/auth.py
+-rw-r--r--   0        0        0     3025 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/clients/file_client.py
+-rw-r--r--   0        0        0     3812 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/clients/handling.py
+-rw-r--r--   0        0        0    10560 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/clients/rest_client.py
+-rw-r--r--   0        0        0     1971 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/config.py
+-rw-r--r--   0        0        0      371 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/exceptions.py
+-rw-r--r--   0        0        0       74 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/execution/__init__.py
+-rw-r--r--   0        0        0     1398 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/execution/serialrunner.py
+-rw-r--r--   0        0        0    18316 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/execution/taskrunner.py
+-rw-r--r--   0        0        0     3631 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/execution/worker.py
+-rw-r--r--   0        0        0     3503 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/execution/worker_checks.py
+-rw-r--r--   0        0        0    19407 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/models.py
+-rw-r--r--   0        0        0     7873 2023-05-08 07:32:22.428753 pytailor-0.7.0/src/pytailor/utils.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 pytailor-0.7.0/PKG-INFO
```

### Comparing `pytailor-0.6.2/LICENSE` & `pytailor-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/pyproject.toml` & `pytailor-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytailor"
-version = "0.6.2"
+version = "0.7.0"
 description = "pyTailor orchestrates your existing python code as *workflows*"
 authors = ["Audun Gravdal Johansen <audun@entail.no>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/entailor/pytailor/"
 include = [
     "LICENSE",
 ]
```

### Comparing `pytailor-0.6.2/src/pytailor/api/account.py` & `pytailor-0.7.0/src/pytailor/api/account.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/dag.py` & `pytailor-0.7.0/src/pytailor/api/dag.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/fileset.py` & `pytailor-0.7.0/src/pytailor/api/fileset.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/local_files.py` & `pytailor-0.7.0/src/pytailor/api/local_files.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/parameterization.py` & `pytailor-0.7.0/src/pytailor/api/parameterization.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/project.py` & `pytailor-0.7.0/src/pytailor/api/project.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/schema/description.py` & `pytailor-0.7.0/src/pytailor/api/schema/description.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/schema/files_schema.py` & `pytailor-0.7.0/src/pytailor/api/schema/files_schema.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/schema/inputs_schema.py` & `pytailor-0.7.0/src/pytailor/api/schema/inputs_schema.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/schema/strategies/additionalProperties.py` & `pytailor-0.7.0/src/pytailor/api/schema/strategies/additionalProperties.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/workflow.py` & `pytailor-0.7.0/src/pytailor/api/workflow.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/api/workflow_definition.py` & `pytailor-0.7.0/src/pytailor/api/workflow_definition.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/cli/main.py` & `pytailor-0.7.0/src/pytailor/cli/main.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/clients/async_rest_client.py` & `pytailor-0.7.0/src/pytailor/clients/async_rest_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/clients/auth.py` & `pytailor-0.7.0/src/pytailor/clients/auth.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/clients/file_client.py` & `pytailor-0.7.0/src/pytailor/clients/file_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/clients/handling.py` & `pytailor-0.7.0/src/pytailor/clients/handling.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/clients/rest_client.py` & `pytailor-0.7.0/src/pytailor/clients/rest_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/config.py` & `pytailor-0.7.0/src/pytailor/config.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/execution/serialrunner.py` & `pytailor-0.7.0/src/pytailor/execution/serialrunner.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/execution/taskrunner.py` & `pytailor-0.7.0/src/pytailor/execution/taskrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         elif TaskType(task_def["type"]) == TaskType.BRANCH:
             self.__run_branch_task()
 
     def __run_python_task(self, task_def):
         # check in state RUNNING, and get exec data
         task_update = TaskUpdate(task_id=self.__task_id, state=self.state, run_dir=str(self.run_dir))
         with RestClient() as client:
-            exec_data = client.checkin_task(task_update)
+            exec_data = client.checkin_task(task_update, wait=True)
         self.__update_exec_data(exec_data)
 
         self.__maybe_download_files(task_def)
         parsed_args = self.__determine_args(task_def)
         parsed_kwargs = self.__determine_kwargs(task_def)
         function_output = self.__run_function(task_def, parsed_args, parsed_kwargs)
         self.__store_output(task_def, function_output)
@@ -210,19 +210,20 @@
                 elif isinstance(v, dict):
                     outputs[k] = walk_and_apply(
                         v,
                         val_cond=as_query,
                         val_apply=lambda x: self.__eval_query(as_query(x), function_output),
                     )
 
-        # check in updated outputs
-        task_update = TaskUpdate(run_id=self.__run_id, task_id=self.__task_id, outputs=outputs)
-        with RestClient() as client:
-            exec_data = client.checkin_task(task_update)
-        self.__update_exec_data(exec_data)
+        # check in updated outputs if any
+        if outputs:
+            task_update = TaskUpdate(run_id=self.__run_id, task_id=self.__task_id, outputs=outputs)
+            with RestClient() as client:
+                exec_data = client.checkin_task(task_update)
+            self.__update_exec_data(exec_data)
 
     def __run_function(self, task_def, args, kwargs):
 
         # DONT do this:
         # sys.path.append('.')
         # this has the effect that python modules that have been downloaded are
         # discovered this is potentially risky as users can execute arbitrary code by
```

### Comparing `pytailor-0.6.2/src/pytailor/execution/worker.py` & `pytailor-0.7.0/src/pytailor/execution/worker.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/execution/worker_checks.py` & `pytailor-0.7.0/src/pytailor/execution/worker_checks.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/models.py` & `pytailor-0.7.0/src/pytailor/models.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/src/pytailor/utils.py` & `pytailor-0.7.0/src/pytailor/utils.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.2/PKG-INFO` & `pytailor-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytailor
-Version: 0.6.2
+Version: 0.7.0
 Summary: pyTailor orchestrates your existing python code as *workflows*
 Home-page: https://github.com/entailor/pytailor/
 License: BSD-3-Clause
 Author: Audun Gravdal Johansen
 Author-email: audun@entail.no
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
```


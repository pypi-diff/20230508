# Comparing `tmp/exe_kg_lib-2.0.3.tar.gz` & `tmp/exe_kg_lib-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exe_kg_lib-2.0.3.tar", max compression
+gzip compressed data, was "exe_kg_lib-2.0.4.tar", max compression
```

## Comparing `exe_kg_lib-2.0.3.tar` & `exe_kg_lib-2.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34283 2023-04-28 16:15:11.562069 exe_kg_lib-2.0.3/LICENSE.md
--rw-r--r--   0        0        0    15731 2023-04-28 16:15:11.562069 exe_kg_lib-2.0.3/README.md
--rw-r--r--   0        0        0       27 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/__init__.py
--rw-r--r--   0        0        0      102 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/__init__.py
--rw-r--r--   0        0        0     1253 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/data_entity.py
--rw-r--r--   0        0        0      788 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/entity.py
--rw-r--r--   0        0        0    31697 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/exe_kg.py
--rw-r--r--   0        0        0      773 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/kg_schema.py
--rw-r--r--   0        0        0     3528 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/task.py
--rw-r--r--   0        0        0     1914 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/README.md
--rw-r--r--   0        0        0        0 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/__init__.py
--rw-r--r--   0        0        0     5619 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/ml_tasks.py
--rw-r--r--   0        0        0     1967 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/statistic_tasks.py
--rw-r--r--   0        0        0     3108 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/visual_tasks.py
--rw-r--r--   0        0        0        0 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/cli/__init__.py
--rw-r--r--   0        0        0      938 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/cli/main.py
--rw-r--r--   0        0        0      108 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/__init__.py
--rw-r--r--   0        0        0     3130 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/cli_utils.py
--rw-r--r--   0        0        0     7290 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/kg_creation_utils.py
--rw-r--r--   0        0        0     6250 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/query_utils.py
--rw-r--r--   0        0        0      679 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/string_utils.py
--rw-r--r--   0        0        0        0 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/__init__.py
--rw-r--r--   0        0        0     2660 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/ml_utils.py
--rw-r--r--   0        0        0     2606 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/statistic_utils.py
--rw-r--r--   0        0        0     2388 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/visual_utils.py
--rw-r--r--   0        0        0     3645 2023-04-28 16:15:36.235572 exe_kg_lib-2.0.3/pyproject.toml
--rw-r--r--   0        0        0    17179 1970-01-01 00:00:00.000000 exe_kg_lib-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34283 2023-05-08 15:34:05.255395 exe_kg_lib-2.0.4/LICENSE.md
+-rw-r--r--   0        0        0    15902 2023-05-08 15:34:05.255395 exe_kg_lib-2.0.4/README.md
+-rw-r--r--   0        0        0       27 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/__init__.py
+-rw-r--r--   0        0        0     1253 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/data_entity.py
+-rw-r--r--   0        0        0      788 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/entity.py
+-rw-r--r--   0        0        0    31697 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/exe_kg.py
+-rw-r--r--   0        0        0      773 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/kg_schema.py
+-rw-r--r--   0        0        0     3528 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/task.py
+-rw-r--r--   0        0        0     1914 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/__init__.py
+-rw-r--r--   0        0        0     5619 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/ml_tasks.py
+-rw-r--r--   0        0        0     1967 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/statistic_tasks.py
+-rw-r--r--   0        0        0     3108 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/visual_tasks.py
+-rw-r--r--   0        0        0        0 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/cli/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/cli/main.py
+-rw-r--r--   0        0        0      108 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/__init__.py
+-rw-r--r--   0        0        0     3130 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/cli_utils.py
+-rw-r--r--   0        0        0     7290 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/kg_creation_utils.py
+-rw-r--r--   0        0        0     6250 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/query_utils.py
+-rw-r--r--   0        0        0      679 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/string_utils.py
+-rw-r--r--   0        0        0        0 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/__init__.py
+-rw-r--r--   0        0        0     2660 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/ml_utils.py
+-rw-r--r--   0        0        0     2606 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/statistic_utils.py
+-rw-r--r--   0        0        0     2388 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/visual_utils.py
+-rw-r--r--   0        0        0     3645 2023-05-08 15:34:28.212725 exe_kg_lib-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0    17350 1970-01-01 00:00:00.000000 exe_kg_lib-2.0.4/PKG-INFO
```

### Comparing `exe_kg_lib-2.0.3/LICENSE.md` & `exe_kg_lib-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/README.md` & `exe_kg_lib-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
 [//]: # (--8<-- [start:usage])
 ### Creating an ML pipeline
 
 - **Via code**: See the [provided examples](https://github.com/boschresearch/ExeKGLib/tree/main/examples). To fetch them to your working directory for easy access, run `typer exe_kg_lib.cli.main run get-examples`.
 - **Step-by-step via CLI**: Run `typer exe_kg_lib.cli.main run create-pipeline`.
 
 ### Executing an ML pipeline
-Run `typer exe_kg_lib.cli.main run run-pipeline <pipeline_path>`.
+- **Via code**: See [example code](https://github.com/boschresearch/ExeKGLib/blob/21e4df0e7de89c27748c8b61759652b7edf7d9b8/exe_kg_lib/cli/main.py#L28-L29).
+- **Via CLI**: Run `typer exe_kg_lib.cli.main run run-pipeline <pipeline_path>`.
 
 [//]: # (--8<-- [end:usage])
 
 ## Adding a new ML-related task and method
 
 [//]: # (--8<-- [start:extending])
 To perform this type of **ExeKGLib** extension, there are 3 required steps:
```

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/data_entity.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/data_entity.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/entity.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/entity.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/exe_kg.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/exe_kg.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/kg_schema.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/kg_schema.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/task.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/task.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/README.md` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/README.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/ml_tasks.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/ml_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/statistic_tasks.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/statistic_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/visual_tasks.py` & `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/visual_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/cli/main.py` & `exe_kg_lib-2.0.4/exe_kg_lib/cli/main.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/utils/cli_utils.py` & `exe_kg_lib-2.0.4/exe_kg_lib/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/utils/kg_creation_utils.py` & `exe_kg_lib-2.0.4/exe_kg_lib/utils/kg_creation_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/utils/query_utils.py` & `exe_kg_lib-2.0.4/exe_kg_lib/utils/query_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/utils/string_utils.py` & `exe_kg_lib-2.0.4/exe_kg_lib/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/ml_utils.py` & `exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/ml_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/statistic_utils.py` & `exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/statistic_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/visual_utils.py` & `exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/visual_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.3/pyproject.toml` & `exe_kg_lib-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exe-kg-lib"
-version = "2.0.3" # not used when bumping version via poe bump-version-tag or cd.yaml
+version = "2.0.4" # not used when bumping version via poe bump-version-tag or cd.yaml
 description = "Library for executable ML pipelines represented by KGs."
 license = "AGPL-3.0"
 authors = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
 
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Developers",
```

### Comparing `exe_kg_lib-2.0.3/PKG-INFO` & `exe_kg_lib-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exe-kg-lib
-Version: 2.0.3
+Version: 2.0.4
 Summary: Library for executable ML pipelines represented by KGs.
 Home-page: https://boschresearch.github.io/ExeKGLib
 License: AGPL-3.0
 Author: Antonis Klironomos
 Author-email: antonis.klironomos@de.bosch.com
 Maintainer: Antonis Klironomos
 Maintainer-email: antonis.klironomos@de.bosch.com
@@ -105,15 +105,16 @@
 [//]: # (--8<-- [start:usage])
 ### Creating an ML pipeline
 
 - **Via code**: See the [provided examples](https://github.com/boschresearch/ExeKGLib/tree/main/examples). To fetch them to your working directory for easy access, run `typer exe_kg_lib.cli.main run get-examples`.
 - **Step-by-step via CLI**: Run `typer exe_kg_lib.cli.main run create-pipeline`.
 
 ### Executing an ML pipeline
-Run `typer exe_kg_lib.cli.main run run-pipeline <pipeline_path>`.
+- **Via code**: See [example code](https://github.com/boschresearch/ExeKGLib/blob/21e4df0e7de89c27748c8b61759652b7edf7d9b8/exe_kg_lib/cli/main.py#L28-L29).
+- **Via CLI**: Run `typer exe_kg_lib.cli.main run run-pipeline <pipeline_path>`.
 
 [//]: # (--8<-- [end:usage])
 
 ## Adding a new ML-related task and method
 
 [//]: # (--8<-- [start:extending])
 To perform this type of **ExeKGLib** extension, there are 3 required steps:
```


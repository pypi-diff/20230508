# Comparing `tmp/sidetrek-0.0.8.tar.gz` & `tmp/sidetrek-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.8.tar", max compression
+gzip compressed data, was "sidetrek-0.0.9.tar", max compression
```

## Comparing `sidetrek-0.0.8.tar` & `sidetrek-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.8/README.md
--rw-r--r--   0        0        0      689 2023-04-08 23:52:13.993874 sidetrek-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      558 2023-04-08 23:51:45.364985 sidetrek-0.0.8/sidetrek/__init__.py
--rw-r--r--   0        0        0     1607 2023-03-30 15:37:18.710028 sidetrek-0.0.8/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.8/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.8/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      388 2023-03-30 16:36:26.685225 sidetrek-0.0.8/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     8815 2023-04-06 20:18:36.881239 sidetrek-0.0.8/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     2395 2023-04-06 20:18:55.453228 sidetrek-0.0.8/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      244 2023-03-30 16:14:08.795493 sidetrek-0.0.8/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0     9970 2023-04-06 20:18:33.249911 sidetrek-0.0.8/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     3115 2023-04-06 20:19:34.857751 sidetrek-0.0.8/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.8/sidetrek/core/constants.py
--rw-r--r--   0        0        0      491 2023-04-08 23:51:25.980013 sidetrek-0.0.8/sidetrek/core/global_fns.py
--rw-r--r--   0        0        0      661 2023-03-16 01:49:43.511125 sidetrek-0.0.8/sidetrek/loggers/loggers.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 sidetrek-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.9/README.md
+-rw-r--r--   0        0        0      689 2023-04-09 00:09:19.420892 sidetrek-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      558 2023-04-08 23:51:45.364985 sidetrek-0.0.9/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1607 2023-03-30 15:37:18.710028 sidetrek-0.0.9/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.9/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      388 2023-03-30 16:36:26.685225 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     8815 2023-04-06 20:18:36.881239 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     2395 2023-04-06 20:18:55.453228 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      244 2023-03-30 16:14:08.795493 sidetrek-0.0.9/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0     9970 2023-04-06 20:18:33.249911 sidetrek-0.0.9/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     3115 2023-04-06 20:19:34.857751 sidetrek-0.0.9/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:08:56.569055 sidetrek-0.0.9/sidetrek/core/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.9/sidetrek/core/constants.py
+-rw-r--r--   0        0        0      491 2023-04-08 23:51:25.980013 sidetrek-0.0.9/sidetrek/core/global_fns.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:09:01.575253 sidetrek-0.0.9/sidetrek/loggers/__init__.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.9/sidetrek/loggers/loggers.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 sidetrek-0.0.9/PKG-INFO
```

### Comparing `sidetrek-0.0.8/pyproject.toml` & `sidetrek-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
```

### Comparing `sidetrek-0.0.8/sidetrek/__init__.py` & `sidetrek-0.0.9/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.8/sidetrek/cli.py` & `sidetrek-0.0.9/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.8/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.8/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.8/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.9/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.8/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.9/sidetrek/cli_commands/workflow.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.8/sidetrek/loggers/loggers.py` & `sidetrek-0.0.9/sidetrek/loggers/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.8/PKG-INFO` & `sidetrek-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: flytekit (<=1.4.2)
```


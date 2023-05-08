# Comparing `tmp/sag-py-execution-time-decorator-0.1.0.tar.gz` & `tmp/sag-py-execution-time-decorator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-execution-time-decorator-0.1.0.tar", last modified: Mon May  8 10:57:00 2023, max compression
+gzip compressed data, was "sag-py-execution-time-decorator-1.0.0.tar", last modified: Mon May  8 11:20:01 2023, max compression
```

## Comparing `sag-py-execution-time-decorator-0.1.0.tar` & `sag-py-execution-time-decorator-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:57:00.501716 sag-py-execution-time-decorator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 10:57:00.501716 sag-py-execution-time-decorator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:57:00.501716 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator/execution_time_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:57:00.501716 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 10:57:00.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 10:57:00.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:57:00.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 10:57:00.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 10:57:00.000000 sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 10:57:00.501716 sag-py-execution-time-decorator-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:57:00.501716 sag-py-execution-time-decorator-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-08 10:56:49.000000 sag-py-execution-time-decorator-0.1.0/tests/test_execution_time_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/execution_time_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/tests/test_execution_time_decorator.py
```

### Comparing `sag-py-execution-time-decorator-0.1.0/LICENSE.txt` & `sag-py-execution-time-decorator-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-0.1.0/PKG-INFO` & `sag-py-execution-time-decorator-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-execution-time-decorator
-Version: 0.1.0
+Version: 1.0.0
 Summary: A decorator for methods to log the execution time (sync and async)
 Home-page: https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_execution_time_decorator/issues
@@ -85,13 +85,14 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
-[codeclimate-image]:https://api.codeclimate.com/v1/badges/98f082759f74f1d06159/maintainability
+
+[codeclimate-image]:https://api.codeclimate.com/v1/badges/fa4312e587c8185db077/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_execution_time_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_execution_time_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator
```

### Comparing `sag-py-execution-time-decorator-0.1.0/README.md` & `sag-py-execution-time-decorator-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -62,13 +62,14 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
-[codeclimate-image]:https://api.codeclimate.com/v1/badges/98f082759f74f1d06159/maintainability
+
+[codeclimate-image]:https://api.codeclimate.com/v1/badges/fa4312e587c8185db077/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_execution_time_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_execution_time_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator
```

### Comparing `sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator/execution_time_decorator.py` & `sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/execution_time_decorator.py`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/PKG-INFO` & `sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-execution-time-decorator
-Version: 0.1.0
+Version: 1.0.0
 Summary: A decorator for methods to log the execution time (sync and async)
 Home-page: https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_execution_time_decorator/issues
@@ -85,13 +85,14 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
-[codeclimate-image]:https://api.codeclimate.com/v1/badges/98f082759f74f1d06159/maintainability
+
+[codeclimate-image]:https://api.codeclimate.com/v1/badges/fa4312e587c8185db077/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_execution_time_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_execution_time_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator
```

### Comparing `sag-py-execution-time-decorator-0.1.0/sag_py_execution_time_decorator.egg-info/SOURCES.txt` & `sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-0.1.0/setup.py` & `sag-py-execution-time-decorator-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-execution-time-decorator",
-    version="0.1.0",
+    version="1.0.0",
     description="A decorator for methods to log the execution time (sync and async)",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_execution_time_decorator",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-execution-time-decorator-0.1.0/tests/test_execution_time_decorator.py` & `sag-py-execution-time-decorator-1.0.0/tests/test_execution_time_decorator.py`

 * *Files identical despite different names*


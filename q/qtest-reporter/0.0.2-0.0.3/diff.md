# Comparing `tmp/qtest_reporter-0.0.2.tar.gz` & `tmp/qtest_reporter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtest_reporter-0.0.2.tar", last modified: Mon May  8 10:04:25 2023, max compression
+gzip compressed data, was "qtest_reporter-0.0.3.tar", last modified: Mon May  8 11:19:04 2023, max compression
```

## Comparing `qtest_reporter-0.0.2.tar` & `qtest_reporter-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 10:04:25.176017 qtest_reporter-0.0.2/
--rw-r--r--   0 vzyhmund   (501) staff       (20)    35148 2023-05-04 16:40:04.000000 qtest_reporter-0.0.2/LICENSE
--rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 10:04:25.175869 qtest_reporter-0.0.2/PKG-INFO
--rw-r--r--   0 vzyhmund   (501) staff       (20)      148 2023-05-08 08:28:42.000000 qtest_reporter-0.0.2/README.md
--rw-r--r--   0 vzyhmund   (501) staff       (20)      727 2023-05-08 10:03:54.000000 qtest_reporter-0.0.2/pyproject.toml
--rw-r--r--   0 vzyhmund   (501) staff       (20)       38 2023-05-08 10:04:25.176067 qtest_reporter-0.0.2/setup.cfg
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 10:04:25.169498 qtest_reporter-0.0.2/src/
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 10:04:25.172122 qtest_reporter-0.0.2/src/qtest_reporter/
--rw-r--r--   0 vzyhmund   (501) staff       (20)       97 2023-05-08 10:04:07.000000 qtest_reporter-0.0.2/src/qtest_reporter/__init__.py
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 10:04:25.175633 qtest_reporter-0.0.2/src/qtest_reporter/api/
--rw-r--r--   0 vzyhmund   (501) staff       (20)     1654 2023-05-08 10:01:34.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/login.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     3148 2023-05-08 10:01:45.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/project.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    12270 2023-05-08 10:01:53.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/test_case.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    11536 2023-05-08 10:02:05.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/test_cycle.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     9731 2023-05-08 10:02:55.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/test_log.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    12800 2023-05-08 10:03:13.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/test_run.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    11629 2023-05-08 10:03:25.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/test_suite.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     1475 2023-05-08 10:03:35.000000 qtest_reporter-0.0.2/src/qtest_reporter/api/user_profile.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      337 2023-05-04 16:26:28.000000 qtest_reporter-0.0.2/src/qtest_reporter/logger.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      376 2023-05-08 09:58:32.000000 qtest_reporter-0.0.2/src/qtest_reporter/qtest.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      421 2023-04-25 12:22:26.000000 qtest_reporter-0.0.2/src/qtest_reporter/requester.py
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 10:04:25.173138 qtest_reporter-0.0.2/src/qtest_reporter.egg-info/
--rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 10:04:25.000000 qtest_reporter-0.0.2/src/qtest_reporter.egg-info/PKG-INFO
--rw-r--r--   0 vzyhmund   (501) staff       (20)      605 2023-05-08 10:04:25.000000 qtest_reporter-0.0.2/src/qtest_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 vzyhmund   (501) staff       (20)        1 2023-05-08 10:04:25.000000 qtest_reporter-0.0.2/src/qtest_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 vzyhmund   (501) staff       (20)       15 2023-05-08 10:04:25.000000 qtest_reporter-0.0.2/src/qtest_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 11:19:04.316051 qtest_reporter-0.0.3/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    35148 2023-05-04 16:40:04.000000 qtest_reporter-0.0.3/LICENSE
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 11:19:04.315882 qtest_reporter-0.0.3/PKG-INFO
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      148 2023-05-08 08:28:42.000000 qtest_reporter-0.0.3/README.md
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      727 2023-05-08 10:13:21.000000 qtest_reporter-0.0.3/pyproject.toml
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       38 2023-05-08 11:19:04.316108 qtest_reporter-0.0.3/setup.cfg
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 11:19:04.309352 qtest_reporter-0.0.3/src/
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 11:19:04.311807 qtest_reporter-0.0.3/src/qtest_reporter/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       97 2023-05-08 10:29:29.000000 qtest_reporter-0.0.3/src/qtest_reporter/__init__.py
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 11:19:04.315530 qtest_reporter-0.0.3/src/qtest_reporter/api/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)        0 2023-05-08 11:17:55.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/__init__.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     1653 2023-05-08 11:17:29.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/login.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     3147 2023-05-08 11:17:20.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/project.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    12269 2023-05-08 11:17:12.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/test_case.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    11534 2023-05-08 11:17:00.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/test_cycle.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     9727 2023-05-08 11:16:44.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/test_log.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    12796 2023-05-08 10:54:07.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/test_run.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    11626 2023-05-08 10:54:18.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/test_suite.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     1474 2023-05-08 10:52:36.000000 qtest_reporter-0.0.3/src/qtest_reporter/api/user_profile.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      337 2023-05-04 16:26:28.000000 qtest_reporter-0.0.3/src/qtest_reporter/logger.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      375 2023-05-08 10:51:37.000000 qtest_reporter-0.0.3/src/qtest_reporter/qtest.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      421 2023-04-25 12:22:26.000000 qtest_reporter-0.0.3/src/qtest_reporter/requester.py
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 11:19:04.312726 qtest_reporter-0.0.3/src/qtest_reporter.egg-info/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 11:19:04.000000 qtest_reporter-0.0.3/src/qtest_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      640 2023-05-08 11:19:04.000000 qtest_reporter-0.0.3/src/qtest_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)        1 2023-05-08 11:19:04.000000 qtest_reporter-0.0.3/src/qtest_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       15 2023-05-08 11:19:04.000000 qtest_reporter-0.0.3/src/qtest_reporter.egg-info/top_level.txt
```

### Comparing `qtest_reporter-0.0.2/LICENSE` & `qtest_reporter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.2/PKG-INFO` & `qtest_reporter-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtest_reporter
-Version: 0.0.2
+Version: 0.0.3
 Summary: qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool.
 Author-email: Volodymyr Zyhmund <volodymyr.romanovych@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `qtest_reporter-0.0.2/pyproject.toml` & `qtest_reporter-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qtest_reporter"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Volodymyr Zyhmund", email="volodymyr.romanovych@gmail.com" },
 ]
 description = "qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/login.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides a set of APIs to login into qTest"""
-from .requester import get, post
+from requester import get, post
 import base64
 
 
 class Login:
     """Login API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/project.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides a set of qTest user profile APIs"""
-from .requester import get
+from requester import get
 
 
 class Project:
     """Project API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
         self._token = qtest._token
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/test_case.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides a set of Test Case qTest APIs"""
-from .requester import get
+from requester import get
 
 
 class Test_Case:
     """Test Case API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
         self._token = qtest._token
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/test_cycle.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/test_cycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module provides a set of Test Cycle qTest APIs"""
-from .logger import Logger
-from .requester import get, post
+from logger import Logger
+from requester import get, post
 
 
 class Test_Cycle:
     """Test Cycle API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
         self._token = qtest._token
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/test_log.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module provides a set of Test Log qTest APIs"""
 from datetime import datetime
-from .api.test_case import Test_Case
-from .api.test_run import Test_Run
-from .logger import Logger
-from .requester import post
+from api.test_case import Test_Case
+from api.test_run import Test_Run
+from logger import Logger
+from requester import post
 
 
 class Test_Log:
     """Test Log API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
         self._token = qtest._token
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/test_run.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This module provides a set of Test Run qTest APIs"""
-from .api.test_case import Test_Case
-from .api.test_suite import Test_Suite
-from .logger import Logger
-from .requester import get, post
+from api.test_case import Test_Case
+from api.test_suite import Test_Suite
+from logger import Logger
+from requester import get, post
 
 
 class Test_Run:
     """Test Run API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
         self._token = qtest._token
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/test_suite.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/test_suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module provides a set of Test Suite qTest APIs"""
-from .api.test_cycle import Test_Cycle
-from .logger import Logger
-from .requester import get, post
+from api.test_cycle import Test_Cycle
+from logger import Logger
+from requester import get, post
 
 
 class Test_Suite:
     """Test Suite API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
         self._token = qtest._token
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter/api/user_profile.py` & `qtest_reporter-0.0.3/src/qtest_reporter/api/user_profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module provides a set of qTest user profile APIs"""
-from .requester import get
+from requester import get
 
 
 class User_Profile:
     """User Profile API"""
     def __init__(self, qtest: object):
         self._host = qtest._host
         self._username = qtest._username
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter.egg-info/PKG-INFO` & `qtest_reporter-0.0.3/src/qtest_reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtest-reporter
-Version: 0.0.2
+Version: 0.0.3
 Summary: qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool.
 Author-email: Volodymyr Zyhmund <volodymyr.romanovych@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `qtest_reporter-0.0.2/src/qtest_reporter.egg-info/SOURCES.txt` & `qtest_reporter-0.0.3/src/qtest_reporter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/qtest_reporter/logger.py
 src/qtest_reporter/qtest.py
 src/qtest_reporter/requester.py
 src/qtest_reporter.egg-info/PKG-INFO
 src/qtest_reporter.egg-info/SOURCES.txt
 src/qtest_reporter.egg-info/dependency_links.txt
 src/qtest_reporter.egg-info/top_level.txt
+src/qtest_reporter/api/__init__.py
 src/qtest_reporter/api/login.py
 src/qtest_reporter/api/project.py
 src/qtest_reporter/api/test_case.py
 src/qtest_reporter/api/test_cycle.py
 src/qtest_reporter/api/test_log.py
 src/qtest_reporter/api/test_run.py
 src/qtest_reporter/api/test_suite.py
```


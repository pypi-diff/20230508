# Comparing `tmp/qtest_reporter-0.0.4.tar.gz` & `tmp/qtest_reporter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtest_reporter-0.0.4.tar", last modified: Mon May  8 12:31:23 2023, max compression
+gzip compressed data, was "qtest_reporter-0.0.5.tar", last modified: Mon May  8 13:30:06 2023, max compression
```

## Comparing `qtest_reporter-0.0.4.tar` & `qtest_reporter-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:31:23.907609 qtest_reporter-0.0.4/
--rw-r--r--   0 vzyhmund   (501) staff       (20)    35148 2023-05-04 16:40:04.000000 qtest_reporter-0.0.4/LICENSE
--rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 12:31:23.907427 qtest_reporter-0.0.4/PKG-INFO
--rw-r--r--   0 vzyhmund   (501) staff       (20)      148 2023-05-08 08:28:42.000000 qtest_reporter-0.0.4/README.md
--rw-r--r--   0 vzyhmund   (501) staff       (20)      727 2023-05-08 12:31:00.000000 qtest_reporter-0.0.4/pyproject.toml
--rw-r--r--   0 vzyhmund   (501) staff       (20)       38 2023-05-08 12:31:23.907674 qtest_reporter-0.0.4/setup.cfg
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:31:23.900337 qtest_reporter-0.0.4/src/
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:31:23.903216 qtest_reporter-0.0.4/src/qtest_reporter/
--rw-r--r--   0 vzyhmund   (501) staff       (20)       97 2023-05-08 12:30:54.000000 qtest_reporter-0.0.4/src/qtest_reporter/__init__.py
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:31:23.907053 qtest_reporter-0.0.4/src/qtest_reporter/api/
--rw-r--r--   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:24:57.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/__init__.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     1668 2023-05-08 12:28:27.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/login.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     3162 2023-05-08 12:28:35.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/project.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    12284 2023-05-08 12:28:40.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/test_case.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    11564 2023-05-08 12:28:52.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/test_cycle.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     9787 2023-05-08 12:29:06.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/test_log.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    12856 2023-05-08 12:29:32.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/test_run.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    11671 2023-05-08 12:29:41.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/test_suite.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     1489 2023-05-08 12:29:56.000000 qtest_reporter-0.0.4/src/qtest_reporter/api/user_profile.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      337 2023-05-04 16:26:28.000000 qtest_reporter-0.0.4/src/qtest_reporter/logger.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      376 2023-05-08 12:30:14.000000 qtest_reporter-0.0.4/src/qtest_reporter/qtest.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      421 2023-04-25 12:22:26.000000 qtest_reporter-0.0.4/src/qtest_reporter/requester.py
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:31:23.904197 qtest_reporter-0.0.4/src/qtest_reporter.egg-info/
--rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 12:31:23.000000 qtest_reporter-0.0.4/src/qtest_reporter.egg-info/PKG-INFO
--rw-r--r--   0 vzyhmund   (501) staff       (20)      640 2023-05-08 12:31:23.000000 qtest_reporter-0.0.4/src/qtest_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 vzyhmund   (501) staff       (20)        1 2023-05-08 12:31:23.000000 qtest_reporter-0.0.4/src/qtest_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 vzyhmund   (501) staff       (20)       15 2023-05-08 12:31:23.000000 qtest_reporter-0.0.4/src/qtest_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 13:30:06.792014 qtest_reporter-0.0.5/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    35148 2023-05-04 16:40:04.000000 qtest_reporter-0.0.5/LICENSE
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 13:30:06.791856 qtest_reporter-0.0.5/PKG-INFO
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      148 2023-05-08 08:28:42.000000 qtest_reporter-0.0.5/README.md
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      749 2023-05-08 13:29:38.000000 qtest_reporter-0.0.5/pyproject.toml
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       38 2023-05-08 13:30:06.792070 qtest_reporter-0.0.5/setup.cfg
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 13:30:06.784969 qtest_reporter-0.0.5/src/
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 13:30:06.787699 qtest_reporter-0.0.5/src/qtest_reporter/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       97 2023-05-08 13:29:45.000000 qtest_reporter-0.0.5/src/qtest_reporter/__init__.py
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 13:30:06.791548 qtest_reporter-0.0.5/src/qtest_reporter/api/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:24:57.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/__init__.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     1668 2023-05-08 12:28:27.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/login.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     3162 2023-05-08 12:28:35.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/project.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    12284 2023-05-08 12:28:40.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/test_case.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    11564 2023-05-08 12:28:52.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/test_cycle.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     9787 2023-05-08 12:29:06.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/test_log.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    12856 2023-05-08 12:29:32.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/test_run.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    11671 2023-05-08 12:29:41.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/test_suite.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     1489 2023-05-08 12:29:56.000000 qtest_reporter-0.0.5/src/qtest_reporter/api/user_profile.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      337 2023-05-04 16:26:28.000000 qtest_reporter-0.0.5/src/qtest_reporter/logger.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      376 2023-05-08 12:30:14.000000 qtest_reporter-0.0.5/src/qtest_reporter/qtest.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      421 2023-04-25 12:22:26.000000 qtest_reporter-0.0.5/src/qtest_reporter/requester.py
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-08 13:30:06.788825 qtest_reporter-0.0.5/src/qtest_reporter.egg-info/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-08 13:30:06.000000 qtest_reporter-0.0.5/src/qtest_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      681 2023-05-08 13:30:06.000000 qtest_reporter-0.0.5/src/qtest_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)        1 2023-05-08 13:30:06.000000 qtest_reporter-0.0.5/src/qtest_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)        9 2023-05-08 13:30:06.000000 qtest_reporter-0.0.5/src/qtest_reporter.egg-info/requires.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       15 2023-05-08 13:30:06.000000 qtest_reporter-0.0.5/src/qtest_reporter.egg-info/top_level.txt
```

### Comparing `qtest_reporter-0.0.4/LICENSE` & `qtest_reporter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/PKG-INFO` & `qtest_reporter-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtest_reporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool.
 Author-email: Volodymyr Zyhmund <volodymyr.romanovych@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `qtest_reporter-0.0.4/pyproject.toml` & `qtest_reporter-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "requests"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qtest_reporter"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Volodymyr Zyhmund", email="volodymyr.romanovych@gmail.com" },
 ]
 description = "qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -16,7 +16,10 @@
     "Intended Audience :: Developers",
     "License :: Freeware",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
     "Natural Language :: English",
     "Topic :: Software Development :: Testing",
 ]
+dependencies = [
+    "requests"
+]
```

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/login.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/login.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/project.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/project.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/test_case.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/test_case.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/test_cycle.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/test_cycle.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/test_log.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/test_log.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/test_run.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/test_run.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/test_suite.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/test_suite.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter/api/user_profile.py` & `qtest_reporter-0.0.5/src/qtest_reporter/api/user_profile.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter.egg-info/PKG-INFO` & `qtest_reporter-0.0.5/src/qtest_reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtest-reporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool.
 Author-email: Volodymyr Zyhmund <volodymyr.romanovych@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `qtest_reporter-0.0.4/src/qtest_reporter.egg-info/SOURCES.txt` & `qtest_reporter-0.0.5/src/qtest_reporter.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/qtest_reporter/__init__.py
 src/qtest_reporter/logger.py
 src/qtest_reporter/qtest.py
 src/qtest_reporter/requester.py
 src/qtest_reporter.egg-info/PKG-INFO
 src/qtest_reporter.egg-info/SOURCES.txt
 src/qtest_reporter.egg-info/dependency_links.txt
+src/qtest_reporter.egg-info/requires.txt
 src/qtest_reporter.egg-info/top_level.txt
 src/qtest_reporter/api/__init__.py
 src/qtest_reporter/api/login.py
 src/qtest_reporter/api/project.py
 src/qtest_reporter/api/test_case.py
 src/qtest_reporter/api/test_cycle.py
 src/qtest_reporter/api/test_log.py
```


# Comparing `tmp/robotframework-reportportal_updated-1.0.1.tar.gz` & `tmp/robotframework-reportportal_updated-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-reportportal_updated-1.0.1.tar", last modified: Mon May  8 07:03:54 2023, max compression
+gzip compressed data, was "robotframework-reportportal_updated-1.0.2.tar", last modified: Mon May  8 07:21:55 2023, max compression
```

## Comparing `robotframework-reportportal_updated-1.0.1.tar` & `robotframework-reportportal_updated-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:03:54.270840 robotframework-reportportal_updated-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-08 07:03:54.270840 robotframework-reportportal_updated-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:03:54.270840 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/listener.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/post_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/result_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/result_visitor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/static.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/time_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/variables.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:03:54.270840 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-08 07:03:54.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 07:03:54.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:03:54.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 07:03:54.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 07:03:54.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 07:03:54.000000 robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 07:03:54.270840 robotframework-reportportal_updated-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 07:03:49.000000 robotframework-reportportal_updated-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:21:55.955238 robotframework-reportportal_updated-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-08 07:21:55.955238 robotframework-reportportal_updated-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:21:55.955238 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/post_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/result_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/result_visitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/time_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/variables.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:21:55.955238 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-08 07:21:55.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 07:21:55.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:21:55.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 07:21:55.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 07:21:55.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 07:21:55.000000 robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 07:21:55.955238 robotframework-reportportal_updated-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 07:21:51.000000 robotframework-reportportal_updated-1.0.2/setup.py
```

### Comparing `robotframework-reportportal_updated-1.0.1/CONTRIBUTING.rst` & `robotframework-reportportal_updated-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/LICENSE.txt` & `robotframework-reportportal_updated-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/PKG-INFO` & `robotframework-reportportal_updated-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal_updated
-Version: 1.0.1
+Version: 1.0.2
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.0.1
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.0.2
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `robotframework-reportportal_updated-1.0.1/README.md` & `robotframework-reportportal_updated-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/__init__.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/exception.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/exception.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/listener.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/listener.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/listener.pyi` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/listener.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/logger.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/model.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/model.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/model.pyi` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/model.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/post_report.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/post_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/result_visitor.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/result_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/result_visitor.pyi` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/result_visitor.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/service.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/service.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/service.pyi` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/service.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/static.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/static.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/static.pyi` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/static.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/time_visitor.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/time_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/variables.py` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/variables.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated/variables.pyi` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated/variables.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/PKG-INFO` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal-updated
-Version: 1.0.1
+Version: 1.0.2
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.0.1
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.0.2
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `robotframework-reportportal_updated-1.0.1/robotframework_reportportal_updated.egg-info/SOURCES.txt` & `robotframework-reportportal_updated-1.0.2/robotframework_reportportal_updated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.0.1/setup.py` & `robotframework-reportportal_updated-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup instructions for the package."""
 
 import os
 from setuptools import setup, find_packages
 
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Name of the file to be read
     :return:      Output of the given file
```


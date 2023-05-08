# Comparing `tmp/renovosolutions.aws-cdk-one-time-event-2.1.98.tar.gz` & `tmp/renovosolutions.aws-cdk-one-time-event-2.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-one-time-event-2.1.98.tar", last modified: Mon Jan 30 13:54:13 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-one-time-event-2.1.99.tar", last modified: Wed Feb  1 13:35:45 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98.tar` & `renovosolutions.aws-cdk-one-time-event-2.1.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:54:13.369759 renovosolutions.aws-cdk-one-time-event-2.1.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-01-30 13:54:13.365759 renovosolutions.aws-cdk-one-time-event-2.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 13:54:13.369759 renovosolutions.aws-cdk-one-time-event-2.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:54:13.365759 renovosolutions.aws-cdk-one-time-event-2.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:54:13.365759 renovosolutions.aws-cdk-one-time-event-2.1.98/src/one_time_event/
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/one_time_event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:54:13.365759 renovosolutions.aws-cdk-one-time-event-2.1.98/src/one_time_event/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/one_time_event/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/one_time_event/_jsii/cdk-library-one-time-event@2.1.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 13:54:00.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/one_time_event/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:54:13.365759 renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-01-30 13:54:12.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-30 13:54:13.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 13:54:12.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-30 13:54:13.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-30 13:54:13.000000 renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:35:45.175474 renovosolutions.aws-cdk-one-time-event-2.1.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-02-01 13:35:45.175474 renovosolutions.aws-cdk-one-time-event-2.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 13:35:45.175474 renovosolutions.aws-cdk-one-time-event-2.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:35:45.175474 renovosolutions.aws-cdk-one-time-event-2.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:35:45.175474 renovosolutions.aws-cdk-one-time-event-2.1.99/src/one_time_event/
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/one_time_event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:35:45.175474 renovosolutions.aws-cdk-one-time-event-2.1.99/src/one_time_event/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/one_time_event/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/one_time_event/_jsii/cdk-library-one-time-event@2.1.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 13:35:30.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/one_time_event/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:35:45.175474 renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-02-01 13:35:44.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-01 13:35:45.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 13:35:44.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-01 13:35:45.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-01 13:35:45.000000 renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98/LICENSE` & `renovosolutions.aws-cdk-one-time-event-2.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98/PKG-INFO` & `renovosolutions.aws-cdk-one-time-event-2.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-one-time-event
-Version: 2.1.98
+Version: 2.1.99
 Summary: AWS CDK Construct Library to create one time event schedules.
 Home-page: https://github.com/RenovoSolutions/cdk-library-one-time-event.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-one-time-event.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98/README.md` & `renovosolutions.aws-cdk-one-time-event-2.1.99/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98/setup.py` & `renovosolutions.aws-cdk-one-time-event-2.1.99/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-one-time-event",
-    "version": "2.1.98",
+    "version": "2.1.99",
     "description": "AWS CDK Construct Library to create one time event schedules.",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-one-time-event.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "one_time_event",
         "one_time_event._jsii"
     ],
     "package_data": {
         "one_time_event._jsii": [
-            "cdk-library-one-time-event@2.1.98.jsii.tgz"
+            "cdk-library-one-time-event@2.1.99.jsii.tgz"
         ],
         "one_time_event": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.62.2, <3.0.0",
+        "aws-cdk-lib>=2.63.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.73.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98/src/one_time_event/__init__.py` & `renovosolutions.aws-cdk-one-time-event-2.1.99/src/one_time_event/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-one-time-event
-Version: 2.1.98
+Version: 2.1.99
 Summary: AWS CDK Construct Library to create one time event schedules.
 Home-page: https://github.com/RenovoSolutions/cdk-library-one-time-event.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-one-time-event.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-one-time-event-2.1.98/src/renovosolutions.aws_cdk_one_time_event.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-one-time-event-2.1.99/src/renovosolutions.aws_cdk_one_time_event.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/one_time_event/__init__.py
 src/one_time_event/py.typed
 src/one_time_event/_jsii/__init__.py
-src/one_time_event/_jsii/cdk-library-one-time-event@2.1.98.jsii.tgz
+src/one_time_event/_jsii/cdk-library-one-time-event@2.1.99.jsii.tgz
 src/renovosolutions.aws_cdk_one_time_event.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_one_time_event.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_one_time_event.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_one_time_event.egg-info/requires.txt
 src/renovosolutions.aws_cdk_one_time_event.egg-info/top_level.txt
```


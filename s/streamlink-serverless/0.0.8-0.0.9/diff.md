# Comparing `tmp/streamlink-serverless-0.0.8.tar.gz` & `tmp/streamlink-serverless-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-serverless-0.0.8.tar", last modified: Tue Oct 25 00:29:49 2022, max compression
+gzip compressed data, was "streamlink-serverless-0.0.9.tar", last modified: Wed Oct 26 00:23:02 2022, max compression
```

## Comparing `streamlink-serverless-0.0.8.tar` & `streamlink-serverless-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 00:29:49.784985 streamlink-serverless-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6325 2022-10-25 00:29:49.784985 streamlink-serverless-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5411 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-25 00:29:49.784985 streamlink-serverless-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 00:29:49.784985 streamlink-serverless-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 00:29:49.784985 streamlink-serverless-0.0.8/src/streamlink_serverless/
--rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/src/streamlink_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 00:29:49.784985 streamlink-serverless-0.0.8/src/streamlink_serverless/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/src/streamlink_serverless/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   369928 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/src/streamlink_serverless/_jsii/streamlink-serverless@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 00:29:36.000000 streamlink-serverless-0.0.8/src/streamlink_serverless/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 00:29:49.784985 streamlink-serverless-0.0.8/src/streamlink_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6325 2022-10-25 00:29:49.000000 streamlink-serverless-0.0.8/src/streamlink_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-25 00:29:49.000000 streamlink-serverless-0.0.8/src/streamlink_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 00:29:49.000000 streamlink-serverless-0.0.8/src/streamlink_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-25 00:29:49.000000 streamlink-serverless-0.0.8/src/streamlink_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-25 00:29:49.000000 streamlink-serverless-0.0.8/src/streamlink_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 00:23:02.316248 streamlink-serverless-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6325 2022-10-26 00:23:02.316248 streamlink-serverless-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5411 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 00:23:02.316248 streamlink-serverless-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 00:23:02.316248 streamlink-serverless-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 00:23:02.316248 streamlink-serverless-0.0.9/src/streamlink_serverless/
+-rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/src/streamlink_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 00:23:02.316248 streamlink-serverless-0.0.9/src/streamlink_serverless/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/src/streamlink_serverless/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   369928 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/src/streamlink_serverless/_jsii/streamlink-serverless@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 00:22:50.000000 streamlink-serverless-0.0.9/src/streamlink_serverless/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 00:23:02.316248 streamlink-serverless-0.0.9/src/streamlink_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6325 2022-10-26 00:23:01.000000 streamlink-serverless-0.0.9/src/streamlink_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-26 00:23:02.000000 streamlink-serverless-0.0.9/src/streamlink_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 00:23:01.000000 streamlink-serverless-0.0.9/src/streamlink_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-26 00:23:02.000000 streamlink-serverless-0.0.9/src/streamlink_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-26 00:23:02.000000 streamlink-serverless-0.0.9/src/streamlink_serverless.egg-info/top_level.txt
```

### Comparing `streamlink-serverless-0.0.8/LICENSE` & `streamlink-serverless-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-serverless-0.0.8/PKG-INFO` & `streamlink-serverless-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink-serverless
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlink as a Service
 Home-page: https://github.com/mrgrain/streamlink-serverless.git
 Author: Momo Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/streamlink-serverless.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `streamlink-serverless-0.0.8/README.md` & `streamlink-serverless-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-serverless-0.0.8/setup.py` & `streamlink-serverless-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "streamlink-serverless",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Streamlink as a Service",
     "license": "MIT",
     "url": "https://github.com/mrgrain/streamlink-serverless.git",
     "long_description_content_type": "text/markdown",
     "author": "Momo Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "streamlink_serverless",
         "streamlink_serverless._jsii"
     ],
     "package_data": {
         "streamlink_serverless._jsii": [
-            "streamlink-serverless@0.0.8.jsii.tgz"
+            "streamlink-serverless@0.0.9.jsii.tgz"
         ],
         "streamlink_serverless": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `streamlink-serverless-0.0.8/src/streamlink_serverless/__init__.py` & `streamlink-serverless-0.0.9/src/streamlink_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-serverless-0.0.8/src/streamlink_serverless.egg-info/PKG-INFO` & `streamlink-serverless-0.0.9/src/streamlink_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink-serverless
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlink as a Service
 Home-page: https://github.com/mrgrain/streamlink-serverless.git
 Author: Momo Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/streamlink-serverless.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


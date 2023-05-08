# Comparing `tmp/aws_prototyping_sdk.nx_monorepo-0.9.3.tar.gz` & `tmp/aws_prototyping_sdk.nx_monorepo-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.nx_monorepo-0.9.3.tar", last modified: Thu Sep  8 03:54:36 2022, max compression
+gzip compressed data, was "aws_prototyping_sdk.nx_monorepo-0.9.4.tar", last modified: Mon Sep 12 23:20:52 2022, max compression
```

## Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3.tar` & `aws_prototyping_sdk.nx_monorepo-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.595864 aws_prototyping_sdk.nx_monorepo-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7815 2022-09-08 03:54:36.595864 aws_prototyping_sdk.nx_monorepo-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 03:54:36.595864 aws_prototyping_sdk.nx_monorepo-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.591864 aws_prototyping_sdk.nx_monorepo-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.591864 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.595864 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/nx_monorepo/
--rw-r--r--   0 runner    (1001) docker     (121)   213976 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/nx_monorepo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.595864 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/nx_monorepo/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/nx_monorepo/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31970 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/nx_monorepo/_jsii/nx-monorepo@0.9.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 03:54:24.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/nx_monorepo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.591864 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7815 2022-09-08 03:54:35.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-08 03:54:36.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 03:54:36.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-08 03:54:36.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-08 03:54:36.000000 aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:52.720296 aws_prototyping_sdk.nx_monorepo-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7815 2022-09-12 23:20:52.720296 aws_prototyping_sdk.nx_monorepo-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 23:20:52.720296 aws_prototyping_sdk.nx_monorepo-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:52.716296 aws_prototyping_sdk.nx_monorepo-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:52.716296 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:52.720296 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/nx_monorepo/
+-rw-r--r--   0 runner    (1001) docker     (121)   213976 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/nx_monorepo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:52.720296 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/nx_monorepo/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/nx_monorepo/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31986 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/nx_monorepo/_jsii/nx-monorepo@0.9.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 23:20:38.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/nx_monorepo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:52.720296 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7815 2022-09-12 23:20:51.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-12 23:20:52.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 23:20:52.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-12 23:20:52.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-12 23:20:52.000000 aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3/LICENSE` & `aws_prototyping_sdk.nx_monorepo-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3/PKG-INFO` & `aws_prototyping_sdk.nx_monorepo-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.nx_monorepo
-Version: 0.9.3
+Version: 0.9.4
 Summary: @aws-prototyping-sdk/nx-monorepo
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3/README.md` & `aws_prototyping_sdk.nx_monorepo-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3/setup.py` & `aws_prototyping_sdk.nx_monorepo-0.9.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.nx_monorepo",
-    "version": "0.9.3",
+    "version": "0.9.4",
     "description": "@aws-prototyping-sdk/nx-monorepo",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_prototyping_sdk.nx_monorepo",
         "aws_prototyping_sdk.nx_monorepo._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.nx_monorepo._jsii": [
-            "nx-monorepo@0.9.3.jsii.tgz"
+            "nx-monorepo@0.9.4.jsii.tgz"
         ],
         "aws_prototyping_sdk.nx_monorepo": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "jsii>=1.67.0, <2.0.0",
-        "projen>=0.61.41, <0.62.0",
+        "projen>=0.62.2, <0.63.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk/nx_monorepo/__init__.py` & `aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk/nx_monorepo/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/PKG-INFO` & `aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.nx-monorepo
-Version: 0.9.3
+Version: 0.9.4
 Summary: @aws-prototyping-sdk/nx-monorepo
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_prototyping_sdk.nx_monorepo-0.9.3/src/aws_prototyping_sdk.nx_monorepo.egg-info/SOURCES.txt` & `aws_prototyping_sdk.nx_monorepo-0.9.4/src/aws_prototyping_sdk.nx_monorepo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.nx_monorepo.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.nx_monorepo.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.nx_monorepo.egg-info/requires.txt
 src/aws_prototyping_sdk.nx_monorepo.egg-info/top_level.txt
 src/aws_prototyping_sdk/nx_monorepo/__init__.py
 src/aws_prototyping_sdk/nx_monorepo/py.typed
 src/aws_prototyping_sdk/nx_monorepo/_jsii/__init__.py
-src/aws_prototyping_sdk/nx_monorepo/_jsii/nx-monorepo@0.9.3.jsii.tgz
+src/aws_prototyping_sdk/nx_monorepo/_jsii/nx-monorepo@0.9.4.jsii.tgz
```


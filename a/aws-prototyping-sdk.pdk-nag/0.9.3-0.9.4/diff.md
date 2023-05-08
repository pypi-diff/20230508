# Comparing `tmp/aws_prototyping_sdk.pdk_nag-0.9.3.tar.gz` & `tmp/aws_prototyping_sdk.pdk_nag-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.pdk_nag-0.9.3.tar", last modified: Thu Sep  8 03:54:36 2022, max compression
+gzip compressed data, was "aws_prototyping_sdk.pdk_nag-0.9.4.tar", last modified: Mon Sep 12 23:20:58 2022, max compression
```

## Comparing `aws_prototyping_sdk.pdk_nag-0.9.3.tar` & `aws_prototyping_sdk.pdk_nag-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.951866 aws_prototyping_sdk.pdk_nag-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-08 03:54:36.951866 aws_prototyping_sdk.pdk_nag-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 03:54:36.951866 aws_prototyping_sdk.pdk_nag-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.947866 aws_prototyping_sdk.pdk_nag-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.947866 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.947866 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/pdk_nag/
--rw-r--r--   0 runner    (1001) docker     (121)    25562 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/pdk_nag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.951866 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/pdk_nag/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/pdk_nag/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22123 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/pdk_nag/_jsii/pdk-nag@0.9.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 03:54:25.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/pdk_nag/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:54:36.947866 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-08 03:54:36.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-09-08 03:54:36.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 03:54:36.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-08 03:54:36.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-08 03:54:36.000000 aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:58.216341 aws_prototyping_sdk.pdk_nag-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-12 23:20:58.216341 aws_prototyping_sdk.pdk_nag-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 23:20:58.216341 aws_prototyping_sdk.pdk_nag-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:58.204341 aws_prototyping_sdk.pdk_nag-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:58.204341 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:58.216341 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/pdk_nag/
+-rw-r--r--   0 runner    (1001) docker     (121)    25562 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/pdk_nag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:58.216341 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/pdk_nag/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/pdk_nag/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22144 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/pdk_nag/_jsii/pdk-nag@0.9.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 23:20:44.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/pdk_nag/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:20:58.216341 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-12 23:20:57.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-09-12 23:20:58.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 23:20:57.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-12 23:20:57.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-12 23:20:58.000000 aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.pdk_nag-0.9.3/LICENSE` & `aws_prototyping_sdk.pdk_nag-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.pdk_nag-0.9.3/PKG-INFO` & `aws_prototyping_sdk.pdk_nag-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.pdk_nag
-Version: 0.9.3
+Version: 0.9.4
 Summary: @aws-prototyping-sdk/pdk-nag
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_prototyping_sdk.pdk_nag-0.9.3/README.md` & `aws_prototyping_sdk.pdk_nag-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.pdk_nag-0.9.3/setup.py` & `aws_prototyping_sdk.pdk_nag-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.pdk_nag",
-    "version": "0.9.3",
+    "version": "0.9.4",
     "description": "@aws-prototyping-sdk/pdk-nag",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "aws_prototyping_sdk.pdk_nag",
         "aws_prototyping_sdk.pdk_nag._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.pdk_nag._jsii": [
-            "pdk-nag@0.9.3.jsii.tgz"
+            "pdk-nag@0.9.4.jsii.tgz"
         ],
         "aws_prototyping_sdk.pdk_nag": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.40.0, <3.0.0",
-        "cdk-nag>=2.18.1, <3.0.0",
-        "constructs>=10.1.94, <11.0.0",
+        "aws-cdk-lib>=2.41.0, <3.0.0",
+        "cdk-nag>=2.18.7, <3.0.0",
+        "constructs>=10.1.100, <11.0.0",
         "jsii>=1.67.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk/pdk_nag/__init__.py` & `aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk/pdk_nag/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/PKG-INFO` & `aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.pdk-nag
-Version: 0.9.3
+Version: 0.9.4
 Summary: @aws-prototyping-sdk/pdk-nag
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_prototyping_sdk.pdk_nag-0.9.3/src/aws_prototyping_sdk.pdk_nag.egg-info/SOURCES.txt` & `aws_prototyping_sdk.pdk_nag-0.9.4/src/aws_prototyping_sdk.pdk_nag.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.pdk_nag.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.pdk_nag.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.pdk_nag.egg-info/requires.txt
 src/aws_prototyping_sdk.pdk_nag.egg-info/top_level.txt
 src/aws_prototyping_sdk/pdk_nag/__init__.py
 src/aws_prototyping_sdk/pdk_nag/py.typed
 src/aws_prototyping_sdk/pdk_nag/_jsii/__init__.py
-src/aws_prototyping_sdk/pdk_nag/_jsii/pdk-nag@0.9.3.jsii.tgz
+src/aws_prototyping_sdk/pdk_nag/_jsii/pdk-nag@0.9.4.jsii.tgz
```


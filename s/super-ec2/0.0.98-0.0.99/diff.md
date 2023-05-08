# Comparing `tmp/super-ec2-0.0.98.tar.gz` & `tmp/super-ec2-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/super-ec2/super-ec2/dist/python/super-ec2-0.0.98.tar", last modified: Tue Aug  3 01:18:02 2021, max compression
+gzip compressed data, was "/__w/super-ec2/super-ec2/dist/python/super-ec2-0.0.99.tar", last modified: Wed Aug  4 01:12:48 2021, max compression
```

## Comparing `super-ec2-0.0.98.tar` & `super-ec2-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 01:18:02.000000 super-ec2-0.0.98/
--rw-r--r--   0 root         (0) root         (0)    11358 2021-08-03 01:17:56.000000 super-ec2-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2021-08-03 01:17:56.000000 super-ec2-0.0.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3955 2021-08-03 01:18:02.000000 super-ec2-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2517 2021-08-03 01:17:56.000000 super-ec2-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-08-03 01:17:56.000000 super-ec2-0.0.98/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-03 01:18:02.000000 super-ec2-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2485 2021-08-03 01:17:56.000000 super-ec2-0.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 01:18:02.000000 super-ec2-0.0.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 01:18:02.000000 super-ec2-0.0.98/src/super_ec2/
--rw-r--r--   0 root         (0) root         (0)    23055 2021-08-03 01:17:56.000000 super-ec2-0.0.98/src/super_ec2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 01:18:02.000000 super-ec2-0.0.98/src/super_ec2/_jsii/
--rw-r--r--   0 root         (0) root         (0)      993 2021-08-03 01:17:56.000000 super-ec2-0.0.98/src/super_ec2/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  3828665 2021-08-03 01:17:56.000000 super-ec2-0.0.98/src/super_ec2/_jsii/super-ec2@0.0.98.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-03 01:17:56.000000 super-ec2-0.0.98/src/super_ec2/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 01:18:02.000000 super-ec2-0.0.98/src/super_ec2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3955 2021-08-03 01:18:01.000000 super-ec2-0.0.98/src/super_ec2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      364 2021-08-03 01:18:01.000000 super-ec2-0.0.98/src/super_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-03 01:18:01.000000 super-ec2-0.0.98/src/super_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      726 2021-08-03 01:18:01.000000 super-ec2-0.0.98/src/super_ec2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-08-03 01:18:01.000000 super-ec2-0.0.98/src/super_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 01:12:48.000000 super-ec2-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)    11358 2021-08-04 01:12:43.000000 super-ec2-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-08-04 01:12:43.000000 super-ec2-0.0.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3955 2021-08-04 01:12:48.000000 super-ec2-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2517 2021-08-04 01:12:43.000000 super-ec2-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-08-04 01:12:43.000000 super-ec2-0.0.99/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-04 01:12:48.000000 super-ec2-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2485 2021-08-04 01:12:43.000000 super-ec2-0.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2/
+-rw-r--r--   0 root         (0) root         (0)    23055 2021-08-04 01:12:43.000000 super-ec2-0.0.99/src/super_ec2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      993 2021-08-04 01:12:43.000000 super-ec2-0.0.99/src/super_ec2/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  3828666 2021-08-04 01:12:43.000000 super-ec2-0.0.99/src/super_ec2/_jsii/super-ec2@0.0.99.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-04 01:12:43.000000 super-ec2-0.0.99/src/super_ec2/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3955 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      364 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      726 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-08-04 01:12:48.000000 super-ec2-0.0.99/src/super_ec2.egg-info/top_level.txt
```

### Comparing `super-ec2-0.0.98/LICENSE` & `super-ec2-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `super-ec2-0.0.98/PKG-INFO` & `super-ec2-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-ec2
-Version: 0.0.98
+Version: 0.0.99
 Summary: A construct lib for AWS CDK EC2
 Home-page: https://github.com/cdk-constructs-zone/super-ec2.git
 Author: @cdk-constructs-zone
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk-constructs-zone/super-ec2.git
 Description: [![NPM version](https://badge.fury.io/js/%40cdk-constructs-zone%2Fsuper-ec2.svg)](https://badge.fury.io/js/%40cdk-constructs-zone%2Fsuper-ec2)
         [![PyPI version](https://badge.fury.io/py/super-ec2.svg)](https://badge.fury.io/py/super-ec2)
```

### Comparing `super-ec2-0.0.98/README.md` & `super-ec2-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `super-ec2-0.0.98/setup.py` & `super-ec2-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "super-ec2",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "A construct lib for AWS CDK EC2",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk-constructs-zone/super-ec2.git",
     "long_description_content_type": "text/markdown",
     "author": "@cdk-constructs-zone",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "super_ec2",
         "super_ec2._jsii"
     ],
     "package_data": {
         "super_ec2._jsii": [
-            "super-ec2@0.0.98.jsii.tgz"
+            "super-ec2@0.0.99.jsii.tgz"
         ],
         "super_ec2": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `super-ec2-0.0.98/src/super_ec2/__init__.py` & `super-ec2-0.0.99/src/super_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ec2-0.0.98/src/super_ec2/_jsii/__init__.py` & `super-ec2-0.0.99/src/super_ec2/_jsii/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 import aws_cdk.aws_sns_subscriptions._jsii
 import aws_cdk.core._jsii
 import aws_cdk.custom_resources._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdk-constructs-zone/super-ec2",
-    "0.0.98",
+    "0.0.99",
     __name__[0:-6],
-    "super-ec2@0.0.98.jsii.tgz",
+    "super-ec2@0.0.99.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `super-ec2-0.0.98/src/super_ec2.egg-info/PKG-INFO` & `super-ec2-0.0.99/src/super_ec2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-ec2
-Version: 0.0.98
+Version: 0.0.99
 Summary: A construct lib for AWS CDK EC2
 Home-page: https://github.com/cdk-constructs-zone/super-ec2.git
 Author: @cdk-constructs-zone
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk-constructs-zone/super-ec2.git
 Description: [![NPM version](https://badge.fury.io/js/%40cdk-constructs-zone%2Fsuper-ec2.svg)](https://badge.fury.io/js/%40cdk-constructs-zone%2Fsuper-ec2)
         [![PyPI version](https://badge.fury.io/py/super-ec2.svg)](https://badge.fury.io/py/super-ec2)
```

### Comparing `super-ec2-0.0.98/src/super_ec2.egg-info/requires.txt` & `super-ec2-0.0.99/src/super_ec2.egg-info/requires.txt`

 * *Files identical despite different names*


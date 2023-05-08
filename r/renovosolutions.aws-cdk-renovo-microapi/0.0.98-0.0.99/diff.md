# Comparing `tmp/renovosolutions.aws-cdk-renovo-microapi-0.0.98.tar.gz` & `tmp/renovosolutions.aws-cdk-renovo-microapi-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-renovo-microapi-0.0.98.tar", last modified: Tue Aug  9 18:51:41 2022, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-renovo-microapi-0.0.99.tar", last modified: Wed Aug 10 13:11:32 2022, max compression
```

## Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98.tar` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 18:51:41.562214 renovosolutions.aws-cdk-renovo-microapi-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-08-09 18:51:41.562214 renovosolutions.aws-cdk-renovo-microapi-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 18:51:41.562214 renovosolutions.aws-cdk-renovo-microapi-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 18:51:41.558214 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 18:51:41.562214 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/ipam/
--rw-r--r--   0 runner    (1001) docker     (121)    16744 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/ipam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 18:51:41.562214 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/ipam/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/ipam/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   160409 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/ipam/_jsii/cdk-library-renovo-microapi@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 18:51:30.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/ipam/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 18:51:41.562214 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-08-09 18:51:41.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-08-09 18:51:41.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 18:51:41.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-09 18:51:41.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-09 18:51:41.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:11:32.989592 renovosolutions.aws-cdk-renovo-microapi-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-08-10 13:11:32.989592 renovosolutions.aws-cdk-renovo-microapi-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-10 13:11:32.989592 renovosolutions.aws-cdk-renovo-microapi-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:11:32.985592 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:11:32.985592 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/ipam/
+-rw-r--r--   0 runner    (1001) docker     (121)    16744 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/ipam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:11:32.985592 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/ipam/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/ipam/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   160409 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/ipam/_jsii/cdk-library-renovo-microapi@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 13:11:21.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/ipam/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:11:32.989592 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-08-10 13:11:32.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-08-10 13:11:32.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 13:11:32.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-10 13:11:32.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-10 13:11:32.000000 renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98/LICENSE` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98/PKG-INFO` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-renovo-microapi
-Version: 0.0.98
+Version: 0.0.99
 Summary: AWS CDK Construct Library to manage micro apis for Renovo Solutions
 Home-page: https://github.com/RenovoSolutions/cdk-library-renovo-microapi.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-renovo-microapi.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98/README.md` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98/setup.py` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-renovo-microapi",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "AWS CDK Construct Library to manage micro apis for Renovo Solutions",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-renovo-microapi.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "ipam",
         "ipam._jsii"
     ],
     "package_data": {
         "ipam._jsii": [
-            "cdk-library-renovo-microapi@0.0.98.jsii.tgz"
+            "cdk-library-renovo-microapi@0.0.99.jsii.tgz"
         ],
         "ipam": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.36.0, <3.0.0",
+        "aws-cdk-lib>=2.37.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.63.2, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/ipam/__init__.py` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/ipam/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-renovo-microapi
-Version: 0.0.98
+Version: 0.0.99
 Summary: AWS CDK Construct Library to manage micro apis for Renovo Solutions
 Home-page: https://github.com/RenovoSolutions/cdk-library-renovo-microapi.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-renovo-microapi.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-renovo-microapi-0.0.98/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-renovo-microapi-0.0.99/src/renovosolutions.aws_cdk_renovo_microapi.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/ipam/__init__.py
 src/ipam/py.typed
 src/ipam/_jsii/__init__.py
-src/ipam/_jsii/cdk-library-renovo-microapi@0.0.98.jsii.tgz
+src/ipam/_jsii/cdk-library-renovo-microapi@0.0.99.jsii.tgz
 src/renovosolutions.aws_cdk_renovo_microapi.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_renovo_microapi.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_renovo_microapi.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_renovo_microapi.egg-info/requires.txt
 src/renovosolutions.aws_cdk_renovo_microapi.egg-info/top_level.txt
```


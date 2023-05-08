# Comparing `tmp/pepperize.cdk-lambda-deno-0.0.98.tar.gz` & `tmp/pepperize.cdk-lambda-deno-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperize.cdk-lambda-deno-0.0.98.tar", last modified: Fri Sep 30 16:55:17 2022, max compression
+gzip compressed data, was "pepperize.cdk-lambda-deno-0.0.99.tar", last modified: Mon Oct  3 16:53:44 2022, max compression
```

## Comparing `pepperize.cdk-lambda-deno-0.0.98.tar` & `pepperize.cdk-lambda-deno-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 16:55:17.648369 pepperize.cdk-lambda-deno-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-09-30 16:55:17.648369 pepperize.cdk-lambda-deno-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-30 16:55:17.648369 pepperize.cdk-lambda-deno-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 16:55:17.648369 pepperize.cdk-lambda-deno-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 16:55:17.648369 pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-09-30 16:55:16.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-09-30 16:55:17.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 16:55:17.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-30 16:55:17.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-30 16:55:17.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 16:55:17.648369 pepperize.cdk-lambda-deno-0.0.98/src/pepperize_cdk_lambda_deno/
--rw-r--r--   0 runner    (1001) docker     (121)    58789 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize_cdk_lambda_deno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 16:55:17.648369 pepperize.cdk-lambda-deno-0.0.98/src/pepperize_cdk_lambda_deno/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize_cdk_lambda_deno/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31018 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize_cdk_lambda_deno/_jsii/cdk-lambda-deno@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 16:55:03.000000 pepperize.cdk-lambda-deno-0.0.98/src/pepperize_cdk_lambda_deno/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:53:44.105158 pepperize.cdk-lambda-deno-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-10-03 16:53:44.105158 pepperize.cdk-lambda-deno-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 16:53:44.105158 pepperize.cdk-lambda-deno-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:53:44.101158 pepperize.cdk-lambda-deno-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:53:44.105158 pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-10-03 16:53:43.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-10-03 16:53:44.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 16:53:43.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-03 16:53:43.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-03 16:53:43.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:53:44.105158 pepperize.cdk-lambda-deno-0.0.99/src/pepperize_cdk_lambda_deno/
+-rw-r--r--   0 runner    (1001) docker     (121)    58789 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize_cdk_lambda_deno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:53:44.105158 pepperize.cdk-lambda-deno-0.0.99/src/pepperize_cdk_lambda_deno/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize_cdk_lambda_deno/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31018 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize_cdk_lambda_deno/_jsii/cdk-lambda-deno@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 16:53:29.000000 pepperize.cdk-lambda-deno-0.0.99/src/pepperize_cdk_lambda_deno/py.typed
```

### Comparing `pepperize.cdk-lambda-deno-0.0.98/LICENSE` & `pepperize.cdk-lambda-deno-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-lambda-deno-0.0.98/PKG-INFO` & `pepperize.cdk-lambda-deno-0.0.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-lambda-deno
-Version: 0.0.98
+Version: 0.0.99
 Summary: AWS CDK custom AWS Lambda runtime with Deno
 Home-page: https://github.com/pepperize/cdk-lambda-deno.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-lambda-deno.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.cdk-lambda-deno-0.0.98/README.md` & `pepperize.cdk-lambda-deno-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-lambda-deno-0.0.98/setup.py` & `pepperize.cdk-lambda-deno-0.0.99/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pepperize.cdk-lambda-deno",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "AWS CDK custom AWS Lambda runtime with Deno",
     "license": "MIT",
     "url": "https://github.com/pepperize/cdk-lambda-deno.git",
     "long_description_content_type": "text/markdown",
     "author": "Patrick Florek<patrick.florek@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pepperize_cdk_lambda_deno",
         "pepperize_cdk_lambda_deno._jsii"
     ],
     "package_data": {
         "pepperize_cdk_lambda_deno._jsii": [
-            "cdk-lambda-deno@0.0.98.jsii.tgz"
+            "cdk-lambda-deno@0.0.99.jsii.tgz"
         ],
         "pepperize_cdk_lambda_deno": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/PKG-INFO` & `pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-lambda-deno
-Version: 0.0.98
+Version: 0.0.99
 Summary: AWS CDK custom AWS Lambda runtime with Deno
 Home-page: https://github.com/pepperize/cdk-lambda-deno.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-lambda-deno.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.cdk-lambda-deno-0.0.98/src/pepperize.cdk_lambda_deno.egg-info/SOURCES.txt` & `pepperize.cdk-lambda-deno-0.0.99/src/pepperize.cdk_lambda_deno.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pepperize.cdk_lambda_deno.egg-info/SOURCES.txt
 src/pepperize.cdk_lambda_deno.egg-info/dependency_links.txt
 src/pepperize.cdk_lambda_deno.egg-info/requires.txt
 src/pepperize.cdk_lambda_deno.egg-info/top_level.txt
 src/pepperize_cdk_lambda_deno/__init__.py
 src/pepperize_cdk_lambda_deno/py.typed
 src/pepperize_cdk_lambda_deno/_jsii/__init__.py
-src/pepperize_cdk_lambda_deno/_jsii/cdk-lambda-deno@0.0.98.jsii.tgz
+src/pepperize_cdk_lambda_deno/_jsii/cdk-lambda-deno@0.0.99.jsii.tgz
```

### Comparing `pepperize.cdk-lambda-deno-0.0.98/src/pepperize_cdk_lambda_deno/__init__.py` & `pepperize.cdk-lambda-deno-0.0.99/src/pepperize_cdk_lambda_deno/__init__.py`

 * *Files identical despite different names*


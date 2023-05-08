# Comparing `tmp/renovosolutions.aws-cdk-route53targets-0.0.98.tar.gz` & `tmp/renovosolutions.aws-cdk-route53targets-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-route53targets-0.0.98.tar", last modified: Fri Jan  6 14:30:57 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-route53targets-0.0.99.tar", last modified: Tue Jan 17 14:11:02 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-route53targets-0.0.98.tar` & `renovosolutions.aws-cdk-route53targets-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:30:57.465207 renovosolutions.aws-cdk-route53targets-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-06 14:30:57.461207 renovosolutions.aws-cdk-route53targets-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 14:30:57.465207 renovosolutions.aws-cdk-route53targets-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:30:57.461207 renovosolutions.aws-cdk-route53targets-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:30:57.461207 renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-06 14:30:56.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-06 14:30:57.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:30:56.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-06 14:30:57.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-06 14:30:57.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:30:57.461207 renovosolutions.aws-cdk-route53targets-0.0.98/src/route53targets/
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/route53targets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:30:57.461207 renovosolutions.aws-cdk-route53targets-0.0.98/src/route53targets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/route53targets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16536 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/route53targets/_jsii/cdk-library-route53targets@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:30:43.000000 renovosolutions.aws-cdk-route53targets-0.0.98/src/route53targets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:11:02.854802 renovosolutions.aws-cdk-route53targets-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-17 14:11:02.854802 renovosolutions.aws-cdk-route53targets-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:11:02.854802 renovosolutions.aws-cdk-route53targets-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:11:02.850802 renovosolutions.aws-cdk-route53targets-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:11:02.854802 renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-17 14:11:02.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-17 14:11:02.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:11:02.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-17 14:11:02.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-17 14:11:02.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:11:02.854802 renovosolutions.aws-cdk-route53targets-0.0.99/src/route53targets/
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/route53targets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:11:02.854802 renovosolutions.aws-cdk-route53targets-0.0.99/src/route53targets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/route53targets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/route53targets/_jsii/cdk-library-route53targets@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:10:47.000000 renovosolutions.aws-cdk-route53targets-0.0.99/src/route53targets/py.typed
```

### Comparing `renovosolutions.aws-cdk-route53targets-0.0.98/LICENSE` & `renovosolutions.aws-cdk-route53targets-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-route53targets-0.0.98/PKG-INFO` & `renovosolutions.aws-cdk-route53targets-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-route53targets
-Version: 0.0.98
+Version: 0.0.99
 Summary: An AWS CDK library that adds functionality for targetting additional resources in Route53
 Home-page: https://github.com/RenovoSolutions/cdk-library-route53targets.git
 Author: Renovo Solutions<devops@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-route53targets.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-route53targets-0.0.98/README.md` & `renovosolutions.aws-cdk-route53targets-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-route53targets-0.0.98/setup.py` & `renovosolutions.aws-cdk-route53targets-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-route53targets",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "An AWS CDK library that adds functionality for targetting additional resources in Route53",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-route53targets.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<devops@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "route53targets",
         "route53targets._jsii"
     ],
     "package_data": {
         "route53targets._jsii": [
-            "cdk-library-route53targets@0.0.98.jsii.tgz"
+            "cdk-library-route53targets@0.0.99.jsii.tgz"
         ],
         "route53targets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-route53targets
-Version: 0.0.98
+Version: 0.0.99
 Summary: An AWS CDK library that adds functionality for targetting additional resources in Route53
 Home-page: https://github.com/RenovoSolutions/cdk-library-route53targets.git
 Author: Renovo Solutions<devops@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-route53targets.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-route53targets-0.0.98/src/renovosolutions.aws_cdk_route53targets.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-route53targets-0.0.99/src/renovosolutions.aws_cdk_route53targets.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/renovosolutions.aws_cdk_route53targets.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_route53targets.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_route53targets.egg-info/requires.txt
 src/renovosolutions.aws_cdk_route53targets.egg-info/top_level.txt
 src/route53targets/__init__.py
 src/route53targets/py.typed
 src/route53targets/_jsii/__init__.py
-src/route53targets/_jsii/cdk-library-route53targets@0.0.98.jsii.tgz
+src/route53targets/_jsii/cdk-library-route53targets@0.0.99.jsii.tgz
```

### Comparing `renovosolutions.aws-cdk-route53targets-0.0.98/src/route53targets/__init__.py` & `renovosolutions.aws-cdk-route53targets-0.0.99/src/route53targets/__init__.py`

 * *Files identical despite different names*


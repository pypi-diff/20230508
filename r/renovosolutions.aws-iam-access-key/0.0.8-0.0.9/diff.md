# Comparing `tmp/renovosolutions.aws-iam-access-key-0.0.8.tar.gz` & `tmp/renovosolutions.aws-iam-access-key-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-iam-access-key-0.0.8.tar", last modified: Wed Feb  1 13:36:50 2023, max compression
+gzip compressed data, was "renovosolutions.aws-iam-access-key-0.0.9.tar", last modified: Wed Feb  8 20:11:47 2023, max compression
```

## Comparing `renovosolutions.aws-iam-access-key-0.0.8.tar` & `renovosolutions.aws-iam-access-key-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:36:50.831420 renovosolutions.aws-iam-access-key-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-01 13:36:50.831420 renovosolutions.aws-iam-access-key-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 13:36:50.831420 renovosolutions.aws-iam-access-key-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:36:50.827420 renovosolutions.aws-iam-access-key-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:36:50.827420 renovosolutions.aws-iam-access-key-0.0.8/src/iam-access-key/
--rw-r--r--   0 runner    (1001) docker     (123)    58989 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/src/iam-access-key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:36:50.831420 renovosolutions.aws-iam-access-key-0.0.8/src/iam-access-key/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/src/iam-access-key/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37117 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/src/iam-access-key/_jsii/cdk-library-aws-iam-access-key@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 13:36:35.000000 renovosolutions.aws-iam-access-key-0.0.8/src/iam-access-key/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:36:50.831420 renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-01 13:36:50.000000 renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-01 13:36:50.000000 renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 13:36:50.000000 renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-01 13:36:50.000000 renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-01 13:36:50.000000 renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:11:47.235664 renovosolutions.aws-iam-access-key-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-08 20:11:47.235664 renovosolutions.aws-iam-access-key-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 20:11:47.235664 renovosolutions.aws-iam-access-key-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:11:47.235664 renovosolutions.aws-iam-access-key-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:11:47.235664 renovosolutions.aws-iam-access-key-0.0.9/src/iam-access-key/
+-rw-r--r--   0 runner    (1001) docker     (123)    58989 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/src/iam-access-key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:11:47.235664 renovosolutions.aws-iam-access-key-0.0.9/src/iam-access-key/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/src/iam-access-key/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37110 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/src/iam-access-key/_jsii/cdk-library-aws-iam-access-key@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:11:32.000000 renovosolutions.aws-iam-access-key-0.0.9/src/iam-access-key/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:11:47.235664 renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-08 20:11:46.000000 renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-08 20:11:47.000000 renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:11:46.000000 renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-08 20:11:47.000000 renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-08 20:11:47.000000 renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-iam-access-key-0.0.8/LICENSE` & `renovosolutions.aws-iam-access-key-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-iam-access-key-0.0.8/PKG-INFO` & `renovosolutions.aws-iam-access-key-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-iam-access-key
-Version: 0.0.8
+Version: 0.0.9
 Summary: AWS CDK Construct Library for generating AWS access keys and storing them in Secrets Manager
 Home-page: https://github.com/brandon/cdk-library-aws-iam-access-key.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/brandon/cdk-library-aws-iam-access-key.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-iam-access-key-0.0.8/README.md` & `renovosolutions.aws-iam-access-key-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-iam-access-key-0.0.8/setup.py` & `renovosolutions.aws-iam-access-key-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-iam-access-key",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "AWS CDK Construct Library for generating AWS access keys and storing them in Secrets Manager",
     "license": "Apache-2.0",
     "url": "https://github.com/brandon/cdk-library-aws-iam-access-key.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "iam-access-key",
         "iam-access-key._jsii"
     ],
     "package_data": {
         "iam-access-key._jsii": [
-            "cdk-library-aws-iam-access-key@0.0.8.jsii.tgz"
+            "cdk-library-aws-iam-access-key@0.0.9.jsii.tgz"
         ],
         "iam-access-key": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `renovosolutions.aws-iam-access-key-0.0.8/src/iam-access-key/__init__.py` & `renovosolutions.aws-iam-access-key-0.0.9/src/iam-access-key/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/PKG-INFO` & `renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-iam-access-key
-Version: 0.0.8
+Version: 0.0.9
 Summary: AWS CDK Construct Library for generating AWS access keys and storing them in Secrets Manager
 Home-page: https://github.com/brandon/cdk-library-aws-iam-access-key.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/brandon/cdk-library-aws-iam-access-key.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-iam-access-key-0.0.8/src/renovosolutions.aws_iam_access_key.egg-info/SOURCES.txt` & `renovosolutions.aws-iam-access-key-0.0.9/src/renovosolutions.aws_iam_access_key.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/iam-access-key/__init__.py
 src/iam-access-key/py.typed
 src/iam-access-key/_jsii/__init__.py
-src/iam-access-key/_jsii/cdk-library-aws-iam-access-key@0.0.8.jsii.tgz
+src/iam-access-key/_jsii/cdk-library-aws-iam-access-key@0.0.9.jsii.tgz
 src/renovosolutions.aws_iam_access_key.egg-info/PKG-INFO
 src/renovosolutions.aws_iam_access_key.egg-info/SOURCES.txt
 src/renovosolutions.aws_iam_access_key.egg-info/dependency_links.txt
 src/renovosolutions.aws_iam_access_key.egg-info/requires.txt
 src/renovosolutions.aws_iam_access_key.egg-info/top_level.txt
```


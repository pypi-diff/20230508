# Comparing `tmp/renovosolutions.aws-cdk-aspects-security-group-2.1.98.tar.gz` & `tmp/renovosolutions.aws-cdk-aspects-security-group-2.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-aspects-security-group-2.1.98.tar", last modified: Mon Feb 27 13:49:28 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-aspects-security-group-2.1.99.tar", last modified: Mon Feb 27 14:18:54 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98.tar` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:49:28.346572 renovosolutions.aws-cdk-aspects-security-group-2.1.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-02-27 13:49:28.346572 renovosolutions.aws-cdk-aspects-security-group-2.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 13:49:28.346572 renovosolutions.aws-cdk-aspects-security-group-2.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:49:28.342572 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:49:28.346572 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/aspects-security-group/
--rw-r--r--   0 runner    (1001) docker     (123)    38484 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/aspects-security-group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:49:28.346572 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/aspects-security-group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/aspects-security-group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31342 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/aspects-security-group/_jsii/cdk-aspects-library-security-group@2.1.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 13:49:13.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/aspects-security-group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:49:28.346572 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-02-27 13:49:27.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-27 13:49:28.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 13:49:27.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-27 13:49:28.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 13:49:28.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:18:54.424341 renovosolutions.aws-cdk-aspects-security-group-2.1.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-02-27 14:18:54.424341 renovosolutions.aws-cdk-aspects-security-group-2.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 14:18:54.424341 renovosolutions.aws-cdk-aspects-security-group-2.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:18:54.424341 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:18:54.424341 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/aspects-security-group/
+-rw-r--r--   0 runner    (1001) docker     (123)    38484 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/aspects-security-group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:18:54.424341 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/aspects-security-group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/aspects-security-group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31342 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/aspects-security-group/_jsii/cdk-aspects-library-security-group@2.1.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 14:18:40.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/aspects-security-group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:18:54.424341 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-02-27 14:18:53.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-27 14:18:54.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 14:18:53.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-27 14:18:54.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 14:18:54.000000 renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98/LICENSE` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98/PKG-INFO` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-aspects-security-group
-Version: 2.1.98
+Version: 2.1.99
 Summary: A library of CDK aspects applying to security groups.
 Home-page: https://github.com/RenovoSolutions/cdk-aspects-library-security-group.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-aspects-library-security-group.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98/README.md` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98/setup.py` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-aspects-security-group",
-    "version": "2.1.98",
+    "version": "2.1.99",
     "description": "A library of CDK aspects applying to security groups.",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-aspects-library-security-group.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aspects-security-group",
         "aspects-security-group._jsii"
     ],
     "package_data": {
         "aspects-security-group._jsii": [
-            "cdk-aspects-library-security-group@2.1.98.jsii.tgz"
+            "cdk-aspects-library-security-group@2.1.99.jsii.tgz"
         ],
         "aspects-security-group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.64.0, <3.0.0",
+        "aws-cdk-lib>=2.66.1, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.73.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/aspects-security-group/__init__.py` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/aspects-security-group/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-aspects-security-group
-Version: 2.1.98
+Version: 2.1.99
 Summary: A library of CDK aspects applying to security groups.
 Home-page: https://github.com/RenovoSolutions/cdk-aspects-library-security-group.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-aspects-library-security-group.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-aspects-security-group-2.1.98/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-aspects-security-group-2.1.99/src/renovosolutions.aws_cdk_aspects_security_group.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/aspects-security-group/__init__.py
 src/aspects-security-group/py.typed
 src/aspects-security-group/_jsii/__init__.py
-src/aspects-security-group/_jsii/cdk-aspects-library-security-group@2.1.98.jsii.tgz
+src/aspects-security-group/_jsii/cdk-aspects-library-security-group@2.1.99.jsii.tgz
 src/renovosolutions.aws_cdk_aspects_security_group.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_aspects_security_group.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_aspects_security_group.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_aspects_security_group.egg-info/requires.txt
 src/renovosolutions.aws_cdk_aspects_security_group.egg-info/top_level.txt
```


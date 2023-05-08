# Comparing `tmp/aws_prototyping_sdk.identity-0.9.3.tar.gz` & `tmp/aws_prototyping_sdk.identity-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.identity-0.9.3.tar", last modified: Thu Sep  8 03:58:44 2022, max compression
+gzip compressed data, was "aws_prototyping_sdk.identity-0.9.4.tar", last modified: Mon Sep 12 23:25:49 2022, max compression
```

## Comparing `aws_prototyping_sdk.identity-0.9.3.tar` & `aws_prototyping_sdk.identity-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:58:44.628807 aws_prototyping_sdk.identity-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-08 03:58:44.628807 aws_prototyping_sdk.identity-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 03:58:44.628807 aws_prototyping_sdk.identity-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:58:44.624807 aws_prototyping_sdk.identity-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:58:44.624807 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:58:44.628807 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:58:44.628807 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19226 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/_jsii/identity@0.9.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 03:58:26.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 03:58:44.628807 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-08 03:58:43.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-08 03:58:44.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 03:58:43.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-09-08 03:58:44.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-08 03:58:44.000000 aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:25:49.319387 aws_prototyping_sdk.identity-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-12 23:25:49.319387 aws_prototyping_sdk.identity-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 23:25:49.319387 aws_prototyping_sdk.identity-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:25:49.315387 aws_prototyping_sdk.identity-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:25:49.315387 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:25:49.315387 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/
+-rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:25:49.319387 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19241 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/_jsii/identity@0.9.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 23:25:28.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 23:25:49.315387 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-12 23:25:48.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-12 23:25:49.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 23:25:48.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-09-12 23:25:48.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-12 23:25:49.000000 aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.identity-0.9.3/LICENSE` & `aws_prototyping_sdk.identity-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.identity-0.9.3/PKG-INFO` & `aws_prototyping_sdk.identity-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.identity
-Version: 0.9.3
+Version: 0.9.4
 Summary: @aws-prototyping-sdk/identity
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_prototyping_sdk.identity-0.9.3/README.md` & `aws_prototyping_sdk.identity-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.identity-0.9.3/setup.py` & `aws_prototyping_sdk.identity-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.identity",
-    "version": "0.9.3",
+    "version": "0.9.4",
     "description": "@aws-prototyping-sdk/identity",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,29 +22,29 @@
     },
     "packages": [
         "aws_prototyping_sdk.identity",
         "aws_prototyping_sdk.identity._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.identity._jsii": [
-            "identity@0.9.3.jsii.tgz"
+            "identity@0.9.4.jsii.tgz"
         ],
         "aws_prototyping_sdk.identity": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.40.0, <3.0.0",
-        "aws-cdk.aws-cognito-identitypool-alpha==2.40.0.a0",
-        "aws_prototyping_sdk.pdk_nag>=0.8.4, <0.9.0",
-        "cdk-nag>=2.18.1, <3.0.0",
-        "constructs>=10.1.94, <11.0.0",
+        "aws-cdk-lib>=2.41.0, <3.0.0",
+        "aws-cdk.aws-cognito-identitypool-alpha==2.41.0.a0",
+        "aws_prototyping_sdk.pdk_nag>=0.9.3, <0.10.0",
+        "cdk-nag>=2.18.7, <3.0.0",
+        "constructs>=10.1.100, <11.0.0",
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

### Comparing `aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/__init__.py` & `aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk/identity/_jsii/__init__.py` & `aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk/identity/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import aws_cdk.aws_cognito_identitypool_alpha._jsii
 import aws_prototyping_sdk.pdk_nag._jsii
 import cdk_nag._jsii
 import constructs._jsii
 import projen._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "@aws-prototyping-sdk/identity", "0.9.3", __name__[0:-6], "identity@0.9.3.jsii.tgz"
+    "@aws-prototyping-sdk/identity", "0.9.4", __name__[0:-6], "identity@0.9.4.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/PKG-INFO` & `aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.identity
-Version: 0.9.3
+Version: 0.9.4
 Summary: @aws-prototyping-sdk/identity
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_prototyping_sdk.identity-0.9.3/src/aws_prototyping_sdk.identity.egg-info/SOURCES.txt` & `aws_prototyping_sdk.identity-0.9.4/src/aws_prototyping_sdk.identity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.identity.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.identity.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.identity.egg-info/requires.txt
 src/aws_prototyping_sdk.identity.egg-info/top_level.txt
 src/aws_prototyping_sdk/identity/__init__.py
 src/aws_prototyping_sdk/identity/py.typed
 src/aws_prototyping_sdk/identity/_jsii/__init__.py
-src/aws_prototyping_sdk/identity/_jsii/identity@0.9.3.jsii.tgz
+src/aws_prototyping_sdk/identity/_jsii/identity@0.9.4.jsii.tgz
```


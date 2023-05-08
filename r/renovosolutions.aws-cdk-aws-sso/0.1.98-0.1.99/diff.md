# Comparing `tmp/renovosolutions.aws-cdk-aws-sso-0.1.98.tar.gz` & `tmp/renovosolutions.aws-cdk-aws-sso-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-aws-sso-0.1.98.tar", last modified: Mon Dec 19 13:49:19 2022, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-aws-sso-0.1.99.tar", last modified: Mon Dec 19 14:23:02 2022, max compression
```

## Comparing `renovosolutions.aws-cdk-aws-sso-0.1.98.tar` & `renovosolutions.aws-cdk-aws-sso-0.1.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:49:19.893542 renovosolutions.aws-cdk-aws-sso-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2022-12-19 13:49:19.893542 renovosolutions.aws-cdk-aws-sso-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 13:49:19.893542 renovosolutions.aws-cdk-aws-sso-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:49:19.889542 renovosolutions.aws-cdk-aws-sso-0.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:49:19.893542 renovosolutions.aws-cdk-aws-sso-0.1.98/src/renovosolutions.aws_cdk_aws_sso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2022-12-19 13:49:19.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/renovosolutions.aws_cdk_aws_sso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2022-12-19 13:49:19.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/renovosolutions.aws_cdk_aws_sso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 13:49:19.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/renovosolutions.aws_cdk_aws_sso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-19 13:49:19.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/renovosolutions.aws_cdk_aws_sso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-19 13:49:19.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/renovosolutions.aws_cdk_aws_sso.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:49:19.893542 renovosolutions.aws-cdk-aws-sso-0.1.98/src/sso/
--rw-r--r--   0 runner    (1001) docker     (123)    51552 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:49:19.893542 renovosolutions.aws-cdk-aws-sso-0.1.98/src/sso/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/sso/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33931 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/sso/_jsii/cdk-library-aws-sso@0.1.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 13:49:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.98/src/sso/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:23:02.353162 renovosolutions.aws-cdk-aws-sso-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2022-12-19 14:23:02.353162 renovosolutions.aws-cdk-aws-sso-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 14:23:02.353162 renovosolutions.aws-cdk-aws-sso-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:23:02.353162 renovosolutions.aws-cdk-aws-sso-0.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:23:02.353162 renovosolutions.aws-cdk-aws-sso-0.1.99/src/renovosolutions.aws_cdk_aws_sso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2022-12-19 14:23:01.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/renovosolutions.aws_cdk_aws_sso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2022-12-19 14:23:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/renovosolutions.aws_cdk_aws_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 14:23:01.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/renovosolutions.aws_cdk_aws_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-19 14:23:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/renovosolutions.aws_cdk_aws_sso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-19 14:23:02.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/renovosolutions.aws_cdk_aws_sso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:23:02.353162 renovosolutions.aws-cdk-aws-sso-0.1.99/src/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)    51552 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:23:02.353162 renovosolutions.aws-cdk-aws-sso-0.1.99/src/sso/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/sso/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33984 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/sso/_jsii/cdk-library-aws-sso@0.1.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 14:22:49.000000 renovosolutions.aws-cdk-aws-sso-0.1.99/src/sso/py.typed
```

### Comparing `renovosolutions.aws-cdk-aws-sso-0.1.98/LICENSE` & `renovosolutions.aws-cdk-aws-sso-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-aws-sso-0.1.98/PKG-INFO` & `renovosolutions.aws-cdk-aws-sso-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-aws-sso
-Version: 0.1.98
+Version: 0.1.99
 Summary: AWS CDK Construct Library for AWS SSO
 Home-page: https://github.com/brandon/cdk-library-aws-sso.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/brandon/cdk-library-aws-sso.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-aws-sso-0.1.98/README.md` & `renovosolutions.aws-cdk-aws-sso-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-aws-sso-0.1.98/setup.py` & `renovosolutions.aws-cdk-aws-sso-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-aws-sso",
-    "version": "0.1.98",
+    "version": "0.1.99",
     "description": "AWS CDK Construct Library for AWS SSO",
     "license": "Apache-2.0",
     "url": "https://github.com/brandon/cdk-library-aws-sso.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "sso",
         "sso._jsii"
     ],
     "package_data": {
         "sso._jsii": [
-            "cdk-library-aws-sso@0.1.98.jsii.tgz"
+            "cdk-library-aws-sso@0.1.99.jsii.tgz"
         ],
         "sso": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.54.0, <3.0.0",
+        "aws-cdk-lib>=2.55.1, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.72.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `renovosolutions.aws-cdk-aws-sso-0.1.98/src/renovosolutions.aws_cdk_aws_sso.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-aws-sso-0.1.99/src/renovosolutions.aws_cdk_aws_sso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-aws-sso
-Version: 0.1.98
+Version: 0.1.99
 Summary: AWS CDK Construct Library for AWS SSO
 Home-page: https://github.com/brandon/cdk-library-aws-sso.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/brandon/cdk-library-aws-sso.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-aws-sso-0.1.98/src/sso/__init__.py` & `renovosolutions.aws-cdk-aws-sso-0.1.99/src/sso/__init__.py`

 * *Files identical despite different names*


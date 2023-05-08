# Comparing `tmp/renovosolutions.aws-cdk-aws-ipam-0.1.98.tar.gz` & `tmp/renovosolutions.aws-cdk-aws-ipam-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-aws-ipam-0.1.98.tar", last modified: Thu Jul 14 10:27:49 2022, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-aws-ipam-0.1.99.tar", last modified: Fri Jul 15 12:54:57 2022, max compression
```

## Comparing `renovosolutions.aws-cdk-aws-ipam-0.1.98.tar` & `renovosolutions.aws-cdk-aws-ipam-0.1.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 10:27:49.221521 renovosolutions.aws-cdk-aws-ipam-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-07-14 10:27:49.221521 renovosolutions.aws-cdk-aws-ipam-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-14 10:27:49.221521 renovosolutions.aws-cdk-aws-ipam-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 10:27:49.217522 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 10:27:49.217522 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/ipam/
--rw-r--r--   0 runner    (1001) docker     (121)    39729 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/ipam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 10:27:49.217522 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/ipam/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/ipam/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30958 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/ipam/_jsii/cdk-library-aws-ipam@0.1.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 10:27:33.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/ipam/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 10:27:49.221521 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/renovosolutions.aws_cdk_aws_ipam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-07-14 10:27:48.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/renovosolutions.aws_cdk_aws_ipam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-07-14 10:27:49.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/renovosolutions.aws_cdk_aws_ipam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 10:27:48.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/renovosolutions.aws_cdk_aws_ipam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-07-14 10:27:49.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/renovosolutions.aws_cdk_aws_ipam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-14 10:27:49.000000 renovosolutions.aws-cdk-aws-ipam-0.1.98/src/renovosolutions.aws_cdk_aws_ipam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 12:54:57.352115 renovosolutions.aws-cdk-aws-ipam-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-07-15 12:54:57.352115 renovosolutions.aws-cdk-aws-ipam-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-15 12:54:57.352115 renovosolutions.aws-cdk-aws-ipam-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 12:54:57.348115 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 12:54:57.352115 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/ipam/
+-rw-r--r--   0 runner    (1001) docker     (121)    39729 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/ipam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 12:54:57.352115 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/ipam/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/ipam/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30959 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/ipam/_jsii/cdk-library-aws-ipam@0.1.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 12:54:45.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/ipam/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 12:54:57.352115 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/renovosolutions.aws_cdk_aws_ipam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-07-15 12:54:56.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/renovosolutions.aws_cdk_aws_ipam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-07-15 12:54:57.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/renovosolutions.aws_cdk_aws_ipam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 12:54:56.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/renovosolutions.aws_cdk_aws_ipam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-07-15 12:54:57.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/renovosolutions.aws_cdk_aws_ipam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-15 12:54:57.000000 renovosolutions.aws-cdk-aws-ipam-0.1.99/src/renovosolutions.aws_cdk_aws_ipam.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-aws-ipam-0.1.98/LICENSE` & `renovosolutions.aws-cdk-aws-ipam-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-aws-ipam-0.1.98/PKG-INFO` & `renovosolutions.aws-cdk-aws-ipam-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-aws-ipam
-Version: 0.1.98
+Version: 0.1.99
 Summary: AWS CDK Construct Library to manage AWS VPC IP Address Manager resources
 Home-page: https://github.com/RenovoSolutions/cdk-library-aws-ipam.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-aws-ipam.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-aws-ipam-0.1.98/setup.py` & `renovosolutions.aws-cdk-aws-ipam-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-aws-ipam",
-    "version": "0.1.98",
+    "version": "0.1.99",
     "description": "AWS CDK Construct Library to manage AWS VPC IP Address Manager resources",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-aws-ipam.git",
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
-            "cdk-library-aws-ipam@0.1.98.jsii.tgz"
+            "cdk-library-aws-ipam@0.1.99.jsii.tgz"
         ],
         "ipam": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.31.2, <3.0.0",
+        "aws-cdk-lib>=2.32.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.62.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `renovosolutions.aws-cdk-aws-ipam-0.1.98/src/ipam/__init__.py` & `renovosolutions.aws-cdk-aws-ipam-0.1.99/src/ipam/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-aws-ipam-0.1.98/src/renovosolutions.aws_cdk_aws_ipam.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-aws-ipam-0.1.99/src/renovosolutions.aws_cdk_aws_ipam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-aws-ipam
-Version: 0.1.98
+Version: 0.1.99
 Summary: AWS CDK Construct Library to manage AWS VPC IP Address Manager resources
 Home-page: https://github.com/RenovoSolutions/cdk-library-aws-ipam.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-aws-ipam.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


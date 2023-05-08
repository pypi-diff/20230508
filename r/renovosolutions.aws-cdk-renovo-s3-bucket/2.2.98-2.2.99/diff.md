# Comparing `tmp/renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98.tar.gz` & `tmp/renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98.tar", last modified: Wed Feb 15 14:43:07 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99.tar", last modified: Mon Feb 27 13:55:25 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98.tar` & `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:43:07.816684 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-15 14:43:07.816684 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 14:43:07.816684 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:43:07.816684 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:43:07.816684 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovo_s3_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovo_s3_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:43:07.816684 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovo_s3_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovo_s3_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovo_s3_bucket/_jsii/cdk-library-renovo-s3-bucket@2.2.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 14:42:55.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovo_s3_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:43:07.816684 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-15 14:43:07.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-15 14:43:07.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 14:43:07.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-15 14:43:07.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-15 14:43:07.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:55:25.453474 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-27 13:55:25.453474 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 13:55:25.453474 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:55:25.449474 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:55:25.449474 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovo_s3_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovo_s3_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:55:25.449474 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovo_s3_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovo_s3_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovo_s3_bucket/_jsii/cdk-library-renovo-s3-bucket@2.2.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 13:55:09.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovo_s3_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:55:25.449474 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-27 13:55:24.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-27 13:55:25.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 13:55:24.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-27 13:55:25.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-27 13:55:25.000000 renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/LICENSE` & `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/PKG-INFO` & `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-renovo-s3-bucket
-Version: 2.2.98
+Version: 2.2.99
 Summary: An AWS CDK construct library for creating S3 buckets with desirable defaults.
 Home-page: https://github.com/RenovoSolutions/cdk-library-renovo-s3-bucket.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-renovo-s3-bucket.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/setup.py` & `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-renovo-s3-bucket",
-    "version": "2.2.98",
+    "version": "2.2.99",
     "description": "An AWS CDK construct library for creating S3 buckets with desirable defaults.",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-renovo-s3-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "renovo_s3_bucket",
         "renovo_s3_bucket._jsii"
     ],
     "package_data": {
         "renovo_s3_bucket._jsii": [
-            "cdk-library-renovo-s3-bucket@2.2.98.jsii.tgz"
+            "cdk-library-renovo-s3-bucket@2.2.99.jsii.tgz"
         ],
         "renovo_s3_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovo_s3_bucket/__init__.py` & `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovo_s3_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-renovo-s3-bucket
-Version: 2.2.98
+Version: 2.2.99
 Summary: An AWS CDK construct library for creating S3 buckets with desirable defaults.
 Home-page: https://github.com/RenovoSolutions/cdk-library-renovo-s3-bucket.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-renovo-s3-bucket.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.98/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-renovo-s3-bucket-2.2.99/src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/renovo_s3_bucket/__init__.py
 src/renovo_s3_bucket/py.typed
 src/renovo_s3_bucket/_jsii/__init__.py
-src/renovo_s3_bucket/_jsii/cdk-library-renovo-s3-bucket@2.2.98.jsii.tgz
+src/renovo_s3_bucket/_jsii/cdk-library-renovo-s3-bucket@2.2.99.jsii.tgz
 src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/requires.txt
 src/renovosolutions.aws_cdk_renovo_s3_bucket.egg-info/top_level.txt
```


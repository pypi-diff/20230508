# Comparing `tmp/cdk-serverless-clamscan-2.4.98.tar.gz` & `tmp/cdk-serverless-clamscan-2.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-serverless-clamscan-2.4.98.tar", last modified: Mon Nov 28 00:29:19 2022, max compression
+gzip compressed data, was "cdk-serverless-clamscan-2.4.99.tar", last modified: Tue Nov 29 00:33:02 2022, max compression
```

## Comparing `cdk-serverless-clamscan-2.4.98.tar` & `cdk-serverless-clamscan-2.4.99.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 00:29:19.467129 cdk-serverless-clamscan-2.4.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2022-11-28 00:29:19.467129 cdk-serverless-clamscan-2.4.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-28 00:29:19.467129 cdk-serverless-clamscan-2.4.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 00:29:19.463129 cdk-serverless-clamscan-2.4.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 00:29:19.463129 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/
--rw-r--r--   0 runner    (1001) docker     (123)    32243 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 00:29:19.463129 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 00:29:19.467129 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/_jsii/bin/0
--rw-r--r--   0 runner    (1001) docker     (123)   137128 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.4.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 00:29:05.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 00:29:19.463129 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2022-11-28 00:29:18.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-11-28 00:29:19.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 00:29:18.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-11-28 00:29:19.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-11-28 00:29:19.000000 cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.507713 cdk-serverless-clamscan-2.4.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2022-11-29 00:33:02.507713 cdk-serverless-clamscan-2.4.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-29 00:33:02.507713 cdk-serverless-clamscan-2.4.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/
+-rw-r--r--   0 runner    (1001) docker     (123)    32243 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/bin/0
+-rw-r--r--   0 runner    (1001) docker     (123)   137147 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.4.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2022-11-29 00:33:01.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2022-11-29 00:33:02.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 00:33:01.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-11-29 00:33:02.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-11-29 00:33:02.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/top_level.txt
```

### Comparing `cdk-serverless-clamscan-2.4.98/LICENSE` & `cdk-serverless-clamscan-2.4.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.4.98/PKG-INFO` & `cdk-serverless-clamscan-2.4.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.4.98
+Version: 2.4.99
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-serverless-clamscan-2.4.98/README.md` & `cdk-serverless-clamscan-2.4.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.4.98/setup.py` & `cdk-serverless-clamscan-2.4.99/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-serverless-clamscan",
-    "version": "2.4.98",
+    "version": "2.4.99",
     "description": "Serverless architecture to virus scan objects in Amazon S3.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/cdk-serverless-clamscan",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<donti@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_serverless_clamscan",
         "cdk_serverless_clamscan._jsii"
     ],
     "package_data": {
         "cdk_serverless_clamscan._jsii": [
-            "cdk-serverless-clamscan@2.4.98.jsii.tgz"
+            "cdk-serverless-clamscan@2.4.99.jsii.tgz"
         ],
         "cdk_serverless_clamscan": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan/__init__.py` & `cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/PKG-INFO` & `cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.4.98
+Version: 2.4.99
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-serverless-clamscan-2.4.98/src/cdk_serverless_clamscan.egg-info/SOURCES.txt` & `cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 src/cdk_serverless_clamscan/py.typed
 src/cdk_serverless_clamscan.egg-info/PKG-INFO
 src/cdk_serverless_clamscan.egg-info/SOURCES.txt
 src/cdk_serverless_clamscan.egg-info/dependency_links.txt
 src/cdk_serverless_clamscan.egg-info/requires.txt
 src/cdk_serverless_clamscan.egg-info/top_level.txt
 src/cdk_serverless_clamscan/_jsii/__init__.py
-src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.4.98.jsii.tgz
+src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.4.99.jsii.tgz
 src/cdk_serverless_clamscan/_jsii/bin/0
```


# Comparing `tmp/cdk8s-redis-0.1.98.tar.gz` & `tmp/cdk8s-redis-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk8s-redis/cdk8s-redis/dist/python/cdk8s-redis-0.1.98.tar", last modified: Sat Nov 27 00:17:30 2021, max compression
+gzip compressed data, was "/__w/cdk8s-redis/cdk8s-redis/dist/python/cdk8s-redis-0.1.99.tar", last modified: Sun Nov 28 00:21:56 2021, max compression
```

## Comparing `cdk8s-redis-0.1.98.tar` & `cdk8s-redis-0.1.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1783 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      888 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      106 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1670 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     4452 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/src/cdk8s_redis/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      355 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/src/cdk8s_redis/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)   249571 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/src/cdk8s_redis/_jsii/cdk8s-redis@0.1.98.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2021-11-27 00:17:26.000000 cdk8s-redis-0.1.98/src/cdk8s_redis/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1783 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      384 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       87 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       12 2021-11-27 00:17:30.000000 cdk8s-redis-0.1.98/src/cdk8s_redis.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1783 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      888 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      106 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1670 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     4452 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/src/cdk8s_redis/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      355 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/src/cdk8s_redis/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)   249573 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/src/cdk8s_redis/_jsii/cdk8s-redis@0.1.99.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2021-11-28 00:21:53.000000 cdk8s-redis-0.1.99/src/cdk8s_redis/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1783 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      384 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       87 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       12 2021-11-28 00:21:56.000000 cdk8s-redis-0.1.99/src/cdk8s_redis.egg-info/top_level.txt
```

### Comparing `cdk8s-redis-0.1.98/LICENSE` & `cdk8s-redis-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-redis-0.1.98/PKG-INFO` & `cdk8s-redis-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-redis
-Version: 0.1.98
+Version: 0.1.99
 Summary: redis constructs for cdk8s
 Home-page: https://github.com/cdk8s-team/cdk8s-redis.git
 Author: Amazon Web Services<https://aws.amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-redis.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk8s-redis-0.1.98/README.md` & `cdk8s-redis-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-redis-0.1.98/setup.py` & `cdk8s-redis-0.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-redis",
-    "version": "0.1.98",
+    "version": "0.1.99",
     "description": "redis constructs for cdk8s",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-redis.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<https://aws.amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cdk8s_redis",
         "cdk8s_redis._jsii"
     ],
     "package_data": {
         "cdk8s_redis._jsii": [
-            "cdk8s-redis@0.1.98.jsii.tgz"
+            "cdk8s-redis@0.1.99.jsii.tgz"
         ],
         "cdk8s_redis": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "cdk8s>=1.1.44, <2.0.0",
+        "cdk8s>=1.1.45, <2.0.0",
         "constructs>=3.3.161, <4.0.0",
         "jsii>=1.46.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk8s-redis-0.1.98/src/cdk8s_redis/__init__.py` & `cdk8s-redis-0.1.99/src/cdk8s_redis/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-redis-0.1.98/src/cdk8s_redis.egg-info/PKG-INFO` & `cdk8s-redis-0.1.99/src/cdk8s_redis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-redis
-Version: 0.1.98
+Version: 0.1.99
 Summary: redis constructs for cdk8s
 Home-page: https://github.com/cdk8s-team/cdk8s-redis.git
 Author: Amazon Web Services<https://aws.amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-redis.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


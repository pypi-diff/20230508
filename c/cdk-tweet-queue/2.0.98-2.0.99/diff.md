# Comparing `tmp/cdk-tweet-queue-2.0.98.tar.gz` & `tmp/cdk-tweet-queue-2.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-tweet-queue-2.0.98.tar", last modified: Tue Sep 13 00:33:28 2022, max compression
+gzip compressed data, was "cdk-tweet-queue-2.0.99.tar", last modified: Thu Sep 15 00:33:21 2022, max compression
```

## Comparing `cdk-tweet-queue-2.0.98.tar` & `cdk-tweet-queue-2.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:33:28.155885 cdk-tweet-queue-2.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-09-13 00:33:28.155885 cdk-tweet-queue-2.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-13 00:33:28.155885 cdk-tweet-queue-2.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:33:28.151885 cdk-tweet-queue-2.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:33:28.155885 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue/
--rw-r--r--   0 runner    (1001) docker     (121)    10933 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:33:28.155885 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    92756 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue/_jsii/cdk-tweet-queue@2.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 00:33:14.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:33:28.155885 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-09-13 00:33:27.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-13 00:33:28.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 00:33:27.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-13 00:33:27.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-13 00:33:28.000000 cdk-tweet-queue-2.0.98/src/cdk_tweet_queue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 00:33:21.993265 cdk-tweet-queue-2.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-09-15 00:33:21.993265 cdk-tweet-queue-2.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 00:33:21.993265 cdk-tweet-queue-2.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 00:33:21.989265 cdk-tweet-queue-2.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 00:33:21.989265 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue/
+-rw-r--r--   0 runner    (1001) docker     (121)    10933 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 00:33:21.993265 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    92756 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue/_jsii/cdk-tweet-queue@2.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 00:33:10.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 00:33:21.993265 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-09-15 00:33:21.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-15 00:33:21.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 00:33:21.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-15 00:33:21.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-15 00:33:21.000000 cdk-tweet-queue-2.0.99/src/cdk_tweet_queue.egg-info/top_level.txt
```

### Comparing `cdk-tweet-queue-2.0.98/LICENSE` & `cdk-tweet-queue-2.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-tweet-queue-2.0.98/PKG-INFO` & `cdk-tweet-queue-2.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-tweet-queue
-Version: 2.0.98
+Version: 2.0.99
 Summary: Defines an SQS queue with tweet stream from a search
 Home-page: https://github.com/eladb/cdk-tweet-queue
 Author: Elad Ben-Israel<elad.benisrael@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/eladb/cdk-tweet-queue
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-tweet-queue-2.0.98/README.md` & `cdk-tweet-queue-2.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-tweet-queue-2.0.98/setup.py` & `cdk-tweet-queue-2.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-tweet-queue",
-    "version": "2.0.98",
+    "version": "2.0.99",
     "description": "Defines an SQS queue with tweet stream from a search",
     "license": "Apache-2.0",
     "url": "https://github.com/eladb/cdk-tweet-queue",
     "long_description_content_type": "text/markdown",
     "author": "Elad Ben-Israel<elad.benisrael@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk_tweet_queue",
         "cdk_tweet_queue._jsii"
     ],
     "package_data": {
         "cdk_tweet_queue._jsii": [
-            "cdk-tweet-queue@2.0.98.jsii.tgz"
+            "cdk-tweet-queue@2.0.99.jsii.tgz"
         ],
         "cdk_tweet_queue": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.41.0, <3.0.0",
-        "constructs>=10.1.101, <11.0.0",
+        "constructs>=10.1.103, <11.0.0",
         "jsii>=1.67.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk-tweet-queue-2.0.98/src/cdk_tweet_queue/__init__.py` & `cdk-tweet-queue-2.0.99/src/cdk_tweet_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-tweet-queue-2.0.98/src/cdk_tweet_queue.egg-info/PKG-INFO` & `cdk-tweet-queue-2.0.99/src/cdk_tweet_queue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-tweet-queue
-Version: 2.0.98
+Version: 2.0.99
 Summary: Defines an SQS queue with tweet stream from a search
 Home-page: https://github.com/eladb/cdk-tweet-queue
 Author: Elad Ben-Israel<elad.benisrael@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/eladb/cdk-tweet-queue
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


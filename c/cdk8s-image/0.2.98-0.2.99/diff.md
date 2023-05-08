# Comparing `tmp/cdk8s-image-0.2.98.tar.gz` & `tmp/cdk8s-image-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-image-0.2.98.tar", last modified: Sat Mar 26 00:22:40 2022, max compression
+gzip compressed data, was "cdk8s-image-0.2.99.tar", last modified: Sun Mar 27 00:26:27 2022, max compression
```

## Comparing `cdk8s-image-0.2.98.tar` & `cdk8s-image-0.2.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 00:22:40.063360 cdk8s-image-0.2.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-03-26 00:22:40.063360 cdk8s-image-0.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-26 00:22:40.063360 cdk8s-image-0.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 00:22:40.059360 cdk8s-image-0.2.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 00:22:40.059360 cdk8s-image-0.2.98/src/cdk8s_image/
--rw-r--r--   0 runner    (1001) docker     (121)     6522 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/src/cdk8s_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 00:22:40.063360 cdk8s-image-0.2.98/src/cdk8s_image/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/src/cdk8s_image/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15279 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/src/cdk8s_image/_jsii/cdk8s-image@0.2.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 00:22:29.000000 cdk8s-image-0.2.98/src/cdk8s_image/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 00:22:40.063360 cdk8s-image-0.2.98/src/cdk8s_image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-03-26 00:22:39.000000 cdk8s-image-0.2.98/src/cdk8s_image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-03-26 00:22:39.000000 cdk8s-image-0.2.98/src/cdk8s_image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 00:22:39.000000 cdk8s-image-0.2.98/src/cdk8s_image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-03-26 00:22:39.000000 cdk8s-image-0.2.98/src/cdk8s_image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-26 00:22:39.000000 cdk8s-image-0.2.98/src/cdk8s_image.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 00:26:27.681080 cdk8s-image-0.2.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-03-27 00:26:27.681080 cdk8s-image-0.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-27 00:26:27.681080 cdk8s-image-0.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 00:26:27.681080 cdk8s-image-0.2.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 00:26:27.681080 cdk8s-image-0.2.99/src/cdk8s_image/
+-rw-r--r--   0 runner    (1001) docker     (121)     6522 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/src/cdk8s_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 00:26:27.681080 cdk8s-image-0.2.99/src/cdk8s_image/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/src/cdk8s_image/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15280 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/src/cdk8s_image/_jsii/cdk8s-image@0.2.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 00:26:14.000000 cdk8s-image-0.2.99/src/cdk8s_image/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 00:26:27.681080 cdk8s-image-0.2.99/src/cdk8s_image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-03-27 00:26:27.000000 cdk8s-image-0.2.99/src/cdk8s_image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-03-27 00:26:27.000000 cdk8s-image-0.2.99/src/cdk8s_image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 00:26:27.000000 cdk8s-image-0.2.99/src/cdk8s_image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-03-27 00:26:27.000000 cdk8s-image-0.2.99/src/cdk8s_image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-27 00:26:27.000000 cdk8s-image-0.2.99/src/cdk8s_image.egg-info/top_level.txt
```

### Comparing `cdk8s-image-0.2.98/LICENSE` & `cdk8s-image-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-image-0.2.98/PKG-INFO` & `cdk8s-image-0.2.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-image
-Version: 0.2.98
+Version: 0.2.99
 Summary: Build & Push local docker images inside CDK8s applications
 Home-page: https://github.com/cdk8s-team/cdk8s-image
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-image
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk8s-image-0.2.98/README.md` & `cdk8s-image-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-image-0.2.98/setup.py` & `cdk8s-image-0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-image",
-    "version": "0.2.98",
+    "version": "0.2.99",
     "description": "Build & Push local docker images inside CDK8s applications",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-image",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk8s_image",
         "cdk8s_image._jsii"
     ],
     "package_data": {
         "cdk8s_image._jsii": [
-            "cdk8s-image@0.2.98.jsii.tgz"
+            "cdk8s-image@0.2.99.jsii.tgz"
         ],
         "cdk8s_image": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "cdk8s>=1.5.51, <2.0.0",
-        "constructs>=3.3.249, <4.0.0",
+        "cdk8s>=1.5.52, <2.0.0",
+        "constructs>=3.3.250, <4.0.0",
         "jsii>=1.55.1, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-image-0.2.98/src/cdk8s_image/__init__.py` & `cdk8s-image-0.2.99/src/cdk8s_image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-image-0.2.98/src/cdk8s_image.egg-info/PKG-INFO` & `cdk8s-image-0.2.99/src/cdk8s_image.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-image
-Version: 0.2.98
+Version: 0.2.99
 Summary: Build & Push local docker images inside CDK8s applications
 Home-page: https://github.com/cdk8s-team/cdk8s-image
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-image
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


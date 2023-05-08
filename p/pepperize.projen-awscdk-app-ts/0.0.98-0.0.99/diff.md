# Comparing `tmp/pepperize.projen-awscdk-app-ts-0.0.98.tar.gz` & `tmp/pepperize.projen-awscdk-app-ts-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperize.projen-awscdk-app-ts-0.0.98.tar", last modified: Thu Apr 21 10:39:09 2022, max compression
+gzip compressed data, was "pepperize.projen-awscdk-app-ts-0.0.99.tar", last modified: Mon Apr 25 10:39:32 2022, max compression
```

## Comparing `pepperize.projen-awscdk-app-ts-0.0.98.tar` & `pepperize.projen-awscdk-app-ts-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 10:39:09.891442 pepperize.projen-awscdk-app-ts-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-04-21 10:39:09.891442 pepperize.projen-awscdk-app-ts-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-21 10:39:09.891442 pepperize.projen-awscdk-app-ts-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 10:39:09.887442 pepperize.projen-awscdk-app-ts-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 10:39:09.891442 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-04-21 10:39:09.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-04-21 10:39:09.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 10:39:09.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-21 10:39:09.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-04-21 10:39:09.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 10:39:09.891442 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize_projen_awscdk_app_ts/
--rw-r--r--   0 runner    (1001) docker     (121)   168036 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize_projen_awscdk_app_ts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 10:39:09.891442 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize_projen_awscdk_app_ts/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize_projen_awscdk_app_ts/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25225 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize_projen_awscdk_app_ts/_jsii/projen-awscdk-app-ts@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 10:38:58.000000 pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize_projen_awscdk_app_ts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 10:39:32.814688 pepperize.projen-awscdk-app-ts-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-04-25 10:39:32.814688 pepperize.projen-awscdk-app-ts-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 10:39:32.814688 pepperize.projen-awscdk-app-ts-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 10:39:32.814688 pepperize.projen-awscdk-app-ts-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 10:39:32.814688 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-04-25 10:39:32.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-04-25 10:39:32.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 10:39:32.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-25 10:39:32.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-04-25 10:39:32.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 10:39:32.814688 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize_projen_awscdk_app_ts/
+-rw-r--r--   0 runner    (1001) docker     (121)   168036 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize_projen_awscdk_app_ts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 10:39:32.814688 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize_projen_awscdk_app_ts/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize_projen_awscdk_app_ts/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25221 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize_projen_awscdk_app_ts/_jsii/projen-awscdk-app-ts@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 10:39:22.000000 pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize_projen_awscdk_app_ts/py.typed
```

### Comparing `pepperize.projen-awscdk-app-ts-0.0.98/LICENSE` & `pepperize.projen-awscdk-app-ts-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperize.projen-awscdk-app-ts-0.0.98/PKG-INFO` & `pepperize.projen-awscdk-app-ts-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.projen-awscdk-app-ts
-Version: 0.0.98
+Version: 0.0.99
 Summary: This project provides a projen project type providing presets for an AWS CDK construct library project
 Home-page: https://github.com/pepperize/projen-awscdk-app-ts.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/projen-awscdk-app-ts.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.projen-awscdk-app-ts-0.0.98/README.md` & `pepperize.projen-awscdk-app-ts-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `pepperize.projen-awscdk-app-ts-0.0.98/setup.py` & `pepperize.projen-awscdk-app-ts-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pepperize.projen-awscdk-app-ts",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "This project provides a projen project type providing presets for an AWS CDK construct library project",
     "license": "MIT",
     "url": "https://github.com/pepperize/projen-awscdk-app-ts.git",
     "long_description_content_type": "text/markdown",
     "author": "Patrick Florek<patrick.florek@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pepperize_projen_awscdk_app_ts",
         "pepperize_projen_awscdk_app_ts._jsii"
     ],
     "package_data": {
         "pepperize_projen_awscdk_app_ts._jsii": [
-            "projen-awscdk-app-ts@0.0.98.jsii.tgz"
+            "projen-awscdk-app-ts@0.0.99.jsii.tgz"
         ],
         "pepperize_projen_awscdk_app_ts": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/PKG-INFO` & `pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.projen-awscdk-app-ts
-Version: 0.0.98
+Version: 0.0.99
 Summary: This project provides a projen project type providing presets for an AWS CDK construct library project
 Home-page: https://github.com/pepperize/projen-awscdk-app-ts.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/projen-awscdk-app-ts.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize.projen_awscdk_app_ts.egg-info/SOURCES.txt` & `pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize.projen_awscdk_app_ts.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pepperize.projen_awscdk_app_ts.egg-info/SOURCES.txt
 src/pepperize.projen_awscdk_app_ts.egg-info/dependency_links.txt
 src/pepperize.projen_awscdk_app_ts.egg-info/requires.txt
 src/pepperize.projen_awscdk_app_ts.egg-info/top_level.txt
 src/pepperize_projen_awscdk_app_ts/__init__.py
 src/pepperize_projen_awscdk_app_ts/py.typed
 src/pepperize_projen_awscdk_app_ts/_jsii/__init__.py
-src/pepperize_projen_awscdk_app_ts/_jsii/projen-awscdk-app-ts@0.0.98.jsii.tgz
+src/pepperize_projen_awscdk_app_ts/_jsii/projen-awscdk-app-ts@0.0.99.jsii.tgz
```

### Comparing `pepperize.projen-awscdk-app-ts-0.0.98/src/pepperize_projen_awscdk_app_ts/__init__.py` & `pepperize.projen-awscdk-app-ts-0.0.99/src/pepperize_projen_awscdk_app_ts/__init__.py`

 * *Files identical despite different names*


# Comparing `tmp/cdk8s-grafana-0.1.98.tar.gz` & `tmp/cdk8s-grafana-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-grafana-0.1.98.tar", last modified: Mon Apr 25 01:33:57 2022, max compression
+gzip compressed data, was "cdk8s-grafana-0.1.99.tar", last modified: Tue Apr 26 01:34:00 2022, max compression
```

## Comparing `cdk8s-grafana-0.1.98.tar` & `cdk8s-grafana-0.1.99.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 01:33:57.936902 cdk8s-grafana-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-04-25 01:33:57.932902 cdk8s-grafana-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 01:33:57.936902 cdk8s-grafana-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 01:33:57.932902 cdk8s-grafana-0.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 01:33:57.932902 cdk8s-grafana-0.1.98/src/cdk8s_grafana/
--rw-r--r--   0 runner    (1001) docker     (121)    34811 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 01:33:57.932902 cdk8s-grafana-0.1.98/src/cdk8s_grafana/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   312291 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana/_jsii/cdk8s-grafana@0.1.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 01:33:46.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 01:33:57.932902 cdk8s-grafana-0.1.98/src/cdk8s_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-04-25 01:33:57.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-04-25 01:33:57.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 01:33:57.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-04-25 01:33:57.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-25 01:33:57.000000 cdk8s-grafana-0.1.98/src/cdk8s_grafana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 01:34:00.066641 cdk8s-grafana-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-04-26 01:34:00.062641 cdk8s-grafana-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-26 01:34:00.066641 cdk8s-grafana-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 01:34:00.062641 cdk8s-grafana-0.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 01:34:00.062641 cdk8s-grafana-0.1.99/src/cdk8s_grafana/
+-rw-r--r--   0 runner    (1001) docker     (121)    34811 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 01:34:00.062641 cdk8s-grafana-0.1.99/src/cdk8s_grafana/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   312292 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana/_jsii/cdk8s-grafana@0.1.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 01:33:48.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 01:34:00.062641 cdk8s-grafana-0.1.99/src/cdk8s_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-04-26 01:34:00.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-04-26 01:34:00.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 01:34:00.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-04-26 01:34:00.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-26 01:34:00.000000 cdk8s-grafana-0.1.99/src/cdk8s_grafana.egg-info/top_level.txt
```

### Comparing `cdk8s-grafana-0.1.98/LICENSE` & `cdk8s-grafana-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-grafana-0.1.98/PKG-INFO` & `cdk8s-grafana-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-grafana
-Version: 0.1.98
+Version: 0.1.99
 Summary: Grafana construct for cdk8s.
 Home-page: https://github.com/cdk8s-team/cdk8s-grafana.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-grafana.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk8s-grafana-0.1.98/README.md` & `cdk8s-grafana-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-grafana-0.1.98/setup.py` & `cdk8s-grafana-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-grafana",
-    "version": "0.1.98",
+    "version": "0.1.99",
     "description": "Grafana construct for cdk8s.",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-grafana.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk8s_grafana",
         "cdk8s_grafana._jsii"
     ],
     "package_data": {
         "cdk8s_grafana._jsii": [
-            "cdk8s-grafana@0.1.98.jsii.tgz"
+            "cdk8s-grafana@0.1.99.jsii.tgz"
         ],
         "cdk8s_grafana": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "cdk8s>=1.5.79, <2.0.0",
-        "constructs>=3.3.278, <4.0.0",
+        "cdk8s>=1.5.80, <2.0.0",
+        "constructs>=3.3.279, <4.0.0",
         "jsii>=1.57.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-grafana-0.1.98/src/cdk8s_grafana/__init__.py` & `cdk8s-grafana-0.1.99/src/cdk8s_grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-grafana-0.1.98/src/cdk8s_grafana.egg-info/PKG-INFO` & `cdk8s-grafana-0.1.99/src/cdk8s_grafana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-grafana
-Version: 0.1.98
+Version: 0.1.99
 Summary: Grafana construct for cdk8s.
 Home-page: https://github.com/cdk8s-team/cdk8s-grafana.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-grafana.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


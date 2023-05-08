# Comparing `tmp/cdk8s-operator-0.1.98.tar.gz` & `tmp/cdk8s-operator-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-operator-0.1.98.tar", last modified: Sun Apr 30 00:31:13 2023, max compression
+gzip compressed data, was "cdk8s-operator-0.1.99.tar", last modified: Mon May  1 00:30:27 2023, max compression
```

## Comparing `cdk8s-operator-0.1.98.tar` & `cdk8s-operator-0.1.99.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:13.326088 cdk8s-operator-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-30 00:31:13.322088 cdk8s-operator-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:31:13.326088 cdk8s-operator-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:13.322088 cdk8s-operator-0.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:13.322088 cdk8s-operator-0.1.98/src/cdk8s_operator/
--rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/src/cdk8s_operator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:13.322088 cdk8s-operator-0.1.98/src/cdk8s_operator/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/src/cdk8s_operator/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:13.322088 cdk8s-operator-0.1.98/src/cdk8s_operator/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/src/cdk8s_operator/_jsii/bin/cdk8s-server
--rw-r--r--   0 runner    (1001) docker     (123)   123590 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:30:57.000000 cdk8s-operator-0.1.98/src/cdk8s_operator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:13.322088 cdk8s-operator-0.1.98/src/cdk8s_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-30 00:31:13.000000 cdk8s-operator-0.1.98/src/cdk8s_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-30 00:31:13.000000 cdk8s-operator-0.1.98/src/cdk8s_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:31:13.000000 cdk8s-operator-0.1.98/src/cdk8s_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-30 00:31:13.000000 cdk8s-operator-0.1.98/src/cdk8s_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 00:31:13.000000 cdk8s-operator-0.1.98/src/cdk8s_operator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/src/cdk8s_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/src/cdk8s_operator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/src/cdk8s_operator/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/src/cdk8s_operator/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/src/cdk8s_operator/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/src/cdk8s_operator/_jsii/bin/cdk8s-server
+-rw-r--r--   0 runner    (1001) docker     (123)   123591 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:30:13.000000 cdk8s-operator-0.1.99/src/cdk8s_operator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:30:27.944248 cdk8s-operator-0.1.99/src/cdk8s_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-01 00:30:27.000000 cdk8s-operator-0.1.99/src/cdk8s_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 00:30:27.000000 cdk8s-operator-0.1.99/src/cdk8s_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:30:27.000000 cdk8s-operator-0.1.99/src/cdk8s_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 00:30:27.000000 cdk8s-operator-0.1.99/src/cdk8s_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 00:30:27.000000 cdk8s-operator-0.1.99/src/cdk8s_operator.egg-info/top_level.txt
```

### Comparing `cdk8s-operator-0.1.98/LICENSE` & `cdk8s-operator-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.98/PKG-INFO` & `cdk8s-operator-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.98
+Version: 0.1.99
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
 Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-operator-0.1.98/README.md` & `cdk8s-operator-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.98/setup.py` & `cdk8s-operator-0.1.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-operator",
-    "version": "0.1.98",
+    "version": "0.1.99",
     "description": "Create Kubernetes CRD Operators using CDK8s Constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-operator.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_operator",
         "cdk8s_operator._jsii"
     ],
     "package_data": {
         "cdk8s_operator._jsii": [
-            "cdk8s-operator@0.1.98.jsii.tgz"
+            "cdk8s-operator@0.1.99.jsii.tgz"
         ],
         "cdk8s_operator": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-operator-0.1.98/src/cdk8s_operator/__init__.py` & `cdk8s-operator-0.1.99/src/cdk8s_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.98/src/cdk8s_operator.egg-info/PKG-INFO` & `cdk8s-operator-0.1.99/src/cdk8s_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.98
+Version: 0.1.99
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
 Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


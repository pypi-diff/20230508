# Comparing `tmp/pharindoko.cdk-internal-gateway-1.1.8.tar.gz` & `tmp/pharindoko.cdk-internal-gateway-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharindoko.cdk-internal-gateway-1.1.8.tar", last modified: Tue Apr 25 16:26:34 2023, max compression
+gzip compressed data, was "pharindoko.cdk-internal-gateway-1.1.9.tar", last modified: Wed Apr 26 20:30:45 2023, max compression
```

## Comparing `pharindoko.cdk-internal-gateway-1.1.8.tar` & `pharindoko.cdk-internal-gateway-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:26:34.689431 pharindoko.cdk-internal-gateway-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-25 16:26:34.689431 pharindoko.cdk-internal-gateway-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:26:34.689431 pharindoko.cdk-internal-gateway-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:26:34.685431 pharindoko.cdk-internal-gateway-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:26:34.685431 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:26:34.689431 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/cdk_internal_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)    41254 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/cdk_internal_gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:26:34.689431 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/cdk_internal_gateway/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/cdk_internal_gateway/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   185450 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:26:22.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/cdk_internal_gateway/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:26:34.689431 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-25 16:26:34.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-25 16:26:34.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:26:34.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 16:26:34.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 16:26:34.000000 pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:45.288029 pharindoko.cdk-internal-gateway-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-26 20:30:45.288029 pharindoko.cdk-internal-gateway-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:30:45.288029 pharindoko.cdk-internal-gateway-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:45.284029 pharindoko.cdk-internal-gateway-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:45.284029 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:45.288029 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/cdk_internal_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)    41254 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/cdk_internal_gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:45.288029 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/cdk_internal_gateway/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/cdk_internal_gateway/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   185449 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:30:31.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/cdk_internal_gateway/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:45.288029 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-26 20:30:45.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 20:30:45.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:30:45.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 20:30:45.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:30:45.000000 pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/top_level.txt
```

### Comparing `pharindoko.cdk-internal-gateway-1.1.8/LICENSE` & `pharindoko.cdk-internal-gateway-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pharindoko.cdk-internal-gateway-1.1.8/PKG-INFO` & `pharindoko.cdk-internal-gateway-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharindoko.cdk-internal-gateway
-Version: 1.1.8
+Version: 1.1.9
 Summary: CDK construct to create to create internal serverless applications.
 Home-page: https://github.com/pharindoko/cdk-internal-gateway.git
 Author: Florian Fuß
 License: Apache-2.0
 Project-URL: Source, https://github.com/pharindoko/cdk-internal-gateway.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pharindoko.cdk-internal-gateway-1.1.8/README.md` & `pharindoko.cdk-internal-gateway-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pharindoko.cdk-internal-gateway-1.1.8/setup.py` & `pharindoko.cdk-internal-gateway-1.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pharindoko.cdk-internal-gateway",
-    "version": "1.1.8",
+    "version": "1.1.9",
     "description": "CDK construct to create to create internal serverless applications.",
     "license": "Apache-2.0",
     "url": "https://github.com/pharindoko/cdk-internal-gateway.git",
     "long_description_content_type": "text/markdown",
     "author": "Florian Fuß",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pharindoko.cdk_internal_gateway",
         "pharindoko.cdk_internal_gateway._jsii"
     ],
     "package_data": {
         "pharindoko.cdk_internal_gateway._jsii": [
-            "cdk-internal-gateway@1.1.8.jsii.tgz"
+            "cdk-internal-gateway@1.1.9.jsii.tgz"
         ],
         "pharindoko.cdk_internal_gateway": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko/cdk_internal_gateway/__init__.py` & `pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko/cdk_internal_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO` & `pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharindoko.cdk-internal-gateway
-Version: 1.1.8
+Version: 1.1.9
 Summary: CDK construct to create to create internal serverless applications.
 Home-page: https://github.com/pharindoko/cdk-internal-gateway.git
 Author: Florian Fuß
 License: Apache-2.0
 Project-URL: Source, https://github.com/pharindoko/cdk-internal-gateway.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pharindoko.cdk-internal-gateway-1.1.8/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt` & `pharindoko.cdk-internal-gateway-1.1.9/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt
 src/pharindoko.cdk_internal_gateway.egg-info/dependency_links.txt
 src/pharindoko.cdk_internal_gateway.egg-info/requires.txt
 src/pharindoko.cdk_internal_gateway.egg-info/top_level.txt
 src/pharindoko/cdk_internal_gateway/__init__.py
 src/pharindoko/cdk_internal_gateway/py.typed
 src/pharindoko/cdk_internal_gateway/_jsii/__init__.py
-src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.1.8.jsii.tgz
+src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.1.9.jsii.tgz
```


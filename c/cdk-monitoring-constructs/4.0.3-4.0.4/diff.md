# Comparing `tmp/cdk-monitoring-constructs-4.0.3.tar.gz` & `tmp/cdk-monitoring-constructs-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-monitoring-constructs-4.0.3.tar", last modified: Mon May  1 00:36:17 2023, max compression
+gzip compressed data, was "cdk-monitoring-constructs-4.0.4.tar", last modified: Mon May  8 00:36:31 2023, max compression
```

## Comparing `cdk-monitoring-constructs-4.0.3.tar` & `cdk-monitoring-constructs-4.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:17.460001 cdk-monitoring-constructs-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-05-01 00:36:17.460001 cdk-monitoring-constructs-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 00:36:17.460001 cdk-monitoring-constructs-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:17.452001 cdk-monitoring-constructs-4.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:17.456001 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)  4426122 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:17.460001 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   769397 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@4.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:36:03.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:17.456001 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-05-01 00:36:17.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-01 00:36:17.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:36:17.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-01 00:36:17.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 00:36:17.000000 cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:36:31.106496 cdk-monitoring-constructs-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-05-08 00:36:31.106496 cdk-monitoring-constructs-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 00:36:31.106496 cdk-monitoring-constructs-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:36:31.098496 cdk-monitoring-constructs-4.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:36:31.102496 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)  4426122 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:36:31.106496 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   769397 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@4.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:36:17.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:36:31.106496 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-05-08 00:36:31.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 00:36:31.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:36:31.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 00:36:31.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 00:36:31.000000 cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/top_level.txt
```

### Comparing `cdk-monitoring-constructs-4.0.3/LICENSE` & `cdk-monitoring-constructs-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-4.0.3/PKG-INFO` & `cdk-monitoring-constructs-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 4.0.3
+Version: 4.0.4
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-4.0.3/README.md` & `cdk-monitoring-constructs-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-4.0.3/setup.py` & `cdk-monitoring-constructs-4.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-monitoring-constructs",
-    "version": "4.0.3",
+    "version": "4.0.4",
     "description": "cdk-monitoring-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-monitoring-constructs",
     "long_description_content_type": "text/markdown",
     "author": "CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_monitoring_constructs",
         "cdk_monitoring_constructs._jsii"
     ],
     "package_data": {
         "cdk_monitoring_constructs._jsii": [
-            "cdk-monitoring-constructs@4.0.3.jsii.tgz"
+            "cdk-monitoring-constructs@4.0.4.jsii.tgz"
         ],
         "cdk_monitoring_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/__init__.py` & `cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs/_jsii/__init__.py` & `cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs/_jsii/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_redshift_alpha._jsii
 import aws_cdk.aws_synthetics_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-monitoring-constructs",
-    "4.0.3",
+    "4.0.4",
     __name__[0:-6],
-    "cdk-monitoring-constructs@4.0.3.jsii.tgz",
+    "cdk-monitoring-constructs@4.0.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/PKG-INFO` & `cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 4.0.3
+Version: 4.0.4
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-4.0.3/src/cdk_monitoring_constructs.egg-info/SOURCES.txt` & `cdk-monitoring-constructs-4.0.4/src/cdk_monitoring_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_monitoring_constructs/py.typed
 src/cdk_monitoring_constructs.egg-info/PKG-INFO
 src/cdk_monitoring_constructs.egg-info/SOURCES.txt
 src/cdk_monitoring_constructs.egg-info/dependency_links.txt
 src/cdk_monitoring_constructs.egg-info/requires.txt
 src/cdk_monitoring_constructs.egg-info/top_level.txt
 src/cdk_monitoring_constructs/_jsii/__init__.py
-src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@4.0.3.jsii.tgz
+src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@4.0.4.jsii.tgz
```


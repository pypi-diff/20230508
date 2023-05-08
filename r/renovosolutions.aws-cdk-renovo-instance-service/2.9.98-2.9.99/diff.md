# Comparing `tmp/renovosolutions.aws-cdk-renovo-instance-service-2.9.98.tar.gz` & `tmp/renovosolutions.aws-cdk-renovo-instance-service-2.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-renovo-instance-service-2.9.98.tar", last modified: Thu Feb  9 13:46:23 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-renovo-instance-service-2.9.99.tar", last modified: Wed Feb 15 14:16:34 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98.tar` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:46:23.812142 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-09 13:46:23.812142 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 13:46:23.812142 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:46:23.812142 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:46:23.812142 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/
--rw-r--r--   0 runner    (1001) docker     (123)    40125 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:46:23.812142 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31535 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/_jsii/cdk-library-renovo-instance-service@2.9.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 13:46:10.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:46:23.812142 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-09 13:46:23.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-09 13:46:23.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 13:46:23.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-09 13:46:23.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-09 13:46:23.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:16:34.391651 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-15 14:16:34.391651 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 14:16:34.391651 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:16:34.387651 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:16:34.391651 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/
+-rw-r--r--   0 runner    (1001) docker     (123)    40125 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:16:34.391651 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31536 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/_jsii/cdk-library-renovo-instance-service@2.9.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 14:16:21.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:16:34.391651 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-15 14:16:33.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-15 14:16:34.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 14:16:33.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-15 14:16:34.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-15 14:16:34.000000 renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98/LICENSE` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98/PKG-INFO` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-renovo-instance-service
-Version: 2.9.98
+Version: 2.9.99
 Summary: CDK Construct Library to create instance based services utilizing default configurations for Renovo Solutions.
 Home-page: https://github.com/RenovoSolutions/cdk-library-renovo-instance-service.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-renovo-instance-service.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98/setup.py` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-renovo-instance-service",
-    "version": "2.9.98",
+    "version": "2.9.99",
     "description": "CDK Construct Library to create instance based services utilizing default configurations for Renovo Solutions.",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-renovo-instance-service.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "renovo-instance-service",
         "renovo-instance-service._jsii"
     ],
     "package_data": {
         "renovo-instance-service._jsii": [
-            "cdk-library-renovo-instance-service@2.9.98.jsii.tgz"
+            "cdk-library-renovo-instance-service@2.9.99.jsii.tgz"
         ],
         "renovo-instance-service": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/__init__.py` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovo-instance-service/_jsii/__init__.py` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovo-instance-service/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aspects-security-group._jsii
 import aws_cdk._jsii
 import constructs._jsii
 import managed_instance_role._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@renovosolutions/cdk-library-renovo-instance-service",
-    "2.9.98",
+    "2.9.99",
     __name__[0:-6],
-    "cdk-library-renovo-instance-service@2.9.98.jsii.tgz",
+    "cdk-library-renovo-instance-service@2.9.99.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-renovo-instance-service
-Version: 2.9.98
+Version: 2.9.99
 Summary: CDK Construct Library to create instance based services utilizing default configurations for Renovo Solutions.
 Home-page: https://github.com/RenovoSolutions/cdk-library-renovo-instance-service.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-renovo-instance-service.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-renovo-instance-service-2.9.98/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-renovo-instance-service-2.9.99/src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/renovo-instance-service/__init__.py
 src/renovo-instance-service/py.typed
 src/renovo-instance-service/_jsii/__init__.py
-src/renovo-instance-service/_jsii/cdk-library-renovo-instance-service@2.9.98.jsii.tgz
+src/renovo-instance-service/_jsii/cdk-library-renovo-instance-service@2.9.99.jsii.tgz
 src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/requires.txt
 src/renovosolutions.aws_cdk_renovo_instance_service.egg-info/top_level.txt
```


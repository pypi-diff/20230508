# Comparing `tmp/renovosolutions.aws-cdk-managed-instance-role-2.3.98.tar.gz` & `tmp/renovosolutions.aws-cdk-managed-instance-role-2.3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-managed-instance-role-2.3.98.tar", last modified: Mon Apr 17 13:25:19 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-managed-instance-role-2.3.99.tar", last modified: Mon May  1 12:42:24 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98.tar` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.548142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-17 13:25:19.548142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:25:19.548142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:42:24.780617 renovosolutions.aws-cdk-managed-instance-role-2.3.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-01 12:42:24.780617 renovosolutions.aws-cdk-managed-instance-role-2.3.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 12:42:24.780617 renovosolutions.aws-cdk-managed-instance-role-2.3.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:42:24.776617 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:42:24.780617 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/managed_instance_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/managed_instance_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:42:24.780617 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/managed_instance_role/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/managed_instance_role/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:42:01.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/managed_instance_role/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:42:24.780617 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-01 12:42:24.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 12:42:24.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:42:24.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 12:42:24.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 12:42:24.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98/LICENSE` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98/PKG-INFO` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-managed-instance-role
-Version: 2.3.98
+Version: 2.3.99
 Summary: AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.
 Home-page: https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98/README.md` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98/setup.py` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-managed-instance-role",
-    "version": "2.3.98",
+    "version": "2.3.99",
     "description": "AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "managed_instance_role",
         "managed_instance_role._jsii"
     ],
     "package_data": {
         "managed_instance_role._jsii": [
-            "cdk-library-managed-instance-role@2.3.98.jsii.tgz"
+            "cdk-library-managed-instance-role@2.3.99.jsii.tgz"
         ],
         "managed_instance_role": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/__init__.py` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/managed_instance_role/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-managed-instance-role
-Version: 2.3.98
+Version: 2.3.99
 Summary: AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.
 Home-page: https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-managed-instance-role-2.3.99/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/managed_instance_role/__init__.py
 src/managed_instance_role/py.typed
 src/managed_instance_role/_jsii/__init__.py
-src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.98.jsii.tgz
+src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.99.jsii.tgz
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
```


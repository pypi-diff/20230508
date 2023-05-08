# Comparing `tmp/renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8.tar.gz` & `tmp/renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8.tar", last modified: Mon Dec 19 14:10:12 2022, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9.tar", last modified: Mon Dec 19 14:59:46 2022, max compression
```

## Comparing `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8.tar` & `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:10:12.017686 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-19 14:10:12.017686 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 14:10:12.017686 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:10:12.013686 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:10:12.017686 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/multi_account_az_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/multi_account_az_mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:10:12.017686 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/multi_account_az_mapping/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/multi_account_az_mapping/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/multi_account_az_mapping/_jsii/cdk-library-multi-account-az-mapping@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 14:09:52.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/multi_account_az_mapping/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:10:12.017686 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-19 14:10:11.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-19 14:10:11.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 14:10:11.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-19 14:10:11.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-19 14:10:11.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:59:46.479361 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-19 14:59:46.479361 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 14:59:46.479361 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:59:46.475361 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:59:46.475361 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/multi_account_az_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/multi_account_az_mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:59:46.479361 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/multi_account_az_mapping/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/multi_account_az_mapping/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/multi_account_az_mapping/_jsii/cdk-library-multi-account-az-mapping@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 14:59:33.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/multi_account_az_mapping/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 14:59:46.479361 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-19 14:59:45.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-19 14:59:46.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 14:59:45.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-19 14:59:46.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-19 14:59:46.000000 renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/LICENSE` & `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/PKG-INFO` & `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-multi-account-az-mapping
-Version: 0.0.8
+Version: 0.0.9
 Summary: AWS CDK Construct Library to map zone-ids to zone-names to support multi-account zonal consistency for VPCs
 Home-page: https://github.com/RenovoSolutions/cdk-library-multi-account-az-mapping.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-multi-account-az-mapping.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/setup.py` & `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-multi-account-az-mapping",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "AWS CDK Construct Library to map zone-ids to zone-names to support multi-account zonal consistency for VPCs",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-multi-account-az-mapping.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "multi_account_az_mapping",
         "multi_account_az_mapping._jsii"
     ],
     "package_data": {
         "multi_account_az_mapping._jsii": [
-            "cdk-library-multi-account-az-mapping@0.0.8.jsii.tgz"
+            "cdk-library-multi-account-az-mapping@0.0.9.jsii.tgz"
         ],
         "multi_account_az_mapping": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/multi_account_az_mapping/__init__.py` & `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/multi_account_az_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-multi-account-az-mapping
-Version: 0.0.8
+Version: 0.0.9
 Summary: AWS CDK Construct Library to map zone-ids to zone-names to support multi-account zonal consistency for VPCs
 Home-page: https://github.com/RenovoSolutions/cdk-library-multi-account-az-mapping.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-multi-account-az-mapping.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.8/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-multi-account-az-mapping-0.0.9/src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/multi_account_az_mapping/__init__.py
 src/multi_account_az_mapping/py.typed
 src/multi_account_az_mapping/_jsii/__init__.py
-src/multi_account_az_mapping/_jsii/cdk-library-multi-account-az-mapping@0.0.8.jsii.tgz
+src/multi_account_az_mapping/_jsii/cdk-library-multi-account-az-mapping@0.0.9.jsii.tgz
 src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/requires.txt
 src/renovosolutions.aws_cdk_multi_account_az_mapping.egg-info/top_level.txt
```


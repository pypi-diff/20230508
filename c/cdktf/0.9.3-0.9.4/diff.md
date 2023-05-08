# Comparing `tmp/cdktf-0.9.3.tar.gz` & `tmp/cdktf-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/terraform-cdk/terraform-cdk/packages/cdktf/dist/python/cdktf-0.9.3.tar", last modified: Thu Feb 24 12:56:24 2022, max compression
+gzip compressed data, was "/__w/terraform-cdk/terraform-cdk/packages/cdktf/dist/python/cdktf-0.9.4.tar", last modified: Thu Feb 24 15:50:02 2022, max compression
```

## Comparing `cdktf-0.9.3.tar` & `cdktf-0.9.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 12:56:24.000000 cdktf-0.9.3/
--rw-r--r--   0 root         (0) root         (0)    15176 2022-02-24 12:56:13.000000 cdktf-0.9.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-02-24 12:56:13.000000 cdktf-0.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1159 2022-02-24 12:56:24.000000 cdktf-0.9.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2022-02-24 12:56:13.000000 cdktf-0.9.3/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-02-24 12:56:13.000000 cdktf-0.9.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-24 12:56:24.000000 cdktf-0.9.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1604 2022-02-24 12:56:13.000000 cdktf-0.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf/
--rw-r--r--   0 root         (0) root         (0)   541369 2022-02-24 12:56:13.000000 cdktf-0.9.3/src/cdktf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf/_jsii/
--rw-r--r--   0 root         (0) root         (0)      322 2022-02-24 12:56:13.000000 cdktf-0.9.3/src/cdktf/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   771860 2022-02-24 12:56:13.000000 cdktf-0.9.3/src/cdktf/_jsii/cdktf@0.9.3.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-24 12:56:13.000000 cdktf-0.9.3/src/cdktf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf/testing_matchers/
--rw-r--r--   0 root         (0) root         (0)     1385 2022-02-24 12:56:13.000000 cdktf-0.9.3/src/cdktf/testing_matchers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1159 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      362 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-02-24 12:56:24.000000 cdktf-0.9.3/src/cdktf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 15:50:02.000000 cdktf-0.9.4/
+-rw-r--r--   0 root         (0) root         (0)    15176 2022-02-24 15:49:51.000000 cdktf-0.9.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-02-24 15:49:51.000000 cdktf-0.9.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1159 2022-02-24 15:50:02.000000 cdktf-0.9.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2022-02-24 15:49:51.000000 cdktf-0.9.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-02-24 15:49:51.000000 cdktf-0.9.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-02-24 15:50:02.000000 cdktf-0.9.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1604 2022-02-24 15:49:51.000000 cdktf-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf/
+-rw-r--r--   0 root         (0) root         (0)   541369 2022-02-24 15:49:51.000000 cdktf-0.9.4/src/cdktf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      322 2022-02-24 15:49:51.000000 cdktf-0.9.4/src/cdktf/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   771907 2022-02-24 15:49:51.000000 cdktf-0.9.4/src/cdktf/_jsii/cdktf@0.9.4.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-24 15:49:51.000000 cdktf-0.9.4/src/cdktf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf/testing_matchers/
+-rw-r--r--   0 root         (0) root         (0)     1385 2022-02-24 15:49:51.000000 cdktf-0.9.4/src/cdktf/testing_matchers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1159 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      362 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-02-24 15:50:02.000000 cdktf-0.9.4/src/cdktf.egg-info/top_level.txt
```

### Comparing `cdktf-0.9.3/LICENSE` & `cdktf-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-0.9.3/PKG-INFO` & `cdktf-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf
-Version: 0.9.3
+Version: 0.9.4
 Summary: Cloud Development Kit for Terraform
 Home-page: https://github.com/hashicorp/terraform-cdk
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/hashicorp/terraform-cdk.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdktf-0.9.3/setup.py` & `cdktf-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf",
-    "version": "0.9.3",
+    "version": "0.9.4",
     "description": "Cloud Development Kit for Terraform",
     "license": "MPL-2.0",
     "url": "https://github.com/hashicorp/terraform-cdk",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "cdktf",
         "cdktf._jsii",
         "cdktf.testing_matchers"
     ],
     "package_data": {
         "cdktf._jsii": [
-            "cdktf@0.9.3.jsii.tgz"
+            "cdktf@0.9.4.jsii.tgz"
         ],
         "cdktf": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `cdktf-0.9.3/src/cdktf/__init__.py` & `cdktf-0.9.4/src/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-0.9.3/src/cdktf/testing_matchers/__init__.py` & `cdktf-0.9.4/src/cdktf/testing_matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-0.9.3/src/cdktf.egg-info/PKG-INFO` & `cdktf-0.9.4/src/cdktf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf
-Version: 0.9.3
+Version: 0.9.4
 Summary: Cloud Development Kit for Terraform
 Home-page: https://github.com/hashicorp/terraform-cdk
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/hashicorp/terraform-cdk.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


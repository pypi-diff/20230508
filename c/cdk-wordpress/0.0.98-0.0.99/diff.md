# Comparing `tmp/cdk-wordpress-0.0.98.tar.gz` & `tmp/cdk-wordpress-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-wordpress/cdk-wordpress/dist/python/cdk-wordpress-0.0.98.tar", last modified: Fri Oct 22 00:50:03 2021, max compression
+gzip compressed data, was "/__w/cdk-wordpress/cdk-wordpress/dist/python/cdk-wordpress-0.0.99.tar", last modified: Tue Oct 26 00:44:24 2021, max compression
```

## Comparing `cdk-wordpress-0.0.98.tar` & `cdk-wordpress-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/
--rw-r--r--   0 root         (0) root         (0)    11358 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1862 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      965 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1912 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress/
--rw-r--r--   0 root         (0) root         (0)     4364 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/src/cdk_wordpress/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress/_jsii/
--rw-r--r--   0 root         (0) root         (0)      520 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/src/cdk_wordpress/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16648 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/src/cdk_wordpress/_jsii/cdk-wordpress@0.0.98.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-22 00:49:58.000000 cdk-wordpress-0.0.98/src/cdk_wordpress/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1862 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      257 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-10-22 00:50:03.000000 cdk-wordpress-0.0.98/src/cdk_wordpress.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)    11358 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1862 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      965 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1912 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress/
+-rw-r--r--   0 root         (0) root         (0)     4364 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/src/cdk_wordpress/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      520 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/src/cdk_wordpress/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16648 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/src/cdk_wordpress/_jsii/cdk-wordpress@0.0.99.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-26 00:44:19.000000 cdk-wordpress-0.0.99/src/cdk_wordpress/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1862 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      404 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      257 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-10-26 00:44:24.000000 cdk-wordpress-0.0.99/src/cdk_wordpress.egg-info/top_level.txt
```

### Comparing `cdk-wordpress-0.0.98/LICENSE` & `cdk-wordpress-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-wordpress-0.0.98/PKG-INFO` & `cdk-wordpress-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-wordpress
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-wordpress
 Home-page: https://github.com/clarencetw/cdk-wordpress.git
 Author: Clarence Lin<mr.lin.clarence@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/clarencetw/cdk-wordpress.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-wordpress-0.0.98/README.md` & `cdk-wordpress-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-wordpress-0.0.98/setup.py` & `cdk-wordpress-0.0.99/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-wordpress",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "cdk-wordpress",
     "license": "Apache-2.0",
     "url": "https://github.com/clarencetw/cdk-wordpress.git",
     "long_description_content_type": "text/markdown",
     "author": "Clarence Lin<mr.lin.clarence@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_wordpress",
         "cdk_wordpress._jsii"
     ],
     "package_data": {
         "cdk_wordpress._jsii": [
-            "cdk-wordpress@0.0.98.jsii.tgz"
+            "cdk-wordpress@0.0.99.jsii.tgz"
         ],
         "cdk_wordpress": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `cdk-wordpress-0.0.98/src/cdk_wordpress/__init__.py` & `cdk-wordpress-0.0.99/src/cdk_wordpress/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-wordpress-0.0.98/src/cdk_wordpress/_jsii/__init__.py` & `cdk-wordpress-0.0.99/src/cdk_wordpress/_jsii/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import aws_cdk.aws_ecs_patterns._jsii
 import aws_cdk.aws_efs._jsii
 import aws_cdk.aws_rds._jsii
 import aws_cdk.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "cdk-wordpress", "0.0.98", __name__[0:-6], "cdk-wordpress@0.0.98.jsii.tgz"
+    "cdk-wordpress", "0.0.99", __name__[0:-6], "cdk-wordpress@0.0.99.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-wordpress-0.0.98/src/cdk_wordpress.egg-info/PKG-INFO` & `cdk-wordpress-0.0.99/src/cdk_wordpress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-wordpress
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-wordpress
 Home-page: https://github.com/clarencetw/cdk-wordpress.git
 Author: Clarence Lin<mr.lin.clarence@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/clarencetw/cdk-wordpress.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


# Comparing `tmp/cdk-sns-notify-0.0.98.tar.gz` & `tmp/cdk-sns-notify-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-sns-notify/cdk-sns-notify/dist/python/cdk-sns-notify-0.0.98.tar", last modified: Sun Nov 28 00:30:26 2021, max compression
+gzip compressed data, was "/__w/cdk-sns-notify/cdk-sns-notify/dist/python/cdk-sns-notify-0.0.99.tar", last modified: Thu Dec  2 00:30:27 2021, max compression
```

## Comparing `cdk-sns-notify-0.0.98.tar` & `cdk-sns-notify-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/
--rw-r--r--   0 root         (0) root         (0)    11358 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2116 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2086 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify/
--rw-r--r--   0 root         (0) root         (0)     3389 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify/_jsii/
--rw-r--r--   0 root         (0) root         (0)      649 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16497 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify/_jsii/cdk-sns-notify@0.0.98.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-28 00:30:21.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2116 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-11-28 00:30:26.000000 cdk-sns-notify-0.0.98/src/cdk_sns_notify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)    11358 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2116 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1219 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2086 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify/
+-rw-r--r--   0 root         (0) root         (0)     3389 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      649 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16492 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify/_jsii/cdk-sns-notify@0.0.99.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-02 00:30:23.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2116 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2021-12-02 00:30:27.000000 cdk-sns-notify-0.0.99/src/cdk_sns_notify.egg-info/top_level.txt
```

### Comparing `cdk-sns-notify-0.0.98/LICENSE` & `cdk-sns-notify-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sns-notify-0.0.98/PKG-INFO` & `cdk-sns-notify-0.0.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sns-notify
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-sns-notify
 Home-page: https://github.com/clarencetw/cdk-sns-notify.git
 Author: Clarence<mr.lin.clarence@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/clarencetw/cdk-sns-notify.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-sns-notify-0.0.98/README.md` & `cdk-sns-notify-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sns-notify-0.0.98/setup.py` & `cdk-sns-notify-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sns-notify",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "cdk-sns-notify",
     "license": "Apache-2.0",
     "url": "https://github.com/clarencetw/cdk-sns-notify.git",
     "long_description_content_type": "text/markdown",
     "author": "Clarence<mr.lin.clarence@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_sns_notify",
         "cdk_sns_notify._jsii"
     ],
     "package_data": {
         "cdk_sns_notify._jsii": [
-            "cdk-sns-notify@0.0.98.jsii.tgz"
+            "cdk-sns-notify@0.0.99.jsii.tgz"
         ],
         "cdk_sns_notify": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `cdk-sns-notify-0.0.98/src/cdk_sns_notify/__init__.py` & `cdk-sns-notify-0.0.99/src/cdk_sns_notify/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-sns-notify-0.0.98/src/cdk_sns_notify/_jsii/__init__.py` & `cdk-sns-notify-0.0.99/src/cdk_sns_notify/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import aws_cdk.aws_lambda_nodejs._jsii
 import aws_cdk.aws_sns._jsii
 import aws_cdk.aws_sns_subscriptions._jsii
 import aws_cdk.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "cdk-sns-notify", "0.0.98", __name__[0:-6], "cdk-sns-notify@0.0.98.jsii.tgz"
+    "cdk-sns-notify", "0.0.99", __name__[0:-6], "cdk-sns-notify@0.0.99.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-sns-notify-0.0.98/src/cdk_sns_notify.egg-info/PKG-INFO` & `cdk-sns-notify-0.0.99/src/cdk_sns_notify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sns-notify
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-sns-notify
 Home-page: https://github.com/clarencetw/cdk-sns-notify.git
 Author: Clarence<mr.lin.clarence@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/clarencetw/cdk-sns-notify.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


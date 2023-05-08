# Comparing `tmp/cdklabs.appsync-utils-0.0.82.tar.gz` & `tmp/cdklabs.appsync-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.appsync-utils-0.0.82.tar", last modified: Mon May  8 00:16:20 2023, max compression
+gzip compressed data, was "cdklabs.appsync-utils-0.0.9.tar", last modified: Thu Feb 23 17:08:51 2023, max compression
```

## Comparing `cdklabs.appsync-utils-0.0.82.tar` & `cdklabs.appsync-utils-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/src/awscdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/src/awscdk/appsync_utils/
--rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/src/awscdk/appsync_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/src/awscdk/appsync_utils/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/src/awscdk/appsync_utils/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82437 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.82.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:16:09.000000 cdklabs.appsync-utils-0.0.82/src/awscdk/appsync_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:16:20.588842 cdklabs.appsync-utils-0.0.82/src/cdklabs.appsync_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-08 00:16:20.000000 cdklabs.appsync-utils-0.0.82/src/cdklabs.appsync_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 00:16:20.000000 cdklabs.appsync-utils-0.0.82/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:16:20.000000 cdklabs.appsync-utils-0.0.82/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 00:16:20.000000 cdklabs.appsync-utils-0.0.82/src/cdklabs.appsync_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 00:16:20.000000 cdklabs.appsync-utils-0.0.82/src/cdklabs.appsync_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:08:51.241582 cdklabs.appsync-utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-02-23 17:08:51.241582 cdklabs.appsync-utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 17:08:51.241582 cdklabs.appsync-utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:08:51.241582 cdklabs.appsync-utils-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:08:51.237581 cdklabs.appsync-utils-0.0.9/src/awscdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:08:51.241582 cdklabs.appsync-utils-0.0.9/src/awscdk/appsync_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/src/awscdk/appsync_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:08:51.241582 cdklabs.appsync-utils-0.0.9/src/awscdk/appsync_utils/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/src/awscdk/appsync_utils/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78736 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:08:38.000000 cdklabs.appsync-utils-0.0.9/src/awscdk/appsync_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:08:51.241582 cdklabs.appsync-utils-0.0.9/src/cdklabs.appsync_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-02-23 17:08:51.000000 cdklabs.appsync-utils-0.0.9/src/cdklabs.appsync_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-23 17:08:51.000000 cdklabs.appsync-utils-0.0.9/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:08:51.000000 cdklabs.appsync-utils-0.0.9/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-23 17:08:51.000000 cdklabs.appsync-utils-0.0.9/src/cdklabs.appsync_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-23 17:08:51.000000 cdklabs.appsync-utils-0.0.9/src/cdklabs.appsync_utils.egg-info/top_level.txt
```

### Comparing `cdklabs.appsync-utils-0.0.82/LICENSE` & `cdklabs.appsync-utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.82/PKG-INFO` & `cdklabs.appsync-utils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.82
+Version: 0.0.9
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `cdklabs.appsync-utils-0.0.82/README.md` & `cdklabs.appsync-utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.82/setup.py` & `cdklabs.appsync-utils-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.appsync-utils",
-    "version": "0.0.82",
+    "version": "0.0.9",
     "description": "Utilities for creating appsync apis using aws-cdk",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/awscdk-appsync-utils.git",
     "long_description_content_type": "text/markdown",
     "author": "Mitchell Valine<mitchellvaline@yahoo.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,38 +22,37 @@
     },
     "packages": [
         "awscdk.appsync_utils",
         "awscdk.appsync_utils._jsii"
     ],
     "package_data": {
         "awscdk.appsync_utils._jsii": [
-            "awscdk-appsync-utils@0.0.82.jsii.tgz"
+            "awscdk-appsync-utils@0.0.9.jsii.tgz"
         ],
         "awscdk.appsync_utils": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.60.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.75.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdklabs.appsync-utils-0.0.82/src/awscdk/appsync_utils/__init__.py` & `cdklabs.appsync-utils-0.0.9/src/awscdk/appsync_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.82/src/cdklabs.appsync_utils.egg-info/PKG-INFO` & `cdklabs.appsync-utils-0.0.9/src/cdklabs.appsync_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.82
+Version: 0.0.9
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```


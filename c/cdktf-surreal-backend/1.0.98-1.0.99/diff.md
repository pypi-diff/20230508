# Comparing `tmp/cdktf-surreal-backend-1.0.98.tar.gz` & `tmp/cdktf-surreal-backend-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-surreal-backend-1.0.98.tar", last modified: Wed May  3 00:18:56 2023, max compression
+gzip compressed data, was "cdktf-surreal-backend-1.0.99.tar", last modified: Thu May  4 00:18:00 2023, max compression
```

## Comparing `cdktf-surreal-backend-1.0.98.tar` & `cdktf-surreal-backend-1.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:18:56.546450 cdktf-surreal-backend-1.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 00:18:56.546450 cdktf-surreal-backend-1.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:18:56.546450 cdktf-surreal-backend-1.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:18:56.542450 cdktf-surreal-backend-1.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:18:56.546450 cdktf-surreal-backend-1.0.98/src/cdktf_surreal-backend/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal-backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:18:56.546450 cdktf-surreal-backend-1.0.98/src/cdktf_surreal-backend/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal-backend/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:18:43.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal-backend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:18:56.546450 cdktf-surreal-backend-1.0.98/src/cdktf_surreal_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 00:18:56.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 00:18:56.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:18:56.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 00:18:56.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 00:18:56.000000 cdktf-surreal-backend-1.0.98/src/cdktf_surreal_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:18:00.910777 cdktf-surreal-backend-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-04 00:18:00.910777 cdktf-surreal-backend-1.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:18:00.910777 cdktf-surreal-backend-1.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:18:00.910777 cdktf-surreal-backend-1.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:18:00.910777 cdktf-surreal-backend-1.0.99/src/cdktf_surreal-backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal-backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:18:00.910777 cdktf-surreal-backend-1.0.99/src/cdktf_surreal-backend/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal-backend/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:17:49.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal-backend/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:18:00.910777 cdktf-surreal-backend-1.0.99/src/cdktf_surreal_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-04 00:18:00.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 00:18:00.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:18:00.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 00:18:00.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 00:18:00.000000 cdktf-surreal-backend-1.0.99/src/cdktf_surreal_backend.egg-info/top_level.txt
```

### Comparing `cdktf-surreal-backend-1.0.98/LICENSE` & `cdktf-surreal-backend-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.98/PKG-INFO` & `cdktf-surreal-backend-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.98
+Version: 1.0.99
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-surreal-backend-1.0.98/README.md` & `cdktf-surreal-backend-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.98/setup.py` & `cdktf-surreal-backend-1.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-surreal-backend",
-    "version": "1.0.98",
+    "version": "1.0.99",
     "description": "A package that vends a construct to setup the surreal backend in CDKTF",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-surreal-backend.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_surreal-backend",
         "cdktf_surreal-backend._jsii"
     ],
     "package_data": {
         "cdktf_surreal-backend._jsii": [
-            "cdktf-surreal-backend@1.0.98.jsii.tgz"
+            "cdktf-surreal-backend@1.0.99.jsii.tgz"
         ],
         "cdktf_surreal-backend": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-surreal-backend-1.0.98/src/cdktf_surreal-backend/__init__.py` & `cdktf-surreal-backend-1.0.99/src/cdktf_surreal-backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.98/src/cdktf_surreal_backend.egg-info/PKG-INFO` & `cdktf-surreal-backend-1.0.99/src/cdktf_surreal_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.98
+Version: 1.0.99
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


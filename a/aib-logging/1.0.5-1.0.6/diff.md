# Comparing `tmp/aib_logging-1.0.5.tar.gz` & `tmp/aib_logging-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-1.0.5.tar", last modified: Mon May  8 05:24:46 2023, max compression
+gzip compressed data, was "aib_logging-1.0.6.tar", last modified: Mon May  8 05:49:09 2023, max compression
```

## Comparing `aib_logging-1.0.5.tar` & `aib_logging-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:24:46.997889 aib_logging-1.0.5/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.5/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-08 05:24:46.996889 aib_logging-1.0.5/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.5/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      635 2023-05-08 05:22:53.000000 aib_logging-1.0.5/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-08 05:24:46.997889 aib_logging-1.0.5/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:24:46.993889 aib_logging-1.0.5/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:24:46.995889 aib_logging-1.0.5/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.5/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14620 2023-05-08 05:21:52.000000 aib_logging-1.0.5/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:24:46.996889 aib_logging-1.0.5/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-08 05:24:46.000000 aib_logging-1.0.5/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-08 05:24:46.000000 aib_logging-1.0.5/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-08 05:24:46.000000 aib_logging-1.0.5/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       26 2023-05-08 05:24:46.000000 aib_logging-1.0.5/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-08 05:24:46.000000 aib_logging-1.0.5/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:49:09.032477 aib_logging-1.0.6/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.6/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-08 05:49:09.032477 aib_logging-1.0.6/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.6/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      623 2023-05-08 05:46:56.000000 aib_logging-1.0.6/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-08 05:49:09.032477 aib_logging-1.0.6/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:49:09.030477 aib_logging-1.0.6/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:49:09.031477 aib_logging-1.0.6/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.6/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14620 2023-05-08 05:21:52.000000 aib_logging-1.0.6/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-08 05:49:09.032477 aib_logging-1.0.6/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-08 05:49:09.000000 aib_logging-1.0.6/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-08 05:49:09.000000 aib_logging-1.0.6/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-08 05:49:09.000000 aib_logging-1.0.6/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       28 2023-05-08 05:49:09.000000 aib_logging-1.0.6/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-08 05:49:09.000000 aib_logging-1.0.6/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-1.0.5/LICENSE.txt` & `aib_logging-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-1.0.5/PKG-INFO` & `aib_logging-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib_logging
-Version: 1.0.5
+Version: 1.0.6
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aib_logging-1.0.5/pyproject.toml` & `aib_logging-1.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-    "google-cloud-logging",
-    "time",
-]
+dependencies = ["google-cloud-logging==3.2.5"]
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `aib_logging-1.0.5/src/aib_logging/logger.py` & `aib_logging-1.0.6/src/aib_logging/logger.py`

 * *Files identical despite different names*

### Comparing `aib_logging-1.0.5/src/aib_logging.egg-info/PKG-INFO` & `aib_logging-1.0.6/src/aib_logging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib-logging
-Version: 1.0.5
+Version: 1.0.6
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


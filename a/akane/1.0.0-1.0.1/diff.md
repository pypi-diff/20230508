# Comparing `tmp/akane-1.0.0.tar.gz` & `tmp/akane-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akane-1.0.0.tar", last modified: Sun May  7 18:56:16 2023, max compression
+gzip compressed data, was "akane-1.0.1.tar", last modified: Mon May  8 06:58:45 2023, max compression
```

## Comparing `akane-1.0.0.tar` & `akane-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:56:16.391522 akane-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 18:56:04.000000 akane-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-07 18:56:16.391522 akane-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-07 18:56:04.000000 akane-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:56:16.391522 akane-1.0.0/akane/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-07 18:56:04.000000 akane-1.0.0/akane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-07 18:56:04.000000 akane-1.0.0/akane/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-07 18:56:04.000000 akane-1.0.0/akane/helpder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-07 18:56:04.000000 akane-1.0.0/akane/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:56:16.391522 akane-1.0.0/akane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-07 18:56:16.000000 akane-1.0.0/akane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-07 18:56:16.000000 akane-1.0.0/akane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:56:16.000000 akane-1.0.0/akane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 18:56:16.000000 akane-1.0.0/akane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 18:56:16.000000 akane-1.0.0/akane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-07 18:56:16.395522 akane-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-07 18:56:04.000000 akane-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:45.338439 akane-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 06:58:29.000000 akane-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-08 06:58:45.338439 akane-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-08 06:58:29.000000 akane-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:45.338439 akane-1.0.1/akane/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-08 06:58:29.000000 akane-1.0.1/akane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-08 06:58:29.000000 akane-1.0.1/akane/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 06:58:29.000000 akane-1.0.1/akane/helpder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-08 06:58:29.000000 akane-1.0.1/akane/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:45.338439 akane-1.0.1/akane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-08 06:58:45.000000 akane-1.0.1/akane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 06:58:45.000000 akane-1.0.1/akane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:58:45.000000 akane-1.0.1/akane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 06:58:45.000000 akane-1.0.1/akane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 06:58:45.000000 akane-1.0.1/akane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 06:58:45.338439 akane-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-08 06:58:29.000000 akane-1.0.1/setup.py
```

### Comparing `akane-1.0.0/LICENSE` & `akane-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `akane-1.0.0/PKG-INFO` & `akane-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akane
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple, stronly typed library to create tests for anything
 Home-page: https://github.com/zekrotja/akane
 Download-URL: https://github.com/zekrotja/akane/archive/main.tar.gz
 Author: zekro
 Author-email: contact@zekro.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akane-1.0.0/README.md` & `akane-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `akane-1.0.0/akane/assertions.py` & `akane-1.0.1/akane/assertions.py`

 * *Files identical despite different names*

### Comparing `akane-1.0.0/akane/procedures.py` & `akane-1.0.1/akane/procedures.py`

 * *Files identical despite different names*

### Comparing `akane-1.0.0/akane.egg-info/PKG-INFO` & `akane-1.0.1/akane.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akane
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple, stronly typed library to create tests for anything
 Home-page: https://github.com/zekrotja/akane
 Download-URL: https://github.com/zekrotja/akane/archive/main.tar.gz
 Author: zekro
 Author-email: contact@zekro.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akane-1.0.0/setup.py` & `akane-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import setuptools
 
 with open('README.md', encoding='utf-8') as f:
     long_desc = f.read()
 
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
+requirements = ["rich"]
 
 setuptools.setup(
-    version="1.0.0",
+    version="1.0.1",
     name="akane",
     author="zekro",
     author_email="contact@zekro.de",
     description="Simple, stronly typed library to create tests for anything",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/zekrotja/akane",
```


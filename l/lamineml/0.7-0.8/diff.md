# Comparing `tmp/lamineml-0.7.tar.gz` & `tmp/lamineml-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.7.tar", last modified: Sun Jan  8 15:42:55 2023, max compression
+gzip compressed data, was "lamineml-0.8.tar", last modified: Sun Jan  8 15:50:45 2023, max compression
```

## Comparing `lamineml-0.7.tar` & `lamineml-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:42:55.391121 lamineml-0.7/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.7/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-01-08 15:42:55.391121 lamineml-0.7/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.7/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      144 2023-01-08 15:38:13.000000 lamineml-0.7/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      612 2023-01-08 15:42:55.391121 lamineml-0.7/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:42:55.387121 lamineml-0.7/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:42:55.387121 lamineml-0.7/src/lamineml/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-01-08 14:42:04.000000 lamineml-0.7/src/lamineml/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)      311 2023-01-08 15:41:39.000000 lamineml-0.7/src/lamineml/run.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:42:55.391121 lamineml-0.7/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-01-08 15:42:55.000000 lamineml-0.7/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      231 2023-01-08 15:42:55.000000 lamineml-0.7/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-01-08 15:42:55.000000 lamineml-0.7/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        9 2023-01-08 15:42:55.000000 lamineml-0.7/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:50:45.133660 lamineml-0.8/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.8/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-01-08 15:50:45.133660 lamineml-0.8/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.8/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      144 2023-01-08 15:38:13.000000 lamineml-0.8/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      612 2023-01-08 15:50:45.133660 lamineml-0.8/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:50:45.129660 lamineml-0.8/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:50:45.129660 lamineml-0.8/src/lamineml/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-01-08 14:42:04.000000 lamineml-0.8/src/lamineml/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)      355 2023-01-08 15:49:19.000000 lamineml-0.8/src/lamineml/browser.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-01-08 15:50:45.129660 lamineml-0.8/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-01-08 15:50:45.000000 lamineml-0.8/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      235 2023-01-08 15:50:45.000000 lamineml-0.8/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-01-08 15:50:45.000000 lamineml-0.8/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        9 2023-01-08 15:50:45.000000 lamineml-0.8/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.7/PKG-INFO` & `lamineml-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.7
+Version: 0.8
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Brad
 Author-email: devopswithbrad@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.7/README.md` & `lamineml-0.8/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.7/setup.cfg` & `lamineml-0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.7
+version = 0.8
 author = Brad
 author_email = devopswithbrad@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.7/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.8/src/lamineml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.7
+Version: 0.8
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Brad
 Author-email: devopswithbrad@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


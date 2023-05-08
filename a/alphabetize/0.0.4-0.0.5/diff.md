# Comparing `tmp/alphabetize-0.0.4.tar.gz` & `tmp/alphabetize-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphabetize-0.0.4.tar", last modified: Mon May  8 11:56:20 2023, max compression
+gzip compressed data, was "alphabetize-0.0.5.tar", last modified: Mon May  8 12:06:41 2023, max compression
```

## Comparing `alphabetize-0.0.4.tar` & `alphabetize-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 11:56:20.527345 alphabetize-0.0.4/
--rw-rw-rw-   0        0        0     1087 2023-05-08 10:43:11.000000 alphabetize-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1231 2023-05-08 11:56:20.527345 alphabetize-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-05-08 08:35:05.000000 alphabetize-0.0.4/README.md
--rw-rw-rw-   0        0        0       88 2023-05-08 10:27:09.000000 alphabetize-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1240 2023-05-08 11:56:20.534389 alphabetize-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1563 2023-05-08 11:56:01.000000 alphabetize-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:56:20.492580 alphabetize-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 11:56:20.526333 alphabetize-0.0.4/src/alphabetize.egg-info/
--rw-rw-rw-   0        0        0     1231 2023-05-08 11:56:20.000000 alphabetize-0.0.4/src/alphabetize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-08 11:56:20.000000 alphabetize-0.0.4/src/alphabetize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:56:20.000000 alphabetize-0.0.4/src/alphabetize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-08 11:56:20.000000 alphabetize-0.0.4/src/alphabetize.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 11:56:20.000000 alphabetize-0.0.4/src/alphabetize.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:56:20.000000 alphabetize-0.0.4/src/alphabetize.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 12:06:41.440414 alphabetize-0.0.5/
+-rw-rw-rw-   0        0        0       94 2023-05-08 10:10:51.000000 alphabetize-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1087 2023-05-08 10:43:11.000000 alphabetize-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:05:31.000000 alphabetize-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1231 2023-05-08 12:06:41.440414 alphabetize-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2023-05-08 08:35:05.000000 alphabetize-0.0.5/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-08 10:27:09.000000 alphabetize-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1240 2023-05-08 12:06:41.447414 alphabetize-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1563 2023-05-08 12:06:15.000000 alphabetize-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:06:41.415825 alphabetize-0.0.5/src/
+-rw-rw-rw-   0        0        0        0 2023-05-08 10:45:55.000000 alphabetize-0.0.5/src/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-08 11:55:44.000000 alphabetize-0.0.5/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:06:41.439414 alphabetize-0.0.5/src/alphabetize.egg-info/
+-rw-rw-rw-   0        0        0     1231 2023-05-08 12:06:41.000000 alphabetize-0.0.5/src/alphabetize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-05-08 12:06:41.000000 alphabetize-0.0.5/src/alphabetize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:06:41.000000 alphabetize-0.0.5/src/alphabetize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-08 12:06:41.000000 alphabetize-0.0.5/src/alphabetize.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 12:06:41.000000 alphabetize-0.0.5/src/alphabetize.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:06:41.000000 alphabetize-0.0.5/src/alphabetize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2682 2023-05-08 10:50:08.000000 alphabetize-0.0.5/src/alphabetize.py
```

### Comparing `alphabetize-0.0.4/LICENSE` & `alphabetize-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alphabetize-0.0.4/PKG-INFO` & `alphabetize-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabetize
-Version: 0.0.4
+Version: 0.0.5
 Summary: Alphabetize variables within your files
 Home-page: https://github.com/JakeAdey/alphabetize
 Author: Jake Adey
 Author-email: jakespenceradey@gmail.com
 License: MIT
 Keywords: variable-sorting
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alphabetize-0.0.4/setup.cfg` & `alphabetize-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alphabetize
-version = 0.0.4
+version = 0.0.5
 description = Alphabetize variables within your files
 long_description = long_description
 keywords = variable-sorting
 author = Jake Adey
 author_email = jakespenceradey@gmail.com
 url = https://github.com/JakeAdey/alphabetize
 license = MIT
```

### Comparing `alphabetize-0.0.4/setup.py` & `alphabetize-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f1:
     long_description = f1.read()
 
 setup(
     name='alphabetize',
-    version='0.0.4',
+    version='0.0.5',
     description='Alphabetize variables within your files',
     long_description=long_description,
     keywords="variable-sorting",
     author="Jake Adey",
     author_email="jakespenceradey@gmail.com",
     url="https://github.com/JakeAdey/alphabetize",
     license="MIT",
```

### Comparing `alphabetize-0.0.4/src/alphabetize.egg-info/PKG-INFO` & `alphabetize-0.0.5/src/alphabetize.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabetize
-Version: 0.0.4
+Version: 0.0.5
 Summary: Alphabetize variables within your files
 Home-page: https://github.com/JakeAdey/alphabetize
 Author: Jake Adey
 Author-email: jakespenceradey@gmail.com
 License: MIT
 Keywords: variable-sorting
 Classifier: Development Status :: 5 - Production/Stable
```


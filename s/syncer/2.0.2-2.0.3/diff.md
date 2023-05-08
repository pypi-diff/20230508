# Comparing `tmp/syncer-2.0.2.tar.gz` & `tmp/syncer-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncer-2.0.2.tar", last modified: Mon May  8 07:44:27 2023, max compression
+gzip compressed data, was "syncer-2.0.3.tar", last modified: Mon May  8 07:50:06 2023, max compression
```

## Comparing `syncer-2.0.2.tar` & `syncer-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/
--rw-r--r--   0 takagi    (1000) users      (985)     1082 2023-05-08 07:34:27.000000 syncer-2.0.2/LICENSE
--rw-r--r--   0 takagi    (1000) users      (985)      179 2023-05-08 07:34:27.000000 syncer-2.0.2/MANIFEST.in
--rw-r--r--   0 takagi    (1000) users      (985)     3123 2023-05-08 07:44:27.526271 syncer-2.0.2/PKG-INFO
--rw-r--r--   0 takagi    (1000) users      (985)     2385 2023-05-08 07:36:46.000000 syncer-2.0.2/README.rst
-drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/docs/
--rw-r--r--   0 takagi    (1000) users      (985)     6762 2023-05-08 07:34:27.000000 syncer-2.0.2/docs/Makefile
--rw-r--r--   0 takagi    (1000) users      (985)     9198 2023-05-08 07:41:53.000000 syncer-2.0.2/docs/conf.py
--rw-r--r--   0 takagi    (1000) users      (985)      299 2023-05-08 07:34:27.000000 syncer-2.0.2/docs/index.rst
--rw-r--r--   0 takagi    (1000) users      (985)     6459 2023-05-08 07:34:27.000000 syncer-2.0.2/docs/make.bat
--rw-r--r--   0 takagi    (1000) users      (985)      212 2023-05-08 07:44:27.526271 syncer-2.0.2/setup.cfg
--rwxr-xr-x   0 takagi    (1000) users      (985)     1220 2023-05-08 07:41:53.000000 syncer-2.0.2/setup.py
-drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/syncer.egg-info/
--rwxr-xr-x   0 takagi    (1000) users      (985)     3123 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/PKG-INFO
--rwxr-xr-x   0 takagi    (1000) users      (985)      303 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/SOURCES.txt
--rwxr-xr-x   0 takagi    (1000) users      (985)        1 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/dependency_links.txt
--rwxr-xr-x   0 takagi    (1000) users      (985)        1 2018-02-15 06:26:26.000000 syncer-2.0.2/syncer.egg-info/not-zip-safe
--rwxr-xr-x   0 takagi    (1000) users      (985)        7 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/top_level.txt
--rw-r--r--   0 takagi    (1000) users      (985)     1007 2023-05-08 07:34:27.000000 syncer-2.0.2/syncer.py
-drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/tests/
--rw-r--r--   0 takagi    (1000) users      (985)        0 2023-05-08 07:34:27.000000 syncer-2.0.2/tests/__init__.py
--rw-r--r--   0 takagi    (1000) users      (985)     2291 2023-05-08 07:34:27.000000 syncer-2.0.2/tests/test_syncer.py
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:50:06.151960 syncer-2.0.3/
+-rw-r--r--   0 takagi    (1000) users      (985)     1082 2023-05-08 07:34:27.000000 syncer-2.0.3/LICENSE
+-rw-r--r--   0 takagi    (1000) users      (985)      179 2023-05-08 07:34:27.000000 syncer-2.0.3/MANIFEST.in
+-rw-r--r--   0 takagi    (1000) users      (985)     3123 2023-05-08 07:50:06.151960 syncer-2.0.3/PKG-INFO
+-rw-r--r--   0 takagi    (1000) users      (985)     2385 2023-05-08 07:36:46.000000 syncer-2.0.3/README.rst
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:50:06.151960 syncer-2.0.3/docs/
+-rw-r--r--   0 takagi    (1000) users      (985)     6762 2023-05-08 07:34:27.000000 syncer-2.0.3/docs/Makefile
+-rw-r--r--   0 takagi    (1000) users      (985)     9198 2023-05-08 07:50:01.000000 syncer-2.0.3/docs/conf.py
+-rw-r--r--   0 takagi    (1000) users      (985)      299 2023-05-08 07:34:27.000000 syncer-2.0.3/docs/index.rst
+-rw-r--r--   0 takagi    (1000) users      (985)     6459 2023-05-08 07:34:27.000000 syncer-2.0.3/docs/make.bat
+-rw-r--r--   0 takagi    (1000) users      (985)      212 2023-05-08 07:50:06.153959 syncer-2.0.3/setup.cfg
+-rwxr-xr-x   0 takagi    (1000) users      (985)     1220 2023-05-08 07:50:01.000000 syncer-2.0.3/setup.py
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:50:06.151960 syncer-2.0.3/syncer.egg-info/
+-rwxr-xr-x   0 takagi    (1000) users      (985)     3123 2023-05-08 07:50:06.000000 syncer-2.0.3/syncer.egg-info/PKG-INFO
+-rwxr-xr-x   0 takagi    (1000) users      (985)      303 2023-05-08 07:50:06.000000 syncer-2.0.3/syncer.egg-info/SOURCES.txt
+-rwxr-xr-x   0 takagi    (1000) users      (985)        1 2023-05-08 07:50:06.000000 syncer-2.0.3/syncer.egg-info/dependency_links.txt
+-rwxr-xr-x   0 takagi    (1000) users      (985)        1 2018-02-15 06:26:26.000000 syncer-2.0.3/syncer.egg-info/not-zip-safe
+-rwxr-xr-x   0 takagi    (1000) users      (985)        7 2023-05-08 07:50:06.000000 syncer-2.0.3/syncer.egg-info/top_level.txt
+-rw-r--r--   0 takagi    (1000) users      (985)     1007 2023-05-08 07:34:27.000000 syncer-2.0.3/syncer.py
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:50:06.151960 syncer-2.0.3/tests/
+-rw-r--r--   0 takagi    (1000) users      (985)        0 2023-05-08 07:34:27.000000 syncer-2.0.3/tests/__init__.py
+-rw-r--r--   0 takagi    (1000) users      (985)     2291 2023-05-08 07:34:27.000000 syncer-2.0.3/tests/test_syncer.py
```

### Comparing `syncer-2.0.2/LICENSE` & `syncer-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syncer-2.0.2/PKG-INFO` & `syncer-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncer
-Version: 2.0.2
+Version: 2.0.3
 Summary: Async to sync converter
 Home-page: https://github.com/miyakogi/syncer
 Author: Hiroyuki Takagi
 Author-email: miyako.dev@gmail.com
 License: MIT
 Keywords: syncer
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `syncer-2.0.2/README.rst` & `syncer-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `syncer-2.0.2/docs/Makefile` & `syncer-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `syncer-2.0.2/docs/conf.py` & `syncer-2.0.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 copyright = '2016, Hiroyuki Takagi'
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = '2.0.2'
+version = '2.0.3'
 # The full version, including alpha/beta/rc tags.
-release = '2.0.2'
+release = '2.0.3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
```

### Comparing `syncer-2.0.2/docs/make.bat` & `syncer-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `syncer-2.0.2/setup.py` & `syncer-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(readme_file) as readme_file:
     readme = readme_file.read()
 
 test_requirements = ['xfail']
 
 setup(
     name='syncer',
-    version='2.0.2',
+    version='2.0.3',
     description='Async to sync converter',
     long_description=readme,
     author='Hiroyuki Takagi',
     author_email='miyako.dev@gmail.com',
     url='https://github.com/miyakogi/syncer',
     py_modules=['syncer'],
     include_package_data=True,
```

### Comparing `syncer-2.0.2/syncer.egg-info/PKG-INFO` & `syncer-2.0.3/syncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncer
-Version: 2.0.2
+Version: 2.0.3
 Summary: Async to sync converter
 Home-page: https://github.com/miyakogi/syncer
 Author: Hiroyuki Takagi
 Author-email: miyako.dev@gmail.com
 License: MIT
 Keywords: syncer
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `syncer-2.0.2/syncer.py` & `syncer-2.0.3/syncer.py`

 * *Files identical despite different names*

### Comparing `syncer-2.0.2/tests/test_syncer.py` & `syncer-2.0.3/tests/test_syncer.py`

 * *Files identical despite different names*


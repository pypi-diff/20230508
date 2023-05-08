# Comparing `tmp/docassemble-1.4.8.tar.gz` & `tmp/docassemble-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble-1.4.8.tar", last modified: Thu Aug 25 13:37:10 2022, max compression
+gzip compressed data, was "docassemble-1.4.9.tar", last modified: Sat Sep 10 18:15:33 2022, max compression
```

## Comparing `docassemble-1.4.8.tar` & `docassemble-1.4.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:10.217669 docassemble-1.4.8/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:48.000000 docassemble-1.4.8/MANIFEST.in
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      668 2022-08-25 13:37:10.217669 docassemble-1.4.8/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2021-12-05 22:33:51.000000 docassemble-1.4.8/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:10.217669 docassemble-1.4.8/docassemble/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      176 2022-08-25 13:37:07.000000 docassemble-1.4.8/docassemble/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:10.217669 docassemble-1.4.8/docassemble.egg-info/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      668 2022-08-25 13:37:09.000000 docassemble-1.4.8/docassemble.egg-info/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      238 2022-08-25 13:37:09.000000 docassemble-1.4.8/docassemble.egg-info/SOURCES.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-08-25 13:37:09.000000 docassemble-1.4.8/docassemble.egg-info/dependency_links.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-08-25 13:37:09.000000 docassemble-1.4.8/docassemble.egg-info/not-zip-safe
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-08-25 13:37:09.000000 docassemble-1.4.8/docassemble.egg-info/top_level.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       79 2022-08-25 13:37:10.217669 docassemble-1.4.8/setup.cfg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      599 2022-08-25 13:37:07.000000 docassemble-1.4.8/setup.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:33.482581 docassemble-1.4.9/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:48.000000 docassemble-1.4.9/MANIFEST.in
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      668 2022-09-10 18:15:33.482581 docassemble-1.4.9/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2021-12-05 22:33:51.000000 docassemble-1.4.9/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:33.482581 docassemble-1.4.9/docassemble/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      176 2022-09-10 18:15:31.000000 docassemble-1.4.9/docassemble/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:33.482581 docassemble-1.4.9/docassemble.egg-info/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      668 2022-09-10 18:15:33.000000 docassemble-1.4.9/docassemble.egg-info/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      238 2022-09-10 18:15:33.000000 docassemble-1.4.9/docassemble.egg-info/SOURCES.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-09-10 18:15:33.000000 docassemble-1.4.9/docassemble.egg-info/dependency_links.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-09-10 18:15:33.000000 docassemble-1.4.9/docassemble.egg-info/not-zip-safe
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-09-10 18:15:33.000000 docassemble-1.4.9/docassemble.egg-info/top_level.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       79 2022-09-10 18:15:33.482581 docassemble-1.4.9/setup.cfg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      599 2022-09-10 18:15:31.000000 docassemble-1.4.9/setup.py
```

### Comparing `docassemble-1.4.8/PKG-INFO` & `docassemble-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble
-Version: 1.4.8
+Version: 1.4.9
 Summary: The namespace package for the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Description: See the [docassemble web site] for a description of **docassemble**
         and installation instructions.
```

### Comparing `docassemble-1.4.8/docassemble.egg-info/PKG-INFO` & `docassemble-1.4.9/docassemble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble
-Version: 1.4.8
+Version: 1.4.9
 Summary: The namespace package for the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Description: See the [docassemble web site] for a description of **docassemble**
         and installation instructions.
```

### Comparing `docassemble-1.4.8/setup.py` & `docassemble-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
 
 setup(name='docassemble',
-      version='1.4.8',
+      version='1.4.9',
       python_requires='>=3.8',
       description=('The namespace package for the docassemble system.'),
       long_description=read("README.md"),
       long_description_content_type='text/markdown',
       author='Jonathan Pyle',
       author_email='jhpyle@gmail.com',
       license='MIT',
```


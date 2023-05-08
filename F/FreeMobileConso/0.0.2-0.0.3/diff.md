# Comparing `tmp/FreeMobileConso-0.0.2.tar.gz` & `tmp/FreeMobileConso-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeMobileConso-0.0.2.tar", last modified: Mon May  8 18:52:28 2023, max compression
+gzip compressed data, was "FreeMobileConso-0.0.3.tar", last modified: Mon May  8 18:53:49 2023, max compression
```

## Comparing `FreeMobileConso-0.0.2.tar` & `FreeMobileConso-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:52:28.484990 FreeMobileConso-0.0.2/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:52:28.484094 FreeMobileConso-0.0.2/FreeMobileConso/
--rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-08 18:51:43.000000 FreeMobileConso-0.0.2/FreeMobileConso/__init__.py
--rw-r--r--   0 corentin   (501) staff       (20)     5894 2023-05-08 18:48:46.000000 FreeMobileConso-0.0.2/FreeMobileConso/client.py
--rw-r--r--   0 corentin   (501) staff       (20)     2000 2023-05-08 18:49:46.000000 FreeMobileConso-0.0.2/FreeMobileConso/dataClassification.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:52:28.484692 FreeMobileConso-0.0.2/FreeMobileConso.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     2615 2023-05-08 18:52:28.000000 FreeMobileConso-0.0.2/FreeMobileConso.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-08 18:52:28.000000 FreeMobileConso-0.0.2/FreeMobileConso.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-08 18:52:28.000000 FreeMobileConso-0.0.2/FreeMobileConso.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-08 18:52:28.000000 FreeMobileConso-0.0.2/FreeMobileConso.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-08 18:52:28.000000 FreeMobileConso-0.0.2/FreeMobileConso.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.0.2/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     2615 2023-05-08 18:52:28.484871 FreeMobileConso-0.0.2/PKG-INFO
--rwxrwxrwx   0 corentin   (501) staff       (20)     2130 2023-05-08 17:41:52.000000 FreeMobileConso-0.0.2/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-08 18:52:28.485028 FreeMobileConso-0.0.2/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-08 18:51:48.000000 FreeMobileConso-0.0.2/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:53:49.022197 FreeMobileConso-0.0.3/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:53:49.021378 FreeMobileConso-0.0.3/FreeMobileConso/
+-rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-08 18:53:28.000000 FreeMobileConso-0.0.3/FreeMobileConso/__init__.py
+-rw-r--r--   0 corentin   (501) staff       (20)     5894 2023-05-08 18:48:46.000000 FreeMobileConso-0.0.3/FreeMobileConso/client.py
+-rw-r--r--   0 corentin   (501) staff       (20)     2000 2023-05-08 18:49:46.000000 FreeMobileConso-0.0.3/FreeMobileConso/dataClassification.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:53:49.021932 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.0.3/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-08 18:53:49.022089 FreeMobileConso-0.0.3/PKG-INFO
+-rwxrwxrwx   0 corentin   (501) staff       (20)     5574 2023-05-08 18:53:17.000000 FreeMobileConso-0.0.3/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-08 18:53:49.022236 FreeMobileConso-0.0.3/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-08 18:53:23.000000 FreeMobileConso-0.0.3/setup.py
```

### Comparing `FreeMobileConso-0.0.2/FreeMobileConso/__init__.py` & `FreeMobileConso-0.0.3/FreeMobileConso/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 """
 
 
 __title__ = "FreeMobileConso"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 from .dataClassification import *
 from .client import *
```

### Comparing `FreeMobileConso-0.0.2/FreeMobileConso/client.py` & `FreeMobileConso-0.0.3/FreeMobileConso/client.py`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.0.2/FreeMobileConso/dataClassification.py` & `FreeMobileConso-0.0.3/FreeMobileConso/dataClassification.py`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.0.2/LICENSE` & `FreeMobileConso-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.0.2/setup.py` & `FreeMobileConso-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='FreeMobileConso',
-    version='0.0.2',    
+    version='0.0.3',    
     description='A python API for get your consommation of your Free mobile account',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/FreeMobileConso',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```


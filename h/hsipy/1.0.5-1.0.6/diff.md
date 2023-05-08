# Comparing `tmp/hsipy-1.0.5.tar.gz` & `tmp/hsipy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsipy-1.0.5.tar", last modified: Tue Mar 28 15:12:23 2023, max compression
+gzip compressed data, was "hsipy-1.0.6.tar", last modified: Mon May  8 14:31:52 2023, max compression
```

## Comparing `hsipy-1.0.5.tar` & `hsipy-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-03-28 15:12:23.580103 hsipy-1.0.5/
--rw-rw-r--   0 bruno     (1000) bruno     (1000)     3219 2023-03-28 15:12:23.580103 hsipy-1.0.5/PKG-INFO
--rw-rw-r--   0 bruno     (1000) bruno     (1000)     2902 2023-03-28 12:41:10.000000 hsipy-1.0.5/README.md
-drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-03-28 15:12:23.580103 hsipy-1.0.5/hsipy/
--rw-rw-r--   0 bruno     (1000) bruno     (1000)       56 2023-03-28 00:18:48.000000 hsipy-1.0.5/hsipy/__init__.py
--rw-rw-r--   0 bruno     (1000) bruno     (1000)     9497 2023-03-28 15:11:46.000000 hsipy-1.0.5/hsipy/hsi_visualization.py
--rw-rw-r--   0 bruno     (1000) bruno     (1000)    16624 2023-03-26 13:51:46.000000 hsipy-1.0.5/hsipy/hsitools.py
-drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-03-28 15:12:23.580103 hsipy-1.0.5/hsipy.egg-info/
--rw-rw-r--   0 bruno     (1000) bruno     (1000)     3219 2023-03-28 15:12:23.000000 hsipy-1.0.5/hsipy.egg-info/PKG-INFO
--rw-rw-r--   0 bruno     (1000) bruno     (1000)      197 2023-03-28 15:12:23.000000 hsipy-1.0.5/hsipy.egg-info/SOURCES.txt
--rw-rw-r--   0 bruno     (1000) bruno     (1000)        1 2023-03-28 15:12:23.000000 hsipy-1.0.5/hsipy.egg-info/dependency_links.txt
--rw-rw-r--   0 bruno     (1000) bruno     (1000)        6 2023-03-28 15:12:23.000000 hsipy-1.0.5/hsipy.egg-info/top_level.txt
--rw-rw-r--   0 bruno     (1000) bruno     (1000)       38 2023-03-28 15:12:23.580103 hsipy-1.0.5/setup.cfg
--rw-rw-r--   0 bruno     (1000) bruno     (1000)      780 2023-03-28 15:12:12.000000 hsipy-1.0.5/setup.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-08 14:31:52.560458 hsipy-1.0.6/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     3219 2023-05-08 14:31:52.560458 hsipy-1.0.6/PKG-INFO
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     2902 2023-03-28 12:41:10.000000 hsipy-1.0.6/README.md
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-08 14:31:52.560458 hsipy-1.0.6/hsipy/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)       56 2023-03-28 00:18:48.000000 hsipy-1.0.6/hsipy/__init__.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     9497 2023-03-28 15:11:46.000000 hsipy-1.0.6/hsipy/hsi_visualization.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)    16624 2023-03-26 13:51:46.000000 hsipy-1.0.6/hsipy/hsitools.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-08 14:31:52.560458 hsipy-1.0.6/hsipy.egg-info/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     3219 2023-05-08 14:31:52.000000 hsipy-1.0.6/hsipy.egg-info/PKG-INFO
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      197 2023-05-08 14:31:52.000000 hsipy-1.0.6/hsipy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        1 2023-05-08 14:31:52.000000 hsipy-1.0.6/hsipy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        6 2023-05-08 14:31:52.000000 hsipy-1.0.6/hsipy.egg-info/top_level.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)       38 2023-05-08 14:31:52.560458 hsipy-1.0.6/setup.cfg
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      780 2023-05-08 14:30:03.000000 hsipy-1.0.6/setup.py
```

### Comparing `hsipy-1.0.5/PKG-INFO` & `hsipy-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsipy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Module to do Hypespectral Imaging Analysis using the Phasor Transform
 Home-page: https://github.com/schutyb
 Author: Bruno Schuty Teske
 Author-email: schutyb@schutyb.com
 License: bsd-3-clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `hsipy-1.0.5/README.md` & `hsipy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hsipy-1.0.5/hsipy/hsi_visualization.py` & `hsipy-1.0.6/hsipy/hsi_visualization.py`

 * *Files identical despite different names*

### Comparing `hsipy-1.0.5/hsipy/hsitools.py` & `hsipy-1.0.6/hsipy/hsitools.py`

 * *Files identical despite different names*

### Comparing `hsipy-1.0.5/hsipy.egg-info/PKG-INFO` & `hsipy-1.0.6/hsipy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsipy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Module to do Hypespectral Imaging Analysis using the Phasor Transform
 Home-page: https://github.com/schutyb
 Author: Bruno Schuty Teske
 Author-email: schutyb@schutyb.com
 License: bsd-3-clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `hsipy-1.0.5/setup.py` & `hsipy-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.5' 
+VERSION = '1.0.6' 
 PACKAGE_NAME = 'hsipy' 
 AUTHOR = 'Bruno Schuty Teske'
 AUTHOR_EMAIL = 'schutyb@schutyb.com'
 URL = 'https://github.com/schutyb'
 
 LICENSE = 'bsd-3-clause'
 DESCRIPTION = 'Python Module to do Hypespectral Imaging Analysis using the Phasor Transform'
```


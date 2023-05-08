# Comparing `tmp/ProtWave_VAE-0.0.2.tar.gz` & `tmp/ProtWave_VAE-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProtWave_VAE-0.0.2.tar", last modified: Mon May  8 14:36:15 2023, max compression
+gzip compressed data, was "ProtWave_VAE-0.0.3.tar", last modified: Mon May  8 14:51:37 2023, max compression
```

## Comparing `ProtWave_VAE-0.0.2.tar` & `ProtWave_VAE-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        0 2023-05-08 14:36:15.411806 ProtWave_VAE-0.0.2/
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)     1070 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.2/LICENSE
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      443 2023-05-08 14:36:15.411296 ProtWave_VAE-0.0.2/PKG-INFO
-drwxrwxr-x   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        0 2023-05-08 14:36:15.312427 ProtWave_VAE-0.0.2/ProtWave_VAE.egg-info/
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      443 2023-05-08 14:36:14.000000 ProtWave_VAE-0.0.2/ProtWave_VAE.egg-info/PKG-INFO
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      290 2023-05-08 14:36:14.000000 ProtWave_VAE-0.0.2/ProtWave_VAE.egg-info/SOURCES.txt
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        1 2023-05-08 14:36:14.000000 ProtWave_VAE-0.0.2/ProtWave_VAE.egg-info/dependency_links.txt
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)       38 2023-05-08 14:36:14.000000 ProtWave_VAE-0.0.2/ProtWave_VAE.egg-info/requires.txt
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        4 2023-05-08 14:36:14.000000 ProtWave_VAE-0.0.2/ProtWave_VAE.egg-info/top_level.txt
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      221 2023-05-08 13:17:21.000000 ProtWave_VAE-0.0.2/README.md
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)       38 2023-05-08 14:36:15.411911 ProtWave_VAE-0.0.2/setup.cfg
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      726 2023-05-08 14:35:51.000000 ProtWave_VAE-0.0.2/setup.py
-drwxrwxr-x   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        0 2023-05-08 14:36:15.369286 ProtWave_VAE-0.0.2/src/
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      240 2023-05-08 14:23:47.000000 ProtWave_VAE-0.0.2/src/__init__.py
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)    11792 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.2/src/model_components.py
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)    33378 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.2/src/model_ensemble.py
--rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)     9691 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.2/src/wavenet_decoder.py
+drwxrwxr-x   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        0 2023-05-08 14:51:37.242366 ProtWave_VAE-0.0.3/
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)     1070 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.3/LICENSE
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      443 2023-05-08 14:51:37.242146 ProtWave_VAE-0.0.3/PKG-INFO
+drwxrwxr-x   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        0 2023-05-08 14:51:37.240063 ProtWave_VAE-0.0.3/ProtWave_VAE/
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      240 2023-05-08 14:23:47.000000 ProtWave_VAE-0.0.3/ProtWave_VAE/__init__.py
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)    11792 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.3/ProtWave_VAE/model_components.py
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)    33378 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.3/ProtWave_VAE/model_ensemble.py
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)     9691 2023-05-08 13:12:34.000000 ProtWave_VAE-0.0.3/ProtWave_VAE/wavenet_decoder.py
+drwxrwxr-x   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        0 2023-05-08 14:51:37.241782 ProtWave_VAE-0.0.3/ProtWave_VAE.egg-info/
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      443 2023-05-08 14:51:36.000000 ProtWave_VAE-0.0.3/ProtWave_VAE.egg-info/PKG-INFO
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      326 2023-05-08 14:51:36.000000 ProtWave_VAE-0.0.3/ProtWave_VAE.egg-info/SOURCES.txt
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)        1 2023-05-08 14:51:36.000000 ProtWave_VAE-0.0.3/ProtWave_VAE.egg-info/dependency_links.txt
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)       38 2023-05-08 14:51:36.000000 ProtWave_VAE-0.0.3/ProtWave_VAE.egg-info/requires.txt
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)       13 2023-05-08 14:51:36.000000 ProtWave_VAE-0.0.3/ProtWave_VAE.egg-info/top_level.txt
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      221 2023-05-08 13:17:21.000000 ProtWave_VAE-0.0.3/README.md
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)       38 2023-05-08 14:51:37.242439 ProtWave_VAE-0.0.3/setup.cfg
+-rw-rw-r--   0 niksapraljak1 (1441358176) niksapraljak1 (1441358176)      726 2023-05-08 14:51:24.000000 ProtWave_VAE-0.0.3/setup.py
```

### Comparing `ProtWave_VAE-0.0.2/LICENSE` & `ProtWave_VAE-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ProtWave_VAE-0.0.2/setup.py` & `ProtWave_VAE-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name="ProtWave_VAE",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here, e.g.:
         "torch",
         "numpy",
     ],
     extras_require={
```

### Comparing `ProtWave_VAE-0.0.2/src/model_components.py` & `ProtWave_VAE-0.0.3/ProtWave_VAE/model_components.py`

 * *Files identical despite different names*

### Comparing `ProtWave_VAE-0.0.2/src/model_ensemble.py` & `ProtWave_VAE-0.0.3/ProtWave_VAE/model_ensemble.py`

 * *Files identical despite different names*

### Comparing `ProtWave_VAE-0.0.2/src/wavenet_decoder.py` & `ProtWave_VAE-0.0.3/ProtWave_VAE/wavenet_decoder.py`

 * *Files identical despite different names*


# Comparing `tmp/pycromanager-0.8.0.tar.gz` & `tmp/pycromanager-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycromanager-0.8.0.tar", last modified: Thu Jan 28 20:24:52 2021, max compression
+gzip compressed data, was "pycromanager-0.9.0.tar", last modified: Fri Jan 29 18:26:05 2021, max compression
```

## Comparing `pycromanager-0.8.0.tar` & `pycromanager-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-28 20:24:52.033018 pycromanager-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (117)     4215 2021-01-28 20:24:52.033018 pycromanager-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)     3099 2021-01-28 20:24:42.000000 pycromanager-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-28 20:24:52.029018 pycromanager-0.8.0/pycromanager/
--rw-r--r--   0 runner    (1001) docker     (117)      237 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pycromanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)       72 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pycromanager/_version.py
--rw-r--r--   0 runner    (1001) docker     (117)    26715 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pycromanager/acquire.py
--rw-r--r--   0 runner    (1001) docker     (117)    31299 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pycromanager/core.py
--rw-r--r--   0 runner    (1001) docker     (117)    45140 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pycromanager/data.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-28 20:24:52.029018 pycromanager-0.8.0/pycromanager/test/
--rw-r--r--   0 runner    (1001) docker     (117)        0 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pycromanager/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)     7825 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pycromanager/test/test_MDA_events.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-28 20:24:52.029018 pycromanager-0.8.0/pycromanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (117)     4215 2021-01-28 20:24:51.000000 pycromanager-0.8.0/pycromanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      395 2021-01-28 20:24:51.000000 pycromanager-0.8.0/pycromanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-01-28 20:24:51.000000 pycromanager-0.8.0/pycromanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (117)       50 2021-01-28 20:24:51.000000 pycromanager-0.8.0/pycromanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (117)       13 2021-01-28 20:24:51.000000 pycromanager-0.8.0/pycromanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (117)       99 2021-01-28 20:24:42.000000 pycromanager-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (117)       38 2021-01-28 20:24:52.033018 pycromanager-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (117)     1192 2021-01-28 20:24:42.000000 pycromanager-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 18:26:05.525289 pycromanager-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (117)     4215 2021-01-29 18:26:05.525289 pycromanager-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)     3099 2021-01-29 18:25:56.000000 pycromanager-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 18:26:05.525289 pycromanager-0.9.0/pycromanager/
+-rw-r--r--   0 runner    (1001) docker     (117)      237 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pycromanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)       72 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pycromanager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (117)    26738 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pycromanager/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (117)    31299 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pycromanager/core.py
+-rw-r--r--   0 runner    (1001) docker     (117)    45140 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pycromanager/data.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 18:26:05.525289 pycromanager-0.9.0/pycromanager/test/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pycromanager/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)     7825 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pycromanager/test/test_MDA_events.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 18:26:05.525289 pycromanager-0.9.0/pycromanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (117)     4215 2021-01-29 18:26:05.000000 pycromanager-0.9.0/pycromanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)      395 2021-01-29 18:26:05.000000 pycromanager-0.9.0/pycromanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        1 2021-01-29 18:26:05.000000 pycromanager-0.9.0/pycromanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       50 2021-01-29 18:26:05.000000 pycromanager-0.9.0/pycromanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       13 2021-01-29 18:26:05.000000 pycromanager-0.9.0/pycromanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       99 2021-01-29 18:25:56.000000 pycromanager-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (117)       38 2021-01-29 18:26:05.525289 pycromanager-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (117)     1192 2021-01-29 18:25:56.000000 pycromanager-0.9.0/setup.py
```

### Comparing `pycromanager-0.8.0/PKG-INFO` & `pycromanager-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycromanager
-Version: 0.8.0
+Version: 0.9.0
 Summary: Open source microscope control using python
 Home-page: https://github.com/micro-manager/pycro-manager
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 License: UNKNOWN
 Description: [![Documentation Status](https://readthedocs.org/projects/pycro-manager/badge/?version=latest)](https://pycro-manager.readthedocs.io/en/latest/?badge=latest)
         [![License](https://img.shields.io/pypi/l/pycromanager.svg)](https://github.com/micro-manager/pycromanager/raw/master/LICENSE)
```

### Comparing `pycromanager-0.8.0/README.md` & `pycromanager-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pycromanager-0.8.0/pycromanager/acquire.py` & `pycromanager-0.9.0/pycromanager/acquire.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,14 +337,15 @@
                 directory,
                 name,
                 show_viewer,
                 tile_overlap is not None,
                 x_overlap,
                 y_overlap,
                 max_multi_res_index if max_multi_res_index is not None else -1,
+                debug,
             )
         storage = self._remote_acq.get_data_sink()
         if storage is not None:
             self.disk_location = storage.get_disk_location()
 
         if image_process_fn is not None:
             processor = self.bridge.construct_java_object(
```

### Comparing `pycromanager-0.8.0/pycromanager/core.py` & `pycromanager-0.9.0/pycromanager/core.py`

 * *Files identical despite different names*

### Comparing `pycromanager-0.8.0/pycromanager/data.py` & `pycromanager-0.9.0/pycromanager/data.py`

 * *Files identical despite different names*

### Comparing `pycromanager-0.8.0/pycromanager/test/test_MDA_events.py` & `pycromanager-0.9.0/pycromanager/test/test_MDA_events.py`

 * *Files identical despite different names*

### Comparing `pycromanager-0.8.0/pycromanager.egg-info/PKG-INFO` & `pycromanager-0.9.0/pycromanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycromanager
-Version: 0.8.0
+Version: 0.9.0
 Summary: Open source microscope control using python
 Home-page: https://github.com/micro-manager/pycro-manager
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 License: UNKNOWN
 Description: [![Documentation Status](https://readthedocs.org/projects/pycro-manager/badge/?version=latest)](https://pycro-manager.readthedocs.io/en/latest/?badge=latest)
         [![License](https://img.shields.io/pypi/l/pycromanager.svg)](https://github.com/micro-manager/pycromanager/raw/master/LICENSE)
```

### Comparing `pycromanager-0.8.0/setup.py` & `pycromanager-0.9.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/abm_shape_collection-0.4.0.tar.gz` & `tmp/abm_shape_collection-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_shape_collection-0.4.0.tar", max compression
+gzip compressed data, was "abm_shape_collection-0.5.0.tar", max compression
```

## Comparing `abm_shape_collection-0.4.0.tar` & `abm_shape_collection-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1519 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/LICENSE
--rw-r--r--   0        0        0      844 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/README.md
--rw-r--r--   0        0        0     1907 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      819 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/__main__.py
--rw-r--r--   0        0        0     2898 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/calculate_shape_stats.py
--rw-r--r--   0        0        0     2765 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/calculate_size_stats.py
--rw-r--r--   0        0        0     6161 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/compile_shape_modes.py
--rw-r--r--   0        0        0     3201 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/extract_shape_modes.py
--rw-r--r--   0        0        0      508 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/fit_pca_model.py
--rw-r--r--   0        0        0      430 2023-03-30 19:21:20.689648 abm_shape_collection-0.4.0/src/abm_shape_collection/get_shape_coefficients.py
--rw-r--r--   0        0        0      942 2023-03-30 19:21:20.693648 abm_shape_collection-0.4.0/src/abm_shape_collection/make_voxels_array.py
--rw-r--r--   0        0        0     3648 2023-03-30 19:21:20.693648 abm_shape_collection-0.4.0/src/abm_shape_collection/merge_shape_modes.py
--rw-r--r--   0        0        0        0 2023-03-30 19:21:20.693648 abm_shape_collection-0.4.0/src/abm_shape_collection/py.typed
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 abm_shape_collection-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/LICENSE
+-rw-r--r--   0        0        0      844 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/README.md
+-rw-r--r--   0        0        0     1924 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/__main__.py
+-rw-r--r--   0        0        0     2898 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_shape_stats.py
+-rw-r--r--   0        0        0     2765 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_size_stats.py
+-rw-r--r--   0        0        0     6161 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/compile_shape_modes.py
+-rw-r--r--   0        0        0     3201 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/extract_shape_modes.py
+-rw-r--r--   0        0        0      508 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/fit_pca_model.py
+-rw-r--r--   0        0        0      430 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/get_shape_coefficients.py
+-rw-r--r--   0        0        0      352 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/get_shape_properties.py
+-rw-r--r--   0        0        0      942 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/make_voxels_array.py
+-rw-r--r--   0        0        0     3648 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/merge_shape_modes.py
+-rw-r--r--   0        0        0        0 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/py.typed
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 abm_shape_collection-0.5.0/PKG-INFO
```

### Comparing `abm_shape_collection-0.4.0/LICENSE` & `abm_shape_collection-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/README.md` & `abm_shape_collection-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/pyproject.toml` & `abm_shape_collection-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abm-shape-collection"
-version = "0.4.0"
+version = "0.5.0"
 description = "Collection of tasks for analyzing cell shapes."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -55,14 +55,15 @@
 namespace_packages = true
 
 [[tool.mypy.overrides]]
 module = [
     "aicsshparam.*",
     "pandas.*",
     "scipy.*",
+    "skimage.*",
     "sklearn.*",
     "trimesh.*",
     "vtkmodules.*",
 ]
 ignore_missing_imports = true
 
 [tool.tox]
```

### Comparing `abm_shape_collection-0.4.0/src/abm_shape_collection/__init__.py` & `abm_shape_collection-0.5.0/src/abm_shape_collection/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 from .calculate_shape_stats import calculate_shape_stats
 from .calculate_size_stats import calculate_size_stats
 from .compile_shape_modes import compile_shape_modes
 from .extract_shape_modes import extract_shape_modes
 from .fit_pca_model import fit_pca_model
 from .get_shape_coefficients import get_shape_coefficients
+from .get_shape_properties import get_shape_properties
 from .make_voxels_array import make_voxels_array
 from .merge_shape_modes import merge_shape_modes
 
 calculate_shape_stats = task(calculate_shape_stats)
 calculate_size_stats = task(calculate_size_stats)
 compile_shape_modes = task(compile_shape_modes)
 extract_shape_modes = task(extract_shape_modes)
 fit_pca_model = task(fit_pca_model)
 get_shape_coefficients = task(get_shape_coefficients)
+get_shape_properties = task(get_shape_properties)
 make_voxels_array = task(make_voxels_array)
 merge_shape_modes = task(merge_shape_modes)
```

### Comparing `abm_shape_collection-0.4.0/src/abm_shape_collection/calculate_shape_stats.py` & `abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_shape_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/src/abm_shape_collection/calculate_size_stats.py` & `abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_size_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/src/abm_shape_collection/compile_shape_modes.py` & `abm_shape_collection-0.5.0/src/abm_shape_collection/compile_shape_modes.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/src/abm_shape_collection/extract_shape_modes.py` & `abm_shape_collection-0.5.0/src/abm_shape_collection/extract_shape_modes.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/src/abm_shape_collection/make_voxels_array.py` & `abm_shape_collection-0.5.0/src/abm_shape_collection/make_voxels_array.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/src/abm_shape_collection/merge_shape_modes.py` & `abm_shape_collection-0.5.0/src/abm_shape_collection/merge_shape_modes.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.4.0/PKG-INFO` & `abm_shape_collection-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abm-shape-collection
-Version: 0.4.0
+Version: 0.5.0
 Summary: Collection of tasks for analyzing cell shapes.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```


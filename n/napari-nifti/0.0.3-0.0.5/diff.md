# Comparing `tmp/napari-nifti-0.0.3.tar.gz` & `tmp/napari-nifti-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-nifti-0.0.3.tar", last modified: Tue Apr 18 15:47:27 2023, max compression
+gzip compressed data, was "napari-nifti-0.0.5.tar", last modified: Tue Apr 18 15:52:01 2023, max compression
```

## Comparing `napari-nifti-0.0.3.tar` & `napari-nifti-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:47:27.228215 napari-nifti-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-18 15:47:27.228215 napari-nifti-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-18 15:47:27.228215 napari-nifti-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:47:27.228215 napari-nifti-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:47:27.228215 napari-nifti-0.0.3/src/napari_nifti/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/src/napari_nifti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/src/napari_nifti/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/src/napari_nifti/_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-18 15:47:08.000000 napari-nifti-0.0.3/src/napari_nifti/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:47:27.228215 napari-nifti-0.0.3/src/napari_nifti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-18 15:47:27.000000 napari-nifti-0.0.3/src/napari_nifti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 15:47:27.000000 napari-nifti-0.0.3/src/napari_nifti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:47:27.000000 napari-nifti-0.0.3/src/napari_nifti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 15:47:27.000000 napari-nifti-0.0.3/src/napari_nifti.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 15:47:27.000000 napari-nifti-0.0.3/src/napari_nifti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 15:47:27.000000 napari-nifti-0.0.3/src/napari_nifti.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:01.861078 napari-nifti-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-18 15:52:01.861078 napari-nifti-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-18 15:52:01.861078 napari-nifti-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:01.861078 napari-nifti-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:01.861078 napari-nifti-0.0.5/src/napari_nifti/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/src/napari_nifti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/src/napari_nifti/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/src/napari_nifti/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-18 15:51:44.000000 napari-nifti-0.0.5/src/napari_nifti/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:01.861078 napari-nifti-0.0.5/src/napari_nifti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-18 15:52:01.000000 napari-nifti-0.0.5/src/napari_nifti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 15:52:01.000000 napari-nifti-0.0.5/src/napari_nifti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:52:01.000000 napari-nifti-0.0.5/src/napari_nifti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 15:52:01.000000 napari-nifti-0.0.5/src/napari_nifti.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 15:52:01.000000 napari-nifti-0.0.5/src/napari_nifti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 15:52:01.000000 napari-nifti-0.0.5/src/napari_nifti.egg-info/top_level.txt
```

### Comparing `napari-nifti-0.0.3/LICENSE` & `napari-nifti-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-nifti-0.0.3/PKG-INFO` & `napari-nifti-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-nifti
-Version: 0.0.3
+Version: 0.0.5
 Summary: A napari plugin for reading and writing NIFTI files that have the extension .nii or .nii.gz.
 Home-page: https://github.com/MIC-DKFZ/napari-nifti
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-nifti/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-nifti#README.md
```

### Comparing `napari-nifti-0.0.3/README.md` & `napari-nifti-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-nifti-0.0.3/pyproject.toml` & `napari-nifti-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-nifti-0.0.3/setup.cfg` & `napari-nifti-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-nifti-0.0.3/src/napari_nifti/_reader.py` & `napari-nifti-0.0.5/src/napari_nifti/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-nifti-0.0.3/src/napari_nifti/_writer.py` & `napari-nifti-0.0.5/src/napari_nifti/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-nifti-0.0.3/src/napari_nifti/napari.yaml` & `napari-nifti-0.0.5/src/napari_nifti/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-nifti-0.0.3/src/napari_nifti.egg-info/PKG-INFO` & `napari-nifti-0.0.5/src/napari_nifti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-nifti
-Version: 0.0.3
+Version: 0.0.5
 Summary: A napari plugin for reading and writing NIFTI files that have the extension .nii or .nii.gz.
 Home-page: https://github.com/MIC-DKFZ/napari-nifti
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-nifti/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-nifti#README.md
```


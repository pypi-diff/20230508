# Comparing `tmp/morph_utils-0.1.0.tar.gz` & `tmp/morph_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/morph_utils-0.1.0.tar", last modified: Mon May  8 15:11:21 2023, max compression
+gzip compressed data, was "morph_utils-0.1.1.tar", last modified: Mon May  8 15:19:12 2023, max compression
```

## Comparing `morph_utils-0.1.0.tar` & `morph_utils-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:11:21.000000 morph_utils-0.1.0/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      270 2023-05-08 15:11:21.000000 morph_utils-0.1.0/PKG-INFO
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      305 2023-05-08 15:08:12.000000 morph_utils-0.1.0/README.md
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:11:21.000000 morph_utils-0.1.0/morph_utils/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-11 07:03:51.000000 morph_utils-0.1.0/morph_utils/__init__.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:11:21.000000 morph_utils-0.1.0/morph_utils/executable_scripts/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-28 17:46:53.000000 morph_utils-0.1.0/morph_utils/executable_scripts/__init__.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3324 2022-04-14 00:47:59.000000 morph_utils-0.1.0/morph_utils/executable_scripts/distance_between_nodes_for_directory.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11628 2022-04-14 00:02:57.000000 morph_utils-0.1.0/morph_utils/executable_scripts/full_morphology_soma_correction.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2933 2023-03-24 20:41:01.000000 morph_utils-0.1.0/morph_utils/executable_scripts/sort_morphology_ids.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2520 2022-04-28 19:34:21.000000 morph_utils-0.1.0/morph_utils/executable_scripts/validate_swc_dir.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     5504 2023-01-06 22:52:17.000000 morph_utils-0.1.0/morph_utils/graph_traversal.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     9764 2023-03-24 22:00:52.000000 morph_utils-0.1.0/morph_utils/measurements.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    15941 2023-03-24 20:57:09.000000 morph_utils-0.1.0/morph_utils/modifications.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11049 2022-04-28 19:07:08.000000 morph_utils-0.1.0/morph_utils/validation.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3952 2023-01-06 22:55:22.000000 morph_utils-0.1.0/morph_utils/visuals.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:11:21.000000 morph_utils-0.1.0/morph_utils.egg-info/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      270 2023-05-08 15:11:20.000000 morph_utils-0.1.0/morph_utils.egg-info/PKG-INFO
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      686 2023-05-08 15:11:20.000000 morph_utils-0.1.0/morph_utils.egg-info/SOURCES.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        1 2023-05-08 15:11:20.000000 morph_utils-0.1.0/morph_utils.egg-info/dependency_links.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      238 2023-05-08 15:11:20.000000 morph_utils-0.1.0/morph_utils.egg-info/entry_points.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       71 2023-05-08 15:11:20.000000 morph_utils-0.1.0/morph_utils.egg-info/requires.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       12 2023-05-08 15:11:20.000000 morph_utils-0.1.0/morph_utils.egg-info/top_level.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      461 2023-05-08 15:11:21.000000 morph_utils-0.1.0/setup.cfg
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      519 2022-01-28 07:02:40.000000 morph_utils-0.1.0/setup.py
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:19:12.950928 morph_utils-0.1.1/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      207 2023-05-08 15:19:12.952317 morph_utils-0.1.1/PKG-INFO
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      305 2023-05-08 15:08:12.000000 morph_utils-0.1.1/README.md
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:19:12.843501 morph_utils-0.1.1/morph_utils/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-11 07:03:51.000000 morph_utils-0.1.1/morph_utils/__init__.py
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:19:12.944002 morph_utils-0.1.1/morph_utils/executable_scripts/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-28 17:46:53.000000 morph_utils-0.1.1/morph_utils/executable_scripts/__init__.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3324 2022-04-14 00:47:59.000000 morph_utils-0.1.1/morph_utils/executable_scripts/distance_between_nodes_for_directory.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11628 2022-04-14 00:02:57.000000 morph_utils-0.1.1/morph_utils/executable_scripts/full_morphology_soma_correction.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2933 2023-03-24 20:41:01.000000 morph_utils-0.1.1/morph_utils/executable_scripts/sort_morphology_ids.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2520 2022-04-28 19:34:21.000000 morph_utils-0.1.1/morph_utils/executable_scripts/validate_swc_dir.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     5504 2023-01-06 22:52:17.000000 morph_utils-0.1.1/morph_utils/graph_traversal.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     9764 2023-03-24 22:00:52.000000 morph_utils-0.1.1/morph_utils/measurements.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    15941 2023-03-24 20:57:09.000000 morph_utils-0.1.1/morph_utils/modifications.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11049 2022-04-28 19:07:08.000000 morph_utils-0.1.1/morph_utils/validation.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3952 2023-01-06 22:55:22.000000 morph_utils-0.1.1/morph_utils/visuals.py
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:19:12.900604 morph_utils-0.1.1/morph_utils.egg-info/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      207 2023-05-08 15:19:12.000000 morph_utils-0.1.1/morph_utils.egg-info/PKG-INFO
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      686 2023-05-08 15:19:12.000000 morph_utils-0.1.1/morph_utils.egg-info/SOURCES.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        1 2023-05-08 15:19:12.000000 morph_utils-0.1.1/morph_utils.egg-info/dependency_links.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      237 2023-05-08 15:19:12.000000 morph_utils-0.1.1/morph_utils.egg-info/entry_points.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       71 2023-05-08 15:19:12.000000 morph_utils-0.1.1/morph_utils.egg-info/requires.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       12 2023-05-08 15:19:12.000000 morph_utils-0.1.1/morph_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      490 2023-05-08 15:19:12.959450 morph_utils-0.1.1/setup.cfg
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      515 2023-05-08 15:18:44.000000 morph_utils-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `morph_utils-0.1.0/morph_utils/executable_scripts/distance_between_nodes_for_directory.py` & `morph_utils-0.1.1/morph_utils/executable_scripts/distance_between_nodes_for_directory.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/executable_scripts/full_morphology_soma_correction.py` & `morph_utils-0.1.1/morph_utils/executable_scripts/full_morphology_soma_correction.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/executable_scripts/sort_morphology_ids.py` & `morph_utils-0.1.1/morph_utils/executable_scripts/sort_morphology_ids.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/executable_scripts/validate_swc_dir.py` & `morph_utils-0.1.1/morph_utils/executable_scripts/validate_swc_dir.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/graph_traversal.py` & `morph_utils-0.1.1/morph_utils/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/measurements.py` & `morph_utils-0.1.1/morph_utils/measurements.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/modifications.py` & `morph_utils-0.1.1/morph_utils/modifications.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/validation.py` & `morph_utils-0.1.1/morph_utils/validation.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils/visuals.py` & `morph_utils-0.1.1/morph_utils/visuals.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/morph_utils.egg-info/SOURCES.txt` & `morph_utils-0.1.1/morph_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.0/setup.py` & `morph_utils-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 
 with open('requirements.txt', 'r') as f:
     required = f.read().splitlines()
 
 setup(
     name = 'morph_utils',
-    version = '0.1.0',
-    description = """Functions for common and not so common morphology operations""",
+    version = '0.1.1',
+    description = "Functions for common and not so common morphology operations",
     author = "Matthew Mallory",
     author_email = "matt.mallory@alleninstitute.org",
     url = '',
     packages = find_packages(),
     install_requires = required,
     include_package_data=True,
     setup_requires=['pytest-runner'],
```


# Comparing `tmp/morph_utils-0.1.2.tar.gz` & `tmp/morph_utils-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morph_utils-0.1.2.tar", last modified: Mon May  8 15:46:30 2023, max compression
+gzip compressed data, was "morph_utils-0.1.2a0.tar", last modified: Mon May  8 15:44:44 2023, max compression
```

## Comparing `morph_utils-0.1.2.tar` & `morph_utils-0.1.2a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:46:30.091857 morph_utils-0.1.2/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      514 2023-05-08 15:46:30.093117 morph_utils-0.1.2/PKG-INFO
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      305 2023-05-08 15:08:12.000000 morph_utils-0.1.2/README.md
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:46:29.997142 morph_utils-0.1.2/morph_utils/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-11 07:03:51.000000 morph_utils-0.1.2/morph_utils/__init__.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:46:30.084893 morph_utils-0.1.2/morph_utils/executable_scripts/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-28 17:46:53.000000 morph_utils-0.1.2/morph_utils/executable_scripts/__init__.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3324 2022-04-14 00:47:59.000000 morph_utils-0.1.2/morph_utils/executable_scripts/distance_between_nodes_for_directory.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11628 2022-04-14 00:02:57.000000 morph_utils-0.1.2/morph_utils/executable_scripts/full_morphology_soma_correction.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2933 2023-03-24 20:41:01.000000 morph_utils-0.1.2/morph_utils/executable_scripts/sort_morphology_ids.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2520 2022-04-28 19:34:21.000000 morph_utils-0.1.2/morph_utils/executable_scripts/validate_swc_dir.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     5504 2023-01-06 22:52:17.000000 morph_utils-0.1.2/morph_utils/graph_traversal.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     9764 2023-03-24 22:00:52.000000 morph_utils-0.1.2/morph_utils/measurements.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    15941 2023-03-24 20:57:09.000000 morph_utils-0.1.2/morph_utils/modifications.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11049 2022-04-28 19:07:08.000000 morph_utils-0.1.2/morph_utils/validation.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3952 2023-01-06 22:55:22.000000 morph_utils-0.1.2/morph_utils/visuals.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:46:30.044807 morph_utils-0.1.2/morph_utils.egg-info/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      514 2023-05-08 15:46:29.000000 morph_utils-0.1.2/morph_utils.egg-info/PKG-INFO
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      686 2023-05-08 15:46:29.000000 morph_utils-0.1.2/morph_utils.egg-info/SOURCES.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        1 2023-05-08 15:46:29.000000 morph_utils-0.1.2/morph_utils.egg-info/dependency_links.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      237 2023-05-08 15:46:29.000000 morph_utils-0.1.2/morph_utils.egg-info/entry_points.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       71 2023-05-08 15:46:29.000000 morph_utils-0.1.2/morph_utils.egg-info/requires.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       12 2023-05-08 15:46:29.000000 morph_utils-0.1.2/morph_utils.egg-info/top_level.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      677 2023-05-08 15:46:30.099674 morph_utils-0.1.2/setup.cfg
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      702 2023-05-08 15:46:15.000000 morph_utils-0.1.2/setup.py
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:44:44.968509 morph_utils-0.1.2a0/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      516 2023-05-08 15:44:44.969992 morph_utils-0.1.2a0/PKG-INFO
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      305 2023-05-08 15:08:12.000000 morph_utils-0.1.2a0/README.md
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:44:44.877619 morph_utils-0.1.2a0/morph_utils/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-11 07:03:51.000000 morph_utils-0.1.2a0/morph_utils/__init__.py
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:44:44.962731 morph_utils-0.1.2a0/morph_utils/executable_scripts/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2022-01-28 17:46:53.000000 morph_utils-0.1.2a0/morph_utils/executable_scripts/__init__.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3324 2022-04-14 00:47:59.000000 morph_utils-0.1.2a0/morph_utils/executable_scripts/distance_between_nodes_for_directory.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11628 2022-04-14 00:02:57.000000 morph_utils-0.1.2a0/morph_utils/executable_scripts/full_morphology_soma_correction.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2933 2023-03-24 20:41:01.000000 morph_utils-0.1.2a0/morph_utils/executable_scripts/sort_morphology_ids.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2520 2022-04-28 19:34:21.000000 morph_utils-0.1.2a0/morph_utils/executable_scripts/validate_swc_dir.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     5504 2023-01-06 22:52:17.000000 morph_utils-0.1.2a0/morph_utils/graph_traversal.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     9764 2023-03-24 22:00:52.000000 morph_utils-0.1.2a0/morph_utils/measurements.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    15941 2023-03-24 20:57:09.000000 morph_utils-0.1.2a0/morph_utils/modifications.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    11049 2022-04-28 19:07:08.000000 morph_utils-0.1.2a0/morph_utils/validation.py
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3952 2023-01-06 22:55:22.000000 morph_utils-0.1.2a0/morph_utils/visuals.py
+drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-05-08 15:44:44.923753 morph_utils-0.1.2a0/morph_utils.egg-info/
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      516 2023-05-08 15:44:44.000000 morph_utils-0.1.2a0/morph_utils.egg-info/PKG-INFO
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      686 2023-05-08 15:44:44.000000 morph_utils-0.1.2a0/morph_utils.egg-info/SOURCES.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        1 2023-05-08 15:44:44.000000 morph_utils-0.1.2a0/morph_utils.egg-info/dependency_links.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      237 2023-05-08 15:44:44.000000 morph_utils-0.1.2a0/morph_utils.egg-info/entry_points.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       71 2023-05-08 15:44:44.000000 morph_utils-0.1.2a0/morph_utils.egg-info/requires.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       12 2023-05-08 15:44:44.000000 morph_utils-0.1.2a0/morph_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      678 2023-05-08 15:44:44.975171 morph_utils-0.1.2a0/setup.cfg
+-rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      703 2023-05-08 15:42:30.000000 morph_utils-0.1.2a0/setup.py
```

### Comparing `morph_utils-0.1.2/PKG-INFO` & `morph_utils-0.1.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morph_utils
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: Functions for common and not so common morphology operations
 Home-page: 
 Author: Matthew Mallory
 Author-email: matt.mallory@alleninstitute.org
 
 # morph-utils
 This is a lightweight package for common neuron morphology operations inlcuding: graph traversal/measurments, visualization, modifications, node sorting, and various other processes
```

### Comparing `morph_utils-0.1.2/morph_utils/executable_scripts/distance_between_nodes_for_directory.py` & `morph_utils-0.1.2a0/morph_utils/executable_scripts/distance_between_nodes_for_directory.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/executable_scripts/full_morphology_soma_correction.py` & `morph_utils-0.1.2a0/morph_utils/executable_scripts/full_morphology_soma_correction.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/executable_scripts/sort_morphology_ids.py` & `morph_utils-0.1.2a0/morph_utils/executable_scripts/sort_morphology_ids.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/executable_scripts/validate_swc_dir.py` & `morph_utils-0.1.2a0/morph_utils/executable_scripts/validate_swc_dir.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/graph_traversal.py` & `morph_utils-0.1.2a0/morph_utils/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/measurements.py` & `morph_utils-0.1.2a0/morph_utils/measurements.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/modifications.py` & `morph_utils-0.1.2a0/morph_utils/modifications.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/validation.py` & `morph_utils-0.1.2a0/morph_utils/validation.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils/visuals.py` & `morph_utils-0.1.2a0/morph_utils/visuals.py`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/morph_utils.egg-info/PKG-INFO` & `morph_utils-0.1.2a0/morph_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morph-utils
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: Functions for common and not so common morphology operations
 Home-page: 
 Author: Matthew Mallory
 Author-email: matt.mallory@alleninstitute.org
 
 # morph-utils
 This is a lightweight package for common neuron morphology operations inlcuding: graph traversal/measurments, visualization, modifications, node sorting, and various other processes
```

### Comparing `morph_utils-0.1.2/morph_utils.egg-info/SOURCES.txt` & `morph_utils-0.1.2a0/morph_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morph_utils-0.1.2/setup.cfg` & `morph_utils-0.1.2a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = morph_utils
-version = 0.1.2
+version = 0.1.2a
 description-file = README.md
 readme = "README.md"
 Homepage = "https://github.com/MatthewMallory/morph_utils"
 
 [project]
 readme = "README.md"
```

### Comparing `morph_utils-0.1.2/setup.py` & `morph_utils-0.1.2a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = readme_file.read()
 
 with open('requirements.txt', 'r') as f:
     required = f.read().splitlines()
 
 setup(
     name = 'morph_utils',
-    version = '0.1.2',
+    version = '0.1.2a',
     description = "Functions for common and not so common morphology operations",
     long_description=readme,
     author = "Matthew Mallory",
     author_email = "matt.mallory@alleninstitute.org",
     url = '',
     packages = find_packages(),
     install_requires = required,
```


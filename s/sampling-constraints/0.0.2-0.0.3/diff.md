# Comparing `tmp/sampling-constraints-0.0.2.tar.gz` & `tmp/sampling-constraints-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampling-constraints-0.0.2.tar", last modified: Sun May  7 22:07:43 2023, max compression
+gzip compressed data, was "sampling-constraints-0.0.3.tar", last modified: Sun May  7 22:10:08 2023, max compression
```

## Comparing `sampling-constraints-0.0.2.tar` & `sampling-constraints-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.2/LICENSE
--rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.2/README.md
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/scs/
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/scs/constraint/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.2/scs/constraint/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.2/scs/constraint/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/scs/incremental_parse/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.2/scs/incremental_parse/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)    11185 2023-05-07 21:21:55.000000 sampling-constraints-0.0.2/scs/incremental_parse/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/scs/sampling_constraints.egg-info/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:07:43.000000 sampling-constraints-0.0.2/scs/sampling_constraints.egg-info/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      351 2023-05-07 22:07:43.000000 sampling-constraints-0.0.2/scs/sampling_constraints.egg-info/SOURCES.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:07:43.000000 sampling-constraints-0.0.2/scs/sampling_constraints.egg-info/dependency_links.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)       29 2023-05-07 22:07:43.000000 sampling-constraints-0.0.2/scs/sampling_constraints.egg-info/top_level.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/setup.cfg
--rw-r--r--   0 isaac     (1000) isaac     (1000)      504 2023-05-07 22:07:18.000000 sampling-constraints-0.0.2/setup.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:07:43.684571 sampling-constraints-0.0.2/tests/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     4413 2023-05-07 21:17:28.000000 sampling-constraints-0.0.2/tests/test_json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.3/LICENSE
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.3/README.md
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/constraint/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.3/scs/constraint/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.3/scs/constraint/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/incremental_parse/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.3/scs/incremental_parse/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)    11185 2023-05-07 21:21:55.000000 sampling-constraints-0.0.3/scs/incremental_parse/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      351 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/top_level.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/setup.cfg
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      530 2023-05-07 22:09:54.000000 sampling-constraints-0.0.3/setup.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/tests/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     4413 2023-05-07 21:17:28.000000 sampling-constraints-0.0.3/tests/test_json.py
```

### Comparing `sampling-constraints-0.0.2/LICENSE` & `sampling-constraints-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.2/scs/constraint/__init__.py` & `sampling-constraints-0.0.3/scs/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.2/scs/incremental_parse/__init__.py` & `sampling-constraints-0.0.3/scs/incremental_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.2/scs/incremental_parse/json.py` & `sampling-constraints-0.0.3/scs/incremental_parse/json.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.2/tests/test_json.py` & `sampling-constraints-0.0.3/tests/test_json.py`

 * *Files identical despite different names*


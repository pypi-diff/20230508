# Comparing `tmp/sampling-constraints-0.0.4.tar.gz` & `tmp/sampling-constraints-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampling-constraints-0.0.4.tar", last modified: Sun May  7 22:29:26 2023, max compression
+gzip compressed data, was "sampling-constraints-0.0.5.tar", last modified: Mon May  8 00:22:27 2023, max compression
```

## Comparing `sampling-constraints-0.0.4.tar` & `sampling-constraints-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.4/LICENSE
--rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.4/README.md
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.953963 sampling-constraints-0.0.4/scs/
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/scs/constraint/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.4/scs/constraint/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.4/scs/constraint/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/scs/incremental_parse/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.4/scs/incremental_parse/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)    11411 2023-05-07 22:27:06.000000 sampling-constraints-0.0.4/scs/incremental_parse/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      351 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/SOURCES.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/dependency_links.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/top_level.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/setup.cfg
--rw-r--r--   0 isaac     (1000) isaac     (1000)      530 2023-05-07 22:29:22.000000 sampling-constraints-0.0.4/setup.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/tests/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     4660 2023-05-07 22:28:41.000000 sampling-constraints-0.0.4/tests/test_json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.5/LICENSE
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      566 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.5/README.md
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      632 2023-05-08 00:22:08.000000 sampling-constraints-0.0.5/pyproject.toml
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/setup.cfg
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      566 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      393 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        4 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/top_level.txt
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/scs/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        0 2023-05-07 20:06:06.000000 sampling-constraints-0.0.5/src/scs/__init__.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/scs/constraint/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.5/src/scs/constraint/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.5/src/scs/constraint/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/scs/incremental_parse/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.5/src/scs/incremental_parse/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)    11411 2023-05-07 22:27:06.000000 sampling-constraints-0.0.5/src/scs/incremental_parse/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/tests/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     4660 2023-05-08 00:18:23.000000 sampling-constraints-0.0.5/tests/test_json.py
```

### Comparing `sampling-constraints-0.0.4/LICENSE` & `sampling-constraints-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.4/scs/constraint/__init__.py` & `sampling-constraints-0.0.5/src/scs/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.4/scs/incremental_parse/__init__.py` & `sampling-constraints-0.0.5/src/scs/incremental_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.4/scs/incremental_parse/json.py` & `sampling-constraints-0.0.5/src/scs/incremental_parse/json.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.4/tests/test_json.py` & `sampling-constraints-0.0.5/tests/test_json.py`

 * *Files identical despite different names*


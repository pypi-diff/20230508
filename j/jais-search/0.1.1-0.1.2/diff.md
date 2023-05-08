# Comparing `tmp/jais_search-0.1.1.tar.gz` & `tmp/jais_search-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jais_search-0.1.1.tar", max compression
+gzip compressed data, was "jais_search-0.1.2.tar", max compression
```

## Comparing `jais_search-0.1.1.tar` & `jais_search-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1264 2023-05-08 00:07:08.423170 jais_search-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-07 10:29:37.541703 jais_search-0.1.1/jais/__init__.py
--rw-r--r--   0        0        0       45 2023-05-07 10:39:56.352848 jais_search-0.1.1/jais/__main__.py
--rw-r--r--   0        0        0     2599 2023-05-07 23:31:57.129607 jais_search-0.1.1/jais/main.py
--rw-r--r--   0        0        0     2791 2023-05-07 23:25:22.356131 jais_search-0.1.1/jais/models/business.py
--rw-r--r--   0        0        0      971 2023-05-07 10:30:46.511335 jais_search-0.1.1/jais/tmp.py
--rw-r--r--   0        0        0      500 2023-05-08 00:07:14.354222 jais_search-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 jais_search-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1264 2023-05-08 00:07:08.423170 jais_search-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 10:29:37.541703 jais_search-0.1.2/jais/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-07 10:39:56.352848 jais_search-0.1.2/jais/__main__.py
+-rw-r--r--   0        0        0     2599 2023-05-07 23:31:57.129607 jais_search-0.1.2/jais/main.py
+-rw-r--r--   0        0        0     2791 2023-05-07 23:25:22.356131 jais_search-0.1.2/jais/models/business.py
+-rw-r--r--   0        0        0      971 2023-05-07 10:30:46.511335 jais_search-0.1.2/jais/tmp.py
+-rw-r--r--   0        0        0      549 2023-05-08 00:16:20.800012 jais_search-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 jais_search-0.1.2/PKG-INFO
```

### Comparing `jais_search-0.1.1/README.md` & `jais_search-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jais_search-0.1.1/jais/main.py` & `jais_search-0.1.2/jais/main.py`

 * *Files identical despite different names*

### Comparing `jais_search-0.1.1/jais/models/business.py` & `jais_search-0.1.2/jais/models/business.py`

 * *Files identical despite different names*

### Comparing `jais_search-0.1.1/jais/tmp.py` & `jais_search-0.1.2/jais/tmp.py`

 * *Files identical despite different names*

### Comparing `jais_search-0.1.1/PKG-INFO` & `jais_search-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: jais-search
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
+Home-page: https://github.com/busla/jais-cli
 Author: Jón Levy
 Author-email: jon.levy@pm.me
 Requires-Python: >=3.10,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/busla/jais-cli
 Description-Content-Type: text/markdown
 
 # Simple cli client for ja.is
 
 Personal tool that is probably not useful for anyone else
 
 ## Install
```


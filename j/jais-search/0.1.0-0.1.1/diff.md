# Comparing `tmp/jais_search-0.1.0.tar.gz` & `tmp/jais_search-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jais_search-0.1.0.tar", max compression
+gzip compressed data, was "jais_search-0.1.1.tar", max compression
```

## Comparing `jais_search-0.1.0.tar` & `jais_search-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0       96 2023-05-07 23:33:54.265638 jais_search-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-07 10:29:37.541703 jais_search-0.1.0/jais/__init__.py
--rw-r--r--   0        0        0       45 2023-05-07 10:39:56.352848 jais_search-0.1.0/jais/__main__.py
--rw-r--r--   0        0        0     2599 2023-05-07 23:31:57.129607 jais_search-0.1.0/jais/main.py
--rw-r--r--   0        0        0     6993 2023-05-07 23:27:36.145309 jais_search-0.1.0/jais/models/__pycache__/business.cpython-311.pyc
--rw-r--r--   0        0        0     2157 2023-05-07 16:13:17.426176 jais_search-0.1.0/jais/models/business.json
--rw-r--r--   0        0        0     2791 2023-05-07 23:25:22.356131 jais_search-0.1.0/jais/models/business.py
--rw-r--r--   0        0        0      971 2023-05-07 10:30:46.511335 jais_search-0.1.0/jais/tmp.py
--rw-r--r--   0        0        0      500 2023-05-07 23:48:18.375244 jais_search-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 jais_search-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1264 2023-05-08 00:07:08.423170 jais_search-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 10:29:37.541703 jais_search-0.1.1/jais/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-07 10:39:56.352848 jais_search-0.1.1/jais/__main__.py
+-rw-r--r--   0        0        0     2599 2023-05-07 23:31:57.129607 jais_search-0.1.1/jais/main.py
+-rw-r--r--   0        0        0     2791 2023-05-07 23:25:22.356131 jais_search-0.1.1/jais/models/business.py
+-rw-r--r--   0        0        0      971 2023-05-07 10:30:46.511335 jais_search-0.1.1/jais/tmp.py
+-rw-r--r--   0        0        0      500 2023-05-08 00:07:14.354222 jais_search-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 jais_search-0.1.1/PKG-INFO
```

### Comparing `jais_search-0.1.0/jais/main.py` & `jais_search-0.1.1/jais/main.py`

 * *Files identical despite different names*

### Comparing `jais_search-0.1.0/jais/models/business.py` & `jais_search-0.1.1/jais/models/business.py`

 * *Files identical despite different names*

### Comparing `jais_search-0.1.0/jais/tmp.py` & `jais_search-0.1.1/jais/tmp.py`

 * *Files identical despite different names*


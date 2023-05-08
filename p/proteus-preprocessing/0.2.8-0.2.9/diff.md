# Comparing `tmp/proteus_preprocessing-0.2.8.tar.gz` & `tmp/proteus_preprocessing-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_preprocessing-0.2.8.tar", max compression
+gzip compressed data, was "proteus_preprocessing-0.2.9.tar", max compression
```

## Comparing `proteus_preprocessing-0.2.8.tar` & `proteus_preprocessing-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0        0 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/deck/__init__.py
--rw-r--r--   0        0        0      909 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/deck/ecl_deck.py
--rw-r--r--   0        0        0     8550 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/deck/runspec.py
--rw-r--r--   0        0        0     4028 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/deck/section.py
--rw-r--r--   0        0        0        0 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/__init__.py
--rw-r--r--   0        0        0      594 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/dat.py
--rw-r--r--   0        0        0    16684 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/data.py
--rw-r--r--   0        0        0      415 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/egrid.py
--rw-r--r--   0        0        0      365 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/grdecl.py
--rw-r--r--   0        0        0     2123 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/init.py
--rw-r--r--   0        0        0     5402 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/s.py
--rw-r--r--   0        0        0      178 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/modular/x.py
--rw-r--r--   0        0        0       71 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/utils/__init__.py
--rw-r--r--   0        0        0     1062 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/utils/expand_dates.py
--rw-r--r--   0        0        0      901 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/preprocessing/utils/expand_wcon.py
--rw-r--r--   0        0        0     1424 2023-03-15 13:11:53.795332 proteus_preprocessing-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 proteus_preprocessing-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/__init__.py
+-rw-r--r--   0        0        0      909 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/ecl_deck.py
+-rw-r--r--   0        0        0     8550 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/runspec.py
+-rw-r--r--   0        0        0     4028 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/section.py
+-rw-r--r--   0        0        0        0 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/__init__.py
+-rw-r--r--   0        0        0      594 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/dat.py
+-rw-r--r--   0        0        0    16684 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/data.py
+-rw-r--r--   0        0        0      415 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/egrid.py
+-rw-r--r--   0        0        0      365 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/grdecl.py
+-rw-r--r--   0        0        0     2123 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/init.py
+-rw-r--r--   0        0        0     5402 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/s.py
+-rw-r--r--   0        0        0      178 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/x.py
+-rw-r--r--   0        0        0      221 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/patches.py
+-rw-r--r--   0        0        0       71 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/utils/__init__.py
+-rw-r--r--   0        0        0     1062 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/utils/expand_dates.py
+-rw-r--r--   0        0        0      901 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/utils/expand_wcon.py
+-rw-r--r--   0        0        0     1513 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 proteus_preprocessing-0.2.9/PKG-INFO
```

### Comparing `proteus_preprocessing-0.2.8/preprocessing/deck/ecl_deck.py` & `proteus_preprocessing-0.2.9/preprocessing/deck/ecl_deck.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/deck/runspec.py` & `proteus_preprocessing-0.2.9/preprocessing/deck/runspec.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/deck/section.py` & `proteus_preprocessing-0.2.9/preprocessing/deck/section.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/modular/dat.py` & `proteus_preprocessing-0.2.9/preprocessing/modular/dat.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/modular/data.py` & `proteus_preprocessing-0.2.9/preprocessing/modular/data.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/modular/init.py` & `proteus_preprocessing-0.2.9/preprocessing/modular/init.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/modular/s.py` & `proteus_preprocessing-0.2.9/preprocessing/modular/s.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/utils/expand_dates.py` & `proteus_preprocessing-0.2.9/preprocessing/utils/expand_dates.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/preprocessing/utils/expand_wcon.py` & `proteus_preprocessing-0.2.9/preprocessing/utils/expand_wcon.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.8/pyproject.toml` & `proteus_preprocessing-0.2.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "proteus-preprocessing"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = []
 packages = [
     { include = "preprocessing/modular" },
     { include = "preprocessing/deck" },
     { include = "preprocessing/utils" },
+    { include = "preprocessing/patches.py" },
+    { include = "preprocessing/__init__.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-json-logger = "^2.0.1"
 tqdm = "^4.61.0"
 tabulate = "^0.8.9"
@@ -45,15 +47,15 @@
             black preprocessing --check --diff
                 --line-length=120
         """
         help="Check code style using black does not refactor"
     [tool.poe.tasks.pytest]
         cmd="pytest tests"
         help="Run python tests"
-    
+
     [tool.poe.tasks.black_format]
         cmd="""
             black . --line-length=120
         """
         help="Refactor using black, excluding migrations"
 
 [build-system]
```

### Comparing `proteus_preprocessing-0.2.8/PKG-INFO` & `proteus_preprocessing-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-preprocessing
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


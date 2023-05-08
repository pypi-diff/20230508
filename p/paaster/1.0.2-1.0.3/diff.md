# Comparing `tmp/paaster-1.0.2.tar.gz` & `tmp/paaster-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paaster-1.0.2.tar", max compression
+gzip compressed data, was "paaster-1.0.3.tar", max compression
```

## Comparing `paaster-1.0.2.tar` & `paaster-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-05-01 08:58:52.915287 paaster-1.0.2/LICENSE
--rw-r--r--   0        0        0      659 2023-05-01 08:58:52.915287 paaster-1.0.2/README.md
--rw-r--r--   0        0        0     2831 2023-05-01 08:58:52.915287 paaster-1.0.2/paaster_cli/__init__.py
--rw-r--r--   0        0        0      332 2023-05-01 08:58:52.915287 paaster-1.0.2/paaster_cli/misc.py
--rw-r--r--   0        0        0     1409 2023-05-01 08:58:52.915287 paaster-1.0.2/paaster_cli/storage.py
--rw-r--r--   0        0        0      522 2023-05-01 08:58:52.915287 paaster-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 paaster-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 03:51:11.707119 paaster-1.0.3/LICENSE
+-rw-r--r--   0        0        0      659 2023-05-08 03:51:11.707119 paaster-1.0.3/README.md
+-rw-r--r--   0        0        0     2831 2023-05-08 03:51:11.707119 paaster-1.0.3/paaster_cli/__init__.py
+-rw-r--r--   0        0        0      332 2023-05-08 03:51:11.707119 paaster-1.0.3/paaster_cli/misc.py
+-rw-r--r--   0        0        0     1409 2023-05-08 03:51:11.707119 paaster-1.0.3/paaster_cli/storage.py
+-rw-r--r--   0        0        0      522 2023-05-08 03:51:11.707119 paaster-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 paaster-1.0.3/PKG-INFO
```

### Comparing `paaster-1.0.2/LICENSE` & `paaster-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paaster-1.0.2/README.md` & `paaster-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `paaster-1.0.2/paaster_cli/__init__.py` & `paaster-1.0.3/paaster_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `paaster-1.0.2/paaster_cli/storage.py` & `paaster-1.0.3/paaster_cli/storage.py`

 * *Files identical despite different names*

### Comparing `paaster-1.0.2/pyproject.toml` & `paaster-1.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paaster"
-version = "1.0.2"
+version = "1.0.3"
 description = "Upload locally encrypted pastes from your terminal to Paaster"
 authors = ["WardPearce <wardpearce@protonmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "paaster_cli"}]
 
 [tool.poetry.dependencies]
```

### Comparing `paaster-1.0.2/PKG-INFO` & `paaster-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paaster
-Version: 1.0.2
+Version: 1.0.3
 Summary: Upload locally encrypted pastes from your terminal to Paaster
 License: GPL-3.0
 Author: WardPearce
 Author-email: wardpearce@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```


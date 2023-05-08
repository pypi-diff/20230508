# Comparing `tmp/auptitcafe-0.1.2.tar.gz` & `tmp/auptitcafe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auptitcafe-0.1.2.tar", max compression
+gzip compressed data, was "auptitcafe-0.1.3.tar", max compression
```

## Comparing `auptitcafe-0.1.2.tar` & `auptitcafe-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.2/auptitcafe/__init__.py
--rw-r--r--   0        0        0     1928 2023-05-08 01:45:43.605501 auptitcafe-0.1.2/auptitcafe/menus.py
--rw-r--r--   0        0        0      501 2023-05-08 01:45:31.385359 auptitcafe-0.1.2/auptitcafe/plat.py
--rw-r--r--   0        0        0      441 2023-05-08 01:45:22.073255 auptitcafe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.3/auptitcafe/__init__.py
+-rw-r--r--   0        0        0     1928 2023-05-08 01:45:43.605501 auptitcafe-0.1.3/auptitcafe/menus.py
+-rw-r--r--   0        0        0      501 2023-05-08 01:45:31.385359 auptitcafe-0.1.3/auptitcafe/plat.py
+-rw-r--r--   0        0        0      441 2023-05-08 01:49:51.028751 auptitcafe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.3/PKG-INFO
```

### Comparing `auptitcafe-0.1.2/auptitcafe/menus.py` & `auptitcafe-0.1.3/auptitcafe/menus.py`

 * *Files identical despite different names*

### Comparing `auptitcafe-0.1.2/PKG-INFO` & `auptitcafe-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auptitcafe
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


# Comparing `tmp/budgetguard-0.8.0.tar.gz` & `tmp/budgetguard-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetguard-0.8.0.tar", max compression
+gzip compressed data, was "budgetguard-0.9.0.tar", max compression
```

## Comparing `budgetguard-0.8.0.tar` & `budgetguard-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1211 2023-05-07 17:22:54.378658 budgetguard-0.8.0/LICENSE
--rw-r--r--   0        0        0      680 2023-05-07 17:22:54.378658 budgetguard-0.8.0/README.md
--rw-r--r--   0        0        0       22 2023-05-07 17:24:06.962719 budgetguard-0.8.0/budgetguard/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/budgetguard/pipelines/__init__.py
--rw-r--r--   0        0        0      335 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/budgetguard/pipelines/base.py
--rw-r--r--   0        0        0        0 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/budgetguard/scripts/__init__.py
--rw-r--r--   0        0        0      493 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/tests/__init__.py
--rw-r--r--   0        0        0      994 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/tests/test_dummy.py
--rw-r--r--   0        0        0      610 2023-05-07 17:24:06.962719 budgetguard-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 budgetguard-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-05-08 09:09:01.919735 budgetguard-0.9.0/LICENSE
+-rw-r--r--   0        0        0      680 2023-05-08 09:09:01.919735 budgetguard-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 09:10:16.472951 budgetguard-0.9.0/budgetguard/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:09:01.919735 budgetguard-0.9.0/budgetguard/budgetguard/pipelines/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-08 09:09:01.919735 budgetguard-0.9.0/budgetguard/budgetguard/pipelines/base.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:09:01.919735 budgetguard-0.9.0/budgetguard/budgetguard/scripts/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-08 09:09:01.919735 budgetguard-0.9.0/budgetguard/tests/__init__.py
+-rw-r--r--   0        0        0      994 2023-05-08 09:09:01.919735 budgetguard-0.9.0/budgetguard/tests/test_dummy.py
+-rw-r--r--   0        0        0      610 2023-05-08 09:10:16.472951 budgetguard-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 budgetguard-0.9.0/PKG-INFO
```

### Comparing `budgetguard-0.8.0/LICENSE` & `budgetguard-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetguard-0.8.0/README.md` & `budgetguard-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `budgetguard-0.8.0/budgetguard/tests/test_dummy.py` & `budgetguard-0.9.0/budgetguard/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `budgetguard-0.8.0/pyproject.toml` & `budgetguard-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "budgetguard"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["Mateusz Borsuk <mtszborsuk212@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.8"
 pyspark = "3.2.0"
```

### Comparing `budgetguard-0.8.0/PKG-INFO` & `budgetguard-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetguard
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Author: Mateusz Borsuk
 Author-email: mtszborsuk212@gmail.com
 Requires-Python: >=3.8.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


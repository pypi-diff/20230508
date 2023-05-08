# Comparing `tmp/kalm-0.2.1.tar.gz` & `tmp/kalm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.2.1.tar", max compression
+gzip compressed data, was "kalm-0.2.2.tar", max compression
```

## Comparing `kalm-0.2.1.tar` & `kalm-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1790 2023-05-06 18:29:03.413708 kalm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-05 20:49:24.884279 kalm-0.2.1/src/kalm/__init__.py
--rw-r--r--   0        0        0    32280 2023-05-05 20:49:24.884279 kalm-0.2.1/src/kalm/kalm.py
--rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.2.1/src/kalm/kalm_api.py
--rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.2.1/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.2.1/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.2.1/src/kalm/toolbox.py
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-08 11:54:16.776225 kalm-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1790 2023-05-08 11:54:16.776225 kalm-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-08 11:54:16.776225 kalm-0.2.2/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32306 2023-05-08 11:54:16.776225 kalm-0.2.2/src/kalm/kalm.py
+-rw-r--r--   0        0        0     6484 2023-05-08 11:54:16.776225 kalm-0.2.2/src/kalm/kalm_api.py
+-rw-r--r--   0        0        0     1296 2023-05-08 11:54:16.776225 kalm-0.2.2/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-08 11:54:16.776225 kalm-0.2.2/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-08 11:54:16.776225 kalm-0.2.2/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.2.2/PKG-INFO
```

### Comparing `kalm-0.2.1/LICENSE.txt` & `kalm-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.2.1/pyproject.toml` & `kalm-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "kalm"
-version = "0.2.1"
-description = "Knowit automation lifecycle management"
+version = "0.2.2"
+description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kalm-0.2.1/src/kalm/__init__.py` & `kalm-0.2.2/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.2.1/src/kalm/kalm.py` & `kalm-0.2.2/src/kalm/kalm.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import datetime
 
 def prettyllog(function, action, item, organization, statuscode, text):
   d_date = datetime.datetime.now()
   reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
   print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
 
-  
-
+def dummy:
+    print("dummy")
 
 #def prettyllog(function, action, item, organization, statuscode, text):
  # d_date = datetime.datetime.now()
  # reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
  # print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
 
 class Hvac:
```

### Comparing `kalm-0.2.1/src/kalm/kalm_api.py` & `kalm-0.2.2/src/kalm/kalm_api.py`

 * *Files identical despite different names*

### Comparing `kalm-0.2.1/src/kalm/netbox.py` & `kalm-0.2.2/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.2.1/PKG-INFO` & `kalm-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.2.1
-Summary: Knowit automation lifecycle management
+Version: 0.2.2
+Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


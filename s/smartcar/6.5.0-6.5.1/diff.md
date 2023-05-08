# Comparing `tmp/smartcar-6.5.0.tar.gz` & `tmp/smartcar-6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smartcar-6.5.0.tar", last modified: Thu Apr 13 20:19:03 2023, max compression
+gzip compressed data, was "dist/smartcar-6.5.1.tar", last modified: Mon May  8 18:30:30 2023, max compression
```

## Comparing `smartcar-6.5.0.tar` & `smartcar-6.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-13 20:19:03.239466 smartcar-6.5.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2023-04-13 20:18:12.000000 smartcar-6.5.0/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-04-13 20:19:03.239466 smartcar-6.5.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6355 2023-04-13 20:18:12.000000 smartcar-6.5.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-04-13 20:19:03.243466 smartcar-6.5.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1215 2023-04-13 20:18:12.000000 smartcar-6.5.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-13 20:19:03.239466 smartcar-6.5.0/smartcar/
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2023-04-13 20:18:38.000000 smartcar-6.5.0/smartcar/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9282 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/auth_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4118 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3587 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9064 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/smartcar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11006 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19528 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/vehicle.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-13 20:19:03.239466 smartcar-6.5.0/smartcar.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 18:30:30.540749 smartcar-6.5.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2023-05-08 18:29:37.000000 smartcar-6.5.1/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-05-08 18:30:30.540749 smartcar-6.5.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6355 2023-05-08 18:29:37.000000 smartcar-6.5.1/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-08 18:30:30.540749 smartcar-6.5.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1215 2023-05-08 18:29:37.000000 smartcar-6.5.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 18:30:30.540749 smartcar-6.5.1/smartcar/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2023-05-08 18:30:05.000000 smartcar-6.5.1/smartcar/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9282 2023-05-08 18:29:37.000000 smartcar-6.5.1/smartcar/auth_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2023-05-08 18:29:37.000000 smartcar-6.5.1/smartcar/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4118 2023-05-08 18:29:37.000000 smartcar-6.5.1/smartcar/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3832 2023-05-08 18:29:37.000000 smartcar-6.5.1/smartcar/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9064 2023-05-08 18:29:37.000000 smartcar-6.5.1/smartcar/smartcar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11006 2023-05-08 18:29:37.000000 smartcar-6.5.1/smartcar/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19528 2023-05-08 18:29:37.000000 smartcar-6.5.1/smartcar/vehicle.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 18:30:30.540749 smartcar-6.5.1/smartcar.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-05-08 18:30:30.000000 smartcar-6.5.1/smartcar.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-05-08 18:30:30.000000 smartcar-6.5.1/smartcar.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-08 18:30:30.000000 smartcar-6.5.1/smartcar.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-08 18:30:30.000000 smartcar-6.5.1/smartcar.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-05-08 18:30:30.000000 smartcar-6.5.1/smartcar.egg-info/top_level.txt
```

### Comparing `smartcar-6.5.0/LICENSE.md` & `smartcar-6.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/PKG-INFO` & `smartcar-6.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcar
-Version: 6.5.0
+Version: 6.5.1
 Summary: Smartcar Python SDK
 Home-page: https://github.com/smartcar/python-sdk
 Author: Smartcar
 Author-email: hello@smartcar.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `smartcar-6.5.0/README.md` & `smartcar-6.5.1/README.md`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/setup.py` & `smartcar-6.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/smartcar/auth_client.py` & `smartcar-6.5.1/smartcar/auth_client.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/smartcar/exception.py` & `smartcar-6.5.1/smartcar/exception.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/smartcar/helpers.py` & `smartcar-6.5.1/smartcar/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,16 +110,20 @@
         (<formatted path>, <formatted attribute>)
 
         e.g.
         1. "EMPTY" raw_path  == '/' -> ('', 'attributes')
         2. "NORMAL" raw_path == '/odometer' -> ('odometer', 'odometer')
         3. "NESTED" raw_path == '/engine/oil' -> ('engine/oil', 'engine_oil')
     """
+    # mapper holds unique situations where the path does not exactly line up with the function to call
+    # we have a set_charge_limit but are not concerned with it in batch calls
     mapper = {
-        "battery/capacity": "battery_capacity",
-        "engine/oil": "engine_oil",
+        "charge/limit": "get_charge_limit",
         "tires/pressure": "tire_pressure",
         "": "attributes",
     }
     formatted_path = raw_path[1:] if raw_path[0] == "/" else raw_path
     formatted_attribute = mapper.get(formatted_path, formatted_path)
+    if "/" in formatted_attribute:
+        formatted_attribute = formatted_attribute.replace("/", "_")
+
     return formatted_path, formatted_attribute
```

### Comparing `smartcar-6.5.0/smartcar/smartcar.py` & `smartcar-6.5.1/smartcar/smartcar.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/smartcar/types.py` & `smartcar-6.5.1/smartcar/types.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/smartcar/vehicle.py` & `smartcar-6.5.1/smartcar/vehicle.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.5.0/smartcar.egg-info/PKG-INFO` & `smartcar-6.5.1/smartcar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcar
-Version: 6.5.0
+Version: 6.5.1
 Summary: Smartcar Python SDK
 Home-page: https://github.com/smartcar/python-sdk
 Author: Smartcar
 Author-email: hello@smartcar.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```


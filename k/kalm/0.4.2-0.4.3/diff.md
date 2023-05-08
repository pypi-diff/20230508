# Comparing `tmp/kalm-0.4.2.tar.gz` & `tmp/kalm-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.4.2.tar", max compression
+gzip compressed data, was "kalm-0.4.3.tar", max compression
```

## Comparing `kalm-0.4.2.tar` & `kalm-0.4.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     1832 2023-05-08 13:30:46.934159 kalm-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    10666 2023-05-08 13:30:22.230015 kalm-0.4.2/src/kalm/__init__.py
--rw-r--r--   0        0        0    32308 2023-05-08 13:21:45.550993 kalm-0.4.2/src/kalm/kalm.py
--rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.4.2/src/kalm/kalm_api.py
--rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.4.2/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.4.2/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.4.2/src/kalm/toolbox.py
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     1832 2023-05-08 13:32:39.302817 kalm-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    10663 2023-05-08 13:32:39.302817 kalm-0.4.3/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32308 2023-05-08 13:21:45.550993 kalm-0.4.3/src/kalm/kalm.py
+-rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/kalm_api.py
+-rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.4.3/PKG-INFO
```

### Comparing `kalm-0.4.2/LICENSE.txt` & `kalm-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.4.2/pyproject.toml` & `kalm-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.4.2"
+version = "0.4.3"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
```

### Comparing `kalm-0.4.2/src/kalm/__init__.py` & `kalm-0.4.3/src/kalm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     ready = False
     print("check if we are ready to go")
     ready  = connectiontest()
 
     if args.action[0] == "jenkins":
         if ready:
             print("Jenkins adminitrator")
-            jenkins.jenkins()
+            kalm.jenkins()
 
             exit(0)
         else:
             exit(1)
 
     if args.action[0] == "check":
         if ready:
```

### Comparing `kalm-0.4.2/src/kalm/kalm.py` & `kalm-0.4.3/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.2/src/kalm/kalm_api.py` & `kalm-0.4.3/src/kalm/kalm_api.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.2/src/kalm/netbox.py` & `kalm-0.4.3/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.2/PKG-INFO` & `kalm-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.4.2
+Version: 0.4.3
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


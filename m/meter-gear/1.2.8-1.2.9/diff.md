# Comparing `tmp/meter-gear-1.2.8.tar.gz` & `tmp/meter-gear-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meter-gear-1.2.8.tar", last modified: Mon Jun 13 15:58:21 2022, max compression
+gzip compressed data, was "meter-gear-1.2.9.tar", last modified: Tue Jun 14 15:55:20 2022, max compression
```

## Comparing `meter-gear-1.2.8.tar` & `meter-gear-1.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-13 15:58:21.899361 meter-gear-1.2.8/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1094 2022-06-13 15:58:21.000000 meter-gear-1.2.8/LICENSE
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       60 2022-06-13 15:58:21.000000 meter-gear-1.2.8/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3200 2022-06-13 15:58:21.899361 meter-gear-1.2.8/PKG-INFO
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2734 2022-06-13 15:58:21.000000 meter-gear-1.2.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-13 15:58:21.899361 meter-gear-1.2.8/gear/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       19 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    12937 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1304 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/log.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-13 15:58:21.899361 meter-gear-1.2.8/gear/meter/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/meter/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1587 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/meter/account.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    10008 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/meter/client.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2661 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/meter/request.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     7299 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/rpc.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      318 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/testclient.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-13 15:58:21.899361 meter-gear-1.2.8/gear/utils/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/utils/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     9435 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/utils/compat.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3728 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/utils/keystore.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      363 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/utils/singleton.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      952 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/utils/thread.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5240 2022-06-13 15:58:21.000000 meter-gear-1.2.8/gear/utils/types.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-13 15:58:21.899361 meter-gear-1.2.8/meter_gear.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3200 2022-06-13 15:58:21.000000 meter-gear-1.2.8/meter_gear.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2022-06-13 15:58:21.000000 meter-gear-1.2.8/meter_gear.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-13 15:58:21.000000 meter-gear-1.2.8/meter_gear.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2022-06-13 15:58:21.000000 meter-gear-1.2.8/meter_gear.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      144 2022-06-13 15:58:21.000000 meter-gear-1.2.8/meter_gear.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-06-13 15:58:21.000000 meter-gear-1.2.8/meter_gear.egg-info/top_level.txt
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      143 2022-06-13 15:58:21.000000 meter-gear-1.2.8/requirements.txt
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       71 2022-06-13 15:58:21.899361 meter-gear-1.2.8/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1050 2022-06-13 15:58:21.000000 meter-gear-1.2.8/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-14 15:55:20.235638 meter-gear-1.2.9/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1094 2022-06-14 15:55:19.000000 meter-gear-1.2.9/LICENSE
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       60 2022-06-14 15:55:19.000000 meter-gear-1.2.9/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3200 2022-06-14 15:55:20.235638 meter-gear-1.2.9/PKG-INFO
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2734 2022-06-14 15:55:19.000000 meter-gear-1.2.9/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-14 15:55:20.235638 meter-gear-1.2.9/gear/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       19 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    12937 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1304 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/log.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-14 15:55:20.235638 meter-gear-1.2.9/gear/meter/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/meter/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1587 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/meter/account.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    10008 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/meter/client.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2661 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/meter/request.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     7299 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/rpc.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      318 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/testclient.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-14 15:55:20.235638 meter-gear-1.2.9/gear/utils/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/utils/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     9435 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/utils/compat.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3728 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/utils/keystore.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      363 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/utils/singleton.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      952 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/utils/thread.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5247 2022-06-14 15:55:19.000000 meter-gear-1.2.9/gear/utils/types.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-14 15:55:20.235638 meter-gear-1.2.9/meter_gear.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3200 2022-06-14 15:55:20.000000 meter-gear-1.2.9/meter_gear.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2022-06-14 15:55:20.000000 meter-gear-1.2.9/meter_gear.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-14 15:55:20.000000 meter-gear-1.2.9/meter_gear.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2022-06-14 15:55:20.000000 meter-gear-1.2.9/meter_gear.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      144 2022-06-14 15:55:20.000000 meter-gear-1.2.9/meter_gear.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-06-14 15:55:20.000000 meter-gear-1.2.9/meter_gear.egg-info/top_level.txt
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      143 2022-06-14 15:55:19.000000 meter-gear-1.2.9/requirements.txt
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       71 2022-06-14 15:55:20.239638 meter-gear-1.2.9/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1050 2022-06-14 15:55:19.000000 meter-gear-1.2.9/setup.py
```

### Comparing `meter-gear-1.2.8/LICENSE` & `meter-gear-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/PKG-INFO` & `meter-gear-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meter-gear
-Version: 1.2.8
+Version: 1.2.9
 Summary: An adapter between meter-restful and eth-rpc.
 Home-page: https://github.com/meterio/meter-gear
 Author: Simon Zhang
 Author-email: zhanghan.simon@gmail.com
 License: MIT
 Keywords: meter blockchain ethereum
 Platform: UNKNOWN
```

### Comparing `meter-gear-1.2.8/README.md` & `meter-gear-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/cli.py` & `meter-gear-1.2.9/gear/cli.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/log.py` & `meter-gear-1.2.9/gear/log.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/meter/account.py` & `meter-gear-1.2.9/gear/meter/account.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/meter/client.py` & `meter-gear-1.2.9/gear/meter/client.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/meter/request.py` & `meter-gear-1.2.9/gear/meter/request.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/rpc.py` & `meter-gear-1.2.9/gear/rpc.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/utils/compat.py` & `meter-gear-1.2.9/gear/utils/compat.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/utils/keystore.py` & `meter-gear-1.2.9/gear/utils/keystore.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/utils/thread.py` & `meter-gear-1.2.9/gear/utils/thread.py`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/gear/utils/types.py` & `meter-gear-1.2.9/gear/utils/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 def decode_hex(value):
     return _decode_hex(strip_0x(value))
 
 
 def normalize_number(value):
     if is_numeric(value):
         return value
-    elif is_numeric_str:
+    elif is_numeric_str(value):
         return int(value, 10)
     elif is_hex_str(value):
         return int(value, 16)
     elif is_hex_str('0x'+value):
         return int('0x'+value, 16)
     else:
         raise ValueError("Unknown numeric encoding: {0}".format(value))
```

### Comparing `meter-gear-1.2.8/meter_gear.egg-info/PKG-INFO` & `meter-gear-1.2.9/meter_gear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meter-gear
-Version: 1.2.8
+Version: 1.2.9
 Summary: An adapter between meter-restful and eth-rpc.
 Home-page: https://github.com/meterio/meter-gear
 Author: Simon Zhang
 Author-email: zhanghan.simon@gmail.com
 License: MIT
 Keywords: meter blockchain ethereum
 Platform: UNKNOWN
```

### Comparing `meter-gear-1.2.8/meter_gear.egg-info/SOURCES.txt` & `meter-gear-1.2.9/meter_gear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meter-gear-1.2.8/setup.py` & `meter-gear-1.2.9/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/aioairzone-0.5.3.tar.gz` & `tmp/aioairzone-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-0.5.3.tar", last modified: Wed Mar  8 20:20:44 2023, max compression
+gzip compressed data, was "aioairzone-0.5.4.tar", last modified: Mon May  8 15:46:52 2023, max compression
```

## Comparing `aioairzone-0.5.3.tar` & `aioairzone-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-03-08 20:20:44.744914 aioairzone-0.5.3/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.5.3/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.5.3/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2222 2023-03-08 20:20:44.744914 aioairzone-0.5.3/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1488 2022-05-10 12:55:46.000000 aioairzone-0.5.3/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-03-08 20:20:44.744914 aioairzone-0.5.3/aioairzone/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.5.3/aioairzone/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4261 2023-03-08 19:43:48.000000 aioairzone-0.5.3/aioairzone/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4431 2023-03-08 19:32:37.000000 aioairzone-0.5.3/aioairzone/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    28229 2023-03-08 20:13:44.000000 aioairzone-0.5.3/aioairzone/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.5.3/aioairzone/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    13531 2022-11-17 19:04:03.000000 aioairzone-0.5.3/aioairzone/localapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.5.3/aioairzone/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.5.3/aioairzone/webserver.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-03-08 20:20:44.744914 aioairzone-0.5.3/aioairzone.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2222 2023-03-08 20:20:44.000000 aioairzone-0.5.3/aioairzone.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      444 2023-03-08 20:20:44.000000 aioairzone-0.5.3/aioairzone.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-03-08 20:20:44.000000 aioairzone-0.5.3/aioairzone.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-03-08 20:20:44.000000 aioairzone-0.5.3/aioairzone.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-03-08 20:20:44.000000 aioairzone-0.5.3/aioairzone.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-03-08 20:20:44.000000 aioairzone-0.5.3/aioairzone.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.5.3/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-03-08 20:20:44.744914 aioairzone-0.5.3/setup.cfg
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1151 2023-03-08 20:18:48.000000 aioairzone-0.5.3/setup.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-08 15:46:52.878488 aioairzone-0.5.4/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.5.4/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.5.4/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2222 2023-05-08 15:46:52.878488 aioairzone-0.5.4/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1488 2022-05-10 12:55:46.000000 aioairzone-0.5.4/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-08 15:46:52.878488 aioairzone-0.5.4/aioairzone/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.5.4/aioairzone/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4261 2023-03-08 19:43:48.000000 aioairzone-0.5.4/aioairzone/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4431 2023-03-08 19:32:37.000000 aioairzone-0.5.4/aioairzone/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    28229 2023-03-08 20:13:44.000000 aioairzone-0.5.4/aioairzone/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.5.4/aioairzone/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    13801 2023-05-08 15:42:47.000000 aioairzone-0.5.4/aioairzone/localapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.5.4/aioairzone/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.5.4/aioairzone/webserver.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-08 15:46:52.878488 aioairzone-0.5.4/aioairzone.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2222 2023-05-08 15:46:52.000000 aioairzone-0.5.4/aioairzone.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      444 2023-05-08 15:46:52.000000 aioairzone-0.5.4/aioairzone.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-08 15:46:52.000000 aioairzone-0.5.4/aioairzone.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-08 15:46:52.000000 aioairzone-0.5.4/aioairzone.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-08 15:46:52.000000 aioairzone-0.5.4/aioairzone.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-08 15:46:52.000000 aioairzone-0.5.4/aioairzone.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.5.4/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-08 15:46:52.878488 aioairzone-0.5.4/setup.cfg
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1151 2023-05-08 15:45:33.000000 aioairzone-0.5.4/setup.py
```

### Comparing `aioairzone-0.5.3/LICENSE` & `aioairzone-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.3/PKG-INFO` & `aioairzone-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.5.3
+Version: 0.5.4
 Summary: Library to control Airzone devices
 Home-page: https://github.com/Noltari/aioairzone
 Download-URL: https://github.com/Noltari/aioairzone
 Author: Álvaro Fernández Rojas
 Author-email: noltari@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aioairzone-0.5.3/README.md` & `aioairzone-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.3/aioairzone/common.py` & `aioairzone-0.5.4/aioairzone/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.3/aioairzone/const.py` & `aioairzone-0.5.4/aioairzone/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.3/aioairzone/device.py` & `aioairzone-0.5.4/aioairzone/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.3/aioairzone/exceptions.py` & `aioairzone-0.5.4/aioairzone/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.3/aioairzone/localapi.py` & `aioairzone-0.5.4/aioairzone/localapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 from json import JSONDecodeError
 from typing import Any, cast
 
 from aiohttp import ClientConnectorError, ClientSession
 from aiohttp.client_reqrep import ClientResponse
 
 from .const import (
+    API_COOL_SET_POINT,
     API_DATA,
     API_DEMO,
     API_ERROR_METHOD_NOT_SUPPORTED,
     API_ERROR_REQUEST_MALFORMED,
     API_ERROR_SYSTEM_ID_NOT_AVAILABLE,
     API_ERROR_SYSTEM_ID_OUT_RANGE,
     API_ERROR_ZONE_ID_NOT_AVAILABLE,
     API_ERROR_ZONE_ID_NOT_PROVIDED,
     API_ERROR_ZONE_ID_OUT_RANGE,
     API_ERRORS,
+    API_HEAT_SET_POINT,
     API_HVAC,
     API_INTEGRATION,
     API_MAC,
+    API_SET_POINT,
     API_SYSTEM_ID,
     API_SYSTEM_PARAMS,
     API_SYSTEMS,
     API_V1,
     API_VERSION,
     API_WEBSERVER,
     API_ZONE_ID,
@@ -342,27 +345,33 @@
         if API_DATA not in res:
             if API_ERRORS in res:
                 self.handle_errors(res[API_ERRORS])
             raise APIError(f"set_hvac: {API_DATA} not in API response")
 
         data: dict[str, Any] = res[API_DATA][0]
         for key, value in params.items():
-            if key not in data or data[key] != value:
+            update_fail = key not in data
+
+            if not update_fail:
+                if key not in [API_COOL_SET_POINT, API_HEAT_SET_POINT, API_SET_POINT]:
+                    update_fail = data[key] != value
+
+            if update_fail:
                 if key == API_SYSTEM_ID and value != 0:
                     raise InvalidSystem(
                         f"set_hvac: System mismatch: {data.get(key)} vs {value}"
                     )
                 if key == API_ZONE_ID and value != 0:
                     raise InvalidZone(
                         f"set_hvac: Zone mismatch: {data.get(key)} vs {value}"
                     )
                 if key not in data:
                     raise InvalidParam(f"set_hvac: param not in data: {key}={value}")
                 raise ParamUpdateFailure(
-                    f"set_hvac: param update failure: {key}={value}"
+                    f"set_hvac: {key} update failure: {data.get(key)} vs {value}"
                 )
 
         system = self.get_system(data[API_SYSTEM_ID])
         zone = self.get_zone(data[API_SYSTEM_ID], data[API_ZONE_ID])
         for key, value in data.items():
             if key in API_SYSTEM_PARAMS:
                 system.set_param(key, value)
```

### Comparing `aioairzone-0.5.3/aioairzone/webserver.py` & `aioairzone-0.5.4/aioairzone/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.3/aioairzone.egg-info/PKG-INFO` & `aioairzone-0.5.4/aioairzone.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.5.3
+Version: 0.5.4
 Summary: Library to control Airzone devices
 Home-page: https://github.com/Noltari/aioairzone
 Download-URL: https://github.com/Noltari/aioairzone
 Author: Álvaro Fernández Rojas
 Author-email: noltari@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aioairzone-0.5.3/setup.py` & `aioairzone-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for aioairzone."""
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.5.3"
+VERSION = "0.5.4"
 
 
 setup(
     name="aioairzone",
     version=VERSION,
     url="https://github.com/Noltari/aioairzone",
     download_url="https://github.com/Noltari/aioairzone",
```


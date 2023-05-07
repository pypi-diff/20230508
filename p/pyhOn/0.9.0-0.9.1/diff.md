# Comparing `tmp/pyhOn-0.9.0.tar.gz` & `tmp/pyhOn-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.9.0.tar", last modified: Mon Apr 24 02:37:50 2023, max compression
+gzip compressed data, was "pyhOn-0.9.1.tar", last modified: Mon Apr 24 19:52:43 2023, max compression
```

## Comparing `pyhOn-0.9.0.tar` & `pyhOn-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:50.723829 pyhOn-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 02:37:39.000000 pyhOn-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-24 02:37:50.723829 pyhOn-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-24 02:37:39.000000 pyhOn-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:50.719829 pyhOn-0.9.0/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-24 02:37:50.000000 pyhOn-0.9.0/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 02:37:50.000000 pyhOn-0.9.0/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 02:37:50.000000 pyhOn-0.9.0/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 02:37:50.000000 pyhOn-0.9.0/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 02:37:50.000000 pyhOn-0.9.0/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 02:37:50.000000 pyhOn-0.9.0/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:50.719829 pyhOn-0.9.0/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:50.723829 pyhOn-0.9.0/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/appliances/dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:50.723829 pyhOn-0.9.0/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:50.723829 pyhOn-0.9.0/pyhon/connection/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/handler/anonym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/handler/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/handler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/connection/handler/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/hon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:50.723829 pyhOn-0.9.0/pyhon/parameter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/parameter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/parameter/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/parameter/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/parameter/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-24 02:37:39.000000 pyhOn-0.9.0/pyhon/parameter/range.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:37:50.723829 pyhOn-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-24 02:37:39.000000 pyhOn-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:43.872986 pyhOn-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 19:52:32.000000 pyhOn-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-24 19:52:43.872986 pyhOn-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-24 19:52:32.000000 pyhOn-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:43.868986 pyhOn-0.9.1/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-24 19:52:43.000000 pyhOn-0.9.1/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 19:52:43.000000 pyhOn-0.9.1/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:52:43.000000 pyhOn-0.9.1/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 19:52:43.000000 pyhOn-0.9.1/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 19:52:43.000000 pyhOn-0.9.1/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 19:52:43.000000 pyhOn-0.9.1/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:43.868986 pyhOn-0.9.1/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:43.868986 pyhOn-0.9.1/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/appliances/dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:43.872986 pyhOn-0.9.1/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:43.872986 pyhOn-0.9.1/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/hon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:43.872986 pyhOn-0.9.1/pyhon/parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/parameter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/parameter/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/parameter/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/parameter/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-24 19:52:32.000000 pyhOn-0.9.1/pyhon/parameter/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:52:43.872986 pyhOn-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-24 19:52:32.000000 pyhOn-0.9.1/setup.py
```

### Comparing `pyhOn-0.9.0/LICENSE` & `pyhOn-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/PKG-INFO` & `pyhOn-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.9.0
+Version: 0.9.1
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.9.0/README.md` & `pyhOn-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.9.1/pyhOn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.9.0
+Version: 0.9.1
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.9.0/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.9.1/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/__main__.py` & `pyhOn-0.9.1/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/appliance.py` & `pyhOn-0.9.1/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/appliances/ov.py` & `pyhOn-0.9.1/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/appliances/td.py` & `pyhOn-0.9.1/pyhon/appliances/td.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/commands.py` & `pyhOn-0.9.1/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/connection/api.py` & `pyhOn-0.9.1/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/connection/auth.py` & `pyhOn-0.9.1/pyhon/connection/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,21 +178,22 @@
             if response.status == 200:
                 with suppress(json.JSONDecodeError, KeyError):
                     result = await response.json()
                     return result["events"][0]["attributes"]["values"]["url"]
             await self._error_logger(response)
             return ""
 
-    def _parse_token_data(self, text: str) -> None:
+    def _parse_token_data(self, text: str) -> bool:
         if access_token := re.findall("access_token=(.*?)&", text):
             self._access_token = access_token[0]
         if refresh_token := re.findall("refresh_token=(.*?)&", text):
             self._refresh_token = refresh_token[0]
         if id_token := re.findall("id_token=(.*?)&", text):
             self._id_token = id_token[0]
+        return True if access_token and refresh_token and id_token else False
 
     async def _get_token(self, url: str) -> bool:
         async with self._request.get(url) as response:
             if response.status != 200:
                 await self._error_logger(response)
                 return False
             url_search = re.findall(
@@ -210,15 +211,17 @@
                     "href\\s*=\\s*[\"'](.*?)[\"']", await response.text()
                 )
         url = "/".join(const.AUTH_API.split("/")[:-1]) + url_search[0]
         async with self._request.get(url) as response:
             if response.status != 200:
                 await self._error_logger(response)
                 return False
-            self._parse_token_data(await response.text())
+            if not self._parse_token_data(await response.text()):
+                await self._error_logger(response)
+                return False
         return True
 
     async def _api_auth(self) -> bool:
         post_headers = {"id-token": self._id_token}
         data = self._device.get()
         async with self._request.post(
             f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
```

### Comparing `pyhOn-0.9.0/pyhon/connection/device.py` & `pyhOn-0.9.1/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/connection/handler/anonym.py` & `pyhOn-0.9.1/pyhon/connection/handler/anonym.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/connection/handler/auth.py` & `pyhOn-0.9.1/pyhon/connection/handler/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/connection/handler/base.py` & `pyhOn-0.9.1/pyhon/connection/handler/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/connection/handler/hon.py` & `pyhOn-0.9.1/pyhon/connection/handler/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/helper.py` & `pyhOn-0.9.1/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/hon.py` & `pyhOn-0.9.1/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/parameter/base.py` & `pyhOn-0.9.1/pyhon/parameter/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/parameter/enum.py` & `pyhOn-0.9.1/pyhon/parameter/enum.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/parameter/fixed.py` & `pyhOn-0.9.1/pyhon/parameter/fixed.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/parameter/program.py` & `pyhOn-0.9.1/pyhon/parameter/program.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/pyhon/parameter/range.py` & `pyhOn-0.9.1/pyhon/parameter/range.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.9.0/setup.py` & `pyhOn-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.9.0",
+    version="0.9.1",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```


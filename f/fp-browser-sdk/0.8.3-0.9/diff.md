# Comparing `tmp/fp_browser_sdk-0.8.3.tar.gz` & `tmp/fp_browser_sdk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fp_browser_sdk-0.8.3.tar", last modified: Mon Apr 10 11:49:43 2023, max compression
+gzip compressed data, was "dist/fp_browser_sdk-0.9.tar", last modified: Mon May  8 07:10:10 2023, max compression
```

## Comparing `fp_browser_sdk-0.8.3.tar` & `fp_browser_sdk-0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/
--rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/PKG-INFO
--rw-r--r--   0 leeyang    (501) staff       (20)     8453 2023-02-12 04:55:25.000000 fp_browser_sdk-0.8.3/README.md
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/
--rw-r--r--   0 leeyang    (501) staff       (20)    15571 2022-12-15 04:40:42.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/__init__.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/data/
--rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/data/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)   183083 2022-08-16 02:45:13.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/data/motion.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/
--rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)     6386 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/basic.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3212 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/battery.py
--rw-r--r--   0 leeyang    (501) staff       (20)    17258 2023-04-07 07:59:18.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/browser_enum.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3357 2023-03-13 13:15:24.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/client_hints.py
--rw-r--r--   0 leeyang    (501) staff       (20)     5336 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/device_motion.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2059 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/device_orientation.py
--rw-r--r--   0 leeyang    (501) staff       (20)     7142 2023-01-15 06:50:48.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/document.py
--rw-r--r--   0 leeyang    (501) staff       (20)      451 2022-08-07 03:58:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/exception.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3291 2023-04-10 11:49:02.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/fingerprint_offset.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1851 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/geo.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3266 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/header.py
--rw-r--r--   0 leeyang    (501) staff       (20)      465 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/inject_js.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2223 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/media.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2539 2022-08-05 07:15:01.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/module.py
--rw-r--r--   0 leeyang    (501) staff       (20)     6293 2023-01-15 06:50:48.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/navigator.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3917 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/network.py
--rw-r--r--   0 leeyang    (501) staff       (20)     9140 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/performance.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/
--rw-r--r--   0 leeyang    (501) staff       (20)      294 2022-09-18 13:15:09.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)    13786 2022-12-17 12:48:42.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type.py
--rw-r--r--   0 leeyang    (501) staff       (20)    12917 2022-09-18 13:09:11.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_102.py
--rw-r--r--   0 leeyang    (501) staff       (20)    12683 2022-12-17 12:48:42.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_107.py
--rw-r--r--   0 leeyang    (501) staff       (20)     9857 2022-09-18 13:09:11.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_88.py
--rw-r--r--   0 leeyang    (501) staff       (20)    10280 2022-09-18 13:09:11.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_90.py
--rw-r--r--   0 leeyang    (501) staff       (20)    11710 2022-09-18 13:09:11.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_93.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1049 2022-12-17 12:48:42.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/util.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2087 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/plugin.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3923 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/screen.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2343 2022-11-10 12:59:52.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/speech_synthesis_voice.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1678 2023-02-12 04:54:23.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/ext/webrtc.py
--rw-r--r--   0 leeyang    (501) staff       (20)      471 2022-11-11 04:36:45.000000 fp_browser_sdk-0.8.3/fp_browser_sdk/fp_browser_settings.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk.egg-info/
--rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk.egg-info/PKG-INFO
--rw-r--r--   0 leeyang    (501) staff       (20)     1448 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 leeyang    (501) staff       (20)        1 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 leeyang    (501) staff       (20)       15 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/fp_browser_sdk.egg-info/top_level.txt
--rw-r--r--   0 leeyang    (501) staff       (20)       38 2023-04-10 11:49:43.000000 fp_browser_sdk-0.8.3/setup.cfg
--rw-r--r--   0 leeyang    (501) staff       (20)      387 2023-04-10 11:49:31.000000 fp_browser_sdk-0.8.3/setup.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/
+-rw-r--r--   0 leeyang    (501) staff       (20)      262 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/PKG-INFO
+-rw-r--r--   0 leeyang    (501) staff       (20)     8453 2023-02-12 04:55:25.000000 fp_browser_sdk-0.9/README.md
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/
+-rw-r--r--   0 leeyang    (501) staff       (20)    15571 2022-12-15 04:40:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/__init__.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/data/
+-rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9/fp_browser_sdk/data/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)   183083 2022-08-16 02:45:13.000000 fp_browser_sdk-0.9/fp_browser_sdk/data/motion.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/
+-rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     6386 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/basic.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3212 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/battery.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    17258 2023-04-07 07:59:18.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/browser_enum.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3357 2023-03-13 13:15:24.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/client_hints.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     5336 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/device_motion.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2059 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/device_orientation.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     7142 2023-01-15 06:50:48.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/document.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      451 2022-08-07 03:58:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/exception.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3291 2023-04-10 11:49:02.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/fingerprint_offset.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1851 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/geo.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3266 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/header.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      465 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/inject_js.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2223 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/media.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2539 2022-08-05 07:15:01.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/module.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     6966 2023-05-08 07:08:22.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/navigator.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3917 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/network.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     9140 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/performance.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/
+-rw-r--r--   0 leeyang    (501) staff       (20)      294 2022-09-18 13:15:09.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    13786 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    12917 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_102.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    12683 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_107.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     9857 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_88.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    10280 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_90.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    11710 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_93.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1049 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/util.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2087 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/plugin.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3923 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/screen.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2343 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/speech_synthesis_voice.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1678 2023-02-12 04:54:23.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/webrtc.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      471 2022-11-11 04:36:45.000000 fp_browser_sdk-0.9/fp_browser_sdk/fp_browser_settings.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/
+-rw-r--r--   0 leeyang    (501) staff       (20)      262 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 leeyang    (501) staff       (20)     1448 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)        1 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)       15 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/top_level.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)       38 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/setup.cfg
+-rw-r--r--   0 leeyang    (501) staff       (20)      385 2023-05-08 07:10:04.000000 fp_browser_sdk-0.9/setup.py
```

### Comparing `fp_browser_sdk-0.8.3/README.md` & `fp_browser_sdk-0.9/README.md`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/__init__.py` & `fp_browser_sdk-0.9/fp_browser_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/data/motion.py` & `fp_browser_sdk-0.9/fp_browser_sdk/data/motion.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/basic.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/basic.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/battery.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/battery.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/browser_enum.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/browser_enum.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/client_hints.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/client_hints.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/device_motion.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/device_motion.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/device_orientation.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/device_orientation.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/document.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/document.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/fingerprint_offset.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/fingerprint_offset.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/geo.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/geo.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/header.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/header.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/media.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/media.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/module.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/module.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/navigator.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/navigator.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 class Navigator(Module):
     def __init__(self):
         super(Navigator, self).__init__()
         self._user_agent = None
         self._user_agent_auto_match = True
         self._reduced_major_in_minor_version_number = False
+        self._navigator_app_version = None
+        self._navigator_product_sub = None
         self._webdriver_status = False
         self._platform = Platform.LINUX_ARMV8L
         self._vendor = 'Google Inc.'
         self._max_touch_points = MaxTouchPoint.MOBILE
         self._hardware_concurrency = 8
         self._device_memory = 4
         self._do_not_track = None
@@ -51,14 +53,20 @@
             "navigator.java-enabled": self._bool_to_int(self._java_enabled),
             "navigator.pdf-viewer-enabled": self._bool_to_int(self._pdf_viewer_enabled),
             "navigator.bluetooth-availability": self._bool_to_int(self._bluetooth_availability),
             "navigator.locale": self._locale,
             "navigator.languages": self._languages,
         }
 
+        if self._navigator_app_version is not None:
+            result["navigator.app_version"] = self._navigator_app_version
+
+        if self._navigator_product_sub is not None:
+            result["navigator.product_sub"] = self._navigator_product_sub
+
         if self._do_not_track is not None:
             result["navigator.do-not-track"] = self._do_not_track.value
 
         return result
 
     def set_user_agent(self, value: str):
         """
@@ -77,14 +85,28 @@
     def set_reduced_major_in_minor_version_number(self, value: bool):
         """
         强制只获取主版本号（例如：把 96.0.4664.104 变成 96.0.0.0）
         """
         self._reduced_major_in_minor_version_number = value
         return self
 
+    def set_navigator_app_version(self, value: str):
+        """
+        设置  appVersion
+        """
+        self._navigator_app_version = value
+        return self
+
+    def set_navigator_product_sub(self, value: str):
+        """
+        设置 productSub
+        """
+        self._navigator_product_sub = value
+        return self
+
     def set_webdriver_status(self, value: bool):
         """
         设置  webdriver 状态
         """
         self._webdriver_status = value
         return self
 
@@ -195,14 +217,14 @@
 
     def set_performance_type(self, value: PerformanceNavigationType):
         """
         如何导航到该页面
         """
         self._performance_type = value
         return self
-    
+
     def set_performance_redirect_count(self, value: int):
         """
         如果有重定向的话，页面通过几次重定向跳转而来，默认为0
         """
         self._performance_redirect_count = value
         return self
```

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/network.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/network.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/performance.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/performance.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_102.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_102.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_107.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_107.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_88.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_88.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_90.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_90.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/permission_type_93.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_93.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/permission_types/util.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/util.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/plugin.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/plugin.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/screen.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/screen.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/speech_synthesis_voice.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/speech_synthesis_voice.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk/ext/webrtc.py` & `fp_browser_sdk-0.9/fp_browser_sdk/ext/webrtc.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.8.3/fp_browser_sdk.egg-info/SOURCES.txt` & `fp_browser_sdk-0.9/fp_browser_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


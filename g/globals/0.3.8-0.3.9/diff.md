# Comparing `tmp/globals-0.3.8.tar.gz` & `tmp/globals-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globals-0.3.8.tar", last modified: Wed Nov  3 23:58:34 2021, max compression
+gzip compressed data, was "globals-0.3.9.tar", last modified: Thu Nov  4 00:50:46 2021, max compression
```

## Comparing `globals-0.3.8.tar` & `globals-0.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2021-11-03 23:58:34.625254 globals-0.3.8/
--rw-rw-rw-   0        0        0      672 2021-11-03 23:58:34.626252 globals-0.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-11-03 23:58:34.621274 globals-0.3.8/globals/
--rw-rw-rw-   0        0        0      385 2021-03-15 03:33:20.000000 globals-0.3.8/globals/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-03 23:58:34.615283 globals-0.3.8/globals/api/
-drwxrwxrwx   0        0        0        0 2021-11-03 23:58:34.615283 globals-0.3.8/globals/api/src/
-drwxrwxrwx   0        0        0        0 2021-11-03 23:58:34.624259 globals-0.3.8/globals/api/src/service/
--rw-rw-rw-   0        0        0    36317 2021-11-02 06:41:11.059798 globals-0.3.8/globals/api/src/service/GlobalsManager.py
--rw-rw-rw-   0        0        0       42 2020-07-03 06:07:22.000000 globals-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1117 2021-11-03 23:56:46.391144 globals-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-11-04 00:50:46.508006 globals-0.3.9/
+-rw-rw-rw-   0        0        0      672 2021-11-04 00:50:46.509003 globals-0.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-11-04 00:50:46.505015 globals-0.3.9/globals/
+-rw-rw-rw-   0        0        0      385 2021-03-15 03:33:20.000000 globals-0.3.9/globals/__init__.py
+drwxrwxrwx   0        0        0        0 2021-11-04 00:50:46.499031 globals-0.3.9/globals/api/
+drwxrwxrwx   0        0        0        0 2021-11-04 00:50:46.499031 globals-0.3.9/globals/api/src/
+drwxrwxrwx   0        0        0        0 2021-11-04 00:50:46.507011 globals-0.3.9/globals/api/src/service/
+-rw-rw-rw-   0        0        0    36318 2021-11-04 00:30:48.452873 globals-0.3.9/globals/api/src/service/GlobalsManager.py
+-rw-rw-rw-   0        0        0       42 2020-07-03 06:07:22.000000 globals-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2021-11-04 00:48:52.935320 globals-0.3.9/setup.py
```

### Comparing `globals-0.3.8/PKG-INFO` & `globals-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: globals
-Version: 0.3.8
+Version: 0.3.9
 Summary: import package handler
 Home-page: https://github.com/SamuelJansen/globals/
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
-Download-URL: https://github.com/SamuelJansen/globals/archive/v0.3.8.tar.gz
+Download-URL: https://github.com/SamuelJansen/globals/archive/v0.3.9.tar.gz
 Description: UNKNOWN
 Keywords: global,python global package,python package manager,global package manager
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `globals-0.3.8/globals/api/src/service/GlobalsManager.py` & `globals-0.3.9/globals/api/src/service/GlobalsManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         logsWithColors = DEFAULT_LOGS_WITH_COLORS,
         encoding = c.ENCODING,
         printRootPathStatus = False,
         globalsEverything = False
     ):
 
         if globalsInstanceIsNone() :
-            
-            self.logsWithColors = EnvironmentHelper.update(log.ENABLE_LOGS_WITH_COLORS, logsWithColors or SettingHelper.activeEnvironmentIsLocal())
+
+            self.logsWithColors = EnvironmentHelper.update(log.ENABLE_LOGS_WITH_COLORS, logsWithColors or log.colorsEnabled(), default=DEFAULT_LOGS_WITH_COLORS)
 
             self.logStatus = EnvironmentHelper.update(log.LOG, logStatus, default=DEFAULT_LOG_STATUS)
             self.infoStatus = EnvironmentHelper.update(log.INFO, infoStatus, default=DEFAULT_INFO_STATUS)
             self.statusStatus = EnvironmentHelper.update(log.STATUS, statusStatus, default=DEFAULT_STATUS_STATUS)
             self.successStatus = EnvironmentHelper.update(log.SUCCESS, successStatus, default=DEFAULT_SUCCESS_STATUS)
             self.settingStatus = EnvironmentHelper.update(log.SETTING, settingStatus, default=DEFAULT_SETTING_STATUS)
             self.debugStatus = EnvironmentHelper.update(log.DEBUG, debugStatus, default=DEFAULT_DEBUG_STATUS)
```

### Comparing `globals-0.3.8/setup.py` & `globals-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from distutils.core import setup
 import os
 
-version = '0.3.8'
+version = '0.3.9'
 name = 'globals'
 url = f'https://github.com/SamuelJansen/{name}/'
 
 OS_SEPARATOR = os.path.sep
 
 setup(
     name = name,
```


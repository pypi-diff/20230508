# Comparing `tmp/eptools-8.5.6.tar.gz` & `tmp/eptools-8.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\EasypostLibrary\eptools\dist\tmpqu9r0_6q\eptools-8.5.6.tar", last modified: Tue Apr 25 13:26:38 2023, max compression
+gzip compressed data, was "c:\EasypostLibrary\eptools\dist\tmpwj91j_5i\eptools-8.5.8.tar", last modified: Mon May  8 10:05:42 2023, max compression
```

## Comparing `eptools-8.5.6.tar` & `eptools-8.5.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.000000 eptools-8.5.6/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.000000 eptools-8.5.6/eptools/
--rw-rw-rw-   0        0        0      759 2022-10-20 08:53:57.000000 eptools-8.5.6/eptools/configuration.py
--rw-rw-rw-   0        0        0     6313 2022-06-28 08:12:23.000000 eptools-8.5.6/eptools/InvoiceDate.py
--rw-rw-rw-   0        0        0     9099 2023-03-24 15:00:32.000000 eptools-8.5.6/eptools/logger.py
--rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.5.6/eptools/mail_factory.py
--rw-rw-rw-   0        0        0    21143 2023-04-25 12:44:02.000000 eptools-8.5.6/eptools/SalesForceApiIntegration.py
--rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.5.6/eptools/sf_factory.py
--rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.5.6/eptools/slacker.py
--rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.5.6/eptools/slack_factory.py
--rw-rw-rw-   0        0        0    12117 2023-04-04 16:10:33.000000 eptools-8.5.6/eptools/SQLFactory.py
--rw-rw-rw-   0        0        0    31294 2023-03-24 15:03:41.000000 eptools-8.5.6/eptools/WindowsServiceBase.py
--rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.5.6/eptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.000000 eptools-8.5.6/eptools.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-25 13:26:38.000000 eptools-8.5.6/eptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      944 2023-04-25 13:26:38.000000 eptools-8.5.6/eptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-04-25 13:26:38.000000 eptools-8.5.6/eptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      469 2023-04-25 13:26:38.000000 eptools-8.5.6/eptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 13:26:38.000000 eptools-8.5.6/eptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.5.6/LICENSE
--rw-rw-rw-   0        0        0      944 2023-04-25 13:26:38.000000 eptools-8.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.5.6/pyproject.toml
--rw-rw-rw-   0        0        0      500 2022-03-29 12:52:14.000000 eptools-8.5.6/README.md
--rw-rw-rw-   0        0        0      588 2023-04-25 13:26:38.000000 eptools-8.5.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:05:42.000000 eptools-8.5.8/
+drwxrwxrwx   0        0        0        0 2023-05-08 10:05:42.000000 eptools-8.5.8/eptools/
+-rw-rw-rw-   0        0        0      792 2023-04-27 15:46:33.000000 eptools-8.5.8/eptools/configuration.py
+-rw-rw-rw-   0        0        0     6313 2022-06-28 08:12:23.000000 eptools-8.5.8/eptools/InvoiceDate.py
+-rw-rw-rw-   0        0        0     9196 2023-04-27 15:50:12.000000 eptools-8.5.8/eptools/logger.py
+-rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.5.8/eptools/mail_factory.py
+-rw-rw-rw-   0        0        0    17637 2023-04-26 14:43:11.000000 eptools-8.5.8/eptools/SalesForceApiIntegration.py
+-rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.5.8/eptools/sf_factory.py
+-rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.5.8/eptools/slacker.py
+-rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.5.8/eptools/slack_factory.py
+-rw-rw-rw-   0        0        0    12121 2023-04-27 15:51:48.000000 eptools-8.5.8/eptools/SQLFactory.py
+-rw-rw-rw-   0        0        0    31294 2023-03-24 15:03:41.000000 eptools-8.5.8/eptools/WindowsServiceBase.py
+-rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.5.8/eptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:05:42.000000 eptools-8.5.8/eptools.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:05:41.000000 eptools-8.5.8/eptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      944 2023-05-08 10:05:41.000000 eptools-8.5.8/eptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-05-08 10:05:41.000000 eptools-8.5.8/eptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      469 2023-05-08 10:05:41.000000 eptools-8.5.8/eptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 10:05:41.000000 eptools-8.5.8/eptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.5.8/LICENSE
+-rw-rw-rw-   0        0        0      944 2023-05-08 10:05:42.000000 eptools-8.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0      500 2022-03-29 12:52:14.000000 eptools-8.5.8/README.md
+-rw-rw-rw-   0        0        0      588 2023-05-08 10:05:42.000000 eptools-8.5.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.5.8/setup.py
```

### Comparing `eptools-8.5.6/eptools/configuration.py` & `eptools-8.5.8/eptools/configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 C_DEFAULT_CONFIG_PATH = "c:\\Software\\Configs\\eptools.json"
+C_DEFAULT_LOG_PATH = "c:\\Logs"
 
 def getglobals():
     return globals()
 
 def setglobals(new_globals):
     globals().update(new_globals)
```

### Comparing `eptools-8.5.6/eptools/InvoiceDate.py` & `eptools-8.5.8/eptools/InvoiceDate.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.6/eptools/logger.py` & `eptools-8.5.8/eptools/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from distutils.command.config import config
+from datetime import datetime
 import logging
 from logging.handlers import RotatingFileHandler
 from eptools.slack_factory import SlackFactory
 import os
 from inspect import getframeinfo, stack
 import traceback
 
@@ -76,14 +76,15 @@
         self.slack_logger = None
         self.config_path = config_path
         self.name = name
         if not name:
             self.name = "AnonymousLogger"
         self._svc_logger_ = self.name + '_logger'
         if logpath:
+            self.name = self.name + f'{(datetime.now()).strftime("%Y-%m-%d_%H-%M-%S")}.json'.replace(' ','_')
             self._svc_logpath_ = logpath + self.name + '\\'
         else:
             self._svc_logpath_ = '\\\\10.10.10.12\\F-drive\\Shares\\IT\\ServiceLogs\\' + self.name + '\\'
         if not os.path.exists(self._svc_logpath_):
             os.makedirs(self._svc_logpath_)
         self.file_logger = createRotatingLogger(self._svc_logger_ , self._svc_logpath_)
         self.slack_logger = createSlackLogger(self.name,logger=self.file_logger,config_path=self.config_path)
```

### Comparing `eptools-8.5.6/eptools/mail_factory.py` & `eptools-8.5.8/eptools/mail_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.6/eptools/sf_factory.py` & `eptools-8.5.8/eptools/sf_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.6/eptools/slacker.py` & `eptools-8.5.8/eptools/slacker.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.6/eptools/slack_factory.py` & `eptools-8.5.8/eptools/slack_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.6/eptools/SQLFactory.py` & `eptools-8.5.8/eptools/SQLFactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,11 +351,11 @@
     #     data = con.fetchall()
     #     print(data)
     # con2 = SQLFactory(SQLConnection.PRINTDB)
     # con2.execute("SELECT * FROM [EasyPost].[dbo].[Companies] where id = 7255;")
     # data = con2.fetchall()
     # con2.close_all()
 
-    with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools_1.json') as conn:
-        conn.execute("Select * from sysdatabases;")
+    with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json') as conn:
+        conn.execute("Select * from sysdatabasescxwcwx;")
         data = conn.fetchall(withColumns=True)
         print(data)
```

### Comparing `eptools-8.5.6/eptools/WindowsServiceBase.py` & `eptools-8.5.8/eptools/WindowsServiceBase.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.6/eptools.egg-info/PKG-INFO` & `eptools-8.5.8/eptools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.5.6
+Version: 8.5.8
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.5.6/LICENSE` & `eptools-8.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eptools-8.5.6/PKG-INFO` & `eptools-8.5.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.5.6
+Version: 8.5.8
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.5.6/setup.cfg` & `eptools-8.5.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7074 6f6f 6c73 0d0a 7665 7273   = eptools..vers
-00000020: 696f 6e20 3d20 382e 352e 360d 0a61 7574  ion = 8.5.6..aut
+00000020: 696f 6e20 3d20 382e 352e 380d 0a61 7574  ion = 8.5.8..aut
 00000030: 686f 7220 3d20 4172 6e6f 2044 6520 4465  hor = Arno De De
 00000040: 636b 6572 0d0a 6175 7468 6f72 5f65 6d61  cker..author_ema
 00000050: 696c 203d 2061 726e 6f2e 6465 6465 636b  il = arno.dedeck
 00000060: 6572 4065 6173 7970 6f73 742e 6575 0d0a  er@easypost.eu..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4561  description = Ea
 00000080: 7379 506f 7374 2054 6f6f 6c73 0d0a 6c6f  syPost Tools..lo
 00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
```


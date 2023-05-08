# Comparing `tmp/pybeans-1.7.3.tar.gz` & `tmp/pybeans-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybeans-1.7.3.tar", last modified: Fri May 13 02:30:45 2022, max compression
+gzip compressed data, was "dist/pybeans-1.7.4.tar", last modified: Mon May  8 12:07:39 2023, max compression
```

## Comparing `pybeans-1.7.3.tar` & `pybeans-1.7.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-13 02:30:45.000000 pybeans-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-05-13 02:30:30.000000 pybeans-1.7.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-05-13 02:30:45.000000 pybeans-1.7.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-13 02:30:45.000000 pybeans-1.7.3/pybeans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-05-13 02:30:45.000000 pybeans-1.7.3/pybeans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-13 02:30:45.000000 pybeans-1.7.3/pybeans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-05-13 02:30:45.000000 pybeans-1.7.3/pybeans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-13 02:30:45.000000 pybeans-1.7.3/pybeans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-13 02:30:45.000000 pybeans-1.7.3/pybeans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-05-13 02:30:30.000000 pybeans-1.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-13 02:30:45.000000 pybeans-1.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-13 02:30:45.000000 pybeans-1.7.3/pybeans/
--rw-r--r--   0 runner    (1001) docker     (121)    14596 2022-05-13 02:30:30.000000 pybeans-1.7.3/pybeans/app_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)    21969 2022-05-13 02:30:30.000000 pybeans-1.7.3/pybeans/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-13 02:30:30.000000 pybeans-1.7.3/pybeans/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-05-13 02:30:30.000000 pybeans-1.7.3/pybeans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-05-13 02:30:30.000000 pybeans-1.7.3/pybeans/config_sample.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-05-13 02:30:30.000000 pybeans-1.7.3/pybeans/get_ch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-05-13 02:30:30.000000 pybeans-1.7.3/pybeans/ColorfulFormatter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:07:39.000000 pybeans-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:07:39.000000 pybeans-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-08 12:07:25.000000 pybeans-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:07:39.000000 pybeans-1.7.4/pybeans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-08 12:07:39.000000 pybeans-1.7.4/pybeans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-08 12:07:25.000000 pybeans-1.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:07:39.000000 pybeans-1.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:07:39.000000 pybeans-1.7.4/pybeans/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15388 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/app_tool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/ColorfulFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/get_ch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/config_sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/utils.py
```

### Comparing `pybeans-1.7.3/setup.py` & `pybeans-1.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NAME = 'pybeans'
 DESCRIPTION = 'Common toolkit for python.'
 PY_MODULES = ['pybeans']
 PACKAGES = ['pybeans']
 URL = 'https://github.com/chariothy/pybeans.git'
 EMAIL = 'chariothy@gmail.com'
 AUTHOR = 'Henry TIAN'
-VERSION = '1.7.3'
+VERSION = '1.7.4'
 
 LONG_DESCRIPTION = '''
 This is a helper which includes common methods and classes.
 
 '''
 
 # What packages are required for this module to be executed?
```

### Comparing `pybeans-1.7.3/PKG-INFO` & `pybeans-1.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.3
+Version: 1.7.4
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.3/pybeans.egg-info/PKG-INFO` & `pybeans-1.7.4/pybeans.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.3
+Version: 1.7.4
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.3/README.md` & `pybeans-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.3/pybeans/app_tool.py` & `pybeans-1.7.4/pybeans/app_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os, sys, logging
+from logging import handlers
 from os import path
 from email.utils import formataddr
 from collections.abc import Iterable
-from logging import handlers
 import functools
 import time
 import re
 import traceback
 from typing import Union
 from pprint import pformat
 from colorama import Fore, Back, init, Style
@@ -112,15 +112,15 @@
         assert(type(local_config_dir) == str)
 
         sys.path.append(self._app_path)
         try:
             self._config = __import__(config_name).CONFIG
         except Exception:
             self._config = {}
-
+        
         config_local_path = path.join(self._app_path, local_config_dir)
         sys.path.append(config_local_path)
         try:
             config_local = __import__(config_name + '_local').CONFIG
             self._config = deep_merge(self._config, config_local)
         except Exception:
             pass
@@ -143,62 +143,77 @@
 
     def init_logger(self) -> logging.Logger:
         """Initialize logger
         
         Returns:
             [logger] -- Initialized logger.
         """
-
+        
         smtp = self._config.get('smtp')
         mail = self._config.get('mail')
         logConfig = self._config.get('log', {})
 
         logs_path = path.join(self._app_path, 'logs')
         if not os.path.exists(logs_path):
             os.mkdir(logs_path)
 
         logger = logging.getLogger(self._app_name)
         logLevel = logConfig.get('level', logging.DEBUG)
         logger.setLevel(logLevel)
 
         logDst = logConfig.get('dest', {})
 
-        fileDest = logDst.get('file', 1)
-        if fileDest == 1:
+        fileDest = logDst.get('file')
+        if fileDest is not None:
+            if not fileDest: # Empty
+                regular_log_name = re.sub(r'\W+', '_', self._app_name.lower())
+                fileDest = path.join(logs_path, f'{regular_log_name}.log')
             regular_log_name = re.sub(r'\W+', '_', self._app_name.lower())
-            rf_handler = handlers.TimedRotatingFileHandler(path.join(logs_path, f'{regular_log_name}.log'), when='D', interval=1, backupCount=7, encoding='utf-8')
+            rf_handler = handlers.TimedRotatingFileHandler(fileDest, when='D', interval=1, backupCount=7, encoding='utf-8')
             rf_handler.suffix = "%Y-%m-%d_%H-%M-%S.log"
             rf_handler.level = logging.INFO
             rf_handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
             logger.addHandler(rf_handler)
 
         mailDest = logDst.get('mail')
-        if smtp and mailDest == 1:
+        if smtp and mailDest is not None:
             from_addr = mail.get('from')
             #TODO: Use schema to validate smtp
-            if mailDest == 1:
+            if not mailDest:    # Empty
                 to_addrs = mail.get('to')
             else:   # Ex. 'Henry TIAN <chariothy@gmail.com>'
                 to_addrs = mailDest
 
             mail_handler = MySMTPHandler(
                     mailhost = (smtp['host'], smtp['port']),
                     fromaddr = from_addr,
                     toaddrs = to_addrs,
                     subject = '%(name)s - %(levelname)s - %(message)s',
                     credentials = (smtp['user'], smtp['pwd']))
             mail_handler.setLevel(logging.ERROR)
             logger.addHandler(mail_handler)
 
-        stdoutDest = logDst.get('stdout', 1)
-        if stdoutDest == 1:
+        stdoutDest = logDst.get('stdout')
+        if stdoutDest is not None:
             st_handler = logging.StreamHandler()
             st_handler.level = logging.DEBUG
             st_handler.setFormatter(ColorfulFormatter())
             logger.addHandler(st_handler)
+            
+        syslogDest = logDst.get('syslog')
+        if syslogDest is not None:
+            sl_handler = logging.handlers.SysLogHandler(address=tuple(syslogDest))
+            sl_handler.level = logging.DEBUG
+            formatterDict = logConfig.get('formatter', {})
+            syslogFormatter = formatterDict.get('syslog', None)
+            if not syslogFormatter:
+                syslogFormatter = f'{self._app_name}[%(process)d]: %(filename)s[%(lineno)d] - %(message)s'
+            sl_handler.setFormatter(logging.Formatter(syslogFormatter))
+            logger.addHandler(sl_handler)
+
         self._logger = logger
         return logger
 
 
     def send_email(self, subject: str, text_body: str='', from_addr: str=None, to_addrs:str=None, html_body: str=None, 
         image_paths: tuple=None, file_paths: tuple=None, 
         debug: bool=False, send_to_file: bool=False, email_file_dir=None) -> dict:
```

### Comparing `pybeans-1.7.3/pybeans/utils.py` & `pybeans-1.7.4/pybeans/utils.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.3/pybeans/get_ch.py` & `pybeans-1.7.4/pybeans/get_ch.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.3/pybeans/ColorfulFormatter.py` & `pybeans-1.7.4/pybeans/ColorfulFormatter.py`

 * *Files identical despite different names*


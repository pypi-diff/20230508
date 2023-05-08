# Comparing `tmp/pybeans-1.7.4.tar.gz` & `tmp/pybeans-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybeans-1.7.4.tar", last modified: Mon May  8 12:07:39 2023, max compression
+gzip compressed data, was "dist/pybeans-1.7.5.tar", last modified: Mon May  8 12:21:06 2023, max compression
```

## Comparing `pybeans-1.7.4.tar` & `pybeans-1.7.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:07:39.000000 pybeans-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:07:39.000000 pybeans-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-08 12:07:25.000000 pybeans-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:07:39.000000 pybeans-1.7.4/pybeans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-08 12:07:38.000000 pybeans-1.7.4/pybeans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-08 12:07:39.000000 pybeans-1.7.4/pybeans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-08 12:07:25.000000 pybeans-1.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:07:39.000000 pybeans-1.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:07:39.000000 pybeans-1.7.4/pybeans/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/exception.py
--rw-r--r--   0 runner    (1001) docker     (122)    15388 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/app_tool.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/ColorfulFormatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/get_ch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/config_sample.py
--rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-08 12:07:25.000000 pybeans-1.7.4/pybeans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:21:06.000000 pybeans-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:21:06.000000 pybeans-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-08 12:20:54.000000 pybeans-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:21:06.000000 pybeans-1.7.5/pybeans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-08 12:21:06.000000 pybeans-1.7.5/pybeans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-08 12:20:54.000000 pybeans-1.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:21:06.000000 pybeans-1.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:21:06.000000 pybeans-1.7.5/pybeans/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15361 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/app_tool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/ColorfulFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/get_ch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/config_sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/utils.py
```

### Comparing `pybeans-1.7.4/PKG-INFO` & `pybeans-1.7.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.4
+Version: 1.7.5
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.4/setup.py` & `pybeans-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NAME = 'pybeans'
 DESCRIPTION = 'Common toolkit for python.'
 PY_MODULES = ['pybeans']
 PACKAGES = ['pybeans']
 URL = 'https://github.com/chariothy/pybeans.git'
 EMAIL = 'chariothy@gmail.com'
 AUTHOR = 'Henry TIAN'
-VERSION = '1.7.4'
+VERSION = '1.7.5'
 
 LONG_DESCRIPTION = '''
 This is a helper which includes common methods and classes.
 
 '''
 
 # What packages are required for this module to be executed?
```

### Comparing `pybeans-1.7.4/pybeans.egg-info/PKG-INFO` & `pybeans-1.7.5/pybeans.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.4
+Version: 1.7.5
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.4/README.md` & `pybeans-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.4/pybeans/app_tool.py` & `pybeans-1.7.5/pybeans/app_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         syslogDest = logDst.get('syslog')
         if syslogDest is not None:
             sl_handler = logging.handlers.SysLogHandler(address=tuple(syslogDest))
             sl_handler.level = logging.DEBUG
             formatterDict = logConfig.get('formatter', {})
             syslogFormatter = formatterDict.get('syslog', None)
             if not syslogFormatter:
-                syslogFormatter = f'{self._app_name}[%(process)d]: %(filename)s[%(lineno)d] - %(message)s'
+                syslogFormatter = f'{self._app_name}[%(process)d]: %(message)s'
             sl_handler.setFormatter(logging.Formatter(syslogFormatter))
             logger.addHandler(sl_handler)
 
         self._logger = logger
         return logger
```

### Comparing `pybeans-1.7.4/pybeans/ColorfulFormatter.py` & `pybeans-1.7.5/pybeans/ColorfulFormatter.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.4/pybeans/get_ch.py` & `pybeans-1.7.5/pybeans/get_ch.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.4/pybeans/config_sample.py` & `pybeans-1.7.5/pybeans/config_sample.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.4/pybeans/utils.py` & `pybeans-1.7.5/pybeans/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/threadsafevariable-1.2.tar.gz` & `tmp/threadsafevariable-20230507.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/threadsafevariable-1.2.tar", last modified: Thu Dec  9 09:00:15 2021, max compression
+gzip compressed data, was "threadsafevariable-20230507.1.tar", last modified: Mon May  8 00:16:58 2023, max compression
```

## Comparing `threadsafevariable-1.2.tar` & `threadsafevariable-20230507.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2021-12-09 09:00:15.000000 threadsafevariable-1.2/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     1291 2021-12-09 09:00:15.000000 threadsafevariable-1.2/PKG-INFO
--rw-rw-r--   0 mdp       (1000) mdp       (1000)       38 2021-12-09 09:00:15.000000 threadsafevariable-1.2/setup.cfg
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2021-12-09 09:00:15.000000 threadsafevariable-1.2/threadsafevariable/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)      846 2021-12-09 08:59:35.000000 threadsafevariable-1.2/threadsafevariable/__init__.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2021-12-09 09:00:15.000000 threadsafevariable-1.2/threadsafevariable.egg-info/
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1291 2021-12-09 09:00:15.000000 threadsafevariable-1.2/threadsafevariable.egg-info/PKG-INFO
--rw-r--r--   0 mdp       (1000) mdp       (1000)       19 2021-12-09 09:00:15.000000 threadsafevariable-1.2/threadsafevariable.egg-info/top_level.txt
--rw-r--r--   0 mdp       (1000) mdp       (1000)        1 2021-12-09 09:00:15.000000 threadsafevariable-1.2/threadsafevariable.egg-info/dependency_links.txt
--rw-r--r--   0 mdp       (1000) mdp       (1000)      258 2021-12-09 09:00:15.000000 threadsafevariable-1.2/threadsafevariable.egg-info/SOURCES.txt
--rw-r--r--   0 mdp       (1000) mdp       (1000)        1 2019-07-23 06:13:34.000000 threadsafevariable-1.2/threadsafevariable.egg-info/not-zip-safe
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1519 2021-12-09 08:37:44.000000 threadsafevariable-1.2/setup.py
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1529 2019-07-23 06:13:34.000000 threadsafevariable-1.2/README.md
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:16:58.889182 threadsafevariable-20230507.1/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2018 2023-05-08 00:16:58.873182 threadsafevariable-20230507.1/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1529 2019-07-23 06:13:34.000000 threadsafevariable-20230507.1/README.md
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      498 2023-05-08 00:13:37.000000 threadsafevariable-20230507.1/pyproject.toml
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-08 00:16:58.889182 threadsafevariable-20230507.1/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:16:58.849181 threadsafevariable-20230507.1/tests/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      934 2021-02-08 01:58:00.000000 threadsafevariable-20230507.1/tests/test_tsv.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:16:58.849181 threadsafevariable-20230507.1/threadsafevariable/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      845 2023-05-08 00:12:36.000000 threadsafevariable-20230507.1/threadsafevariable/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:16:58.873182 threadsafevariable-20230507.1/threadsafevariable.egg-info/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2018 2023-05-08 00:16:58.000000 threadsafevariable-20230507.1/threadsafevariable.egg-info/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      241 2023-05-08 00:16:58.000000 threadsafevariable-20230507.1/threadsafevariable.egg-info/SOURCES.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:16:58.000000 threadsafevariable-20230507.1/threadsafevariable.egg-info/dependency_links.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       19 2023-05-08 00:16:58.000000 threadsafevariable-20230507.1/threadsafevariable.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `threadsafevariable-1.2/threadsafevariable/__init__.py` & `threadsafevariable-20230507.1/threadsafevariable/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import copy
 import threading
 
 
-__version__ = 1.2
+__version__ = 20230507.1
 
 
 class ThreadSafeVariable:
 
     storage = threading.local()
     master_thread = threading.current_thread()
     defaults = {}
 
     def __set__(self, instance, value):
         key = "%s.%s" % (id(instance), id(self))
         if self.master_thread == threading.current_thread():
             self.defaults[key] = value
-        setattr(self.storage, key, value)        
+        setattr(self.storage, key, value)
 
     def __get__(self, instance, owner):
         key = "%s.%s" % (id(instance), id(self))
         return getattr(
             self.storage,
             key,
             self.defaults.get(key))
```

### Comparing `threadsafevariable-1.2/README.md` & `threadsafevariable-20230507.1/README.md`

 * *Files identical despite different names*


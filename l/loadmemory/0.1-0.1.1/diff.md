# Comparing `tmp/loadmemory-0.1.tar.gz` & `tmp/loadmemory-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadmemory-0.1.tar", last modified: Fri Apr 28 11:03:49 2023, max compression
+gzip compressed data, was "loadmemory-0.1.1.tar", last modified: Mon May  8 09:09:06 2023, max compression
```

## Comparing `loadmemory-0.1.tar` & `loadmemory-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-28 11:03:49.945979 loadmemory-0.1/
--rw-r--r--   0 zhouwei    (501) staff       (20)      343 2023-04-28 11:03:49.945853 loadmemory-0.1/PKG-INFO
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-28 11:03:49.945014 loadmemory-0.1/loadmemory.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)      343 2023-04-28 11:03:49.000000 loadmemory-0.1/loadmemory.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)      203 2023-04-28 11:03:49.000000 loadmemory-0.1/loadmemory.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-04-28 11:03:49.000000 loadmemory-0.1/loadmemory.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        6 2023-04-28 11:03:49.000000 loadmemory-0.1/loadmemory.egg-info/top_level.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-04-28 11:03:49.946027 loadmemory-0.1/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)      616 2023-04-28 11:00:14.000000 loadmemory-0.1/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-28 11:03:49.945632 loadmemory-0.1/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       45 2023-04-28 11:00:14.000000 loadmemory-0.1/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      234 2023-04-28 11:00:14.000000 loadmemory-0.1/utils/configparser.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      459 2023-04-28 11:00:14.000000 loadmemory-0.1/utils/time_util.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-08 09:09:06.246003 loadmemory-0.1.1/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      345 2023-05-08 09:09:06.245853 loadmemory-0.1.1/PKG-INFO
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-08 09:09:06.244243 loadmemory-0.1.1/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-05-04 09:19:02.000000 loadmemory-0.1.1/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      674 2023-05-08 08:59:40.000000 loadmemory-0.1.1/db/tiny_db.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-08 09:09:06.244985 loadmemory-0.1.1/loadmemory.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      345 2023-05-08 09:09:06.000000 loadmemory-0.1.1/loadmemory.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)      232 2023-05-08 09:09:06.000000 loadmemory-0.1.1/loadmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-05-08 09:09:06.000000 loadmemory-0.1.1/loadmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        9 2023-05-08 09:09:06.000000 loadmemory-0.1.1/loadmemory.egg-info/top_level.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-05-08 09:09:06.246050 loadmemory-0.1.1/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)      638 2023-05-08 09:09:04.000000 loadmemory-0.1.1/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-08 09:09:06.245653 loadmemory-0.1.1/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       45 2023-04-28 11:00:14.000000 loadmemory-0.1.1/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      234 2023-04-28 11:00:14.000000 loadmemory-0.1.1/utils/configparser.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      459 2023-04-28 11:00:14.000000 loadmemory-0.1.1/utils/time_util.py
```

### Comparing `loadmemory-0.1/setup.py` & `loadmemory-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python3.8+
 # -*- coding:utf-8 -*-
 import setuptools
 
 setuptools.setup(
     name="loadmemory",
-    version="0.1",
+    version="0.1.1",
 
     description="tools",
     long_description="tools",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     url="https://github.com/zhouwe1/loadmemory_util",
 
@@ -18,11 +18,12 @@
         "Operating System :: OS Independent",
     ],
 
     packages=setuptools.find_packages(),
     python_requires='>=3.8',
     package_data={
         'loadmemory': [
+            'db/*',
             'utils/*',
         ]
     }
 )
```


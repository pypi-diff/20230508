# Comparing `tmp/mango-cli-0.3.8.tar.gz` & `tmp/mango-cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.3.8.tar", last modified: Sat May  6 03:47:23 2023, max compression
+gzip compressed data, was "mango-cli-0.3.9.tar", last modified: Mon May  8 13:19:17 2023, max compression
```

## Comparing `mango-cli-0.3.8.tar` & `mango-cli-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 03:47:23.094745 mango-cli-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 03:47:00.000000 mango-cli-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/app/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/handlers/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/mango_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-06 03:47:23.000000 mango-cli-0.3.8/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:47:23.094745 mango-cli-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-06 03:47:00.000000 mango-cli-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:17.133695 mango-cli-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 13:19:17.133695 mango-cli-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 13:18:53.000000 mango-cli-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:17.133695 mango-cli-0.3.9/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:53.000000 mango-cli-0.3.9/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-08 13:18:53.000000 mango-cli-0.3.9/app/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:17.133695 mango-cli-0.3.9/app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:53.000000 mango-cli-0.3.9/app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-08 13:18:53.000000 mango-cli-0.3.9/app/handlers/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:17.133695 mango-cli-0.3.9/app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:53.000000 mango-cli-0.3.9/app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-08 13:18:53.000000 mango-cli-0.3.9/app/services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:17.133695 mango-cli-0.3.9/mango_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 13:19:16.000000 mango-cli-0.3.9/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 13:19:17.000000 mango-cli-0.3.9/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:19:16.000000 mango-cli-0.3.9/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 13:19:16.000000 mango-cli-0.3.9/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 13:19:16.000000 mango-cli-0.3.9/mango_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 13:19:16.000000 mango-cli-0.3.9/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:19:17.133695 mango-cli-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-08 13:18:53.000000 mango-cli-0.3.9/setup.py
```

### Comparing `mango-cli-0.3.8/app/handlers/download_data.py` & `mango-cli-0.3.9/app/handlers/download_data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.3.8/app/services/data.py` & `mango-cli-0.3.9/app/services/data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.3.8/mango_cli.egg-info/requires.txt` & `mango-cli-0.3.9/mango_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mango-cli-0.3.8/setup.py` & `mango-cli-0.3.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from setuptools import setup, find_packages
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
-with open("VERSION", "r", encoding="utf-8") as fh:
-    version = fh.read()
 
 setup(
     name='mango-cli',
-    version=version,
+    version="0.3.9",
     packages=find_packages(),
     author='Mangosoft',
     author_email="wilson.mendoza@mango-soft.com",
     description="Mangosoft CLI",
     py_modules=["app"],
     include_dirs=["app"],
     includes=["VERSION"],
```


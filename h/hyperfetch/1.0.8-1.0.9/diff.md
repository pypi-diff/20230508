# Comparing `tmp/hyperfetch-1.0.8.tar.gz` & `tmp/hyperfetch-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfetch-1.0.8.tar", last modified: Thu Apr 27 13:00:19 2023, max compression
+gzip compressed data, was "hyperfetch-1.0.9.tar", last modified: Thu Apr 27 13:04:28 2023, max compression
```

## Comparing `hyperfetch-1.0.8.tar` & `hyperfetch-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.731766 hyperfetch-1.0.8/
--rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.8/LICENSE
--rw-rw-rw-   0        0        0    10466 2023-04-27 13:00:19.731766 hyperfetch-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.8/README.md
--rw-rw-rw-   0        0        0     1689 2023-04-27 13:00:05.000000 hyperfetch-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 13:00:19.731766 hyperfetch-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.702104 hyperfetch-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.710359 hyperfetch-1.0.8/src/hyperfetch/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/__init__.py
--rw-rw-rw-   0        0        0    10569 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/alg_samplers.py
--rw-rw-rw-   0        0        0      654 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/auth_connection.py
--rw-rw-rw-   0        0        0     2118 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/callbacks.py
--rw-rw-rw-   0        0        0    34085 2023-04-27 12:55:49.000000 hyperfetch-1.0.8/src/hyperfetch/manager.py
--rw-rw-rw-   0        0        0     4994 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/tuning.py
--rw-rw-rw-   0        0        0      825 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/util.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.731260 hyperfetch-1.0.8/src/hyperfetch.egg-info/
--rw-rw-rw-   0        0        0    10466 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      211 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.479568 hyperfetch-1.0.9/
+-rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    10466 2023-04-27 13:04:28.479568 hyperfetch-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1690 2023-04-27 13:04:04.000000 hyperfetch-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:04:28.479568 hyperfetch-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.456411 hyperfetch-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.464232 hyperfetch-1.0.9/src/hyperfetch/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/alg_samplers.py
+-rw-rw-rw-   0        0        0      654 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/auth_connection.py
+-rw-rw-rw-   0        0        0     2118 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/callbacks.py
+-rw-rw-rw-   0        0        0    34085 2023-04-27 12:55:49.000000 hyperfetch-1.0.9/src/hyperfetch/manager.py
+-rw-rw-rw-   0        0        0     4994 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/tuning.py
+-rw-rw-rw-   0        0        0      825 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/util.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.478575 hyperfetch-1.0.9/src/hyperfetch.egg-info/
+-rw-rw-rw-   0        0        0    10466 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      212 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/top_level.txt
```

### Comparing `hyperfetch-1.0.8/LICENSE` & `hyperfetch-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/PKG-INFO` & `hyperfetch-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.8
+Version: 1.0.9
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```

### Comparing `hyperfetch-1.0.8/README.md` & `hyperfetch-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/pyproject.toml` & `hyperfetch-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["hyperfetch"]
 
 [project]
 name = "hyperfetch"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Karoline Sund Wahl", email="karolines.wahl@gmail.com" },
 ]
 description = "HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application."
 readme = "README.md"
 requires-python = ">=3.9, <3.11.0"
 license = {file = "LICENSE"}
@@ -32,15 +32,15 @@
 
 dependencies = [
       'python-benedict==0.30.0',
       'codecarbon==2.1.4',
       'torch== 1.11',
       'gym==0.21.0',
       'pandas==2.0.1',
-      'PyYAM==6.0',
+      'PyYAML==6.0',
       'motor==3.1.2',
       'numpy==1.24.3',
       'optuna==3.1.1',
       'stable-baselines3==1.8.0',
       'rl-zoo3==1.8.0',
       'python-dotenv==1.0.0',
       'starlette==0.26.1'
```

### Comparing `hyperfetch-1.0.8/src/hyperfetch/alg_samplers.py` & `hyperfetch-1.0.9/src/hyperfetch/alg_samplers.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/src/hyperfetch/auth_connection.py` & `hyperfetch-1.0.9/src/hyperfetch/auth_connection.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/src/hyperfetch/callbacks.py` & `hyperfetch-1.0.9/src/hyperfetch/callbacks.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/src/hyperfetch/manager.py` & `hyperfetch-1.0.9/src/hyperfetch/manager.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/src/hyperfetch/tuning.py` & `hyperfetch-1.0.9/src/hyperfetch/tuning.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/src/hyperfetch/util.py` & `hyperfetch-1.0.9/src/hyperfetch/util.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.8/src/hyperfetch.egg-info/PKG-INFO` & `hyperfetch-1.0.9/src/hyperfetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.8
+Version: 1.0.9
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```


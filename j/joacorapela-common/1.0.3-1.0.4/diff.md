# Comparing `tmp/joacorapela_common-1.0.3.tar.gz` & `tmp/joacorapela_common-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rapela/dev/research/programs/repos/python/joacorapela_common/dist/tmpoe4kmaam/joacorapela_common-1.0.3.tar", last modified: Wed Nov  2 01:09:25 2022, max compression
+gzip compressed data, was "joacorapela_common-1.0.4.tar", last modified: Mon May  8 18:20:42 2023, max compression
```

## Comparing `joacorapela_common-1.0.3.tar` & `joacorapela_common-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/
--rw-r--r--   0 rapela    (1000) rapela    (1000)      524 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/PKG-INFO
--rw-r--r--   0 rapela    (1000) rapela    (1000)      116 2022-11-02 00:18:47.000000 joacorapela_common-1.0.3/README.md
--rw-r--r--   0 rapela    (1000) rapela    (1000)       81 2022-11-02 00:26:46.000000 joacorapela_common-1.0.3/pyproject.toml
--rw-r--r--   0 rapela    (1000) rapela    (1000)      595 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/setup.cfg
--rw-r--r--   0 rapela    (1000) rapela    (1000)       37 2022-11-02 00:26:54.000000 joacorapela_common-1.0.3/setup.py
-drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/
-drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common/
--rw-r--r--   0 rapela    (1000) rapela    (1000)        2 2022-11-02 00:57:18.000000 joacorapela_common-1.0.3/src/joacorapela_common/__init__.py
-drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common/utils/
--rw-r--r--   0 rapela    (1000) rapela    (1000)        2 2022-11-02 00:57:31.000000 joacorapela_common-1.0.3/src/joacorapela_common/utils/__init__.py
--rw-r--r--   0 rapela    (1000) rapela    (1000)     1755 2022-10-05 20:08:26.000000 joacorapela_common-1.0.3/src/joacorapela_common/utils/geometry.py
--rw-r--r--   0 rapela    (1000) rapela    (1000)     1430 2022-10-05 20:55:51.000000 joacorapela_common-1.0.3/src/joacorapela_common/utils/probability.py
-drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common.egg-info/
--rw-r--r--   0 rapela    (1000) rapela    (1000)      524 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common.egg-info/PKG-INFO
--rw-r--r--   0 rapela    (1000) rapela    (1000)      433 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common.egg-info/SOURCES.txt
--rw-r--r--   0 rapela    (1000) rapela    (1000)        1 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common.egg-info/dependency_links.txt
--rw-r--r--   0 rapela    (1000) rapela    (1000)       12 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common.egg-info/requires.txt
--rw-r--r--   0 rapela    (1000) rapela    (1000)       19 2022-11-02 01:09:25.000000 joacorapela_common-1.0.3/src/joacorapela_common.egg-info/top_level.txt
+drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2023-05-08 18:20:42.942088 joacorapela_common-1.0.4/
+-rw-r--r--   0 rapela    (1000) rapela    (1000)      524 2023-05-08 18:20:42.946088 joacorapela_common-1.0.4/PKG-INFO
+-rw-r--r--   0 rapela    (1000) rapela    (1000)      116 2022-11-02 00:18:47.000000 joacorapela_common-1.0.4/README.md
+-rw-r--r--   0 rapela    (1000) rapela    (1000)       81 2022-11-02 00:26:46.000000 joacorapela_common-1.0.4/pyproject.toml
+-rw-r--r--   0 rapela    (1000) rapela    (1000)      595 2023-05-08 18:20:42.946088 joacorapela_common-1.0.4/setup.cfg
+-rw-r--r--   0 rapela    (1000) rapela    (1000)       37 2022-11-02 00:26:54.000000 joacorapela_common-1.0.4/setup.py
+drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2023-05-08 18:20:42.902088 joacorapela_common-1.0.4/src/
+drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2023-05-08 18:20:42.906088 joacorapela_common-1.0.4/src/joacorapela_common/
+-rw-r--r--   0 rapela    (1000) rapela    (1000)        2 2022-11-02 00:57:18.000000 joacorapela_common-1.0.4/src/joacorapela_common/__init__.py
+drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2023-05-08 18:20:42.938088 joacorapela_common-1.0.4/src/joacorapela_common/utils/
+-rw-r--r--   0 rapela    (1000) rapela    (1000)        2 2022-11-02 00:57:31.000000 joacorapela_common-1.0.4/src/joacorapela_common/utils/__init__.py
+-rw-r--r--   0 rapela    (1000) rapela    (1000)     1755 2022-10-05 20:08:26.000000 joacorapela_common-1.0.4/src/joacorapela_common/utils/geometry.py
+-rw-r--r--   0 rapela    (1000) rapela    (1000)      104 2022-12-17 23:31:11.000000 joacorapela_common-1.0.4/src/joacorapela_common/utils/numerical_methods.py
+-rw-r--r--   0 rapela    (1000) rapela    (1000)     1430 2022-10-05 20:55:51.000000 joacorapela_common-1.0.4/src/joacorapela_common/utils/probability.py
+drwxr-xr-x   0 rapela    (1000) rapela    (1000)        0 2023-05-08 18:20:42.922088 joacorapela_common-1.0.4/src/joacorapela_common.egg-info/
+-rw-r--r--   0 rapela    (1000) rapela    (1000)      524 2023-05-08 18:20:42.000000 joacorapela_common-1.0.4/src/joacorapela_common.egg-info/PKG-INFO
+-rw-r--r--   0 rapela    (1000) rapela    (1000)      483 2023-05-08 18:20:42.000000 joacorapela_common-1.0.4/src/joacorapela_common.egg-info/SOURCES.txt
+-rw-r--r--   0 rapela    (1000) rapela    (1000)        1 2023-05-08 18:20:42.000000 joacorapela_common-1.0.4/src/joacorapela_common.egg-info/dependency_links.txt
+-rw-r--r--   0 rapela    (1000) rapela    (1000)       12 2023-05-08 18:20:42.000000 joacorapela_common-1.0.4/src/joacorapela_common.egg-info/requires.txt
+-rw-r--r--   0 rapela    (1000) rapela    (1000)       19 2023-05-08 18:20:42.000000 joacorapela_common-1.0.4/src/joacorapela_common.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `joacorapela_common-1.0.3/PKG-INFO` & `joacorapela_common-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joacorapela_common
-Version: 1.0.3
+Version: 1.0.4
 Summary: Repository of common functionality for joacorapela's codebase
 Home-page: https://github.com/joacorapela/joacorapela_common
 Author: Joaquin Rapela
 Author-email: joacorapela@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `joacorapela_common-1.0.3/setup.cfg` & `joacorapela_common-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = joacorapela_common
-version = 1.0.3
+version = 1.0.4
 description = Repository of common functionality for joacorapela's codebase
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/joacorapela/joacorapela_common
 author = Joaquin Rapela
 author_email = joacorapela@gmail.com
 license = MIT
```

### Comparing `joacorapela_common-1.0.3/src/joacorapela_common/utils/geometry.py` & `joacorapela_common-1.0.4/src/joacorapela_common/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `joacorapela_common-1.0.3/src/joacorapela_common/utils/probability.py` & `joacorapela_common-1.0.4/src/joacorapela_common/utils/probability.py`

 * *Files identical despite different names*

### Comparing `joacorapela_common-1.0.3/src/joacorapela_common.egg-info/PKG-INFO` & `joacorapela_common-1.0.4/src/joacorapela_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joacorapela-common
-Version: 1.0.3
+Version: 1.0.4
 Summary: Repository of common functionality for joacorapela's codebase
 Home-page: https://github.com/joacorapela/joacorapela_common
 Author: Joaquin Rapela
 Author-email: joacorapela@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```


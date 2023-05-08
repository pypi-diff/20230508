# Comparing `tmp/userfs-1.0.2.tar.gz` & `tmp/userfs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userfs-1.0.2.tar", last modified: Mon May  8 06:15:58 2023, max compression
+gzip compressed data, was "userfs-1.1.0.tar", last modified: Mon May  8 06:30:34 2023, max compression
```

## Comparing `userfs-1.0.2.tar` & `userfs-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 06:14:40.000000 userfs-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 06:15:58.949362 userfs-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 06:14:40.000000 userfs-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 06:14:40.000000 userfs-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:15:58.949362 userfs-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 06:14:40.000000 userfs-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.945362 userfs-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 06:14:40.000000 userfs-1.0.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 06:14:40.000000 userfs-1.0.2/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.945362 userfs-1.0.2/userfs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.945362 userfs-1.0.2/userfs/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/commands/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/config/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/data/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/data/schemas/ProjectSpecification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/data/schemas/SourceSpecification.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/hooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/project/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.949362 userfs-1.0.2/userfs/update/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 06:14:40.000000 userfs-1.0.2/userfs/update/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:58.945362 userfs-1.0.2/userfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 06:15:58.000000 userfs-1.0.2/userfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-08 06:15:58.000000 userfs-1.0.2/userfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:15:58.000000 userfs-1.0.2/userfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 06:15:58.000000 userfs-1.0.2/userfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 06:15:58.000000 userfs-1.0.2/userfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 06:15:58.000000 userfs-1.0.2/userfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 06:29:23.000000 userfs-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 06:30:34.034633 userfs-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 06:29:23.000000 userfs-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 06:29:23.000000 userfs-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:30:34.034633 userfs-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 06:29:23.000000 userfs-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 06:29:23.000000 userfs-1.1.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 06:29:23.000000 userfs-1.1.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/userfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/userfs/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/config/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/schemas/ProjectSpecification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/schemas/SourceSpecification.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/update/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/userfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/top_level.txt
```

### Comparing `userfs-1.0.2/LICENSE` & `userfs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/PKG-INFO` & `userfs-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.0.2
+Version: 1.1.0
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ae6d8345565af8ac9b349c7b95f5091c
+    hash=a1d4bf97f19efef60eb4f55ef88be7ee
     =====================================
 -->
 
-# userfs ([1.0.2](https://pypi.org/project/userfs/))
+# userfs ([1.1.0](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-1.0.2/README.md` & `userfs-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ae6d8345565af8ac9b349c7b95f5091c
+    hash=a1d4bf97f19efef60eb4f55ef88be7ee
     =====================================
 -->
 
-# userfs ([1.0.2](https://pypi.org/project/userfs/))
+# userfs ([1.1.0](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-1.0.2/pyproject.toml` & `userfs-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "userfs"
-version = "1.0.2"
+version = "1.1.0"
 description = "A system-bootstrapping automation and introspection tool."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `userfs-1.0.2/setup.py` & `userfs-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/tests/test_entry.py` & `userfs-1.1.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/app.py` & `userfs-1.1.0/userfs/app.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/build/__init__.py` & `userfs-1.1.0/userfs/build/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/commands/all.py` & `userfs-1.1.0/userfs/commands/all.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/commands/build.py` & `userfs-1.1.0/userfs/commands/build.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/commands/common.py` & `userfs-1.1.0/userfs/commands/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from argparse import Namespace as _Namespace
 from pathlib import Path as _Path
 from re import search
 from typing import Any, Dict, Iterable, Set, Tuple
 
 # internal
 from userfs.config import Config, ProjectInteraction, load_config
+from userfs.paths import paths_added
 from userfs.project import execute_interactions
 
 
 def add_common(parser: _ArgumentParser, projects: bool = True) -> None:
     """Add common command options."""
 
     parser.add_argument(
@@ -66,15 +67,15 @@
         split = opt.split("=", maxsplit=1)
         opts[split[0]] = split[1]
 
     # Apply filter.
     return (
         set(
             filter(
-                lambda x: search(args.pattern, x),
+                lambda x: search(args.pattern, x) and x in config.projects,
                 # Gather the set of projects.
                 set(x for x in args.projects if "=" not in x)
                 if not args.all
                 else set(config.projects.keys()),
             )
         ),
         opts,
@@ -86,14 +87,15 @@
 ) -> int:
     """Run a project interaction command."""
 
     config = load_config(root=args.config)
 
     projects, options = get_projects(args, config)
 
-    return execute_interactions(
-        interactions,
-        projects,
-        config,
-        options,
-        hooks_only=args.no_interact,
-    )
+    with paths_added(config.hook_paths):
+        return execute_interactions(
+            interactions,
+            projects,
+            config,
+            options,
+            hooks_only=args.no_interact,
+        )
```

### Comparing `userfs-1.0.2/userfs/commands/custom.py` & `userfs-1.1.0/userfs/commands/custom.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/commands/fetch.py` & `userfs-1.1.0/userfs/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/config/__init__.py` & `userfs-1.1.0/userfs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/config/project.py` & `userfs-1.1.0/userfs/config/project.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/config/source.py` & `userfs-1.1.0/userfs/config/source.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/data/schemas/Config.yaml` & `userfs-1.1.0/userfs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/data/schemas/ProjectSpecification.yaml` & `userfs-1.1.0/userfs/data/schemas/ProjectSpecification.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/entry.py` & `userfs-1.1.0/userfs/entry.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/fetch/__init__.py` & `userfs-1.1.0/userfs/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/project/__init__.py` & `userfs-1.1.0/userfs/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 interact,
                 [
                     ProjectInteractionTask(
                         interaction,
                         config.directory,
                         config.projects[x],
                         cli_options,
-                        hooks=get_hooks(hook_names, x, interaction, config),
+                        hooks=get_hooks(hook_names, x, interaction),
                         hooks_only=hooks_only,
                     )
                     for x in projects
                 ],
             )
             pool.close()
             pool.join()
```

### Comparing `userfs-1.0.2/userfs/schemas.py` & `userfs-1.1.0/userfs/schemas.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs/update/__init__.py` & `userfs-1.1.0/userfs/update/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.0.2/userfs.egg-info/PKG-INFO` & `userfs-1.1.0/userfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.0.2
+Version: 1.1.0
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ae6d8345565af8ac9b349c7b95f5091c
+    hash=a1d4bf97f19efef60eb4f55ef88be7ee
     =====================================
 -->
 
-# userfs ([1.0.2](https://pypi.org/project/userfs/))
+# userfs ([1.1.0](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-1.0.2/userfs.egg-info/SOURCES.txt` & `userfs-1.1.0/userfs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 tests/test_entry.py
 tests/test_resources.py
 userfs/__init__.py
 userfs/__main__.py
 userfs/app.py
 userfs/dev_requirements.txt
 userfs/entry.py
+userfs/paths.py
 userfs/py.typed
 userfs/requirements.txt
 userfs/schemas.py
 userfs.egg-info/PKG-INFO
 userfs.egg-info/SOURCES.txt
 userfs.egg-info/dependency_links.txt
 userfs.egg-info/entry_points.txt
```


# Comparing `tmp/data_cliff-0.1.2.tar.gz` & `tmp/data_cliff-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_cliff-0.1.2.tar", last modified: Thu Apr 13 12:07:20 2023, max compression
+gzip compressed data, was "data_cliff-0.1.3.tar", last modified: Mon May  8 17:10:35 2023, max compression
```

## Comparing `data_cliff-0.1.2.tar` & `data_cliff-0.1.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 12:07:13.000000 data_cliff-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-13 12:07:13.000000 data_cliff-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 12:07:13.000000 data_cliff-0.1.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 12:07:13.000000 data_cliff-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-13 12:07:13.000000 data_cliff-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-13 12:07:20.668955 data_cliff-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-13 12:07:13.000000 data_cliff-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/data_cliff/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/arg_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/data_cliff.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/data_cliff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4814 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/data_cliff.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-13 12:07:20.668955 data_cliff-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-13 12:07:18.000000 data_cliff-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_arg_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_data_cliff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/local_data/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/local_data/dir.dvc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.660955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/38/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/38/9af16f6ea3dd642636ebd29745313e.dir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/4c/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/4c/4885c2fcf398194990138a70dfd826
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/61/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/61/2420ac8c564d2bf1cb65de08322a15
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/bd/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/bd/7bc28baf5816c0404f8adbad51e0bc.dir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/dc/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/dc/84b0d741e5beae8070013addcc8c28
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/f9/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/f9/2164d14b41244ade9045a5736a1054.dir
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 17:10:33.000000 data_cliff-0.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-08 17:10:33.000000 data_cliff-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 17:10:33.000000 data_cliff-0.1.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 17:10:33.000000 data_cliff-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-08 17:10:33.000000 data_cliff-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-08 17:10:35.980202 data_cliff-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-08 17:10:33.000000 data_cliff-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.976202 data_cliff-0.1.3/data_cliff/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 17:10:33.000000 data_cliff-0.1.3/data_cliff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-08 17:10:33.000000 data_cliff-0.1.3/data_cliff/arg_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 17:10:33.000000 data_cliff-0.1.3/data_cliff/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-08 17:10:33.000000 data_cliff-0.1.3/data_cliff/data_cliff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-08 17:10:33.000000 data_cliff-0.1.3/data_cliff/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:33.000000 data_cliff-0.1.3/data_cliff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.976202 data_cliff-0.1.3/data_cliff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-08 17:10:35.000000 data_cliff-0.1.3/data_cliff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-08 17:10:35.000000 data_cliff-0.1.3/data_cliff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:10:35.000000 data_cliff-0.1.3/data_cliff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 17:10:35.000000 data_cliff-0.1.3/data_cliff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:10:35.000000 data_cliff-0.1.3/data_cliff.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 17:10:35.000000 data_cliff-0.1.3/data_cliff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4814 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/data_cliff.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-08 17:10:33.000000 data_cliff-0.1.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-08 17:10:35.980202 data_cliff-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-08 17:10:35.000000 data_cliff-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_arg_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_data_cliff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/local_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/local_data/dir.dvc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.976202 data_cliff-0.1.3/tests/test_dvc_data/remote_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/remote_data/38/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/remote_data/38/9af16f6ea3dd642636ebd29745313e.dir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/remote_data/4c/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/remote_data/4c/4885c2fcf398194990138a70dfd826
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/remote_data/61/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/remote_data/61/2420ac8c564d2bf1cb65de08322a15
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/remote_data/bd/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/remote_data/bd/7bc28baf5816c0404f8adbad51e0bc.dir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/remote_data/dc/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/remote_data/dc/84b0d741e5beae8070013addcc8c28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:10:35.980202 data_cliff-0.1.3/tests/test_dvc_data/remote_data/f9/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_dvc_data/remote_data/f9/2164d14b41244ade9045a5736a1054.dir
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 17:10:33.000000 data_cliff-0.1.3/tests/test_getter.py
```

### Comparing `data_cliff-0.1.2/CONTRIBUTING.rst` & `data_cliff-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/LICENSE` & `data_cliff-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/PKG-INFO` & `data_cliff-0.1.3/data_cliff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: data_cliff
-Version: 0.1.2
+Name: data-cliff
+Version: 0.1.3
 Summary: CLI tool to show differences on text data tracked by dvc.
 Home-page: https://github.com/ruizdesotto/data_cliff
 Author: Miguel Ruiz
 Author-email: miguel.ruizdesotto@gmail.com
 License: Apache Software License 2.0
 Keywords: data_cliff
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `data_cliff-0.1.2/README.rst` & `data_cliff-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/data_cliff/arg_parse.py` & `data_cliff-0.1.3/data_cliff/arg_parse.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 class CLIException(Exception):
     pass
 
 
 @dataclass(frozen=True)
 class _Args:
-    a_rev: str
-    b_rev: Optional[str]
+    before_rev: str
+    after_rev: Optional[str]
     data_path: str
 
 
 def parse_args(args: list[str]) -> _Args:
     raw_args = parse_command_line_raw_args(args)
-    a_rev = raw_args.pos_1 if _is_git_rev(raw_args.pos_1) else "HEAD"
-    b_rev = raw_args.pos_2 if _is_git_rev(raw_args.pos_2) else None
+    before_rev = raw_args.pos_1 if _is_git_rev(raw_args.pos_1) else "HEAD"
+    after_rev = raw_args.pos_2 if _is_git_rev(raw_args.pos_2) else None
     data_path = _get_data_path(raw_args)
-    return _Args(a_rev=a_rev, b_rev=b_rev, data_path=data_path)
+    return _Args(before_rev=before_rev, after_rev=after_rev, data_path=data_path)
 
 
 def parse_command_line_raw_args(args: list[str]) -> argparse.Namespace:
     raw_parser = _cli_parse_factory()
     try:
         return raw_parser.parse_args(args)
     except SystemExit:
```

### Comparing `data_cliff-0.1.2/data_cliff.egg-info/PKG-INFO` & `data_cliff-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: data-cliff
-Version: 0.1.2
+Name: data_cliff
+Version: 0.1.3
 Summary: CLI tool to show differences on text data tracked by dvc.
 Home-page: https://github.com/ruizdesotto/data_cliff
 Author: Miguel Ruiz
 Author-email: miguel.ruizdesotto@gmail.com
 License: Apache Software License 2.0
 Keywords: data_cliff
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `data_cliff-0.1.2/data_cliff.egg-info/SOURCES.txt` & `data_cliff-0.1.3/data_cliff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/docs/Makefile` & `data_cliff-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/docs/conf.py` & `data_cliff-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/docs/data_cliff.rst` & `data_cliff-0.1.3/docs/data_cliff.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/docs/installation.rst` & `data_cliff-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/docs/make.bat` & `data_cliff-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/setup.cfg` & `data_cliff-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.2/setup.py` & `data_cliff-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords="data_cliff",
     name="data_cliff",
     packages=find_packages(include=["data_cliff", "data_cliff.*"]),
     package_data={"data_cliff": ["py.typed"]},
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ruizdesotto/data_cliff",
-    version="0.1.2",
+    version="0.1.3",
     zip_safe=False,
 )
```

### Comparing `data_cliff-0.1.2/tests/test_arg_parse.py` & `data_cliff-0.1.3/tests/test_arg_parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 
 import pytest
 
 from data_cliff.arg_parse import CLIException
 
 
 @pytest.mark.parametrize(
-    "args, a_rev, b_rev, data_path",
+    "args, before_rev, after_rev, data_path",
     [
         ([], "HEAD", None, ""),
         (["origin/main"], "origin/main", None, ""),
         (["some/path/"], "HEAD", None, "some/path/"),
         (["origin/main", "some/path"], "origin/main", None, "some/path"),
         (["origin/main", "HEAD", "some/path"], "origin/main", "HEAD", "some/path"),
     ],
 )
-def test_parse_args(args: list[str], a_rev: str, b_rev: str, data_path: str) -> None:
+def test_parse_args(
+    args: list[str], before_rev: str, after_rev: str, data_path: str
+) -> None:
     # Given
     from data_cliff.arg_parse import _Args, parse_args
 
     # When
     parsed_args = parse_args(args)
 
     # Then
     assert isinstance(parsed_args, _Args)
-    assert parsed_args.a_rev == a_rev
-    assert parsed_args.b_rev == b_rev
+    assert parsed_args.before_rev == before_rev
+    assert parsed_args.after_rev == after_rev
     assert parsed_args.data_path == data_path
 
 
 @pytest.mark.parametrize(
     "args, expectation",
     [
         ([], nullcontext()),
```

### Comparing `data_cliff-0.1.2/tests/test_cli.py` & `data_cliff-0.1.3/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import io
 import json
 from pathlib import Path
 from unittest.mock import patch
 
 
-def test_main(dvc_path, capsys) -> None:
+def test_main(dvc_path, captured_print: io.StringIO) -> None:
     # Given
     import sys
 
     from dvc.api import DVCFileSystem
 
     from data_cliff.cli import main
 
@@ -19,27 +20,26 @@
         "cliff a/tests/test_dvc_data/local_data/dir/file.json"
         " b/tests/test_dvc_data/local_data/dir/file.json\n"
         "index 612420a..db800ff 100644\n"
         "--- a/tests/test_dvc_data/local_data/dir/file.json\n"
         "+++ b/tests/test_dvc_data/local_data/dir/file.json\n"
         "@@ -1,3 +1,4 @@\n"
         " {\n"
-        '-    "test": "file"\n'
-        '+    "test": "file",\n'
-        '+    "new_key": "new_value"\n'
+        '\x1b[91m-    "test": "file"\x1b[00m\n'
+        '\x1b[92m+    "test": "file",\x1b[00m\n'
+        '\x1b[92m+    "new_key": "new_value"\x1b[00m\n'
         " }\n"
     )
 
     # When
     with patch.object(sys, "argv", test_args):
         main()
-    stdout, _ = capsys.readouterr()
 
     # Then
-    assert stdout == expected_output
+    assert captured_print.getvalue() == expected_output
 
     # Finally
     DVCFileSystem(rev="HEAD").get(str(file), str(file))
 
 
 def _add_line_to_path(file: Path) -> None:
     with open(file) as fid:
```

### Comparing `data_cliff-0.1.2/tests/test_getter.py` & `data_cliff-0.1.3/tests/test_getter.py`

 * *Files identical despite different names*


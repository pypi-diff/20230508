# Comparing `tmp/audinterface-1.0.1.tar.gz` & `tmp/audinterface-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audinterface-1.0.1.tar", last modified: Wed Mar 29 10:05:57 2023, max compression
+gzip compressed data, was "audinterface-1.0.2.tar", last modified: Mon May  8 12:54:47 2023, max compression
```

## Comparing `audinterface-1.0.1.tar` & `audinterface-1.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.946145 audinterface-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.946145 audinterface-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-29 10:05:44.000000 audinterface-1.0.1/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-29 10:05:44.000000 audinterface-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-29 10:05:44.000000 audinterface-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-29 10:05:44.000000 audinterface-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-29 10:05:44.000000 audinterface-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-03-29 10:05:44.000000 audinterface-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-03-29 10:05:44.000000 audinterface-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-29 10:05:44.000000 audinterface-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-03-29 10:05:57.950146 audinterface-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-29 10:05:44.000000 audinterface-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.946145 audinterface-1.0.1/audinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/audinterface/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/core/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    30239 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/core/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/core/process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/core/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/audinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-29 10:05:44.000000 audinterface-1.0.1/audinterface/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/audinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-03-29 10:05:57.000000 audinterface-1.0.1/audinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-29 10:05:57.000000 audinterface-1.0.1/audinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 10:05:57.000000 audinterface-1.0.1/audinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-29 10:05:57.000000 audinterface-1.0.1/audinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-29 10:05:57.000000 audinterface-1.0.1/audinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.946145 audinterface-1.0.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/api-src/audinterface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/api-src/audinterface.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-03-29 10:05:44.000000 audinterface-1.0.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/misc/
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-03-29 10:05:44.000000 audinterface-1.0.1/misc/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-29 10:05:44.000000 audinterface-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-29 10:05:57.950146 audinterface-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-29 10:05:44.000000 audinterface-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:57.950146 audinterface-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-29 10:05:44.000000 audinterface-1.0.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-03-29 10:05:44.000000 audinterface-1.0.1/tests/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    38382 2023-03-29 10:05:44.000000 audinterface-1.0.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-03-29 10:05:44.000000 audinterface-1.0.1/tests/test_process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-03-29 10:05:44.000000 audinterface-1.0.1/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-03-29 10:05:44.000000 audinterface-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.317754 audinterface-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 12:54:31.000000 audinterface-1.0.2/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-08 12:54:31.000000 audinterface-1.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-08 12:54:31.000000 audinterface-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 12:54:31.000000 audinterface-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 12:54:31.000000 audinterface-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-05-08 12:54:31.000000 audinterface-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-08 12:54:31.000000 audinterface-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 12:54:31.000000 audinterface-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-08 12:54:47.325755 audinterface-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-08 12:54:31.000000 audinterface-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30239 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-08 12:54:47.000000 audinterface-1.0.2/audinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.317754 audinterface-1.0.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/api-src/audinterface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/api-src/audinterface.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-08 12:54:31.000000 audinterface-1.0.2/misc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 12:54:31.000000 audinterface-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-08 12:54:47.325755 audinterface-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 12:54:31.000000 audinterface-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39773 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_utils.py
```

### Comparing `audinterface-1.0.1/.github/workflows/publish.yml` & `audinterface-1.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/.github/workflows/test.yml` & `audinterface-1.0.2/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest, windows-latest, macos-latest ]
-        python-version: [ '3.8', '3.9', '3.10' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11' ]
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Cache emodb
       uses: actions/cache@v3
       with:
```

### Comparing `audinterface-1.0.1/CHANGELOG.rst` & `audinterface-1.0.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.0.2 (2023/05/08)
+--------------------------
+
+* Added: support for Python 3.11
+* Changed: require ``audformat>=1.0.1``
+* Fixed: ``*.process_index()``
+  keeps precision of ``end`` values
+  when a segmented index
+  is returned
+
+
 Version 1.0.1 (2023/03/29)
 --------------------------
 
 * Fixed: do not truncate strings
   in values returned by process methods of
   ``audinterface.Feature``
```

### Comparing `audinterface-1.0.1/CONTRIBUTING.rst` & `audinterface-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/LICENSE` & `audinterface-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/PKG-INFO` & `audinterface-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audinterface
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generic interfaces for signal processing
 Home-page: https://github.com/audeering/audinterface/
 Author: Johannes Wagner, Hagen Wierstorf, Andreas Triantafyllopoulos
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com, atriant@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audinterface/
 Description: ============
@@ -49,14 +49,25 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.2 (2023/05/08)
+        --------------------------
+        
+        * Added: support for Python 3.11
+        * Changed: require ``audformat>=1.0.1``
+        * Fixed: ``*.process_index()``
+          keeps precision of ``end`` values
+          when a segmented index
+          is returned
+        
+        
         Version 1.0.1 (2023/03/29)
         --------------------------
         
         * Fixed: do not truncate strings
           in values returned by process methods of
           ``audinterface.Feature``
         
@@ -421,9 +432,10 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
```

### Comparing `audinterface-1.0.1/README.rst` & `audinterface-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/audinterface/__init__.py` & `audinterface-1.0.2/audinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/audinterface/core/feature.py` & `audinterface-1.0.2/audinterface/core/feature.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/audinterface/core/process.py` & `audinterface-1.0.2/audinterface/core/process.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/audinterface/core/process_with_context.py` & `audinterface-1.0.2/audinterface/core/process_with_context.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/audinterface/core/segment.py` & `audinterface-1.0.2/audinterface/core/segment.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/audinterface/core/utils.py` & `audinterface-1.0.2/audinterface/core/utils.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/audinterface.egg-info/PKG-INFO` & `audinterface-1.0.2/audinterface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audinterface
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generic interfaces for signal processing
 Home-page: https://github.com/audeering/audinterface/
 Author: Johannes Wagner, Hagen Wierstorf, Andreas Triantafyllopoulos
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com, atriant@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audinterface/
 Description: ============
@@ -49,14 +49,25 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.2 (2023/05/08)
+        --------------------------
+        
+        * Added: support for Python 3.11
+        * Changed: require ``audformat>=1.0.1``
+        * Fixed: ``*.process_index()``
+          keeps precision of ``end`` values
+          when a segmented index
+          is returned
+        
+        
         Version 1.0.1 (2023/03/29)
         --------------------------
         
         * Fixed: do not truncate strings
           in values returned by process methods of
           ``audinterface.Feature``
         
@@ -421,9 +432,10 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
```

### Comparing `audinterface-1.0.1/audinterface.egg-info/SOURCES.txt` & `audinterface-1.0.2/audinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/docs/_templates/autosummary/class.rst` & `audinterface-1.0.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/docs/api-src/audinterface.rst` & `audinterface-1.0.2/docs/api-src/audinterface.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/docs/conf.py` & `audinterface-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/docs/index.rst` & `audinterface-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/docs/usage.rst` & `audinterface-1.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/misc/logo.png` & `audinterface-1.0.2/misc/logo.png`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/setup.cfg` & `audinterface-1.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 install_requires = 
-	audformat >=0.15.3,<2.0.0
+	audformat >=1.0.1,<2.0.0
 	audmath >=1.2.1
 	audresample >=1.1.0,<2.0.0
 python_requires = >=3.8
 setup_requires = 
 	setuptools_scm
 
 [tool:pytest]
```

### Comparing `audinterface-1.0.1/tests/test_feature.py` & `audinterface-1.0.2/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/tests/test_process.py` & `audinterface-1.0.2/tests/test_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import audiofile
 import audiofile as af
 import numpy as np
 import pandas as pd
 import pytest
 
+import audeer
 import audinterface
 import audformat
 import audobject
 
 
 def signal_duration(signal, sampling_rate):
     return signal.shape[1] / sampling_rate
@@ -557,15 +558,16 @@
         sampling_rate=None,
         resample=False,
         num_workers=num_workers,
         multiprocessing=multiprocessing,
         verbose=False,
     )
     sampling_rate = 8000
-    signal = np.random.uniform(-1.0, 1.0, (1, 3 * sampling_rate))
+    duration = 3.5225
+    signal = np.random.uniform(-1.0, 1.0, (1, int(duration * sampling_rate)))
 
     # create file
     root = str(tmpdir.mkdir('wav'))
     file = 'file.wav'
     path = os.path.join(root, file)
     af.write(path, signal, sampling_rate)
 
@@ -619,14 +621,21 @@
     )
     if preserve_index:
         pd.testing.assert_index_equal(y.index, index)
         for path, value in y.items():
             signal, sampling_rate = audinterface.utils.read_audio(path)
             np.testing.assert_equal(signal, value)
     else:
+        durations = [audiofile.duration(file) for file in index]
+        expected_index = audformat.segmented_index(
+            files=list(index),
+            starts=[0] * len(index),
+            ends=durations,
+        )
+        pd.testing.assert_index_equal(y.index, expected_index)
         for (path, start, end), value in y.items():
             signal, sampling_rate = audinterface.utils.read_audio(
                 path, start=start, end=end
             )
             np.testing.assert_equal(signal, value)
 
     # filewise index with relative paths
@@ -673,14 +682,42 @@
         preserve_index=preserve_index,
         root=root,
         cache_root=cache_root,
     )
     pd.testing.assert_series_equal(y, y_cached)
 
 
+def test_process_index_filewise_end_times(tmpdir):
+
+    # Ensure the resulting segmented index
+    # returned by audinterface.process_index()
+    # and by audformat.Table.get()
+    # have identical end times
+    # if NaT is forbidden,
+    # see https://github.com/audeering/audinterface/issues/113
+
+    db_root = audeer.mkdir(audeer.path(tmpdir, 'tmp'))
+    sampling_rate = 8000
+    duration = 2.5225
+    signal = np.ones((1, int(duration * sampling_rate)))
+    audiofile.write(audeer.path(db_root, 'f.wav'), signal, sampling_rate)
+    db = audformat.Database('db')
+    index = audformat.filewise_index(['f.wav'])
+    db['table'] = audformat.Table(index)
+    db['table']['column'] = audformat.Column()
+    db['table']['column'].set(['label'])
+    db.save(db_root)
+
+    df = db['table'].get(as_segmented=True, allow_nat=False)
+    expected_index = df.index
+    interface = audinterface.Process(process_func=lambda x, fs: x.max())
+    df = interface.process_index(db['table'].index, root=db_root)
+    pd.testing.assert_index_equal(df.index, expected_index)
+
+
 @pytest.mark.parametrize(
     'process_func, process_func_args, segment, signal, '
     'sampling_rate, file, start, end, keep_nat, expected_signal',
     [
         (
             None,
             {},
```

### Comparing `audinterface-1.0.1/tests/test_process_with_context.py` & `audinterface-1.0.2/tests/test_process_with_context.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/tests/test_segment.py` & `audinterface-1.0.2/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.1/tests/test_utils.py` & `audinterface-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*


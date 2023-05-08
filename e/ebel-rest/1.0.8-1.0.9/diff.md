# Comparing `tmp/ebel_rest-1.0.8.tar.gz` & `tmp/ebel_rest-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ebel_rest-1.0.8.tar", last modified: Fri Apr 24 11:44:56 2020, max compression
+gzip compressed data, was "dist/ebel_rest-1.0.9.tar", last modified: Mon Apr 27 13:57:27 2020, max compression
```

## Comparing `ebel_rest-1.0.8.tar` & `ebel_rest-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      198 2020-04-15 08:27:06.000000 ebel_rest-1.0.8/AUTHORS.rst
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     3536 2020-04-15 07:21:55.000000 ebel_rest-1.0.8/CONTRIBUTING.rst
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       89 2020-04-15 13:57:33.000000 ebel_rest-1.0.8/HISTORY.rst
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1076 2020-04-17 07:31:02.000000 ebel_rest-1.0.8/LICENSE
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      327 2020-04-17 07:25:13.000000 ebel_rest-1.0.8/MANIFEST.in
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     3164 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/PKG-INFO
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1842 2020-04-23 05:52:19.000000 ebel_rest-1.0.8/README.rst
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/docs/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      638 2020-04-15 09:13:42.000000 ebel_rest-1.0.8/docs/Makefile
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/docs/build/
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/docs/build/_static/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      286 2020-04-15 09:02:12.000000 ebel_rest-1.0.8/docs/build/_static/file.png
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       90 2020-04-15 09:02:12.000000 ebel_rest-1.0.8/docs/build/_static/minus.png
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       90 2020-04-15 09:02:12.000000 ebel_rest-1.0.8/docs/build/_static/plus.png
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/docs/source/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1939 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/docs/source/conf.py
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      443 2020-04-15 09:13:42.000000 ebel_rest-1.0.8/docs/source/index.rst
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/notebooks/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)  1850669 2020-04-15 13:42:54.000000 ebel_rest-1.0.8/notebooks/Examples.ipynb
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1475 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/setup.cfg
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       94 2020-04-15 08:46:16.000000 ebel_rest-1.0.8/setup.py
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      192 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest/__init__.py
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     9695 2020-04-22 10:31:25.000000 ebel_rest-1.0.8/src/ebel_rest/core.py
--rw-r--r--   0 bschultz  (1002) bschultz  (1002)      173 2020-04-22 10:31:25.000000 ebel_rest-1.0.8/src/ebel_rest/defaults.py
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     2565 2020-04-23 06:24:21.000000 ebel_rest-1.0.8/src/ebel_rest/query.py
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     4847 2020-04-24 11:34:15.000000 ebel_rest-1.0.8/src/ebel_rest/statistics.py
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest/visualisation/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        0 2020-04-15 07:21:55.000000 ebel_rest-1.0.8/src/ebel_rest/visualisation/__init__.py
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest/visualisation/colours/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        0 2020-04-15 07:21:55.000000 ebel_rest-1.0.8/src/ebel_rest/visualisation/colours/__init__.py
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      554 2020-04-15 07:21:55.000000 ebel_rest-1.0.8/src/ebel_rest/visualisation/colours/graphviz.py
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest.egg-info/
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     3164 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest.egg-info/PKG-INFO
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      917 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest.egg-info/SOURCES.txt
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        1 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest.egg-info/dependency_links.txt
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        1 2020-04-15 14:01:36.000000 ebel_rest-1.0.8/src/ebel_rest.egg-info/not-zip-safe
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       35 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest.egg-info/requires.txt
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       10 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/src/ebel_rest.egg-info/top_level.txt
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/tests/
--rw-r--r--   0 bschultz  (1002) bschultz  (1002)       56 2020-04-22 10:07:51.000000 ebel_rest-1.0.8/tests/__init__.py
--rw-r--r--   0 bschultz  (1002) bschultz  (1002)      231 2020-04-22 10:50:08.000000 ebel_rest-1.0.8/tests/constants.py
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/tests/test_query/
--rw-r--r--   0 bschultz  (1002) bschultz  (1002)       51 2020-04-22 10:45:31.000000 ebel_rest-1.0.8/tests/test_query/__init__.py
--rw-r--r--   0 bschultz  (1002) bschultz  (1002)     1245 2020-04-24 06:15:51.000000 ebel_rest-1.0.8/tests/test_query/test_query.py
-drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-24 11:44:56.000000 ebel_rest-1.0.8/tests/test_statistics/
--rw-r--r--   0 bschultz  (1002) bschultz  (1002)        0 2020-04-22 10:05:18.000000 ebel_rest-1.0.8/tests/test_statistics/__init__.py
--rw-r--r--   0 bschultz  (1002) bschultz  (1002)     3533 2020-04-24 11:38:58.000000 ebel_rest-1.0.8/tests/test_statistics/test_statistics.py
--rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1344 2020-04-24 11:43:35.000000 ebel_rest-1.0.8/tox.ini
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      198 2020-04-15 08:27:06.000000 ebel_rest-1.0.9/AUTHORS.rst
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     3536 2020-04-15 07:21:55.000000 ebel_rest-1.0.9/CONTRIBUTING.rst
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       89 2020-04-15 13:57:33.000000 ebel_rest-1.0.9/HISTORY.rst
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1076 2020-04-17 07:31:02.000000 ebel_rest-1.0.9/LICENSE
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      327 2020-04-17 07:25:13.000000 ebel_rest-1.0.9/MANIFEST.in
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     3164 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/PKG-INFO
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1842 2020-04-23 05:52:19.000000 ebel_rest-1.0.9/README.rst
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/docs/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      638 2020-04-15 09:13:42.000000 ebel_rest-1.0.9/docs/Makefile
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/docs/build/
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/docs/build/_static/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      286 2020-04-15 09:02:12.000000 ebel_rest-1.0.9/docs/build/_static/file.png
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       90 2020-04-15 09:02:12.000000 ebel_rest-1.0.9/docs/build/_static/minus.png
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       90 2020-04-15 09:02:12.000000 ebel_rest-1.0.9/docs/build/_static/plus.png
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/docs/source/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1939 2020-04-27 13:57:26.000000 ebel_rest-1.0.9/docs/source/conf.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      443 2020-04-15 09:13:42.000000 ebel_rest-1.0.9/docs/source/index.rst
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/notebooks/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)  1850669 2020-04-15 13:42:54.000000 ebel_rest-1.0.9/notebooks/Examples.ipynb
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1483 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/setup.cfg
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       94 2020-04-15 08:46:16.000000 ebel_rest-1.0.9/setup.py
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      234 2020-04-27 13:57:26.000000 ebel_rest-1.0.9/src/ebel_rest/__init__.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       28 2020-04-27 13:53:32.000000 ebel_rest-1.0.9/src/ebel_rest/constants.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     9695 2020-04-22 10:31:25.000000 ebel_rest-1.0.9/src/ebel_rest/core.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      215 2020-04-27 13:53:32.000000 ebel_rest-1.0.9/src/ebel_rest/defaults.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     6074 2020-04-27 13:56:13.000000 ebel_rest-1.0.9/src/ebel_rest/export.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1598 2020-04-27 13:56:38.000000 ebel_rest-1.0.9/src/ebel_rest/query.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     4847 2020-04-24 11:34:15.000000 ebel_rest-1.0.9/src/ebel_rest/statistics.py
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest/visualisation/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        0 2020-04-15 07:21:55.000000 ebel_rest-1.0.9/src/ebel_rest/visualisation/__init__.py
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest/visualisation/colours/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        0 2020-04-15 07:21:55.000000 ebel_rest-1.0.9/src/ebel_rest/visualisation/colours/__init__.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)      554 2020-04-15 07:21:55.000000 ebel_rest-1.0.9/src/ebel_rest/visualisation/colours/graphviz.py
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest.egg-info/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     3164 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest.egg-info/PKG-INFO
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1031 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest.egg-info/SOURCES.txt
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        1 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest.egg-info/dependency_links.txt
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        1 2020-04-15 14:01:36.000000 ebel_rest-1.0.9/src/ebel_rest.egg-info/not-zip-safe
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       42 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest.egg-info/requires.txt
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)       10 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/src/ebel_rest.egg-info/top_level.txt
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/tests/
+-rw-r--r--   0 bschultz  (1002) bschultz  (1002)       56 2020-04-22 10:07:51.000000 ebel_rest-1.0.9/tests/__init__.py
+-rw-r--r--   0 bschultz  (1002) bschultz  (1002)      231 2020-04-22 10:50:08.000000 ebel_rest-1.0.9/tests/constants.py
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/tests/test_export/
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:53:32.000000 ebel_rest-1.0.9/tests/test_export/__init__.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     2613 2020-04-27 13:53:32.000000 ebel_rest-1.0.9/tests/test_export/test_export.py
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/tests/test_query/
+-rw-r--r--   0 bschultz  (1002) bschultz  (1002)       51 2020-04-22 10:45:31.000000 ebel_rest-1.0.9/tests/test_query/__init__.py
+-rw-r--r--   0 bschultz  (1002) bschultz  (1002)     1245 2020-04-27 13:40:27.000000 ebel_rest-1.0.9/tests/test_query/test_query.py
+drwxrwxr-x   0 bschultz  (1002) bschultz  (1002)        0 2020-04-27 13:57:27.000000 ebel_rest-1.0.9/tests/test_statistics/
+-rw-r--r--   0 bschultz  (1002) bschultz  (1002)        0 2020-04-22 10:05:18.000000 ebel_rest-1.0.9/tests/test_statistics/__init__.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     3776 2020-04-27 13:53:32.000000 ebel_rest-1.0.9/tests/test_statistics/test_statistics.py
+-rw-rw-r--   0 bschultz  (1002) bschultz  (1002)     1344 2020-04-24 11:43:35.000000 ebel_rest-1.0.9/tox.ini
```

### Comparing `ebel_rest-1.0.8/CONTRIBUTING.rst` & `ebel_rest-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/LICENSE` & `ebel_rest-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/PKG-INFO` & `ebel_rest-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ebel_rest
-Version: 1.0.8
+Version: 1.0.9
 Summary: e(BE:L) API client
 Home-page: https://github.com/e-bel/ebel_rest
 Author: Christian Ebeling, Bruce Schultz
 Author-email: Christian.Ebeling@scai.fraunhofer.de, bruce.schultz@scai.fraunhofer.de
 Maintainer: Bruce Schultz
 Maintainer-email: bruce.schultz@scai.fraunhofer.de
 License: MIT License
```

### Comparing `ebel_rest-1.0.8/README.rst` & `ebel_rest-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/docs/Makefile` & `ebel_rest-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/docs/source/conf.py` & `ebel_rest-1.0.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'ebel_rest'
 copyright = '2020, Christian Ebeling, Bruce Schultz'
 author = 'Christian Ebeling, Bruce Schultz'
 
 # The full version, including alpha/beta/rc tags
-release = '1.0.8'
+release = '1.0.9'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `ebel_rest-1.0.8/notebooks/Examples.ipynb` & `ebel_rest-1.0.9/notebooks/Examples.ipynb`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/setup.cfg` & `ebel_rest-1.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ebel_rest
-version = 1.0.8
+version = 1.0.9
 description = e(BE:L) API client
 long_description = file: README.rst
 url = https://github.com/e-bel/ebel_rest
 author = Christian Ebeling, Bruce Schultz
 author_email = Christian.Ebeling@scai.fraunhofer.de, bruce.schultz@scai.fraunhofer.de
 maintainer = Bruce Schultz
 maintainer_email = bruce.schultz@scai.fraunhofer.de
@@ -25,14 +25,15 @@
 	BEL
 	API
 	OrientDB
 	Knowledge Graph
 
 [options]
 install_requires = 
+	pytest
 	pandas
 	IPython
 	graphviz
 	matplotlib
 zip_safe = false
 python_requires = >=3.6
 include_package_data = True
```

### Comparing `ebel_rest-1.0.8/src/ebel_rest/core.py` & `ebel_rest-1.0.9/src/ebel_rest/core.py`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/src/ebel_rest/statistics.py` & `ebel_rest-1.0.9/src/ebel_rest/statistics.py`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/src/ebel_rest/visualisation/colours/graphviz.py` & `ebel_rest-1.0.9/src/ebel_rest/visualisation/colours/graphviz.py`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/src/ebel_rest.egg-info/PKG-INFO` & `ebel_rest-1.0.9/src/ebel_rest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ebel-rest
-Version: 1.0.8
+Version: 1.0.9
 Summary: e(BE:L) API client
 Home-page: https://github.com/e-bel/ebel_rest
 Author: Christian Ebeling, Bruce Schultz
 Author-email: Christian.Ebeling@scai.fraunhofer.de, bruce.schultz@scai.fraunhofer.de
 Maintainer: Bruce Schultz
 Maintainer-email: bruce.schultz@scai.fraunhofer.de
 License: MIT License
```

### Comparing `ebel_rest-1.0.8/src/ebel_rest.egg-info/SOURCES.txt` & `ebel_rest-1.0.9/src/ebel_rest.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 docs/build/_static/file.png
 docs/build/_static/minus.png
 docs/build/_static/plus.png
 docs/source/conf.py
 docs/source/index.rst
 notebooks/Examples.ipynb
 src/ebel_rest/__init__.py
+src/ebel_rest/constants.py
 src/ebel_rest/core.py
 src/ebel_rest/defaults.py
+src/ebel_rest/export.py
 src/ebel_rest/query.py
 src/ebel_rest/statistics.py
 src/ebel_rest.egg-info/PKG-INFO
 src/ebel_rest.egg-info/SOURCES.txt
 src/ebel_rest.egg-info/dependency_links.txt
 src/ebel_rest.egg-info/not-zip-safe
 src/ebel_rest.egg-info/requires.txt
 src/ebel_rest.egg-info/top_level.txt
 src/ebel_rest/visualisation/__init__.py
 src/ebel_rest/visualisation/colours/__init__.py
 src/ebel_rest/visualisation/colours/graphviz.py
 tests/__init__.py
 tests/constants.py
+tests/test_export/__init__.py
+tests/test_export/test_export.py
 tests/test_query/__init__.py
 tests/test_query/test_query.py
 tests/test_statistics/__init__.py
 tests/test_statistics/test_statistics.py
```

### Comparing `ebel_rest-1.0.8/tests/test_query/test_query.py` & `ebel_rest-1.0.9/tests/test_query/test_query.py`

 * *Files identical despite different names*

### Comparing `ebel_rest-1.0.8/tests/test_statistics/test_statistics.py` & `ebel_rest-1.0.9/tests/test_statistics/test_statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 
     def test_last_author_by_number_of_publications(self):
         stats = statistics.last_author_by_number_of_publications()
         assert stats.data is not None
         assert len(stats.table.columns) == 2
         assert len(stats.table.index) > 0
 
+    def test_node_namespace_order_by_namespace(self):
+        stats = statistics.node_namespace_order_by_namespace()
+        assert stats.data is not None
+        assert len(stats.table.columns) == 3
+        assert len(stats.table.index) > 0
+
     def test_namespace_by_count(self):
         stats = statistics.namespace_by_count()
         assert type(stats.table) == pd.DataFrame
         assert len(stats.table.columns) == 2
         assert 'HGNC' in stats.table['namespace'].values
 
     def test_last_author_by_number_of_statements(self):
@@ -84,16 +90,16 @@
 
         pivot = statistics.edges_by_pmid(pivot=True)
         assert isinstance(pivot, pd.DataFrame)
         assert len(pivot.columns) >= 0
         assert len(pivot.index) > 0
 
     def test_nodes_by_pmid(self):
-        no_pivot = statistics.edges_by_pmid(pivot=False)
+        no_pivot = statistics.nodes_by_pmid(pivot=False)
         assert no_pivot.data is not None
-        assert len(no_pivot.table.columns) == 3
+        assert len(no_pivot.table.columns) == 2
         assert len(no_pivot.table.index) > 0
 
         pivot = statistics.nodes_by_pmid(pivot=True)
         assert isinstance(pivot, pd.DataFrame)
         assert len(pivot.columns) >= 0
         assert len(pivot.index) > 0
```

### Comparing `ebel_rest-1.0.8/tox.ini` & `ebel_rest-1.0.9/tox.ini`

 * *Files identical despite different names*


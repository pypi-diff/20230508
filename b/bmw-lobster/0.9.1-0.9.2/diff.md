# Comparing `tmp/bmw-lobster-0.9.1.tar.gz` & `tmp/bmw-lobster-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-0.9.1.tar", last modified: Wed May  3 14:22:59 2023, max compression
+gzip compressed data, was "bmw-lobster-0.9.2.tar", last modified: Mon May  8 15:06:40 2023, max compression
```

## Comparing `bmw-lobster-0.9.1.tar` & `bmw-lobster-0.9.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:59.068387 bmw-lobster-0.9.1/
--rw-r--r--   0 florian   (1000) florian   (1000)     1504 2023-05-03 14:22:59.064387 bmw-lobster-0.9.1/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      567 2023-05-03 14:09:11.000000 bmw-lobster-0.9.1/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:59.064387 bmw-lobster-0.9.1/bmw_lobster.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1504 2023-05-03 14:22:59.000000 bmw-lobster-0.9.1/bmw_lobster.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-05-03 14:22:59.000000 bmw-lobster-0.9.1/bmw_lobster.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-03 14:22:59.000000 bmw-lobster-0.9.1/bmw_lobster.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      165 2023-05-03 14:22:59.000000 bmw-lobster-0.9.1/bmw_lobster.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-03 14:22:59.000000 bmw-lobster-0.9.1/bmw_lobster.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-03 14:22:59.068387 bmw-lobster-0.9.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2334 2023-05-03 14:17:25.000000 bmw-lobster-0.9.1/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.945498 bmw-lobster-0.9.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1504 2023-05-08 15:06:40.945498 bmw-lobster-0.9.2/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      567 2023-05-08 15:03:18.000000 bmw-lobster-0.9.2/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.945498 bmw-lobster-0.9.2/bmw_lobster.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1504 2023-05-08 15:06:40.000000 bmw-lobster-0.9.2/bmw_lobster.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-05-08 15:06:40.000000 bmw-lobster-0.9.2/bmw_lobster.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:06:40.000000 bmw-lobster-0.9.2/bmw_lobster.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-05-08 15:06:40.000000 bmw-lobster-0.9.2/bmw_lobster.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:06:40.000000 bmw-lobster-0.9.2/bmw_lobster.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-08 15:06:40.945498 bmw-lobster-0.9.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2334 2023-05-08 15:03:18.000000 bmw-lobster-0.9.2/setup.py
```

### Comparing `bmw-lobster-0.9.1/PKG-INFO` & `bmw-lobster-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.1
+Version: 0.9.2
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-0.9.1/README.md` & `bmw-lobster-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-0.9.1/bmw_lobster.egg-info/PKG-INFO` & `bmw-lobster-0.9.2/bmw_lobster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.1
+Version: 0.9.2
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-0.9.1/setup.py` & `bmw-lobster-0.9.2/setup.py`

 * *Files identical despite different names*


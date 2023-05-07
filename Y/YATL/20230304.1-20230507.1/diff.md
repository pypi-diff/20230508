# Comparing `tmp/yatl-20230304.1.tar.gz` & `tmp/YATL-20230507.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatl-20230304.1.tar", last modified: Sat Mar  4 18:10:25 2023, max compression
+gzip compressed data, was "YATL-20230507.1.tar", last modified: Sun May  7 23:52:04 2023, max compression
```

## Comparing `yatl-20230304.1.tar` & `YATL-20230507.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-04 18:10:25.552578 yatl-20230304.1/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1405 2023-03-04 18:10:25.552578 yatl-20230304.1/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1661 2022-09-04 22:54:40.000000 yatl-20230304.1/README.md
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-03-04 18:10:25.552578 yatl-20230304.1/setup.cfg
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1636 2022-09-04 22:54:40.000000 yatl-20230304.1/setup.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-04 18:10:25.552578 yatl-20230304.1/yatl/
--rw-r--r--   0 massimo   (1000) massimo   (1000)       75 2023-03-04 18:09:37.000000 yatl-20230304.1/yatl/__init__.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    17679 2023-03-04 18:09:13.000000 yatl-20230304.1/yatl/helpers.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     7637 2022-09-04 22:54:40.000000 yatl-20230304.1/yatl/sanitizer.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    33797 2023-03-04 18:09:13.000000 yatl-20230304.1/yatl/template.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-04 18:10:25.552578 yatl-20230304.1/yatl.egg-info/
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1405 2023-03-04 18:10:25.000000 yatl-20230304.1/yatl.egg-info/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)      225 2023-03-04 18:10:25.000000 yatl-20230304.1/yatl.egg-info/SOURCES.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-03-04 18:10:25.000000 yatl-20230304.1/yatl.egg-info/dependency_links.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2022-09-04 22:54:40.000000 yatl-20230304.1/yatl.egg-info/not-zip-safe
--rw-r--r--   0 massimo   (1000) massimo   (1000)        5 2023-03-04 18:10:25.000000 yatl-20230304.1/yatl.egg-info/top_level.txt
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-07 23:52:04.777334 YATL-20230507.1/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1555 2022-09-04 22:54:40.000000 YATL-20230507.1/LICENSE.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2287 2023-05-07 23:52:04.777334 YATL-20230507.1/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1661 2022-09-04 22:54:40.000000 YATL-20230507.1/README.md
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-07 23:52:04.745334 YATL-20230507.1/YATL.egg-info/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2287 2023-05-07 23:52:04.000000 YATL-20230507.1/YATL.egg-info/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      261 2023-05-07 23:52:04.000000 YATL-20230507.1/YATL.egg-info/SOURCES.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-07 23:52:04.000000 YATL-20230507.1/YATL.egg-info/dependency_links.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        5 2023-05-07 23:52:04.000000 YATL-20230507.1/YATL.egg-info/top_level.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      602 2023-05-07 23:45:05.000000 YATL-20230507.1/pyproject.toml
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-07 23:52:04.777334 YATL-20230507.1/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-07 23:52:04.749334 YATL-20230507.1/tests/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     9896 2022-09-04 22:54:40.000000 YATL-20230507.1/tests/test_helpers.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     6570 2022-09-04 22:54:40.000000 YATL-20230507.1/tests/test_template.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-07 23:52:04.777334 YATL-20230507.1/yatl/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)       75 2023-05-07 23:40:34.000000 YATL-20230507.1/yatl/__init__.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    17679 2023-03-04 18:09:13.000000 YATL-20230507.1/yatl/helpers.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     7637 2022-09-04 22:54:40.000000 YATL-20230507.1/yatl/sanitizer.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    33797 2023-03-04 18:09:13.000000 YATL-20230507.1/yatl/template.py
```

### Comparing `yatl-20230304.1/README.md` & `YATL-20230507.1/README.md`

 * *Files identical despite different names*

### Comparing `yatl-20230304.1/yatl/helpers.py` & `YATL-20230507.1/yatl/helpers.py`

 * *Files identical despite different names*

### Comparing `yatl-20230304.1/yatl/sanitizer.py` & `YATL-20230507.1/yatl/sanitizer.py`

 * *Files identical despite different names*

### Comparing `yatl-20230304.1/yatl/template.py` & `YATL-20230507.1/yatl/template.py`

 * *Files identical despite different names*


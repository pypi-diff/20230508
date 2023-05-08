# Comparing `tmp/gayadsdb6969-1.0.0.tar.gz` & `tmp/gayadsdb6969-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gayadsdb6969-1.0.0.tar", last modified: Mon May  8 16:17:23 2023, max compression
+gzip compressed data, was "gayadsdb6969-1.3.0.tar", last modified: Mon May  8 16:23:08 2023, max compression
```

## Comparing `gayadsdb6969-1.0.0.tar` & `gayadsdb6969-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 16:17:23.615478 gayadsdb6969-1.0.0/
--rw-rw-rw-   0        0        0      191 2023-05-08 16:17:23.611497 gayadsdb6969-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 16:17:23.527477 gayadsdb6969-1.0.0/gayadsdb/
--rw-rw-rw-   0        0        0     3572 2023-05-08 10:08:14.000000 gayadsdb6969-1.0.0/gayadsdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:17:23.603477 gayadsdb6969-1.0.0/gayadsdb6969.egg-info/
--rw-rw-rw-   0        0        0      191 2023-05-08 16:17:23.000000 gayadsdb6969-1.0.0/gayadsdb6969.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-05-08 16:17:23.000000 gayadsdb6969-1.0.0/gayadsdb6969.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 16:17:23.000000 gayadsdb6969-1.0.0/gayadsdb6969.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 16:17:23.000000 gayadsdb6969-1.0.0/gayadsdb6969.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 16:17:23.000000 gayadsdb6969-1.0.0/gayadsdb6969.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 16:17:23.617479 gayadsdb6969-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      322 2023-05-08 16:17:19.000000 gayadsdb6969-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:23:08.451544 gayadsdb6969-1.3.0/
+-rw-rw-rw-   0        0        0      191 2023-05-08 16:23:08.448541 gayadsdb6969-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 16:23:08.407549 gayadsdb6969-1.3.0/gayadsdb/
+-rw-rw-rw-   0        0        0     3572 2023-05-08 10:08:14.000000 gayadsdb6969-1.3.0/gayadsdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:23:08.442548 gayadsdb6969-1.3.0/gayadsdb6969.egg-info/
+-rw-rw-rw-   0        0        0      191 2023-05-08 16:23:08.000000 gayadsdb6969-1.3.0/gayadsdb6969.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-08 16:23:08.000000 gayadsdb6969-1.3.0/gayadsdb6969.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:23:08.000000 gayadsdb6969-1.3.0/gayadsdb6969.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 16:23:08.000000 gayadsdb6969-1.3.0/gayadsdb6969.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:23:08.451544 gayadsdb6969-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-05-08 16:22:09.000000 gayadsdb6969-1.3.0/setup.py
```

### Comparing `gayadsdb6969-1.0.0/gayadsdb/__init__.py` & `gayadsdb6969-1.3.0/gayadsdb/__init__.py`

 * *Files identical despite different names*


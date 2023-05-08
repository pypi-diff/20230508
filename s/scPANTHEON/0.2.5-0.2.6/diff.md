# Comparing `tmp/scPANTHEON-0.2.5.tar.gz` & `tmp/scPANTHEON-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.2.5.tar", last modified: Fri Apr 21 02:49:38 2023, max compression
+gzip compressed data, was "scPANTHEON-0.2.6.tar", last modified: Mon May  8 07:40:55 2023, max compression
```

## Comparing `scPANTHEON-0.2.5.tar` & `scPANTHEON-0.2.6.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.856409 scPANTHEON-0.2.5/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-04-21 02:49:38.855409 scPANTHEON-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.814609 scPANTHEON-0.2.5/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1676 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.823885 scPANTHEON-0.2.5/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.799620 scPANTHEON-0.2.5/scpantheon/extension/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.824889 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.827899 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/
--rw-rw-rw-   0        0        0     1691 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     2286 2023-02-24 01:11:07.000000 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1776 2023-02-24 01:10:45.000000 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/module.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.829901 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.832005 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/__pycache__/
--rw-rw-rw-   0        0        0     4005 2023-03-16 11:08:13.000000 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4034 2023-03-11 03:04:00.000000 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.833007 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.837027 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     2896 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     3643 2023-02-23 14:39:59.000000 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3181 2023-02-23 14:21:27.000000 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.838033 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.841060 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/
--rw-rw-rw-   0        0        0     4423 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5499 2023-02-23 14:40:38.000000 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5496 2023-02-23 14:24:26.000000 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/module.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.842063 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.845311 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/
--rw-rw-rw-   0        0        0     3786 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     4688 2023-02-23 14:40:47.000000 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4694 2023-02-23 14:26:51.000000 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/module.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.846392 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.849403 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     5877 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5883 2023-02-17 13:16:06.000000 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     7872 2023-02-23 14:33:09.000000 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.851408 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.854409 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/
--rw-rw-rw-   0        0        0     7544 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     9069 2023-02-23 14:40:54.000000 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0    10919 2023-02-23 14:39:22.000000 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/module.py
--rw-rw-rw-   0        0        0     1040 2023-04-20 09:00:00.000000 scPANTHEON-0.2.5/scpantheon/main.py
--rw-rw-rw-   0        0        0     5627 2023-04-21 02:43:50.000000 scPANTHEON-0.2.5/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/run.py
--rw-rw-rw-   0        0        0    59203 2023-04-20 04:56:28.000000 scPANTHEON-0.2.5/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/transform.py
--rw-rw-rw-   0        0        0       42 2023-04-21 02:49:38.856409 scPANTHEON-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-04-21 02:49:34.000000 scPANTHEON-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.930051 scPANTHEON-0.2.6/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-05-08 07:40:55.930051 scPANTHEON-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.878797 scPANTHEON-0.2.6/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1721 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.891432 scPANTHEON-0.2.6/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-05-08 07:38:57.000000 scPANTHEON-0.2.6/scpantheon/bokeh_qt.py
+-rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.2.6/scpantheon/data_qt.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.865349 scPANTHEON-0.2.6/scpantheon/extension/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.893955 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.897305 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/
+-rw-rw-rw-   0        0        0     1691 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2286 2023-02-24 01:11:07.000000 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1776 2023-02-24 01:10:45.000000 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.899307 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.901308 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/__pycache__/
+-rw-rw-rw-   0        0        0     4005 2023-03-16 11:08:13.000000 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4034 2023-03-11 03:04:00.000000 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.903392 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.906055 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     2896 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3643 2023-02-23 14:39:59.000000 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3181 2023-02-23 14:21:27.000000 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.908061 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.911568 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/
+-rw-rw-rw-   0        0        0     4423 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5499 2023-02-23 14:40:38.000000 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5496 2023-02-23 14:24:26.000000 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.913088 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.917184 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/
+-rw-rw-rw-   0        0        0     3786 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4688 2023-02-23 14:40:47.000000 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4694 2023-02-23 14:26:51.000000 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.919282 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.922539 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     5877 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5883 2023-02-17 13:16:06.000000 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7872 2023-02-23 14:33:09.000000 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.924942 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.928035 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/
+-rw-rw-rw-   0        0        0     7544 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9069 2023-02-23 14:40:54.000000 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10919 2023-02-23 14:39:22.000000 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/module.py
+-rw-rw-rw-   0        0        0     1162 2023-05-08 06:41:40.000000 scPANTHEON-0.2.6/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.2.6/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/run.py
+-rw-rw-rw-   0        0        0    59203 2023-04-20 04:56:28.000000 scPANTHEON-0.2.6/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 07:40:55.931554 scPANTHEON-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-05-08 06:46:02.000000 scPANTHEON-0.2.6/setup.py
```

### Comparing `scPANTHEON-0.2.5/scPANTHEON.egg-info/SOURCES.txt` & `scPANTHEON-0.2.6/scPANTHEON.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 scPANTHEON.egg-info/PKG-INFO
 scPANTHEON.egg-info/SOURCES.txt
 scPANTHEON.egg-info/dependency_links.txt
 scPANTHEON.egg-info/entry_points.txt
 scPANTHEON.egg-info/requires.txt
 scPANTHEON.egg-info/top_level.txt
 scpantheon/__init__.py
+scpantheon/bokeh_qt.py
+scpantheon/data_qt.py
 scpantheon/main.py
 scpantheon/qt.py
 scpantheon/run.py
 scpantheon/source.py
 scpantheon/transform.py
 scpantheon/extension/Change_Color/module.py
 scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
```

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Change_Color/module.py` & `scPANTHEON-0.2.6/scpantheon/extension/Change_Color/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/module.py` & `scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/module.py` & `scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/module.py` & `scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/module.py` & `scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/module.py` & `scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/extension/TOMAS/module.py` & `scPANTHEON-0.2.6/scpantheon/extension/TOMAS/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/main.py` & `scPANTHEON-0.2.6/scpantheon/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 
 import warnings
 
 from bokeh.server.server import Server
 import multiprocessing
 import warnings
 
+from scpantheon import bokeh_qt, data_qt
+
 class InstallWarning(Warning):
     def __init__(self, message):
         self.message = message
     def __str__(self):
         return repr(self.message)
         
 try: 
-    from scpantheon import qt, source # import from online
+    from scpantheon import source # import from online
 except:
     warnings.warn('YOU HAVE TO INSTALL PyQt5',InstallWarning)
 
 def run():
     global server
     print('Opening Bokeh application on http://localhost:5006/')
     server = Server({'/': source.main},
                     allow_websocket_origin=["localhost:5006"], port=5006, show=False, num_procs=1) 
     server.start()  
     server.io_loop.start()
     server.show()
 
 def app():
-    if qt.main() == 'app closed':
+    if data_qt.main() == 'app closed':
+        print('choosing finished')
+    if bokeh_qt.main() == 'app closed':
         p1.terminate()
         print('app ended')
     
 
 def main():
     global p1
     p1 = multiprocessing.Process(target=run)
```

### Comparing `scPANTHEON-0.2.5/scpantheon/qt.py` & `scPANTHEON-0.2.6/scpantheon/qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/source.py` & `scPANTHEON-0.2.6/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/scpantheon/transform.py` & `scPANTHEON-0.2.6/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.5/setup.py` & `scPANTHEON-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.2.5',#版本
+    version='0.2.6',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                         'appdirs==1.4.4'], # 依赖包,如果没有,可以不要
```


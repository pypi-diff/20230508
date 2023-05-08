# Comparing `tmp/graph_z_c-0.0.2.tar.gz` & `tmp/graph_z_c-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_z_c-0.0.2.tar", last modified: Mon May  8 02:16:21 2023, max compression
+gzip compressed data, was "graph_z_c-0.0.3.tar", last modified: Mon May  8 02:22:14 2023, max compression
```

## Comparing `graph_z_c-0.0.2.tar` & `graph_z_c-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:16:21.185161 graph_z_c-0.0.2/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-08 02:16:21.184903 graph_z_c-0.0.2/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.2/README.md
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:16:21.183500 graph_z_c-0.0.2/graph_z/
--rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-07 10:10:11.000000 graph_z_c-0.0.2/graph_z/__init__.py
--rw-r--r--   0 zelpha     (501) staff       (20)     4101 2023-05-08 01:58:50.000000 graph_z_c-0.0.2/graph_z/graph_z.py
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:16:21.184655 graph_z_c-0.0.2/graph_z_c.egg-info/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-08 02:16:21.000000 graph_z_c-0.0.2/graph_z_c.egg-info/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-08 02:16:21.000000 graph_z_c-0.0.2/graph_z_c.egg-info/SOURCES.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-08 02:16:21.000000 graph_z_c-0.0.2/graph_z_c.egg-info/dependency_links.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-08 02:16:21.000000 graph_z_c-0.0.2/graph_z_c.egg-info/top_level.txt
--rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-08 02:16:21.185218 graph_z_c-0.0.2/setup.cfg
--rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-08 02:15:47.000000 graph_z_c-0.0.2/setup.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:22:14.602539 graph_z_c-0.0.3/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-08 02:22:14.602171 graph_z_c-0.0.3/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.3/README.md
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:22:14.601396 graph_z_c-0.0.3/graph_z/
+-rw-r--r--   0 zelpha     (501) staff       (20)       46 2023-05-08 02:22:00.000000 graph_z_c-0.0.3/graph_z/__init__.py
+-rw-r--r--   0 zelpha     (501) staff       (20)     4101 2023-05-08 01:58:50.000000 graph_z_c-0.0.3/graph_z/graph_z.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:22:14.601959 graph_z_c-0.0.3/graph_z_c.egg-info/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/SOURCES.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/dependency_links.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/top_level.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-08 02:22:14.602637 graph_z_c-0.0.3/setup.cfg
+-rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-08 02:21:58.000000 graph_z_c-0.0.3/setup.py
```

### Comparing `graph_z_c-0.0.2/graph_z/graph_z.py` & `graph_z_c-0.0.3/graph_z/graph_z.py`

 * *Files identical despite different names*


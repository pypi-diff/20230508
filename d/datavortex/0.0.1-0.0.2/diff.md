# Comparing `tmp/datavortex-0.0.1.tar.gz` & `tmp/datavortex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datavortex-0.0.1.tar", last modified: Mon May  8 14:13:43 2023, max compression
+gzip compressed data, was "datavortex-0.0.2.tar", last modified: Mon May  8 15:15:31 2023, max compression
```

## Comparing `datavortex-0.0.1.tar` & `datavortex-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 14:13:43.009659 datavortex-0.0.1/
--rw-rw-r--   0 oem      (29999) oem      (29999)     1079 2023-05-08 13:41:26.000000 datavortex-0.0.1/LICENCE
--rw-rw-r--   0 oem      (29999) oem      (29999)      445 2023-05-08 14:13:43.009659 datavortex-0.0.1/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)       75 2023-05-08 13:48:09.000000 datavortex-0.0.1/README.md
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 14:13:43.005659 datavortex-0.0.1/datavortex/
--rw-rw-r--   0 oem      (29999) oem      (29999)       20 2023-05-08 13:36:09.000000 datavortex-0.0.1/datavortex/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)    23977 2023-05-08 13:44:47.000000 datavortex-0.0.1/datavortex/dados.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 14:13:43.009659 datavortex-0.0.1/datavortex.egg-info/
--rw-rw-r--   0 oem      (29999) oem      (29999)      445 2023-05-08 14:13:42.000000 datavortex-0.0.1/datavortex.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)      238 2023-05-08 14:13:42.000000 datavortex-0.0.1/datavortex.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-05-08 14:13:42.000000 datavortex-0.0.1/datavortex.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       46 2023-05-08 14:13:42.000000 datavortex-0.0.1/datavortex.egg-info/requires.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       11 2023-05-08 14:13:42.000000 datavortex-0.0.1/datavortex.egg-info/top_level.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-05-08 14:13:43.009659 datavortex-0.0.1/setup.cfg
--rw-rw-r--   0 oem      (29999) oem      (29999)      585 2023-05-08 14:13:18.000000 datavortex-0.0.1/setup.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 15:15:31.962098 datavortex-0.0.2/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1079 2023-05-08 13:41:26.000000 datavortex-0.0.2/LICENCE
+-rw-rw-r--   0 oem      (29999) oem      (29999)      445 2023-05-08 15:15:31.962098 datavortex-0.0.2/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)       75 2023-05-08 13:48:09.000000 datavortex-0.0.2/README.md
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 15:15:31.962098 datavortex-0.0.2/datavortex/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       20 2023-05-08 13:36:09.000000 datavortex-0.0.2/datavortex/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)    23977 2023-05-08 13:44:47.000000 datavortex-0.0.2/datavortex/dados.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 15:15:31.962098 datavortex-0.0.2/datavortex.egg-info/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      445 2023-05-08 15:15:31.000000 datavortex-0.0.2/datavortex.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      238 2023-05-08 15:15:31.000000 datavortex-0.0.2/datavortex.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-05-08 15:15:31.000000 datavortex-0.0.2/datavortex.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       55 2023-05-08 15:15:31.000000 datavortex-0.0.2/datavortex.egg-info/requires.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       11 2023-05-08 15:15:31.000000 datavortex-0.0.2/datavortex.egg-info/top_level.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-05-08 15:15:31.962098 datavortex-0.0.2/setup.cfg
+-rw-rw-r--   0 oem      (29999) oem      (29999)      597 2023-05-08 15:15:23.000000 datavortex-0.0.2/setup.py
```

### Comparing `datavortex-0.0.1/LICENCE` & `datavortex-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `datavortex-0.0.1/datavortex/dados.py` & `datavortex-0.0.2/datavortex/dados.py`

 * *Files identical despite different names*


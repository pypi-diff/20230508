# Comparing `tmp/pipcolouringskitsV1-1.0.0.tar.gz` & `tmp/pipcolouringskitsV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcolouringskitsV1-1.0.0.tar", last modified: Mon May  8 20:59:59 2023, max compression
+gzip compressed data, was "pipcolouringskitsV1-1.1.0.tar", last modified: Mon May  8 21:02:10 2023, max compression
```

## Comparing `pipcolouringskitsV1-1.0.0.tar` & `pipcolouringskitsV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:59:59.814818 pipcolouringskitsV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-08 20:59:59.814818 pipcolouringskitsV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:59:59.814818 pipcolouringskitsV1-1.0.0/pipcolouringskitsV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 20:59:59.000000 pipcolouringskitsV1-1.0.0/pipcolouringskitsV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:59:59.814818 pipcolouringskitsV1-1.0.0/pipcolouringskitsV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-08 20:59:59.000000 pipcolouringskitsV1-1.0.0/pipcolouringskitsV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-08 20:59:59.000000 pipcolouringskitsV1-1.0.0/pipcolouringskitsV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 20:59:59.000000 pipcolouringskitsV1-1.0.0/pipcolouringskitsV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-08 20:59:59.000000 pipcolouringskitsV1-1.0.0/pipcolouringskitsV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 20:59:59.814818 pipcolouringskitsV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-08 20:59:59.000000 pipcolouringskitsV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:02:10.061497 pipcolouringskitsV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-08 21:02:10.061497 pipcolouringskitsV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:02:10.061497 pipcolouringskitsV1-1.1.0/pipcolouringskitsV1/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-08 21:02:09.000000 pipcolouringskitsV1-1.1.0/pipcolouringskitsV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:02:10.061497 pipcolouringskitsV1-1.1.0/pipcolouringskitsV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-08 21:02:09.000000 pipcolouringskitsV1-1.1.0/pipcolouringskitsV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-08 21:02:10.000000 pipcolouringskitsV1-1.1.0/pipcolouringskitsV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 21:02:09.000000 pipcolouringskitsV1-1.1.0/pipcolouringskitsV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-08 21:02:09.000000 pipcolouringskitsV1-1.1.0/pipcolouringskitsV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 21:02:10.061497 pipcolouringskitsV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-08 21:02:09.000000 pipcolouringskitsV1-1.1.0/setup.py
```

### Comparing `pipcolouringskitsV1-1.0.0/setup.py` & `pipcolouringskitsV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcolouringskitsV1",
     version=VERSION,
```


# Comparing `tmp/pipcryptlibary-1.0.0.tar.gz` & `tmp/pipcryptlibary-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptlibary-1.0.0.tar", last modified: Mon May  8 21:12:43 2023, max compression
+gzip compressed data, was "pipcryptlibary-1.1.0.tar", last modified: Mon May  8 21:14:51 2023, max compression
```

## Comparing `pipcryptlibary-1.0.0.tar` & `pipcryptlibary-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:12:43.190970 pipcryptlibary-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 21:12:43.190970 pipcryptlibary-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:12:43.190970 pipcryptlibary-1.0.0/pipcryptlibary/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 21:12:42.000000 pipcryptlibary-1.0.0/pipcryptlibary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:12:43.190970 pipcryptlibary-1.0.0/pipcryptlibary.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 21:12:43.000000 pipcryptlibary-1.0.0/pipcryptlibary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-08 21:12:43.000000 pipcryptlibary-1.0.0/pipcryptlibary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 21:12:43.000000 pipcryptlibary-1.0.0/pipcryptlibary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-08 21:12:43.000000 pipcryptlibary-1.0.0/pipcryptlibary.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 21:12:43.190970 pipcryptlibary-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-08 21:12:42.000000 pipcryptlibary-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:14:51.281637 pipcryptlibary-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 21:14:51.281637 pipcryptlibary-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:14:51.277637 pipcryptlibary-1.1.0/pipcryptlibary/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-08 21:14:51.000000 pipcryptlibary-1.1.0/pipcryptlibary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 21:14:51.281637 pipcryptlibary-1.1.0/pipcryptlibary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 21:14:51.000000 pipcryptlibary-1.1.0/pipcryptlibary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-08 21:14:51.000000 pipcryptlibary-1.1.0/pipcryptlibary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 21:14:51.000000 pipcryptlibary-1.1.0/pipcryptlibary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-08 21:14:51.000000 pipcryptlibary-1.1.0/pipcryptlibary.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 21:14:51.281637 pipcryptlibary-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-08 21:14:51.000000 pipcryptlibary-1.1.0/setup.py
```

### Comparing `pipcryptlibary-1.0.0/setup.py` & `pipcryptlibary-1.1.0/setup.py`

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
     name="pipcryptlibary",
     version=VERSION,
```


# Comparing `tmp/Pypicor-1.0.3.tar.gz` & `tmp/Pypicor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pypicor-1.0.3.tar", last modified: Mon May  8 18:39:39 2023, max compression
+gzip compressed data, was "Pypicor-1.0.4.tar", last modified: Mon May  8 18:40:48 2023, max compression
```

## Comparing `Pypicor-1.0.3.tar` & `Pypicor-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 18:39:39.246911 Pypicor-1.0.3/
--rw-rw-rw-   0        0        0      270 2023-05-08 18:39:39.245908 Pypicor-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 18:39:39.233909 Pypicor-1.0.3/Pypicor.egg-info/
--rw-rw-rw-   0        0        0      270 2023-05-08 18:39:39.000000 Pypicor-1.0.3/Pypicor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-08 18:39:39.000000 Pypicor-1.0.3/Pypicor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 18:39:39.000000 Pypicor-1.0.3/Pypicor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-08 18:39:39.000000 Pypicor-1.0.3/Pypicor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 18:39:39.000000 Pypicor-1.0.3/Pypicor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 18:39:39.240910 Pypicor-1.0.3/pypicor/
--rw-rw-rw-   0        0        0        0 2023-05-04 17:36:45.000000 Pypicor-1.0.3/pypicor/__init__.py
--rw-rw-rw-   0        0        0     2206 2023-05-04 14:51:07.000000 Pypicor-1.0.3/pypicor/baq.py
--rw-rw-rw-   0        0        0      110 2023-05-03 16:05:56.000000 Pypicor-1.0.3/pypicor/credentials.py
--rw-rw-rw-   0        0        0       42 2023-05-08 18:39:39.247916 Pypicor-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-05-04 18:37:50.000000 Pypicor-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:40:48.841626 Pypicor-1.0.4/
+-rw-rw-rw-   0        0        0      270 2023-05-08 18:40:48.839625 Pypicor-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 18:40:48.830623 Pypicor-1.0.4/Pypicor.egg-info/
+-rw-rw-rw-   0        0        0      270 2023-05-08 18:40:48.000000 Pypicor-1.0.4/Pypicor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-05-08 18:40:48.000000 Pypicor-1.0.4/Pypicor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 18:40:48.000000 Pypicor-1.0.4/Pypicor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-08 18:40:48.000000 Pypicor-1.0.4/Pypicor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 18:40:48.000000 Pypicor-1.0.4/Pypicor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 18:40:48.835625 Pypicor-1.0.4/pypicor/
+-rw-rw-rw-   0        0        0        0 2023-05-04 17:36:45.000000 Pypicor-1.0.4/pypicor/__init__.py
+-rw-rw-rw-   0        0        0     2206 2023-05-04 14:51:07.000000 Pypicor-1.0.4/pypicor/baq.py
+-rw-rw-rw-   0        0        0      110 2023-05-03 16:05:56.000000 Pypicor-1.0.4/pypicor/credentials.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 18:40:48.841626 Pypicor-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-05-08 18:40:41.000000 Pypicor-1.0.4/setup.py
```

### Comparing `Pypicor-1.0.3/pypicor/baq.py` & `Pypicor-1.0.4/pypicor/baq.py`

 * *Files identical despite different names*


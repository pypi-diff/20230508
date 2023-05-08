# Comparing `tmp/plover_french_extended_stenotype-0.1.0.tar.gz` & `tmp/plover_french_extended_stenotype-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover_french_extended_stenotype-0.1.0.tar", last modified: Mon May  8 12:54:29 2023, max compression
+gzip compressed data, was "plover_french_extended_stenotype-1.0.0.tar", last modified: Sun Mar 12 17:55:13 2023, max compression
```

## Comparing `plover_french_extended_stenotype-0.1.0.tar` & `plover_french_extended_stenotype-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2023-05-08 12:54:29.743723 plover_french_extended_stenotype-0.1.0/
--rw-r--r--   0 stl       (1000) stl       (1000)     1299 2023-05-08 12:54:29.743723 plover_french_extended_stenotype-0.1.0/PKG-INFO
--rw-r--r--   0 stl       (1000) stl       (1000)      224 2023-03-12 18:08:59.000000 plover_french_extended_stenotype-0.1.0/README
-drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2023-05-08 12:54:29.743723 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/
--rw-r--r--   0 stl       (1000) stl       (1000)     1299 2023-05-08 12:54:29.000000 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/PKG-INFO
--rw-r--r--   0 stl       (1000) stl       (1000)      414 2023-05-08 12:54:29.000000 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/SOURCES.txt
--rw-r--r--   0 stl       (1000) stl       (1000)        1 2023-05-08 12:54:29.000000 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/dependency_links.txt
--rw-r--r--   0 stl       (1000) stl       (1000)       85 2023-05-08 12:54:29.000000 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/entry_points.txt
--rw-r--r--   0 stl       (1000) stl       (1000)       19 2023-05-08 12:54:29.000000 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/requires.txt
--rw-r--r--   0 stl       (1000) stl       (1000)       33 2023-05-08 12:54:29.000000 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/top_level.txt
--rw-r--r--   0 stl       (1000) stl       (1000)        1 2022-09-12 12:33:36.000000 plover_french_extended_stenotype-0.1.0/plover_french_extended_stenotype.egg-info/zip-safe
--rw-r--r--   0 stl       (1000) stl       (1000)      788 2023-05-08 12:54:29.743723 plover_french_extended_stenotype-0.1.0/setup.cfg
--rwxr-xr-x   0 stl       (1000) stl       (1000)       63 2023-05-08 11:41:57.000000 plover_french_extended_stenotype-0.1.0/setup.py
+drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2023-03-12 17:55:13.354073 plover_french_extended_stenotype-1.0.0/
+-rw-r--r--   0 stl       (1000) stl       (1000)      437 2023-03-12 17:55:13.354073 plover_french_extended_stenotype-1.0.0/PKG-INFO
+-rw-r--r--   0 stl       (1000) stl       (1000)      166 2022-09-12 12:21:15.000000 plover_french_extended_stenotype-1.0.0/README
+drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2023-03-12 17:55:13.354073 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/
+-rw-r--r--   0 stl       (1000) stl       (1000)      437 2023-03-12 17:55:13.000000 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/PKG-INFO
+-rw-r--r--   0 stl       (1000) stl       (1000)      414 2023-03-12 17:55:13.000000 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/SOURCES.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)        1 2023-03-12 17:55:13.000000 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/dependency_links.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)       84 2023-03-12 17:55:13.000000 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/entry_points.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)       19 2023-03-12 17:55:13.000000 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/requires.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)       33 2023-03-12 17:55:13.000000 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/top_level.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)        1 2022-09-12 12:33:36.000000 plover_french_extended_stenotype-1.0.0/plover_french_extended_stenotype.egg-info/zip-safe
+-rw-r--r--   0 stl       (1000) stl       (1000)      633 2023-03-12 17:55:13.354073 plover_french_extended_stenotype-1.0.0/setup.cfg
+-rwxr-xr-x   0 stl       (1000) stl       (1000)       63 2022-09-12 12:21:15.000000 plover_french_extended_stenotype-1.0.0/setup.py
```


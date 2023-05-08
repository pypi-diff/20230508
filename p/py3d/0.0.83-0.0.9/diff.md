# Comparing `tmp/py3d-0.0.83.tar.gz` & `tmp/py3d-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.83.tar", last modified: Mon May  8 15:20:45 2023, max compression
+gzip compressed data, was "dist/py3d-0.0.9.tar", last modified: Wed Nov  3 12:56:47 2021, max compression
```

## Comparing `py3d-0.0.83.tar` & `py3d-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:20:45.309646 py3d-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-08 15:20:45.309646 py3d-0.0.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-08 15:20:34.000000 py3d-0.0.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:20:45.309646 py3d-0.0.83/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-08 15:20:34.000000 py3d-0.0.83/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26792 2023-05-08 15:20:34.000000 py3d-0.0.83/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    21644 2023-05-08 15:20:34.000000 py3d-0.0.83/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:20:45.309646 py3d-0.0.83/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-08 15:20:45.000000 py3d-0.0.83/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-08 15:20:45.000000 py3d-0.0.83/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 15:20:45.000000 py3d-0.0.83/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-08 15:20:45.000000 py3d-0.0.83/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-08 15:20:45.000000 py3d-0.0.83/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 15:20:45.309646 py3d-0.0.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-08 15:20:34.000000 py3d-0.0.83/setup.py
+drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-03 12:56:47.682647 py3d-0.0.9/
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    28086 2021-11-03 12:56:47.679647 py3d-0.0.9/PKG-INFO
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    18365 2021-06-06 10:33:39.000000 py3d-0.0.9/README.md
+drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-03 12:56:46.439569 py3d-0.0.9/py3d.egg-info/
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    28086 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/PKG-INFO
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      220 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        1 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       14 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/requires.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       12 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/top_level.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    21734 2021-11-01 16:28:28.000000 py3d-0.0.9/py3d.py
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)     5123 2021-10-23 06:22:53.000000 py3d-0.0.9/server.py
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       38 2021-11-03 12:56:47.684649 py3d-0.0.9/setup.cfg
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      719 2021-11-03 12:56:00.000000 py3d-0.0.9/setup.py
+drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-03 12:56:47.653184 py3d-0.0.9/static/
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)  1800083 2021-10-23 14:06:00.000000 py3d-0.0.9/static/bundle.js
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)     4550 2021-06-18 15:29:48.000000 py3d-0.0.9/static/logo.png
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      527 2021-09-12 10:41:59.000000 py3d-0.0.9/viewer.html
```


# Comparing `tmp/sorcerun-0.1.1.tar.gz` & `tmp/sorcerun-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.1.1.tar", last modified: Mon Apr 24 02:52:37 2023, max compression
+gzip compressed data, was "sorcerun-0.2.1.tar", last modified: Mon May  8 19:34:05 2023, max compression
```

## Comparing `sorcerun-0.1.1.tar` & `sorcerun-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:52:37.994015 sorcerun-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 02:52:26.000000 sorcerun-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 02:52:37.994015 sorcerun-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 02:52:26.000000 sorcerun-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:52:37.994015 sorcerun-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-24 02:52:26.000000 sorcerun-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:52:37.994015 sorcerun-0.1.1/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 02:52:37.000000 sorcerun-0.1.1/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-24 02:52:37.000000 sorcerun-0.1.1/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 02:52:37.000000 sorcerun-0.1.1/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 02:52:37.000000 sorcerun-0.1.1/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 02:52:37.000000 sorcerun-0.1.1/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 02:52:37.000000 sorcerun-0.1.1/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:52:37.994015 sorcerun-0.1.1/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:52:26.000000 sorcerun-0.1.1/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 02:52:26.000000 sorcerun-0.1.1/sorcerun_package/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:05.477507 sorcerun-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 19:33:51.000000 sorcerun-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 19:34:05.477507 sorcerun-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 19:33:51.000000 sorcerun-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:34:05.477507 sorcerun-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-08 19:33:51.000000 sorcerun-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:05.477507 sorcerun-0.2.1/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:05.477507 sorcerun-0.2.1/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.1.1/LICENSE` & `sorcerun-0.2.1/LICENSE`

 * *Files identical despite different names*


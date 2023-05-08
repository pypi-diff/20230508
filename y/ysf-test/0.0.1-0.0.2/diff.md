# Comparing `tmp/ysf_test-0.0.1.tar.gz` & `tmp/ysf_test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ysf_test-0.0.1.tar", last modified: Mon May  8 08:06:39 2023, max compression
+gzip compressed data, was "ysf_test-0.0.2.tar", last modified: Mon May  8 08:16:56 2023, max compression
```

## Comparing `ysf_test-0.0.1.tar` & `ysf_test-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:06:39.882684 ysf_test-0.0.1/
--rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:06:39.882562 ysf_test-0.0.1/PKG-INFO
--rw-r--r--   0 fan        (501) staff       (20)       38 2023-05-08 08:06:39.882719 ysf_test-0.0.1/setup.cfg
--rw-r--r--   0 fan        (501) staff       (20)      490 2023-05-08 08:06:05.000000 ysf_test-0.0.1/setup.py
-drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:06:39.881838 ysf_test-0.0.1/test/
--rw-r--r--   0 fan        (501) staff       (20)      161 2023-05-08 07:43:22.000000 ysf_test-0.0.1/test/__init__.py
-drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:06:39.882411 ysf_test-0.0.1/ysf_test.egg-info/
--rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:06:39.000000 ysf_test-0.0.1/ysf_test.egg-info/PKG-INFO
--rw-r--r--   0 fan        (501) staff       (20)      153 2023-05-08 08:06:39.000000 ysf_test-0.0.1/ysf_test.egg-info/SOURCES.txt
--rw-r--r--   0 fan        (501) staff       (20)        1 2023-05-08 08:06:39.000000 ysf_test-0.0.1/ysf_test.egg-info/dependency_links.txt
--rw-r--r--   0 fan        (501) staff       (20)        5 2023-05-08 08:06:39.000000 ysf_test-0.0.1/ysf_test.egg-info/top_level.txt
+drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:16:56.803374 ysf_test-0.0.2/
+-rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:16:56.803181 ysf_test-0.0.2/PKG-INFO
+-rw-r--r--   0 fan        (501) staff       (20)       38 2023-05-08 08:16:56.803415 ysf_test-0.0.2/setup.cfg
+-rw-r--r--   0 fan        (501) staff       (20)      490 2023-05-08 08:15:16.000000 ysf_test-0.0.2/setup.py
+drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:16:56.802290 ysf_test-0.0.2/test/
+-rw-r--r--   0 fan        (501) staff       (20)      161 2023-05-08 07:43:22.000000 ysf_test-0.0.2/test/__init__.py
+-rw-r--r--   0 fan        (501) staff       (20)      241 2023-05-08 08:14:24.000000 ysf_test-0.0.2/test/cat.py
+drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:16:56.803011 ysf_test-0.0.2/ysf_test.egg-info/
+-rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:16:56.000000 ysf_test-0.0.2/ysf_test.egg-info/PKG-INFO
+-rw-r--r--   0 fan        (501) staff       (20)      165 2023-05-08 08:16:56.000000 ysf_test-0.0.2/ysf_test.egg-info/SOURCES.txt
+-rw-r--r--   0 fan        (501) staff       (20)        1 2023-05-08 08:16:56.000000 ysf_test-0.0.2/ysf_test.egg-info/dependency_links.txt
+-rw-r--r--   0 fan        (501) staff       (20)        5 2023-05-08 08:16:56.000000 ysf_test-0.0.2/ysf_test.egg-info/top_level.txt
```


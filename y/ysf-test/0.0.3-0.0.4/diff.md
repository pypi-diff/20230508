# Comparing `tmp/ysf-test-0.0.3.tar.gz` & `tmp/ysf_test-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ysf-test-0.0.3.tar", last modified: Mon May  8 08:29:35 2023, max compression
+gzip compressed data, was "ysf_test-0.0.4.tar", last modified: Mon May  8 08:45:35 2023, max compression
```

## Comparing `ysf-test-0.0.3.tar` & `ysf_test-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:29:35.354596 ysf-test-0.0.3/
--rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:29:35.354467 ysf-test-0.0.3/PKG-INFO
--rw-r--r--   0 fan        (501) staff       (20)       38 2023-05-08 08:29:35.354632 ysf-test-0.0.3/setup.cfg
--rw-r--r--   0 fan        (501) staff       (20)      490 2023-05-08 08:29:06.000000 ysf-test-0.0.3/setup.py
-drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:29:35.353750 ysf-test-0.0.3/ysf-test/
--rw-r--r--   0 fan        (501) staff       (20)      161 2023-05-08 07:43:22.000000 ysf-test-0.0.3/ysf-test/__init__.py
--rw-r--r--   0 fan        (501) staff       (20)      241 2023-05-08 08:14:24.000000 ysf-test-0.0.3/ysf-test/cat.py
-drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:29:35.354317 ysf-test-0.0.3/ysf_test.egg-info/
--rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:29:35.000000 ysf-test-0.0.3/ysf_test.egg-info/PKG-INFO
--rw-r--r--   0 fan        (501) staff       (20)      173 2023-05-08 08:29:35.000000 ysf-test-0.0.3/ysf_test.egg-info/SOURCES.txt
--rw-r--r--   0 fan        (501) staff       (20)        1 2023-05-08 08:29:35.000000 ysf-test-0.0.3/ysf_test.egg-info/dependency_links.txt
--rw-r--r--   0 fan        (501) staff       (20)        9 2023-05-08 08:29:35.000000 ysf-test-0.0.3/ysf_test.egg-info/top_level.txt
+drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:45:35.278942 ysf_test-0.0.4/
+-rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:45:35.278812 ysf_test-0.0.4/PKG-INFO
+-rw-r--r--   0 fan        (501) staff       (20)       38 2023-05-08 08:45:35.278977 ysf_test-0.0.4/setup.cfg
+-rw-r--r--   0 fan        (501) staff       (20)      490 2023-05-08 08:45:33.000000 ysf_test-0.0.4/setup.py
+drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:45:35.278013 ysf_test-0.0.4/ysf_test/
+-rw-r--r--   0 fan        (501) staff       (20)      183 2023-05-08 08:35:14.000000 ysf_test-0.0.4/ysf_test/__init__.py
+-rw-r--r--   0 fan        (501) staff       (20)      241 2023-05-08 08:14:24.000000 ysf_test-0.0.4/ysf_test/cat.py
+drwxr-xr-x   0 fan        (501) staff       (20)        0 2023-05-08 08:45:35.278658 ysf_test-0.0.4/ysf_test.egg-info/
+-rw-r--r--   0 fan        (501) staff       (20)      247 2023-05-08 08:45:35.000000 ysf_test-0.0.4/ysf_test.egg-info/PKG-INFO
+-rw-r--r--   0 fan        (501) staff       (20)      173 2023-05-08 08:45:35.000000 ysf_test-0.0.4/ysf_test.egg-info/SOURCES.txt
+-rw-r--r--   0 fan        (501) staff       (20)        1 2023-05-08 08:45:35.000000 ysf_test-0.0.4/ysf_test.egg-info/dependency_links.txt
+-rw-r--r--   0 fan        (501) staff       (20)        9 2023-05-08 08:45:35.000000 ysf_test-0.0.4/ysf_test.egg-info/top_level.txt
```


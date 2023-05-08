# Comparing `tmp/PyQuantimClient-1.0.8.tar.gz` & `tmp/PyQuantimClient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQuantimClient-1.0.8.tar", last modified: Mon Dec 19 18:19:13 2022, max compression
+gzip compressed data, was "PyQuantimClient-1.0.9.tar", last modified: Mon Dec 19 20:05:36 2022, max compression
```

## Comparing `PyQuantimClient-1.0.8.tar` & `PyQuantimClient-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:19:13.188602 PyQuantimClient-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 18:19:13.188602 PyQuantimClient-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:19:13.188602 PyQuantimClient-1.0.8/PyQuantimClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 18:19:13.000000 PyQuantimClient-1.0.8/PyQuantimClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-19 18:19:13.000000 PyQuantimClient-1.0.8/PyQuantimClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 18:19:13.000000 PyQuantimClient-1.0.8/PyQuantimClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-19 18:19:13.000000 PyQuantimClient-1.0.8/PyQuantimClient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 18:19:13.188602 PyQuantimClient-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:19:13.188602 PyQuantimClient-1.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/src/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/src/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/src/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/src/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    16715 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/src/preprocess_co.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2022-12-19 18:19:05.000000 PyQuantimClient-1.0.8/src/risk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/preprocess_co.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/risk.py
```

### Comparing `PyQuantimClient-1.0.8/src/api.py` & `PyQuantimClient-1.0.9/src/api.py`

 * *Files identical despite different names*

### Comparing `PyQuantimClient-1.0.8/src/data.py` & `PyQuantimClient-1.0.9/src/data.py`

 * *Files identical despite different names*

### Comparing `PyQuantimClient-1.0.8/src/energy.py` & `PyQuantimClient-1.0.9/src/energy.py`

 * *Files identical despite different names*

### Comparing `PyQuantimClient-1.0.8/src/portfolios.py` & `PyQuantimClient-1.0.9/src/portfolios.py`

 * *Files identical despite different names*

### Comparing `PyQuantimClient-1.0.8/src/preprocess_co.py` & `PyQuantimClient-1.0.9/src/preprocess_co.py`

 * *Files identical despite different names*

### Comparing `PyQuantimClient-1.0.8/src/risk.py` & `PyQuantimClient-1.0.9/src/risk.py`

 * *Files identical despite different names*


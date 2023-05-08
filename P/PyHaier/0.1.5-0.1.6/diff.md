# Comparing `tmp/PyHaier-0.1.5.tar.gz` & `tmp/PyHaier-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHaier-0.1.5.tar", last modified: Mon May  8 15:33:57 2023, max compression
+gzip compressed data, was "PyHaier-0.1.6.tar", last modified: Mon May  8 15:43:05 2023, max compression
```

## Comparing `PyHaier-0.1.5.tar` & `PyHaier-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:33:57.967453 PyHaier-0.1.5/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      204 2023-05-08 15:33:57.966537 PyHaier-0.1.5/PKG-INFO
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:33:57.966537 PyHaier-0.1.5/PyHaier/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      164 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetCHTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)       24 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetCompFreq.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      174 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetDHWCurTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      155 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetDHWTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      271 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetMode.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      776 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetState.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      570 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetTwiTwo.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      458 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetCHTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      463 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetDHWTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      248 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetMode.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     1282 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetState.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      399 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/__init__.py
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:33:57.966537 PyHaier-0.1.5/PyHaier.egg-info/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      204 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/PKG-INFO
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      395 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/SOURCES.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)        1 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/dependency_links.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)        8 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/top_level.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5238 2023-05-08 15:33:40.000000 PyHaier-0.1.5/README.md
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)       38 2023-05-08 15:33:57.967453 PyHaier-0.1.5/setup.cfg
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      323 2023-05-08 15:33:40.000000 PyHaier-0.1.5/setup.py
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:43:05.171454 PyHaier-0.1.6/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5845 2023-05-08 15:43:05.171454 PyHaier-0.1.6/PKG-INFO
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:43:05.171454 PyHaier-0.1.6/PyHaier/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      164 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/GetCHTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)       24 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/GetCompFreq.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      174 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/GetDHWCurTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      155 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/GetDHWTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      271 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/GetMode.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      776 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/GetState.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      570 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/GetTwiTwo.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      458 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/SetCHTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      463 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/SetDHWTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      248 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/SetMode.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     1282 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/SetState.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      399 2023-05-08 15:33:40.000000 PyHaier-0.1.6/PyHaier/__init__.py
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:43:05.171454 PyHaier-0.1.6/PyHaier.egg-info/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5845 2023-05-08 15:43:05.000000 PyHaier-0.1.6/PyHaier.egg-info/PKG-INFO
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      401 2023-05-08 15:43:05.000000 PyHaier-0.1.6/PyHaier.egg-info/SOURCES.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)        1 2023-05-08 15:43:05.000000 PyHaier-0.1.6/PyHaier.egg-info/dependency_links.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)        8 2023-05-08 15:43:05.000000 PyHaier-0.1.6/PyHaier.egg-info/top_level.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5238 2023-05-08 15:33:40.000000 PyHaier-0.1.6/README.md
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      609 2023-05-08 15:42:30.000000 PyHaier-0.1.6/pyproject.toml
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)       38 2023-05-08 15:43:05.171454 PyHaier-0.1.6/setup.cfg
```

### Comparing `PyHaier-0.1.5/PyHaier/GetState.py` & `PyHaier-0.1.6/PyHaier/GetState.py`

 * *Files identical despite different names*

### Comparing `PyHaier-0.1.5/PyHaier/GetTwiTwo.py` & `PyHaier-0.1.6/PyHaier/GetTwiTwo.py`

 * *Files identical despite different names*

### Comparing `PyHaier-0.1.5/PyHaier/SetState.py` & `PyHaier-0.1.6/PyHaier/SetState.py`

 * *Files identical despite different names*

### Comparing `PyHaier-0.1.5/README.md` & `PyHaier-0.1.6/README.md`

 * *Files identical despite different names*


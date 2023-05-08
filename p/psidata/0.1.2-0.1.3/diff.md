# Comparing `tmp/psidata-0.1.2.tar.gz` & `tmp/psidata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psidata-0.1.2.tar", last modified: Thu May  4 14:53:55 2023, max compression
+gzip compressed data, was "psidata-0.1.3.tar", last modified: Mon May  8 16:11:15 2023, max compression
```

## Comparing `psidata-0.1.2.tar` & `psidata-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.402316 psidata-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.398316 psidata-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.398316 psidata-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 14:53:44.000000 psidata-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-04 14:53:44.000000 psidata-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-04 14:53:44.000000 psidata-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-04 14:53:55.402316 psidata-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 14:53:44.000000 psidata-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.402316 psidata-0.1.2/psidata/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/legacy_bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/zarr_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.402316 psidata-0.1.2/psidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-04 14:53:44.000000 psidata-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:53:55.402316 psidata-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.317857 psidata-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.309857 psidata-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.313857 psidata-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-08 16:11:02.000000 psidata-0.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-08 16:11:02.000000 psidata-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 16:11:02.000000 psidata-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-08 16:11:15.317857 psidata-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 16:11:02.000000 psidata-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.313857 psidata-0.1.3/psidata/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/legacy_bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-08 16:11:02.000000 psidata-0.1.3/psidata/zarr_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:15.317857 psidata-0.1.3/psidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 16:11:15.000000 psidata-0.1.3/psidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-08 16:11:02.000000 psidata-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:11:15.317857 psidata-0.1.3/setup.cfg
```

### Comparing `psidata-0.1.2/.github/workflows/publish-to-pypi.yml` & `psidata-0.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/.gitignore` & `psidata-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/LICENSE.txt` & `psidata-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/PKG-INFO` & `psidata-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
```

### Comparing `psidata-0.1.2/psidata/bcolz_tools.py` & `psidata-0.1.3/psidata/bcolz_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os.path
 
 import bcolz
 import numpy as np
 import pandas as pd
 from scipy import signal
 
-from . import Signal
+from .signal import Signal
 
 
 # Max size of LRU cache
 MAXSIZE = 1024
 
 
 def repair_carray_size(path):
```

### Comparing `psidata-0.1.2/psidata/calibration.py` & `psidata-0.1.3/psidata/calibration.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/psidata/legacy_bcolz_tools.py` & `psidata-0.1.3/psidata/legacy_bcolz_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/psidata/recording.py` & `psidata-0.1.3/psidata/recording.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/psidata/signal.py` & `psidata-0.1.3/psidata/signal.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/psidata/zarr_tools.py` & `psidata-0.1.3/psidata/zarr_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.2/psidata.egg-info/PKG-INFO` & `psidata-0.1.3/psidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
```

### Comparing `psidata-0.1.2/pyproject.toml` & `psidata-0.1.3/pyproject.toml`

 * *Files identical despite different names*


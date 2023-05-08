# Comparing `tmp/flytekitplugins-vaex-1.6.0b2.tar.gz` & `tmp/flytekitplugins-vaex-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-vaex-1.6.0b2.tar", last modified: Fri May  5 17:49:50 2023, max compression
+gzip compressed data, was "flytekitplugins-vaex-1.6.0b3.tar", last modified: Mon May  8 20:18:47 2023, max compression
```

## Comparing `flytekitplugins-vaex-1.6.0b2.tar` & `flytekitplugins-vaex-1.6.0b3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.886227 flytekitplugins-vaex-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-05 17:49:50.886227 flytekitplugins-vaex-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-05 17:49:25.000000 flytekitplugins-vaex-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.882228 flytekitplugins-vaex-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.882228 flytekitplugins-vaex-1.6.0b2/flytekitplugins/vaex/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-05 17:49:25.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins/vaex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-05 17:49:25.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins/vaex/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.882228 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-05 17:49:50.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 17:49:50.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:50.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 17:49:50.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:50.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 17:49:50.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:50.000000 flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:50.886227 flytekitplugins-vaex-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-05 17:49:40.000000 flytekitplugins-vaex-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.932851 flytekitplugins-vaex-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-08 20:18:47.932851 flytekitplugins-vaex-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-08 20:18:20.000000 flytekitplugins-vaex-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.928851 flytekitplugins-vaex-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.932851 flytekitplugins-vaex-1.6.0b3/flytekitplugins/vaex/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 20:18:20.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins/vaex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-08 20:18:20.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins/vaex/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.932851 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-08 20:18:47.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 20:18:47.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:47.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 20:18:47.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:47.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 20:18:47.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:47.000000 flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:47.932851 flytekitplugins-vaex-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-08 20:18:37.000000 flytekitplugins-vaex-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-vaex-1.6.0b2/PKG-INFO` & `flytekitplugins-vaex-1.6.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-vaex
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Vaex plugin for flytekit
 Author: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-vaex-1.6.0b2/flytekitplugins/vaex/sd_transformers.py` & `flytekitplugins-vaex-1.6.0b3/flytekitplugins/vaex/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-vaex-1.6.0b2/flytekitplugins_vaex.egg-info/PKG-INFO` & `flytekitplugins-vaex-1.6.0b3/flytekitplugins_vaex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-vaex
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Vaex plugin for flytekit
 Author: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-vaex-1.6.0b2/setup.py` & `flytekitplugins-vaex-1.6.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "vaex"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "vaex-core>=4.13.0,<4.14"]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="admin@flyte.org",
     description="Vaex plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```


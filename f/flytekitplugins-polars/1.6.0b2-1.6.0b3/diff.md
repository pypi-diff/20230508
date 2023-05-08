# Comparing `tmp/flytekitplugins-polars-1.6.0b2.tar.gz` & `tmp/flytekitplugins-polars-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-polars-1.6.0b2.tar", last modified: Fri May  5 17:49:49 2023, max compression
+gzip compressed data, was "flytekitplugins-polars-1.6.0b3.tar", last modified: Mon May  8 20:18:46 2023, max compression
```

## Comparing `flytekitplugins-polars-1.6.0b2.tar` & `flytekitplugins-polars-1.6.0b3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-05 17:49:25.000000 flytekitplugins-polars-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 17:49:25.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-05 17:49:25.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 17:49:40.000000 flytekitplugins-polars-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.164857 flytekitplugins-polars-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-08 20:18:46.164857 flytekitplugins-polars-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-08 20:18:20.000000 flytekitplugins-polars-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.160857 flytekitplugins-polars-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.160857 flytekitplugins-polars-1.6.0b3/flytekitplugins/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-08 20:18:20.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-08 20:18:20.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins/polars/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.164857 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-08 20:18:46.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 20:18:46.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:46.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 20:18:46.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:46.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 20:18:46.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:46.000000 flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:46.164857 flytekitplugins-polars-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 20:18:37.000000 flytekitplugins-polars-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-polars-1.6.0b2/PKG-INFO` & `flytekitplugins-polars-1.6.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/sd_transformers.py` & `flytekitplugins-polars-1.6.0b3/flytekitplugins/polars/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/PKG-INFO` & `flytekitplugins-polars-1.6.0b3/flytekitplugins_polars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.6.0b2/setup.py` & `flytekitplugins-polars-1.6.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "polars>=0.8.27",
 ]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Robin Kahlow",
     description="Polars plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```


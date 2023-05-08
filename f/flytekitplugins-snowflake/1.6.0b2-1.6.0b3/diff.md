# Comparing `tmp/flytekitplugins-snowflake-1.6.0b2.tar.gz` & `tmp/flytekitplugins-snowflake-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-snowflake-1.6.0b2.tar", last modified: Fri May  5 17:49:49 2023, max compression
+gzip compressed data, was "flytekitplugins-snowflake-1.6.0b3.tar", last modified: Mon May  8 20:18:46 2023, max compression
```

## Comparing `flytekitplugins-snowflake-1.6.0b2.tar` & `flytekitplugins-snowflake-1.6.0b3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.806213 flytekitplugins-snowflake-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 17:49:49.806213 flytekitplugins-snowflake-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-05 17:49:25.000000 flytekitplugins-snowflake-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.806213 flytekitplugins-snowflake-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.806213 flytekitplugins-snowflake-1.6.0b2/flytekitplugins/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-05 17:49:25.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-05 17:49:25.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins/snowflake/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.806213 flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 17:49:49.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 17:49:49.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:49.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 17:49:49.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:49.806213 flytekitplugins-snowflake-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-05 17:49:40.000000 flytekitplugins-snowflake-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.872855 flytekitplugins-snowflake-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-08 20:18:46.872855 flytekitplugins-snowflake-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-08 20:18:20.000000 flytekitplugins-snowflake-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.868855 flytekitplugins-snowflake-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.868855 flytekitplugins-snowflake-1.6.0b3/flytekitplugins/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-08 20:18:20.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-08 20:18:20.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins/snowflake/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.868855 flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-08 20:18:46.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 20:18:46.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:46.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:46.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 20:18:46.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:46.000000 flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:46.872855 flytekitplugins-snowflake-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 20:18:37.000000 flytekitplugins-snowflake-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-snowflake-1.6.0b2/PKG-INFO` & `flytekitplugins-snowflake-1.6.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.6.0b2/README.md` & `flytekitplugins-snowflake-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.6.0b2/flytekitplugins/snowflake/task.py` & `flytekitplugins-snowflake-1.6.0b3/flytekitplugins/snowflake/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.6.0b2/flytekitplugins_snowflake.egg-info/PKG-INFO` & `flytekitplugins-snowflake-1.6.0b3/flytekitplugins_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.6.0b2/setup.py` & `flytekitplugins-snowflake-1.6.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "snowflake"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Snowflake plugins for flytekit",
```


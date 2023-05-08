# Comparing `tmp/flytekitplugins-pandera-1.6.0b2.tar.gz` & `tmp/flytekitplugins-pandera-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-pandera-1.6.0b2.tar", last modified: Fri May  5 17:49:48 2023, max compression
+gzip compressed data, was "flytekitplugins-pandera-1.6.0b3.tar", last modified: Mon May  8 20:18:45 2023, max compression
```

## Comparing `flytekitplugins-pandera-1.6.0b2.tar` & `flytekitplugins-pandera-1.6.0b3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.362193 flytekitplugins-pandera-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-05 17:49:48.358193 flytekitplugins-pandera-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 17:49:25.000000 flytekitplugins-pandera-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.358193 flytekitplugins-pandera-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.358193 flytekitplugins-pandera-1.6.0b2/flytekitplugins/pandera/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-05 17:49:25.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins/pandera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-05 17:49:25.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins/pandera/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.358193 flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-05 17:49:48.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 17:49:48.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:48.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:48.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 17:49:48.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:48.000000 flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:48.362193 flytekitplugins-pandera-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-05 17:49:40.000000 flytekitplugins-pandera-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.456860 flytekitplugins-pandera-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-08 20:18:45.456860 flytekitplugins-pandera-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 20:18:20.000000 flytekitplugins-pandera-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.452860 flytekitplugins-pandera-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.452860 flytekitplugins-pandera-1.6.0b3/flytekitplugins/pandera/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 20:18:20.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins/pandera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-08 20:18:20.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins/pandera/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.456860 flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-08 20:18:45.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 20:18:45.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:45.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:45.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 20:18:45.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:45.000000 flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:45.456860 flytekitplugins-pandera-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-08 20:18:37.000000 flytekitplugins-pandera-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-pandera-1.6.0b2/PKG-INFO` & `flytekitplugins-pandera-1.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.6.0b2/README.md` & `flytekitplugins-pandera-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.6.0b2/flytekitplugins/pandera/schema.py` & `flytekitplugins-pandera-1.6.0b3/flytekitplugins/pandera/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.6.0b2/flytekitplugins_pandera.egg-info/PKG-INFO` & `flytekitplugins-pandera-1.6.0b3/flytekitplugins_pandera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.6.0b2/setup.py` & `flytekitplugins-pandera-1.6.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "pandera"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pandera>=0.7.1"]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Pandera plugin for flytekit",
```


# Comparing `tmp/flytekitplugins-ray-1.6.0b2.tar.gz` & `tmp/flytekitplugins-ray-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-ray-1.6.0b2.tar", last modified: Fri May  5 17:49:49 2023, max compression
+gzip compressed data, was "flytekitplugins-ray-1.6.0b3.tar", last modified: Mon May  8 20:18:46 2023, max compression
```

## Comparing `flytekitplugins-ray-1.6.0b2.tar` & `flytekitplugins-ray-1.6.0b3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.446208 flytekitplugins-ray-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 17:49:49.446208 flytekitplugins-ray-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 17:49:25.000000 flytekitplugins-ray-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.442208 flytekitplugins-ray-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.442208 flytekitplugins-ray-1.6.0b2/flytekitplugins/ray/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 17:49:25.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 17:49:25.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins/ray/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-05 17:49:25.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins/ray/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.442208 flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 17:49:49.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 17:49:49.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:49.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 17:49:49.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:49.446208 flytekitplugins-ray-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-05 17:49:40.000000 flytekitplugins-ray-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.516856 flytekitplugins-ray-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-08 20:18:46.516856 flytekitplugins-ray-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 20:18:20.000000 flytekitplugins-ray-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.516856 flytekitplugins-ray-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.516856 flytekitplugins-ray-1.6.0b3/flytekitplugins/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-08 20:18:20.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-08 20:18:20.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins/ray/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-08 20:18:20.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins/ray/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:46.516856 flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-08 20:18:46.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 20:18:46.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:46.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:46.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 20:18:46.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:46.000000 flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:46.516856 flytekitplugins-ray-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-08 20:18:37.000000 flytekitplugins-ray-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-ray-1.6.0b2/PKG-INFO` & `flytekitplugins-ray-1.6.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-ray
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This package holds the Ray plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-ray-1.6.0b2/flytekitplugins/ray/models.py` & `flytekitplugins-ray-1.6.0b3/flytekitplugins/ray/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-ray-1.6.0b2/flytekitplugins/ray/task.py` & `flytekitplugins-ray-1.6.0b3/flytekitplugins/ray/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-ray-1.6.0b2/flytekitplugins_ray.egg-info/PKG-INFO` & `flytekitplugins-ray-1.6.0b3/flytekitplugins_ray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-ray
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This package holds the Ray plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-ray-1.6.0b2/setup.py` & `flytekitplugins-ray-1.6.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "ray"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["ray[default]", "flytekit>=1.3.0b2,<2.0.0", "flyteidl>=1.1.10"]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Ray plugins for flytekit",
```


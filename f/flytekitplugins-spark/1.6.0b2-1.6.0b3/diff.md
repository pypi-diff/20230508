# Comparing `tmp/flytekitplugins-spark-1.6.0b2.tar.gz` & `tmp/flytekitplugins-spark-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-spark-1.6.0b2.tar", last modified: Fri May  5 17:49:50 2023, max compression
+gzip compressed data, was "flytekitplugins-spark-1.6.0b3.tar", last modified: Mon May  8 20:18:47 2023, max compression
```

## Comparing `flytekitplugins-spark-1.6.0b2.tar` & `flytekitplugins-spark-1.6.0b3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/pyspark_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/sd_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/scripts/flytekit_install_spark3.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-05 17:49:40.000000 flytekitplugins-spark-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.228854 flytekitplugins-spark-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-08 20:18:47.228854 flytekitplugins-spark-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.224854 flytekitplugins-spark-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.224854 flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/pyspark_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/sd_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.224854 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-08 20:18:47.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 20:18:47.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:47.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 20:18:47.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:47.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 20:18:47.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:47.000000 flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.224854 flytekitplugins-spark-1.6.0b3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-08 20:18:20.000000 flytekitplugins-spark-1.6.0b3/scripts/flytekit_install_spark3.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:47.228854 flytekitplugins-spark-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-08 20:18:37.000000 flytekitplugins-spark-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-spark-1.6.0b2/PKG-INFO` & `flytekitplugins-spark-1.6.0b3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b2/README.md` & `flytekitplugins-spark-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/__init__.py` & `flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/models.py` & `flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/pyspark_transformers.py` & `flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/pyspark_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/schema.py` & `flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/sd_transformers.py` & `flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/task.py` & `flytekitplugins-spark-1.6.0b3/flytekitplugins/spark/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/PKG-INFO` & `flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/SOURCES.txt` & `flytekitplugins-spark-1.6.0b3/flytekitplugins_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/scripts/flytekit_install_spark3.sh` & `flytekitplugins-spark-1.6.0b3/scripts/flytekit_install_spark3.sh`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b2/setup.py` & `flytekitplugins-spark-1.6.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "spark"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pyspark>=3.0.0"]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Spark 3 plugin for flytekit",
```


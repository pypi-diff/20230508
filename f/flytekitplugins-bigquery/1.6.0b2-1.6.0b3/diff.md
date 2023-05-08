# Comparing `tmp/flytekitplugins-bigquery-1.6.0b2.tar.gz` & `tmp/flytekitplugins-bigquery-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.6.0b2.tar", last modified: Fri May  5 17:49:41 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.6.0b3.tar", last modified: Mon May  8 20:18:38 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.6.0b2.tar` & `flytekitplugins-bigquery-1.6.0b3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:41.510098 flytekitplugins-bigquery-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-05 17:49:41.510098 flytekitplugins-bigquery-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-05 17:49:25.000000 flytekitplugins-bigquery-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:41.506097 flytekitplugins-bigquery-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:41.506097 flytekitplugins-bigquery-1.6.0b2/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 17:49:25.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-05 17:49:25.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:41.506097 flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-05 17:49:41.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 17:49:41.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:41.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:41.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 17:49:41.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:41.000000 flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:41.510098 flytekitplugins-bigquery-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-05 17:49:40.000000 flytekitplugins-bigquery-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/backend_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 20:18:37.000000 flytekitplugins-bigquery-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-bigquery-1.6.0b2/PKG-INFO` & `flytekitplugins-bigquery-1.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.0b2/README.md` & `flytekitplugins-bigquery-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.0b2/flytekitplugins/bigquery/task.py` & `flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass
 from typing import Any, Dict, Optional, Type
 
 from google.cloud import bigquery
 from google.protobuf import json_format
 from google.protobuf.struct_pb2 import Struct
 
-from flytekit import StructuredDataset
 from flytekit.configuration import SerializationSettings
 from flytekit.extend import SQLTask
 from flytekit.models import task as _task_model
+from flytekit.types.structured import StructuredDataset
 
 
 @dataclass
 class BigQueryConfig(object):
     """
     BigQueryConfig should be used to configure a BigQuery Task.
     """
@@ -77,7 +77,10 @@
         s = Struct()
         s.update(config)
         return json_format.MessageToDict(s)
 
     def get_sql(self, settings: SerializationSettings) -> Optional[_task_model.Sql]:
         sql = _task_model.Sql(statement=self.query_template, dialect=_task_model.Sql.Dialect.ANSI)
         return sql
+
+    def execute(self, **kwargs) -> Any:
+        raise Exception("Cannot run a SQL Task natively, please mock.")
```

### Comparing `flytekitplugins-bigquery-1.6.0b2/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.0b2/setup.py` & `flytekitplugins-bigquery-1.6.0b3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
@@ -28,8 +28,9 @@
         "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    entry_points={"flytekit.plugins": [f"{PLUGIN_NAME}=flytekitplugins.{PLUGIN_NAME}"]},
 )
```


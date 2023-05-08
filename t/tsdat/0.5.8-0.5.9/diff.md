# Comparing `tmp/tsdat-0.5.8.tar.gz` & `tmp/tsdat-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsdat-0.5.8.tar", last modified: Fri Jan  6 00:20:06 2023, max compression
+gzip compressed data, was "tsdat-0.5.9.tar", last modified: Fri Jan 27 22:14:13 2023, max compression
```

## Comparing `tsdat-0.5.8.tar` & `tsdat-0.5.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.534017 tsdat-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-01-06 00:19:51.000000 tsdat-0.5.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-01-06 00:20:06.534017 tsdat-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-01-06 00:19:51.000000 tsdat-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-06 00:20:06.534017 tsdat-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-06 00:19:51.000000 tsdat-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.530017 tsdat-0.5.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-01-06 00:19:51.000000 tsdat-0.5.8/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.530017 tsdat-0.5.8/tsdat/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.530017 tsdat-0.5.8/tsdat/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/config/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.534017 tsdat-0.5.8/tsdat/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28925 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/io/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.534017 tsdat-0.5.8/tsdat/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/pipeline/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/pipeline/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.534017 tsdat-0.5.8/tsdat/qc/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/qc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/qc/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/qc/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-01-06 00:19:51.000000 tsdat-0.5.8/tsdat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:20:06.530017 tsdat-0.5.8/tsdat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-01-06 00:20:06.000000 tsdat-0.5.8/tsdat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-01-06 00:20:06.000000 tsdat-0.5.8/tsdat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 00:20:06.000000 tsdat-0.5.8/tsdat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-06 00:20:06.000000 tsdat-0.5.8/tsdat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 00:20:06.000000 tsdat-0.5.8/tsdat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-06 00:20:06.000000 tsdat-0.5.8/tsdat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-06 00:20:06.000000 tsdat-0.5.8/tsdat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.201209 tsdat-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-01-27 22:14:02.000000 tsdat-0.5.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-01-27 22:14:13.201209 tsdat-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-01-27 22:14:02.000000 tsdat-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-27 22:14:13.205209 tsdat-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-27 22:14:03.000000 tsdat-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.197209 tsdat-0.5.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-01-27 22:14:03.000000 tsdat-0.5.9/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.201209 tsdat-0.5.9/tsdat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.201209 tsdat-0.5.9/tsdat/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/config/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.201209 tsdat-0.5.9/tsdat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29131 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/io/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.201209 tsdat-0.5.9/tsdat/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/pipeline/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/pipeline/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.201209 tsdat-0.5.9/tsdat/qc/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/qc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/qc/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/qc/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-01-27 22:14:03.000000 tsdat-0.5.9/tsdat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 22:14:13.201209 tsdat-0.5.9/tsdat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-01-27 22:14:13.000000 tsdat-0.5.9/tsdat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-01-27 22:14:13.000000 tsdat-0.5.9/tsdat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 22:14:13.000000 tsdat-0.5.9/tsdat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-27 22:14:13.000000 tsdat-0.5.9/tsdat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 22:14:12.000000 tsdat-0.5.9/tsdat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-27 22:14:13.000000 tsdat-0.5.9/tsdat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-27 22:14:13.000000 tsdat-0.5.9/tsdat.egg-info/top_level.txt
```

### Comparing `tsdat-0.5.8/LICENSE.md` & `tsdat-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/PKG-INFO` & `tsdat-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsdat
-Version: 0.5.8
+Version: 0.5.9
 Summary: A data processing framework used to convert time series data into standardized format.
 Home-page: https://github.com/tsdat/tsdat
 Author: tsdat
 Author-email: tsdat@pnnl.gov
 License: Simplified BSD (2-clause)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsdat Version: 0.5.8 Summary: A data processing
+Metadata-Version: 2.1 Name: tsdat Version: 0.5.9 Summary: A data processing
 framework used to convert time series data into standardized format. Home-page:
 https://github.com/tsdat/tsdat Author: tsdat Author-email: tsdat@pnnl.gov
 License: Simplified BSD (2-clause) Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Topic :: Scientific/Engineering Classifier: Intended
```

### Comparing `tsdat-0.5.8/README.md` & `tsdat-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/setup.py` & `tsdat-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/__init__.py` & `tsdat-0.5.9/tsdat/__init__.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/attributes.py` & `tsdat-0.5.9/tsdat/config/attributes.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/dataset.py` & `tsdat-0.5.9/tsdat/config/dataset.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/pipeline.py` & `tsdat-0.5.9/tsdat/config/pipeline.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/quality.py` & `tsdat-0.5.9/tsdat/config/quality.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/retriever.py` & `tsdat-0.5.9/tsdat/config/retriever.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/storage.py` & `tsdat-0.5.9/tsdat/config/storage.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/utils.py` & `tsdat-0.5.9/tsdat/config/utils.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/config/variables.py` & `tsdat-0.5.9/tsdat/config/variables.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/io/base.py` & `tsdat-0.5.9/tsdat/io/base.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/io/converters.py` & `tsdat-0.5.9/tsdat/io/converters.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/io/handlers.py` & `tsdat-0.5.9/tsdat/io/handlers.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/io/readers.py` & `tsdat-0.5.9/tsdat/io/readers.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/io/retrievers.py` & `tsdat-0.5.9/tsdat/io/retrievers.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/io/storage.py` & `tsdat-0.5.9/tsdat/io/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,14 +390,18 @@
         
         Defaults to ``us-west-2``."""
 
         merge_fetched_data_kwargs: Dict[str, Any] = dict()
         """Keyword arguments to xr.merge. This will only be called if the
         DataReader returns a dictionary of xr.Datasets for a single saved file."""
 
+        @validator("storage_root")
+        def _ensure_storage_root_exists(cls, storage_root: Path) -> Path:
+            return storage_root  # HACK: Don't run parent validator to create storage root file
+
     parameters: Parameters = Field(default_factory=Parameters)  # type: ignore
 
     @validator("parameters")
     def _check_authentication(cls, parameters: Parameters):
         session = FileSystemS3._get_session(
             region=parameters.region, timehash=FileSystemS3._get_timehash()
         )
```

### Comparing `tsdat-0.5.8/tsdat/io/writers.py` & `tsdat-0.5.9/tsdat/io/writers.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/main.py` & `tsdat-0.5.9/tsdat/main.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/pipeline/base.py` & `tsdat-0.5.9/tsdat/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/pipeline/pipelines.py` & `tsdat-0.5.9/tsdat/pipeline/pipelines.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/qc/base.py` & `tsdat-0.5.9/tsdat/qc/base.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/qc/checkers.py` & `tsdat-0.5.9/tsdat/qc/checkers.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/qc/handlers.py` & `tsdat-0.5.9/tsdat/qc/handlers.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/testing.py` & `tsdat-0.5.9/tsdat/testing.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat/utils.py` & `tsdat-0.5.9/tsdat/utils.py`

 * *Files identical despite different names*

### Comparing `tsdat-0.5.8/tsdat.egg-info/PKG-INFO` & `tsdat-0.5.9/tsdat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsdat
-Version: 0.5.8
+Version: 0.5.9
 Summary: A data processing framework used to convert time series data into standardized format.
 Home-page: https://github.com/tsdat/tsdat
 Author: tsdat
 Author-email: tsdat@pnnl.gov
 License: Simplified BSD (2-clause)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsdat Version: 0.5.8 Summary: A data processing
+Metadata-Version: 2.1 Name: tsdat Version: 0.5.9 Summary: A data processing
 framework used to convert time series data into standardized format. Home-page:
 https://github.com/tsdat/tsdat Author: tsdat Author-email: tsdat@pnnl.gov
 License: Simplified BSD (2-clause) Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Topic :: Scientific/Engineering Classifier: Intended
```

### Comparing `tsdat-0.5.8/tsdat.egg-info/SOURCES.txt` & `tsdat-0.5.9/tsdat.egg-info/SOURCES.txt`

 * *Files identical despite different names*


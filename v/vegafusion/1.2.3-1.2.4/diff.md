# Comparing `tmp/vegafusion-1.2.3.tar.gz` & `tmp/vegafusion-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.2.3.tar", last modified: Mon May  1 16:02:23 2023, max compression
+gzip compressed data, was "vegafusion-1.2.4.tar", last modified: Mon May  8 19:46:50 2023, max compression
```

## Comparing `vegafusion-1.2.3.tar` & `vegafusion-1.2.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:02:23.860242 vegafusion-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-01 16:01:10.000000 vegafusion-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-01 16:02:23.860242 vegafusion-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-01 16:01:10.000000 vegafusion-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 16:01:10.000000 vegafusion-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-01 16:02:23.860242 vegafusion-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:01:10.000000 vegafusion-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:02:23.856243 vegafusion-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-01 16:01:10.000000 vegafusion-1.2.3/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:02:23.856243 vegafusion-1.2.3/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:02:23.860242 vegafusion-1.2.3/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 16:01:10.000000 vegafusion-1.2.3/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:02:23.856243 vegafusion-1.2.3/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-01 16:02:23.000000 vegafusion-1.2.3/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-01 16:02:23.000000 vegafusion-1.2.3/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:02:23.000000 vegafusion-1.2.3/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 16:02:23.000000 vegafusion-1.2.3/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 16:02:23.000000 vegafusion-1.2.3/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:46:50.716281 vegafusion-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 19:45:28.000000 vegafusion-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 19:46:50.716281 vegafusion-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 19:45:28.000000 vegafusion-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-08 19:45:28.000000 vegafusion-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-08 19:46:50.716281 vegafusion-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:45:28.000000 vegafusion-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:46:50.712281 vegafusion-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-08 19:45:28.000000 vegafusion-1.2.4/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:46:50.716281 vegafusion-1.2.4/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:46:50.716281 vegafusion-1.2.4/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-08 19:45:28.000000 vegafusion-1.2.4/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:46:50.716281 vegafusion-1.2.4/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 19:46:50.000000 vegafusion-1.2.4/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-08 19:46:50.000000 vegafusion-1.2.4/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:46:50.000000 vegafusion-1.2.4/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 19:46:50.000000 vegafusion-1.2.4/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 19:46:50.000000 vegafusion-1.2.4/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.2.3/LICENSE.txt` & `vegafusion-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/PKG-INFO` & `vegafusion-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.2.3
+Version: 1.2.4
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.2.3/README.md` & `vegafusion-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/setup.cfg` & `vegafusion-1.2.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.2.3
+version = 1.2.4
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.2.3
+	vegafusion-python-embed==1.2.4
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.2.3/tests/test_conext_manager.py` & `vegafusion-1.2.4/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/tests/test_input_utc.py` & `vegafusion-1.2.4/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/tests/test_pretransform.py` & `vegafusion-1.2.4/tests/test_pretransform.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/tests/test_pretransform_specs.py` & `vegafusion-1.2.4/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/tests/test_row_limit.py` & `vegafusion-1.2.4/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/tests/test_save.py` & `vegafusion-1.2.4/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/tests/test_transformed_data.py` & `vegafusion-1.2.4/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/tests/test_transformer.py` & `vegafusion-1.2.4/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/__init__.py` & `vegafusion-1.2.4/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/compilers.py` & `vegafusion-1.2.4/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/connection/__init__.py` & `vegafusion-1.2.4/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/connection/duckdb.py` & `vegafusion-1.2.4/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/evaluation.py` & `vegafusion-1.2.4/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/local_tz.py` & `vegafusion-1.2.4/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/renderer.py` & `vegafusion-1.2.4/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/runtime.py` & `vegafusion-1.2.4/vegafusion/runtime.py`

 * *Files 16% similar despite different names*

```diff
@@ -380,14 +380,39 @@
             finally:
                 # Clean up temporary tables
                 if self._connection is not None:
                     self._connection.unregister_temporary_tables()
 
             return new_spec, datasets, warnings
 
+    def patch_pre_transformed_spec(self, spec1, pre_transformed_spec1, spec2):
+        """
+        Attempt to patch a Vega spec was returned by the pre_transform_spec method without
+        rerunning the pre_transform_spec logic. When possible, this can be significantly
+        faster than rerunning the pre_transform_spec method.
+
+        :param spec1: The input Vega spec to a prior call to pre_transform_spec
+        :param pre_transformed_spec1: The prior result of passing spec1 to pre_transform_spec
+        :param spec2: A Vega spec that is assumed to be a small delta compared to spec1
+
+        :return: dict or None
+            If the delta between spec1 and spec2 is in the portions of spec1 that were not
+            modified by pre_transform_spec, then this delta can be applied cleanly to
+            pre_transform_spec1 and the result is returned. If the delta cannot be
+            applied cleanly, None is returned and spec2 should be passed through the
+            pre_transform_spec method.
+        """
+        if self._grpc_channel:
+            raise ValueError("patch_pre_transformed_spec not yet supported over gRPC")
+        else:
+            pre_transformed_spec2 = self.embedded_runtime.patch_pre_transformed_spec(
+                spec1, pre_transformed_spec1, spec2
+            )
+            return pre_transformed_spec2
+
     @property
     def worker_threads(self):
         return self._worker_threads
 
     @worker_threads.setter
     def worker_threads(self, value):
         """
```

### Comparing `vegafusion-1.2.3/vegafusion/save.py` & `vegafusion-1.2.4/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/transformer.py` & `vegafusion-1.2.4/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion/utils.py` & `vegafusion-1.2.4/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.3/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.2.4/vegafusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.2.3
+Version: 1.2.4
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.2.3/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.2.4/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*


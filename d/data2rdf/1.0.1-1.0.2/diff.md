# Comparing `tmp/data2rdf-1.0.1.tar.gz` & `tmp/data2rdf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-1.0.1.tar", last modified: Tue May  2 12:13:27 2023, max compression
+gzip compressed data, was "data2rdf-1.0.2.tar", last modified: Mon May  8 07:35:20 2023, max compression
```

## Comparing `data2rdf-1.0.1.tar` & `data2rdf-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.905405 data2rdf-1.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-02 12:13:12.000000 data2rdf-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-02 12:13:27.905405 data2rdf-1.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2505 2023-05-02 12:13:12.000000 data2rdf-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.901405 data2rdf-1.0.1/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6592 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/abox_template_generation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/annotation_confs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.901405 data2rdf-1.0.1/data2rdf/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/cli/abox_conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6658 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/csv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.901405 data2rdf-1.0.1/data2rdf/emmo_lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/emmo_lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3053 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/emmo_lib/chowlk_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/emmo_lib/emmo_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      732 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/emmo_lib/get_emmo_label_mappping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2024 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/emmo_lib/get_emmo_unit_prefix_df.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9989 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/excel_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16561 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/mapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      223 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/pipeline_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8078 2023-05-02 12:13:12.000000 data2rdf-1.0.1/data2rdf/rdf_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.901405 data2rdf-1.0.1/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-02 12:13:27.000000 data2rdf-1.0.1/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-02 12:13:27.000000 data2rdf-1.0.1/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:13:27.000000 data2rdf-1.0.1/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 12:13:27.000000 data2rdf-1.0.1/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-02 12:13:27.000000 data2rdf-1.0.1/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 12:13:27.000000 data2rdf-1.0.1/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1861 2023-05-02 12:13:27.905405 data2rdf-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-05-02 12:13:12.000000 data2rdf-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.901405 data2rdf-1.0.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.905405 data2rdf-1.0.1/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.905405 data2rdf-1.0.1/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/csv_pipeline_test/input/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/csv_pipeline_test/test_abox_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2555 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/csv_pipeline_test/test_csv2rdf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/csv_pipeline_test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:27.905405 data2rdf-1.0.1/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/xls_pipeline_test/test_abox_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2090 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/xls_pipeline_test/test_excel2rdf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-05-02 12:13:12.000000 data2rdf-1.0.1/tests/xls_pipeline_test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.238593 data2rdf-1.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-08 07:35:05.000000 data2rdf-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-08 07:35:20.238593 data2rdf-1.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2505 2023-05-08 07:35:05.000000 data2rdf-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.234593 data2rdf-1.0.2/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6592 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/abox_template_generation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/annotation_confs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.234593 data2rdf-1.0.2/data2rdf/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/cli/abox_conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6658 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/csv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.234593 data2rdf-1.0.2/data2rdf/emmo_lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/emmo_lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3053 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/emmo_lib/chowlk_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/emmo_lib/emmo_unit_prefixes.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/emmo_lib/emmo_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      732 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/emmo_lib/get_emmo_label_mappping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2024 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/emmo_lib/get_emmo_unit_prefix_df.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9989 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/excel_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16561 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/mapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      223 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/pipeline_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8078 2023-05-08 07:35:05.000000 data2rdf-1.0.2/data2rdf/rdf_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.234593 data2rdf-1.0.2/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-08 07:35:20.000000 data2rdf-1.0.2/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-08 07:35:20.000000 data2rdf-1.0.2/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:35:20.000000 data2rdf-1.0.2/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 07:35:20.000000 data2rdf-1.0.2/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-08 07:35:20.000000 data2rdf-1.0.2/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 07:35:20.000000 data2rdf-1.0.2/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-05-08 07:35:20.238593 data2rdf-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-05-08 07:35:05.000000 data2rdf-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.234593 data2rdf-1.0.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.234593 data2rdf-1.0.2/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.234593 data2rdf-1.0.2/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/csv_pipeline_test/input/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/csv_pipeline_test/test_abox_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2555 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/csv_pipeline_test/test_csv2rdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/csv_pipeline_test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:20.238593 data2rdf-1.0.2/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/xls_pipeline_test/test_abox_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2090 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/xls_pipeline_test/test_excel2rdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-05-08 07:35:05.000000 data2rdf-1.0.2/tests/xls_pipeline_test/test_utils.py
```

### Comparing `data2rdf-1.0.1/LICENSE` & `data2rdf-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/PKG-INFO` & `data2rdf-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 1.0.1
+Version: 1.0.2
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy
 Author-email: paul.zierep@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-1.0.1/README.md` & `data2rdf-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/abox_template_generation.py` & `data2rdf-1.0.2/data2rdf/abox_template_generation.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/annotation_confs.py` & `data2rdf-1.0.2/data2rdf/annotation_confs.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/annotation_pipeline.py` & `data2rdf-1.0.2/data2rdf/annotation_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/cli/abox_conversion.py` & `data2rdf-1.0.2/data2rdf/cli/abox_conversion.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/csv_parser.py` & `data2rdf-1.0.2/data2rdf/csv_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/emmo_lib/chowlk_utils.py` & `data2rdf-1.0.2/data2rdf/emmo_lib/chowlk_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/emmo_lib/emmo_utils.py` & `data2rdf-1.0.2/data2rdf/emmo_lib/emmo_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/emmo_lib/get_emmo_label_mappping.py` & `data2rdf-1.0.2/data2rdf/emmo_lib/get_emmo_label_mappping.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/emmo_lib/get_emmo_unit_prefix_df.py` & `data2rdf-1.0.2/data2rdf/emmo_lib/get_emmo_unit_prefix_df.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/excel_parser.py` & `data2rdf-1.0.2/data2rdf/excel_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/mapper.py` & `data2rdf-1.0.2/data2rdf/mapper.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf/rdf_generation.py` & `data2rdf-1.0.2/data2rdf/rdf_generation.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/data2rdf.egg-info/PKG-INFO` & `data2rdf-1.0.2/data2rdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 1.0.1
+Version: 1.0.2
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy
 Author-email: paul.zierep@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-1.0.1/data2rdf.egg-info/SOURCES.txt` & `data2rdf-1.0.2/data2rdf.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 data2rdf.egg-info/entry_points.txt
 data2rdf.egg-info/requires.txt
 data2rdf.egg-info/top_level.txt
 data2rdf/cli/__init__.py
 data2rdf/cli/abox_conversion.py
 data2rdf/emmo_lib/__init__.py
 data2rdf/emmo_lib/chowlk_utils.py
+data2rdf/emmo_lib/emmo_unit_prefixes.csv
 data2rdf/emmo_lib/emmo_utils.py
 data2rdf/emmo_lib/get_emmo_label_mappping.py
 data2rdf/emmo_lib/get_emmo_unit_prefix_df.py
 tests/__init__.py
 tests/csv_pipeline_test/__init__.py
 tests/csv_pipeline_test/test_abox_pipeline.py
 tests/csv_pipeline_test/test_csv2rdf.py
```

### Comparing `data2rdf-1.0.1/setup.cfg` & `data2rdf-1.0.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v1.0.1
+version = v1.0.2
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy
 author_email = paul.zierep@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de
 license = BSD-3-Clause
@@ -52,19 +52,16 @@
 	sphinxcontrib-redoc==1.6.0
 pre_commit = 
 	pre-commit==2.15.0
 tests = 
 	pytest==6.2.5
 
 [options.package_data]
-* = emmo_units.csv,
-	emmo_unit_prefixes.csv,
-	chowlk/*,
-	chowlk/*/*,
-	chowlk/*/*/*
+* = emmo_lib/emmo_units.csv,
+	emmo_lib/emmo_unit_prefixes.csv
 
 [bumpver]
 current_version = "v0.0.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
```

### Comparing `data2rdf-1.0.1/tests/csv_pipeline_test/test_abox_pipeline.py` & `data2rdf-1.0.2/tests/csv_pipeline_test/test_abox_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/tests/csv_pipeline_test/test_csv2rdf.py` & `data2rdf-1.0.2/tests/csv_pipeline_test/test_csv2rdf.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/tests/xls_pipeline_test/test_abox_pipeline.py` & `data2rdf-1.0.2/tests/xls_pipeline_test/test_abox_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-1.0.1/tests/xls_pipeline_test/test_excel2rdf.py` & `data2rdf-1.0.2/tests/xls_pipeline_test/test_excel2rdf.py`

 * *Files identical despite different names*


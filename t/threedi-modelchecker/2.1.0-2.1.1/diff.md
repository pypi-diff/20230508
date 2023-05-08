# Comparing `tmp/threedi-modelchecker-2.1.0.tar.gz` & `tmp/threedi-modelchecker-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-modelchecker-2.1.0.tar", last modified: Mon Mar 27 14:26:22 2023, max compression
+gzip compressed data, was "threedi-modelchecker-2.1.1.tar", last modified: Mon May  8 13:57:24 2023, max compression
```

## Comparing `threedi-modelchecker-2.1.0.tar` & `threedi-modelchecker-2.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:22.146506 threedi-modelchecker-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-27 14:26:22.146506 threedi-modelchecker-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-27 14:26:22.150506 threedi-modelchecker-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:22.138506 threedi-modelchecker-2.1.0/threedi_modelchecker/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:22.142506 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/geo_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/checks/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    87872 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:22.142506 threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/raster_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/raster_interface_gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/raster_interface_rasterio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/model_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:22.146506 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:22.146506 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:17.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/data/empty_v4.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_other.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-27 14:26:18.000000 threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_model_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:26:22.142506 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-27 14:26:22.000000 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-27 14:26:22.000000 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:26:22.000000 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-27 14:26:22.000000 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:26:22.000000 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-27 14:26:22.000000 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 14:26:22.000000 threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.678184 threedi-modelchecker-2.1.1/threedi_modelchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.682184 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/geo_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29978 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90598 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.682184 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_rasterio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/data/empty_v4.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_model_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.682184 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/top_level.txt
```

### Comparing `threedi-modelchecker-2.1.0/CHANGES.rst` & `threedi-modelchecker-2.1.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changelog of threedi-modelchecker
 =================================
 
 
+2.1.1 (2023-05-08)
+------------------
+
+- Vegetation_drag column names have changed. Update column names in code.
+
+- Bump threedi-schema version to 0.217.0.
+
+
 2.1.0 (2023-03-27)
 ------------------
 
 - Add support for designating beta features in threedi-schema. If a user puts a
   non-null value in a column marked as beta in threedi-schema, a BetaFeaturesCheck
   error 1300 will be raised by the modelchecker. The allow-beta flag has been added
   to the CLI interface to disable this check temporarily.
```

### Comparing `threedi-modelchecker-2.1.0/LICENSE` & `threedi-modelchecker-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/PKG-INFO` & `threedi-modelchecker-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.1.0
+Version: 2.1.1
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.1.0/README.rst` & `threedi-modelchecker-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/setup.py` & `threedi-modelchecker-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 
 from setuptools import setup
 
 long_description = "\n\n".join([open("README.rst").read()])
 
 install_requires = [
-    "threedi-schema==0.216.*,>=0.216.2",
+    "threedi-schema==0.217.*",
     "Click",
     "GeoAlchemy2>=0.9,!=0.11.*",
     "SQLAlchemy>=1.4",
 ]
 
 tests_require = [
     "pytest",
```

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/checks/base.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/checks/cross_section_definitions.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/checks/factories.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/checks/geo_query.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/geo_query.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/checks/other.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/other.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import List, Literal, NamedTuple
 
-from sqlalchemy import func, text
+from sqlalchemy import case, cast, distinct, func, REAL, select, text
 from sqlalchemy.orm import aliased, Query, Session
 from threedi_schema import constants, models
 
 from .base import BaseCheck, CheckLevel
 from .geo_query import distance, length, transform
 
 # Use these to make checks only work on the first global settings entry:
@@ -40,14 +40,168 @@
     def description(self):
         return (
             f"v2_cross_section_location.the_geom is invalid: the cross-section location "
             f"should be located on the channel geometry (tolerance = {self.max_distance} m)"
         )
 
 
+class CrossSectionSameConfigurationCheck(BaseCheck):
+    """Check the cross-sections on the object are either all open or all closed."""
+
+    def first_number_in_spaced_string(self, spaced_string):
+        """return the first number in a space-separated string like '1 2 3'"""
+        return cast(
+            func.substr(
+                spaced_string,
+                1,
+                func.instr(spaced_string, " ") - 1,
+            ),
+            REAL,
+        )
+
+    def last_number_in_spaced_string(self, spaced_string):
+        """return the last number in a space-separated string like '1 2 3'"""
+        return cast(
+            func.replace(
+                spaced_string,
+                func.rtrim(
+                    spaced_string,
+                    func.replace(spaced_string, " ", ""),
+                ),
+                "",
+            ),
+            REAL,
+        )
+
+    def configuration_type(
+        self, shape, first_width, last_width, first_height, last_height
+    ):
+        return case(
+            (
+                (
+                    (shape.in_([0, 2, 3, 8]))
+                    | (shape.in_([5, 6]) & (last_width == 0))
+                    | (
+                        (shape == 7)
+                        & (first_width == last_width)
+                        & (first_height == last_height)
+                    )
+                ),
+                "closed",
+            ),
+            (
+                (
+                    (shape == 1)
+                    | ((shape.in_([5, 6]) & (last_width > 0)))
+                    | (
+                        (shape == 7)
+                        & ((first_width != last_width) | (first_height != last_height))
+                    )
+                ),
+                "open",
+            ),
+            else_="open",
+        )
+
+    def get_invalid(self, session):
+        # get all channels with more than 1 cross section location
+        cross_sections = (
+            select(
+                models.CrossSectionLocation.id.label("cross_section_id"),
+                models.CrossSectionLocation.channel_id,
+                models.CrossSectionDefinition.shape,
+                models.CrossSectionDefinition.width,
+                models.CrossSectionDefinition.height,
+                self.first_number_in_spaced_string(
+                    models.CrossSectionDefinition.width
+                ).label("first_width"),
+                self.first_number_in_spaced_string(
+                    models.CrossSectionDefinition.height
+                ).label("first_height"),
+                self.last_number_in_spaced_string(
+                    models.CrossSectionDefinition.width
+                ).label("last_width"),
+                self.last_number_in_spaced_string(
+                    models.CrossSectionDefinition.height
+                ).label("last_height"),
+            )
+            .select_from(models.CrossSectionLocation)
+            .join(
+                models.CrossSectionDefinition,
+                models.CrossSectionLocation.definition_id
+                == models.CrossSectionDefinition.id,
+            )
+            .subquery()
+        )
+        cross_sections_with_configuration = select(
+            cross_sections.c.cross_section_id,
+            cross_sections.c.shape,
+            cross_sections.c.last_width,
+            cross_sections.c.channel_id,
+            self.configuration_type(
+                shape=cross_sections.c.shape,
+                first_width=cross_sections.c.first_width,
+                last_width=cross_sections.c.last_width,
+                first_height=cross_sections.c.first_height,
+                last_height=cross_sections.c.last_height,
+            ).label("configuration"),
+        ).subquery()
+        filtered_cross_sections = (
+            select(cross_sections_with_configuration)
+            .group_by(cross_sections_with_configuration.c.channel_id)
+            .having(
+                func.count(distinct(cross_sections_with_configuration.c.configuration))
+                > 1
+            )
+            .subquery()
+        )
+
+        def is_valid_series(input):
+            try:
+                [float(i) for i in input.split(" ")]
+                return True
+            except ValueError:
+                return False
+
+        def is_valid_value(input):
+            if input in ["", None] or is_valid_series(input):
+                return True
+            else:
+                return False
+
+        all_cross_sections = session.execute(
+            select(
+                models.CrossSectionDefinition.width,
+                models.CrossSectionDefinition.height,
+            )
+        )
+
+        error_in_cross_sections = False
+
+        for row in all_cross_sections.all():
+            if not is_valid_value(row[0]) or not is_valid_value(row[1]):
+                error_in_cross_sections = True
+                break  # no need to continue checking; one error is enough to not run the check
+
+        # only run the check if all the cross-section definitions have a parsable width and height
+        # otherwise sqlalchemy will throw an exception
+        # this is also checked in checks 87 and 88 (CrossSectionFloatListCheck), where it gives an error to the user
+        if not error_in_cross_sections:
+            return (
+                self.to_check(session)
+                .filter(self.column == filtered_cross_sections.c.channel_id)
+                .all()
+            )
+        else:
+            return []
+
+    def description(self):
+        return f"{self.column_name} has both open and closed cross-sections along its length. All cross-sections on a {self.column_name} object must be either open or closed."
+
+
 class Use0DFlowCheck(BaseCheck):
     """Check that when use_0d_flow in global settings is configured to 1 or to
     2, there is at least one impervious surface or surfaces respectively.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(column=models.GlobalSetting.use_0d_inflow, *args, **kwargs)
@@ -549,14 +703,73 @@
             .all()
         )
 
     def description(self) -> str:
         return f"{self.column_name} will empty its storage faster than one timestep, which can cause simulation instabilities"
 
 
+class ImperviousNodeInflowAreaCheck(BaseCheck):
+    """Check that total inflow area per connection node is no larger than 10000 square metres"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(column=models.ConnectionNode.id, *args, **kwargs)
+
+    def get_invalid(self, session: Session) -> List[NamedTuple]:
+        impervious_surfaces = (
+            select(models.ImperviousSurfaceMap.connection_node_id)
+            .select_from(models.ImperviousSurfaceMap)
+            .join(
+                models.ImperviousSurface,
+                models.ImperviousSurfaceMap.impervious_surface_id
+                == models.ImperviousSurface.id,
+            )
+            .group_by(models.ImperviousSurfaceMap.connection_node_id)
+            .having(func.sum(models.ImperviousSurface.area) > 10000)
+        ).subquery()
+
+        return (
+            session.query(models.ConnectionNode)
+            .filter(
+                models.ConnectionNode.id == impervious_surfaces.c.connection_node_id
+            )
+            .all()
+        )
+
+    def description(self) -> str:
+        return f"{self.column_name} has a an associated inflow area larger than 10000 m2; this might be an error."
+
+
+class PerviousNodeInflowAreaCheck(BaseCheck):
+    """Check that total inflow area per connection node is no larger than 10000 square metres"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(column=models.ConnectionNode.id, *args, **kwargs)
+
+    def get_invalid(self, session: Session) -> List[NamedTuple]:
+        pervious_surfaces = (
+            select(models.SurfaceMap.connection_node_id)
+            .select_from(models.SurfaceMap)
+            .join(
+                models.Surface,
+                models.SurfaceMap.surface_id == models.Surface.id,
+            )
+            .group_by(models.SurfaceMap.connection_node_id)
+            .having(func.sum(models.Surface.area) > 10000)
+        ).subquery()
+
+        return (
+            session.query(models.ConnectionNode)
+            .filter(models.ConnectionNode.id == pervious_surfaces.c.connection_node_id)
+            .all()
+        )
+
+    def description(self) -> str:
+        return f"{self.column_name} has a an associated inflow area larger than 10000 m2; this might be an error."
+
+
 class BetaColumnsCheck(BaseCheck):
     """Check that no beta columns were used in the database"""
 
     def get_invalid(self, session: Session) -> List[NamedTuple]:
         return session.query(self.table).filter(self.column.isnot(None)).all()
 
     def description(self) -> str:
```

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/checks/raster.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/checks/timeseries.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/config.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,19 @@
     BetaColumnsCheck,
     BetaValuesCheck,
     BoundaryCondition1DObjectNumberCheck,
     ChannelManholeLevelCheck,
     ConnectionNodesDistance,
     ConnectionNodesLength,
     CrossSectionLocationCheck,
+    CrossSectionSameConfigurationCheck,
+    ImperviousNodeInflowAreaCheck,
     LinestringLocationCheck,
     OpenChannelsWithNestedNewton,
+    PerviousNodeInflowAreaCheck,
     PotentialBreachInterdistanceCheck,
     PotentialBreachStartEndCheck,
     PumpStorageTimestepCheck,
     SpatialIndexCheck,
     Use0DFlowCheck,
 )
 from .checks.raster import (
@@ -313,14 +316,19 @@
         error_code=55,
         column=models.Channel.id,
         invalid=Query(models.Channel).filter(
             ~models.Channel.cross_section_locations.any()
         ),
         message="v2_channel has no cross section locations",
     ),
+    CrossSectionSameConfigurationCheck(
+        error_code=56,
+        level=CheckLevel.ERROR,
+        column=models.Channel.id,
+    ),
 ]
 
 ## 006x: PUMPSTATIONS
 
 CHECKS += [
     QueryCheck(
         error_code=61,
@@ -334,14 +342,32 @@
         error_code=62,
         column=models.Pumpstation.lower_stop_level,
         invalid=Query(models.Pumpstation).filter(
             models.Pumpstation.lower_stop_level >= models.Pumpstation.start_level,
         ),
         message="v2_pumpstation.lower_stop_level should be less than v2_pumpstation.start_level",
     ),
+    QueryCheck(
+        error_code=63,
+        level=CheckLevel.ERROR,
+        column=models.ConnectionNode.storage_area,
+        invalid=Query(models.ConnectionNode)
+        .join(
+            models.Pumpstation,
+            models.Pumpstation.connection_node_end_id == models.ConnectionNode.id,
+        )
+        .filter(models.ConnectionNode.storage_area != None)
+        .filter(
+            models.ConnectionNode.storage_area * 1000 <= models.Pumpstation.capacity
+        ),
+        message=(
+            "v2_connection_nodes.storage_area * 1000 for each pumpstation's end connection node must be greater than v2_pumpstation.capacity; "
+            + "water level should not rise >= 1 m in one second"
+        ),
+    ),
     RangeCheck(
         error_code=64,
         column=models.Pumpstation.capacity,
         min_value=0,
     ),
     QueryCheck(
         error_code=65,
@@ -1655,123 +1681,123 @@
     ),
 ]
 
 ## 05xx: VEGETATION DRAG
 CHECKS += [
     RangeCheck(
         error_code=501,
-        column=models.VegetationDrag.height,
+        column=models.VegetationDrag.vegetation_height,
         filters=vegetation_drag_filter,
         min_value=0,
         left_inclusive=False,
     ),
     QueryCheck(
         error_code=502,
-        column=models.VegetationDrag.height,
+        column=models.VegetationDrag.vegetation_height,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.height == None,
-            is_none_or_empty(models.VegetationDrag.height_file),
+            models.VegetationDrag.vegetation_height == None,
+            is_none_or_empty(models.VegetationDrag.vegetation_height_file),
         ),
         message="v2_vegetation_drag.height must be defined.",
     ),
     QueryCheck(
         error_code=503,
         level=CheckLevel.WARNING,
-        column=models.VegetationDrag.height,
+        column=models.VegetationDrag.vegetation_height,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.height == None,
-            ~is_none_or_empty(models.VegetationDrag.height_file),
+            models.VegetationDrag.vegetation_height == None,
+            ~is_none_or_empty(models.VegetationDrag.vegetation_height_file),
         ),
-        message="v2_vegetation_drag.height is recommended as fallback value when using a height_file.",
+        message="v2_vegetation_drag.height is recommended as fallback value when using a vegetation_height_file.",
     ),
     RangeCheck(
         error_code=504,
-        column=models.VegetationDrag.stem_count,
+        column=models.VegetationDrag.vegetation_stem_count,
         filters=vegetation_drag_filter,
         min_value=0,
         left_inclusive=False,
     ),
     QueryCheck(
         error_code=505,
-        column=models.VegetationDrag.stem_count,
+        column=models.VegetationDrag.vegetation_stem_count,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.stem_count == None,
-            is_none_or_empty(models.VegetationDrag.stem_count_file),
+            models.VegetationDrag.vegetation_stem_count == None,
+            is_none_or_empty(models.VegetationDrag.vegetation_stem_count_file),
         ),
-        message="v2_vegetation_drag.stem_count must be defined.",
+        message="v2_vegetation_drag.vegetation_stem_count must be defined.",
     ),
     QueryCheck(
         error_code=506,
         level=CheckLevel.WARNING,
-        column=models.VegetationDrag.stem_count,
+        column=models.VegetationDrag.vegetation_stem_count,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.stem_count == None,
-            ~is_none_or_empty(models.VegetationDrag.stem_count_file),
+            models.VegetationDrag.vegetation_stem_count == None,
+            ~is_none_or_empty(models.VegetationDrag.vegetation_stem_count_file),
         ),
-        message="v2_vegetation_drag.stem_count is recommended as fallback value when using a stem_count_file.",
+        message="v2_vegetation_drag.vegetation_stem_count is recommended as fallback value when using a vegetation_stem_count_file.",
     ),
     RangeCheck(
         error_code=507,
-        column=models.VegetationDrag.stem_diameter,
+        column=models.VegetationDrag.vegetation_stem_diameter,
         filters=vegetation_drag_filter,
         min_value=0,
         left_inclusive=False,
     ),
     QueryCheck(
         error_code=508,
-        column=models.VegetationDrag.stem_diameter,
+        column=models.VegetationDrag.vegetation_stem_diameter,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.stem_diameter == None,
-            is_none_or_empty(models.VegetationDrag.stem_diameter_file),
+            models.VegetationDrag.vegetation_stem_diameter == None,
+            is_none_or_empty(models.VegetationDrag.vegetation_stem_diameter_file),
         ),
-        message="v2_vegetation_drag.stem_diameter must be defined.",
+        message="v2_vegetation_drag.vegetation_stem_diameter must be defined.",
     ),
     QueryCheck(
         error_code=509,
         level=CheckLevel.WARNING,
-        column=models.VegetationDrag.stem_diameter,
+        column=models.VegetationDrag.vegetation_stem_diameter,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.stem_diameter == None,
-            ~is_none_or_empty(models.VegetationDrag.stem_diameter_file),
+            models.VegetationDrag.vegetation_stem_diameter == None,
+            ~is_none_or_empty(models.VegetationDrag.vegetation_stem_diameter_file),
         ),
-        message="v2_vegetation_drag.stem_diameter is recommended as fallback value when using a stem_diameter_file.",
+        message="v2_vegetation_drag.vegetation_stem_diameter is recommended as fallback value when using a vegetation_stem_diameter_file.",
     ),
     RangeCheck(
         error_code=510,
-        column=models.VegetationDrag.drag_coefficient,
+        column=models.VegetationDrag.vegetation_drag_coefficient,
         filters=vegetation_drag_filter,
         min_value=0,
         left_inclusive=False,
     ),
     QueryCheck(
         error_code=511,
-        column=models.VegetationDrag.drag_coefficient,
+        column=models.VegetationDrag.vegetation_drag_coefficient,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.drag_coefficient == None,
-            is_none_or_empty(models.VegetationDrag.drag_coefficient_file),
+            models.VegetationDrag.vegetation_drag_coefficient == None,
+            is_none_or_empty(models.VegetationDrag.vegetation_drag_coefficient_file),
         ),
-        message="v2_vegetation_drag.drag_coefficient must be defined.",
+        message="v2_vegetation_drag.vegetation_drag_coefficient must be defined.",
     ),
     QueryCheck(
         error_code=512,
         level=CheckLevel.WARNING,
-        column=models.VegetationDrag.drag_coefficient,
+        column=models.VegetationDrag.vegetation_drag_coefficient,
         invalid=Query(models.VegetationDrag).filter(
             vegetation_drag_filter,
-            models.VegetationDrag.drag_coefficient == None,
-            ~is_none_or_empty(models.VegetationDrag.drag_coefficient_file),
+            models.VegetationDrag.vegetation_drag_coefficient == None,
+            ~is_none_or_empty(models.VegetationDrag.vegetation_drag_coefficient_file),
         ),
-        message="v2_vegetation_drag.drag_coefficient is recommended as fallback value when using a drag_coefficient_file.",
+        message="v2_vegetation_drag.vegetation_drag_coefficient is recommended as fallback value when using a vegetation_drag_coefficient_file.",
     ),
 ]
 
 ## 06xx: INFLOW
 for (surface, surface_map, filters) in [
     (models.Surface, models.SurfaceMap, CONDITIONS["0d_surf"].exists()),
     (
@@ -1822,14 +1848,22 @@
                 surface_map.connection_node_id.in_(
                     Query(models.BoundaryCondition1D.connection_node_id)
                 ),
             ),
             message=f"{surface_map.__tablename__} will be ignored because it is connected to a 1D boundary condition.",
         ),
     ]
+CHECKS += [
+    ImperviousNodeInflowAreaCheck(
+        error_code=613, level=CheckLevel.WARNING, filters=CONDITIONS["0d_imp"].exists()
+    ),
+    PerviousNodeInflowAreaCheck(
+        error_code=613, level=CheckLevel.WARNING, filters=CONDITIONS["0d_surf"].exists()
+    ),
+]
 
 
 CHECKS += [
     RangeCheck(
         error_code=606,
         column=models.SurfaceParameter.outflow_delay,
         min_value=0,
@@ -1907,18 +1941,18 @@
     ),
     (models.GroundWater.leakage_file, groundwater_filter),
     (models.GlobalSetting.initial_waterlevel_file, first_setting_filter),
     (
         models.GlobalSetting.initial_groundwater_level_file,
         first_setting_filter & (models.GlobalSetting.groundwater_settings_id != None),
     ),
-    (models.VegetationDrag.height_file, vegetation_drag_filter),
-    (models.VegetationDrag.stem_count_file, vegetation_drag_filter),
-    (models.VegetationDrag.stem_diameter_file, vegetation_drag_filter),
-    (models.VegetationDrag.drag_coefficient_file, vegetation_drag_filter),
+    (models.VegetationDrag.vegetation_height_file, vegetation_drag_filter),
+    (models.VegetationDrag.vegetation_stem_count_file, vegetation_drag_filter),
+    (models.VegetationDrag.vegetation_stem_diameter_file, vegetation_drag_filter),
+    (models.VegetationDrag.vegetation_drag_coefficient_file, vegetation_drag_filter),
 ]
 
 CHECKS += [
     GDALAvailableCheck(
         error_code=700, level=CheckLevel.WARNING, column=models.GlobalSetting.dem_file
     )
 ]
@@ -2071,36 +2105,36 @@
         filters=first_setting_filter,
     ),
     RasterGridSizeCheck(
         error_code=798,
         column=models.GlobalSetting.dem_file,
         filters=first_setting_filter,
     ),
-    ## 100xx: We continue raster checks from 10000
+    ## 100xx: We continue raster checks from 1400
     RasterRangeCheck(
-        error_code=10001,
-        column=models.VegetationDrag.height_file,
+        error_code=1401,
+        column=models.VegetationDrag.vegetation_height_file,
         filters=vegetation_drag_filter,
         min_value=0,
     ),
     RasterRangeCheck(
-        error_code=10002,
-        column=models.VegetationDrag.stem_count_file,
+        error_code=1402,
+        column=models.VegetationDrag.vegetation_stem_count_file,
         filters=vegetation_drag_filter,
         min_value=0,
     ),
     RasterRangeCheck(
-        error_code=10003,
-        column=models.VegetationDrag.stem_diameter_file,
+        error_code=1403,
+        column=models.VegetationDrag.vegetation_stem_diameter_file,
         filters=vegetation_drag_filter,
         min_value=0,
     ),
     RasterRangeCheck(
-        error_code=10004,
-        column=models.VegetationDrag.drag_coefficient_file,
+        error_code=1404,
+        column=models.VegetationDrag.vegetation_drag_coefficient_file,
         filters=vegetation_drag_filter,
         min_value=0,
     ),
 ]
 
 ## 080x: refinement levels
 CHECKS += [
@@ -2461,14 +2495,31 @@
         error_code=1226,
         column=control_table.target_id,
         reference_column=models.Pumpstation.id,
         filters=control_table.target_type == "v2_pumpstation",
     )
     for control_table in (models.ControlMemory, models.ControlTable)
 ]
+CHECKS += [
+    QueryCheck(
+        error_code=1227,
+        column=models.Control.id,
+        invalid=Query(models.Control).filter(
+            (
+                (models.Control.control_type == "memory")
+                & models.Control.control_id.not_in(Query(models.ControlMemory.id))
+            )
+            | (
+                (models.Control.control_type == "table")
+                & models.Control.control_id.not_in(Query(models.ControlTable.id))
+            )
+        ),
+        message="v2_control.control_id references an id in v2_control_memory or v2_control_table, but the table it references does not contain an entry with that id.",
+    )
+]
 
 # These checks are optional, depending on a command line argument
 beta_features_check = []
 beta_features_check += [
     BetaColumnsCheck(
         error_code=1300,
         column=col,
@@ -2531,14 +2582,23 @@
                 error_code=7,
                 custom_level_map={
                     "*.zoom_category": "INFO",
                     "v2_pipe.sewerage_type": "INFO",
                     "v2_pipe.material": "INFO",
                 },
             )
+            self.checks += [
+                RangeCheck(
+                    column=model.id,
+                    error_code=8,
+                    min_value=0,
+                    max_value=2147483647,
+                    message=f"{model.id.name} must be a positive signed 32-bit integer.",
+                )
+            ]
 
         self.checks += CHECKS
         if not self.allow_beta_features:
             self.checks += beta_features_check
 
     def iter_checks(self, level=CheckLevel.ERROR):
         """Iterate over checks with at least 'level'"""
```

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/exporters.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/raster_interface.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/raster_interface_gdal.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_gdal.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/interfaces/raster_interface_rasterio.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_rasterio.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/model_checks.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/scripts.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/conftest.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/factories.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,18 +342,18 @@
 
 class VegetationDragFactory(factory.alchemy.SQLAlchemyModelFactory):
     class Meta:
         model = models.VegetationDrag
         sqlalchemy_session = None
 
     display_name = Faker("name")
-    height = 1.0
-    height_file = "height_file.txt"
+    vegetation_height = 1.0
+    vegetation_height_file = "vegetation_height_file.txt"
 
-    stem_count = 50000
-    stem_count_file = "stem_count_file.txt"
+    vegetation_stem_count = 50000
+    vegetation_stem_count_file = "vegetation_stem_count_file.txt"
 
-    stem_diameter = 0.5
-    stem_diameter_file = "stem_diameter_file.txt"
+    vegetation_stem_diameter = 0.5
+    vegetation_stem_diameter_file = "vegetation_stem_diameter_file.txt"
 
-    drag_coefficient = 0.4
-    drag_coefficient_file = "drag_coefficient_file.txt"
+    vegetation_drag_coefficient = 0.4
+    vegetation_drag_coefficient_file = "vegetation_drag_coefficient_file.txt"
```

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_base.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_cross_section_definitions.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_factories.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_other.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_other.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 from threedi_modelchecker.checks.other import (
     BetaColumnsCheck,
     BetaValuesCheck,
     ChannelManholeLevelCheck,
     ConnectionNodesDistance,
     ConnectionNodesLength,
     CrossSectionLocationCheck,
+    CrossSectionSameConfigurationCheck,
+    ImperviousNodeInflowAreaCheck,
     LinestringLocationCheck,
     OpenChannelsWithNestedNewton,
+    PerviousNodeInflowAreaCheck,
     PotentialBreachInterdistanceCheck,
     PotentialBreachStartEndCheck,
     PumpStorageTimestepCheck,
     SpatialIndexCheck,
 )
 from threedi_modelchecker.model_checks import ThreediModelChecker
 
@@ -289,14 +292,101 @@
     factories.CrossSectionLocationFactory(
         channel=channel, the_geom="SRID=4326;POINT(5.387218 52.155244)"
     )
     errors = CrossSectionLocationCheck(0.1).get_invalid(session)
     assert len(errors) == 1
 
 
+@pytest.mark.parametrize(
+    "shape, width, height, same_channels, ok",
+    [
+        # --- closed cross-sections ---
+        # shapes 0, 2, 3 and 8 are always closed
+        (0, "3", "4", True, False),
+        *[(i, "3", None, True, False) for i in [2, 3, 8]],
+        # shapes 5 and 6 are closed if the width at the highest increment (last number in the width string) is 0
+        *[
+            (
+                i,
+                "0 4.142 5.143 5.143 5.869 0",
+                "0 0.174 0.348 0.522 0.696 0.87",
+                True,
+                False,
+            )
+            for i in [5, 6]
+        ],
+        # shape 7 is closed if the first and last (width, height) coordinates are the same
+        (7, "2 4.142 5.143 5.143 5.869 2", "3 0.174 0.348 0.522 0.696 3", True, False),
+        #
+        # --- open cross-sections ---
+        # shape 1 is always open
+        (1, "3", "4", True, True),
+        # shapes 5 and 6 are open if the width at the highest increment (last number in the width string) is > 0
+        *[
+            (
+                i,
+                "0 4.142 5.143 5.143 5.869 1",
+                "0 0.174 0.348 0.522 0.696 0.87",
+                True,
+                True,
+            )
+            for i in [5, 6]
+        ],
+        # shape 7 is open if the first and last (width, height) coordinates are not the same
+        # different width
+        (7, "2 4.142 5.143 5.143 5.869 3", "4 0.174 0.348 0.522 0.696 4", True, True),
+        # different height
+        (7, "2 4.142 5.143 5.143 5.869 2", "3 0.174 0.348 0.522 0.696 4", True, True),
+        # different height and width
+        (7, "2 4.142 5.143 5.143 5.869 3", "4 0.174 0.348 0.522 0.696 5", True, True),
+        #
+        # Bad data, should silently fail, returning no invalid rows. The data is checked in other checks.
+        (7, "foo", "bar", True, True),
+        #
+        # Check on different channels
+        # this should fail if the cross-sections are on the same channel, but pass on different channels
+        (0, "3", "4", False, True),
+    ],
+)
+def test_cross_section_same_configuration(
+    session, shape, width, height, same_channels, ok
+):
+    """
+    This test checks two cross-sections on a channel against each other; they should both be open or both be closed.
+    In this test, the first cross-section has been set to always be open.
+    Therefore, the channel should be invalid when the second cross-section is closed, and valid when it is open.
+    """
+    first_channel = factories.ChannelFactory(
+        the_geom="SRID=4326;LINESTRING(4.718301 52.696686, 4.718255 52.696709)",
+    )
+    second_channel = factories.ChannelFactory(
+        the_geom="SRID=4326;LINESTRING(4.718301 52.696686, 4.718255 52.696709)",
+    )
+    # shape 1 is always open
+    open_definition = factories.CrossSectionDefinitionFactory(
+        id=1, shape=1, width="3", height="4"
+    )
+    factories.CrossSectionLocationFactory(
+        channel=first_channel,
+        the_geom="SRID=4326;POINT(4.718278 52.696697)",
+        definition=open_definition,
+    )
+    testing_definition = factories.CrossSectionDefinitionFactory(
+        id=2, width=width, height=height, shape=shape
+    )
+    # the second one is parametrised
+    factories.CrossSectionLocationFactory(
+        channel=first_channel if same_channels else second_channel,
+        the_geom="SRID=4326;POINT(4.718265 52.696704)",
+        definition=testing_definition,
+    )
+    errors = CrossSectionSameConfigurationCheck(models.Channel.id).get_invalid(session)
+    assert len(errors) == (0 if ok else 1)
+
+
 def test_spatial_index_ok(session):
     check = SpatialIndexCheck(models.ConnectionNode.the_geom)
     invalid = check.get_invalid(session)
     assert len(invalid) == 0
 
 
 def test_spatial_index_disabled(empty_sqlite_v4):
@@ -399,14 +489,54 @@
     invalid = check.get_invalid(session)
     assert len(invalid) == expected_result
 
 
 @pytest.mark.parametrize(
     "value,expected_result",
     [
+        (1000, 0),  # total area = 1000 + 9000 = 10000 <= 10000; no error
+        (1001, 1),  # total area = 1001 + 9000 = 10001 > 10000; error
+    ],
+)
+def test_impervious_connection_node_inflow_area(session, value, expected_result):
+    connection_node = factories.ConnectionNodeFactory()
+    first_impervious_surface = factories.ImperviousSurfaceFactory(area=9000)
+    second_impervious_surface = factories.ImperviousSurfaceFactory(area=value)
+    factories.ImperviousSurfaceMapFactory(
+        impervious_surface=first_impervious_surface, connection_node=connection_node
+    )
+    factories.ImperviousSurfaceMapFactory(
+        impervious_surface=second_impervious_surface, connection_node=connection_node
+    )
+    check = ImperviousNodeInflowAreaCheck()
+    invalid = check.get_invalid(session)
+    assert len(invalid) == expected_result
+
+
+@pytest.mark.parametrize(
+    "value,expected_result",
+    [
+        (1000, 0),  # total area = 1000 + 9000 = 10000 <= 10000; no error
+        (1001, 1),  # total area = 1001 + 9000 = 10001 > 10000; error
+    ],
+)
+def test_pervious_connection_node_inflow_area(session, value, expected_result):
+    factories.ConnectionNodeFactory(id=1)
+    factories.SurfaceFactory(id=1, area=9000)
+    factories.SurfaceFactory(id=2, area=value)
+    factories.SurfaceMapFactory(surface_id=1, connection_node_id=1)
+    factories.SurfaceMapFactory(surface_id=2, connection_node_id=1)
+    check = PerviousNodeInflowAreaCheck()
+    invalid = check.get_invalid(session)
+    assert len(invalid) == expected_result
+
+
+@pytest.mark.parametrize(
+    "value,expected_result",
+    [
         (None, 0),  # column not set, valid result
         (5, 1),  # column set, invalid result
     ],
 )
 def test_beta_columns(session, value, expected_result):
     factories.GlobalSettingsFactory(vegetation_drag_settings_id=value)
     check = BetaColumnsCheck(models.GlobalSetting.vegetation_drag_settings_id)
```

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_raster.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_checks_timeseries.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_exporters.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker/tests/test_model_checks.py` & `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/PKG-INFO` & `threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.1.0
+Version: 2.1.1
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.1.0/threedi_modelchecker.egg-info/SOURCES.txt` & `threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


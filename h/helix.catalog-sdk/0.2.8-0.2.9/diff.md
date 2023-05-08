# Comparing `tmp/helix.catalog-sdk-0.2.8.tar.gz` & `tmp/helix.catalog-sdk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/helix.catalog-sdk-0.2.8.tar", last modified: Sun Jun 26 22:08:01 2022, max compression
+gzip compressed data, was "dist/helix.catalog-sdk-0.2.9.tar", last modified: Tue Jun 28 19:23:47 2022, max compression
```

## Comparing `helix.catalog-sdk-0.2.8.tar` & `helix.catalog-sdk-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-26 22:07:59.000000 helix.catalog-sdk-0.2.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-06-26 22:08:00.000000 helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-26 22:08:00.000000 helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-26 22:08:00.000000 helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-26 22:08:00.000000 helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/helix_catalog_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/helix_catalog_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16614 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/helix_catalog_sdk/catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)     7081 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/helix_catalog_sdk/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/helix_catalog_sdk/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/helix_catalog_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/helix_catalog_sdk/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-06-26 22:07:59.000000 helix.catalog-sdk-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:08:01.000000 helix.catalog-sdk-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17058 2022-06-26 22:06:55.000000 helix.catalog-sdk-0.2.8/tests/test_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-28 19:23:46.000000 helix.catalog-sdk-0.2.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16614 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7105 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-06-28 19:23:45.000000 helix.catalog-sdk-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17163 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/tests/test_catalog.py
```

### Comparing `helix.catalog-sdk-0.2.8/LICENSE` & `helix.catalog-sdk-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.8/Makefile` & `helix.catalog-sdk-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.8/PKG-INFO` & `helix.catalog-sdk-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.catalog-sdk
-Version: 0.2.8
+Version: 0.2.9
 Summary: SDK for interacting with the Helix Data and Connection Catalog
 Home-page: https://github.com/icanbwell/helix.catalog-sdk
 Author: Michael Vidal
 Author-email: michael.vidal@icanbwell.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/PKG-INFO` & `helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.catalog-sdk
-Version: 0.2.8
+Version: 0.2.9
 Summary: SDK for interacting with the Helix Data and Connection Catalog
 Home-page: https://github.com/icanbwell/helix.catalog-sdk
 Author: Michael Vidal
 Author-email: michael.vidal@icanbwell.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helix.catalog-sdk-0.2.8/helix.catalog_sdk.egg-info/SOURCES.txt` & `helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.8/helix_catalog_sdk/catalog.py` & `helix.catalog-sdk-0.2.9/helix_catalog_sdk/catalog.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.8/helix_catalog_sdk/data_source.py` & `helix.catalog-sdk-0.2.9/helix_catalog_sdk/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class ResourceItem:
     JSON_KEYS = (
         "name",
         "path",
         "path_slug",
+        "load_folders",
         "last_processed",
         "date_segment",
         "date_format",
     )
 
     def __init__(
         self,
```

### Comparing `helix.catalog-sdk-0.2.8/helix_catalog_sdk/repo.py` & `helix.catalog-sdk-0.2.9/helix_catalog_sdk/repo.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.8/setup.py` & `helix.catalog-sdk-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.8/tests/test_catalog.py` & `helix.catalog-sdk-0.2.9/tests/test_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,35 +158,38 @@
 
     # Load json from file for comparison as well, not just from in-memory object and confirm data properly updated
     json_file = "catalog/raw/gencon/icd.json"
     json_data = json.load(open(json_file))
     json_resources = json_data.get("resources")
     assert json_resources == [
         {
+            "load_folders": False,
             "last_processed": {
                 "dev": "s3://dev-ingestion/raw/gencon/icd/People/PeopleFeed_06092021.json",
                 "production": "s3://prod-ingestion/raw/gencon/icd/People/PeopleFeed_06092021.json",
                 "qa": "",
                 "staging": "s3://staging-ingestion/raw/gencon/icd/People/PeopleFeed_06092021.json",
             },
             "name": "people",
             "path": "People/PeopleFeed_06142021.json",
             "path_slug": "People/PeopleFeed_",
             "date_segment": None,
             "date_format": None,
         },
         {
+            "load_folders": False,
             "last_processed": None,
             "name": "places",
             "path": "Places/PlaceFeed_06172021.json",
             "path_slug": "Places/PlaceFeed_",
             "date_segment": None,
             "date_format": None,
         },
         {
+            "load_folders": False,
             "last_processed": None,
             "name": "things",
             "path": "Things/ThingFeed_06092021.json",
             "path_slug": "Things/ThingFeed_",
             "date_segment": None,
             "date_format": None,
         },
```


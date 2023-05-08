# Comparing `tmp/cognite_gql_pygen-0.4.2.tar.gz` & `tmp/cognite_gql_pygen-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.4.2.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.4.3.tar", max compression
```

## Comparing `cognite_gql_pygen-0.4.2.tar` & `cognite_gql_pygen-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11349 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/LICENSE
--rw-r--r--   0        0        0     4486 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/README.md
--rw-r--r--   0        0        0     8651 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      167 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19000 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3909 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2629 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      346 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6324 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     3863 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    19106 2023-05-08 11:14:17.503413 cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     5929 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7060 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0     1423 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0     1904 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/data_classes.py
--rw-r--r--   0        0        0     1560 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/generator.py
--rw-r--r--   0        0        0     7728 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0      596 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/misc.py
--rw-r--r--   0        0        0     1355 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/parser.py
--rw-r--r--   0        0        0     1333 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/templates/client.txt
--rw-r--r--   0        0        0      803 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     2024 2023-05-08 11:14:17.507413 cognite_gql_pygen-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5588 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4486 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/README.md
+-rw-r--r--   0        0        0     8651 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19000 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3909 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2629 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      346 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6324 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     3863 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    19106 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     5929 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7060 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0     1423 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:57:45.877008 cognite_gql_pygen-0.4.3/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1904 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1560 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     7728 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      596 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1355 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1333 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      803 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     2047 2023-05-08 12:57:45.881008 cognite_gql_pygen-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.4.3/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.4.2/LICENSE` & `cognite_gql_pygen-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/README.md` & `cognite_gql_pygen-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.4.3/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/gqlpygen/data_classes.py` & `cognite_gql_pygen-0.4.3/cognite/gqlpygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/gqlpygen/generator.py` & `cognite_gql_pygen-0.4.3/cognite/gqlpygen/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/gqlpygen/main.py` & `cognite_gql_pygen-0.4.3/cognite/gqlpygen/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/gqlpygen/misc.py` & `cognite_gql_pygen-0.4.3/cognite/gqlpygen/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/gqlpygen/parser.py` & `cognite_gql_pygen-0.4.3/cognite/gqlpygen/parser.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/gqlpygen/templates/client.txt` & `cognite_gql_pygen-0.4.3/cognite/gqlpygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/cognite/gqlpygen/templates/schema.txt` & `cognite_gql_pygen-0.4.3/cognite/gqlpygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.2/pyproject.toml` & `cognite_gql_pygen-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.4.2"
+version = "0.4.3"
 description = "Cognite graphQL Python generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
+license = "Apache-2.0"
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
 
 [tool.black]
 line-length = 120
 target_version = ['py39']
```

### Comparing `cognite_gql_pygen-0.4.2/PKG-INFO` & `cognite_gql_pygen-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.4.2
+Version: 0.4.3
 Summary: Cognite graphQL Python generation SDK
+License: Apache-2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: arrow (>=1.2.2,<2.0.0)
```


# Comparing `tmp/databricks-sdk-0.1.4.tar.gz` & `tmp/databricks-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-sdk-0.1.4.tar", last modified: Fri May  5 15:06:48 2023, max compression
+gzip compressed data, was "databricks-sdk-0.1.5.tar", last modified: Mon May  8 10:35:33 2023, max compression
```

## Comparing `databricks-sdk-0.1.4.tar` & `databricks-sdk-0.1.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28605 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.123141 databricks-sdk-0.1.4/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12817 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/dbconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/dbutils.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/mixins/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/mixins/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/runtime/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/_internal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30457 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/billing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   157480 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/catalog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   188918 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/compute.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14727 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68249 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/iam.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    99652 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113286 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/ml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19395 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/oauth2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51501 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/pipelines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    87514 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/provisioning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/serving.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33670 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44357 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/sharing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   140031 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/sql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43457 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/databricks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:33.774424 databricks-sdk-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-08 10:35:33.774424 databricks-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28605 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:33.770424 databricks-sdk-0.1.5/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:33.770424 databricks-sdk-0.1.5/databricks/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12817 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/dbconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:33.770424 databricks-sdk-0.1.5/databricks/sdk/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/mixins/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/mixins/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:33.770424 databricks-sdk-0.1.5/databricks/sdk/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/runtime/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:33.770424 databricks-sdk-0.1.5/databricks/sdk/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/_internal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30457 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/billing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   157480 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/catalog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   188918 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/compute.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14727 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68249 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/iam.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99652 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113286 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/ml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19395 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/oauth2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51501 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/pipelines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87514 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/provisioning.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/serving.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33670 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44357 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/sharing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   140031 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/sql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43457 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/service/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/databricks/sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:35:33.774424 databricks-sdk-0.1.5/databricks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-08 10:35:33.000000 databricks-sdk-0.1.5/databricks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-08 10:35:33.000000 databricks-sdk-0.1.5/databricks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:35:33.000000 databricks-sdk-0.1.5/databricks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-08 10:35:33.000000 databricks-sdk-0.1.5/databricks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 10:35:33.000000 databricks-sdk-0.1.5/databricks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-08 10:35:33.774424 databricks-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-08 10:35:21.000000 databricks-sdk-0.1.5/setup.py
```

### Comparing `databricks-sdk-0.1.4/LICENSE` & `databricks-sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/NOTICE` & `databricks-sdk-0.1.5/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/PKG-INFO` & `databricks-sdk-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Databricks SDK for Python (Experimental)
 Home-page: https://github.com/databricks/databricks-sdk-py
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
```

### Comparing `databricks-sdk-0.1.4/README.md` & `databricks-sdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/__init__.py` & `databricks-sdk-0.1.5/databricks/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/azure.py` & `databricks-sdk-0.1.5/databricks/sdk/azure.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/core.py` & `databricks-sdk-0.1.5/databricks/sdk/core.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/dbconnect.py` & `databricks-sdk-0.1.5/databricks/sdk/dbconnect.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/dbutils.py` & `databricks-sdk-0.1.5/databricks/sdk/dbutils.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/mixins/compute.py` & `databricks-sdk-0.1.5/databricks/sdk/mixins/compute.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/mixins/dbfs.py` & `databricks-sdk-0.1.5/databricks/sdk/mixins/dbfs.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/oauth.py` & `databricks-sdk-0.1.5/databricks/sdk/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/runtime/__init__.py` & `databricks-sdk-0.1.5/databricks/sdk/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/runtime/stub.py` & `databricks-sdk-0.1.5/databricks/sdk/runtime/stub.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/_internal.py` & `databricks-sdk-0.1.5/databricks/sdk/service/_internal.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/billing.py` & `databricks-sdk-0.1.5/databricks/sdk/service/billing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/catalog.py` & `databricks-sdk-0.1.5/databricks/sdk/service/catalog.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/compute.py` & `databricks-sdk-0.1.5/databricks/sdk/service/compute.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/files.py` & `databricks-sdk-0.1.5/databricks/sdk/service/files.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/iam.py` & `databricks-sdk-0.1.5/databricks/sdk/service/iam.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/jobs.py` & `databricks-sdk-0.1.5/databricks/sdk/service/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/ml.py` & `databricks-sdk-0.1.5/databricks/sdk/service/ml.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/oauth2.py` & `databricks-sdk-0.1.5/databricks/sdk/service/oauth2.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/pipelines.py` & `databricks-sdk-0.1.5/databricks/sdk/service/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/provisioning.py` & `databricks-sdk-0.1.5/databricks/sdk/service/provisioning.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/serving.py` & `databricks-sdk-0.1.5/databricks/sdk/service/serving.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/settings.py` & `databricks-sdk-0.1.5/databricks/sdk/service/settings.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/sharing.py` & `databricks-sdk-0.1.5/databricks/sdk/service/sharing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/sql.py` & `databricks-sdk-0.1.5/databricks/sdk/service/sql.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks/sdk/service/workspace.py` & `databricks-sdk-0.1.5/databricks/sdk/service/workspace.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/databricks_sdk.egg-info/PKG-INFO` & `databricks-sdk-0.1.5/databricks_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Databricks SDK for Python (Experimental)
 Home-page: https://github.com/databricks/databricks-sdk-py
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
```

### Comparing `databricks-sdk-0.1.4/databricks_sdk.egg-info/SOURCES.txt` & `databricks-sdk-0.1.5/databricks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/setup.cfg` & `databricks-sdk-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.4/setup.py` & `databricks-sdk-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with version_file.open('r') as f:
     exec(f.read(), version_data)
 
 setup(name="databricks-sdk",
       version=version_data['__version__'],
       packages=find_packages(exclude=["tests", "*tests.*", "*tests"]),
       python_requires=">=3.7",
-      install_requires=["requests>=2.28.1"],
+      install_requires=["requests>=2.28.1,<2.29.0"],
       extras_require={"dev": ["pytest", "pytest-cov", "pytest-xdist", "pytest-mock",
                               "yapf", "pycodestyle", "autoflake", "isort", "wheel"]},
       author="Serge Smertin",
       author_email="serge.smertin@databricks.com",
       description="Databricks SDK for Python (Experimental)",
       long_description=io.open("README.md", encoding="utf-8").read(),
       long_description_content_type='text/markdown',
```


# Comparing `tmp/yetl-framework-1.2.8.tar.gz` & `tmp/yetl-framework-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.2.8.tar", last modified: Mon May  8 14:27:58 2023, max compression
+gzip compressed data, was "yetl-framework-1.2.9.tar", last modified: Mon May  8 14:49:47 2023, max compression
```

## Comparing `yetl-framework-1.2.8.tar` & `yetl-framework-1.2.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7544 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3195 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5180 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4683 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.861594 yetl-framework-1.2.9/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7544 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/yetl/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3249 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5180 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.2.8/PKG-INFO` & `yetl-framework-1.2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.8
+Version: 1.2.9
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -26,25 +26,37 @@
 
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
+audit_control:
+  delta_lake:
+    raw_dbx_patterns_control:
+      header_footer:
+        sql: ../sql/{{database}}/{{table}}.sql
+        depends_on:
+          - raw.raw_dbx_patterns.*
+      raw_audit:
+        sql: ../sql/{{database}}/{{table}}.sql
+        depends_on:
+          - raw.raw_dbx_patterns.*
+          - audit_control.raw_dbx_patterns_control.header_footer
 
-landing: # this is the landing stage in the deltalake house
-  read: # this is the type of spark asset that the pipeline needs to read
+landing:
+  read:
     landing_dbx_patterns:
       customer_details_1: null
       customer_details_2: null
 
-raw: # this is the bronze stage in the deltalake house
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
-    raw_dbx_patterns: # this is the database name
-      customers: # this is a table name and it's subsequent properties
+raw:
+  delta_lake:
+    raw_dbx_patterns:
+      customers:
         ids: id
         depends_on:
           - landing.landing_dbx_patterns.customer_details_1
           - landing.landing_dbx_patterns.customer_details_2
         warning_thresholds:
           invalid_ratio: 0.1
           invalid_rows: 0
@@ -53,46 +65,40 @@
         exception_thresholds:
           invalid_ratio: 0.2
           invalid_rows: 2
           max_rows: 1000
           min_rows: 0
         custom_properties:
           process_group: 1
-
-base: # this is the silver stage in the delta lakehouse
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
-    # delta table properties can be set at stage level or table level
-    delta_properties:
-      delta.appendOnly: true
-      delta.autoOptimize.autoCompact: true    
-      delta.autoOptimize.optimizeWrite: true  
-      delta.enableChangeDataFeed: false
-    base_dbx_patterns: # this is a database name
-      customer_details_1: # this is a table name and it's subsequent properties
-        ids: id
-        depends_on:
-          - raw.raw_dbx_patterns.customers
-        # delta table properties can be set at stage level or table level
-        # table level properties will overwride stage level properties
-        delta_properties:
-            delta.enableChangeDataFeed: true
-      customer_details_2: # this is a table name and it's subsequent properties
-        ids: id
-        depends_on:
-          - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
-version: 1.1.0
+version: 1.0.0
 tables: ./tables.yaml
 
-landing: # this is the landing stage in the deltalake house
-  read: # this is the type of spark asset that the pipeline needs to read from
+audit_control:
+  delta_lake:
+    # delta table properties can be set at stage level or table level
+    delta_properties:
+        delta.appendOnly: true
+        delta.autoOptimize.autoCompact: true
+        delta.autoOptimize.optimizeWrite: true
+    managed: false
+    create_table: true
+    container: datalake
+    location: /mnt/{{container}}/data/raw
+    checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
+    path: "{{database}}/{{table}}"
+    options:
+      checkpointLocation: default
+
+landing:
+  read:
     trigger: customerdetailscomplete-{{filename_date_format}}*.flg
     trigger_type: file
     container: datalake
     location: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
     filename: "{{table}}-{{filename_date_format}}*.csv"
     filename_date_format: "%Y%m%d"
     path_date_format: "%Y%m%d"
@@ -113,31 +119,37 @@
       encoding: windows-1252
       delimiter: ","
       escape: '"'
       nullValue: ""
       quote: '"'
       emptyValue: ""
     
-
-raw: # this is the bronze stage in the deltalake house
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
+raw:
+  delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
     create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
+    checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     options:
-      checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
+
+base:
+  delta_lake:
+    container: datalake
+    location: /mnt/{{container}}/data/base
+    path: "{{database}}/{{table}}"
+    options: null
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from yetl import Config, StageType
```

### Comparing `yetl-framework-1.2.8/README.md` & `yetl-framework-1.2.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,25 +11,37 @@
 
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
+audit_control:
+  delta_lake:
+    raw_dbx_patterns_control:
+      header_footer:
+        sql: ../sql/{{database}}/{{table}}.sql
+        depends_on:
+          - raw.raw_dbx_patterns.*
+      raw_audit:
+        sql: ../sql/{{database}}/{{table}}.sql
+        depends_on:
+          - raw.raw_dbx_patterns.*
+          - audit_control.raw_dbx_patterns_control.header_footer
 
-landing: # this is the landing stage in the deltalake house
-  read: # this is the type of spark asset that the pipeline needs to read
+landing:
+  read:
     landing_dbx_patterns:
       customer_details_1: null
       customer_details_2: null
 
-raw: # this is the bronze stage in the deltalake house
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
-    raw_dbx_patterns: # this is the database name
-      customers: # this is a table name and it's subsequent properties
+raw:
+  delta_lake:
+    raw_dbx_patterns:
+      customers:
         ids: id
         depends_on:
           - landing.landing_dbx_patterns.customer_details_1
           - landing.landing_dbx_patterns.customer_details_2
         warning_thresholds:
           invalid_ratio: 0.1
           invalid_rows: 0
@@ -38,46 +50,40 @@
         exception_thresholds:
           invalid_ratio: 0.2
           invalid_rows: 2
           max_rows: 1000
           min_rows: 0
         custom_properties:
           process_group: 1
-
-base: # this is the silver stage in the delta lakehouse
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
-    # delta table properties can be set at stage level or table level
-    delta_properties:
-      delta.appendOnly: true
-      delta.autoOptimize.autoCompact: true    
-      delta.autoOptimize.optimizeWrite: true  
-      delta.enableChangeDataFeed: false
-    base_dbx_patterns: # this is a database name
-      customer_details_1: # this is a table name and it's subsequent properties
-        ids: id
-        depends_on:
-          - raw.raw_dbx_patterns.customers
-        # delta table properties can be set at stage level or table level
-        # table level properties will overwride stage level properties
-        delta_properties:
-            delta.enableChangeDataFeed: true
-      customer_details_2: # this is a table name and it's subsequent properties
-        ids: id
-        depends_on:
-          - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
-version: 1.1.0
+version: 1.0.0
 tables: ./tables.yaml
 
-landing: # this is the landing stage in the deltalake house
-  read: # this is the type of spark asset that the pipeline needs to read from
+audit_control:
+  delta_lake:
+    # delta table properties can be set at stage level or table level
+    delta_properties:
+        delta.appendOnly: true
+        delta.autoOptimize.autoCompact: true
+        delta.autoOptimize.optimizeWrite: true
+    managed: false
+    create_table: true
+    container: datalake
+    location: /mnt/{{container}}/data/raw
+    checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
+    path: "{{database}}/{{table}}"
+    options:
+      checkpointLocation: default
+
+landing:
+  read:
     trigger: customerdetailscomplete-{{filename_date_format}}*.flg
     trigger_type: file
     container: datalake
     location: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
     filename: "{{table}}-{{filename_date_format}}*.csv"
     filename_date_format: "%Y%m%d"
     path_date_format: "%Y%m%d"
@@ -98,31 +104,37 @@
       encoding: windows-1252
       delimiter: ","
       escape: '"'
       nullValue: ""
       quote: '"'
       emptyValue: ""
     
-
-raw: # this is the bronze stage in the deltalake house
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
+raw:
+  delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
     create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
+    checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     options:
-      checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
+
+base:
+  delta_lake:
+    container: datalake
+    location: /mnt/{{container}}/data/base
+    path: "{{database}}/{{table}}"
+    options: null
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from yetl import Config, StageType
```

### Comparing `yetl-framework-1.2.8/setup.py` & `yetl-framework-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.2.8",
+    version="1.2.9",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.2.8/yetl/__init__.py` & `yetl-framework-1.2.9/yetl/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_config.py` & `yetl-framework-1.2.9/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_decorators.py` & `yetl-framework-1.2.9/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_logging_config.py` & `yetl-framework-1.2.9/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_project.py` & `yetl-framework-1.2.9/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_spark_context.py` & `yetl-framework-1.2.9/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_tables.py` & `yetl-framework-1.2.9/yetl/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_timeslice.py` & `yetl-framework-1.2.9/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/_utils.py` & `yetl-framework-1.2.9/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/deltalake.py` & `yetl-framework-1.2.9/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/table/_deltalake.py` & `yetl-framework-1.2.9/yetl/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/table/_factory.py` & `yetl-framework-1.2.9/yetl/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/table/_read.py` & `yetl-framework-1.2.9/yetl/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl/table/_table.py` & `yetl-framework-1.2.9/yetl/table/_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 
     @classmethod
     def default_select_sql(cls):
         sql = "null"
         return sql
 
     def select_sql(self):
-        warning_thresholds_sql = []
+        thresholds_sql = []
         if self.invalid_ratio:
-            warning_thresholds_sql.append(f"{self.invalid_ratio} as invalid_ratio")
+            thresholds_sql.append(f"{self.invalid_ratio} as invalid_ratio")
         else:
-            self.append("null as invalid_ratio")
+            thresholds_sql.append("null as invalid_ratio")
 
         if self.invalid_rows:
-            self.append(f"{self.invalid_rows} as invalid_rows")
+            thresholds_sql.append(f"{self.invalid_rows} as invalid_rows")
         else:
-            self.append("null as invalid_rows")
+            thresholds_sql.append("null as invalid_rows")
 
         if self.max_rows:
-            self.append(f"{self.max_rows} as max_rows")
+            thresholds_sql.append(f"{self.max_rows} as max_rows")
         else:
-            self.append("null as max_rows")
+            thresholds_sql.append("null as max_rows")
 
         if self.min_rows:
-            self.append(f"{self.min_rows} as min_rows")
+            thresholds_sql.append(f"{self.min_rows} as min_rows")
         else:
-            self.append("null as min_rows")
+            thresholds_sql.append("null as min_rows")
 
         sql = """
             struct(
                 ",".join(warning_thresholds_sql)
             )
         """
```

### Comparing `yetl-framework-1.2.8/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.2.9/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.8/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.2.9/yetl_framework.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.8
+Version: 1.2.9
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -26,25 +26,37 @@
 
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
+audit_control:
+  delta_lake:
+    raw_dbx_patterns_control:
+      header_footer:
+        sql: ../sql/{{database}}/{{table}}.sql
+        depends_on:
+          - raw.raw_dbx_patterns.*
+      raw_audit:
+        sql: ../sql/{{database}}/{{table}}.sql
+        depends_on:
+          - raw.raw_dbx_patterns.*
+          - audit_control.raw_dbx_patterns_control.header_footer
 
-landing: # this is the landing stage in the deltalake house
-  read: # this is the type of spark asset that the pipeline needs to read
+landing:
+  read:
     landing_dbx_patterns:
       customer_details_1: null
       customer_details_2: null
 
-raw: # this is the bronze stage in the deltalake house
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
-    raw_dbx_patterns: # this is the database name
-      customers: # this is a table name and it's subsequent properties
+raw:
+  delta_lake:
+    raw_dbx_patterns:
+      customers:
         ids: id
         depends_on:
           - landing.landing_dbx_patterns.customer_details_1
           - landing.landing_dbx_patterns.customer_details_2
         warning_thresholds:
           invalid_ratio: 0.1
           invalid_rows: 0
@@ -53,46 +65,40 @@
         exception_thresholds:
           invalid_ratio: 0.2
           invalid_rows: 2
           max_rows: 1000
           min_rows: 0
         custom_properties:
           process_group: 1
-
-base: # this is the silver stage in the delta lakehouse
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
-    # delta table properties can be set at stage level or table level
-    delta_properties:
-      delta.appendOnly: true
-      delta.autoOptimize.autoCompact: true    
-      delta.autoOptimize.optimizeWrite: true  
-      delta.enableChangeDataFeed: false
-    base_dbx_patterns: # this is a database name
-      customer_details_1: # this is a table name and it's subsequent properties
-        ids: id
-        depends_on:
-          - raw.raw_dbx_patterns.customers
-        # delta table properties can be set at stage level or table level
-        # table level properties will overwride stage level properties
-        delta_properties:
-            delta.enableChangeDataFeed: true
-      customer_details_2: # this is a table name and it's subsequent properties
-        ids: id
-        depends_on:
-          - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
-version: 1.1.0
+version: 1.0.0
 tables: ./tables.yaml
 
-landing: # this is the landing stage in the deltalake house
-  read: # this is the type of spark asset that the pipeline needs to read from
+audit_control:
+  delta_lake:
+    # delta table properties can be set at stage level or table level
+    delta_properties:
+        delta.appendOnly: true
+        delta.autoOptimize.autoCompact: true
+        delta.autoOptimize.optimizeWrite: true
+    managed: false
+    create_table: true
+    container: datalake
+    location: /mnt/{{container}}/data/raw
+    checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
+    path: "{{database}}/{{table}}"
+    options:
+      checkpointLocation: default
+
+landing:
+  read:
     trigger: customerdetailscomplete-{{filename_date_format}}*.flg
     trigger_type: file
     container: datalake
     location: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
     filename: "{{table}}-{{filename_date_format}}*.csv"
     filename_date_format: "%Y%m%d"
     path_date_format: "%Y%m%d"
@@ -113,31 +119,37 @@
       encoding: windows-1252
       delimiter: ","
       escape: '"'
       nullValue: ""
       quote: '"'
       emptyValue: ""
     
-
-raw: # this is the bronze stage in the deltalake house
-  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
+raw:
+  delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
     create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
+    checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     options:
-      checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
+
+base:
+  delta_lake:
+    container: datalake
+    location: /mnt/{{container}}/data/base
+    path: "{{database}}/{{table}}"
+    options: null
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from yetl import Config, StageType
```

### Comparing `yetl-framework-1.2.8/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.2.9/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*


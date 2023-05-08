# Comparing `tmp/yetl-framework-1.2.9.tar.gz` & `tmp/yetl-framework-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.2.9.tar", last modified: Mon May  8 14:49:47 2023, max compression
+gzip compressed data, was "yetl-framework-1.3.0.tar", last modified: Mon May  8 15:20:31 2023, max compression
```

## Comparing `yetl-framework-1.2.9.tar` & `yetl-framework-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/
--rw-r--r--   0 vsts      (1001) docker     (123)     5180 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4683 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.861594 yetl-framework-1.2.9/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7544 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/yetl/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3249 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-08 14:48:52.000000 yetl-framework-1.2.9/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:49:47.865594 yetl-framework-1.2.9/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5180 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-08 14:49:47.000000 yetl-framework-1.2.9/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 15:20:31.162970 yetl-framework-1.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-08 15:20:31.162970 yetl-framework-1.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4699 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-08 15:20:31.162970 yetl-framework-1.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 15:20:31.158969 yetl-framework-1.3.0/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7544 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 15:20:31.158969 yetl-framework-1.3.0/yetl/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3380 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 15:20:31.162970 yetl-framework-1.3.0/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-08 15:19:41.000000 yetl-framework-1.3.0/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 15:20:31.162970 yetl-framework-1.3.0/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-08 15:20:31.000000 yetl-framework-1.3.0/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-08 15:20:31.000000 yetl-framework-1.3.0/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 15:20:31.000000 yetl-framework-1.3.0/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 15:20:31.000000 yetl-framework-1.3.0/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-08 15:20:31.000000 yetl-framework-1.3.0/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-08 15:20:31.000000 yetl-framework-1.3.0/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.2.9/PKG-INFO` & `yetl-framework-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.9
+Version: 1.3.0
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -26,14 +26,16 @@
 
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
+version: 1.3.0
+
 audit_control:
   delta_lake:
     raw_dbx_patterns_control:
       header_footer:
         sql: ../sql/{{database}}/{{table}}.sql
         depends_on:
           - raw.raw_dbx_patterns.*
@@ -70,15 +72,15 @@
         custom_properties:
           process_group: 1
 ```
 
 Define you load configuration:
 
 ```yaml
-version: 1.0.0
+version: 1.3.0
 tables: ./tables.yaml
 
 audit_control:
   delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
         delta.appendOnly: true
```

### Comparing `yetl-framework-1.2.9/README.md` & `yetl-framework-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
+version: 1.3.0
+
 audit_control:
   delta_lake:
     raw_dbx_patterns_control:
       header_footer:
         sql: ../sql/{{database}}/{{table}}.sql
         depends_on:
           - raw.raw_dbx_patterns.*
@@ -55,15 +57,15 @@
         custom_properties:
           process_group: 1
 ```
 
 Define you load configuration:
 
 ```yaml
-version: 1.0.0
+version: 1.3.0
 tables: ./tables.yaml
 
 audit_control:
   delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
         delta.appendOnly: true
```

### Comparing `yetl-framework-1.2.9/setup.py` & `yetl-framework-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.2.9",
+    version="1.3.0",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.2.9/yetl/__init__.py` & `yetl-framework-1.3.0/yetl/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_config.py` & `yetl-framework-1.3.0/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_decorators.py` & `yetl-framework-1.3.0/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_logging_config.py` & `yetl-framework-1.3.0/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_project.py` & `yetl-framework-1.3.0/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_spark_context.py` & `yetl-framework-1.3.0/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_tables.py` & `yetl-framework-1.3.0/yetl/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_timeslice.py` & `yetl-framework-1.3.0/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/_utils.py` & `yetl-framework-1.3.0/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/deltalake.py` & `yetl-framework-1.3.0/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/table/_deltalake.py` & `yetl-framework-1.3.0/yetl/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/table/_factory.py` & `yetl-framework-1.3.0/yetl/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/table/_read.py` & `yetl-framework-1.3.0/yetl/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl/table/_table.py` & `yetl-framework-1.3.0/yetl/table/_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,37 +26,39 @@
     @classmethod
     def default_select_sql(cls):
         sql = "null"
         return sql
 
     def select_sql(self):
         thresholds_sql = []
-        if self.invalid_ratio:
-            thresholds_sql.append(f"{self.invalid_ratio} as invalid_ratio")
+        if self.invalid_ratio is not None:
+            thresholds_sql.append(
+                f"cast({self.invalid_ratio} as double) as invalid_ratio"
+            )
         else:
             thresholds_sql.append("null as invalid_ratio")
 
-        if self.invalid_rows:
-            thresholds_sql.append(f"{self.invalid_rows} as invalid_rows")
+        if self.invalid_rows is not None:
+            thresholds_sql.append(f"cast({self.invalid_rows} as long) as invalid_rows")
         else:
             thresholds_sql.append("null as invalid_rows")
 
-        if self.max_rows:
-            thresholds_sql.append(f"{self.max_rows} as max_rows")
+        if self.max_rows is not None:
+            thresholds_sql.append(f"cast({self.max_rows} as long) as max_rows")
         else:
             thresholds_sql.append("null as max_rows")
 
-        if self.min_rows:
-            thresholds_sql.append(f"{self.min_rows} as min_rows")
+        if self.min_rows is not None:
+            thresholds_sql.append(f"cast({self.min_rows} as long) as min_rows")
         else:
             thresholds_sql.append("null as min_rows")
 
-        sql = """
+        sql = f"""
             struct(
-                ",".join(warning_thresholds_sql)
+                {",".join(thresholds_sql)}
             )
         """
 
         return sql
 
 
 class Table(BaseModel):
```

### Comparing `yetl-framework-1.2.9/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.3.0/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.9/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.3.0/yetl_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.9
+Version: 1.3.0
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -26,14 +26,16 @@
 
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
+version: 1.3.0
+
 audit_control:
   delta_lake:
     raw_dbx_patterns_control:
       header_footer:
         sql: ../sql/{{database}}/{{table}}.sql
         depends_on:
           - raw.raw_dbx_patterns.*
@@ -70,15 +72,15 @@
         custom_properties:
           process_group: 1
 ```
 
 Define you load configuration:
 
 ```yaml
-version: 1.0.0
+version: 1.3.0
 tables: ./tables.yaml
 
 audit_control:
   delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
         delta.appendOnly: true
```

### Comparing `yetl-framework-1.2.9/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.3.0/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*


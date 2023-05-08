# Comparing `tmp/yetl-framework-1.2.4.tar.gz` & `tmp/yetl-framework-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.2.4.tar", last modified: Sat May  6 23:00:28 2023, max compression
+gzip compressed data, was "yetl-framework-1.2.5.tar", last modified: Mon May  8 12:28:12 2023, max compression
```

## Comparing `yetl-framework-1.2.4.tar` & `yetl-framework-1.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 23:00:28.809832 yetl-framework-1.2.4/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 23:00:28.809832 yetl-framework-1.2.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 23:00:28.809832 yetl-framework-1.2.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 23:00:28.805832 yetl-framework-1.2.4/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      502 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7493 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 23:00:28.805832 yetl-framework-1.2.4/yetl/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1600 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 23:00:28.805832 yetl-framework-1.2.4/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 22:59:29.000000 yetl-framework-1.2.4/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 23:00:28.809832 yetl-framework-1.2.4/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 23:00:28.000000 yetl-framework-1.2.4/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-06 23:00:28.000000 yetl-framework-1.2.4/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 23:00:28.000000 yetl-framework-1.2.4/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 23:00:28.000000 yetl-framework-1.2.4/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 23:00:28.000000 yetl-framework-1.2.4/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 23:00:28.000000 yetl-framework-1.2.4/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 12:28:12.434702 yetl-framework-1.2.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 12:28:12.434702 yetl-framework-1.2.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-08 12:28:12.434702 yetl-framework-1.2.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 12:28:12.430702 yetl-framework-1.2.5/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7544 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 12:28:12.434702 yetl-framework-1.2.5/yetl/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3377 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 12:28:12.434702 yetl-framework-1.2.5/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-08 12:27:21.000000 yetl-framework-1.2.5/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 12:28:12.434702 yetl-framework-1.2.5/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 12:28:12.000000 yetl-framework-1.2.5/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-08 12:28:12.000000 yetl-framework-1.2.5/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 12:28:12.000000 yetl-framework-1.2.5/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 12:28:12.000000 yetl-framework-1.2.5/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-08 12:28:12.000000 yetl-framework-1.2.5/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-08 12:28:12.000000 yetl-framework-1.2.5/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.2.4/PKG-INFO` & `yetl-framework-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.4
+Version: 1.2.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.2.4/README.md` & `yetl-framework-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/setup.py` & `yetl-framework-1.2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.2.4",
+    version="1.2.5",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.2.4/yetl/_config.py` & `yetl-framework-1.2.5/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/_decorators.py` & `yetl-framework-1.2.5/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/_logging_config.py` & `yetl-framework-1.2.5/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/_project.py` & `yetl-framework-1.2.5/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/_spark_context.py` & `yetl-framework-1.2.5/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/_tables.py` & `yetl-framework-1.2.5/yetl/_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,24 +177,27 @@
         self, stage: StageType, table=_INDEX_WILDCARD, database=_INDEX_WILDCARD
     ):
         destination = self.lookup_table(
             stage=stage, database=database, table=table, first_match=True
         )
         source = {}
 
+        tables = []
         try:
             for index in destination.depends_on:
                 do_stage, do_database, do_table = Tables.parse_index(index)
-                table = self.lookup_table(
+                tables = tables + self.lookup_table(
                     stage=do_stage,
                     table=do_table,
                     database=do_database,
-                    first_match=True,
+                    first_match=False,
                 )
-                source[table.table] = table
         except Exception as e:
             raise Exception(f"Error looking up dependencies for table {table}") from e
 
+        for tbl in tables:
+            source[tbl.table] = tbl
+
         if len(list(source.values())) == 1:
             source = list(source.values())[0]
 
         return TableMapping(source=source, destination=destination)
```

### Comparing `yetl-framework-1.2.4/yetl/_timeslice.py` & `yetl-framework-1.2.5/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/_utils.py` & `yetl-framework-1.2.5/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/deltalake.py` & `yetl-framework-1.2.5/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/table/_deltalake.py` & `yetl-framework-1.2.5/yetl/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/table/_factory.py` & `yetl-framework-1.2.5/yetl/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/table/_read.py` & `yetl-framework-1.2.5/yetl/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.2.5/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.4/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.2.5/yetl_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.4
+Version: 1.2.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.2.4/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.2.5/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*


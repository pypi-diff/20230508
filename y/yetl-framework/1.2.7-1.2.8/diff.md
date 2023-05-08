# Comparing `tmp/yetl-framework-1.2.7.tar.gz` & `tmp/yetl-framework-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.2.7.tar", last modified: Mon May  8 14:11:47 2023, max compression
+gzip compressed data, was "yetl-framework-1.2.8.tar", last modified: Mon May  8 14:27:58 2023, max compression
```

## Comparing `yetl-framework-1.2.7.tar` & `yetl-framework-1.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:11:47.535517 yetl-framework-1.2.7/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 14:11:47.535517 yetl-framework-1.2.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-08 14:11:47.535517 yetl-framework-1.2.7/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:11:47.531517 yetl-framework-1.2.7/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7544 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:11:47.535517 yetl-framework-1.2.7/yetl/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3382 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:11:47.535517 yetl-framework-1.2.7/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-08 14:10:58.000000 yetl-framework-1.2.7/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:11:47.535517 yetl-framework-1.2.7/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 14:11:47.000000 yetl-framework-1.2.7/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-08 14:11:47.000000 yetl-framework-1.2.7/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:11:47.000000 yetl-framework-1.2.7/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:11:47.000000 yetl-framework-1.2.7/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-08 14:11:47.000000 yetl-framework-1.2.7/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-08 14:11:47.000000 yetl-framework-1.2.7/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7544 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4580 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5142 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3195 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-08 14:27:05.000000 yetl-framework-1.2.8/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-08 14:27:58.795530 yetl-framework-1.2.8/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-08 14:27:58.000000 yetl-framework-1.2.8/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.2.7/PKG-INFO` & `yetl-framework-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.7
+Version: 1.2.8
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.2.7/README.md` & `yetl-framework-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/setup.py` & `yetl-framework-1.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.2.7",
+    version="1.2.8",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.2.7/yetl/__init__.py` & `yetl-framework-1.2.8/yetl/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_config.py` & `yetl-framework-1.2.8/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_decorators.py` & `yetl-framework-1.2.8/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_logging_config.py` & `yetl-framework-1.2.8/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_project.py` & `yetl-framework-1.2.8/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_spark_context.py` & `yetl-framework-1.2.8/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_tables.py` & `yetl-framework-1.2.8/yetl/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_timeslice.py` & `yetl-framework-1.2.8/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/_utils.py` & `yetl-framework-1.2.8/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/deltalake.py` & `yetl-framework-1.2.8/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/table/_deltalake.py` & `yetl-framework-1.2.8/yetl/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/table/_factory.py` & `yetl-framework-1.2.8/yetl/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/table/_read.py` & `yetl-framework-1.2.8/yetl/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl/table/_table.py` & `yetl-framework-1.2.8/yetl/table/_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,15 @@
     invalid_ratio: float = Field(default=None)
     invalid_rows: int = Field(default=None)
     max_rows: int = Field(default=None)
     min_rows: int = Field(default=None)
 
     @classmethod
     def default_select_sql(cls):
-        sql = """
-            struct(
-                null as invalid_ratio,
-                null as invalid_rows,
-                null as max_rows,
-                null as min_rows
-            )
-        """
+        sql = "null"
         return sql
 
     def select_sql(self):
         warning_thresholds_sql = []
         if self.invalid_ratio:
             warning_thresholds_sql.append(f"{self.invalid_ratio} as invalid_ratio")
         else:
```

### Comparing `yetl-framework-1.2.7/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.2.8/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.7/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.2.8/yetl_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.7
+Version: 1.2.8
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.2.7/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.2.8/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*


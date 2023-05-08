# Comparing `tmp/AI Dashboard-0.2.8.tar.gz` & `tmp/AI Dashboard-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AI Dashboard-0.2.8.tar", last modified: Wed Jan  4 23:33:34 2023, max compression
+gzip compressed data, was "AI Dashboard-0.2.9.tar", last modified: Thu Jan  5 05:15:16 2023, max compression
```

## Comparing `AI Dashboard-0.2.8.tar` & `AI Dashboard-0.2.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.718481 AI Dashboard-0.2.8/AI_Dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-04 23:33:34.000000 AI Dashboard-0.2.8/AI_Dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-01-04 23:33:34.000000 AI Dashboard-0.2.8/AI_Dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 23:33:34.000000 AI Dashboard-0.2.8/AI_Dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-04 23:33:34.000000 AI Dashboard-0.2.8/AI_Dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-04 23:33:34.000000 AI Dashboard-0.2.8/AI_Dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/abstract_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/tabs/category_view/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/category_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/category_view/category_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/tabs/chart_view/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/chart_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/chart_view/chart_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/aggregation_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/data_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/ai_dashboard/tabs/document_view/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/document_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/tabs/document_view/document_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/ai_dashboard/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:34.722481 AI Dashboard-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-04 23:33:18.000000 AI Dashboard-0.2.8/tests/test_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.594242 AI Dashboard-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/AI_Dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-05 05:15:16.000000 AI Dashboard-0.2.9/AI_Dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-01-05 05:15:16.000000 AI Dashboard-0.2.9/AI_Dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 05:15:16.000000 AI Dashboard-0.2.9/AI_Dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-05 05:15:16.000000 AI Dashboard-0.2.9/AI_Dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-05 05:15:16.000000 AI Dashboard-0.2.9/AI_Dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-05 05:15:16.594242 AI Dashboard-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/abstract_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/tabs/category_view/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/category_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/category_view/category_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/tabs/chart_view/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/chart_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/chart_view/chart_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/aggregation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/data_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/ai_dashboard/tabs/document_view/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/document_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/tabs/document_view/document_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/ai_dashboard/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 05:15:16.594242 AI Dashboard-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:16.590242 AI Dashboard-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-01-05 05:15:00.000000 AI Dashboard-0.2.9/tests/test_script.py
```

### Comparing `AI Dashboard-0.2.8/AI_Dashboard.egg-info/SOURCES.txt` & `AI Dashboard-0.2.9/AI_Dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/LICENSE` & `AI Dashboard-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/README.md` & `AI Dashboard-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/api/client.py` & `AI Dashboard-0.2.9/ai_dashboard/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         dataset_id = configuration.get("dataset_id")
         deployable_id = configuration.get("deployable_id")
         project_id = configuration.get("project_id")
         return dashboard.Dashboard(
             endpoints=self._endpoints,
             dataset_id=dataset_id,
             deployable_id=deployable_id,
-            configuration=configuration,
+            configuration=configuration["configuration"],
             project_id=project_id,
         )
 
     def list_deployables(self, page_size: int = 1000):
         return self._endpoints._list_deployables(page_size=page_size)
 
     def create_deployable(
```

### Comparing `AI Dashboard-0.2.8/ai_dashboard/dashboard/dashboard.py` & `AI Dashboard-0.2.9/ai_dashboard/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/json_encoder.py` & `AI Dashboard-0.2.9/ai_dashboard/json_encoder.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/tabs/abstract_tab.py` & `AI Dashboard-0.2.9/ai_dashboard/tabs/abstract_tab.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/aggregation_chart.py` & `AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/aggregation_chart.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/data_report.py` & `AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/data_report.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/image.py` & `AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/image.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/markdown.py` & `AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/markdown.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/tabs/data_report/metric.py` & `AI Dashboard-0.2.9/ai_dashboard/tabs/data_report/metric.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/ai_dashboard/tabs/document_view/document_view.py` & `AI Dashboard-0.2.9/ai_dashboard/tabs/document_view/document_view.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/setup.py` & `AI Dashboard-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `AI Dashboard-0.2.8/tests/test_script.py` & `AI Dashboard-0.2.9/tests/test_script.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,17 +39,19 @@
     dashboard.push()
 
     # dashboard = client.Dashboard(
     #     dataset_id="iris-csv",
     #     name="My Dashboard" # Dashboard Name
     # )
 
-    tab = dashboard.CategoryView(title="new Category View")
+    tab = dashboard.CategoryView(
+        title="new Category View",
+    )
     tab.set_view(
-        primary_field="_cluster_.review_translation_vector_.kmeans-25",
+        cluster_field="_cluster_.review_translation_vector_.kmeans-25",
         # secondary_field="language",
     )
 
     dashboard.append(tab)
     dashboard.push()
 
     tab = dashboard.DocumentView(title="My Document View")
```


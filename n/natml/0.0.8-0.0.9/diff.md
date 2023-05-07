# Comparing `tmp/natml-0.0.8.tar.gz` & `tmp/natml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natml-0.0.8.tar", last modified: Wed Apr 12 03:30:44 2023, max compression
+gzip compressed data, was "natml-0.0.9.tar", last modified: Wed Apr 12 03:55:07 2023, max compression
```

## Comparing `natml-0.0.8.tar` & `natml-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:30:44.803252 natml-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-12 03:30:24.000000 natml-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 03:30:44.803252 natml-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 03:30:24.000000 natml-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:30:44.795252 natml-0.0.8/natml/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 03:30:24.000000 natml-0.0.8/natml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:30:44.799252 natml-0.0.8/natml/api/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 03:30:24.000000 natml-0.0.8/natml/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:30:44.799252 natml-0.0.8/natml/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-12 03:30:24.000000 natml-0.0.8/natml/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 03:30:24.000000 natml-0.0.8/natml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:30:44.795252 natml-0.0.8/natml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 03:30:44.000000 natml-0.0.8/natml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 03:30:44.000000 natml-0.0.8/natml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:30:44.000000 natml-0.0.8/natml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 03:30:44.000000 natml-0.0.8/natml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 03:30:44.000000 natml-0.0.8/natml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 03:30:44.000000 natml-0.0.8/natml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 03:30:44.803252 natml-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-12 03:30:24.000000 natml-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:55:07.584531 natml-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-12 03:54:48.000000 natml-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 03:55:07.584531 natml-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 03:54:48.000000 natml-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:55:07.576532 natml-0.0.9/natml/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 03:54:48.000000 natml-0.0.9/natml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:55:07.580531 natml-0.0.9/natml/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 03:54:48.000000 natml-0.0.9/natml/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:55:07.584531 natml-0.0.9/natml/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-12 03:54:48.000000 natml-0.0.9/natml/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 03:54:48.000000 natml-0.0.9/natml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:55:07.580531 natml-0.0.9/natml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 03:55:07.000000 natml-0.0.9/natml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 03:55:07.000000 natml-0.0.9/natml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:55:07.000000 natml-0.0.9/natml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 03:55:07.000000 natml-0.0.9/natml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 03:55:07.000000 natml-0.0.9/natml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 03:55:07.000000 natml-0.0.9/natml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 03:55:07.584531 natml-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-12 03:54:48.000000 natml-0.0.9/setup.py
```

### Comparing `natml-0.0.8/LICENSE` & `natml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/PKG-INFO` & `natml-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Zero deployment machine learning.
 Home-page: https://natml.ai
 Author: NatML Inc.
 Author-email: hi@natml.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.natml.ai/python
 Project-URL: Source, https://github.com/natmlx/natml-py
```

### Comparing `natml-0.0.8/natml/api/__init__.py` & `natml-0.0.9/natml/api/__init__.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/api.py` & `natml-0.0.9/natml/api/api.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/dtype.py` & `natml-0.0.9/natml/api/dtype.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/endpoint.py` & `natml-0.0.9/natml/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/graph.py` & `natml-0.0.9/natml/api/graph.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/license.py` & `natml-0.0.9/natml/api/license.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/prediction.py` & `natml-0.0.9/natml/api/prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,22 +161,16 @@
             access_key=access_key
         )
         # Check session
         session = response["createPredictionSession"]
         if not session:
             return None
         # Parse outputs
-
-        
-
         session["results"] = [_parse_output_feature(feature) for feature in session["results"]] if session["results"] and not raw_outputs else session["results"]
         session = PredictionSession(**session)
-
-        print(session)
-
         # Return
         return session
 
 def _parse_output_feature (feature: dict) -> Union[Feature, str, float, int, bool, Image.Image, list, dict]:
     data, type, shape = feature["data"], feature["type"], feature["shape"]
     # Handle image
     if type == Dtype.image:
```

### Comparing `natml-0.0.8/natml/api/predictor.py` & `natml-0.0.9/natml/api/predictor.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/profile.py` & `natml-0.0.9/natml/api/profile.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/session.py` & `natml-0.0.9/natml/api/session.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/tag.py` & `natml-0.0.9/natml/api/tag.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/upload.py` & `natml-0.0.9/natml/api/upload.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/api/user.py` & `natml-0.0.9/natml/api/user.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/__init__.py` & `natml-0.0.9/natml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/auth.py` & `natml-0.0.9/natml/cli/auth.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/demos.py` & `natml-0.0.9/natml/cli/demos.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/endpoints.py` & `natml-0.0.9/natml/cli/endpoints.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/graphs.py` & `natml-0.0.9/natml/cli/graphs.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/misc.py` & `natml-0.0.9/natml/cli/misc.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/predictors.py` & `natml-0.0.9/natml/cli/predictors.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml/cli/users.py` & `natml-0.0.9/natml/cli/users.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/natml.egg-info/PKG-INFO` & `natml-0.0.9/natml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Zero deployment machine learning.
 Home-page: https://natml.ai
 Author: NatML Inc.
 Author-email: hi@natml.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.natml.ai/python
 Project-URL: Source, https://github.com/natmlx/natml-py
```

### Comparing `natml-0.0.8/natml.egg-info/SOURCES.txt` & `natml-0.0.9/natml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `natml-0.0.8/setup.py` & `natml-0.0.9/setup.py`

 * *Files identical despite different names*


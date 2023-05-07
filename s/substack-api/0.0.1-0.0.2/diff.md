# Comparing `tmp/substack_api-0.0.1.tar.gz` & `tmp/substack_api-0.0.2.tar.gz`

## Comparing `substack_api-0.0.1.tar` & `substack_api-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 substack_api-0.0.1/src/substack_api/__init__.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 substack_api-0.0.1/src/substack_api/substack_api.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 substack_api-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 substack_api-0.0.1/LICENSE
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 substack_api-0.0.1/README.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 substack_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 substack_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 substack_api-0.0.2/src/substack_api/__init__.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 substack_api-0.0.2/src/substack_api/substack_api.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 substack_api-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 substack_api-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 substack_api-0.0.2/README.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 substack_api-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 substack_api-0.0.2/PKG-INFO
```

### Comparing `substack_api-0.0.1/src/substack_api/substack_api.py` & `substack_api-0.0.2/src/substack_api/substack_api.py`

 * *Files identical despite different names*

### Comparing `substack_api-0.0.1/LICENSE` & `substack_api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `substack_api-0.0.1/README.md` & `substack_api-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ## Installation
 
 `pip install substack-api`
 
 ## Usage
 
-```import substack_api```
+```from substack_api import substack_api```
 
 List all categories on Substack:
 
 ```
 substack_api.list_all_categories()
 ```
```

### Comparing `substack_api-0.0.1/pyproject.toml` & `substack_api-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling",
             "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "substack-api"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Nick Hagar", email="nicholasrhagar@gmail.com" },
 ]
 description = "The unofficial Substack API wrapper for Python."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `substack_api-0.0.1/PKG-INFO` & `substack_api-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substack-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: The unofficial Substack API wrapper for Python.
 Project-URL: Homepage, https://github.com/NHagar/substack_api
 Author-email: Nick Hagar <nicholasrhagar@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nick Hagar
         
@@ -45,15 +45,15 @@
 
 ## Installation
 
 `pip install substack-api`
 
 ## Usage
 
-```import substack_api```
+```from substack_api import substack_api```
 
 List all categories on Substack:
 
 ```
 substack_api.list_all_categories()
 ```
```


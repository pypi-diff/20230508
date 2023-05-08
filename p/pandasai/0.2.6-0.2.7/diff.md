# Comparing `tmp/pandasai-0.2.6.tar.gz` & `tmp/pandasai-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.6.tar", max compression
+gzip compressed data, was "pandasai-0.2.7.tar", max compression
```

## Comparing `pandasai-0.2.6.tar` & `pandasai-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.6/LICENSE
--rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.6/README.md
--rw-r--r--   0        0        0     7591 2023-05-07 22:54:48.892595 pandasai-0.2.6/pandasai/__init__.py
--rw-r--r--   0        0        0      107 2023-05-06 12:44:40.585715 pandasai-0.2.6/pandasai/constants.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.6/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.6/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.6/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.6/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.6/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.6/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3399 2023-05-07 22:56:45.176242 pandasai-0.2.6/pandasai/llm/base.py
--rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.6/pandasai/llm/base_hf.py
--rw-r--r--   0        0        0      505 2023-05-07 12:19:34.602219 pandasai-0.2.6/pandasai/llm/fake.py
--rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.6/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3851 2023-05-07 12:17:45.967747 pandasai-0.2.6/pandasai/llm/openai.py
--rw-r--r--   0        0        0      689 2023-05-07 10:03:05.449931 pandasai-0.2.6/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0      728 2023-05-07 23:01:59.186432 pandasai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.7/README.md
+-rw-r--r--   0        0        0     7591 2023-05-07 22:54:48.892595 pandasai-0.2.7/pandasai/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-08 09:22:18.023055 pandasai-0.2.7/pandasai/constants.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.7/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.7/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.7/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.7/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.7/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.7/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3539 2023-05-08 09:22:18.023356 pandasai-0.2.7/pandasai/llm/base.py
+-rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.7/pandasai/llm/base_hf.py
+-rw-r--r--   0        0        0      505 2023-05-07 12:19:34.602219 pandasai-0.2.7/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.7/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3851 2023-05-07 12:17:45.967747 pandasai-0.2.7/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      689 2023-05-07 10:03:05.449931 pandasai-0.2.7/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      728 2023-05-08 09:23:23.460361 pandasai-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.7/PKG-INFO
```

### Comparing `pandasai-0.2.6/LICENSE` & `pandasai-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/README.md` & `pandasai-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/__init__.py` & `pandasai-0.2.7/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/exceptions.py` & `pandasai-0.2.7/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/helpers/anonymizer.py` & `pandasai-0.2.7/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/helpers/notebook.py` & `pandasai-0.2.7/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/llm/alpaca.py` & `pandasai-0.2.7/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/llm/base.py` & `pandasai-0.2.7/pandasai/llm/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import ast
 import re
 from typing import Optional
 
 import astor
 
-from ..constants import END_CODE_TAG, START_CODE_TAG
+from ..constants import END_CODE_TAG, START_CODE_TAG, WHITELISTED_LIBRARIES
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
 
 
@@ -33,15 +33,18 @@
         raise APIKeyNotFoundError("Type has not been implemented")
 
     def _remove_imports(self, code: str) -> str:
         tree = ast.parse(code)
         new_body = [
             node
             for node in tree.body
-            if not isinstance(node, (ast.Import, ast.ImportFrom))
+            if not (
+                isinstance(node, (ast.Import, ast.ImportFrom))
+                and any(alias.name in WHITELISTED_LIBRARIES for alias in node.names)
+            )
         ]
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree).strip()
 
     def _polish_code(self, code: str) -> str:
         """
         Polish the code by removing the leading "python" or "py",  \
```

### Comparing `pandasai-0.2.6/pandasai/llm/base_hf.py` & `pandasai-0.2.7/pandasai/llm/base_hf.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/llm/open_assistant.py` & `pandasai-0.2.7/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/llm/openai.py` & `pandasai-0.2.7/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pandasai/llm/starcoder.py` & `pandasai-0.2.7/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.6/pyproject.toml` & `pandasai-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.6"
+version = "0.2.7"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.2.6/PKG-INFO` & `pandasai-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.6
+Version: 0.2.7
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


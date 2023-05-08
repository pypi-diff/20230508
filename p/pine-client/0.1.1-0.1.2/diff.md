# Comparing `tmp/pine_client-0.1.1.tar.gz` & `tmp/pine_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pine_client-0.1.1.tar", max compression
+gzip compressed data, was "pine_client-0.1.2.tar", max compression
```

## Comparing `pine_client-0.1.1.tar` & `pine_client-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       95 2023-05-06 16:01:56.000000 pine_client-0.1.1/README.md
--rw-r--r--   0        0        0       60 2023-05-06 16:01:56.000000 pine_client-0.1.1/pine_client/__init__.py
--rw-r--r--   0        0        0    32326 2023-05-06 16:01:56.000000 pine_client-0.1.1/pine_client/client.py
--rw-r--r--   0        0        0     2669 2023-05-06 16:01:56.000000 pine_client-0.1.1/pine_client/utils.py
--rw-r--r--   0        0        0      505 2023-05-06 16:02:11.000000 pine_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-05-08 14:55:52.000000 pine_client-0.1.2/README.md
+-rw-r--r--   0        0        0       60 2023-05-08 14:55:52.000000 pine_client-0.1.2/pine_client/__init__.py
+-rw-r--r--   0        0        0    32326 2023-05-08 14:55:52.000000 pine_client-0.1.2/pine_client/client.py
+-rw-r--r--   0        0        0     2659 2023-05-08 14:55:52.000000 pine_client-0.1.2/pine_client/utils.py
+-rw-r--r--   0        0        0      505 2023-05-08 14:56:04.000000 pine_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.1.2/PKG-INFO
```

### Comparing `pine_client-0.1.1/pine_client/client.py` & `pine_client-0.1.2/pine_client/client.py`

 * *Files identical despite different names*

### Comparing `pine_client-0.1.1/pine_client/utils.py` & `pine_client-0.1.2/pine_client/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from urllib.parse import quote_plus
+from urllib.parse import quote
 from typing import Any, List, Union
 from datetime import datetime
 import re
 
 
 def encode_uri_component(v: str) -> str:
-    return quote_plus(v, safe="~()*!'")
+    return quote(v, safe="~()*!'")
 
 
 encoded_slash = encode_uri_component("/")
 encoded_count = encode_uri_component("$count")
 trailing_count_regex = re.compile(f"(?:(?:{encoded_slash})|/){encoded_count}$")
```

### Comparing `pine_client-0.1.1/PKG-INFO` & `pine_client-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pine-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: This module provides the core layer for python interface for the pinejs API
 Author: Balena
 Author-email: info@balena.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


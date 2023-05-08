# Comparing `tmp/shafara_tool_kit-0.2.1.tar.gz` & `tmp/shafara_tool_kit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shafara_tool_kit-0.2.1.tar", max compression
+gzip compressed data, was "shafara_tool_kit-0.2.2.tar", max compression
```

## Comparing `shafara_tool_kit-0.2.1.tar` & `shafara_tool_kit-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    17098 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/LICENSE
--rw-r--r--   0        0        0      335 2023-05-07 23:44:09.268783 shafara_tool_kit-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      667 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/shafaratoolkit/__init__.py
--rw-r--r--   0        0        0      108 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/shafaratoolkit/props.py
--rw-r--r--   0        0        0     1324 2023-05-07 23:37:19.205311 shafara_tool_kit-0.2.1/shafaratoolkit/pytorchtools.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 shafara_tool_kit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    17098 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.2/LICENSE
+-rw-r--r--   0        0        0      335 2023-05-07 23:53:47.331573 shafara_tool_kit-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      667 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.2/shafaratoolkit/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.2/shafaratoolkit/props.py
+-rw-r--r--   0        0        0     1360 2023-05-07 23:53:15.497894 shafara_tool_kit-0.2.2/shafaratoolkit/pytorchtools.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 shafara_tool_kit-0.2.2/PKG-INFO
```

### Comparing `shafara_tool_kit-0.2.1/LICENSE` & `shafara_tool_kit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shafara_tool_kit-0.2.1/README.md` & `shafara_tool_kit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `shafara_tool_kit-0.2.1/shafaratoolkit/pytorchtools.py` & `shafara_tool_kit-0.2.2/shafaratoolkit/pytorchtools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import torch
+import numpy as np
+
 class EarlyStopping:
     "This uses numpy and torch, make sure they are loaded before using"
     def __init__(self, patience=10, delta=0, path='checkpoint.pt', verbose=False):
         self.patience = patience
         self.delta = delta
         self.path = path
         self.verbose = verbose
```

### Comparing `shafara_tool_kit-0.2.1/PKG-INFO` & `shafara_tool_kit-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shafara-tool-kit
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: jumashafara
 Author-email: jumashafara0@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


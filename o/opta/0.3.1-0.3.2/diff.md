# Comparing `tmp/opta-0.3.1.tar.gz` & `tmp/opta-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opta-0.3.1.tar", max compression
+gzip compressed data, was "opta-0.3.2.tar", max compression
```

## Comparing `opta-0.3.1.tar` & `opta-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2023-04-14 19:53:21.311162 opta-0.3.1/LICENSE
--rw-r--r--   0        0        0     1091 2023-04-14 19:53:21.311162 opta-0.3.1/opta/algorithms/abstract.py
--rw-r--r--   0        0        0     1982 2023-04-14 19:53:21.311162 opta-0.3.1/opta/algorithms/black_hole_optimization.py
--rw-r--r--   0        0        0      777 2023-04-14 19:53:21.311162 opta-0.3.1/opta/algorithms/random_search.py
--rw-r--r--   0        0        0      698 2023-04-14 19:53:21.311162 opta-0.3.1/opta/tools/coding.py
--rw-r--r--   0        0        0      379 2023-04-14 19:53:21.311162 opta-0.3.1/opta/tools/testing.py
--rw-r--r--   0        0        0      601 2023-04-14 19:53:21.311162 opta-0.3.1/opta/tools/vectors.py
--rw-r--r--   0        0        0      433 2023-04-14 19:53:21.311162 opta-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 opta-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-08 12:32:24.041667 opta-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1786 2023-05-08 12:32:24.041667 opta-0.3.2/opta/algorithms/abstract.py
+-rw-r--r--   0        0        0     1982 2023-05-08 12:32:24.041667 opta-0.3.2/opta/algorithms/black_hole_optimization.py
+-rw-r--r--   0        0        0      777 2023-05-08 12:32:24.041667 opta-0.3.2/opta/algorithms/random_search.py
+-rw-r--r--   0        0        0      810 2023-05-08 12:32:24.041667 opta-0.3.2/opta/tools/coding.py
+-rw-r--r--   0        0        0      658 2023-05-08 12:32:24.041667 opta-0.3.2/opta/tools/testing.py
+-rw-r--r--   0        0        0      833 2023-05-08 12:32:24.041667 opta-0.3.2/opta/tools/vectors.py
+-rw-r--r--   0        0        0      433 2023-05-08 12:32:24.041667 opta-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 opta-0.3.2/PKG-INFO
```

### Comparing `opta-0.3.1/LICENSE` & `opta-0.3.2/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Valentin Panovskiy
+Copyright (c) 2023 Valentin Panovskiy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `opta-0.3.1/opta/algorithms/black_hole_optimization.py` & `opta-0.3.2/opta/algorithms/black_hole_optimization.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.1/opta/algorithms/random_search.py` & `opta-0.3.2/opta/algorithms/random_search.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.1/opta/tools/coding.py` & `opta-0.3.2/opta/tools/coding.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
 
 import numpy
 
 
 class EncodeFromNumpy(json.JSONEncoder):
+    """Serialization utilities for numpy (encoding)"""
+
     def default(self, o):
         if isinstance(o, numpy.ndarray):
             return {"_kind_": "ndarray", "_value_": o.tolist()}
         return super().default(o)
 
 
 class DecodeToNumpy(json.JSONDecoder):
+    """Serialization utilities for numpy (decoding)"""
+
     def __init__(self, *args, **kwargs):
         json.JSONDecoder.__init__(
             self,
             object_hook=DecodeToNumpy.decoder_hook,
             *args,
             **kwargs,
         )
```


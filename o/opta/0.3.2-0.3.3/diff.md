# Comparing `tmp/opta-0.3.2.tar.gz` & `tmp/opta-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opta-0.3.2.tar", max compression
+gzip compressed data, was "opta-0.3.3.tar", max compression
```

## Comparing `opta-0.3.2.tar` & `opta-0.3.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2023-05-08 12:32:24.041667 opta-0.3.2/LICENSE
--rw-r--r--   0        0        0     1786 2023-05-08 12:32:24.041667 opta-0.3.2/opta/algorithms/abstract.py
--rw-r--r--   0        0        0     1982 2023-05-08 12:32:24.041667 opta-0.3.2/opta/algorithms/black_hole_optimization.py
--rw-r--r--   0        0        0      777 2023-05-08 12:32:24.041667 opta-0.3.2/opta/algorithms/random_search.py
--rw-r--r--   0        0        0      810 2023-05-08 12:32:24.041667 opta-0.3.2/opta/tools/coding.py
--rw-r--r--   0        0        0      658 2023-05-08 12:32:24.041667 opta-0.3.2/opta/tools/testing.py
--rw-r--r--   0        0        0      833 2023-05-08 12:32:24.041667 opta-0.3.2/opta/tools/vectors.py
--rw-r--r--   0        0        0      433 2023-05-08 12:32:24.041667 opta-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 opta-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-08 12:59:12.859385 opta-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1786 2023-05-08 12:59:12.859385 opta-0.3.3/opta/algorithms/abstract.py
+-rw-r--r--   0        0        0     1982 2023-05-08 12:59:12.859385 opta-0.3.3/opta/algorithms/black_hole_optimization.py
+-rw-r--r--   0        0        0      777 2023-05-08 12:59:12.859385 opta-0.3.3/opta/algorithms/random_search.py
+-rw-r--r--   0        0        0      810 2023-05-08 12:59:12.859385 opta-0.3.3/opta/tools/coding.py
+-rw-r--r--   0        0        0      658 2023-05-08 12:59:12.859385 opta-0.3.3/opta/tools/testing.py
+-rw-r--r--   0        0        0      833 2023-05-08 12:59:12.859385 opta-0.3.3/opta/tools/vectors.py
+-rw-r--r--   0        0        0      433 2023-05-08 12:59:12.859385 opta-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 opta-0.3.3/PKG-INFO
```

### Comparing `opta-0.3.2/LICENSE` & `opta-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opta-0.3.2/opta/algorithms/abstract.py` & `opta-0.3.3/opta/algorithms/abstract.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.2/opta/algorithms/black_hole_optimization.py` & `opta-0.3.3/opta/algorithms/black_hole_optimization.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.2/opta/algorithms/random_search.py` & `opta-0.3.3/opta/algorithms/random_search.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.2/opta/tools/coding.py` & `opta-0.3.3/opta/tools/coding.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.2/opta/tools/testing.py` & `opta-0.3.3/opta/tools/testing.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.2/opta/tools/vectors.py` & `opta-0.3.3/opta/tools/vectors.py`

 * *Files identical despite different names*


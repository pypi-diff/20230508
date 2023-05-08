# Comparing `tmp/findmyorder-1.3.6.tar.gz` & `tmp/findmyorder-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.3.6.tar", max compression
+gzip compressed data, was "findmyorder-1.3.7.tar", max compression
```

## Comparing `findmyorder-1.3.6.tar` & `findmyorder-1.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-08 10:31:32.107159 findmyorder-1.3.6/LICENSE
--rw-r--r--   0        0        0     2155 2023-05-08 10:31:32.107159 findmyorder-1.3.6/README.md
--rw-r--r--   0        0        0      113 2023-05-08 10:31:32.803168 findmyorder-1.3.6/findmyorder/__init__.py
--rw-r--r--   0        0        0      630 2023-05-08 10:31:32.107159 findmyorder-1.3.6/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-08 10:31:32.107159 findmyorder-1.3.6/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4120 2023-05-08 10:31:32.107159 findmyorder-1.3.6/findmyorder/main.py
--rw-r--r--   0        0        0     1758 2023-05-08 10:31:32.803168 findmyorder-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-08 13:42:30.867383 findmyorder-1.3.7/LICENSE
+-rw-r--r--   0        0        0     2155 2023-05-08 13:42:30.867383 findmyorder-1.3.7/README.md
+-rw-r--r--   0        0        0      113 2023-05-08 13:42:31.563390 findmyorder-1.3.7/findmyorder/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-08 13:42:30.867383 findmyorder-1.3.7/findmyorder/config.py
+-rw-r--r--   0        0        0      566 2023-05-08 13:42:30.867383 findmyorder-1.3.7/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     4116 2023-05-08 13:42:30.867383 findmyorder-1.3.7/findmyorder/main.py
+-rw-r--r--   0        0        0     1758 2023-05-08 13:42:31.563390 findmyorder-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.7/PKG-INFO
```

### Comparing `findmyorder-1.3.6/LICENSE` & `findmyorder-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.6/README.md` & `findmyorder-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.6/findmyorder/config.py` & `findmyorder-1.3.7/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.6/findmyorder/default_settings.toml` & `findmyorder-1.3.7/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.6/findmyorder/main.py` & `findmyorder-1.3.7/findmyorder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class FindMyOrder:
     """find an order class """
 
     def __init__(
         self,
     ):
-        self.logger = logging.getLogger(__name__)
+        self.logger = logging.getLogger("FMO")
 
     async def search(
         self,
         mystring: str,
     ) -> bool:
         """Search an order."""
         try:
@@ -34,15 +34,14 @@
                     logging.debug("found order in %s ", mystring)
                     return True
             logging.debug("no order found")
             return False
         except Exception:
             return False
 
-
     async def identify_order(
             self,
             mystring: str,
             ) -> dict:
         """Identify an order."""
         logging.debug("identify_order: %s", mystring)
         try:
```

### Comparing `findmyorder-1.3.6/pyproject.toml` & `findmyorder-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.3.6"
+version = "1.3.7"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.3.6/PKG-INFO` & `findmyorder-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.3.6
+Version: 1.3.7
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```


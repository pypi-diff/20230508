# Comparing `tmp/findmyorder-1.3.5.tar.gz` & `tmp/findmyorder-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.3.5.tar", max compression
+gzip compressed data, was "findmyorder-1.3.6.tar", max compression
```

## Comparing `findmyorder-1.3.5.tar` & `findmyorder-1.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-07 16:22:50.888827 findmyorder-1.3.5/LICENSE
--rw-r--r--   0        0        0     2155 2023-05-07 16:22:50.888827 findmyorder-1.3.5/README.md
--rw-r--r--   0        0        0      113 2023-05-07 16:22:51.556821 findmyorder-1.3.5/findmyorder/__init__.py
--rw-r--r--   0        0        0      631 2023-05-07 16:22:50.888827 findmyorder-1.3.5/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-07 16:22:50.888827 findmyorder-1.3.5/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4170 2023-05-07 16:22:50.888827 findmyorder-1.3.5/findmyorder/main.py
--rw-r--r--   0        0        0     1758 2023-05-07 16:22:51.556821 findmyorder-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-08 10:31:32.107159 findmyorder-1.3.6/LICENSE
+-rw-r--r--   0        0        0     2155 2023-05-08 10:31:32.107159 findmyorder-1.3.6/README.md
+-rw-r--r--   0        0        0      113 2023-05-08 10:31:32.803168 findmyorder-1.3.6/findmyorder/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-08 10:31:32.107159 findmyorder-1.3.6/findmyorder/config.py
+-rw-r--r--   0        0        0      566 2023-05-08 10:31:32.107159 findmyorder-1.3.6/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     4120 2023-05-08 10:31:32.107159 findmyorder-1.3.6/findmyorder/main.py
+-rw-r--r--   0        0        0     1758 2023-05-08 10:31:32.803168 findmyorder-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.6/PKG-INFO
```

### Comparing `findmyorder-1.3.5/LICENSE` & `findmyorder-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.5/README.md` & `findmyorder-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.5/findmyorder/default_settings.toml` & `findmyorder-1.3.6/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.5/findmyorder/main.py` & `findmyorder-1.3.6/findmyorder/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,17 @@
                 logging.debug("action identifier %s",
                               settings.action_identifier)
                 if string_check.lower() in settings.action_identifier.lower():
                     logging.debug("found order in %s ", mystring)
                     return True
             logging.debug("no order found")
             return False
-        except TypeError:
+        except Exception:
             return False
-            raise TypeError("exception in search")
+
 
     async def identify_order(
             self,
             mystring: str,
             ) -> dict:
         """Identify an order."""
         logging.debug("identify_order: %s", mystring)
```

### Comparing `findmyorder-1.3.5/pyproject.toml` & `findmyorder-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.3.5"
+version = "1.3.6"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.3.5/PKG-INFO` & `findmyorder-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.3.5
+Version: 1.3.6
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/pluthon-0.3.6.tar.gz` & `tmp/pluthon-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluthon-0.3.6.tar", last modified: Mon Apr 24 17:38:07 2023, max compression
+gzip compressed data, was "pluthon-0.3.7.tar", last modified: Mon May  8 18:35:29 2023, max compression
```

## Comparing `pluthon-0.3.6.tar` & `pluthon-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:38:07.090744 pluthon-0.3.6/
--rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-04-24 17:38:07.090744 pluthon-0.3.6/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1001 2023-04-24 17:36:57.000000 pluthon-0.3.6/README.md
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:38:07.086744 pluthon-0.3.6/pluthon/
--rw-r--r--   0 travis    (1000) travis    (1000)      594 2023-04-24 17:36:57.000000 pluthon-0.3.6/pluthon/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4583 2023-04-24 17:36:57.000000 pluthon-0.3.6/pluthon/pluthon_ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2582 2023-04-24 17:36:57.000000 pluthon-0.3.6/pluthon/pluthon_functional_data.py
--rw-r--r--   0 travis    (1000) travis    (1000)    17937 2023-04-24 17:36:57.000000 pluthon-0.3.6/pluthon/pluthon_sugar.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:38:07.090744 pluthon-0.3.6/pluthon.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-04-24 17:38:07.000000 pluthon-0.3.6/pluthon.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      275 2023-04-24 17:38:07.000000 pluthon-0.3.6/pluthon.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-24 17:38:07.000000 pluthon-0.3.6/pluthon.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       23 2023-04-24 17:38:07.000000 pluthon-0.3.6/pluthon.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       13 2023-04-24 17:38:07.000000 pluthon-0.3.6/pluthon.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-24 17:38:07.090744 pluthon-0.3.6/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1696 2023-04-24 17:36:57.000000 pluthon-0.3.6/setup.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-05-08 18:35:29.041704 pluthon-0.3.7/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-05-08 18:35:29.041704 pluthon-0.3.7/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1001 2023-05-08 18:34:51.000000 pluthon-0.3.7/README.md
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-05-08 18:35:29.037704 pluthon-0.3.7/pluthon/
+-rw-r--r--   0 travis    (1000) travis    (1000)      594 2023-05-08 18:34:51.000000 pluthon-0.3.7/pluthon/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4914 2023-05-08 18:34:51.000000 pluthon-0.3.7/pluthon/pluthon_ast.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2582 2023-05-08 18:34:51.000000 pluthon-0.3.7/pluthon/pluthon_functional_data.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    17937 2023-05-08 18:34:51.000000 pluthon-0.3.7/pluthon/pluthon_sugar.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-05-08 18:35:29.041704 pluthon-0.3.7/pluthon.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-05-08 18:35:28.000000 pluthon-0.3.7/pluthon.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      275 2023-05-08 18:35:29.000000 pluthon-0.3.7/pluthon.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-05-08 18:35:28.000000 pluthon-0.3.7/pluthon.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       23 2023-05-08 18:35:28.000000 pluthon-0.3.7/pluthon.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       13 2023-05-08 18:35:28.000000 pluthon-0.3.7/pluthon.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-05-08 18:35:29.041704 pluthon-0.3.7/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1696 2023-05-08 18:34:51.000000 pluthon-0.3.7/setup.py
```

### Comparing `pluthon-0.3.6/PKG-INFO` & `pluthon-0.3.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.3.6
+Version: 0.3.7
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/imperatorlang/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.3.6/README.md` & `pluthon-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.6/pluthon/__init__.py` & `pluthon-0.3.7/pluthon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from .pluthon_functional_data import *
 except ImportError as e:
     logging.error(
         "Error, trying to import dependencies. Should only occur upon package installation",
         exc_info=e,
     )
 
-VERSION = (0, 3, 6)
+VERSION = (0, 3, 7)
 
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "nielstron"
 __author_email__ = "n.muendler@web.de"
 __copyright__ = "Copyright (C) 2023 nielstron"
 __license__ = "MIT"
 __url__ = "https://github.com/imperatorlang/pluthon"
```

### Comparing `pluthon-0.3.6/pluthon/pluthon_ast.py` & `pluthon-0.3.7/pluthon/pluthon_ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,30 @@
         return uplc_ast.BuiltinUnit()
 
     def dumps(self) -> str:
         return "()"
 
 
 @dataclass
+class UPLCConstant(AST):
+    """
+    A generic UPLC constant that can be written directly in pluthon
+    Note: not present in pluthon
+    """
+
+    x: uplc_ast.Constant
+
+    def compile(self):
+        return self.x
+
+    def dumps(self) -> str:
+        return f"uplc[{self.x.dumps(dialect=uplc_ast.UPLCDialect.Aiken)}]"
+
+
+@dataclass
 class BuiltIn(AST):
     builtin: uplc_ast.BuiltInFun
 
     def compile(self):
         return uplc_ast.BuiltIn(self.builtin)
 
     def dumps(self) -> str:
```

### Comparing `pluthon-0.3.6/pluthon/pluthon_functional_data.py` & `pluthon-0.3.7/pluthon/pluthon_functional_data.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.6/pluthon/pluthon_sugar.py` & `pluthon-0.3.7/pluthon/pluthon_sugar.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.6/pluthon.egg-info/PKG-INFO` & `pluthon-0.3.7/pluthon.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.3.6
+Version: 0.3.7
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/imperatorlang/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.3.6/setup.py` & `pluthon-0.3.7/setup.py`

 * *Files identical despite different names*


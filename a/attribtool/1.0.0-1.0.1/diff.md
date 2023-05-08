# Comparing `tmp/attribtool-1.0.0.tar.gz` & `tmp/attribtool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attribtool-1.0.0.tar", max compression
+gzip compressed data, was "attribtool-1.0.1.tar", max compression
```

## Comparing `attribtool-1.0.0.tar` & `attribtool-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-05-07 20:48:57.095800 attribtool-1.0.0/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-07 21:45:41.876110 attribtool-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:06:36.254156 attribtool-1.0.0/attribtool/__init__.py
--rw-r--r--   0        0        0      764 2023-05-07 16:45:55.042179 attribtool-1.0.0/attribtool/ndattrib.py
--rw-r--r--   0        0        0     1204 2023-05-07 16:46:28.666206 attribtool-1.0.0/attribtool/nnattrib.py
--rw-r--r--   0        0        0      846 2023-05-07 21:55:34.697843 attribtool-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2611 1970-01-01 00:00:00.000000 attribtool-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-07 20:48:57.095800 attribtool-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1691 2023-05-08 17:43:58.399227 attribtool-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 09:06:36.254156 attribtool-1.0.1/attribtool/__init__.py
+-rw-r--r--   0        0        0      780 2023-05-08 18:12:08.012527 attribtool-1.0.1/attribtool/ndattrib.py
+-rw-r--r--   0        0        0     1303 2023-05-08 18:13:21.401434 attribtool-1.0.1/attribtool/nnattrib.py
+-rw-r--r--   0        0        0      853 2023-05-08 17:44:58.816167 attribtool-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 attribtool-1.0.1/PKG-INFO
```

### Comparing `attribtool-1.0.0/LICENSE` & `attribtool-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.0/README.md` & `attribtool-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AttribTool
 
-The project contains base classes that limit the possibility of adding new attributes without their prior declaration to classes inheriting from them or their objects.
+The project contains base classes that limit the possibility of adding new attributes without their prior declaration inside classes inheriting from them or their objects.
 
 Classes throw an AttributeError exception when trying to add an undefined attribute to a derived class or its object.
 
 ## Usage examples
 
 ```
 from attribtool.ndattrib import NoDynamicAttributes
```

### Comparing `attribtool-1.0.0/attribtool/nnattrib.py` & `attribtool-1.0.1/attribtool/nnattrib.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 # -*- coding: UTF-8 -*-
 """
   Author:  Jacek Kotlarski --<szumak@virthost.pl>
   Created: 07.05.2023
 
-  Purpose: NoNewAttributes class for restricting the dynamic creation
-  of attributes in inheriting classes.
+  Purpose: NoNewAttributes class for restricting the creation of dynamic
+  attributes on instances of derived types.
 
   The solution idea published in: Python Cookbook (2004), A. Martelli,
   A. Ravenscroft, D. Ascher
 """
 
+from types import FunctionType
 from typing import Any
 
 
-def _no_new_attributes(wrapped_setattr: Any):
+def _no_new_attributes(wrapped_setattr: Any) -> FunctionType:
     """Internal function for use in the current module only."""
 
-    def __setattr__(self, name: str, value: Any):
+    def __setattr__(self, name: str, value: Any) -> None:
         """Check if the attribute is defined, throw an exception if not."""
         if hasattr(self, name):
             wrapped_setattr(self, name, value)
         else:
             raise AttributeError(
                 f"Undefined attribute {name} cannot be added to {self}"
             )
 
     return __setattr__
 
 
 class NoNewAttributes:
     """NoNewAttributes - base class.
 
-    Class for restricting the dynamic creation of attributes in inheriting
-    classes.
+    Class for restricting the creation of dynamic attributes on instances
+    of derived types.
     """
 
-    __setattr__ = _no_new_attributes(object.__setattr__)
+    __setattr__: FunctionType = _no_new_attributes(object.__setattr__)
 
     class __metaclass__(type):
-        __setattr__ = _no_new_attributes(type.__setattr__)
+        __setattr__: FunctionType = _no_new_attributes(type.__setattr__)
 
 
 # #[EOF]#######################################################################
```

### Comparing `attribtool-1.0.0/pyproject.toml` & `attribtool-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "attribtool"
-version = "1.0.0"
-description = "Base classes for restricting the dynamic creation of attributes in inheriting classess."
+version = "1.0.1"
+description = "Base classes for restricting the creation of dynamic attributes on instances of derived types."
 authors = ["Jacek Kotlarski <szumak@virthost.pl>"]
 maintainers = ["Jacek Kotlarski <szumak@virthost.pl>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Szumak75/AttribTool"
 classifiers = [
 	"Programming Language :: Python :: 3",
```

### Comparing `attribtool-1.0.0/PKG-INFO` & `attribtool-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: attribtool
-Version: 1.0.0
-Summary: Base classes for restricting the dynamic creation of attributes in inheriting classess.
+Version: 1.0.1
+Summary: Base classes for restricting the creation of dynamic attributes on instances of derived types.
 Home-page: https://github.com/Szumak75/AttribTool
 License: MIT
 Author: Jacek Kotlarski
 Author-email: szumak@virthost.pl
 Maintainer: Jacek Kotlarski
 Maintainer-email: szumak@virthost.pl
 Requires-Python: >=3.7,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Project-URL: Repository, https://github.com/Szumak75/AttribTool
 Description-Content-Type: text/markdown
 
 # AttribTool
 
-The project contains base classes that limit the possibility of adding new attributes without their prior declaration to classes inheriting from them or their objects.
+The project contains base classes that limit the possibility of adding new attributes without their prior declaration inside classes inheriting from them or their objects.
 
 Classes throw an AttributeError exception when trying to add an undefined attribute to a derived class or its object.
 
 ## Usage examples
 
 ```
 from attribtool.ndattrib import NoDynamicAttributes
```


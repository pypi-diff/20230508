# Comparing `tmp/hagis-0.6.1.tar.gz` & `tmp/hagis-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.6.1.tar", last modified: Sun May  7 12:31:58 2023, max compression
+gzip compressed data, was "hagis-0.7.0.tar", last modified: Mon May  8 16:50:20 2023, max compression
```

## Comparing `hagis-0.6.1.tar` & `hagis-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:58.130229 hagis-0.6.1/
--rw-rw-rw-   0        0        0      923 2023-05-07 12:31:58.128402 hagis-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:58.120597 hagis-0.6.1/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22308 2023-05-07 12:30:18.000000 hagis-0.6.1/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-07 12:30:56.000000 hagis-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 12:31:58.130229 hagis-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 16:50:20.937307 hagis-0.7.0/
+-rw-rw-rw-   0        0        0      923 2023-05-08 16:50:20.935307 hagis-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 16:50:20.933317 hagis-0.7.0/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-08 16:50:20.000000 hagis-0.7.0/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-08 16:50:20.000000 hagis-0.7.0/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:50:20.000000 hagis-0.7.0/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 16:50:20.000000 hagis-0.7.0/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    23319 2023-05-08 16:40:56.000000 hagis-0.7.0/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-08 16:41:19.000000 hagis-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:50:20.937307 hagis-0.7.0/setup.cfg
```

### Comparing `hagis-0.6.1/PKG-INFO` & `hagis-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.6.1
+Version: 0.7.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.6.1/hagis.egg-info/PKG-INFO` & `hagis-0.7.0/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.6.1
+Version: 0.7.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.6.1/hagis.py` & `hagis-0.7.0/hagis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ A high availability GIS client. """
 import ast
 from _ast import Attribute, BoolOp, Call, Compare, Constant, Name
 from concurrent import futures
 from datetime import datetime
+from enum import Enum
 from hashlib import md5
 from inspect import getsource, signature
 from itertools import chain, islice
 from json import dumps, loads
 from time import time
 from types import SimpleNamespace
 from typing import Any, Callable, Dict, Generic, Iterator, List, Optional, Tuple, Type, TypeVar, Union
@@ -34,50 +35,54 @@
         """
         self._layer_url = layer_url
         self._model = model
         self._oid_field = oid_field
         self._shape_property_name = shape_property_name
         self._shape_property_type = None
         self._unknown_shape_types = [Any, object, SimpleNamespace]
-        self._fields: Dict[str, str] = {}
+        self._property_name_to_lower_field: Dict[str, str] = {}
+        self._lower_field_to_property_name_type: Dict[str, Tuple[str, type]] = {}
         self._generate_token: Callable[[], str] = lambda: ""
 
         self._has_parameterless_constructor = len(set(chain(
             signature(model.__init__).parameters.keys(),
             signature(model.__new__).parameters.keys()))) == 3
 
         self._is_dynamic = issubclass(model, SimpleNamespace)
 
         if self._is_dynamic:
             return
 
-        # List of custom mapping properties that have been handled.
-        mapped: List[str] = []
+        # Add custom properties that have not been handled as dynamically handled propeties.
+        for property_name, field in mapping.items():
+            self._property_name_to_lower_field[property_name] = field
 
         for model_type in reversed(model.mro()):
             if hasattr(model_type, "__annotations__"):
                 for property_name, property_type in model_type.__annotations__.items():
+                    # If Optional, get the atcual type via the argument.
+                    if hasattr(property_type, "__origin__"):
+                        property_type = property_type.__args__[0]
+
                     if property_name in mapping:
-                        self._fields[property_name] = mapping[property_name]
-                        mapped.append(property_name)
+                        lower_field = mapping[property_name].lower()
                     else:
-                        self._fields[property_name] = property_name
+                        lower_field = property_name.lower()
+
+                    self._property_name_to_lower_field[property_name] = lower_field
 
                     if property_name.lower() == shape_property_name.lower():
                         self._shape_property_name = property_name
                         self._shape_property_type = property_type
 
+                    self._lower_field_to_property_name_type[lower_field] = property_name, property_type
+
         self._is_arcgis_gemetry = hasattr(self._shape_property_type, "__module__")\
             and self._shape_property_type.__module__.startswith("arcgis.geometry.")
 
-        # Add custom properties that have not been handled as dynamically handled propeties.
-        for property_name, field in mapping.items():
-            if property_name not in mapped:
-                self._fields[property_name] = field
-
     _token_cache: Dict[Tuple[str, str], Tuple[str, int]] = {}
 
     def set_token_generator(self, username: str, password: str, referer: str = "",
                             token_url: str = "https://www.arcgis.com/sharing/generateToken", **kwargs: Any) -> None:
         """ Sets the token generation parameters.
 
         Args:
@@ -140,15 +145,16 @@
             return
 
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
             # Otherwise, request only what is used by the model.
-            fields = ",".join([f for f in self._fields.values() if f.lower() != self._shape_property_name.lower()])
+            fields = ",".join([f for f in self._property_name_to_lower_field.values()
+                               if f.lower() != self._shape_property_name.lower()])
             if not self._shape_property_name:
                 kwargs["returnGeometry"] = False
 
         if record_count:
             kwargs["resultRecordCount"] = record_count
 
         if wkid:
@@ -157,15 +163,15 @@
         for row in islice(self._query(where_clause, fields, record_count, max_workers, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
                 if self._has_parameterless_constructor:
                     item = self._model()
                     row_dict = {key.lower(): value for key, value in row.__dict__.items()}
-                    for property_name, field_name in self._fields.items():
+                    for property_name, field_name in self._property_name_to_lower_field.items():
                         setattr(item, property_name, row_dict[field_name.lower()])
                 else:
                     # Support for data classes and named tuples.
                     item = self._model(*row.__dict__.values())
 
                 yield item
 
@@ -209,16 +215,20 @@
             adds (Optional[List[T]], optional): Items to insert.  Defaults to None.
             updates (Optional[List[T]], optional): Items to update.  Defaults to None.
             deletes (Union[List[int], List[str], None], optional): Object IDs of items to delete.  Defaults to None.
 
         Returns:
             SimpleNamespace: Edit result object.
         """
-        adds_json = "" if adds is None else dumps([self._to_dict(x) for x in adds])
-        updates_json = "" if updates is None else dumps([self._to_dict(x) for x in updates])
+        def default(value: Any):
+            if isinstance(value, Enum):
+                return value.value
+
+        adds_json = "" if adds is None else dumps([self._to_dict(x) for x in adds], default=default)
+        updates_json = "" if updates is None else dumps([self._to_dict(x) for x in updates], default=default)
         deletes_json = "" if deletes is None else dumps([x for x in deletes])
         return self._call("applyEdits", adds=adds_json, updates=updates_json, deletes=deletes_json, **kwargs)
 
     def insert(self, items: List[T], **kwargs: Any) -> List[int]:
         """ Inserts new items on the remote server.
 
         Args:
@@ -276,15 +286,15 @@
     def _to_dict(self, item: T) -> Dict[str, Any]:
         dictionary: Dict[str, Any] = {}
         attributes: Dict[str, Any] = {}
 
         dictionary["attributes"] = attributes
 
         for key, value in item.__dict__.items():
-            field = self._fields[key]
+            field = self._property_name_to_lower_field[key]
             if key.lower() == self._shape_property_name.lower():
                 if self._is_arcgis_gemetry:
                     dictionary["geometry"] = loads(value.JSON)
                 else:
                     dictionary["geometry"] = value.__dict__
             elif isinstance(value, datetime):
                 attributes[field] = int((value - datetime.utcfromtimestamp(0)).total_seconds() * 1000)
@@ -317,20 +327,28 @@
             for f in obj.fields:
                 if f.type == "esriFieldTypeDate":
                     date_fields.append(f.name)
                 elif f.type == "esriFieldTypeGlobalID" or f.type == "esriFieldTypeGUID":
                     uuid_fields.append(f.name)
 
         for feature in obj.features:
-            if date_fields:
-                for key, value in feature.attributes.__dict__.items():
-                    if key in date_fields and value:
-                        feature.attributes.__dict__[key] = datetime.utcfromtimestamp(value / 1000)
-                    elif key in uuid_fields and value:
-                        feature.attributes.__dict__[key] = UUID(value)
+            for key, value in feature.attributes.__dict__.items():
+                if value is None:
+                    continue
+                if key in date_fields:
+                    feature.attributes.__dict__[key] = datetime.utcfromtimestamp(value / 1000)
+                elif key in uuid_fields:
+                    feature.attributes.__dict__[key] = UUID(value)
+                elif not self._is_dynamic:
+                    lower_field: str = key.lower()
+                    if lower_field in self._lower_field_to_property_name_type:
+                        _, property_type = self._lower_field_to_property_name_type[lower_field]
+                        if issubclass(property_type, Enum):
+                            feature.attributes.__dict__[key] = property_type(value)
+
             if hasattr(feature, "geometry") and feature.geometry and hasattr(obj, "spatialReference"):
                 feature.geometry.spatialReference = obj.spatialReference.__dict__
 
         return (obj.features, obj.exceededTransferLimit if hasattr(obj, "exceededTransferLimit") else False)
 
     def _get_oids(self, where_clause: str) -> List[int]:
         obj = self._call("query", where=where_clause, returnIdsOnly="true")
@@ -503,15 +521,15 @@
                     text += e.to_sql() if isinstance(e, LambdaVisitor) else f" {e}"
                 return text
 
         # Find the lambda expression and any free variables encapsulated in it.
         expression, freevars = LambdaFinder.find(predicate)
 
         # Generate a where clause.
-        where_clause = LambdaVisitor(expression, freevars, self._fields).to_sql().strip()
+        where_clause = LambdaVisitor(expression, freevars, self._property_name_to_lower_field).to_sql().strip()
 
         return where_clause
 
 
 class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
     """
```

### Comparing `hagis-0.6.1/pyproject.toml` & `hagis-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.6.1"
+version = "0.7.0"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


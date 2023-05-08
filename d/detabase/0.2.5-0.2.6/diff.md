# Comparing `tmp/detabase-0.2.5.tar.gz` & `tmp/detabase-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detabase-0.2.5.tar", max compression
+gzip compressed data, was "detabase-0.2.6.tar", max compression
```

## Comparing `detabase-0.2.5.tar` & `detabase-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      408 2023-05-07 12:41:54.704060 detabase-0.2.5/detabase/__init__.py
--rw-r--r--   0        0        0      972 2023-05-07 02:23:49.679517 detabase-0.2.5/detabase/base_models.py
--rw-r--r--   0        0        0     4970 2023-05-08 00:13:34.117216 detabase-0.2.5/detabase/casting.py
--rw-r--r--   0        0        0     4419 2023-05-06 16:53:36.189206 detabase-0.2.5/detabase/config.py
--rw-r--r--   0        0        0     3229 2023-05-07 22:59:19.779776 detabase-0.2.5/detabase/constants.py
--rw-r--r--   0        0        0     2297 2023-05-07 22:24:17.389745 detabase-0.2.5/detabase/context.py
--rw-r--r--   0        0        0     9559 2023-05-08 00:24:40.717815 detabase-0.2.5/detabase/descriptor.py
--rw-r--r--   0        0        0    10335 2023-05-08 00:13:34.124512 detabase-0.2.5/detabase/deta_model.py
--rw-r--r--   0        0        0     5487 2023-05-07 22:32:30.399216 detabase-0.2.5/detabase/engine.py
--rw-r--r--   0        0        0     1346 2023-05-07 23:00:35.871930 detabase-0.2.5/detabase/enums.py
--rw-r--r--   0        0        0     2147 2023-05-08 00:28:38.796959 detabase-0.2.5/detabase/form.py
--rw-r--r--   0        0        0     1589 2023-05-07 02:26:17.056907 detabase-0.2.5/detabase/json_encoder.py
--rw-r--r--   0        0        0      520 2023-05-06 19:28:05.417332 detabase-0.2.5/detabase/protocols.py
--rw-r--r--   0        0        0     3005 2023-05-07 22:50:49.459643 detabase-0.2.5/detabase/regex.py
--rw-r--r--   0        0        0     3816 2023-05-08 00:13:34.120593 detabase-0.2.5/detabase/types.py
--rw-r--r--   0        0        0      480 2023-05-08 00:28:38.801658 detabase-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      768 2023-05-08 00:28:49.097119 detabase-0.2.5/setup.py
--rw-r--r--   0        0        0      586 2023-05-08 00:28:49.097312 detabase-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      441 2023-05-08 05:04:41.414733 detabase-0.2.6/detabase/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-07 02:23:49.679517 detabase-0.2.6/detabase/base_models.py
+-rw-r--r--   0        0        0     4919 2023-05-08 05:04:41.411860 detabase-0.2.6/detabase/casting.py
+-rw-r--r--   0        0        0     4419 2023-05-06 16:53:36.189206 detabase-0.2.6/detabase/config.py
+-rw-r--r--   0        0        0     3229 2023-05-07 22:59:19.779776 detabase-0.2.6/detabase/constants.py
+-rw-r--r--   0        0        0     2297 2023-05-07 22:24:17.389745 detabase-0.2.6/detabase/context.py
+-rw-r--r--   0        0        0     9961 2023-05-08 05:04:41.407601 detabase-0.2.6/detabase/descriptor.py
+-rw-r--r--   0        0        0    10335 2023-05-08 00:13:34.124512 detabase-0.2.6/detabase/deta_model.py
+-rw-r--r--   0        0        0     5487 2023-05-07 22:32:30.399216 detabase-0.2.6/detabase/engine.py
+-rw-r--r--   0        0        0     1346 2023-05-07 23:00:35.871930 detabase-0.2.6/detabase/enums.py
+-rw-r--r--   0        0        0     2147 2023-05-08 00:28:38.796959 detabase-0.2.6/detabase/form.py
+-rw-r--r--   0        0        0     1589 2023-05-07 02:26:17.056907 detabase-0.2.6/detabase/json_encoder.py
+-rw-r--r--   0        0        0     1436 2023-05-08 02:48:42.445366 detabase-0.2.6/detabase/model_key.py
+-rw-r--r--   0        0        0      520 2023-05-06 19:28:05.417332 detabase-0.2.6/detabase/protocols.py
+-rw-r--r--   0        0        0     3005 2023-05-07 22:50:49.459643 detabase-0.2.6/detabase/regex.py
+-rw-r--r--   0        0        0     3816 2023-05-08 00:13:34.120593 detabase-0.2.6/detabase/types.py
+-rw-r--r--   0        0        0      480 2023-05-08 05:04:41.418133 detabase-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-05-08 05:04:53.175025 detabase-0.2.6/setup.py
+-rw-r--r--   0        0        0      586 2023-05-08 05:04:53.175211 detabase-0.2.6/PKG-INFO
```

### Comparing `detabase-0.2.5/detabase/base_models.py` & `detabase-0.2.6/detabase/base_models.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/casting.py` & `detabase-0.2.6/detabase/casting.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,22 +92,23 @@
     if isinstance(obj, str):
         return split_lines(obj)
     elif not obj:
         return []
 
 
 def parse_to_int(obj: Union[str, float, Decimal, datetime.datetime, datetime.date]) -> int:
-    if isinstance(obj, str):
+    if isinstance(obj, int):
+        return obj
+    elif isinstance(obj, str):
         return int(parse_to_float(obj))
     elif isinstance(obj, Decimal):
         return int(obj)
     elif isinstance(obj, (datetime.date, datetime.datetime)):
         return obj.toordinal()
 
-
 def parse_to_date(obj: Union[str, datetime.date, datetime.datetime, int]) -> datetime.date:
     if type(obj) is datetime.date:
         return obj
     if isinstance(obj, str):
         return datetime.date.fromisoformat(obj)
     elif isinstance(obj, int):
         return datetime.date.fromordinal(obj)
@@ -129,23 +130,18 @@
 def parse_to_enum(obj: Any, enum_type: EnumMeta) -> Enum:
     try:
         return enum_type[obj]
     except KeyError:
         return enum_type(obj)
     
 
-
 def parse_to_regex_type(obj: Any, regex_type: type[RegexType]) -> RegexType:
     if obj is None:
         obj = ''
     return regex_type(obj)
-    # try:
-    #     return regex_type(obj)
-    # except BaseException as e:
-    #     return obj
 
 
 def parse_to_bytes(obj: Union[str, bytes]) -> bytes:
     if type(obj) is bytes:
         return obj
     if isinstance(obj, str):
         return obj.encode('utf-8')
@@ -157,15 +153,14 @@
     elif type(obj) is str:
         return obj
     elif isinstance(obj, bytes):
         return obj.decode('utf-8')
     return str(obj)
     
 
-
 def parse_to_number(obj: Any) -> Union[int, float]:
     if isinstance(obj, str):
         obj = obj.replace(',', '.')
         if '.' in obj:
             return parse_to_float(obj)
         else:
             return parse_to_int(obj)
```

### Comparing `detabase-0.2.5/detabase/config.py` & `detabase-0.2.6/detabase/config.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/constants.py` & `detabase-0.2.6/detabase/constants.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/context.py` & `detabase-0.2.6/detabase/context.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/descriptor.py` & `detabase-0.2.6/detabase/descriptor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 __all__ = ['Descriptor', 'HiddenField', 'DetaModelField', 'DateField', 'DateTimeField', 'TitleField', 'EnumField',
-           'CheckBoxField', 'AutoField', 'StringField', 'RegexField', 'IntField', 'FloatField', 'NumberField']
+           'CheckBoxField', 'AutoField', 'StringField', 'RegexField', 'IntField', 'FloatField', 'NumberField',
+           'TextAreaField', 'PasswordField', 'BytesField', 'ModelKeyField']
 
 import datetime
 from functools import partial
 from dataclasses import MISSING
 from typing import ClassVar, Optional, Union, Any, Callable, Literal, get_type_hints
 from abc import ABC
 
@@ -252,14 +253,19 @@
     
     
 class DateTimeField(Descriptor):
     HTML_TAG = 'input'
     INPUT_TYPE = 'datetime-local'
     FINAL_TYPE = datetime.datetime
     
+
+class TextAreaField(Descriptor):
+    HTML_TAG = 'textarea'
+    FINAL_TYPE = str
+    
     
 class DetaModelField(Descriptor):
     HTML_TAG = 'input'
     INPUT_TYPE = 'text'
     FINAL_TYPE = str
     # HTMX = True
     DATALIST = True
@@ -276,7 +282,22 @@
             value = self.__get__(instance)
             if value not in [None, '']:
                 return f'data-value="{value}"'
             return ''
         return data_value()
         # return f'hx-get="/options/{self.model_type.item_name()}" hx-trigger="load" hx-target="#{self.model_type.item_name()}-list" {data_value()}"'
 
+
+class ModelKeyField(Descriptor):
+    HTML_TAG = 'input'
+    INPUT_TYPE = 'text'
+    HTMX = True
+
+
+class BytesField(Descriptor):
+    HTML_TAG = 'input'
+    INPUT_TYPE = 'text'
+
+
+class PasswordField(BytesField):
+    INPUT_TYPE = 'password'
+
```

### Comparing `detabase-0.2.5/detabase/deta_model.py` & `detabase-0.2.6/detabase/deta_model.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/engine.py` & `detabase-0.2.6/detabase/engine.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/enums.py` & `detabase-0.2.6/detabase/enums.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/form.py` & `detabase-0.2.6/detabase/form.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/json_encoder.py` & `detabase-0.2.6/detabase/json_encoder.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/protocols.py` & `detabase-0.2.6/detabase/protocols.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/regex.py` & `detabase-0.2.6/detabase/regex.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/detabase/types.py` & `detabase-0.2.6/detabase/types.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.5/setup.py` & `detabase-0.2.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'deta[async]==1.1.0a2',
  'smartjs>=0.1.0,<0.2.0',
  'starlette>=0.26.1,<0.27.0',
  'type-extensions>=0.1.2,<0.2.0']
 
 setup_kwargs = {
     'name': 'detabase',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'Base arquitecture for projects using Deta.',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `detabase-0.2.5/PKG-INFO` & `detabase-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detabase
-Version: 0.2.5
+Version: 0.2.6
 Summary: Base arquitecture for projects using Deta.
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```


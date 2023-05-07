# Comparing `tmp/detabase-0.2.2.tar.gz` & `tmp/detabase-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detabase-0.2.2.tar", max compression
+gzip compressed data, was "detabase-0.2.3.tar", max compression
```

## Comparing `detabase-0.2.2.tar` & `detabase-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      408 2023-05-07 12:41:54.704060 detabase-0.2.2/detabase/__init__.py
--rw-r--r--   0        0        0      972 2023-05-07 02:23:49.679517 detabase-0.2.2/detabase/base_models.py
--rw-r--r--   0        0        0     4592 2023-05-07 14:57:05.715206 detabase-0.2.2/detabase/casting.py
--rw-r--r--   0        0        0     4419 2023-05-06 16:53:36.189206 detabase-0.2.2/detabase/config.py
--rw-r--r--   0        0        0     3229 2023-05-07 22:59:19.779776 detabase-0.2.2/detabase/constants.py
--rw-r--r--   0        0        0     2297 2023-05-07 22:24:17.389745 detabase-0.2.2/detabase/context.py
--rw-r--r--   0        0        0     8376 2023-05-07 18:26:36.406632 detabase-0.2.2/detabase/descriptor.py
--rw-r--r--   0        0        0    10149 2023-05-07 22:33:57.443611 detabase-0.2.2/detabase/deta_model.py
--rw-r--r--   0        0        0     5487 2023-05-07 22:32:30.399216 detabase-0.2.2/detabase/engine.py
--rw-r--r--   0        0        0     1346 2023-05-07 23:00:35.871930 detabase-0.2.2/detabase/enums.py
--rw-r--r--   0        0        0     1078 2023-05-07 22:37:24.714167 detabase-0.2.2/detabase/form.py
--rw-r--r--   0        0        0     1589 2023-05-07 02:26:17.056907 detabase-0.2.2/detabase/json_encoder.py
--rw-r--r--   0        0        0      520 2023-05-06 19:28:05.417332 detabase-0.2.2/detabase/protocols.py
--rw-r--r--   0        0        0     3005 2023-05-07 22:50:49.459643 detabase-0.2.2/detabase/regex.py
--rw-r--r--   0        0        0     3793 2023-05-07 02:39:12.720415 detabase-0.2.2/detabase/types.py
--rw-r--r--   0        0        0      480 2023-05-07 23:10:18.609285 detabase-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      768 2023-05-07 23:20:35.471364 detabase-0.2.2/setup.py
--rw-r--r--   0        0        0      586 2023-05-07 23:20:35.471563 detabase-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      408 2023-05-07 12:41:54.704060 detabase-0.2.3/detabase/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-07 02:23:49.679517 detabase-0.2.3/detabase/base_models.py
+-rw-r--r--   0        0        0     4592 2023-05-07 14:57:05.715206 detabase-0.2.3/detabase/casting.py
+-rw-r--r--   0        0        0     4419 2023-05-06 16:53:36.189206 detabase-0.2.3/detabase/config.py
+-rw-r--r--   0        0        0     3229 2023-05-07 22:59:19.779776 detabase-0.2.3/detabase/constants.py
+-rw-r--r--   0        0        0     2297 2023-05-07 22:24:17.389745 detabase-0.2.3/detabase/context.py
+-rw-r--r--   0        0        0     8552 2023-05-07 23:44:40.090080 detabase-0.2.3/detabase/descriptor.py
+-rw-r--r--   0        0        0    10149 2023-05-07 22:33:57.443611 detabase-0.2.3/detabase/deta_model.py
+-rw-r--r--   0        0        0     5487 2023-05-07 22:32:30.399216 detabase-0.2.3/detabase/engine.py
+-rw-r--r--   0        0        0     1346 2023-05-07 23:00:35.871930 detabase-0.2.3/detabase/enums.py
+-rw-r--r--   0        0        0     2149 2023-05-07 23:54:56.722719 detabase-0.2.3/detabase/form.py
+-rw-r--r--   0        0        0     1589 2023-05-07 02:26:17.056907 detabase-0.2.3/detabase/json_encoder.py
+-rw-r--r--   0        0        0      520 2023-05-06 19:28:05.417332 detabase-0.2.3/detabase/protocols.py
+-rw-r--r--   0        0        0     3005 2023-05-07 22:50:49.459643 detabase-0.2.3/detabase/regex.py
+-rw-r--r--   0        0        0     3793 2023-05-07 02:39:12.720415 detabase-0.2.3/detabase/types.py
+-rw-r--r--   0        0        0      480 2023-05-07 23:44:40.092919 detabase-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-05-07 23:55:15.552460 detabase-0.2.3/setup.py
+-rw-r--r--   0        0        0      586 2023-05-07 23:55:15.552856 detabase-0.2.3/PKG-INFO
```

### Comparing `detabase-0.2.2/detabase/base_models.py` & `detabase-0.2.3/detabase/base_models.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/casting.py` & `detabase-0.2.3/detabase/casting.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/config.py` & `detabase-0.2.3/detabase/config.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/constants.py` & `detabase-0.2.3/detabase/constants.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/context.py` & `detabase-0.2.3/detabase/context.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/descriptor.py` & `detabase-0.2.3/detabase/descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         return self.label or self.public_name
     
     def htmx_config(self, instance=None):
         return ''
     
     def datalist(self):
         if self.DATALIST:
-            return f'{self.model_type.item_name()}-list'
-        return None
+            return f'{self.model_type.item_name()}-list"'
+        return ''
     
     def form_field_args(self, instance=None):
         return Arg(self.required), Arg(self.multiple), Kwarg('type', self.input_type), Kwarg('name', self.public_name), \
             Kwarg('id', self.public_name), Kwarg('list', self.datalist()) if self.datalist() else '', \
             Arg(self.htmx_config(instance)) if self.HTMX else '', \
             Klass(self.html_tag.bootstrap if not self.input_type else self.input_type.bootstrap), \
             Kwarg('placeholder', self.public_name)
@@ -160,14 +160,15 @@
         if self.HTML_TAG:
             id = Kwarg('id', f'{self.public_name}__container')
             if self.INPUT_TYPE in ['checkbox', 'range']:
                 return BaseElement(id, Tag('div'), self.form_field_container_class,
                                    elements=[self.label_element(), self.form_field_element(instance)])
             return BaseElement(id, Tag('div'), self.form_field_container_class,
                                elements=[self.form_field_element(instance), self.label_element()])
+        return ''
 
 
     
 class AutoField(Descriptor):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -184,23 +185,30 @@
     HTML_TAG = 'input'
     INPUT_TYPE = 'text'
     
     
 class TitleField(Descriptor):
     HTML_TAG = 'input'
     INPUT_TYPE = 'text'
-    FINAL_TYPE = str
     PARSER = lambda x, y: remove_extra_whitespaces(str(str(cast(x, y)))).title()
 
 class HiddenField(Descriptor):
     HTML_TAG = 'input'
     INPUT_TYPE = 'hidden'
-    FINAL_TYPE = str
     
     
+class IntField(Descriptor):
+    HTML_TAG = 'input'
+    INPUT_TYPE = 'number'
+    
+    
+class FloatField(Descriptor):
+    HTML_TAG = 'input'
+    INPUT_TYPE = 'number'
+    
 class CheckBoxField(Descriptor):
     HTML_TAG = 'input'
     INPUT_TYPE = 'checkbox'
     
     
 class EnumField(Descriptor):
     HTML_TAG = 'select'
@@ -237,9 +245,10 @@
     
     def htmx_config(self, instance=None):
         def data_value():
             value = self.__get__(instance)
             if value not in [None, '']:
                 return f'data-value="{value}"'
             return ''
-        return f'hx-get="/options/{self.model_type.item_name()}" hx-trigger="load" hx-target="#{self.model_type.item_name()}-list" {data_value()}"'
+        return data_value()
+        # return f'hx-get="/options/{self.model_type.item_name()}" hx-trigger="load" hx-target="#{self.model_type.item_name()}-list" {data_value()}"'
```

### Comparing `detabase-0.2.2/detabase/deta_model.py` & `detabase-0.2.3/detabase/deta_model.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/engine.py` & `detabase-0.2.3/detabase/engine.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/enums.py` & `detabase-0.2.3/detabase/enums.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/json_encoder.py` & `detabase-0.2.3/detabase/json_encoder.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/protocols.py` & `detabase-0.2.3/detabase/protocols.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/regex.py` & `detabase-0.2.3/detabase/regex.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/detabase/types.py` & `detabase-0.2.3/detabase/types.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.2/setup.py` & `detabase-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'deta[async]==1.1.0a2',
  'smartjs>=0.1.0,<0.2.0',
  'starlette>=0.26.1,<0.27.0',
  'type-extensions>=0.1.2,<0.2.0']
 
 setup_kwargs = {
     'name': 'detabase',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Base arquitecture for projects using Deta.',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `detabase-0.2.2/PKG-INFO` & `detabase-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detabase
-Version: 0.2.2
+Version: 0.2.3
 Summary: Base arquitecture for projects using Deta.
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/detabase-0.2.4.tar.gz` & `tmp/detabase-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detabase-0.2.4.tar", max compression
+gzip compressed data, was "detabase-0.2.5.tar", max compression
```

## Comparing `detabase-0.2.4.tar` & `detabase-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      408 2023-05-07 12:41:54.704060 detabase-0.2.4/detabase/__init__.py
--rw-r--r--   0        0        0      972 2023-05-07 02:23:49.679517 detabase-0.2.4/detabase/base_models.py
--rw-r--r--   0        0        0     4970 2023-05-08 00:13:34.117216 detabase-0.2.4/detabase/casting.py
--rw-r--r--   0        0        0     4419 2023-05-06 16:53:36.189206 detabase-0.2.4/detabase/config.py
--rw-r--r--   0        0        0     3229 2023-05-07 22:59:19.779776 detabase-0.2.4/detabase/constants.py
--rw-r--r--   0        0        0     2297 2023-05-07 22:24:17.389745 detabase-0.2.4/detabase/context.py
--rw-r--r--   0        0        0     9559 2023-05-08 00:24:40.717815 detabase-0.2.4/detabase/descriptor.py
--rw-r--r--   0        0        0    10335 2023-05-08 00:13:34.124512 detabase-0.2.4/detabase/deta_model.py
--rw-r--r--   0        0        0     5487 2023-05-07 22:32:30.399216 detabase-0.2.4/detabase/engine.py
--rw-r--r--   0        0        0     1346 2023-05-07 23:00:35.871930 detabase-0.2.4/detabase/enums.py
--rw-r--r--   0        0        0     2149 2023-05-07 23:54:56.722719 detabase-0.2.4/detabase/form.py
--rw-r--r--   0        0        0     1589 2023-05-07 02:26:17.056907 detabase-0.2.4/detabase/json_encoder.py
--rw-r--r--   0        0        0      520 2023-05-06 19:28:05.417332 detabase-0.2.4/detabase/protocols.py
--rw-r--r--   0        0        0     3005 2023-05-07 22:50:49.459643 detabase-0.2.4/detabase/regex.py
--rw-r--r--   0        0        0     3816 2023-05-08 00:13:34.120593 detabase-0.2.4/detabase/types.py
--rw-r--r--   0        0        0      480 2023-05-08 00:24:40.722413 detabase-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      768 2023-05-08 00:24:49.472280 detabase-0.2.4/setup.py
--rw-r--r--   0        0        0      586 2023-05-08 00:24:49.472671 detabase-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      408 2023-05-07 12:41:54.704060 detabase-0.2.5/detabase/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-07 02:23:49.679517 detabase-0.2.5/detabase/base_models.py
+-rw-r--r--   0        0        0     4970 2023-05-08 00:13:34.117216 detabase-0.2.5/detabase/casting.py
+-rw-r--r--   0        0        0     4419 2023-05-06 16:53:36.189206 detabase-0.2.5/detabase/config.py
+-rw-r--r--   0        0        0     3229 2023-05-07 22:59:19.779776 detabase-0.2.5/detabase/constants.py
+-rw-r--r--   0        0        0     2297 2023-05-07 22:24:17.389745 detabase-0.2.5/detabase/context.py
+-rw-r--r--   0        0        0     9559 2023-05-08 00:24:40.717815 detabase-0.2.5/detabase/descriptor.py
+-rw-r--r--   0        0        0    10335 2023-05-08 00:13:34.124512 detabase-0.2.5/detabase/deta_model.py
+-rw-r--r--   0        0        0     5487 2023-05-07 22:32:30.399216 detabase-0.2.5/detabase/engine.py
+-rw-r--r--   0        0        0     1346 2023-05-07 23:00:35.871930 detabase-0.2.5/detabase/enums.py
+-rw-r--r--   0        0        0     2147 2023-05-08 00:28:38.796959 detabase-0.2.5/detabase/form.py
+-rw-r--r--   0        0        0     1589 2023-05-07 02:26:17.056907 detabase-0.2.5/detabase/json_encoder.py
+-rw-r--r--   0        0        0      520 2023-05-06 19:28:05.417332 detabase-0.2.5/detabase/protocols.py
+-rw-r--r--   0        0        0     3005 2023-05-07 22:50:49.459643 detabase-0.2.5/detabase/regex.py
+-rw-r--r--   0        0        0     3816 2023-05-08 00:13:34.120593 detabase-0.2.5/detabase/types.py
+-rw-r--r--   0        0        0      480 2023-05-08 00:28:38.801658 detabase-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-05-08 00:28:49.097119 detabase-0.2.5/setup.py
+-rw-r--r--   0        0        0      586 2023-05-08 00:28:49.097312 detabase-0.2.5/PKG-INFO
```

### Comparing `detabase-0.2.4/detabase/base_models.py` & `detabase-0.2.5/detabase/base_models.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/casting.py` & `detabase-0.2.5/detabase/casting.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/config.py` & `detabase-0.2.5/detabase/config.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/constants.py` & `detabase-0.2.5/detabase/constants.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/context.py` & `detabase-0.2.5/detabase/context.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/descriptor.py` & `detabase-0.2.5/detabase/descriptor.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/deta_model.py` & `detabase-0.2.5/detabase/deta_model.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/engine.py` & `detabase-0.2.5/detabase/engine.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/enums.py` & `detabase-0.2.5/detabase/enums.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/form.py` & `detabase-0.2.5/detabase/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             self.model = instance
             self.instance = None
             self.form_title = Heading(3, Text(f'Adicionar {self.model.singular()}'))
             self.action = Kwarg('action', f'/form/new/{self.model.item_name()}')
             self.id = Kwarg('id', f'{self.model.table()}New')
             self.button = BaseElement(Tag('button'), Klass('btn btn-warning form-control new'), Text('salvar'))
 
-        self.form_fields = list_filtered([item.form_field(self.instance) for item in self.form_field_descriptors().values()])
+        self.form_fields = list_filtered([item.form_field(self.instance) for item in self.form_field_descriptors.values()])
         elements.append(self.form_title)
         elements.extend(self.form_fields)
         elements.extend(self.datalists)
         elements.append(self.button)
         args.extend([self.action, self.id, Kwarg('method', 'post'), Klass('form-control')])
         super().__init__(*args, elements=elements, **kwargs)
```

### Comparing `detabase-0.2.4/detabase/json_encoder.py` & `detabase-0.2.5/detabase/json_encoder.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/protocols.py` & `detabase-0.2.5/detabase/protocols.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/regex.py` & `detabase-0.2.5/detabase/regex.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/detabase/types.py` & `detabase-0.2.5/detabase/types.py`

 * *Files identical despite different names*

### Comparing `detabase-0.2.4/setup.py` & `detabase-0.2.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'deta[async]==1.1.0a2',
  'smartjs>=0.1.0,<0.2.0',
  'starlette>=0.26.1,<0.27.0',
  'type-extensions>=0.1.2,<0.2.0']
 
 setup_kwargs = {
     'name': 'detabase',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Base arquitecture for projects using Deta.',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `detabase-0.2.4/PKG-INFO` & `detabase-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detabase
-Version: 0.2.4
+Version: 0.2.5
 Summary: Base arquitecture for projects using Deta.
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```


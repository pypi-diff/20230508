# Comparing `tmp/layrz-forms-1.0.4.tar.gz` & `tmp/layrz-forms-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-forms-1.0.4.tar", last modified: Sat May  6 01:24:57 2023, max compression
+gzip compressed data, was "layrz-forms-1.0.5.tar", last modified: Mon May  8 17:01:55 2023, max compression
```

## Comparing `layrz-forms-1.0.4.tar` & `layrz-forms-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.638823 layrz-forms-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:24:57.638823 layrz-forms-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.633822 layrz-forms-1.0.4/layrz/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.634822 layrz-forms-1.0.4/layrz/forms/
--rw-rw-rw-   0 root         (0) root         (0)     5559 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.636822 layrz-forms-1.0.4/layrz/forms/fields/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/base.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/char.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.638823 layrz-forms-1.0.4/layrz_forms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 01:24:57.639823 layrz-forms-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:01:55.781021 layrz-forms-1.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-08 17:01:55.781021 layrz-forms-1.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:01:55.777021 layrz-forms-1.0.5/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:01:55.777021 layrz-forms-1.0.5/layrz/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     5934 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:01:55.780021 layrz-forms-1.0.5/layrz/forms/fields/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/char.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/layrz/forms/fields/number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:01:55.781021 layrz-forms-1.0.5/layrz_forms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-08 17:01:55.000000 layrz-forms-1.0.5/layrz_forms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-08 17:01:55.000000 layrz-forms-1.0.5/layrz_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 17:01:55.000000 layrz-forms-1.0.5/layrz_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 17:01:55.000000 layrz-forms-1.0.5/layrz_forms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 17:01:55.781021 layrz-forms-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-08 17:01:46.000000 layrz-forms-1.0.5/setup.py
```

### Comparing `layrz-forms-1.0.4/LICENSE` & `layrz-forms-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.4/PKG-INFO` & `layrz-forms-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.4
+Version: 1.0.5
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.4/README.md` & `layrz-forms-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.4/layrz/forms/__init__.py` & `layrz-forms-1.0.5/layrz/forms/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """ Init file """
+import inspect
+
 from .fields.base import Field
 from .fields.boolean import BooleanField
 from .fields.char import CharField
 from .fields.email import EmailField
 from .fields.id import IdField
 from .fields.json import JsonField
 from .fields.number import NumberField
-import inspect
 
 
 class Form:
   """
   Form class
   ---
   Notes:
@@ -26,19 +27,14 @@
 
   def __init__(self, obj=dict):
     """ Constructor """
     self._obj = obj
     self.calculate_members()
 
   @property
-  def _reserverd_words(self):
-    """ Reserved words """
-    return ('add_errors', 'change_obj', 'clean', 'errors', 'is_valid', 'set_obj', 'calculate_members', 'cleaned_data')
-
-  @property
   def cleaned_data(self):
     """ Returns the cleaned data """
     return self._obj
 
   def calculate_members(self):
     """ Calculate members """
     self._errors = {}
@@ -85,15 +81,42 @@
 
     return len(self._errors) == 0
 
   def errors(self):
     """ Returns the list of errors """
     return self._errors
 
-  def _validate_field(self, field):
+  def add_errors(self, key='', code='', extra_args=dict):
+    """ Add custom errors
+    This function is designed to be used in a clean function
+    ---
+    Arguments
+      key: str
+        Key of the field
+      code: str
+        Code of the error
+      extra_args: dict
+        Extra arguments to add to the error
+    """
+    if key == '' or code == '':
+      raise Exception('key and code are required')  #pylint: disable=W0719
+    camel_key = self._convert_to_camel(key=key)
+
+    if camel_key not in self._errors:
+      self._errors[camel_key] = []
+
+    new_error = {'code': code}
+    if extra_args and isinstance(extra_args, dict):
+      if callable(extra_args):
+        extra_args = extra_args()
+
+      new_error.update(extra_args)
+    self._errors[camel_key].append(new_error)
+
+  def _validate_field(self, field, new_key=None):
     """ Validate field """
     if isinstance(field[1], Field):
       func = getattr(field[1], 'validate')
       if callable(func):
         # Validate if the validate function has the correct parameters
         params = [p for p, _ in inspect.signature(func).parameters.items()]
         valid_params = ['key', 'value', 'errors']
@@ -113,54 +136,27 @@
           raise Exception(   #pylint: disable=W0719
             f'{field[0]} of type {type(field[1]).__name__} validate method has no the correct ' +\
             f'parameters. Expected parameters: {", ".join(valid_params)}. ' +\
             f'Actual parameters: {", ".join(params)}'
           )
 
         field[1].validate(
-          key=field[0],
+          key=field[0] if new_key is None else new_key,
           value=self._obj.get(field[0], None),
           errors=self._errors,
         )
       else:
         raise Exception(f'{type(field[1])} has no validate method')  #pylint: disable=W0719
 
   def _clean(self, clean_func):
     """ Clean function """
     func = getattr(self, clean_func)
     if callable(func):
       func()
 
-  def add_errors(self, key='', code='', extra_args=dict):
-    """ Add custom errors
-    This function is designed to be used in a clean function
-    ---
-    Arguments
-      key: str
-        Key of the field
-      code: str
-        Code of the error
-      extra_args: dict
-        Extra arguments to add to the error
-    """
-    if key == '' or code == '':
-      raise Exception('key and code are required')  #pylint: disable=W0719
-    camel_key = self._convert_to_camel(key=key)
-
-    if camel_key not in self._errors:
-      self._errors[camel_key] = []
-
-    new_error = {'code': code}
-    if extra_args and isinstance(extra_args, dict):
-      if callable(extra_args):
-        extra_args = extra_args()
-
-      new_error.update(extra_args)
-    self._errors[camel_key].append(new_error)
-
   def _convert_to_camel(self, key):
     """
     Convert the key to camel case
     """
     init, *temp = key.split('_')
 
     field = ''.join([init, *map(str.title, temp)])
@@ -170,14 +166,16 @@
     for item in field_items:
       field_final.append(''.join([item[0].lower(), item[1:]]))
 
     return '.'.join(field_final)
 
   def _validate_sub_form(self, field, form, data):
     """ Validate sub form """
+    if not isinstance(form, Form):
+      return
     form.set_obj(data)
     form.calculate_members()
     if not form.is_valid():
       for key, errors in form.errors().items():
         for error in errors:
           code = error['code']
           del error['code']
@@ -185,8 +183,32 @@
 
   def _validate_sub_form_as_list(self, field, form):
     """ Validate sub form for list """
     list_obj = self._obj.get(field, [])
 
     if isinstance(list_obj, (list, tuple)):
       for i, obj in enumerate(list_obj):
-        self._validate_sub_form(field=f'{field}.{i}', form=form, data=obj)
+        if isinstance(obj, Field):
+          self._validate_field(
+            field=obj,
+            new_key=f'{field}.{i}',
+          )
+        elif isinstance(obj, Form):
+          self._validate_sub_form(
+            field=f'{field}.{i}',
+            form=form,
+            data=obj,
+          )
+
+  @property
+  def _reserverd_words(self):
+    """ Reserved words """
+    return (
+      'add_errors',
+      'change_obj',
+      'clean',
+      'errors',
+      'is_valid',
+      'set_obj',
+      'calculate_members',
+      'cleaned_data',
+    )
```

### Comparing `layrz-forms-1.0.4/layrz/forms/fields/base.py` & `layrz-forms-1.0.5/layrz/forms/fields/base.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.4/layrz/forms/fields/boolean.py` & `layrz-forms-1.0.5/layrz/forms/fields/boolean.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,13 +26,13 @@
         Value to validate
       errors: dict
         Dict of errors
     """
 
     super(BooleanField, self).validate(key=key, value=value, errors=errors)
 
-    if not isinstance(value, bool):
+    if not isinstance(value, bool) and (self.required and value is not None):
       self._append_error(
         key=key,
         errors=errors,
         to_add={'code': 'invalid'},
       )
```

### Comparing `layrz-forms-1.0.4/layrz/forms/fields/char.py` & `layrz-forms-1.0.5/layrz/forms/fields/char.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.4/layrz/forms/fields/email.py` & `layrz-forms-1.0.5/layrz/forms/fields/email.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.4/layrz/forms/fields/id.py` & `layrz-forms-1.0.5/layrz/forms/fields/id.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         Value to validate
       errors: dict
         Dict of errors
     """
 
     super(IdField, self).validate(key=key, value=value, errors=errors)
 
-    if not isinstance(value, (int, str)):
+    if not isinstance(value, (int, str)) and (self.required and value is not None):
       self._append_error(
         key=key,
         errors=errors,
         to_add={'code': 'invalid'},
       )
     else:
       if isinstance(value, str):
```

### Comparing `layrz-forms-1.0.4/layrz/forms/fields/json.py` & `layrz-forms-1.0.5/layrz/forms/fields/json.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.4/layrz/forms/fields/number.py` & `layrz-forms-1.0.5/layrz/forms/fields/number.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         Value to validate
       errors: dict
         Dict of errors
     """
 
     super(NumberField, self).validate(key=key, value=value, errors=errors)
 
-    if not isinstance(value, self.datatype):
+    if not isinstance(value, self.datatype) and (self.required and value is not None):
       self._append_error(key=key, errors=errors, to_add={'code': 'invalid'})
     else:
       try:
         if self.min_value is not None:
           if self.datatype(value) < self.datatype(self.min_value):
             self._append_error(
               key=key,
```

### Comparing `layrz-forms-1.0.4/layrz_forms.egg-info/PKG-INFO` & `layrz-forms-1.0.5/layrz_forms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.4
+Version: 1.0.5
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.4/setup.py` & `layrz-forms-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   """ Return long description """
   with open('README.md', 'r', encoding='utf-8') as fh:
     return fh.read()
 
 
 setuptools.setup(
   name="layrz-forms",
-  version="1.0.4",
+  version="1.0.5",
   author="Golden M",
   author_email="software@goldenmcorp.com",
   description="Layrz forms and tools for Python",
   long_description=long_description(),
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```


# Comparing `tmp/django_graphbox-1.2.2.tar.gz` & `tmp/django_graphbox-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_graphbox-1.2.2.tar", last modified: Fri Apr 28 18:45:08 2023, max compression
+gzip compressed data, was "django_graphbox-1.2.3.tar", last modified: Mon May  8 00:09:25 2023, max compression
```

## Comparing `django_graphbox-1.2.2.tar` & `django_graphbox-1.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.2/LICENSE
--rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2022-07-20 15:01:25.000000 django_graphbox-1.2.2/MANIFEST.in
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18253 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)    20300 2023-02-23 04:15:18.000000 django_graphbox-1.2.2/README.md
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.525729 django_graphbox-1.2.2/docs/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.529731 django_graphbox-1.2.2/docs/source/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    17710 2023-02-23 15:06:34.000000 django_graphbox-1.2.2/docs/source/quickstart.rst
--rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2022-07-20 15:01:25.000000 django_graphbox-1.2.2/pyproject.toml
--rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/setup.cfg
--rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2022-07-20 15:01:25.000000 django_graphbox-1.2.2/setup.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.525729 django_graphbox-1.2.2/src/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.533733 django_graphbox-1.2.2/src/django_graphbox/
--rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    12252 2023-03-17 16:22:00.000000 django_graphbox-1.2.2/src/django_graphbox/builder.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1750 2023-04-28 18:44:37.000000 django_graphbox-1.2.2/src/django_graphbox/constants.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2022-07-30 04:00:13.000000 django_graphbox-1.2.2/src/django_graphbox/exceptions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/hasher.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/src/django_graphbox/helpers/
--rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    16165 2023-02-24 03:36:43.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/mutations.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     6584 2022-08-08 14:39:50.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/queries.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2022-07-30 04:08:45.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/sessions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/shared.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-02-23 21:40:53.000000 django_graphbox-1.2.2/src/django_graphbox/session.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.533733 django_graphbox-1.2.2/src/django_graphbox.egg-info/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18253 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/top_level.txt
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:09:25.984615 django_graphbox-1.2.3/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.3/LICENSE
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2022-07-20 15:01:25.000000 django_graphbox-1.2.3/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18375 2023-05-08 00:09:25.984615 django_graphbox-1.2.3/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    20300 2023-02-23 04:15:18.000000 django_graphbox-1.2.3/README.md
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:09:25.928614 django_graphbox-1.2.3/docs/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:09:25.956615 django_graphbox-1.2.3/docs/source/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    17832 2023-05-08 00:08:50.000000 django_graphbox-1.2.3/docs/source/quickstart.rst
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2022-07-20 15:01:25.000000 django_graphbox-1.2.3/pyproject.toml
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-05-08 00:09:25.988615 django_graphbox-1.2.3/setup.cfg
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2022-07-20 15:01:25.000000 django_graphbox-1.2.3/setup.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:09:25.940614 django_graphbox-1.2.3/src/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:09:25.960615 django_graphbox-1.2.3/src/django_graphbox/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2022-07-20 02:16:01.000000 django_graphbox-1.2.3/src/django_graphbox/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    12736 2023-05-07 23:57:24.000000 django_graphbox-1.2.3/src/django_graphbox/builder.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1750 2023-04-28 18:44:37.000000 django_graphbox-1.2.3/src/django_graphbox/constants.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2022-07-30 04:00:13.000000 django_graphbox-1.2.3/src/django_graphbox/exceptions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2022-07-20 02:16:01.000000 django_graphbox-1.2.3/src/django_graphbox/hasher.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:09:25.984615 django_graphbox-1.2.3/src/django_graphbox/helpers/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2022-07-20 02:16:01.000000 django_graphbox-1.2.3/src/django_graphbox/helpers/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    16165 2023-02-24 03:36:43.000000 django_graphbox-1.2.3/src/django_graphbox/helpers/mutations.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     6662 2023-05-07 23:58:24.000000 django_graphbox-1.2.3/src/django_graphbox/helpers/queries.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2022-07-30 04:08:45.000000 django_graphbox-1.2.3/src/django_graphbox/helpers/sessions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2022-07-20 02:16:01.000000 django_graphbox-1.2.3/src/django_graphbox/helpers/shared.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-02-23 21:40:53.000000 django_graphbox-1.2.3/src/django_graphbox/session.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-05-08 00:09:25.976615 django_graphbox-1.2.3/src/django_graphbox.egg-info/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18375 2023-05-08 00:09:25.000000 django_graphbox-1.2.3/src/django_graphbox.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-05-08 00:09:25.000000 django_graphbox-1.2.3/src/django_graphbox.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-05-08 00:09:25.000000 django_graphbox-1.2.3/src/django_graphbox.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-05-08 00:09:25.000000 django_graphbox-1.2.3/src/django_graphbox.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-05-08 00:09:25.000000 django_graphbox-1.2.3/src/django_graphbox.egg-info/top_level.txt
```

### Comparing `django_graphbox-1.2.2/LICENSE` & `django_graphbox-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/PKG-INFO` & `django_graphbox-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_graphbox
-Version: 1.2.2
+Version: 1.2.3
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -346,7 +346,8 @@
             
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
+    * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
```

### Comparing `django_graphbox-1.2.2/README.md` & `django_graphbox-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/docs/source/quickstart.rst` & `django_graphbox-1.2.3/docs/source/quickstart.rst`

 * *Files 1% similar despite different names*

```diff
@@ -329,8 +329,9 @@
                 )
             
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
-    * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
+    * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
+    * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
```

### Comparing `django_graphbox-1.2.2/setup.cfg` & `django_graphbox-1.2.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_graphbox
-version = 1.2.2
+version = 1.2.3
 description = Package for easy building GraphQL API with Django
 long_description = file:docs/source/quickstart.rst
 url = https://github.com/yefeza/django-graphbox
 author = Yeison Fernandez
 author_email = contacto@90horasporsemana.com
 license = MIT
 classifiers =
```

### Comparing `django_graphbox-1.2.2/src/django_graphbox/builder.py` & `django_graphbox-1.2.3/src/django_graphbox/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         Args:
             session_manager (SessionManager): Session manager to use.
         """
         self._models_config = {}
         self._models_by_op_name = {}
         self._session_manager = session_manager
 
-    def add_model(self, model, exclude_fields=(), pagination_length=0, pagination_style='infinite', external_filters=[], internal_filters=[], filters_opeator=Q.AND, access_group=None, access_by_operation={}, validators_by_operation={}, internal_field_resolvers={}, exclude_fields_by_operation={}, save_as_password=[], callbacks_by_operation={}, **kwargs):
+    def add_model(self, model, exclude_fields=(), pagination_length=0, pagination_style='infinite', external_filters=[], internal_filters=[], filters_opeator=Q.AND, access_group=None, access_by_operation={}, validators_by_operation={}, internal_field_resolvers={}, exclude_fields_by_operation={}, save_as_password=[], callbacks_by_operation={}, custom_attrs_for_type=[], ordering_field='id', **kwargs):
         """Add model for build operations.
 
         Args:
             model (django.models.Model): Model to add to the schema.
             exclude_fields (tuple or list): Fields to exclude from the model type.
             pagination_length (int): Number of items to return in a paginated response. 0 means no pagination.
             pagination_style (str): Pagination style. Possible values are 'infinite' and 'paginated'.
@@ -36,20 +36,25 @@
             filters_opeator (Q.AND, Q.OR): Operator to use for the filters.
             access_group (str): Access group to use for this model configured in ACCESS_GROUPS of session manager. This will be overriden by the access_by_operation.
             access_by_operation (dict): Dictionary with the operations to use for the access. {'operation': 'access_group', ...}
             validators_by_operation (dict): Dictionary with the validators to use for the access. {'operation': callable(info, model_instance, **kwargs), ...}
             internal_field_resolvers (dict): Dictionary with the internal field value resolvers on create_field and update_field operations
             save_as_password (list): List of fields to save as password with make_password function.
             callbacks_by_operation (dict): Dictionary with the callbacks list to use for the access. {'operation': [callable(info, model_instance, **kwargs)], ...}
+            custom_attrs_for_type (list): List of custom attributes to add to the model type. [{'name': 'attr_name', 'value': 'attr_value'}, ...]
+            ordering_field (str): Field to use for ordering the list_field operation.
         """
         #get the model name
         model_name = model.__name__
         #crreate the model type
         model_metaclass = type(f"Meta", (), {'model': model, 'exclude_fields': exclude_fields})
         model_type = type(f"{model_name}Type", (DjangoObjectType,), {'Meta': model_metaclass})
+        #add custom attributes to the model type
+        for attr in custom_attrs_for_type:
+            setattr(model_type, attr['name'], attr['value'])
         #create paginated type
         if pagination_length > 0 and pagination_style == 'paginated':
             paginated_type = type(f"{model_name}PageType", (graphene.ObjectType,), {'items': graphene.List(model_type), 'page': graphene.Int(), 'has_next_page': graphene.Boolean(), 'has_previous_page': graphene.Boolean(), 'total_pages': graphene.Int(), 'total_items': graphene.Int()})
         else:
             paginated_type = None
         #make a new model config
         config = {
@@ -64,15 +69,16 @@
             'filters_operator': filters_opeator,
             'access_group': access_group,
             'access_by_operation': access_by_operation,
             'validators_by_operation': validators_by_operation,
             'internal_field_resolvers': internal_field_resolvers,
             'exclude_fields_by_operation': exclude_fields_by_operation,
             'save_as_password': save_as_password,
-            'callbacks_by_operation': callbacks_by_operation
+            'callbacks_by_operation': callbacks_by_operation,
+            'ordering_field': ordering_field
         }
         self._models_config[model_name]=config
 
     def build_schema_query(self):
         """ Build query class for the schema.
 
         Returns:
```

### Comparing `django_graphbox-1.2.2/src/django_graphbox/constants.py` & `django_graphbox-1.2.3/src/django_graphbox/constants.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/src/django_graphbox/exceptions.py` & `django_graphbox-1.2.3/src/django_graphbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/src/django_graphbox/hasher.py` & `django_graphbox-1.2.3/src/django_graphbox/hasher.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/src/django_graphbox/helpers/mutations.py` & `django_graphbox-1.2.3/src/django_graphbox/helpers/mutations.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/src/django_graphbox/helpers/queries.py` & `django_graphbox-1.2.3/src/django_graphbox/helpers/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         config=self._models_by_op_name[operation_name]
         pagination_length=config.get('pagination_length')
         pagination_style=config.get('pagination_style')
         paginated_type=config.get('paginated_type')
         external_filters=config.get('external_filters')
         internal_filters=config.get('internal_filters')
         filters_operator=config.get('filters_operator')
+        ordering_field=config.get('ordering_field')
         query_object=None
         for filter_config in external_filters:
             param_value=kwargs.get(filter_config.get('param_name'))
             if param_value is not None:
                 if query_object is None:
                     query_object=Q(**{filter_config.get('field_name'): param_value})
                 else:
@@ -86,15 +87,15 @@
                         if callable(callback):
                             callback(info, result, **kwargs)
                 return result
             else:
                 pagina=kwargs.get('page')
                 inicio=(pagina*pagination_length)-pagination_length
                 fin=inicio+pagination_length
-                items=model.objects.filter(query_object)[inicio:fin]
+                items=model.objects.filter(query_object).order_by(ordering_field)[inicio:fin]
                 callbacks=config.get('callbacks_by_operation').get('list_field')
                 if callbacks is not None:
                     for callback in callbacks:
                         if callable(callback):
                             callback(info, items, **kwargs)
                 if pagination_style=='infinite':
                     return items
```

### Comparing `django_graphbox-1.2.2/src/django_graphbox/helpers/sessions.py` & `django_graphbox-1.2.3/src/django_graphbox/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/src/django_graphbox/helpers/shared.py` & `django_graphbox-1.2.3/src/django_graphbox/helpers/shared.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/src/django_graphbox/session.py` & `django_graphbox-1.2.3/src/django_graphbox/session.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.2/src/django_graphbox.egg-info/PKG-INFO` & `django_graphbox-1.2.3/src/django_graphbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-graphbox
-Version: 1.2.2
+Version: 1.2.3
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -346,7 +346,8 @@
             
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
+    * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
```

### Comparing `django_graphbox-1.2.2/src/django_graphbox.egg-info/SOURCES.txt` & `django_graphbox-1.2.3/src/django_graphbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*


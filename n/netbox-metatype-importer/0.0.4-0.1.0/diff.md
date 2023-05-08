# Comparing `tmp/netbox-metatype-importer-0.0.4.tar.gz` & `tmp/netbox-metatype-importer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-metatype-importer-0.0.4.tar", last modified: Sat Feb  4 08:23:33 2023, max compression
+gzip compressed data, was "netbox-metatype-importer-0.1.0.tar", last modified: Mon May  8 13:18:44 2023, max compression
```

## Comparing `netbox-metatype-importer-0.0.4.tar` & `netbox-metatype-importer-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 08:23:33.607488 netbox-metatype-importer-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-04 08:23:33.607488 netbox-metatype-importer-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 08:23:33.607488 netbox-metatype-importer-0.0.4/netbox_metatype_importer/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/gql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 08:23:33.607488 netbox-metatype-importer-0.0.4/netbox_metatype_importer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 08:23:33.603488 netbox-metatype-importer-0.0.4/netbox_metatype_importer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 08:23:33.607488 netbox-metatype-importer-0.0.4/netbox_metatype_importer/templates/netbox_metatype_importer/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/templates/netbox_metatype_importer/metadevicetype_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/templates/netbox_metatype_importer/metamoduletype_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 08:23:33.607488 netbox-metatype-importer-0.0.4/netbox_metatype_importer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-04 08:23:33.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-04 08:23:33.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 08:23:33.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-04 08:23:33.000000 netbox-metatype-importer-0.0.4/netbox_metatype_importer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 08:23:33.607488 netbox-metatype-importer-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-04 08:23:22.000000 netbox-metatype-importer-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:44.747242 netbox-metatype-importer-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 13:18:44.747242 netbox-metatype-importer-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:44.747242 netbox-metatype-importer-0.1.0/netbox_metatype_importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/gql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:44.747242 netbox-metatype-importer-0.1.0/netbox_metatype_importer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:44.743242 netbox-metatype-importer-0.1.0/netbox_metatype_importer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:44.747242 netbox-metatype-importer-0.1.0/netbox_metatype_importer/templates/netbox_metatype_importer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/templates/netbox_metatype_importer/metadevicetype_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/templates/netbox_metatype_importer/metamoduletype_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:44.747242 netbox-metatype-importer-0.1.0/netbox_metatype_importer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 13:18:44.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-08 13:18:44.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:18:44.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 13:18:44.000000 netbox-metatype-importer-0.1.0/netbox_metatype_importer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:18:44.747242 netbox-metatype-importer-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 13:18:32.000000 netbox-metatype-importer-0.1.0/setup.py
```

### Comparing `netbox-metatype-importer-0.0.4/LICENSE` & `netbox-metatype-importer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/LICENSE.md` & `netbox-metatype-importer-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/PKG-INFO` & `netbox-metatype-importer-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-metatype-importer
-Version: 0.0.4
+Version: 0.1.0
 Summary: Import Metatypes
 Home-page: https://github.com/Onemind-Services-LLC/netbox-metatype-importer
 Author: Abhimanyu Saharan
 Author-email: asaharan@onemindservices.com
 Maintainer: Prince Kumar
 Maintainer-email: pkumar@onemindservices.com
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `netbox-metatype-importer-0.0.4/README.md` & `netbox-metatype-importer-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Netbox DeviceType Import Plugin
+# Netbox DeviceType/ModuleType Import Plugin
 [NetBox](https://github.com/netbox-community/netbox) plugin for easy import DeviceType and ModuleType from [NetBox Device Type Library](https://github.com/netbox-community/devicetype-library). This is the continuation of the [Netbox DeviceType Import Plugin](https://github.com/k01ek/netbox-devicetype-importer) app.
 
 ## Description
 The plugin uses [GitHub GraphQL API](https://docs.github.com/en/graphql) to load DeviceType and ModuleType from [NetBox Device Type Library](https://github.com/netbox-community/devicetype-library). The plugin loads only file tree representation from GitHub repo and shows it as a table with vendor and model columns. DeviceType definitions files are loaded when you try to import selected models.
 To use GraphQL API you need to set GitHub personal access token in plugin settings. How to create the token, see ["Creating a personal access token."](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token)
 
-# Compatibility
+## Compatibility
 
-|  NetBox Version  | Plugin Version |
-|:----------------:|:--------------:|
-|      3.4.x       |     0.0.x      |
+| NetBox Version | Plugin Version |
+|:--------------:|:--------------:|
+|     3.4.x      |     0.0.x      |
+|     3.5.x      |     0.1.x      |
 
-# Installation
+## Installation
 
 * Install NetBox as per NetBox documentation
 * Add to local_requirements.txt:
   * `netbox-metatype-importer`
 * Install requirements: `./venv/bin/pip install -r local_requirements.txt`
 * Add to PLUGINS in NetBox configuration:
   * `'netbox_metatype_importer',`
```

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/filters.py` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/gql.py` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/gql.py`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/migrations/0001_initial.py` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/models.py` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/models.py`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/templates/netbox_metatype_importer/metadevicetype_list.html` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/templates/netbox_metatype_importer/metadevicetype_list.html`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/templates/netbox_metatype_importer/metamoduletype_list.html` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/templates/netbox_metatype_importer/metamoduletype_list.html`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/urls.py` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer/views.py` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django.utils.text import slugify
 from django.views.generic import View
 
 from dcim import forms
 from dcim.models import DeviceType, Manufacturer, ModuleType
 from netbox.views import generic
 from utilities.exceptions import AbortTransaction, PermissionsViolation
-from utilities.forms import ImportForm
+from utilities.forms.bulk_import import BulkImportForm
 from utilities.views import ContentTypePermissionRequiredMixin, GetReturnURLMixin
 from .choices import TypeChoices
 from .filters import MetaTypeFilterSet
 from .forms import MetaTypeFilterForm
 from .gql import GQLError, GitHubGqlAPI
 from .models import MetaType
 from .tables import MetaTypeTable
@@ -184,15 +184,15 @@
         # create manufacturer
         for vendor in vendors_for_cre:
             manufacturer, created = Manufacturer.objects.get_or_create(name=vendor, slug=slugify(vendor))
             if created:
                 vendor_count += 1
 
         for sha, yaml_text in dt_files.items():
-            form = ImportForm(data={'data': yaml_text, 'format': 'yaml'})
+            form = BulkImportForm(data={'data': yaml_text, 'format': 'yaml'})
             if form.is_valid():
                 data = form.cleaned_data['data']
 
                 if isinstance(data, list):
                     data = data[0]
 
                 model_form = self.model_form(data)
```

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer.egg-info/PKG-INFO` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-metatype-importer
-Version: 0.0.4
+Version: 0.1.0
 Summary: Import Metatypes
 Home-page: https://github.com/Onemind-Services-LLC/netbox-metatype-importer
 Author: Abhimanyu Saharan
 Author-email: asaharan@onemindservices.com
 Maintainer: Prince Kumar
 Maintainer-email: pkumar@onemindservices.com
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `netbox-metatype-importer-0.0.4/netbox_metatype_importer.egg-info/SOURCES.txt` & `netbox-metatype-importer-0.1.0/netbox_metatype_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-metatype-importer-0.0.4/setup.py` & `netbox-metatype-importer-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-metatype-importer',
-    version='0.0.4',
+    version='0.1.0',
     description='Import Metatypes',
     long_description='Import MetaTypes into NetBox',
     long_description_content_type="text/markdown",
     url='https://github.com/Onemind-Services-LLC/netbox-metatype-importer',
     author='Abhimanyu Saharan',
     author_email='asaharan@onemindservices.com',
     maintainer='Prince Kumar',
```


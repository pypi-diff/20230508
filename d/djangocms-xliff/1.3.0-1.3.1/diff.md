# Comparing `tmp/djangocms_xliff-1.3.0.tar.gz` & `tmp/djangocms_xliff-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_xliff-1.3.0.tar", max compression
+gzip compressed data, was "djangocms_xliff-1.3.1.tar", max compression
```

## Comparing `djangocms_xliff-1.3.0.tar` & `djangocms_xliff-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1073 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/LICENSE
--rw-r--r--   0        0        0     7132 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/README.md
--rw-r--r--   0        0        0       22 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/__init__.py
--rw-r--r--   0        0        0      216 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/apps.py
--rw-r--r--   0        0        0     2515 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/cms_toolbars.py
--rw-r--r--   0        0        0      186 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/exceptions.py
--rw-r--r--   0        0        0     1276 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/exports.py
--rw-r--r--   0        0        0     9102 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/extractors.py
--rw-r--r--   0        0        0      801 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/forms.py
--rw-r--r--   0        0        0     4297 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/imports.py
--rw-r--r--   0        0        0     4022 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5560 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/__init__.py
--rw-r--r--   0        0        0     1804 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_export.py
--rw-r--r--   0        0        0     1704 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_import.py
--rw-r--r--   0        0        0     1623 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_page_plugins.py
--rw-r--r--   0        0        0     5662 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/parsers.py
--rw-r--r--   0        0        0     1148 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/renderer.py
--rw-r--r--   0        0        0     1534 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/settings.py
--rw-r--r--   0        0        0      193 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/base.html
--rw-r--r--   0        0        0      151 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/error.html
--rw-r--r--   0        0        0      522 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/index.html
--rw-r--r--   0        0        0     1000 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
--rw-r--r--   0        0        0     1389 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html
--rw-r--r--   0        0        0     1116 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/success.html
--rw-r--r--   0        0        0      447 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/upload.html
--rw-r--r--   0        0        0     2152 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/types.py
--rw-r--r--   0        0        0      589 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/urls.py
--rw-r--r--   0        0        0     3919 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/utils.py
--rw-r--r--   0        0        0     6935 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/views.py
--rw-r--r--   0        0        0     1364 2023-05-03 13:02:46.522256 djangocms_xliff-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     8399 1970-01-01 00:00:00.000000 djangocms_xliff-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/LICENSE
+-rw-r--r--   0        0        0     7132 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/apps.py
+-rw-r--r--   0        0        0     2537 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/cms_toolbars.py
+-rw-r--r--   0        0        0      186 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/exceptions.py
+-rw-r--r--   0        0        0     1276 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/exports.py
+-rw-r--r--   0        0        0     9102 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/extractors.py
+-rw-r--r--   0        0        0      801 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/forms.py
+-rw-r--r--   0        0        0     4297 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/imports.py
+-rw-r--r--   0        0        0     4022 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5560 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/management/commands/__init__.py
+-rw-r--r--   0        0        0     1804 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/management/commands/xliff_export.py
+-rw-r--r--   0        0        0     1704 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/management/commands/xliff_import.py
+-rw-r--r--   0        0        0     1623 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/management/commands/xliff_page_plugins.py
+-rw-r--r--   0        0        0     5662 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/parsers.py
+-rw-r--r--   0        0        0     1148 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/renderer.py
+-rw-r--r--   0        0        0     1534 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/settings.py
+-rw-r--r--   0        0        0      193 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/base.html
+-rw-r--r--   0        0        0      151 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/error.html
+-rw-r--r--   0        0        0      522 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/export/index.html
+-rw-r--r--   0        0        0     1000 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
+-rw-r--r--   0        0        0     1389 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/import/preview.html
+-rw-r--r--   0        0        0     1116 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/import/success.html
+-rw-r--r--   0        0        0      447 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/import/upload.html
+-rw-r--r--   0        0        0     2152 2023-05-08 13:51:24.072628 djangocms_xliff-1.3.1/djangocms_xliff/types.py
+-rw-r--r--   0        0        0      589 2023-05-08 13:51:24.076628 djangocms_xliff-1.3.1/djangocms_xliff/urls.py
+-rw-r--r--   0        0        0     3919 2023-05-08 13:51:24.076628 djangocms_xliff-1.3.1/djangocms_xliff/utils.py
+-rw-r--r--   0        0        0     6935 2023-05-08 13:51:24.076628 djangocms_xliff-1.3.1/djangocms_xliff/views.py
+-rw-r--r--   0        0        0     1364 2023-05-08 13:51:24.076628 djangocms_xliff-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8399 1970-01-01 00:00:00.000000 djangocms_xliff-1.3.1/PKG-INFO
```

### Comparing `djangocms_xliff-1.3.0/LICENSE` & `djangocms_xliff-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/README.md` & `djangocms_xliff-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/cms_toolbars.py` & `djangocms_xliff-1.3.1/djangocms_xliff/cms_toolbars.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,9 +66,9 @@
 class XliffModelToolbar(XliffToolbar):
     """
     Inherit from this class to add xliff import and export functionality to your custom models
     """
 
     def user_has_permissions(self, obj) -> bool:
         if self.toolbar.edit_mode_active and obj and type(obj) != Page:
-            return self.request.user.has_perm(f"change_{obj._meta.model_name}")
+            return self.request.user.has_perm(f"{obj._meta.app_label}.change_{obj._meta.model_name}")
         return False
```

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/exports.py` & `djangocms_xliff-1.3.1/djangocms_xliff/exports.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/extractors.py` & `djangocms_xliff-1.3.1/djangocms_xliff/extractors.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/forms.py` & `djangocms_xliff-1.3.1/djangocms_xliff/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/imports.py` & `djangocms_xliff-1.3.1/djangocms_xliff/imports.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo` & `djangocms_xliff-1.3.1/djangocms_xliff/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po` & `djangocms_xliff-1.3.1/djangocms_xliff/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_export.py` & `djangocms_xliff-1.3.1/djangocms_xliff/management/commands/xliff_export.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_import.py` & `djangocms_xliff-1.3.1/djangocms_xliff/management/commands/xliff_import.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_page_plugins.py` & `djangocms_xliff-1.3.1/djangocms_xliff/management/commands/xliff_page_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/parsers.py` & `djangocms_xliff-1.3.1/djangocms_xliff/parsers.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/renderer.py` & `djangocms_xliff-1.3.1/djangocms_xliff/renderer.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/settings.py` & `djangocms_xliff-1.3.1/djangocms_xliff/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/index.html` & `djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/export/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff` & `djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html` & `djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/import/preview.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/success.html` & `djangocms_xliff-1.3.1/djangocms_xliff/templates/djangocms_xliff/import/success.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/types.py` & `djangocms_xliff-1.3.1/djangocms_xliff/types.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/urls.py` & `djangocms_xliff-1.3.1/djangocms_xliff/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/utils.py` & `djangocms_xliff-1.3.1/djangocms_xliff/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/djangocms_xliff/views.py` & `djangocms_xliff-1.3.1/djangocms_xliff/views.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.0/pyproject.toml` & `djangocms_xliff-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djangocms-xliff"
-version = "1.3.0"
+version = "1.3.1"
 description = "XLIFF Import and Export for the Django CMS"
 authors = ["Energie 360 <onlineservice@energie360.ch>"]
 maintainers = ["Energie 360 <onlineservice@energie360.ch>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://energie360.ch"
 repository = "https://github.com/energie360/djangocms-xliff"
```

### Comparing `djangocms_xliff-1.3.0/PKG-INFO` & `djangocms_xliff-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-xliff
-Version: 1.3.0
+Version: 1.3.1
 Summary: XLIFF Import and Export for the Django CMS
 Home-page: https://energie360.ch
 License: MIT
 Keywords: django,django-cms,xliff,import,export
 Author: Energie 360
 Author-email: onlineservice@energie360.ch
 Maintainer: Energie 360
```


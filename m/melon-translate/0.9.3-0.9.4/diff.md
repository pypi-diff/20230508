# Comparing `tmp/melon_translate-0.9.3.tar.gz` & `tmp/melon_translate-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_translate-0.9.3.tar", max compression
+gzip compressed data, was "melon_translate-0.9.4.tar", max compression
```

## Comparing `melon_translate-0.9.3.tar` & `melon_translate-0.9.4.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     2326 2023-02-15 15:01:16.708397 melon_translate-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/core/__init__.py
--rw-r--r--   0        0        0      400 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/core/asgi.py
--rw-r--r--   0        0        0     7519 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/core/settings.py
--rw-r--r--   0        0        0      627 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/core/urls.py
--rw-r--r--   0        0        0      320 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/core/utils/logging.py
--rw-r--r--   0        0        0      400 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/core/wsgi.py
--rw-r--r--   0        0        0        0 2023-02-15 15:01:16.708397 melon_translate-0.9.3/translate/service/__init__.py
--rw-r--r--   0        0        0     1828 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/admin.py
--rw-r--r--   0        0        0      181 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/apps.py
--rw-r--r--   0        0        0     2898 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/filters.py
--rw-r--r--   0        0        0        0 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/management/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/management/commands/__init__.py
--rw-r--r--   0        0        0      683 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/management/commands/delete_no_context_keys.py
--rw-r--r--   0        0        0     2432 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/management/commands/export_csv.py
--rw-r--r--   0        0        0     3298 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/management/commands/import_csv.py
--rw-r--r--   0        0        0    10979 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/management/commands/import_translations.py
--rw-r--r--   0        0        0    10599 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/migrations/0001_initial.py
--rw-r--r--   0        0        0      841 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/migrations/0002_alter_translation_key_alter_translation_language.py
--rw-r--r--   0        0        0      538 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/migrations/0003_translationkey_occ_views_gin.py
--rw-r--r--   0        0        0        0 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/migrations/__init__.py
--rw-r--r--   0        0        0     3341 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/models.py
--rw-r--r--   0        0        0      867 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/paginations.py
--rw-r--r--   0        0        0     6339 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/serializers.py
--rw-r--r--   0        0        0    23462 2023-02-15 15:01:16.709397 melon_translate-0.9.3/translate/service/static/assets/favicon.ico
--rw-r--r--   0        0        0   311841 2023-02-15 15:01:16.710397 melon_translate-0.9.3/translate/service/static/assets/img/swiss.jpeg
--rw-r--r--   0        0        0   706110 2023-02-15 15:01:16.711397 melon_translate-0.9.3/translate/service/static/assets/img/swiss_flg.jpeg
--rw-r--r--   0        0        0     7682 2023-02-15 15:01:16.711397 melon_translate-0.9.3/translate/service/static/css/style.css
--rw-r--r--   0        0        0     1537 2023-02-15 15:01:16.711397 melon_translate-0.9.3/translate/service/static/js/scripts.js
--rw-r--r--   0        0        0     2066 2023-02-15 15:01:16.711397 melon_translate-0.9.3/translate/service/templates/index.html
--rw-r--r--   0        0        0        0 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/__init__.py
--rw-r--r--   0        0        0      707 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/factories.py
--rw-r--r--   0        0        0     1366 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/fixtures/french_fixtures/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1971 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/fixtures/french_fixtures/snake_translations.json
--rw-r--r--   0        0        0     2062 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/fixtures/german_fixtures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      753 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/fixtures/german_fixtures/snake_translations.json
--rw-r--r--   0        0        0    28655 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/fixtures/import_csv_test_fixture.csv
--rw-r--r--   0        0        0     1920 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/providers.py
--rw-r--r--   0        0        0     7069 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/pytest_fixtures.py
--rw-r--r--   0        0        0     5845 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/test_commands.py
--rw-r--r--   0        0        0     5782 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/test_filters.py
--rw-r--r--   0        0        0     2265 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/test_models.py
--rw-r--r--   0        0        0     1144 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/test_paginations.py
--rw-r--r--   0        0        0     8542 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/test_serializers.py
--rw-r--r--   0        0        0     1751 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/tests/test_views.py
--rw-r--r--   0        0        0      439 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/urls.py
--rw-r--r--   0        0        0     3851 2023-02-15 15:01:16.712397 melon_translate-0.9.3/translate/service/views.py
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 melon_translate-0.9.3/setup.py
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 melon_translate-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     2326 2023-03-08 16:57:37.778343 melon_translate-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-03-08 16:57:37.778343 melon_translate-0.9.4/translate/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/core/__init__.py
+-rw-r--r--   0        0        0      400 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/core/asgi.py
+-rw-r--r--   0        0        0     7624 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/core/settings.py
+-rw-r--r--   0        0        0      627 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/core/urls.py
+-rw-r--r--   0        0        0      320 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/core/utils/logging.py
+-rw-r--r--   0        0        0      400 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/core/wsgi.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/__init__.py
+-rw-r--r--   0        0        0     1868 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/admin.py
+-rw-r--r--   0        0        0      181 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/apps.py
+-rw-r--r--   0        0        0     2898 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/filters.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/management/commands/__init__.py
+-rw-r--r--   0        0        0      683 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/management/commands/delete_no_context_keys.py
+-rw-r--r--   0        0        0     2432 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/management/commands/export_csv.py
+-rw-r--r--   0        0        0     3298 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/management/commands/import_csv.py
+-rw-r--r--   0        0        0     9885 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/management/commands/import_translations.py
+-rw-r--r--   0        0        0    10599 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/migrations/0001_initial.py
+-rw-r--r--   0        0        0      841 2023-03-08 16:57:37.779343 melon_translate-0.9.4/translate/service/migrations/0002_alter_translation_key_alter_translation_language.py
+-rw-r--r--   0        0        0      538 2023-03-08 16:57:37.780343 melon_translate-0.9.4/translate/service/migrations/0003_translationkey_occ_views_gin.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:57:37.780343 melon_translate-0.9.4/translate/service/migrations/__init__.py
+-rw-r--r--   0        0        0     3341 2023-03-08 16:57:37.780343 melon_translate-0.9.4/translate/service/models.py
+-rw-r--r--   0        0        0      867 2023-03-08 16:57:37.780343 melon_translate-0.9.4/translate/service/paginations.py
+-rw-r--r--   0        0        0     6339 2023-03-08 16:57:37.780343 melon_translate-0.9.4/translate/service/serializers.py
+-rw-r--r--   0        0        0    23462 2023-03-08 16:57:37.780343 melon_translate-0.9.4/translate/service/static/assets/favicon.ico
+-rw-r--r--   0        0        0   311841 2023-03-08 16:57:37.781343 melon_translate-0.9.4/translate/service/static/assets/img/swiss.jpeg
+-rw-r--r--   0        0        0   706110 2023-03-08 16:57:37.782343 melon_translate-0.9.4/translate/service/static/assets/img/swiss_flg.jpeg
+-rw-r--r--   0        0        0     7682 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/static/css/style.css
+-rw-r--r--   0        0        0     1537 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/static/js/scripts.js
+-rw-r--r--   0        0        0     2066 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/templates/index.html
+-rw-r--r--   0        0        0        0 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/__init__.py
+-rw-r--r--   0        0        0      707 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/factories.py
+-rw-r--r--   0        0        0     1366 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/fixtures/french_fixtures/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1971 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/fixtures/french_fixtures/snake_translations.json
+-rw-r--r--   0        0        0     2062 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/fixtures/german_fixtures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      753 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/fixtures/german_fixtures/snake_translations.json
+-rw-r--r--   0        0        0    28655 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/fixtures/import_csv_test_fixture.csv
+-rw-r--r--   0        0        0     1920 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/providers.py
+-rw-r--r--   0        0        0     7069 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/pytest_fixtures.py
+-rw-r--r--   0        0        0     5845 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/test_commands.py
+-rw-r--r--   0        0        0     5782 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/test_filters.py
+-rw-r--r--   0        0        0     2265 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/test_models.py
+-rw-r--r--   0        0        0     1144 2023-03-08 16:57:37.783343 melon_translate-0.9.4/translate/service/tests/test_paginations.py
+-rw-r--r--   0        0        0     8542 2023-03-08 16:57:37.784344 melon_translate-0.9.4/translate/service/tests/test_serializers.py
+-rw-r--r--   0        0        0     1751 2023-03-08 16:57:37.784344 melon_translate-0.9.4/translate/service/tests/test_views.py
+-rw-r--r--   0        0        0      439 2023-03-08 16:57:37.784344 melon_translate-0.9.4/translate/service/urls.py
+-rw-r--r--   0        0        0      733 2023-03-08 16:57:37.784344 melon_translate-0.9.4/translate/service/utils/version_handler.py
+-rw-r--r--   0        0        0     3851 2023-03-08 16:57:37.784344 melon_translate-0.9.4/translate/service/views.py
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 melon_translate-0.9.4/setup.py
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 melon_translate-0.9.4/PKG-INFO
```

### Comparing `melon_translate-0.9.3/pyproject.toml` & `melon_translate-0.9.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "melon-translate"
-version = "0.9.3"
+version = "0.9.4"
 description = "Melon-translate is a micro service for easing localisation and translation."
 authors = ["sam <contact@justsam.io>"]
 
 packages = [
     { include = "translate", from="." },
 ]
 exclude = ["translate/client"]
```

### Comparing `melon_translate-0.9.3/translate/core/settings.py` & `melon_translate-0.9.4/translate/core/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from pathlib import Path
 
 from decouple import config
 
+from translate.service.utils.version_handler import extract_version
+
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
+VERSION_TAG = extract_version()
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.0/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "django-insecure-yq@*8hm7=0d1mi@lqnnmh$qalu0uv0@m1a0e!_1o09wt%++4^k"
 
@@ -165,15 +168,15 @@
     "DEFAULT_PAGINATION_CLASS": "translate.service.paginations.TranslateClientPagination",
     "PAGE_SIZE": 500,  # default value if not set in paginator
 }
 
 SPECTACULAR_SETTINGS = {
     "TITLE": "melon-translate",
     "DESCRIPTION": "Translation microservice",
-    "VERSION": "0.9.3",
+    "VERSION": VERSION_TAG,
 }
 
 BATON = {
     "SITE_HEADER": "Melon-translate",
     "SITE_TITLE": "Melon-translate",
     "INDEX_TITLE": "Translations administration",
     "SUPPORT_HREF": "https://github.com/",
```

### Comparing `melon_translate-0.9.3/translate/core/urls.py` & `melon_translate-0.9.4/translate/core/urls.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/admin.py` & `melon_translate-0.9.4/translate/service/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 @admin.register(Translation)
 class TranslationAdmin(admin.ModelAdmin):
     """Admin registration for ``Translation``."""
 
     formfield_overrides = {models.TextField: {"widget": TextInput()}}
-    search_fields = ("key__snake_name",)
+    search_fields = ("key__snake_name", "key__id_name", "translation")
     fields = ("translation", "translation_plural", "language")
 
     list_display = ("key", "translation", "translation_plural", "language")
     list_filter = (
         "language",
         ("translation", admin.EmptyFieldListFilter),
         "key__category",
@@ -43,15 +43,15 @@
 @admin.register(TranslationKey)
 class TranslationKeyAdmin(admin.ModelAdmin):
     """Admin registration for ``TranslationKey.``"""
 
     formfield_overrides = {models.TextField: {"widget": TextInput()}}
     fields = ("snake_name", "id_name", "usage_context", "category", "views", "occurrences")
     inlines = (TranslationInline,)
-    search_fields = ("snake_name",)
+    search_fields = ("snake_name", "id_name")
 
     list_display = ("snake_name", "id_name", "usage_context", "category")
     list_filter = (
         "category",
         "created",
         "modified",
         IgnoreMimoKeysFilter,
```

### Comparing `melon_translate-0.9.3/translate/service/filters.py` & `melon_translate-0.9.4/translate/service/filters.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/management/commands/delete_no_context_keys.py` & `melon_translate-0.9.4/translate/service/management/commands/delete_no_context_keys.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/management/commands/export_csv.py` & `melon_translate-0.9.4/translate/service/management/commands/export_csv.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/management/commands/import_csv.py` & `melon_translate-0.9.4/translate/service/management/commands/import_csv.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/management/commands/import_translations.py` & `melon_translate-0.9.4/translate/service/management/commands/import_translations.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,34 +34,14 @@
         parser.add_argument(
             "translations_dir",
             type=str,
             nargs="?",
             default=DEFAULT_DIR_PATH,
         )
 
-        # parser.add_argument(
-        #     "-f",
-        #     "--force",
-        #     action="store_true",
-        #     help="Skips sanity checks and imports all items",
-        # ) will be added in follow up
-
-    @staticmethod
-    def po_keys_sanity_check(obj_keys):
-        """
-        This method returns a QuerySet of already imported translations
-        """
-        key_ids = []
-        for key in obj_keys:
-            key_ids.append(key.id_name)
-
-        already_existing_keys = TranslationKey.objects.filter(id_name__in=key_ids)
-        log.info(f"Already existing po keys: {len(already_existing_keys)}")
-        return already_existing_keys
-
     @staticmethod
     def read_po_files(dirs) -> dict:
         """Read po files."""
         log.info("Reading po files.")
         po_files = {
             po_file: polib.pofile(po_file, encoding="utf-8")
             for po_file in glob.iglob(f"{dirs}/**/*.po", recursive=True)
@@ -72,116 +52,100 @@
             lang = extract_language(file_path)
             files_with_languages[lang].append((file_path, file))
 
         log.info("Done")
         return files_with_languages
 
     @staticmethod
-    def create_po_keys(file_path, file_entries):
+    def create_po_keys(file_entries):
         """Create po keys."""
-        entries = [
-            TranslationKey(
+
+        existing_po_keys = {key.id_name: key for key in TranslationKey.objects.all()}
+
+        new_po_keys = {
+            entry.msgid: TranslationKey(
                 id_name=entry.msgid,
                 id_name_plural=entry.msgid_plural,
                 encoding=entry.encoding,
                 usage_context=entry.msgctxt,
                 occurrences=sorted(map(operator.itemgetter(0), entry.occurrences)),
                 flags=entry.flags,
             )
             for entry in file_entries
-        ]
+            if entry.msgid not in existing_po_keys.keys()
+        }
 
-        return entries
+        return existing_po_keys, new_po_keys
 
     @staticmethod
-    def create_po_translations(file_path, file_entries, key_entries, language):
-        """Import po translations."""
+    def create_po_translations(file_entries, key_entries, language) -> list:
+        """Create po translations."""
+
         entries = [
             Translation(
                 language=language,
-                key=key_entries[idx],
+                key=key_entries.get(entry.msgid),
                 translation=entry.msgstr if entry.msgstr else entry.msgid,
                 translation_plural=entry.msgid_plural,
             )
-            for idx, entry in enumerate(file_entries)
+            for entry in file_entries
         ]
 
         return entries
 
     @staticmethod
     def process_po_files(dirs):
         """Process po files."""
         po_files = Command.read_po_files(dirs)
 
-        raw_key_entries, translations = [], []
+        existing_keys, new_key_entries = {}, {}
         for lang, files in sorted(po_files.items()):
-            language, _ = Language.objects.get_or_create(lang_info=lang)
             for file_path, file_entries in files:
-                raw_key_entries += Command.create_po_keys(file_path, file_entries)
-                translations += Command.create_po_translations(file_path, file_entries, raw_key_entries, language)
-
-        log.info(f"Prepared {len(raw_key_entries)} of RAW TranslationKeys via po files.")
-        log.info("Cleaning...")
-        uniq = {}
-        duplicate_counter = 0
-        for key in raw_key_entries:
-            if key.id_name in uniq.keys():
-                duplicate_counter += 1
-            else:
-                uniq[key.id_name] = key
-
-        log.info(f"Duplicate ID_NAME occurred with {duplicate_counter} TranslationKeys.")
+                d1, d2 = Command.create_po_keys(file_entries)
+                existing_keys = {**existing_keys, **d1}
+                new_key_entries = {**new_key_entries, **d2}
 
-        bulk_inserts = uniq
-        already_imported_keys = Command.po_keys_sanity_check(uniq.values())
+        log.info(f"Found {len(existing_keys.items())} already existing TranslationKeys.")
+        log.info(f"Prepared {len(new_key_entries.items())} of new TranslationKeys via po files.")
 
-        if not already_imported_keys:
-            log.info("NO ALREADY IMPORTED KEYS FOUND!")
-        else:
-            for key in already_imported_keys:
-                if key.id_name in uniq.keys():
-                    bulk_inserts.pop(key.id_name)
-
-        inserts = TranslationKey.objects.bulk_create(bulk_inserts.values(), ignore_conflicts=True)
+        inserts = TranslationKey.objects.bulk_create(new_key_entries.values(), ignore_conflicts=True)
         if not inserts:
             log.info("NO NEW PO TRANSLATIONS HAVE BEEN ADDED")
-        log.info(f"Done. Inserted {len(inserts)} po TranslationKeys.")
+        else:
+            log.info(f"Done. Inserted {len(inserts)} TranslationKeys from po files.")
         log.info("----------------------------------------------------")
 
-        log.info(f"Prepared {len(translations)} of RAW Translations via po files.")
-
-        translation_inserts = []
-        uniq_id_names = set(uniq.keys())  # uniq dictionary keys are id_names
+        all_keys = {**existing_keys, **new_key_entries}
 
-        log.info("Cleaning!")
-        for translation_obj in translations:
-            if translation_obj.translation in uniq_id_names:
-                translation_inserts.append(translation_obj)
-
-        # translation_inserts = translations this will be used later for force argument
+        translations = defaultdict(list)
+        for lang, files in sorted(po_files.items()):
+            language, _ = Language.objects.get_or_create(lang_info=lang)
+            for file_path, file_entries in files:
+                translations[lang].extend(Command.create_po_translations(file_entries, all_keys, language))
 
-        integrity_errors = 0
-        try:
-            log.info(f"Prepared {len(translation_inserts)} of Translations. Inserting bulk... ")
-            translation_inserts = Translation.objects.bulk_create(translation_inserts, ignore_conflicts=True)
-        except django.db.utils.IntegrityError:
-            log.info("Integrity error occurred, and bulk create was canceled! Inserting individually...")
+        for lang, translations_list in translations.items():
             translation_inserts = []
-            for obj in translations:
-                if obj.translation in uniq.keys():
+            integrity_errors = 0
+            try:
+                log.info(f"Prepared {len(translations_list)} Translations for {lang} language. Inserting bulk... ")
+                translation_inserts = Translation.objects.bulk_create(translations_list, ignore_conflicts=True)
+            except django.db.utils.IntegrityError:
+                log.info("Integrity error occurred, and bulk create was canceled! Inserting individually...")
+                for obj in translations_list:
                     try:
                         obj.save()
                         translation_inserts.append(obj)
                     except django.db.utils.IntegrityError:
                         integrity_errors += 1
 
-        log.info(f"Integrity error occurred with {integrity_errors} Translations.")
-        if not translation_inserts:
-            log.info("NO NEW PO TRANSLATIONS HAVE BEEN ADDED")
-        log.info(f"Done. Inserted {len(translation_inserts)} po Translations.")
+            log.info(f"Integrity error occurred with {integrity_errors} Translations for {lang} language.")
+            if not translation_inserts:
+                log.info("NO NEW PO TRANSLATIONS HAVE BEEN ADDED")
+            log.info(f"Done. Inserted {len(translation_inserts)} Translations from po files for {lang} language.")
+            log.info("----------------------------------------------------")
 
     @staticmethod
     def create_json_keys(language_data, language_code):
         """Create language data."""
         log.info("Preparing translation keys.")
         keys = [
             TranslationKey(
@@ -278,13 +242,12 @@
 
         for lang in translations:
             _ = Command.create_json_keys(translations.get(lang), lang)
             _ = Command.create_json_translations(translations, lang)
 
     def handle(self, *args, **options):
         """Entrypoint to the command."""
-        # force = options.get("force")
 
         dir_name = Path(settings.BASE_DIR.parent, options.get("translations_dir"))
 
         Command.process_json_files(dir_name)
         Command.process_po_files(dir_name)
```

### Comparing `melon_translate-0.9.3/translate/service/migrations/0001_initial.py` & `melon_translate-0.9.4/translate/service/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/migrations/0002_alter_translation_key_alter_translation_language.py` & `melon_translate-0.9.4/translate/service/migrations/0002_alter_translation_key_alter_translation_language.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/migrations/0003_translationkey_occ_views_gin.py` & `melon_translate-0.9.4/translate/service/migrations/0003_translationkey_occ_views_gin.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/models.py` & `melon_translate-0.9.4/translate/service/models.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/paginations.py` & `melon_translate-0.9.4/translate/service/paginations.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/serializers.py` & `melon_translate-0.9.4/translate/service/serializers.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/static/assets/favicon.ico` & `melon_translate-0.9.4/translate/service/static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/static/assets/img/swiss.jpeg` & `melon_translate-0.9.4/translate/service/static/assets/img/swiss.jpeg`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/static/assets/img/swiss_flg.jpeg` & `melon_translate-0.9.4/translate/service/static/assets/img/swiss_flg.jpeg`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/static/css/style.css` & `melon_translate-0.9.4/translate/service/static/css/style.css`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/static/js/scripts.js` & `melon_translate-0.9.4/translate/service/static/js/scripts.js`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/templates/index.html` & `melon_translate-0.9.4/translate/service/templates/index.html`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/factories.py` & `melon_translate-0.9.4/translate/service/tests/factories.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/fixtures/french_fixtures/locale/fr/LC_MESSAGES/django.po` & `melon_translate-0.9.4/translate/service/tests/fixtures/french_fixtures/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/fixtures/french_fixtures/snake_translations.json` & `melon_translate-0.9.4/translate/service/tests/fixtures/french_fixtures/snake_translations.json`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/fixtures/german_fixtures/locale/de/LC_MESSAGES/django.po` & `melon_translate-0.9.4/translate/service/tests/fixtures/german_fixtures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/fixtures/german_fixtures/snake_translations.json` & `melon_translate-0.9.4/translate/service/tests/fixtures/german_fixtures/snake_translations.json`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/fixtures/import_csv_test_fixture.csv` & `melon_translate-0.9.4/translate/service/tests/fixtures/import_csv_test_fixture.csv`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/providers.py` & `melon_translate-0.9.4/translate/service/tests/providers.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/pytest_fixtures.py` & `melon_translate-0.9.4/translate/service/tests/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/test_commands.py` & `melon_translate-0.9.4/translate/service/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         from translate.service.models import Language, Translation, TranslationKey
 
         languages = Language.objects.all()
         translations = Translation.objects.all()
         keys = TranslationKey.objects.all()
 
         assert len(languages) == 1
-        assert len(translations) == 8
+        assert len(translations) == 9
         assert len(keys) == 9
 
         for key in keys:
             assert key.usage_context is None, "All imported keys should not have context"
             TranslationKey.objects.filter(id=key.id).update(usage_context="Add some new context")
             key.refresh_from_db()
 
@@ -47,15 +47,15 @@
 
         reloaded_keys = TranslationKey.objects.all()
         for key in reloaded_keys:
             assert key.usage_context == "Add some new context", "Context should not be overwritten by same import"
 
         # recall of the command should not insert any new keys
         assert len(languages) == 1
-        assert len(translations) == 8, "Translations number should stay the same"
+        assert len(translations) == 9, "Translations number should stay the same"
         assert len(keys) == 9, "Keys number should stayed the same"
 
         # cleanup
         Translation.objects.all().delete()
         TranslationKey.objects.all().delete()
         Language.objects.all().delete()
 
@@ -65,15 +65,15 @@
     def test_objects_deletion(self, import_german_translations_fixture):
         """Check deletion of translation keys with no usage_context."""
         from translate.service.models import Translation, TranslationKey
 
         record = Translation.objects.all()
         key_record = TranslationKey.objects.all()
 
-        assert len(record) == 8
+        assert len(record) == 9
         assert len(key_record) == 9
 
         for key in key_record:
             assert key.usage_context is None
 
         call_command("delete_no_context_keys")
 
@@ -85,26 +85,26 @@
     def test_skipping_keys_with_context(self, import_german_translations_fixture):
         """Test not deleting key with usage_context"""
         from translate.service.models import Translation, TranslationKey
 
         record = Translation.objects.all()
         key_record = TranslationKey.objects.all()
 
-        assert len(record) == 8
+        assert len(record) == 9
         assert len(key_record) == 9
 
         # Add usage context for every imported key
         for key in key_record:
             TranslationKey.objects.filter(id=key.id).update(usage_context="Add some new context")
             key.refresh_from_db()
 
         # call the command
         call_command("delete_no_context_keys")
 
-        assert len(record) == 8, "Translation count should stay same after calling of command"
+        assert len(record) == 9, "Translation count should stay same after calling of command"
         assert len(key_record) == 9, "TranslationKeys count should stay same after calling of command"
 
 
 class TestCSV:
     @pytest.mark.command
     def test_export_csv_file_creation(self, export_csv_fixture):
         """Imports data into database and then export it as a CSV file"""
@@ -136,17 +136,17 @@
 
         from translate.service.models import Translation, TranslationKey
 
         all_keys = TranslationKey.objects.all()
         all_translations = Translation.objects.all()
 
         assert len(all_keys) == 18
-        assert len(all_translations) == 11
+        assert len(all_translations) == 18
 
         fixture = Path("translate/service/tests/fixtures/import_csv_test_fixture.csv")
         call_command("import_csv", fixture)
 
         all_keys = TranslationKey.objects.all()
         all_translations = Translation.objects.all()
 
         assert len(all_keys) == 18, "Import command should not add new keys, only update existing ones"
-        assert len(all_translations) == 11, "Import command should not add new translations, only update existing ones"
+        assert len(all_translations) == 18, "Import command should not add new translations, only update existing ones"
```

### Comparing `melon_translate-0.9.3/translate/service/tests/test_filters.py` & `melon_translate-0.9.4/translate/service/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/test_models.py` & `melon_translate-0.9.4/translate/service/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/test_paginations.py` & `melon_translate-0.9.4/translate/service/tests/test_paginations.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/test_serializers.py` & `melon_translate-0.9.4/translate/service/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/tests/test_views.py` & `melon_translate-0.9.4/translate/service/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/translate/service/views.py` & `melon_translate-0.9.4/translate/service/views.py`

 * *Files identical despite different names*

### Comparing `melon_translate-0.9.3/setup.py` & `melon_translate-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 ['translate',
  'translate.core',
  'translate.core.utils',
  'translate.service',
  'translate.service.management',
  'translate.service.management.commands',
  'translate.service.migrations',
- 'translate.service.tests']
+ 'translate.service.tests',
+ 'translate.service.utils']
 
 package_data = \
 {'': ['*'],
  'translate.service': ['static/assets/*',
                        'static/assets/img/*',
                        'static/css/*',
                        'static/js/*',
@@ -42,15 +43,15 @@
  'python-decouple>=3.5,<4.0',
  'python-dotenv>=0.20.0,<0.21.0',
  'redis>=4.3.4,<5.0.0',
  'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'melon-translate',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Melon-translate is a micro service for easing localisation and translation.',
     'long_description': 'None',
     'author': 'sam',
     'author_email': 'contact@justsam.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `melon_translate-0.9.3/PKG-INFO` & `melon_translate-0.9.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melon-translate
-Version: 0.9.3
+Version: 0.9.4
 Summary: Melon-translate is a micro service for easing localisation and translation.
 Author: sam
 Author-email: contact@justsam.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


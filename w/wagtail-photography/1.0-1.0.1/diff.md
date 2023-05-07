# Comparing `tmp/wagtail-photography-1.0.tar.gz` & `tmp/wagtail-photography-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-photography-1.0.tar", last modified: Sun May  7 22:05:19 2023, max compression
+gzip compressed data, was "wagtail-photography-1.0.1.tar", last modified: Sun May  7 23:29:35 2023, max compression
```

## Comparing `wagtail-photography-1.0.tar` & `wagtail-photography-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/
--rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-1.0/LICENSE
--rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-1.0/MANIFEST.in
--rw-rw-r--   0 ave       (1000) ave       (1000)     3038 2023-05-07 22:05:19.745564 wagtail-photography-1.0/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)     2022 2023-05-07 21:54:01.000000 wagtail-photography-1.0/README.md
--rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-1.0/pyproject.toml
--rw-rw-r--   0 ave       (1000) ave       (1000)     1061 2023-05-07 22:05:19.745564 wagtail-photography-1.0/setup.cfg
--rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-1.0/setup.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/apps.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1372 2023-05-07 21:39:01.000000 wagtail-photography-1.0/wagtail_photography/blocks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/forms.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography/migrations/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/migrations/0001_initial.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      814 2023-05-07 18:26:53.000000 wagtail-photography-1.0/wagtail_photography/migrations/0002_remove_albumimage_height_remove_albumimage_width_and_more.py
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/migrations/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     5110 2023-05-07 18:18:36.000000 wagtail-photography-1.0/wagtail_photography/models.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/static/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-1.0/wagtail_photography/static/app.js
--rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-1.0/wagtail_photography/static/photo_gallery.css
--rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.css
--rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.js
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography/templates/
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/templates/includes/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/templates/includes/photo_swipe.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1378 2023-04-30 05:36:56.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/album_detail.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/blocks/
--rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/blocks/photo_gallery.html
--rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-05-07 20:35:54.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_css.html
--rw-rw-r--   0 ave       (1000) ave       (1000)     1106 2023-04-30 05:36:56.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_js.html
--rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/tests.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/views.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/wagtail_hooks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/widgets.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography.egg-info/
--rw-rw-r--   0 ave       (1000) ave       (1000)     3038 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)     1248 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/SOURCES.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/dependency_links.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       54 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/requires.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/top_level.txt
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-1.0.1/LICENSE
+-rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-1.0.1/MANIFEST.in
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3040 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2022 2023-05-07 21:54:01.000000 wagtail-photography-1.0.1/README.md
+-rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-1.0.1/pyproject.toml
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1063 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/setup.cfg
+-rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-1.0.1/setup.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-1.0.1/wagtail_photography/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-1.0.1/wagtail_photography/apps.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1392 2023-05-07 23:28:57.000000 wagtail-photography-1.0.1/wagtail_photography/blocks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-1.0.1/wagtail_photography/forms.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/wagtail_photography/migrations/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-1.0.1/wagtail_photography/migrations/0001_initial.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      814 2023-05-07 18:26:53.000000 wagtail-photography-1.0.1/wagtail_photography/migrations/0002_remove_albumimage_height_remove_albumimage_width_and_more.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-1.0.1/wagtail_photography/migrations/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     5110 2023-05-07 18:18:36.000000 wagtail-photography-1.0.1/wagtail_photography/models.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/wagtail_photography/static/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-1.0.1/wagtail_photography/static/app.js
+-rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-1.0.1/wagtail_photography/static/photo_gallery.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-1.0.1/wagtail_photography/static/photo_gallery_admin.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-1.0.1/wagtail_photography/static/photo_gallery_admin.js
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.259869 wagtail-photography-1.0.1/wagtail_photography/templates/
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/wagtail_photography/templates/includes/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-1.0.1/wagtail_photography/templates/includes/photo_swipe.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1378 2023-04-30 05:36:56.000000 wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/album_detail.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/blocks/
+-rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/blocks/photo_gallery.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-05-07 20:35:54.000000 wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/extra_css.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1106 2023-04-30 05:36:56.000000 wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/extra_js.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-1.0.1/wagtail_photography/tests.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-1.0.1/wagtail_photography/views.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-1.0.1/wagtail_photography/wagtail_hooks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-1.0.1/wagtail_photography/widgets.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 23:29:35.263869 wagtail-photography-1.0.1/wagtail_photography.egg-info/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3040 2023-05-07 23:29:35.000000 wagtail-photography-1.0.1/wagtail_photography.egg-info/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1248 2023-05-07 23:29:35.000000 wagtail-photography-1.0.1/wagtail_photography.egg-info/SOURCES.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-05-07 23:29:35.000000 wagtail-photography-1.0.1/wagtail_photography.egg-info/dependency_links.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       54 2023-05-07 23:29:35.000000 wagtail-photography-1.0.1/wagtail_photography.egg-info/requires.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-05-07 23:29:35.000000 wagtail-photography-1.0.1/wagtail_photography.egg-info/top_level.txt
```

### Comparing `wagtail-photography-1.0/LICENSE` & `wagtail-photography-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/PKG-INFO` & `wagtail-photography-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 1.0
+Version: 1.0.1
 Summary: A Wagtail app to display photographs
 Home-page: https://github.com/TechnoConserve/wagtail-photography
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
```

### Comparing `wagtail-photography-1.0/README.md` & `wagtail-photography-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/setup.cfg` & `wagtail-photography-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-photography
-version = 1.0
+version = 1.0.1
 description = A Wagtail app to display photographs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TechnoConserve/wagtail-photography
 author = Avery Uslaner
 author_email = uslaner.avery@gmail.com
 license = Apache License 2.0
```

### Comparing `wagtail-photography-1.0/wagtail_photography/blocks.py` & `wagtail-photography-1.0.1/wagtail_photography/blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class GalleryBlock(blocks.StructBlock):
     album_class = 'wagtail_photography.Album'
 
     title = blocks.CharBlock()
     collection = CollectionChooserBlock()
 
     class Meta:
-        template = 'blocks/photo_gallery.html'
+        template = 'wagtail_photography/blocks/photo_gallery.html'
         icon = 'image'
 
     @property
     def target_model(self):
         return resolve_model_string(self.album_class)
 
     def filter_albums(self, value):
```

### Comparing `wagtail-photography-1.0/wagtail_photography/forms.py` & `wagtail-photography-1.0.1/wagtail_photography/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/migrations/0001_initial.py` & `wagtail-photography-1.0.1/wagtail_photography/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/migrations/0002_remove_albumimage_height_remove_albumimage_width_and_more.py` & `wagtail-photography-1.0.1/wagtail_photography/migrations/0002_remove_albumimage_height_remove_albumimage_width_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/models.py` & `wagtail-photography-1.0.1/wagtail_photography/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/static/app.js` & `wagtail-photography-1.0.1/wagtail_photography/static/app.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.css` & `wagtail-photography-1.0.1/wagtail_photography/static/photo_gallery_admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.js` & `wagtail-photography-1.0.1/wagtail_photography/static/photo_gallery_admin.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/templates/includes/photo_swipe.html` & `wagtail-photography-1.0.1/wagtail_photography/templates/includes/photo_swipe.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/album_detail.html` & `wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/album_detail.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/blocks/photo_gallery.html` & `wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/blocks/photo_gallery.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_css.html` & `wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/extra_css.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_js.html` & `wagtail-photography-1.0.1/wagtail_photography/templates/wagtail_photography/extra_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/wagtail_hooks.py` & `wagtail-photography-1.0.1/wagtail_photography/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography/widgets.py` & `wagtail-photography-1.0.1/wagtail_photography/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-1.0/wagtail_photography.egg-info/PKG-INFO` & `wagtail-photography-1.0.1/wagtail_photography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 1.0
+Version: 1.0.1
 Summary: A Wagtail app to display photographs
 Home-page: https://github.com/TechnoConserve/wagtail-photography
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
```

### Comparing `wagtail-photography-1.0/wagtail_photography.egg-info/SOURCES.txt` & `wagtail-photography-1.0.1/wagtail_photography.egg-info/SOURCES.txt`

 * *Files identical despite different names*


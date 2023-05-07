# Comparing `tmp/wagtail-photography-0.4.tar.gz` & `tmp/wagtail-photography-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-photography-0.4.tar", last modified: Sun May  7 18:00:36 2023, max compression
+gzip compressed data, was "wagtail-photography-1.0.tar", last modified: Sun May  7 22:05:19 2023, max compression
```

## Comparing `wagtail-photography-0.4.tar` & `wagtail-photography-1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/
--rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-0.4/LICENSE
--rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-0.4/MANIFEST.in
--rw-rw-r--   0 ave       (1000) ave       (1000)     2291 2023-05-07 18:00:36.914357 wagtail-photography-0.4/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)     1375 2023-05-07 17:24:51.000000 wagtail-photography-0.4/README.md
--rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-0.4/pyproject.toml
--rw-rw-r--   0 ave       (1000) ave       (1000)      983 2023-05-07 18:00:36.914357 wagtail-photography-0.4/setup.cfg
--rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-0.4/setup.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/apps.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1372 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/blocks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/forms.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/migrations/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/migrations/0001_initial.py
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/migrations/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     5147 2023-04-30 05:36:56.000000 wagtail-photography-0.4/wagtail_photography/models.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/static/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-0.4/wagtail_photography/static/app.js
--rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-0.4/wagtail_photography/static/photo_gallery.css
--rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.css
--rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.js
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.910357 wagtail-photography-0.4/wagtail_photography/templates/
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/templates/blocks/
--rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/templates/blocks/photo_gallery.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/templates/includes/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/templates/includes/photo_swipe.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1378 2023-04-30 05:36:56.000000 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/album_detail.html
--rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_css.html
--rw-rw-r--   0 ave       (1000) ave       (1000)     1106 2023-04-30 05:36:56.000000 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_js.html
--rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/tests.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/views.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/wagtail_hooks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/widgets.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography.egg-info/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2291 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)     1131 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/SOURCES.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/dependency_links.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       54 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/requires.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/top_level.txt
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-1.0/LICENSE
+-rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-1.0/MANIFEST.in
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3038 2023-05-07 22:05:19.745564 wagtail-photography-1.0/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2022 2023-05-07 21:54:01.000000 wagtail-photography-1.0/README.md
+-rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-1.0/pyproject.toml
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1061 2023-05-07 22:05:19.745564 wagtail-photography-1.0/setup.cfg
+-rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-1.0/setup.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/apps.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1372 2023-05-07 21:39:01.000000 wagtail-photography-1.0/wagtail_photography/blocks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/forms.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography/migrations/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/migrations/0001_initial.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      814 2023-05-07 18:26:53.000000 wagtail-photography-1.0/wagtail_photography/migrations/0002_remove_albumimage_height_remove_albumimage_width_and_more.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/migrations/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     5110 2023-05-07 18:18:36.000000 wagtail-photography-1.0/wagtail_photography/models.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/static/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-1.0/wagtail_photography/static/app.js
+-rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-1.0/wagtail_photography/static/photo_gallery.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.js
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography/templates/
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/templates/includes/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/templates/includes/photo_swipe.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1378 2023-04-30 05:36:56.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/album_detail.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.745564 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/blocks/
+-rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/blocks/photo_gallery.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-05-07 20:35:54.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_css.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1106 2023-04-30 05:36:56.000000 wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_js.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-1.0/wagtail_photography/tests.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/views.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/wagtail_hooks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-1.0/wagtail_photography/widgets.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 22:05:19.741564 wagtail-photography-1.0/wagtail_photography.egg-info/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3038 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1248 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/SOURCES.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/dependency_links.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       54 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/requires.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-05-07 22:05:19.000000 wagtail-photography-1.0/wagtail_photography.egg-info/top_level.txt
```

### Comparing `wagtail-photography-0.4/LICENSE` & `wagtail-photography-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/PKG-INFO` & `wagtail-photography-1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 0.4
+Version: 1.0
 Summary: A Wagtail app to display photographs
 Home-page: https://github.com/TechnoConserve/wagtail-photography
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## Wagtail Photography
 
 
 Based on [wagtail-photo-gallery](https://github.com/donhauser/wagtail-photo-gallery)
 
-Be warned, this project is still kinda garbage. Mostly I'm just messing about with it but I do hope to polish it up in
-the not so distant future.
+Be warned, I'm mostly using this project as a learning experience for developing and distributing apps. I'm new at it so
+things are likely to be broken or break in the future. I use it in production on my own website but would advise against
+doing the same if reliability is important to you. I do hope to add tests and generally polish things up in the not so 
+distant future.
 
 Wagtail-photography is a Wagtail app to display photographs.
 
 Detailed documentation is in the "docs" directory.
 
 Quick start
 -----------
@@ -43,16 +47,18 @@
    ```pip install wagtail-photography```
 
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
       ...
-      "generic_chooser",
+      "wagtail.contrib.modeladmin",
+      "wagtail.contrib.routable_page",
       "wagtail_photography",
+      "generic_chooser",
    ]
    ```
 
 3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
 
    ```python
    from wagtail.images.views.serve import ServeView
@@ -64,12 +70,23 @@
    
        ...
    
        # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
        re_path(r'', include(wagtail_urls)),
    ]
    ```
+4. Create a Page model that inherits from `PhotoGalleryMixin`:
+   ```python
+   class PhotoGallery(PhotoGalleryMixin, Page):
+       content = StreamField([
+           ("gallery", GalleryBlock()),
+       ], blank=True, use_json_field=True)
+   
+       content_panels = Page.content_panels + [
+           FieldPanel("content"),
+       ]
+   ```
    
-4. Run ``python manage.py migrate`` to create the wagtail_photography models.
+5. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
-5. Start the development server and visit http://127.0.0.1:8000/admin/
+6. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.4/setup.cfg` & `wagtail-photography-1.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-photography
-version = 0.4
+version = 1.0
 description = A Wagtail app to display photographs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TechnoConserve/wagtail-photography
 author = Avery Uslaner
 author_email = uslaner.avery@gmail.com
 license = Apache License 2.0
@@ -14,14 +14,16 @@
 	Framework :: Wagtail :: 4
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
```

### Comparing `wagtail-photography-0.4/wagtail_photography/blocks.py` & `wagtail-photography-1.0/wagtail_photography/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/forms.py` & `wagtail-photography-1.0/wagtail_photography/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/migrations/0001_initial.py` & `wagtail-photography-1.0/wagtail_photography/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/models.py` & `wagtail-photography-1.0/wagtail_photography/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import copy
 import itertools
-import json
 import uuid
 
-from django import forms
 from django.db import models
 from django.http import Http404
 from django.shortcuts import render
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
 from wagtail.admin.panels import FieldPanel, MultiFieldPanel, HelpPanel, TabbedInterface, ObjectList, InlinePanel
 from wagtail.contrib.routable_page.models import RoutablePageMixin, route
```

### Comparing `wagtail-photography-0.4/wagtail_photography/static/app.js` & `wagtail-photography-1.0/wagtail_photography/static/app.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.css` & `wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.js` & `wagtail-photography-1.0/wagtail_photography/static/photo_gallery_admin.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/templates/blocks/photo_gallery.html` & `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/blocks/photo_gallery.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/templates/includes/photo_swipe.html` & `wagtail-photography-1.0/wagtail_photography/templates/includes/photo_swipe.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/album_detail.html` & `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/album_detail.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_css.html` & `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_css.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_js.html` & `wagtail-photography-1.0/wagtail_photography/templates/wagtail_photography/extra_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/wagtail_hooks.py` & `wagtail-photography-1.0/wagtail_photography/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography/widgets.py` & `wagtail-photography-1.0/wagtail_photography/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.4/wagtail_photography.egg-info/PKG-INFO` & `wagtail-photography-1.0/wagtail_photography.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 0.4
+Version: 1.0
 Summary: A Wagtail app to display photographs
 Home-page: https://github.com/TechnoConserve/wagtail-photography
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## Wagtail Photography
 
 
 Based on [wagtail-photo-gallery](https://github.com/donhauser/wagtail-photo-gallery)
 
-Be warned, this project is still kinda garbage. Mostly I'm just messing about with it but I do hope to polish it up in
-the not so distant future.
+Be warned, I'm mostly using this project as a learning experience for developing and distributing apps. I'm new at it so
+things are likely to be broken or break in the future. I use it in production on my own website but would advise against
+doing the same if reliability is important to you. I do hope to add tests and generally polish things up in the not so 
+distant future.
 
 Wagtail-photography is a Wagtail app to display photographs.
 
 Detailed documentation is in the "docs" directory.
 
 Quick start
 -----------
@@ -43,16 +47,18 @@
    ```pip install wagtail-photography```
 
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
       ...
-      "generic_chooser",
+      "wagtail.contrib.modeladmin",
+      "wagtail.contrib.routable_page",
       "wagtail_photography",
+      "generic_chooser",
    ]
    ```
 
 3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
 
    ```python
    from wagtail.images.views.serve import ServeView
@@ -64,12 +70,23 @@
    
        ...
    
        # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
        re_path(r'', include(wagtail_urls)),
    ]
    ```
+4. Create a Page model that inherits from `PhotoGalleryMixin`:
+   ```python
+   class PhotoGallery(PhotoGalleryMixin, Page):
+       content = StreamField([
+           ("gallery", GalleryBlock()),
+       ], blank=True, use_json_field=True)
+   
+       content_panels = Page.content_panels + [
+           FieldPanel("content"),
+       ]
+   ```
    
-4. Run ``python manage.py migrate`` to create the wagtail_photography models.
+5. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
-5. Start the development server and visit http://127.0.0.1:8000/admin/
+6. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.4/wagtail_photography.egg-info/SOURCES.txt` & `wagtail-photography-1.0/wagtail_photography.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 wagtail_photography/widgets.py
 wagtail_photography.egg-info/PKG-INFO
 wagtail_photography.egg-info/SOURCES.txt
 wagtail_photography.egg-info/dependency_links.txt
 wagtail_photography.egg-info/requires.txt
 wagtail_photography.egg-info/top_level.txt
 wagtail_photography/migrations/0001_initial.py
+wagtail_photography/migrations/0002_remove_albumimage_height_remove_albumimage_width_and_more.py
 wagtail_photography/migrations/__init__.py
 wagtail_photography/static/app.js
 wagtail_photography/static/photo_gallery.css
 wagtail_photography/static/photo_gallery_admin.css
 wagtail_photography/static/photo_gallery_admin.js
-wagtail_photography/templates/blocks/photo_gallery.html
 wagtail_photography/templates/includes/photo_swipe.html
 wagtail_photography/templates/wagtail_photography/album_detail.html
 wagtail_photography/templates/wagtail_photography/extra_css.html
-wagtail_photography/templates/wagtail_photography/extra_js.html
+wagtail_photography/templates/wagtail_photography/extra_js.html
+wagtail_photography/templates/wagtail_photography/blocks/photo_gallery.html
```


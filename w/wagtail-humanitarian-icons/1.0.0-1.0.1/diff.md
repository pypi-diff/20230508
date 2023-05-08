# Comparing `tmp/wagtail-humanitarian-icons-1.0.0.tar.gz` & `tmp/wagtail-humanitarian-icons-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-humanitarian-icons-1.0.0.tar", last modified: Fri May  5 11:44:23 2023, max compression
+gzip compressed data, was "wagtail-humanitarian-icons-1.0.1.tar", last modified: Mon May  8 09:37:24 2023, max compression
```

## Comparing `wagtail-humanitarian-icons-1.0.0.tar` & `wagtail-humanitarian-icons-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:23.214855 wagtail-humanitarian-icons-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-05 11:44:23.214855 wagtail-humanitarian-icons-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-05 11:44:23.214855 wagtail-humanitarian-icons-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:23.210855 wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-05 11:44:23.000000 wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-05 11:44:23.000000 wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:44:23.000000 wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 11:44:23.000000 wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 11:44:23.000000 wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:23.210855 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:23.214855 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 11:44:02.000000 wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 09:37:24.199824 wagtail-humanitarian-icons-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.191823 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/icons.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/widgets.py
```

### Comparing `wagtail-humanitarian-icons-1.0.0/PKG-INFO` & `wagtail-humanitarian-icons-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-humanitarian-icons
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ocha Humanitarian Icons, for use in  Wagtail projects, with an icon chooser widget.
 Home-page: https://github.com/wmo-raf/wagtail-humanitarian-icons
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-humanitarian-icons-1.0.0/README.md` & `wagtail-humanitarian-icons-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-humanitarian-icons-1.0.0/setup.cfg` & `wagtail-humanitarian-icons-1.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-humanitarian-icons
-version = 1.0.0
+version = 1.0.1
 description = Ocha Humanitarian Icons, for use in  Wagtail projects, with an icon chooser widget.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-humanitarian-icons
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
@@ -23,11 +23,14 @@
 [options]
 packages = find:
 include_package_data = true
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
 
+[options.package_data]
+* = *.json, static/*, templates/*
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/PKG-INFO` & `wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-humanitarian-icons
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ocha Humanitarian Icons, for use in  Wagtail projects, with an icon chooser widget.
 Home-page: https://github.com/wmo-raf/wagtail-humanitarian-icons
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-humanitarian-icons-1.0.0/wagtail_humanitarian_icons.egg-info/SOURCES.txt` & `wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 wagtail_humanitarian_icons.egg-info/SOURCES.txt
 wagtail_humanitarian_icons.egg-info/dependency_links.txt
 wagtail_humanitarian_icons.egg-info/requires.txt
 wagtail_humanitarian_icons.egg-info/top_level.txt
 wagtailhumanitarianicons/__init__.py
 wagtailhumanitarianicons/admin.py
 wagtailhumanitarianicons/apps.py
+wagtailhumanitarianicons/icons.json
 wagtailhumanitarianicons/models.py
 wagtailhumanitarianicons/tests.py
 wagtailhumanitarianicons/utils.py
 wagtailhumanitarianicons/views.py
 wagtailhumanitarianicons/wagtail_hooks.py
 wagtailhumanitarianicons/widgets.py
 wagtailhumanitarianicons/migrations/__init__.py
```

### Comparing `wagtail-humanitarian-icons-1.0.0/wagtailhumanitarianicons/utils.py` & `wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/utils.py`

 * *Files identical despite different names*


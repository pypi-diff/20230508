# Comparing `tmp/django-advanced-pages-0.8.4.tar.gz` & `tmp/django-advanced-pages-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-pages-0.8.4.tar", last modified: Wed Apr 12 19:41:20 2023, max compression
+gzip compressed data, was "django-advanced-pages-0.8.5.tar", last modified: Mon May  8 07:04:00 2023, max compression
```

## Comparing `django-advanced-pages-0.8.4.tar` & `django-advanced-pages-0.8.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 19:41:12.000000 django-advanced-pages-0.8.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.082033 django-advanced-pages-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/pages/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/fixtures/initial_pages.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/pages/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/0002_auto_20210609_2039.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/0003_auto_20210621_0847.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 07:03:53.000000 django-advanced-pages-0.8.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/pages/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/fixtures/initial_pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/src/pages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/0002_auto_20210609_2039.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/0003_auto_20210621_0847.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/urls.py
```

### Comparing `django-advanced-pages-0.8.4/LICENSE` & `django-advanced-pages-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/PKG-INFO` & `django-advanced-pages-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: django-advanced-pages
-Version: 0.8.4
+Version: 0.8.5
 Summary: Django flatpages with advanced features
+Home-page: https://github.com/snake-soft/django-advanced-pages
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
```

### Comparing `django-advanced-pages-0.8.4/README.rst` & `django-advanced-pages-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/setup.py` & `django-advanced-pages-0.8.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ]
 
 tests_require = [
 ]
 
 setup(
     name='django-advanced-pages',
+    url='https://github.com/snake-soft/django-advanced-pages',
     version=__version__,
     author="Snake-Soft",
     author_email="info@snake-soft.com",
     description="Django flatpages with advanced features",
     long_description=open('README.rst').read(),
     license='GPL3',
     package_dir={'': 'src'},
```

### Comparing `django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/PKG-INFO` & `django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: django-advanced-pages
-Version: 0.8.4
+Version: 0.8.5
 Summary: Django flatpages with advanced features
+Home-page: https://github.com/snake-soft/django-advanced-pages
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
```

### Comparing `django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/SOURCES.txt` & `django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/src/pages/admin.py` & `django-advanced-pages-0.8.5/src/pages/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/src/pages/fixtures/initial_pages.json` & `django-advanced-pages-0.8.5/src/pages/fixtures/initial_pages.json`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/src/pages/migrations/0001_initial.py` & `django-advanced-pages-0.8.5/src/pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/src/pages/migrations/0003_auto_20210621_0847.py` & `django-advanced-pages-0.8.5/src/pages/migrations/0003_auto_20210621_0847.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/src/pages/models.py` & `django-advanced-pages-0.8.5/src/pages/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/tests/manage.py` & `django-advanced-pages-0.8.5/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/tests/settings.py` & `django-advanced-pages-0.8.5/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.4/tests/test_models.py` & `django-advanced-pages-0.8.5/tests/test_models.py`

 * *Files identical despite different names*


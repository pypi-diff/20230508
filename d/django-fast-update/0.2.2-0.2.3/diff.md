# Comparing `tmp/django-fast-update-0.2.2.tar.gz` & `tmp/django-fast-update-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-fast-update-0.2.2.tar", last modified: Thu Apr 13 13:57:55 2023, max compression
+gzip compressed data, was "dist/django-fast-update-0.2.3.tar", last modified: Mon May  8 08:31:20 2023, max compression
```

## Comparing `django-fast-update-0.2.2.tar` & `django-fast-update-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1741 2023-04-13 12:40:03.000000 django-fast-update-0.2.2/setup.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/setup.cfg
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      120 2022-04-03 19:37:07.000000 django-fast-update-0.2.2/MANIFEST.in
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/fast_update/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    33274 2023-04-13 12:36:18.000000 django-fast-update-0.2.2/fast_update/copy.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2023-04-13 12:40:13.000000 django-fast-update-0.2.2/fast_update/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5411 2023-04-13 13:06:11.000000 django-fast-update-0.2.2/fast_update/query.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    13548 2022-04-30 18:22:51.000000 django-fast-update-0.2.2/fast_update/fast.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1024 2022-04-03 19:35:58.000000 django-fast-update-0.2.2/LICENSE.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     6017 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     4141 2023-04-13 13:36:58.000000 django-fast-update-0.2.2/README.md
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/dependency_links.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      346 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/SOURCES.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     6017 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       18 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/requires.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       12 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/top_level.txt
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-05-08 08:31:20.000000 django-fast-update-0.2.3/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1735 2023-05-08 08:25:43.000000 django-fast-update-0.2.3/setup.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2023-05-08 08:31:20.000000 django-fast-update-0.2.3/setup.cfg
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      120 2022-04-03 19:37:07.000000 django-fast-update-0.2.3/MANIFEST.in
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-05-08 08:31:20.000000 django-fast-update-0.2.3/fast_update/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    33274 2023-04-13 12:36:18.000000 django-fast-update-0.2.3/fast_update/copy.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2023-05-08 08:25:46.000000 django-fast-update-0.2.3/fast_update/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     5411 2023-04-13 13:59:03.000000 django-fast-update-0.2.3/fast_update/query.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    13548 2022-04-30 18:22:51.000000 django-fast-update-0.2.3/fast_update/fast.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1024 2022-04-03 19:35:58.000000 django-fast-update-0.2.3/LICENSE.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     6017 2023-05-08 08:31:20.000000 django-fast-update-0.2.3/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     4141 2023-04-13 13:59:03.000000 django-fast-update-0.2.3/README.md
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-05-08 08:31:20.000000 django-fast-update-0.2.3/django_fast_update.egg-info/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2023-05-08 08:31:19.000000 django-fast-update-0.2.3/django_fast_update.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      346 2023-05-08 08:31:19.000000 django-fast-update-0.2.3/django_fast_update.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     6017 2023-05-08 08:31:19.000000 django-fast-update-0.2.3/django_fast_update.egg-info/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       12 2023-05-08 08:31:19.000000 django-fast-update-0.2.3/django_fast_update.egg-info/requires.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       12 2023-05-08 08:31:19.000000 django-fast-update-0.2.3/django_fast_update.egg-info/top_level.txt
```

### Comparing `django-fast-update-0.2.2/setup.py` & `django-fast-update-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
                 return line.split(delim)[1]
         raise RuntimeError('Unable to find version string.')
 
 setup(
     name='django-fast-update',
     packages=find_packages(exclude=['example']),
     include_package_data=True,
-    install_requires=['Django>=3.2,<=4.2'],
+    install_requires=['Django>=3.2'],
     version=get_version('fast_update/__init__.py'),
     license='MIT',
     description='Faster db updates for Django using UPDATE FROM VALUES sql variants.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='netzkolchose',
     author_email='j.breitbart@netzkolchose.de',
     url='https://github.com/netzkolchose/django-fast-update',
-    download_url='https://github.com/netzkolchose/django-fast-update/archive/v0.2.2.tar.gz',
+    download_url='https://github.com/netzkolchose/django-fast-update/archive/v0.2.3.tar.gz',
     keywords=['django', 'bulk_update', 'fast', 'update', 'fast_update'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Database',
         'Topic :: Database :: Front-Ends',
         'Topic :: Software Development :: Libraries',
```

### Comparing `django-fast-update-0.2.2/fast_update/copy.py` & `django-fast-update-0.2.3/fast_update/copy.py`

 * *Files identical despite different names*

### Comparing `django-fast-update-0.2.2/fast_update/query.py` & `django-fast-update-0.2.3/fast_update/query.py`

 * *Files identical despite different names*

### Comparing `django-fast-update-0.2.2/fast_update/fast.py` & `django-fast-update-0.2.3/fast_update/fast.py`

 * *Files identical despite different names*

### Comparing `django-fast-update-0.2.2/LICENSE.txt` & `django-fast-update-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-fast-update-0.2.2/PKG-INFO` & `django-fast-update-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-fast-update
-Version: 0.2.2
+Version: 0.2.3
 Summary: Faster db updates for Django using UPDATE FROM VALUES sql variants.
 Home-page: https://github.com/netzkolchose/django-fast-update
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.2.tar.gz
+Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.3.tar.gz
 Description: [![test](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml/badge.svg?branch=master)](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml)
         [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-fast-update/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-fast-update?branch=master)
         
         
         ## django-fast-update ##
         
         Faster db updates using `UPDATE FROM VALUES` sql variants.
```

### Comparing `django-fast-update-0.2.2/README.md` & `django-fast-update-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django-fast-update-0.2.2/django_fast_update.egg-info/PKG-INFO` & `django-fast-update-0.2.3/django_fast_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-fast-update
-Version: 0.2.2
+Version: 0.2.3
 Summary: Faster db updates for Django using UPDATE FROM VALUES sql variants.
 Home-page: https://github.com/netzkolchose/django-fast-update
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.2.tar.gz
+Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.3.tar.gz
 Description: [![test](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml/badge.svg?branch=master)](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml)
         [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-fast-update/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-fast-update?branch=master)
         
         
         ## django-fast-update ##
         
         Faster db updates using `UPDATE FROM VALUES` sql variants.
```


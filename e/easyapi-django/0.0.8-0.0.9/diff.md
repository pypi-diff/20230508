# Comparing `tmp/easyapi_django-0.0.8.tar.gz` & `tmp/easyapi_django-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyapi_django-0.0.8.tar", last modified: Wed Feb 15 04:25:16 2023, max compression
+gzip compressed data, was "easyapi_django-0.0.9.tar", last modified: Wed Feb 15 04:27:28 2023, max compression
```

## Comparing `easyapi_django-0.0.8.tar` & `easyapi_django-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:25:16.314312 easyapi_django-0.0.8/
--rw-r--r--   0 ssjunior   (501) staff       (20)     1076 2023-02-11 03:15:42.000000 easyapi_django-0.0.8/LICENSE
--rw-r--r--   0 ssjunior   (501) staff       (20)     4535 2023-02-15 04:25:16.313884 easyapi_django-0.0.8/PKG-INFO
--rw-r--r--   0 ssjunior   (501) staff       (20)     3984 2023-02-11 17:19:30.000000 easyapi_django-0.0.8/README.md
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:25:16.311067 easyapi_django-0.0.8/easyapi/
--rw-r--r--   0 ssjunior   (501) staff       (20)      171 2023-02-11 04:59:19.000000 easyapi_django-0.0.8/easyapi/__init__.py
--rw-r--r--   0 ssjunior   (501) staff       (20)    23873 2023-02-15 04:24:37.000000 easyapi_django-0.0.8/easyapi/base.py
--rw-r--r--   0 ssjunior   (501) staff       (20)      231 2022-11-04 05:07:41.000000 easyapi_django-0.0.8/easyapi/exception.py
--rw-r--r--   0 ssjunior   (501) staff       (20)    25731 2023-02-15 04:17:48.000000 easyapi_django-0.0.8/easyapi/filters.py
--rw-r--r--   0 ssjunior   (501) staff       (20)      383 2023-02-11 03:26:51.000000 easyapi_django-0.0.8/easyapi/middleware.py
--rw-r--r--   0 ssjunior   (501) staff       (20)      982 2023-02-11 04:38:30.000000 easyapi_django-0.0.8/easyapi/routes.py
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:25:16.313189 easyapi_django-0.0.8/easyapi_django.egg-info/
--rw-r--r--   0 ssjunior   (501) staff       (20)     4535 2023-02-15 04:25:16.000000 easyapi_django-0.0.8/easyapi_django.egg-info/PKG-INFO
--rw-r--r--   0 ssjunior   (501) staff       (20)      300 2023-02-15 04:25:16.000000 easyapi_django-0.0.8/easyapi_django.egg-info/SOURCES.txt
--rw-r--r--   0 ssjunior   (501) staff       (20)        1 2023-02-15 04:25:16.000000 easyapi_django-0.0.8/easyapi_django.egg-info/dependency_links.txt
--rw-r--r--   0 ssjunior   (501) staff       (20)        8 2023-02-15 04:25:16.000000 easyapi_django-0.0.8/easyapi_django.egg-info/top_level.txt
--rw-r--r--   0 ssjunior   (501) staff       (20)      675 2023-02-15 04:24:24.000000 easyapi_django-0.0.8/pyproject.toml
--rw-r--r--   0 ssjunior   (501) staff       (20)       38 2023-02-15 04:25:16.314448 easyapi_django-0.0.8/setup.cfg
+drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:27:28.015940 easyapi_django-0.0.9/
+-rw-r--r--   0 ssjunior   (501) staff       (20)     1076 2023-02-11 03:15:42.000000 easyapi_django-0.0.9/LICENSE
+-rw-r--r--   0 ssjunior   (501) staff       (20)     4535 2023-02-15 04:27:28.015588 easyapi_django-0.0.9/PKG-INFO
+-rw-r--r--   0 ssjunior   (501) staff       (20)     3984 2023-02-11 17:19:30.000000 easyapi_django-0.0.9/README.md
+drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:27:28.013449 easyapi_django-0.0.9/easyapi/
+-rw-r--r--   0 ssjunior   (501) staff       (20)      171 2023-02-11 04:59:19.000000 easyapi_django-0.0.9/easyapi/__init__.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)    23880 2023-02-15 04:26:58.000000 easyapi_django-0.0.9/easyapi/base.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)      231 2022-11-04 05:07:41.000000 easyapi_django-0.0.9/easyapi/exception.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)    25731 2023-02-15 04:17:48.000000 easyapi_django-0.0.9/easyapi/filters.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)      383 2023-02-11 03:26:51.000000 easyapi_django-0.0.9/easyapi/middleware.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)      982 2023-02-11 04:38:30.000000 easyapi_django-0.0.9/easyapi/routes.py
+drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:27:28.014965 easyapi_django-0.0.9/easyapi_django.egg-info/
+-rw-r--r--   0 ssjunior   (501) staff       (20)     4535 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/PKG-INFO
+-rw-r--r--   0 ssjunior   (501) staff       (20)      300 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/SOURCES.txt
+-rw-r--r--   0 ssjunior   (501) staff       (20)        1 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/dependency_links.txt
+-rw-r--r--   0 ssjunior   (501) staff       (20)        8 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/top_level.txt
+-rw-r--r--   0 ssjunior   (501) staff       (20)      675 2023-02-15 04:27:16.000000 easyapi_django-0.0.9/pyproject.toml
+-rw-r--r--   0 ssjunior   (501) staff       (20)       38 2023-02-15 04:27:28.016056 easyapi_django-0.0.9/setup.cfg
```

### Comparing `easyapi_django-0.0.8/LICENSE` & `easyapi_django-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easyapi_django-0.0.8/PKG-INFO` & `easyapi_django-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyapi_django
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple rest api generator for django based on models
 Author-email: Stamatios Stamou Jr <ssjunior@gmail.com>
 Project-URL: Homepage, https://github.com/ssjunior/easyapi-django
 Project-URL: Bug Tracker, https://github.com/ssjunior/easyapi-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easyapi_django-0.0.8/README.md` & `easyapi_django-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `easyapi_django-0.0.8/easyapi/base.py` & `easyapi_django-0.0.9/easyapi/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from .exception import HTTPException
 
 re_id = re.compile(r'(.*)\/(\d+)(\/.)?$')
 search_regex = re.compile(r'__isnull|__gte|__lte|__lt|__gt|__startswith')
 
 
-def fake_tenant(**kwargs):
+def fake_tenant(*args, **kwargs):
     return 'default'
 
 
 tenant = importlib.find_loader('tenant')
 if tenant:
     set_tenant = tenant.set_tenant
     OrmFilter = tenant.Filter
```

### Comparing `easyapi_django-0.0.8/easyapi/filters.py` & `easyapi_django-0.0.9/easyapi/filters.py`

 * *Files identical despite different names*

### Comparing `easyapi_django-0.0.8/easyapi/routes.py` & `easyapi_django-0.0.9/easyapi/routes.py`

 * *Files identical despite different names*

### Comparing `easyapi_django-0.0.8/easyapi_django.egg-info/PKG-INFO` & `easyapi_django-0.0.9/easyapi_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyapi-django
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple rest api generator for django based on models
 Author-email: Stamatios Stamou Jr <ssjunior@gmail.com>
 Project-URL: Homepage, https://github.com/ssjunior/easyapi-django
 Project-URL: Bug Tracker, https://github.com/ssjunior/easyapi-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easyapi_django-0.0.8/pyproject.toml` & `easyapi_django-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Django>=4.1.3",
     "pytz"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "easyapi_django"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Stamatios Stamou Jr", email="ssjunior@gmail.com" },
 ]
 description = "A simple rest api generator for django based on models"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


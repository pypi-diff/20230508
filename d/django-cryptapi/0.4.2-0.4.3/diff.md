# Comparing `tmp/django-cryptapi-0.4.2.tar.gz` & `tmp/django-cryptapi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cryptapi-0.4.2.tar", last modified: Tue Jan 31 09:45:24 2023, max compression
+gzip compressed data, was "django-cryptapi-0.4.3.tar", last modified: Mon May  8 10:43:37 2023, max compression
```

## Comparing `django-cryptapi-0.4.2.tar` & `django-cryptapi-0.4.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:45:24.415256 django-cryptapi-0.4.2/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1098 2022-12-12 09:35:14.000000 django-cryptapi-0.4.2/LICENSE
--rw-r--r--   0 arianoangelo   (501) staff       (20)     9251 2023-01-31 09:45:24.414883 django-cryptapi-0.4.2/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)     8897 2023-01-19 10:18:30.000000 django-cryptapi-0.4.2/README.md
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:45:24.411820 django-cryptapi-0.4.2/cryptapi/
--rw-r--r--   0 arianoangelo   (501) staff       (20)      281 2022-12-12 09:34:52.000000 django-cryptapi-0.4.2/cryptapi/__init__.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1091 2022-12-12 09:34:48.000000 django-cryptapi-0.4.2/cryptapi/admin.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      245 2022-12-12 09:34:50.000000 django-cryptapi-0.4.2/cryptapi/choices.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     3265 2022-12-12 09:38:30.000000 django-cryptapi-0.4.2/cryptapi/cryptapi.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     5766 2023-01-19 10:28:09.000000 django-cryptapi-0.4.2/cryptapi/dispatchers.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1958 2023-01-19 10:15:03.000000 django-cryptapi-0.4.2/cryptapi/forms.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       81 2023-01-19 10:16:29.000000 django-cryptapi-0.4.2/cryptapi/meta.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:45:24.412989 django-cryptapi-0.4.2/cryptapi/migrations/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     4439 2022-12-12 09:34:52.000000 django-cryptapi-0.4.2/cryptapi/migrations/0001_initial.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      404 2022-12-12 09:34:54.000000 django-cryptapi-0.4.2/cryptapi/migrations/0002_provider_last_updated.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      442 2022-12-12 09:34:54.000000 django-cryptapi-0.4.2/cryptapi/migrations/0003_auto_20181112_1939.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1081 2022-12-12 09:34:54.000000 django-cryptapi-0.4.2/cryptapi/migrations/0004_auto_20190729_1132.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      635 2022-12-12 09:34:54.000000 django-cryptapi-0.4.2/cryptapi/migrations/0005_auto_20200504_2323.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      717 2022-12-12 09:34:54.000000 django-cryptapi-0.4.2/cryptapi/migrations/0006_auto_20200505_0304.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      925 2022-12-12 09:34:54.000000 django-cryptapi-0.4.2/cryptapi/migrations/0007_auto_20200827_1510.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1188 2022-12-12 09:34:56.000000 django-cryptapi-0.4.2/cryptapi/migrations/0008_metadata_alter_provider_coin_and_more.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     2027 2023-01-19 10:18:40.000000 django-cryptapi-0.4.2/cryptapi/migrations/0009_remove_payment_value_paid_and_more.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:34:56.000000 django-cryptapi-0.4.2/cryptapi/migrations/__init__.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     6092 2023-01-19 10:16:17.000000 django-cryptapi-0.4.2/cryptapi/models.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1835 2022-12-12 09:34:50.000000 django-cryptapi-0.4.2/cryptapi/settings.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      220 2022-12-12 09:34:52.000000 django-cryptapi-0.4.2/cryptapi/signals.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:45:24.413170 django-cryptapi-0.4.2/cryptapi/templatetags/
--rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:34:52.000000 django-cryptapi-0.4.2/cryptapi/templatetags/__init__.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      300 2022-12-12 09:34:52.000000 django-cryptapi-0.4.2/cryptapi/templatetags/cryptapi_helper.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      222 2022-12-12 09:34:50.000000 django-cryptapi-0.4.2/cryptapi/urls.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1951 2023-01-16 14:41:16.000000 django-cryptapi-0.4.2/cryptapi/utils.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     2629 2023-01-19 10:17:03.000000 django-cryptapi-0.4.2/cryptapi/views.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:45:24.413802 django-cryptapi-0.4.2/django_cryptapi.egg-info/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     9251 2023-01-31 09:45:24.000000 django-cryptapi-0.4.2/django_cryptapi.egg-info/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1218 2023-01-31 09:45:24.000000 django-cryptapi-0.4.2/django_cryptapi.egg-info/SOURCES.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:45:24.000000 django-cryptapi-0.4.2/django_cryptapi.egg-info/dependency_links.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:45:24.000000 django-cryptapi-0.4.2/django_cryptapi.egg-info/not-zip-safe
--rw-r--r--   0 arianoangelo   (501) staff       (20)       16 2023-01-31 09:45:24.000000 django-cryptapi-0.4.2/django_cryptapi.egg-info/requires.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       15 2023-01-31 09:45:24.000000 django-cryptapi-0.4.2/django_cryptapi.egg-info/top_level.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-01-31 09:45:24.415311 django-cryptapi-0.4.2/setup.cfg
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1138 2023-01-31 09:45:19.000000 django-cryptapi-0.4.2/setup.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:45:24.414605 django-cryptapi-0.4.2/store/
--rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-cryptapi-0.4.2/store/__init__.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       66 2022-12-12 09:35:08.000000 django-cryptapi-0.4.2/store/admin.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      148 2022-12-12 09:35:08.000000 django-cryptapi-0.4.2/store/apps.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:08.000000 django-cryptapi-0.4.2/store/forms.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:45:24.414723 django-cryptapi-0.4.2/store/migrations/
--rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-cryptapi-0.4.2/store/migrations/__init__.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       60 2022-12-12 09:35:08.000000 django-cryptapi-0.4.2/store/models.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       63 2022-12-12 09:35:10.000000 django-cryptapi-0.4.2/store/tests.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      221 2022-12-12 09:35:10.000000 django-cryptapi-0.4.2/store/urls.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1428 2022-12-12 09:35:10.000000 django-cryptapi-0.4.2/store/views.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:43:37.434080 django-cryptapi-0.4.3/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1098 2022-12-12 09:35:14.000000 django-cryptapi-0.4.3/LICENSE
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     9271 2023-05-08 10:43:37.433609 django-cryptapi-0.4.3/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     8926 2023-05-08 10:41:09.000000 django-cryptapi-0.4.3/README.md
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:43:37.428941 django-cryptapi-0.4.3/cryptapi/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      281 2022-12-12 09:34:52.000000 django-cryptapi-0.4.3/cryptapi/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1091 2022-12-12 09:34:48.000000 django-cryptapi-0.4.3/cryptapi/admin.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      245 2022-12-12 09:34:50.000000 django-cryptapi-0.4.3/cryptapi/choices.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3265 2022-12-12 09:38:30.000000 django-cryptapi-0.4.3/cryptapi/cryptapi.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     5766 2023-01-19 10:28:09.000000 django-cryptapi-0.4.3/cryptapi/dispatchers.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1958 2023-01-19 10:15:03.000000 django-cryptapi-0.4.3/cryptapi/forms.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       81 2023-05-08 10:41:09.000000 django-cryptapi-0.4.3/cryptapi/meta.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:43:37.430930 django-cryptapi-0.4.3/cryptapi/migrations/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     4439 2022-12-12 09:34:52.000000 django-cryptapi-0.4.3/cryptapi/migrations/0001_initial.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      404 2022-12-12 09:34:54.000000 django-cryptapi-0.4.3/cryptapi/migrations/0002_provider_last_updated.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      442 2022-12-12 09:34:54.000000 django-cryptapi-0.4.3/cryptapi/migrations/0003_auto_20181112_1939.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1081 2022-12-12 09:34:54.000000 django-cryptapi-0.4.3/cryptapi/migrations/0004_auto_20190729_1132.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      635 2022-12-12 09:34:54.000000 django-cryptapi-0.4.3/cryptapi/migrations/0005_auto_20200504_2323.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      717 2022-12-12 09:34:54.000000 django-cryptapi-0.4.3/cryptapi/migrations/0006_auto_20200505_0304.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      925 2022-12-12 09:34:54.000000 django-cryptapi-0.4.3/cryptapi/migrations/0007_auto_20200827_1510.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1188 2022-12-12 09:34:56.000000 django-cryptapi-0.4.3/cryptapi/migrations/0008_metadata_alter_provider_coin_and_more.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     2027 2023-01-19 10:18:40.000000 django-cryptapi-0.4.3/cryptapi/migrations/0009_remove_payment_value_paid_and_more.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:34:56.000000 django-cryptapi-0.4.3/cryptapi/migrations/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     6107 2023-05-08 10:38:51.000000 django-cryptapi-0.4.3/cryptapi/models.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1835 2022-12-12 09:34:50.000000 django-cryptapi-0.4.3/cryptapi/settings.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      220 2022-12-12 09:34:52.000000 django-cryptapi-0.4.3/cryptapi/signals.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:43:37.431118 django-cryptapi-0.4.3/cryptapi/templatetags/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:34:52.000000 django-cryptapi-0.4.3/cryptapi/templatetags/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      300 2022-12-12 09:34:52.000000 django-cryptapi-0.4.3/cryptapi/templatetags/cryptapi_helper.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      222 2022-12-12 09:34:50.000000 django-cryptapi-0.4.3/cryptapi/urls.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1951 2023-01-16 14:41:16.000000 django-cryptapi-0.4.3/cryptapi/utils.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     2629 2023-01-19 10:17:03.000000 django-cryptapi-0.4.3/cryptapi/views.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:43:37.432016 django-cryptapi-0.4.3/django_cryptapi.egg-info/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     9271 2023-05-08 10:43:37.000000 django-cryptapi-0.4.3/django_cryptapi.egg-info/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1218 2023-05-08 10:43:37.000000 django-cryptapi-0.4.3/django_cryptapi.egg-info/SOURCES.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-05-08 10:43:37.000000 django-cryptapi-0.4.3/django_cryptapi.egg-info/dependency_links.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:45:24.000000 django-cryptapi-0.4.3/django_cryptapi.egg-info/not-zip-safe
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       16 2023-05-08 10:43:37.000000 django-cryptapi-0.4.3/django_cryptapi.egg-info/requires.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       15 2023-05-08 10:43:37.000000 django-cryptapi-0.4.3/django_cryptapi.egg-info/top_level.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-05-08 10:43:37.434138 django-cryptapi-0.4.3/setup.cfg
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1151 2023-01-31 10:05:39.000000 django-cryptapi-0.4.3/setup.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:43:37.433202 django-cryptapi-0.4.3/store/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-cryptapi-0.4.3/store/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       66 2022-12-12 09:35:08.000000 django-cryptapi-0.4.3/store/admin.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      148 2022-12-12 09:35:08.000000 django-cryptapi-0.4.3/store/apps.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:08.000000 django-cryptapi-0.4.3/store/forms.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:43:37.433394 django-cryptapi-0.4.3/store/migrations/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-cryptapi-0.4.3/store/migrations/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       60 2022-12-12 09:35:08.000000 django-cryptapi-0.4.3/store/models.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       63 2022-12-12 09:35:10.000000 django-cryptapi-0.4.3/store/tests.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      221 2022-12-12 09:35:10.000000 django-cryptapi-0.4.3/store/urls.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1428 2022-12-12 09:35:10.000000 django-cryptapi-0.4.3/store/views.py
```

### Comparing `django-cryptapi-0.4.2/LICENSE` & `django-cryptapi-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/PKG-INFO` & `django-cryptapi-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-cryptapi
-Version: 0.4.2
+Version: 0.4.3
 Summary: Django implementation of CryptAPI's payment gateway
 Home-page: https://github.com/cryptapi/django-cryptapi
 Author: CryptAPI
 Author-email: info@cryptapi.io
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -329,7 +328,9 @@
 * Minor bugfixes
 
 #### 0.4.2
 * Minor fixes
 * Signals now use the value_coin
 * Removed deprecated fields from the payment model
 
+#### 0.4.3
+* Minor fixes
```

### Comparing `django-cryptapi-0.4.2/README.md` & `django-cryptapi-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -307,8 +307,11 @@
 
 #### 0.4.1
 * Minor bugfixes
 
 #### 0.4.2
 * Minor fixes
 * Signals now use the value_coin
-* Removed deprecated fields from the payment model
+* Removed deprecated fields from the payment model
+
+#### 0.4.3
+* Minor fixes
```

### Comparing `django-cryptapi-0.4.2/cryptapi/admin.py` & `django-cryptapi-0.4.3/cryptapi/admin.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/cryptapi.py` & `django-cryptapi-0.4.3/cryptapi/cryptapi.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/dispatchers.py` & `django-cryptapi-0.4.3/cryptapi/dispatchers.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/forms.py` & `django-cryptapi-0.4.3/cryptapi/forms.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/migrations/0001_initial.py` & `django-cryptapi-0.4.3/cryptapi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/migrations/0004_auto_20190729_1132.py` & `django-cryptapi-0.4.3/cryptapi/migrations/0004_auto_20190729_1132.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/migrations/0005_auto_20200504_2323.py` & `django-cryptapi-0.4.3/cryptapi/migrations/0005_auto_20200504_2323.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/migrations/0006_auto_20200505_0304.py` & `django-cryptapi-0.4.3/cryptapi/migrations/0006_auto_20200505_0304.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/migrations/0007_auto_20200827_1510.py` & `django-cryptapi-0.4.3/cryptapi/migrations/0007_auto_20200827_1510.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/migrations/0008_metadata_alter_provider_coin_and_more.py` & `django-cryptapi-0.4.3/cryptapi/migrations/0008_metadata_alter_provider_coin_and_more.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/migrations/0009_remove_payment_value_paid_and_more.py` & `django-cryptapi-0.4.3/cryptapi/migrations/0009_remove_payment_value_paid_and_more.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/models.py` & `django-cryptapi-0.4.3/cryptapi/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,33 +47,33 @@
     timestamp = models.DateTimeField(auto_now_add=True)
 
     @property
     def total(self):
         qs = self.payment_set.all()
 
         if qs.exists():
-            return qs.aggregate(sum=Sum('value_paid')).get('sum', 0)
+            return qs.aggregate(sum=Sum('value_paid_coin')).get('sum', 0)
 
         return 0
 
     @property
     def total_pending(self):
         qs = self.payment_set.filter(pending=True)
 
         if qs.exists():
-            return qs.aggregate(sum=Sum('value_paid')).get('sum', 0)
+            return qs.aggregate(sum=Sum('value_paid_coin')).get('sum', 0)
 
         return 0
 
     @property
     def total_confirmed(self):
         qs = self.payment_set.filter(pending=False)
 
         if qs.exists():
-            return qs.aggregate(sum=Sum('value_paid')).get('sum', 0)
+            return qs.aggregate(sum=Sum('value_paid_coin')).get('sum', 0)
 
         return 0
 
     def set_value(self, value, commit=False):
         _coin = self.provider.get_coin_display()
 
         self.value_requested = value
```

### Comparing `django-cryptapi-0.4.2/cryptapi/settings.py` & `django-cryptapi-0.4.3/cryptapi/settings.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/utils.py` & `django-cryptapi-0.4.3/cryptapi/utils.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/cryptapi/views.py` & `django-cryptapi-0.4.3/cryptapi/views.py`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/django_cryptapi.egg-info/PKG-INFO` & `django-cryptapi-0.4.3/django_cryptapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-cryptapi
-Version: 0.4.2
+Version: 0.4.3
 Summary: Django implementation of CryptAPI's payment gateway
 Home-page: https://github.com/cryptapi/django-cryptapi
 Author: CryptAPI
 Author-email: info@cryptapi.io
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -329,7 +328,9 @@
 * Minor bugfixes
 
 #### 0.4.2
 * Minor fixes
 * Signals now use the value_coin
 * Removed deprecated fields from the payment model
 
+#### 0.4.3
+* Minor fixes
```

### Comparing `django-cryptapi-0.4.2/django_cryptapi.egg-info/SOURCES.txt` & `django-cryptapi-0.4.3/django_cryptapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cryptapi-0.4.2/setup.py` & `django-cryptapi-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     long_description=long_description,
 
     include_package_data=True,
 
     url='https://github.com/cryptapi/django-cryptapi',
     classifiers=[
         "Programming Language :: Python",
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
```

### Comparing `django-cryptapi-0.4.2/store/views.py` & `django-cryptapi-0.4.3/store/views.py`

 * *Files identical despite different names*


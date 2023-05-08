# Comparing `tmp/django-blockbee-1.0.3.tar.gz` & `tmp/django-blockbee-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-blockbee-1.0.3.tar", last modified: Thu Jan 19 10:11:21 2023, max compression
+gzip compressed data, was "django-blockbee-1.0.4.tar", last modified: Mon May  8 10:47:12 2023, max compression
```

## Comparing `django-blockbee-1.0.3.tar` & `django-blockbee-1.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.838983 django-blockbee-1.0.3/
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     1098 2022-12-12 11:13:24.000000 django-blockbee-1.0.3/LICENSE
--rw-r--r--   0 arianoangelo   (501) staff       (20)     8517 2023-01-19 10:11:21.838843 django-blockbee-1.0.3/PKG-INFO
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     8128 2023-01-19 10:09:39.000000 django-blockbee-1.0.3/README.md
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.834249 django-blockbee-1.0.3/blockbee/
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      283 2022-12-12 11:11:12.000000 django-blockbee-1.0.3/blockbee/__init__.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     1091 2022-12-12 09:34:48.000000 django-blockbee-1.0.3/blockbee/admin.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       39 2023-01-19 10:08:28.000000 django-blockbee-1.0.3/blockbee/apikey.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     3076 2022-12-12 11:09:03.000000 django-blockbee-1.0.3/blockbee/blockbee.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      245 2022-12-12 09:34:50.000000 django-blockbee-1.0.3/blockbee/choices.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     5569 2023-01-19 09:59:46.000000 django-blockbee-1.0.3/blockbee/dispatchers.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     1958 2023-01-19 09:53:49.000000 django-blockbee-1.0.3/blockbee/forms.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)       81 2023-01-19 09:38:09.000000 django-blockbee-1.0.3/blockbee/meta.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.835002 django-blockbee-1.0.3/blockbee/migrations/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     4913 2022-12-12 11:12:06.000000 django-blockbee-1.0.3/blockbee/migrations/0001_initial.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      491 2023-01-16 12:12:37.000000 django-blockbee-1.0.3/blockbee/migrations/0002_alter_provider_cold_wallet.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)      987 2023-01-19 10:03:03.000000 django-blockbee-1.0.3/blockbee/migrations/0003_remove_payment_value_paid_and_more.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-blockbee-1.0.3/blockbee/migrations/__init__.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     6090 2023-01-19 09:54:16.000000 django-blockbee-1.0.3/blockbee/models.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     1835 2023-01-06 13:36:38.000000 django-blockbee-1.0.3/blockbee/settings.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      220 2023-01-19 09:41:19.000000 django-blockbee-1.0.3/blockbee/signals.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.835190 django-blockbee-1.0.3/blockbee/templatetags/
--rw-rw-r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:34:52.000000 django-blockbee-1.0.3/blockbee/templatetags/__init__.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      300 2023-01-06 13:34:28.000000 django-blockbee-1.0.3/blockbee/templatetags/blockbee_helper.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      222 2022-12-12 10:54:29.000000 django-blockbee-1.0.3/blockbee/urls.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     2002 2023-01-16 14:25:39.000000 django-blockbee-1.0.3/blockbee/utils.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     2629 2023-01-19 09:57:28.000000 django-blockbee-1.0.3/blockbee/views.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.836242 django-blockbee-1.0.3/django_blockbee.egg-info/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     8517 2023-01-19 10:11:21.000000 django-blockbee-1.0.3/django_blockbee.egg-info/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1054 2023-01-19 10:11:21.000000 django-blockbee-1.0.3/django_blockbee.egg-info/SOURCES.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-19 10:11:21.000000 django-blockbee-1.0.3/django_blockbee.egg-info/dependency_links.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2022-12-12 17:09:32.000000 django-blockbee-1.0.3/django_blockbee.egg-info/not-zip-safe
--rw-r--r--   0 arianoangelo   (501) staff       (20)       16 2023-01-19 10:11:21.000000 django-blockbee-1.0.3/django_blockbee.egg-info/requires.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       28 2023-01-19 10:11:21.000000 django-blockbee-1.0.3/django_blockbee.egg-info/top_level.txt
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.837254 django-blockbee-1.0.3/django_store/
--rw-rw-r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:06.000000 django-blockbee-1.0.3/django_store/__init__.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      417 2022-12-12 09:35:06.000000 django-blockbee-1.0.3/django_store/asgi.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     3234 2022-12-12 10:54:29.000000 django-blockbee-1.0.3/django_store/settings.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      221 2022-12-12 10:54:29.000000 django-blockbee-1.0.3/django_store/urls.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      417 2022-12-12 09:35:06.000000 django-blockbee-1.0.3/django_store/wsgi.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-01-19 10:11:21.839021 django-blockbee-1.0.3/setup.cfg
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     1130 2022-12-12 17:48:36.000000 django-blockbee-1.0.3/setup.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.838549 django-blockbee-1.0.3/store/
--rw-rw-r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-blockbee-1.0.3/store/__init__.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)       66 2022-12-12 09:35:08.000000 django-blockbee-1.0.3/store/admin.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      148 2022-12-12 09:35:08.000000 django-blockbee-1.0.3/store/apps.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:08.000000 django-blockbee-1.0.3/store/forms.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-19 10:11:21.838676 django-blockbee-1.0.3/store/migrations/
--rw-rw-r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-blockbee-1.0.3/store/migrations/__init__.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)       60 2022-12-12 09:35:08.000000 django-blockbee-1.0.3/store/models.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)       63 2022-12-12 09:35:10.000000 django-blockbee-1.0.3/store/tests.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)      221 2022-12-12 09:35:10.000000 django-blockbee-1.0.3/store/urls.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     1600 2022-12-12 11:39:08.000000 django-blockbee-1.0.3/store/views.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.471284 django-blockbee-1.0.4/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1098 2022-12-12 11:13:24.000000 django-blockbee-1.0.4/LICENSE
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     8524 2023-05-08 10:47:12.471066 django-blockbee-1.0.4/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     8157 2023-05-08 10:44:42.000000 django-blockbee-1.0.4/README.md
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.465264 django-blockbee-1.0.4/blockbee/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      283 2022-12-12 11:11:12.000000 django-blockbee-1.0.4/blockbee/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1091 2022-12-12 09:34:48.000000 django-blockbee-1.0.4/blockbee/admin.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       39 2023-05-08 10:31:11.000000 django-blockbee-1.0.4/blockbee/apikey.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3076 2022-12-12 11:09:03.000000 django-blockbee-1.0.4/blockbee/blockbee.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      245 2022-12-12 09:34:50.000000 django-blockbee-1.0.4/blockbee/choices.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     5569 2023-01-19 09:59:46.000000 django-blockbee-1.0.4/blockbee/dispatchers.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1958 2023-01-19 09:53:49.000000 django-blockbee-1.0.4/blockbee/forms.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       81 2023-05-08 10:44:42.000000 django-blockbee-1.0.4/blockbee/meta.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.466451 django-blockbee-1.0.4/blockbee/migrations/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     4913 2022-12-12 11:12:06.000000 django-blockbee-1.0.4/blockbee/migrations/0001_initial.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      491 2023-01-16 12:12:37.000000 django-blockbee-1.0.4/blockbee/migrations/0002_alter_provider_cold_wallet.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      987 2023-01-19 10:03:03.000000 django-blockbee-1.0.4/blockbee/migrations/0003_remove_payment_value_paid_and_more.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-blockbee-1.0.4/blockbee/migrations/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     6105 2023-05-08 10:44:42.000000 django-blockbee-1.0.4/blockbee/models.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1835 2023-01-06 13:36:38.000000 django-blockbee-1.0.4/blockbee/settings.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      220 2023-01-19 09:41:19.000000 django-blockbee-1.0.4/blockbee/signals.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.466628 django-blockbee-1.0.4/blockbee/templatetags/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:34:52.000000 django-blockbee-1.0.4/blockbee/templatetags/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      300 2023-01-06 13:34:28.000000 django-blockbee-1.0.4/blockbee/templatetags/blockbee_helper.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      222 2022-12-12 10:54:29.000000 django-blockbee-1.0.4/blockbee/urls.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     2002 2023-01-16 14:25:39.000000 django-blockbee-1.0.4/blockbee/utils.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     2629 2023-01-19 09:57:28.000000 django-blockbee-1.0.4/blockbee/views.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.467622 django-blockbee-1.0.4/django_blockbee.egg-info/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     8524 2023-05-08 10:47:12.000000 django-blockbee-1.0.4/django_blockbee.egg-info/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1054 2023-05-08 10:47:12.000000 django-blockbee-1.0.4/django_blockbee.egg-info/SOURCES.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-05-08 10:47:12.000000 django-blockbee-1.0.4/django_blockbee.egg-info/dependency_links.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2022-12-12 17:09:32.000000 django-blockbee-1.0.4/django_blockbee.egg-info/not-zip-safe
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       16 2023-05-08 10:47:12.000000 django-blockbee-1.0.4/django_blockbee.egg-info/requires.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       28 2023-05-08 10:47:12.000000 django-blockbee-1.0.4/django_blockbee.egg-info/top_level.txt
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.468595 django-blockbee-1.0.4/django_store/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:06.000000 django-blockbee-1.0.4/django_store/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      417 2022-12-12 09:35:06.000000 django-blockbee-1.0.4/django_store/asgi.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3234 2022-12-12 10:54:29.000000 django-blockbee-1.0.4/django_store/settings.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      221 2022-12-12 10:54:29.000000 django-blockbee-1.0.4/django_store/urls.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      417 2022-12-12 09:35:06.000000 django-blockbee-1.0.4/django_store/wsgi.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-05-08 10:47:12.471347 django-blockbee-1.0.4/setup.cfg
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1130 2022-12-12 17:48:36.000000 django-blockbee-1.0.4/setup.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.470592 django-blockbee-1.0.4/store/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-blockbee-1.0.4/store/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       66 2022-12-12 09:35:08.000000 django-blockbee-1.0.4/store/admin.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      148 2022-12-12 09:35:08.000000 django-blockbee-1.0.4/store/apps.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:08.000000 django-blockbee-1.0.4/store/forms.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-05-08 10:47:12.470850 django-blockbee-1.0.4/store/migrations/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        0 2022-12-12 09:35:10.000000 django-blockbee-1.0.4/store/migrations/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       60 2022-12-12 09:35:08.000000 django-blockbee-1.0.4/store/models.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       63 2022-12-12 09:35:10.000000 django-blockbee-1.0.4/store/tests.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      221 2022-12-12 09:35:10.000000 django-blockbee-1.0.4/store/urls.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1600 2022-12-12 11:39:08.000000 django-blockbee-1.0.4/store/views.py
```

### Comparing `django-blockbee-1.0.3/LICENSE` & `django-blockbee-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/PKG-INFO` & `django-blockbee-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-blockbee
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django implementation of BlockBee's payment gateway
 Home-page: https://github.com/blockbee-io/django-blockbee
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -310,7 +309,9 @@
 * Minor fixes
 
 #### 1.0.3
 * Minor fixes
 * Signals now use the value_coin
 * Removed deprecated fields from the payment model
 
+#### 1.0.4
+* Minor fixes
```

### Comparing `django-blockbee-1.0.3/README.md` & `django-blockbee-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -288,8 +288,11 @@
 
 #### 1.0.2
 * Minor fixes
 
 #### 1.0.3
 * Minor fixes
 * Signals now use the value_coin
-* Removed deprecated fields from the payment model
+* Removed deprecated fields from the payment model
+
+#### 1.0.4
+* Minor fixes
```

### Comparing `django-blockbee-1.0.3/blockbee/admin.py` & `django-blockbee-1.0.4/blockbee/admin.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/blockbee.py` & `django-blockbee-1.0.4/blockbee/blockbee.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/dispatchers.py` & `django-blockbee-1.0.4/blockbee/dispatchers.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/forms.py` & `django-blockbee-1.0.4/blockbee/forms.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/migrations/0001_initial.py` & `django-blockbee-1.0.4/blockbee/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/migrations/0003_remove_payment_value_paid_and_more.py` & `django-blockbee-1.0.4/blockbee/migrations/0003_remove_payment_value_paid_and_more.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/models.py` & `django-blockbee-1.0.4/blockbee/models.py`

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

### Comparing `django-blockbee-1.0.3/blockbee/settings.py` & `django-blockbee-1.0.4/blockbee/settings.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/utils.py` & `django-blockbee-1.0.4/blockbee/utils.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/blockbee/views.py` & `django-blockbee-1.0.4/blockbee/views.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/django_blockbee.egg-info/PKG-INFO` & `django-blockbee-1.0.4/django_blockbee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-blockbee
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django implementation of BlockBee's payment gateway
 Home-page: https://github.com/blockbee-io/django-blockbee
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -310,7 +309,9 @@
 * Minor fixes
 
 #### 1.0.3
 * Minor fixes
 * Signals now use the value_coin
 * Removed deprecated fields from the payment model
 
+#### 1.0.4
+* Minor fixes
```

### Comparing `django-blockbee-1.0.3/django_blockbee.egg-info/SOURCES.txt` & `django-blockbee-1.0.4/django_blockbee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/django_store/settings.py` & `django-blockbee-1.0.4/django_store/settings.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/setup.py` & `django-blockbee-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-blockbee-1.0.3/store/views.py` & `django-blockbee-1.0.4/store/views.py`

 * *Files identical despite different names*


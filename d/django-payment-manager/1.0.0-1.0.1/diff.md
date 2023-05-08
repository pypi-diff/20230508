# Comparing `tmp/django-payment-manager-1.0.0.tar.gz` & `tmp/django-payment-manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-payment-manager-1.0.0.tar", last modified: Mon May  8 21:00:50 2023, max compression
+gzip compressed data, was "django-payment-manager-1.0.1.tar", last modified: Mon May  8 21:07:01 2023, max compression
```

## Comparing `django-payment-manager-1.0.0.tar` & `django-payment-manager-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.601190 django-payment-manager-1.0.0/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-payment-manager-1.0.0/LICENSE
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      383 2023-04-27 14:39:53.000000 django-payment-manager-1.0.0/MANIFEST.in
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8189 2023-05-08 21:00:50.601290 django-payment-manager-1.0.0/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7084 2023-05-07 19:22:38.000000 django-payment-manager-1.0.0/README.md
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.595002 django-payment-manager-1.0.0/django_payment_manager.egg-info/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8189 2023-05-08 21:00:50.000000 django-payment-manager-1.0.0/django_payment_manager.egg-info/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      849 2023-05-08 21:00:50.000000 django-payment-manager-1.0.0/django_payment_manager.egg-info/SOURCES.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-05-08 21:00:50.000000 django-payment-manager-1.0.0/django_payment_manager.egg-info/dependency_links.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       29 2023-05-08 21:00:50.000000 django-payment-manager-1.0.0/django_payment_manager.egg-info/requires.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        8 2023-05-08 21:00:50.000000 django-payment-manager-1.0.0/django_payment_manager.egg-info/top_level.txt
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.597779 django-payment-manager-1.0.0/payment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-24 20:13:21.000000 django-payment-manager-1.0.0/payment/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      450 2023-05-07 21:20:14.000000 django-payment-manager-1.0.0/payment/admin.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      146 2023-04-24 20:13:21.000000 django-payment-manager-1.0.0/payment/apps.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.598321 django-payment-manager-1.0.0/payment/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-payment-manager-1.0.0/payment/email_sender/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2103 2023-04-27 16:04:51.000000 django-payment-manager-1.0.0/payment/email_sender/email_sender.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.598646 django-payment-manager-1.0.0/payment/migrations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-24 20:13:21.000000 django-payment-manager-1.0.0/payment/migrations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2788 2023-05-07 19:14:16.000000 django-payment-manager-1.0.0/payment/models.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1280 2023-05-07 20:55:37.000000 django-payment-manager-1.0.0/payment/settings.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.592440 django-payment-manager-1.0.0/payment/static/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.598758 django-payment-manager-1.0.0/payment/static/css/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2626 2023-04-24 22:57:35.000000 django-payment-manager-1.0.0/payment/static/css/payment.css
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.592723 django-payment-manager-1.0.0/payment/templates/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.599115 django-payment-manager-1.0.0/payment/templates/base_templates/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1936 2023-04-24 20:43:39.000000 django-payment-manager-1.0.0/payment/templates/base_templates/base.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.599954 django-payment-manager-1.0.0/payment/templates/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    13325 2023-05-07 21:20:14.000000 django-payment-manager-1.0.0/payment/templates/email_sender/notify_admin.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1704 2023-05-07 18:37:25.000000 django-payment-manager-1.0.0/payment/templates/email_sender/payment_email.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:00:50.600809 django-payment-manager-1.0.0/payment/templates/payment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5174 2023-05-08 20:23:27.000000 django-payment-manager-1.0.0/payment/templates/payment/payment.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    12617 2023-05-07 19:02:35.000000 django-payment-manager-1.0.0/payment/templates/payment/payment_details.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1623 2023-05-07 21:20:14.000000 django-payment-manager-1.0.0/payment/templates/payment/success.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       60 2023-04-24 20:13:21.000000 django-payment-manager-1.0.0/payment/tests.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      767 2023-05-07 19:14:16.000000 django-payment-manager-1.0.0/payment/urls.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3047 2023-05-08 19:33:08.000000 django-payment-manager-1.0.0/payment/utils.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     9648 2023-05-08 20:23:27.000000 django-payment-manager-1.0.0/payment/views.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-payment-manager-1.0.0/pyproject.toml
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1113 2023-05-08 21:00:50.601688 django-payment-manager-1.0.0/setup.cfg
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-payment-manager-1.0.0/setup.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.299807 django-payment-manager-1.0.1/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-payment-manager-1.0.1/LICENSE
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      383 2023-04-27 14:39:53.000000 django-payment-manager-1.0.1/MANIFEST.in
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8185 2023-05-08 21:07:01.299957 django-payment-manager-1.0.1/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7084 2023-05-07 19:22:38.000000 django-payment-manager-1.0.1/README.md
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.290333 django-payment-manager-1.0.1/django_payment_manager.egg-info/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8185 2023-05-08 21:07:01.000000 django-payment-manager-1.0.1/django_payment_manager.egg-info/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      849 2023-05-08 21:07:01.000000 django-payment-manager-1.0.1/django_payment_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-05-08 21:07:01.000000 django-payment-manager-1.0.1/django_payment_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       29 2023-05-08 21:07:01.000000 django-payment-manager-1.0.1/django_payment_manager.egg-info/requires.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        8 2023-05-08 21:07:01.000000 django-payment-manager-1.0.1/django_payment_manager.egg-info/top_level.txt
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.293481 django-payment-manager-1.0.1/payment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-24 20:13:21.000000 django-payment-manager-1.0.1/payment/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      450 2023-05-07 21:20:14.000000 django-payment-manager-1.0.1/payment/admin.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      146 2023-04-24 20:13:21.000000 django-payment-manager-1.0.1/payment/apps.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.294019 django-payment-manager-1.0.1/payment/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-payment-manager-1.0.1/payment/email_sender/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2103 2023-04-27 16:04:51.000000 django-payment-manager-1.0.1/payment/email_sender/email_sender.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.294340 django-payment-manager-1.0.1/payment/migrations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-24 20:13:21.000000 django-payment-manager-1.0.1/payment/migrations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2788 2023-05-07 19:14:16.000000 django-payment-manager-1.0.1/payment/models.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1280 2023-05-07 20:55:37.000000 django-payment-manager-1.0.1/payment/settings.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.288081 django-payment-manager-1.0.1/payment/static/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.296601 django-payment-manager-1.0.1/payment/static/css/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2626 2023-04-24 22:57:35.000000 django-payment-manager-1.0.1/payment/static/css/payment.css
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.288373 django-payment-manager-1.0.1/payment/templates/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.297240 django-payment-manager-1.0.1/payment/templates/base_templates/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1936 2023-04-24 20:43:39.000000 django-payment-manager-1.0.1/payment/templates/base_templates/base.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.298261 django-payment-manager-1.0.1/payment/templates/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    13325 2023-05-07 21:20:14.000000 django-payment-manager-1.0.1/payment/templates/email_sender/notify_admin.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1704 2023-05-07 18:37:25.000000 django-payment-manager-1.0.1/payment/templates/email_sender/payment_email.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 21:07:01.299339 django-payment-manager-1.0.1/payment/templates/payment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5174 2023-05-08 20:23:27.000000 django-payment-manager-1.0.1/payment/templates/payment/payment.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    12617 2023-05-07 19:02:35.000000 django-payment-manager-1.0.1/payment/templates/payment/payment_details.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1623 2023-05-07 21:20:14.000000 django-payment-manager-1.0.1/payment/templates/payment/success.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       60 2023-04-24 20:13:21.000000 django-payment-manager-1.0.1/payment/tests.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      767 2023-05-07 19:14:16.000000 django-payment-manager-1.0.1/payment/urls.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3047 2023-05-08 19:33:08.000000 django-payment-manager-1.0.1/payment/utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     9648 2023-05-08 20:23:27.000000 django-payment-manager-1.0.1/payment/views.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-payment-manager-1.0.1/pyproject.toml
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1109 2023-05-08 21:07:01.300414 django-payment-manager-1.0.1/setup.cfg
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-payment-manager-1.0.1/setup.py
```

### Comparing `django-payment-manager-1.0.0/LICENSE` & `django-payment-manager-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/PKG-INFO` & `django-payment-manager-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-payment-manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app for integrating PayPal and Credit Card payments with ease and flexibility.
-Home-page: https://github.com/adamspd/django-appointment
+Home-page: https://github.com/adamspd/django-payment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `django-payment-manager-1.0.0/README.md` & `django-payment-manager-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/django_payment_manager.egg-info/PKG-INFO` & `django-payment-manager-1.0.1/django_payment_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-payment-manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app for integrating PayPal and Credit Card payments with ease and flexibility.
-Home-page: https://github.com/adamspd/django-appointment
+Home-page: https://github.com/adamspd/django-payment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `django-payment-manager-1.0.0/django_payment_manager.egg-info/SOURCES.txt` & `django-payment-manager-1.0.1/django_payment_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/email_sender/email_sender.py` & `django-payment-manager-1.0.1/payment/email_sender/email_sender.py`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/models.py` & `django-payment-manager-1.0.1/payment/models.py`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/settings.py` & `django-payment-manager-1.0.1/payment/settings.py`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/static/css/payment.css` & `django-payment-manager-1.0.1/payment/static/css/payment.css`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/templates/base_templates/base.html` & `django-payment-manager-1.0.1/payment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/templates/email_sender/notify_admin.html` & `django-payment-manager-1.0.1/payment/templates/email_sender/notify_admin.html`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/templates/email_sender/payment_email.html` & `django-payment-manager-1.0.1/payment/templates/email_sender/payment_email.html`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/templates/payment/payment.html` & `django-payment-manager-1.0.1/payment/templates/payment/payment.html`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/templates/payment/payment_details.html` & `django-payment-manager-1.0.1/payment/templates/payment/payment_details.html`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/templates/payment/success.html` & `django-payment-manager-1.0.1/payment/templates/payment/success.html`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/urls.py` & `django-payment-manager-1.0.1/payment/urls.py`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/utils.py` & `django-payment-manager-1.0.1/payment/utils.py`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/payment/views.py` & `django-payment-manager-1.0.1/payment/views.py`

 * *Files identical despite different names*

### Comparing `django-payment-manager-1.0.0/setup.cfg` & `django-payment-manager-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = django-payment-manager
-version = 1.0.0
+version = 1.0.1
 description = A Django app for integrating PayPal and Credit Card payments with ease and flexibility.
-url = https://github.com/adamspd/django-appointment
+url = https://github.com/adamspd/django-payment
 author = Adams Pierre David
 author_email = adamspd.developer@gmail.com
 author_website = https://adamspierredavid.com/
 readme = README.md
 license = Apache License 2.0
 classifiers = 
 	Environment :: Web Environment
```


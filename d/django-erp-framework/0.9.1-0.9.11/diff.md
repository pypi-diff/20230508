# Comparing `tmp/django-erp-framework-0.9.1.tar.gz` & `tmp/django-erp-framework-0.9.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-erp-framework-0.9.1.tar", last modified: Sun May  7 13:03:00 2023, max compression
+gzip compressed data, was "django-erp-framework-0.9.11.tar", last modified: Mon May  8 15:21:57 2023, max compression
```

## Comparing `django-erp-framework-0.9.1.tar` & `django-erp-framework-0.9.11.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/
--rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-0.9.1/LICENSE
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-0.9.1/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4976 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3352 2023-05-06 12:34:52.000000 django-erp-framework-0.9.1/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/django_erp_framework.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4976 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1756 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      205 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/top_level.txt
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       97 2023-05-07 13:02:56.000000 django-erp-framework-0.9.1/erp_framework/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/activity/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8367 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/activity/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/0002_auto_20200711_1253.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/0003_alter_myactivity_options.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/admin/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       62 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    51228 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7476 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/base.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      667 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/helpers.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/admin/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2450 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/erp_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4338 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/ra_admin_list.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1783 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/ra_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    18435 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/suit_menu.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      618 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/base/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2992 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7609 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    16862 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3415 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/registry.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1726 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/widgets.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2422 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/checks.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/contrib/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/contrib/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/contrib/jazzmin_integration/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/contrib/jazzmin_integration/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      346 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      164 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/printing.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5552 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/registry.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    26830 2023-05-07 05:11:23.000000 django-erp-framework-0.9.1/erp_framework/reporting/views.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/utils/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      454 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/navigation.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3937 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/permissions.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/views.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1761 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-0.9.1/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-0.9.11/LICENSE
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-0.9.11/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3352 2023-05-06 12:34:52.000000 django-erp-framework-0.9.11/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/django_erp_framework.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1724 2023-05-08 15:21:57.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      205 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/top_level.txt
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       99 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/erp_framework/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/activity/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8367 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/activity/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/0002_auto_20200711_1253.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/0003_alter_myactivity_options.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/models.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/admin/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       62 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    51303 2023-05-08 14:12:13.000000 django-erp-framework-0.9.11/erp_framework/admin/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7542 2023-05-08 14:10:04.000000 django-erp-framework-0.9.11/erp_framework/admin/base.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      667 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      618 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/base/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2933 2023-05-08 14:23:36.000000 django-erp-framework-0.9.11/erp_framework/base/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7609 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    16862 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3415 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/registry.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1726 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/widgets.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2422 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/checks.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/contrib/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/contrib/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/contrib/jazzmin_integration/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/contrib/jazzmin_integration/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      346 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      164 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/printing.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5552 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      665 2023-05-08 14:33:00.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/_ra_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    18435 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/_suit_menu.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2683 2023-05-08 14:17:14.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/erp_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    26830 2023-05-07 05:11:23.000000 django-erp-framework-0.9.11/erp_framework/reporting/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/utils/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      454 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/navigation.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3937 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/permissions.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/views.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1782 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-0.9.11/setup.py
```

### Comparing `django-erp-framework-0.9.1/LICENSE` & `django-erp-framework-0.9.11/LICENSE`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/PKG-INFO` & `django-erp-framework-0.9.11/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.1
+Version: 0.9.11
 Summary: A light-weight effective Django based framework to create diverse business applications
-Home-page: https://github.com/ra-systems/RA
-Author: Ra Systems
+Home-page: https://github.com/RamezIssac/django-erp-framework
+Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
```

### Comparing `django-erp-framework-0.9.1/README.rst` & `django-erp-framework-0.9.11/README.rst`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/django_erp_framework.egg-info/PKG-INFO` & `django-erp-framework-0.9.11/django_erp_framework.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.1
+Version: 0.9.11
 Summary: A light-weight effective Django based framework to create diverse business applications
-Home-page: https://github.com/ra-systems/RA
-Author: Ra Systems
+Home-page: https://github.com/RamezIssac/django-erp-framework
+Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
```

### Comparing `django-erp-framework-0.9.1/django_erp_framework.egg-info/SOURCES.txt` & `django-erp-framework-0.9.11/django_erp_framework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 erp_framework/activity/migrations/__init__.py
 erp_framework/admin/__init__.py
 erp_framework/admin/admin.py
 erp_framework/admin/apps.py
 erp_framework/admin/base.py
 erp_framework/admin/forms.py
 erp_framework/admin/helpers.py
-erp_framework/admin/templatetags/__init__.py
-erp_framework/admin/templatetags/erp_reporting_tags.py
-erp_framework/admin/templatetags/ra_admin_list.py
-erp_framework/admin/templatetags/ra_tags.py
-erp_framework/admin/templatetags/suit_menu.py
 erp_framework/base/__init__.py
 erp_framework/base/app_settings.py
 erp_framework/base/helpers.py
 erp_framework/base/models.py
 erp_framework/base/registry.py
 erp_framework/base/widgets.py
 erp_framework/contrib/__init__.py
@@ -41,11 +36,15 @@
 erp_framework/reporting/__init__.py
 erp_framework/reporting/apps.py
 erp_framework/reporting/forms.py
 erp_framework/reporting/models.py
 erp_framework/reporting/printing.py
 erp_framework/reporting/registry.py
 erp_framework/reporting/views.py
+erp_framework/reporting/templatetags/__init__.py
+erp_framework/reporting/templatetags/_ra_tags.py
+erp_framework/reporting/templatetags/_suit_menu.py
+erp_framework/reporting/templatetags/erp_reporting_tags.py
 erp_framework/utils/__init__.py
 erp_framework/utils/navigation.py
 erp_framework/utils/permissions.py
 erp_framework/utils/views.py
```

### Comparing `django-erp-framework-0.9.1/erp_framework/activity/admin.py` & `django-erp-framework-0.9.11/erp_framework/activity/admin.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/activity/migrations/0001_initial.py` & `django-erp-framework-0.9.11/erp_framework/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/admin/admin.py` & `django-erp-framework-0.9.11/erp_framework/admin/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,29 +598,29 @@
                     )
                     formfield.widget = RaRelatedFieldWidgetWrapper(
                         formfield.widget,
                         db_field.remote_field,
                         self.admin_site,
                         **wrapper_kwargs,
                     )
-            return app_settings.RA_FORMFIELD_FOR_DBFIELD_FUNC(
+            return app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
                 self, db_field, formfield, request, **kwargs
             )
 
         # if db_field.name == 'date' and db_field.__class__ == DateTimeField:
         #     field = forms.SplitDateTimeField(widget=AdminSplitDateTimeNoBr, label=_('Date'))
         # else:
         field = super(EntityAdmin, self).formfield_for_dbfield(
             db_field, request, **kwargs
         )
         if db_field.name == "slug" and self.enable_next_serial:
             field.initial = self.get_next_serial()
         elif db_field.name == "date":
             field.initial = now()
-        return app_settings.RA_FORMFIELD_FOR_DBFIELD_FUNC(
+        return app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
             self, db_field, field, request, **kwargs
         )
 
     def get_next_serial(self):
         from erp_framework.base.helpers import get_next_serial
 
         return get_next_serial(self.model)
@@ -844,15 +844,15 @@
     copy_form_notes_to_formset = False
     search_fields = ["date", "slug"]
 
     def formfield_for_dbfield(self, db_field, request, **kwargs):
         form_field = super(TransactionAdmin, self).formfield_for_dbfield(
             db_field, request, **kwargs
         )
-        form_field = app_settings.RA_FORMFIELD_FOR_DBFIELD_FUNC(
+        form_field = app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
             self, db_field, form_field, request, **kwargs
         )
         return form_field
 
     def get_foreign_keys(self, form_fields=None):
         fks = [
             field.name
@@ -1019,15 +1019,15 @@
                         db_field.remote_field,
                         self.admin_site,
                         **wrapper_kwargs,
                     )
         form_field = super(TransactionItemAdmin, self).formfield_for_dbfield(
             db_field, request, **kwargs
         )
-        form_field = app_settings.RA_FORMFIELD_FOR_DBFIELD_FUNC(
+        form_field = app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
             self, db_field, form_field, request, **kwargs
         )
         return form_field
 
 
 class RaGenericTabularInline(GenericTabularInline):
     """
@@ -1076,15 +1076,15 @@
                         db_field.remote_field,
                         self.admin_site,
                         **wrapper_kwargs,
                     )
         form_field = super(RaGenericTabularInline, self).formfield_for_dbfield(
             db_field, request, **kwargs
         )
-        form_field = app_settings.RA_FORMFIELD_FOR_DBFIELD_FUNC(
+        form_field = app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
             self, db_field, form_field, request, **kwargs
         )
         return form_field
 
 
 class PrepopulatedAdmin(object):
     prepopulation_querysets = None
```

### Comparing `django-erp-framework-0.9.1/erp_framework/admin/base.py` & `django-erp-framework-0.9.11/erp_framework/admin/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,19 @@
     from erp_framework.reporting.registry import report_registry
 
     klass = report_registry.get(base_model, report_slug)
     return klass.as_view()(request)
 
 
 class RaAdminSiteBase(AdminSite):
-    site_title = app_settings.RA_ADMIN_SITE_TITLE
-    site_header = app_settings.RA_ADMIN_SITE_HEADER
-    index_title = app_settings.RA_ADMIN_INDEX_TITLE
+    site_title = app_settings.ERP_ADMIN_SITE_TITLE
+    site_header = app_settings.ERP_ADMIN_SITE_HEADER
+    index_title = app_settings.ERP_ADMIN_INDEX_TITLE
 
-    index_template = app_settings.RA_ADMIN_INDEX_TEMPLATE
+    index_template = app_settings.ERP_ADMIN_INDEX_TEMPLATE
     app_index_template = app_settings.RA_ADMIN_APP_INDEX_TEMPLATE
     login_template = app_settings.RA_ADMIN_LOGIN_TEMPLATE
 
     # logout_template = app_settings.RA_ADMIN_LOGGED_OUT_TEMPLATE
 
     def get_urls(self):
         # from erp_framework.utils.views import access_denied
@@ -184,14 +184,15 @@
         context = dict(
             self.each_context(request),
             name=self.index_title,
         )
         context.update(extra_context or {})
 
         request.current_app = self.name
+        context["title"] = app_settings.ERP_ADMIN_INDEX_TITLE
 
         return TemplateResponse(
             request, self.index_template or "admin/index.html", context
         )
 
     def each_context(self, request):
         context = super(RaAdminSiteBase, self).each_context(request)
```

### Comparing `django-erp-framework-0.9.1/erp_framework/admin/forms.py` & `django-erp-framework-0.9.11/erp_framework/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/admin/helpers.py` & `django-erp-framework-0.9.11/erp_framework/admin/helpers.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/admin/templatetags/erp_reporting_tags.py` & `django-erp-framework-0.9.11/erp_framework/reporting/templatetags/erp_reporting_tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 
 from erp_framework.base import app_settings
 
 register = template.Library()
 
 
 @register.simple_tag(takes_context=True)
-def render_navigation_menu(context):
-    navigation_class = import_string(app_settings.RA_NAVIGATION_CLASS)
-    request = context["request"]
-    admin_site = context["admin_site"]
-    return mark_safe(navigation_class.get_menu(context, request, admin_site))
-
-
-@register.simple_tag(takes_context=True)
 def render_reports_menu(context):
     request = context["request"]
     is_in_reports = False
     active_base_model = ""
     if request.path.startswith("/reports/"):
         is_in_reports = True
         active_base_model = [x for x in request.path.split("/") if x][1]
@@ -67,7 +59,24 @@
     css_class = css_class or "active"
     current_base_model_name = context["current_base_model_name"]
     return (
         css_class
         if current_base_model_name == base_model._meta.model_name.lower()
         else ""
     )
+
+
+@register.simple_tag
+def get_html_panel(report, template_name="", **kwargs):
+    kwargs["report"] = report
+    if not report:
+        raise ValueError(
+            "report argument is empty. Are you sure you're using the correct report name"
+        )
+
+    # No chart argument default to True if no charts in reports
+    kwargs.setdefault("no_chart", not bool(report.chart_settings))
+
+    template = get_template(
+        template_name or "erp_framework/report_widget_template.html"
+    )
+    return template.render(context=kwargs)
```

### Comparing `django-erp-framework-0.9.1/erp_framework/admin/templatetags/suit_menu.py` & `django-erp-framework-0.9.11/erp_framework/reporting/templatetags/_suit_menu.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/apps.py` & `django-erp-framework-0.9.11/erp_framework/apps.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/base/app_settings.py` & `django-erp-framework-0.9.11/erp_framework/base/app_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,41 +12,26 @@
 # def get_end_of_this_year():
 #     d = datetime.datetime.today()
 #     return datetime.datetime(d.year + 1, 1, 1, 0, 0, 0, 0, pytz.timezone(settings.TIME_ZONE))
 
 
 import datetime
 
-ERP_FRAMEWORK_SETTING_DEFAULT = {
+ERP_FRAMEWORK_SETTINGS = {
     "site_name": "ERP Framework System",
     "site_header": "ERP Framework System",
-    "index_title": "ERP Framework Dashboard",
+    "index_title": "Dashboard Home",
+    "index_template": "",
+    # a function to control be dbfield on all instances, Saves you time to subclass ifonly you need to add a help text or something
+    "admin_default_formfield_for_dbfield": "erp_framework.base.helpers.default_formfield_for_dbfield",
 }
 
-ERP_FRAMEWORK_SETTINGS = getattr(
-    settings, "ERP_FRAMEWORK_SETTINGS", ERP_FRAMEWORK_SETTING_DEFAULT
-)
-
+USER_FRAMEWORK_SETTINGS = getattr(settings, "ERP_FRAMEWORK_SETTINGS", {})
 
-"""
-Documented
-"""
-# a function to control be dbfield on all instances, Saves you time to subclass ifonly you need to add a help text or something
-RA_FORMFIELD_FOR_DBFIELD_FUNC = getattr(
-    settings,
-    "RA_FORMFIELD_FOR_DBFIELD_FUNC",
-    "erp_framework.base.helpers.default_formfield_for_dbfield",
-)
-RA_FORMFIELD_FOR_DBFIELD_FUNC = get_callable(RA_FORMFIELD_FOR_DBFIELD_FUNC)
-# ------
-
-# Navigation class
-RA_NAVIGATION_CLASS = getattr(
-    settings, "RA_NAVIGATION_CLASS", "erp_framework.utils.navigation.RaSuitMenu"
-)
+ERP_FRAMEWORK_SETTINGS.update(USER_FRAMEWORK_SETTINGS)
 
 """
 UnDocumented
 """
 
 RA_ENABLE_ADMIN_DELETE_ALL = getattr(settings, "RA_ENABLE_ADMIN_DELETE_ALL", False)
 
@@ -72,31 +57,36 @@
 
 # Style
 RA_THEME = getattr(settings, "RA_THEME", "admin")
 
 # Admin Looks
 from django.utils.translation import gettext_lazy as _
 
-RA_ADMIN_INDEX_TEMPLATE = getattr(
-    settings, "RA_ADMIN_INDEX_PAGE", f"{RA_THEME}/index.html"
-)
 RA_ADMIN_APP_INDEX_TEMPLATE = getattr(
     settings, "RA_ADMIN_APP_INDEX_PAGE", f"{RA_THEME}/app_index.html"
 )
 RA_ADMIN_LOGIN_TEMPLATE = getattr(
     settings, "RA_ADMIN_LOGIN_TEMPLATE", f"{RA_THEME}/login.html"
 )
 RA_ADMIN_LOGGED_OUT_TEMPLATE = getattr(
     settings, "RA_ADMIN_LOGIN_TEMPLATE", f"{RA_THEME}/logged_out.html"
 )
 
 RA_ADMIN_SITE_CLASS = getattr(
     settings, "RA_ADMIN_SITE_CLASS", "erp_framework.admin.admin.RaAdminSite"
 )
+# correct
+ERP_ADMIN_SITE_TITLE = ERP_FRAMEWORK_SETTINGS.get("site_name", "ERP Framework System")
+
+ERP_ADMIN_SITE_HEADER = ERP_FRAMEWORK_SETTINGS.get("site_name", "ERP Framework Header")
 
-RA_ADMIN_SITE_TITLE = ERP_FRAMEWORK_SETTINGS.get("site_name", "ERP Framework System")
+ERP_ADMIN_INDEX_TITLE = ERP_FRAMEWORK_SETTINGS.get("index_title", "")
 
-RA_ADMIN_SITE_HEADER = ERP_FRAMEWORK_SETTINGS.get("site_name", "ERP Framework System")
+ERP_ADMIN_INDEX_TEMPLATE = ERP_FRAMEWORK_SETTINGS.get("index_template", "")
+
+ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC = ERP_FRAMEWORK_SETTINGS.get(
+    "admin_default_formfield_for_dbfield", ""
+)
 
-RA_ADMIN_INDEX_TITLE = ERP_FRAMEWORK_SETTINGS.get(
-    "index_title", "ERP Framework Dashboard"
+ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC = get_callable(
+    ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC
 )
```

### Comparing `django-erp-framework-0.9.1/erp_framework/base/helpers.py` & `django-erp-framework-0.9.11/erp_framework/base/helpers.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/base/models.py` & `django-erp-framework-0.9.11/erp_framework/base/models.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/base/registry.py` & `django-erp-framework-0.9.11/erp_framework/base/registry.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/base/widgets.py` & `django-erp-framework-0.9.11/erp_framework/base/widgets.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/checks.py` & `django-erp-framework-0.9.11/erp_framework/checks.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/reporting/forms.py` & `django-erp-framework-0.9.11/erp_framework/reporting/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/reporting/printing.py` & `django-erp-framework-0.9.11/erp_framework/reporting/printing.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/reporting/registry.py` & `django-erp-framework-0.9.11/erp_framework/reporting/registry.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/reporting/views.py` & `django-erp-framework-0.9.11/erp_framework/reporting/views.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/utils/permissions.py` & `django-erp-framework-0.9.11/erp_framework/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/erp_framework/utils/views.py` & `django-erp-framework-0.9.11/erp_framework/utils/views.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.1/setup.cfg` & `django-erp-framework-0.9.11/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
-license_file = LICENSE
+license_files = LICENSE,
 name = django-erp-framework
 version = attr: erp_framework.__version__
-author = Ra Systems
+author = Ramez Issac
 author_email = ramez@rasystems.io
 description = A light-weight effective Django based framework to create diverse business applications
 long_description = file:README.rst
 long_description_content_type = text/x-rst
-url = https://github.com/ra-systems/RA
+url = https://github.com/RamezIssac/django-erp-framework
 project_urls = 
 	Travis CI = https://travis-ci.org/ra-systems/RA/
 	Documentation = https://django-erp-framework.readthedocs.io/en/latest/
 	Source = https://github.com/ra-systems/RA
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```


# Comparing `tmp/django-erp-framework-0.9.11.tar.gz` & `tmp/django-erp-framework-0.9.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-erp-framework-0.9.11.tar", last modified: Mon May  8 15:21:57 2023, max compression
+gzip compressed data, was "django-erp-framework-0.9.12.tar", last modified: Mon May  8 15:25:48 2023, max compression
```

## Comparing `django-erp-framework-0.9.11.tar` & `django-erp-framework-0.9.12.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/
--rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-0.9.11/LICENSE
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-0.9.11/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3352 2023-05-06 12:34:52.000000 django-erp-framework-0.9.11/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/django_erp_framework.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1724 2023-05-08 15:21:57.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      205 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/django_erp_framework.egg-info/top_level.txt
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       99 2023-05-08 15:21:56.000000 django-erp-framework-0.9.11/erp_framework/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/activity/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8367 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/activity/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/0002_auto_20200711_1253.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/0003_alter_myactivity_options.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/activity/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.030173 django-erp-framework-0.9.11/erp_framework/admin/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       62 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    51303 2023-05-08 14:12:13.000000 django-erp-framework-0.9.11/erp_framework/admin/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7542 2023-05-08 14:10:04.000000 django-erp-framework-0.9.11/erp_framework/admin/base.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      667 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/admin/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      618 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/base/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2933 2023-05-08 14:23:36.000000 django-erp-framework-0.9.11/erp_framework/base/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7609 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    16862 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3415 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/registry.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1726 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/base/widgets.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2422 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/checks.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/contrib/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/contrib/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/contrib/jazzmin_integration/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/contrib/jazzmin_integration/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      346 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      164 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/printing.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5552 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/registry.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      665 2023-05-08 14:33:00.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/_ra_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    18435 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/_suit_menu.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2683 2023-05-08 14:17:14.000000 django-erp-framework-0.9.11/erp_framework/reporting/templatetags/erp_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    26830 2023-05-07 05:11:23.000000 django-erp-framework-0.9.11/erp_framework/reporting/views.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/erp_framework/utils/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      454 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/navigation.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3937 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/permissions.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-0.9.11/erp_framework/utils/views.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1782 2023-05-08 15:21:57.034173 django-erp-framework-0.9.11/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-0.9.11/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-0.9.12/LICENSE
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-0.9.12/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3352 2023-05-06 12:34:52.000000 django-erp-framework-0.9.12/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.962422 django-erp-framework-0.9.12/django_erp_framework.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1724 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      204 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/top_level.txt
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.962422 django-erp-framework-0.9.12/erp_framework/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       99 2023-05-08 15:25:37.000000 django-erp-framework-0.9.12/erp_framework/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.962422 django-erp-framework-0.9.12/erp_framework/activity/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8367 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/activity/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/0002_auto_20200711_1253.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/0003_alter_myactivity_options.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/models.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/admin/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       62 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    51303 2023-05-08 14:12:13.000000 django-erp-framework-0.9.12/erp_framework/admin/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7542 2023-05-08 14:10:04.000000 django-erp-framework-0.9.12/erp_framework/admin/base.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      667 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      618 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/base/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2933 2023-05-08 14:23:36.000000 django-erp-framework-0.9.12/erp_framework/base/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7609 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    16862 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3415 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/registry.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1726 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/widgets.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2422 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/checks.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/contrib/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/contrib/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/contrib/jazzmin_integration/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/contrib/jazzmin_integration/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      346 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      164 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/printing.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5552 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      665 2023-05-08 14:33:00.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/_ra_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    18435 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/_suit_menu.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2683 2023-05-08 14:17:14.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/erp_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    26830 2023-05-07 05:11:23.000000 django-erp-framework-0.9.12/erp_framework/reporting/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/utils/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      454 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/navigation.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3937 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/permissions.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/views.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1781 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-0.9.12/setup.py
```

### Comparing `django-erp-framework-0.9.11/LICENSE` & `django-erp-framework-0.9.12/LICENSE`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/PKG-INFO` & `django-erp-framework-0.9.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.11
+Version: 0.9.12
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/RamezIssac/django-erp-framework
 Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
```

### Comparing `django-erp-framework-0.9.11/README.rst` & `django-erp-framework-0.9.12/README.rst`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/django_erp_framework.egg-info/PKG-INFO` & `django-erp-framework-0.9.12/django_erp_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.11
+Version: 0.9.12
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/RamezIssac/django-erp-framework
 Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
```

### Comparing `django-erp-framework-0.9.11/django_erp_framework.egg-info/SOURCES.txt` & `django-erp-framework-0.9.12/django_erp_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/activity/admin.py` & `django-erp-framework-0.9.12/erp_framework/activity/admin.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/activity/migrations/0001_initial.py` & `django-erp-framework-0.9.12/erp_framework/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/admin/admin.py` & `django-erp-framework-0.9.12/erp_framework/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/admin/base.py` & `django-erp-framework-0.9.12/erp_framework/admin/base.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/admin/forms.py` & `django-erp-framework-0.9.12/erp_framework/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/admin/helpers.py` & `django-erp-framework-0.9.12/erp_framework/admin/helpers.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/apps.py` & `django-erp-framework-0.9.12/erp_framework/apps.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/base/app_settings.py` & `django-erp-framework-0.9.12/erp_framework/base/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/base/helpers.py` & `django-erp-framework-0.9.12/erp_framework/base/helpers.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/base/models.py` & `django-erp-framework-0.9.12/erp_framework/base/models.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/base/registry.py` & `django-erp-framework-0.9.12/erp_framework/base/registry.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/base/widgets.py` & `django-erp-framework-0.9.12/erp_framework/base/widgets.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/checks.py` & `django-erp-framework-0.9.12/erp_framework/checks.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/reporting/forms.py` & `django-erp-framework-0.9.12/erp_framework/reporting/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/reporting/printing.py` & `django-erp-framework-0.9.12/erp_framework/reporting/printing.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/reporting/registry.py` & `django-erp-framework-0.9.12/erp_framework/reporting/registry.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/reporting/templatetags/_ra_tags.py` & `django-erp-framework-0.9.12/erp_framework/reporting/templatetags/_ra_tags.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/reporting/templatetags/_suit_menu.py` & `django-erp-framework-0.9.12/erp_framework/reporting/templatetags/_suit_menu.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/reporting/templatetags/erp_reporting_tags.py` & `django-erp-framework-0.9.12/erp_framework/reporting/templatetags/erp_reporting_tags.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/reporting/views.py` & `django-erp-framework-0.9.12/erp_framework/reporting/views.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/utils/permissions.py` & `django-erp-framework-0.9.12/erp_framework/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/erp_framework/utils/views.py` & `django-erp-framework-0.9.12/erp_framework/utils/views.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.11/setup.cfg` & `django-erp-framework-0.9.12/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -48,13 +48,13 @@
 	django-crequest>=2018.5.11
 	django-tabular-permissions
 	django-crispy-forms
 	dateutils
 	django-reversion>=3.0.5
 	django-slick-reporting
 	django-jazzmin>=2.5.0
-	django-compressor>==2.3
+	django-compressor>=2.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


# Comparing `tmp/djangocms-page-meta-1.1.0.tar.gz` & `tmp/djangocms-page-meta-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-page-meta-1.1.0.tar", last modified: Sat Aug 27 17:48:59 2022, max compression
+gzip compressed data, was "djangocms-page-meta-1.2.0.tar", last modified: Mon May  8 18:04:55 2023, max compression
```

## Comparing `djangocms-page-meta-1.1.0.tar` & `djangocms-page-meta-1.2.0.tar`

### file list

```diff
@@ -1,94 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.225343 djangocms-page-meta-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5465 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9473 2022-08-27 17:48:59.225343 djangocms-page-meta-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.213342 djangocms-page-meta-1.1.0/djangocms_page_meta/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/cms_toolbars.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.209342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.201342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.217342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.201342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.217342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.201342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.217342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4801 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.201342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.217342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.205342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.217342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4628 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.205342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.217342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4877 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.205342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.221342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4909 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.205342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.221342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4013 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.205342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.221342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.209342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.221342 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.225343 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     7999 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0002_auto_20150807_0936.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0003_auto_20151220_1734.py
--rw-r--r--   0 runner    (1001) docker     (121)     3696 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0004_auto_20160409_1852.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0005_pagemeta_fb_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0006_auto_20160423_1859.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0007_auto_20160530_2257.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0008_auto_20160609_0754.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0009_auto_20171230_1954.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0010_auto_20180108_2316.py
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0011_auto_20190218_1010.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0012_auto_20200706_1230.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0013_auto_20200821_1457.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6917 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.209342 djangocms-page-meta-1.1.0/djangocms_page_meta/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.209342 djangocms-page-meta-1.1.0/djangocms_page_meta/static/djangocms_page_meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.225343 djangocms-page-meta-1.1.0/djangocms_page_meta/static/djangocms_page_meta/css/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/static/djangocms_page_meta/css/djangocms_page_meta_admin.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.209342 djangocms-page-meta-1.1.0/djangocms_page_meta/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.225343 djangocms-page-meta-1.1.0/djangocms_page_meta/templates/djangocms_page_meta/
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/templates/djangocms_page_meta/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.225343 djangocms-page-meta-1.1.0/djangocms_page_meta/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/templatetags/page_meta_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     6382 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/djangocms_page_meta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:48:59.217342 djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9473 2022-08-27 17:48:59.000000 djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-08-27 17:48:59.000000 djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:48:59.000000 djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:48:45.000000 djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-27 17:48:59.000000 djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-27 17:48:59.000000 djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-08-27 17:48:59.229343 djangocms-page-meta-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 17:48:14.000000 djangocms-page-meta-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/cms_toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0002_auto_20150807_0936.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0003_auto_20151220_1734.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0004_auto_20160409_1852.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0005_pagemeta_fb_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0006_auto_20160423_1859.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0007_auto_20160530_2257.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0008_auto_20160609_0754.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0009_auto_20171230_1954.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0010_auto_20180108_2316.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0011_auto_20190218_1010.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0012_auto_20200706_1230.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0013_auto_20200821_1457.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/static/djangocms_page_meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/djangocms_page_meta/static/djangocms_page_meta/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/static/djangocms_page_meta/css/djangocms_page_meta_admin.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.835703 djangocms-page-meta-1.2.0/djangocms_page_meta/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/djangocms_page_meta/templates/djangocms_page_meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/templates/djangocms_page_meta/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/djangocms_page_meta/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/templatetags/page_meta_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/djangocms_page_meta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.839703 djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-08 18:04:55.000000 djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-08 18:04:55.000000 djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:04:55.000000 djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:04:42.000000 djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 18:04:55.000000 djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 18:04:55.000000 djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:04:55.843703 djangocms-page-meta-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/tests/test_adminpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-08 18:04:16.000000 djangocms-page-meta-1.2.0/tests/test_toolbar.py
```

### Comparing `djangocms-page-meta-1.1.0/AUTHORS.rst` & `djangocms-page-meta-1.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/CONTRIBUTING.rst` & `djangocms-page-meta-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/HISTORY.rst` & `djangocms-page-meta-1.2.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+1.2.0 (2023-05-08)
+==================
+
+Features
+--------
+
+- Update GH actions / linting configuration (#157)
+- Add support for Django 4.2 / django CMS 3.11
+
+
 1.1.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Skip creating toolbar item in page types (#150)
```

### Comparing `djangocms-page-meta-1.1.0/LICENSE` & `djangocms-page-meta-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/PKG-INFO` & `djangocms-page-meta-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: djangocms-page-meta
-Version: 1.1.0
+Version: 1.2.0
 Summary: OpenGraph, Twitter Card and Schema.org snippet tags for django CMS 3 pages
 Home-page: https://github.com/nephila/djangocms-page-meta
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: BSD
 Project-URL: Documentation, https://djangocms-page-meta.readthedocs.io/
 Keywords: django cms,meta tags,OpenGraph,Twitter Cards,Schema.org,django-app-enabler addon
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ===================
 djangocms-page-meta
@@ -147,14 +149,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+1.2.0 (2023-05-08)
+==================
+
+Features
+--------
+
+- Update GH actions / linting configuration (#157)
+- Add support for Django 4.2 / django CMS 3.11
+
+
 1.1.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Skip creating toolbar item in page types (#150)
```

### Comparing `djangocms-page-meta-1.1.0/README.rst` & `djangocms-page-meta-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/admin.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cms.admin.pageadmin import PageAdmin
 from cms.extensions import PageExtensionAdmin, TitleExtensionAdmin
 from cms.utils import get_language_from_request
 from django.conf import settings
 from django.contrib import admin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from .forms import GenericAttributeInlineForm, TitleMetaAdminForm
 from .models import GenericMetaAttribute, PageMeta, TitleMeta
 
 
 class GenericAttributePageInline(admin.TabularInline):
     model = GenericMetaAttribute
@@ -19,14 +19,15 @@
 class GenericAttributeTitleInline(admin.TabularInline):
     model = GenericMetaAttribute
     form = GenericAttributeInlineForm
     fields = ("title", "attribute", "name", "value")
     extra = 1
 
 
+@admin.register(PageMeta)
 class PageMetaAdmin(PageExtensionAdmin):
     raw_id_fields = ("og_author",)
     inlines = (GenericAttributePageInline,)
     fieldsets = (
         (None, {"fields": ("image",)}),
         (
             _("OpenGraph"),
@@ -49,34 +50,29 @@
     def get_model_perms(self, request):
         """
         Return empty perms dict thus hiding the model from admin index.
         """
         return {}
 
 
-admin.site.register(PageMeta, PageMetaAdmin)
-
-
+@admin.register(TitleMeta)
 class TitleMetaAdmin(TitleExtensionAdmin):
     form = TitleMetaAdminForm
     inlines = (GenericAttributeTitleInline,)
 
     class Media:
         css = {"all": ("{}djangocms_page_meta/css/{}".format(settings.STATIC_URL, "djangocms_page_meta_admin.css"),)}
 
     def get_model_perms(self, request):
         """
         Return empty perms dict thus hiding the model from admin index.
         """
         return {}
 
 
-admin.site.register(TitleMeta, TitleMetaAdmin)
-
-
 # Monkey patch the PageAdmin with a new get_form method
 _BASE_PAGEADMIN__GET_FORM = PageAdmin.get_form
 
 
 def get_form(self, request, obj=None, **kwargs):
     """
     Patched method for PageAdmin.get_form.
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/cms_toolbars.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/cms_toolbars.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cms.cms_toolbars import PAGE_MENU_SECOND_BREAK
 from cms.toolbar.items import Break
 from cms.toolbar_base import CMSToolbar
 from cms.toolbar_pool import toolbar_pool
 from cms.utils.i18n import get_language_list, get_language_object
 from cms.utils.permissions import has_page_permission
 from django.urls import NoReverseMatch, reverse
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from .models import PageMeta, TitleMeta
 
 try:
     from cms.utils import get_cms_setting
 except ImportError:
     from cms.utils.conf import get_cms_setting
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/forms.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/bg/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.mo` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.po` & `djangocms-page-meta-1.2.0/djangocms_page_meta/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0001_initial.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import filer.fields.file
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("cms", "0003_auto_20140926_2347"),
         ("filer", "0001_initial"),
     ]
 
     operations = [
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0002_auto_20150807_0936.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0002_auto_20150807_0936.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="pagemeta",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0003_auto_20151220_1734.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0003_auto_20151220_1734.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0002_auto_20150807_0936"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="pagemeta",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0004_auto_20160409_1852.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0004_auto_20160409_1852.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 1.9.3 on 2016-04-09 16:52
 
 from django.db import migrations, models
 from meta import settings
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0003_auto_20151220_1734"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="pagemeta",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0006_auto_20160423_1859.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0006_auto_20160423_1859.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0005_pagemeta_fb_pages"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="GenericMetaAttribute",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0007_auto_20160530_2257.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0007_auto_20160530_2257.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.9.6 on 2016-05-30 20:57
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0006_auto_20160423_1859"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="genericmetaattribute",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0009_auto_20171230_1954.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0009_auto_20171230_1954.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.11.8 on 2017-12-30 18:54
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0008_auto_20160609_0754"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="pagemeta",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0010_auto_20180108_2316.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0010_auto_20180108_2316.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.11.9 on 2018-01-08 22:16
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0009_auto_20171230_1954"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="titlemeta",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0011_auto_20190218_1010.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0011_auto_20190218_1010.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.db.models.deletion
 import filer.fields.file
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0010_auto_20180108_2316"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="genericmetaattribute",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0012_auto_20200706_1230.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0012_auto_20200706_1230.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2 on 2020-07-06 12:30
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0011_auto_20190218_1010"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="pagemeta",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/migrations/0013_auto_20200821_1457.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/migrations/0013_auto_20200821_1457.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2 on 2020-08-21 14:57
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_meta", "0012_auto_20200706_1230"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="titlemeta",
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/models.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cms.extensions.extension_pool import extension_pool
 from cms.models import Page, Title
 from django.conf import settings
 from django.core.cache import cache
 from django.db import models
 from django.db.models.signals import post_save, pre_delete
 from django.dispatch import receiver
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from filer.fields.file import FilerFileField
 from meta import settings as meta_settings
 
 from .utils import get_cache_key, get_metatags
 
 try:
     from aldryn_snake.template_api import registry
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/templates/djangocms_page_meta/meta.html` & `djangocms-page-meta-1.2.0/djangocms_page_meta/templates/djangocms_page_meta/meta.html`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/templatetags/page_meta_tags.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/templatetags/page_meta_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta/utils.py` & `djangocms-page-meta-1.2.0/djangocms_page_meta/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/PKG-INFO` & `djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: djangocms-page-meta
-Version: 1.1.0
+Version: 1.2.0
 Summary: OpenGraph, Twitter Card and Schema.org snippet tags for django CMS 3 pages
 Home-page: https://github.com/nephila/djangocms-page-meta
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: BSD
 Project-URL: Documentation, https://djangocms-page-meta.readthedocs.io/
 Keywords: django cms,meta tags,OpenGraph,Twitter Cards,Schema.org,django-app-enabler addon
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ===================
 djangocms-page-meta
@@ -147,14 +149,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+1.2.0 (2023-05-08)
+==================
+
+Features
+--------
+
+- Update GH actions / linting configuration (#157)
+- Add support for Django 4.2 / django CMS 3.11
+
+
 1.1.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Skip creating toolbar item in page types (#150)
```

### Comparing `djangocms-page-meta-1.1.0/djangocms_page_meta.egg-info/SOURCES.txt` & `djangocms-page-meta-1.2.0/djangocms_page_meta.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -55,8 +55,12 @@
 djangocms_page_meta/migrations/0011_auto_20190218_1010.py
 djangocms_page_meta/migrations/0012_auto_20200706_1230.py
 djangocms_page_meta/migrations/0013_auto_20200821_1457.py
 djangocms_page_meta/migrations/__init__.py
 djangocms_page_meta/static/djangocms_page_meta/css/djangocms_page_meta_admin.css
 djangocms_page_meta/templates/djangocms_page_meta/meta.html
 djangocms_page_meta/templatetags/__init__.py
-djangocms_page_meta/templatetags/page_meta_tags.py
+djangocms_page_meta/templatetags/page_meta_tags.py
+tests/test_adminpage.py
+tests/test_general.py
+tests/test_templatetags.py
+tests/test_toolbar.py
```

### Comparing `djangocms-page-meta-1.1.0/setup.cfg` & `djangocms-page-meta-1.2.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-[bumpversion]
-current_version = 1.1.0
-parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.?)(?P<release>[a-z]*)(?P<relver>\d*)
-serialize = 
-	{major}.{minor}.{patch}.{release}{relver}
-	{major}.{minor}.{patch}
-commit = True
-tag = True
-sign_tags = True
-tag_name = {new_version}
-message = Release {new_version}
-
-[bumpversion:part:release]
-optional_value = gamma
-values = 
-	dev
-	a
-	b
-	rc
-	gamma
-
-[bumpversion:file:djangocms_page_meta/__init__.py]
-
 [metadata]
 name = djangocms-page-meta
 version = attr: djangocms_page_meta.__version__
 url = https://github.com/nephila/djangocms-page-meta
 project_urls = 
 	Documentation = https://djangocms-page-meta.readthedocs.io/
 author = Iacopo Spalletti
@@ -38,21 +15,23 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Framework :: Django
-	Framework :: Django :: 2.2
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 install_requires = 
 	django-cms>=3.7
 	django-meta>=2.0.0
 	django-filer>=1.2
@@ -65,20 +44,18 @@
 
 [options.package_data]
 * = *.txt, *.rst
 djangocms_page_meta = *.html *.png *.gif *js *jpg *jpeg *svg *py *mo *po
 
 [options.extras_require]
 docs = 
-	django<4.0
+	django<5.0
+	sphinx>2,<5
 	djangocms-page-tags
 
-[upload]
-repository = https://upload.pypi.org/legacy/
-
 [sdist]
 formats = zip
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
```


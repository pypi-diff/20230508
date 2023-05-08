# Comparing `tmp/djangocms-page-sitemap-1.1.0.tar.gz` & `tmp/djangocms-page-sitemap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-page-sitemap-1.1.0.tar", last modified: Sat Aug 27 17:47:09 2022, max compression
+gzip compressed data, was "djangocms-page-sitemap-1.2.0.tar", last modified: Mon May  8 18:30:16 2023, max compression
```

## Comparing `djangocms-page-sitemap-1.1.0.tar` & `djangocms-page-sitemap-1.2.0.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8994 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5556 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.921497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.917497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.913497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.913497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.913497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.913497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.913497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.913497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.917497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.917497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.917497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0002_auto_20151018_1451.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0003_auto_20151018_1612.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0004_auto_20180202_1044.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0005_auto_20180324_1050.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/sitemap.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/sitemap_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/templatetags/robots_index.py
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:47:09.925497 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8994 2022-08-27 17:47:09.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-08-27 17:47:09.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:47:09.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:46:58.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-27 17:47:09.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-27 17:47:09.000000 djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-27 17:47:09.929497 djangocms-page-sitemap-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 17:46:35.000000 djangocms-page-sitemap-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.129314 djangocms-page-sitemap-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-05-08 18:30:16.129314 djangocms-page-sitemap-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.121314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.117313 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.125314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0002_auto_20151018_1451.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0003_auto_20151018_1612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0004_auto_20180202_1044.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0005_auto_20180324_1050.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/sitemap_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.129314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/templatetags/robots_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.121314 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-05-08 18:30:16.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-08 18:30:16.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:30:16.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:30:02.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 18:30:16.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 18:30:16.000000 djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-08 18:30:16.129314 djangocms-page-sitemap-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:30:16.129314 djangocms-page-sitemap-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/tests/test_sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-08 18:29:40.000000 djangocms-page-sitemap-1.2.0/tests/test_toolbar.py
```

### Comparing `djangocms-page-sitemap-1.1.0/CONTRIBUTING.rst` & `djangocms-page-sitemap-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/HISTORY.rst` & `djangocms-page-sitemap-1.2.0/HISTORY.rst`

 * *Files 8% similar despite different names*

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
+- Update GH actions / linting configuration (#79)
+- Add support for Django 4.2 / django CMS 3.11
+
+
 1.1.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Fix error when populating the toolbar on page types (#67)
```

### Comparing `djangocms-page-sitemap-1.1.0/LICENSE` & `djangocms-page-sitemap-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/PKG-INFO` & `djangocms-page-sitemap-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: djangocms-page-sitemap
-Version: 1.1.0
+Version: 1.2.0
 Summary: django CMS page extension to handle sitemap customization
 Home-page: https://github.com/nephila/djangocms-page-sitemap
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: BSD
 Project-URL: Documentation, https://djangocms-page-sitemap.readthedocs.io/
 Keywords: django cms,sitemap,django-app-enabler addon
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ======================
 djangocms-page-sitemap
@@ -213,14 +215,24 @@
 
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
+- Update GH actions / linting configuration (#79)
+- Add support for Django 4.2 / django CMS 3.11
+
+
 1.1.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Fix error when populating the toolbar on page types (#67)
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: djangocms-page-sitemap Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: djangocms-page-sitemap Version: 1.2.0 Summary:
 django CMS page extension to handle sitemap customization Home-page: https://
 github.com/nephila/djangocms-page-sitemap Author: Iacopo Spalletti Author-
 email: i.spalletti@nephila.digital License: BSD Project-URL: Documentation,
 https://djangocms-page-sitemap.readthedocs.io/ Keywords: django
 cms,sitemap,django-app-enabler addon Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Django Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Framework :: Django Classifier:
-Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier:
-Framework :: Django :: 3.2 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7 Description-Content-Type: text/x-rst Provides-Extra:
-docs License-File: LICENSE ====================== djangocms-page-sitemap
-====================== |Gitter| |PyPiVersion| |PyVersion| |Status|
-|TestCoverage| |CodeClimate| |License| django CMS page extension to handle
-sitemap customization Support Python version: * Python 3.7, 3.8, 3.9, 3.10
-Supported Django versions: * Django 2.2, 3.2 Supported django CMS versions: *
-django CMS 3.7 - 3.10 .. note:: djangocms-page-sitemap 0.8 has been relicensed
-with BSD license. .. note:: djangocms-page-sitemap 1.0 dropped compatibility
-with Python 2 and Django < 2.2 ******** Features ******** * Support for
-changefreq and priority customisation per-page * Option to exclude a page from
-the Sitemap * Values are cached * django CMS toolbar integration * Available on
-Divio Cloud ********** Quickstart ********** * Install djangocms-page-sitemap::
-pip install djangocms-page-sitemap * Add to ``INSTALLED_APPS`` with
-``django.contrib.sitemaps``: .. code-block:: python INSTALLED_APPS = [ ...
+Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.1 Classifier:
+Framework :: Django :: 4.2 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/x-rst Provides-Extra: docs License-File: LICENSE ======================
+djangocms-page-sitemap ====================== |Gitter| |PyPiVersion|
+|PyVersion| |Status| |TestCoverage| |CodeClimate| |License| django CMS page
+extension to handle sitemap customization Support Python version: * Python 3.7,
+3.8, 3.9, 3.10 Supported Django versions: * Django 2.2, 3.2 Supported django
+CMS versions: * django CMS 3.7 - 3.10 .. note:: djangocms-page-sitemap 0.8 has
+been relicensed with BSD license. .. note:: djangocms-page-sitemap 1.0 dropped
+compatibility with Python 2 and Django < 2.2 ******** Features ******** *
+Support for changefreq and priority customisation per-page * Option to exclude
+a page from the Sitemap * Values are cached * django CMS toolbar integration *
+Available on Divio Cloud ********** Quickstart ********** * Install djangocms-
+page-sitemap:: pip install djangocms-page-sitemap * Add to ``INSTALLED_APPS``
+with ``django.contrib.sitemaps``: .. code-block:: python INSTALLED_APPS = [ ...
 "django.contrib.sitemaps", "djangocms_page_sitemap", ] * Load it into the
 urlconf, eventually removing django CMS sitemap: .. code-block:: python ...
 urlpatterns = [ path("admin/", admin.site.urls), ... path("", include
 ("djangocms_page_sitemap.sitemap_urls")), ... ] * Load ``robots_index``
 templatetag and add it to the page in the head tag of the django CMS pages (or
 in a shared base template): .. code-block:: html+django {% load robots_index %}
 ...
@@ -78,38 +79,40 @@
 master.svg?style=flat-square :target: https://coveralls.io/r/nephila/djangocms-
 page-sitemap?branch=master :alt: Test coverage .. |License| image:: https://
 img.shields.io/github/license/nephila/djangocms-page-sitemap.svg?style=flat-
 square :target: https://pypi.python.org/pypi/djangocms-page-sitemap/ :alt:
 License .. |CodeClimate| image:: https://codeclimate.com/github/nephila/
 djangocms-page-sitemap/badges/gpa.svg?style=flat-square :target: https://
 codeclimate.com/github/nephila/djangocms-page-sitemap :alt: Code Climate .. :
-changelog: ******* History ******* .. towncrier release notes start 1.1.0
-(2022-08-27) ================== Bugfixes -------- - Fix error when populating
-the toolbar on page types (#67) - Fixed serialization issue when trying to
-upload the addon to Divio Cloud. (#73) - Add support for Django 3.2 / django
-CMS 3.10 (#74) 1.0.0 (2020-12-21) ================== Features -------- - Add
-support for django-app-enabler (#63) - Update tooling and drop Python 2 /
-Django < 2.2 compatibility (#10208) 0.8.1 (2020-05-02) ================== *
-Enable django CMS 3.7.2 on python 3 0.8.0 (2020-01-12) ================== *
-Relicense under BSD license 0.7.0 (2019-08-22) ================== * Add
-compatibility with Django 2.2 * Drop compatibility with Django < 1.11 * Drop
-compatibility with django CMS < 3.6 * Move to django-app-helper 0.6.0 (2019-07-
-13) ================== * Drop compatibility with Django < 1.11 * Drop
-compatibility with Python 3 < 3.5 0.5.4 (2019-07-13) ================== * Fix
+changelog: ******* History ******* .. towncrier release notes start 1.2.0
+(2023-05-08) ================== Features -------- - Update GH actions / linting
+configuration (#79) - Add support for Django 4.2 / django CMS 3.11 1.1.0 (2022-
+08-27) ================== Bugfixes -------- - Fix error when populating the
+toolbar on page types (#67) - Fixed serialization issue when trying to upload
+the addon to Divio Cloud. (#73) - Add support for Django 3.2 / django CMS 3.10
+(#74) 1.0.0 (2020-12-21) ================== Features -------- - Add support for
+django-app-enabler (#63) - Update tooling and drop Python 2 / Django < 2.2
+compatibility (#10208) 0.8.1 (2020-05-02) ================== * Enable django
+CMS 3.7.2 on python 3 0.8.0 (2020-01-12) ================== * Relicense under
+BSD license 0.7.0 (2019-08-22) ================== * Add compatibility with
+Django 2.2 * Drop compatibility with Django < 1.11 * Drop compatibility with
+django CMS < 3.6 * Move to django-app-helper 0.6.0 (2019-07-13)
+================== * Drop compatibility with Django < 1.11 * Drop compatibility
+with Python 3 < 3.5 0.5.4 (2019-07-13) ================== * Fix error when
+page_robots is executed outside a request * Fix tox for older environments
+0.5.3 (2019-03-09) ================== * Add Django 2.0, 2.1 support * Add
+django CMS 3.6 support * Apply workaround to avoid triggering ``Page.site_id``
+deprecation warning 0.5.2 (2018-04-07) ================== * Make robots_extra
+not required 0.5.1 (2018-02-27) ================== * Fix error in migration
+dependencies 0.5.0 (2018-02-22) ================== * Add Django 1.11 support *
+Add django CMS 3.5 support * Package as Divio Cloud addon * Add support for
+noindex, noarchive robots meta tag 0.4.3 (2019-07-13) ================== * Fix
 error when page_robots is executed outside a request * Fix tox for older
-environments 0.5.3 (2019-03-09) ================== * Add Django 2.0, 2.1
-support * Add django CMS 3.6 support * Apply workaround to avoid triggering
-``Page.site_id`` deprecation warning 0.5.2 (2018-04-07) ================== *
-Make robots_extra not required 0.5.1 (2018-02-27) ================== * Fix
-error in migration dependencies 0.5.0 (2018-02-22) ================== * Add
-Django 1.11 support * Add django CMS 3.5 support * Package as Divio Cloud addon
-* Add support for noindex, noarchive robots meta tag 0.4.3 (2019-07-13)
-================== * Fix error when page_robots is executed outside a request *
-Fix tox for older environments 0.4.2 (2019-04-08) ================== * Add
-support for noindex, noarchive robots meta tag 0.4.1 (2016-12-02)
-================== * Add Django 1.10 support 0.4.0 (2016-10-26)
-================== * Drop compatibility with django CMS 3.1 and below, Django
-1.7 and below 0.3.1 (2015-10-18) ================== * Improve defaults 0.3.0
-(2015-10-18) ================== * Add Python 3.5 * Add option to exclude page
-from sitemap 0.2.0 (2015-08-15) ================== * Update to support django
-CMS 3.1 * Drop support for Django 1.4, 1.5 * Add support for Django 1.8 0.1.0
-(2014-08-26) ================== * Initial version.
+environments 0.4.2 (2019-04-08) ================== * Add support for noindex,
+noarchive robots meta tag 0.4.1 (2016-12-02) ================== * Add Django
+1.10 support 0.4.0 (2016-10-26) ================== * Drop compatibility with
+django CMS 3.1 and below, Django 1.7 and below 0.3.1 (2015-10-18)
+================== * Improve defaults 0.3.0 (2015-10-18) ================== *
+Add Python 3.5 * Add option to exclude page from sitemap 0.2.0 (2015-08-15)
+================== * Update to support django CMS 3.1 * Drop support for Django
+1.4, 1.5 * Add support for Django 1.8 0.1.0 (2014-08-26) ================== *
+Initial version.
```

### Comparing `djangocms-page-sitemap-1.1.0/README.rst` & `djangocms-page-sitemap-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/cms_toolbars.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.mo` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.mo` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.mo` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.mo` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.mo` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.mo` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/django.po` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0001_initial.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import django.core.validators
 from django.db import migrations, models
 
 from djangocms_page_sitemap.settings import PAGE_SITEMAP_CHANGEFREQ_LIST
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("cms", "__first__"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="PageSitemapProperties",
```

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0002_auto_20151018_1451.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0002_auto_20151018_1451.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.db import migrations, models
 
 from djangocms_page_sitemap.settings import PAGE_SITEMAP_CHANGEFREQ_LIST
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_sitemap", "0001_initial"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="pagesitemapproperties",
```

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0003_auto_20151018_1612.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0003_auto_20151018_1612.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import django.core.validators
 from django.db import migrations, models
 
 from djangocms_page_sitemap.settings import PAGE_SITEMAP_CHANGEFREQ_LIST
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_sitemap", "0002_auto_20151018_1451"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="pagesitemapproperties",
```

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0004_auto_20180202_1044.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0004_auto_20180202_1044.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.10.8 on 2018-02-02 09:44
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_sitemap", "0003_auto_20151018_1612"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="pagesitemapproperties",
```

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/migrations/0005_auto_20180324_1050.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/migrations/0005_auto_20180324_1050.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.11.10 on 2018-03-24 09:50
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_page_sitemap", "0004_auto_20180202_1044"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="pagesitemapproperties",
```

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/models.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/settings.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/sitemap.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap/templatetags/robots_index.py` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap/templatetags/robots_index.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/PKG-INFO` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: djangocms-page-sitemap
-Version: 1.1.0
+Version: 1.2.0
 Summary: django CMS page extension to handle sitemap customization
 Home-page: https://github.com/nephila/djangocms-page-sitemap
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: BSD
 Project-URL: Documentation, https://djangocms-page-sitemap.readthedocs.io/
 Keywords: django cms,sitemap,django-app-enabler addon
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ======================
 djangocms-page-sitemap
@@ -213,14 +215,24 @@
 
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
+- Update GH actions / linting configuration (#79)
+- Add support for Django 4.2 / django CMS 3.11
+
+
 1.1.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Fix error when populating the toolbar on page types (#67)
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: djangocms-page-sitemap Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: djangocms-page-sitemap Version: 1.2.0 Summary:
 django CMS page extension to handle sitemap customization Home-page: https://
 github.com/nephila/djangocms-page-sitemap Author: Iacopo Spalletti Author-
 email: i.spalletti@nephila.digital License: BSD Project-URL: Documentation,
 https://djangocms-page-sitemap.readthedocs.io/ Keywords: django
 cms,sitemap,django-app-enabler addon Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Django Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Framework :: Django Classifier:
-Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier:
-Framework :: Django :: 3.2 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7 Description-Content-Type: text/x-rst Provides-Extra:
-docs License-File: LICENSE ====================== djangocms-page-sitemap
-====================== |Gitter| |PyPiVersion| |PyVersion| |Status|
-|TestCoverage| |CodeClimate| |License| django CMS page extension to handle
-sitemap customization Support Python version: * Python 3.7, 3.8, 3.9, 3.10
-Supported Django versions: * Django 2.2, 3.2 Supported django CMS versions: *
-django CMS 3.7 - 3.10 .. note:: djangocms-page-sitemap 0.8 has been relicensed
-with BSD license. .. note:: djangocms-page-sitemap 1.0 dropped compatibility
-with Python 2 and Django < 2.2 ******** Features ******** * Support for
-changefreq and priority customisation per-page * Option to exclude a page from
-the Sitemap * Values are cached * django CMS toolbar integration * Available on
-Divio Cloud ********** Quickstart ********** * Install djangocms-page-sitemap::
-pip install djangocms-page-sitemap * Add to ``INSTALLED_APPS`` with
-``django.contrib.sitemaps``: .. code-block:: python INSTALLED_APPS = [ ...
+Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.1 Classifier:
+Framework :: Django :: 4.2 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/x-rst Provides-Extra: docs License-File: LICENSE ======================
+djangocms-page-sitemap ====================== |Gitter| |PyPiVersion|
+|PyVersion| |Status| |TestCoverage| |CodeClimate| |License| django CMS page
+extension to handle sitemap customization Support Python version: * Python 3.7,
+3.8, 3.9, 3.10 Supported Django versions: * Django 2.2, 3.2 Supported django
+CMS versions: * django CMS 3.7 - 3.10 .. note:: djangocms-page-sitemap 0.8 has
+been relicensed with BSD license. .. note:: djangocms-page-sitemap 1.0 dropped
+compatibility with Python 2 and Django < 2.2 ******** Features ******** *
+Support for changefreq and priority customisation per-page * Option to exclude
+a page from the Sitemap * Values are cached * django CMS toolbar integration *
+Available on Divio Cloud ********** Quickstart ********** * Install djangocms-
+page-sitemap:: pip install djangocms-page-sitemap * Add to ``INSTALLED_APPS``
+with ``django.contrib.sitemaps``: .. code-block:: python INSTALLED_APPS = [ ...
 "django.contrib.sitemaps", "djangocms_page_sitemap", ] * Load it into the
 urlconf, eventually removing django CMS sitemap: .. code-block:: python ...
 urlpatterns = [ path("admin/", admin.site.urls), ... path("", include
 ("djangocms_page_sitemap.sitemap_urls")), ... ] * Load ``robots_index``
 templatetag and add it to the page in the head tag of the django CMS pages (or
 in a shared base template): .. code-block:: html+django {% load robots_index %}
 ...
@@ -78,38 +79,40 @@
 master.svg?style=flat-square :target: https://coveralls.io/r/nephila/djangocms-
 page-sitemap?branch=master :alt: Test coverage .. |License| image:: https://
 img.shields.io/github/license/nephila/djangocms-page-sitemap.svg?style=flat-
 square :target: https://pypi.python.org/pypi/djangocms-page-sitemap/ :alt:
 License .. |CodeClimate| image:: https://codeclimate.com/github/nephila/
 djangocms-page-sitemap/badges/gpa.svg?style=flat-square :target: https://
 codeclimate.com/github/nephila/djangocms-page-sitemap :alt: Code Climate .. :
-changelog: ******* History ******* .. towncrier release notes start 1.1.0
-(2022-08-27) ================== Bugfixes -------- - Fix error when populating
-the toolbar on page types (#67) - Fixed serialization issue when trying to
-upload the addon to Divio Cloud. (#73) - Add support for Django 3.2 / django
-CMS 3.10 (#74) 1.0.0 (2020-12-21) ================== Features -------- - Add
-support for django-app-enabler (#63) - Update tooling and drop Python 2 /
-Django < 2.2 compatibility (#10208) 0.8.1 (2020-05-02) ================== *
-Enable django CMS 3.7.2 on python 3 0.8.0 (2020-01-12) ================== *
-Relicense under BSD license 0.7.0 (2019-08-22) ================== * Add
-compatibility with Django 2.2 * Drop compatibility with Django < 1.11 * Drop
-compatibility with django CMS < 3.6 * Move to django-app-helper 0.6.0 (2019-07-
-13) ================== * Drop compatibility with Django < 1.11 * Drop
-compatibility with Python 3 < 3.5 0.5.4 (2019-07-13) ================== * Fix
+changelog: ******* History ******* .. towncrier release notes start 1.2.0
+(2023-05-08) ================== Features -------- - Update GH actions / linting
+configuration (#79) - Add support for Django 4.2 / django CMS 3.11 1.1.0 (2022-
+08-27) ================== Bugfixes -------- - Fix error when populating the
+toolbar on page types (#67) - Fixed serialization issue when trying to upload
+the addon to Divio Cloud. (#73) - Add support for Django 3.2 / django CMS 3.10
+(#74) 1.0.0 (2020-12-21) ================== Features -------- - Add support for
+django-app-enabler (#63) - Update tooling and drop Python 2 / Django < 2.2
+compatibility (#10208) 0.8.1 (2020-05-02) ================== * Enable django
+CMS 3.7.2 on python 3 0.8.0 (2020-01-12) ================== * Relicense under
+BSD license 0.7.0 (2019-08-22) ================== * Add compatibility with
+Django 2.2 * Drop compatibility with Django < 1.11 * Drop compatibility with
+django CMS < 3.6 * Move to django-app-helper 0.6.0 (2019-07-13)
+================== * Drop compatibility with Django < 1.11 * Drop compatibility
+with Python 3 < 3.5 0.5.4 (2019-07-13) ================== * Fix error when
+page_robots is executed outside a request * Fix tox for older environments
+0.5.3 (2019-03-09) ================== * Add Django 2.0, 2.1 support * Add
+django CMS 3.6 support * Apply workaround to avoid triggering ``Page.site_id``
+deprecation warning 0.5.2 (2018-04-07) ================== * Make robots_extra
+not required 0.5.1 (2018-02-27) ================== * Fix error in migration
+dependencies 0.5.0 (2018-02-22) ================== * Add Django 1.11 support *
+Add django CMS 3.5 support * Package as Divio Cloud addon * Add support for
+noindex, noarchive robots meta tag 0.4.3 (2019-07-13) ================== * Fix
 error when page_robots is executed outside a request * Fix tox for older
-environments 0.5.3 (2019-03-09) ================== * Add Django 2.0, 2.1
-support * Add django CMS 3.6 support * Apply workaround to avoid triggering
-``Page.site_id`` deprecation warning 0.5.2 (2018-04-07) ================== *
-Make robots_extra not required 0.5.1 (2018-02-27) ================== * Fix
-error in migration dependencies 0.5.0 (2018-02-22) ================== * Add
-Django 1.11 support * Add django CMS 3.5 support * Package as Divio Cloud addon
-* Add support for noindex, noarchive robots meta tag 0.4.3 (2019-07-13)
-================== * Fix error when page_robots is executed outside a request *
-Fix tox for older environments 0.4.2 (2019-04-08) ================== * Add
-support for noindex, noarchive robots meta tag 0.4.1 (2016-12-02)
-================== * Add Django 1.10 support 0.4.0 (2016-10-26)
-================== * Drop compatibility with django CMS 3.1 and below, Django
-1.7 and below 0.3.1 (2015-10-18) ================== * Improve defaults 0.3.0
-(2015-10-18) ================== * Add Python 3.5 * Add option to exclude page
-from sitemap 0.2.0 (2015-08-15) ================== * Update to support django
-CMS 3.1 * Drop support for Django 1.4, 1.5 * Add support for Django 1.8 0.1.0
-(2014-08-26) ================== * Initial version.
+environments 0.4.2 (2019-04-08) ================== * Add support for noindex,
+noarchive robots meta tag 0.4.1 (2016-12-02) ================== * Add Django
+1.10 support 0.4.0 (2016-10-26) ================== * Drop compatibility with
+django CMS 3.1 and below, Django 1.7 and below 0.3.1 (2015-10-18)
+================== * Improve defaults 0.3.0 (2015-10-18) ================== *
+Add Python 3.5 * Add option to exclude page from sitemap 0.2.0 (2015-08-15)
+================== * Update to support django CMS 3.1 * Drop support for Django
+1.4, 1.5 * Add support for Django 1.8 0.1.0 (2014-08-26) ================== *
+Initial version.
```

### Comparing `djangocms-page-sitemap-1.1.0/djangocms_page_sitemap.egg-info/SOURCES.txt` & `djangocms-page-sitemap-1.2.0/djangocms_page_sitemap.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,11 @@
 djangocms_page_sitemap/migrations/0001_initial.py
 djangocms_page_sitemap/migrations/0002_auto_20151018_1451.py
 djangocms_page_sitemap/migrations/0003_auto_20151018_1612.py
 djangocms_page_sitemap/migrations/0004_auto_20180202_1044.py
 djangocms_page_sitemap/migrations/0005_auto_20180324_1050.py
 djangocms_page_sitemap/migrations/__init__.py
 djangocms_page_sitemap/templatetags/__init__.py
-djangocms_page_sitemap/templatetags/robots_index.py
+djangocms_page_sitemap/templatetags/robots_index.py
+tests/test_models.py
+tests/test_sitemap.py
+tests/test_toolbar.py
```

### Comparing `djangocms-page-sitemap-1.1.0/setup.cfg` & `djangocms-page-sitemap-1.2.0/setup.cfg`

 * *Files 24% similar despite different names*

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
-[bumpversion:file:djangocms_page_sitemap/__init__.py]
-
 [metadata]
 name = djangocms-page-sitemap
 version = attr: djangocms_page_sitemap.__version__
 url = https://github.com/nephila/djangocms-page-sitemap
 project_urls = 
 	Documentation = https://djangocms-page-sitemap.readthedocs.io/
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
-	Framework :: Django :: 3.0
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
+	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 install_requires = 
 	django-cms>=3.7
 setup_requires = 
 	setuptools
@@ -63,18 +42,15 @@
 
 [options.package_data]
 * = *.txt, *.rst
 djangcms_page_sitemap = *.html *.png *.gif *js *jpg *jpeg *svg *py *mo *po
 
 [options.extras_require]
 docs = 
-	django<4.0
-
-[upload]
-repository = https://upload.pypi.org/legacy/
+	django<5.0
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


# Comparing `tmp/djangocms-page-tags-1.0.0.tar.gz` & `tmp/djangocms-page-tags-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-page-tags-1.0.0.tar", last modified: Sat Aug 27 17:12:37 2022, max compression
+gzip compressed data, was "djangocms-page-tags-1.1.0.tar", last modified: Mon May  8 18:10:48 2023, max compression
```

## Comparing `djangocms-page-tags-1.0.0.tar` & `djangocms-page-tags-1.1.0.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5466 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-08-27 17:12:37.932839 djangocms-page-tags-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.924838 djangocms-page-tags-1.0.0/djangocms_page_tags/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.916838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.924838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/static/djangocms_page_tags/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/static/djangocms_page_tags/css/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/static/djangocms_page_tags/css/djangocms_page_tags_admin.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.920838 djangocms-page-tags-1.0.0/djangocms_page_tags/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/templates/djangocms_page_tags/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/templates/djangocms_page_tags/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/templates/djangocms_page_tags/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/templates/djangocms_page_tags/templatetags/page_tags.html
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/templates/djangocms_page_tags/templatetags/title_tags.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.928838 djangocms-page-tags-1.0.0/djangocms_page_tags/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/templatetags/page_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     4578 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/djangocms_page_tags/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:12:37.924838 djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-08-27 17:12:37.000000 djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-08-27 17:12:37.000000 djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:12:37.000000 djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:12:23.000000 djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-27 17:12:37.000000 djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-27 17:12:37.000000 djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-27 17:12:37.932839 djangocms-page-tags-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 17:11:54.000000 djangocms-page-tags-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.732447 djangocms-page-tags-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-08 18:10:48.732447 djangocms-page-tags-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.724447 djangocms-page-tags-1.1.0/djangocms_page_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.708447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.700447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.724447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.700447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.724447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.700447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.724447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.704447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.724447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.704447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.704447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.704447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.708447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.708447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.708447 djangocms-page-tags-1.1.0/djangocms_page_tags/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.708447 djangocms-page-tags-1.1.0/djangocms_page_tags/static/djangocms_page_tags/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/static/djangocms_page_tags/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/static/djangocms_page_tags/css/djangocms_page_tags_admin.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.712447 djangocms-page-tags-1.1.0/djangocms_page_tags/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/templates/djangocms_page_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/templates/djangocms_page_tags/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/templates/djangocms_page_tags/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/templates/djangocms_page_tags/templatetags/page_tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/templates/djangocms_page_tags/templatetags/title_tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/djangocms_page_tags/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/templatetags/page_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/djangocms_page_tags/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.724447 djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-08 18:10:48.000000 djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 18:10:48.000000 djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:10:48.000000 djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:10:31.000000 djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 18:10:48.000000 djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 18:10:48.000000 djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-08 18:10:48.732447 djangocms-page-tags-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:10:48.728447 djangocms-page-tags-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-08 18:10:03.000000 djangocms-page-tags-1.1.0/tests/test_toolbar.py
```

### Comparing `djangocms-page-tags-1.0.0/CONTRIBUTING.rst` & `djangocms-page-tags-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/HISTORY.rst` & `djangocms-page-tags-1.1.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+1.1.0 (2023-05-08)
+==================
+
+Features
+--------
+
+- Update GH actions / linting configuration (#40)
+
+
 1.0.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Add support for Django 3.2 / django CMS 3.10 (#33)
```

### Comparing `djangocms-page-tags-1.0.0/LICENSE` & `djangocms-page-tags-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/PKG-INFO` & `djangocms-page-tags-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: djangocms-page-tags
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tagged pages for django CMS 3
 Home-page: https://github.com/nephila/djangocms-page-tags
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: BSD
 Project-URL: Documentation, https://djangocms-page-tags.readthedocs.io/
 Keywords: djangocms-page-tags
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
 
 ===================
 djangocms-page-tags
@@ -121,14 +124,23 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+1.1.0 (2023-05-08)
+==================
+
+Features
+--------
+
+- Update GH actions / linting configuration (#40)
+
+
 1.0.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Add support for Django 3.2 / django CMS 3.10 (#33)
```

### Comparing `djangocms-page-tags-1.0.0/README.rst` & `djangocms-page-tags-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/admin.py` & `djangocms-page-tags-1.1.0/djangocms_page_tags/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/cms_toolbars.py` & `djangocms-page-tags-1.1.0/djangocms_page_tags/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.mo` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.mo` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/en/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.mo` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.mo` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.mo` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.mo` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.mo` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.po` & `djangocms-page-tags-1.1.0/djangocms_page_tags/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/migrations/0001_initial.py` & `djangocms-page-tags-1.1.0/djangocms_page_tags/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import taggit_autosuggest.managers
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("taggit", "0002_auto_20150616_2121"),
         ("cms", "0003_auto_20140926_2347"),
     ]
 
     operations = [
         migrations.CreateModel(
```

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/models.py` & `djangocms-page-tags-1.1.0/djangocms_page_tags/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/templates/djangocms_page_tags/base.html` & `djangocms-page-tags-1.1.0/djangocms_page_tags/templates/djangocms_page_tags/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/templatetags/page_tags.py` & `djangocms-page-tags-1.1.0/djangocms_page_tags/templatetags/page_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags/utils.py` & `djangocms-page-tags-1.1.0/djangocms_page_tags/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/PKG-INFO` & `djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: djangocms-page-tags
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tagged pages for django CMS 3
 Home-page: https://github.com/nephila/djangocms-page-tags
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: BSD
 Project-URL: Documentation, https://djangocms-page-tags.readthedocs.io/
 Keywords: djangocms-page-tags
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
 
 ===================
 djangocms-page-tags
@@ -121,14 +124,23 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+1.1.0 (2023-05-08)
+==================
+
+Features
+--------
+
+- Update GH actions / linting configuration (#40)
+
+
 1.0.0 (2022-08-27)
 ==================
 
 Bugfixes
 --------
 
 - Add support for Django 3.2 / django CMS 3.10 (#33)
```

### Comparing `djangocms-page-tags-1.0.0/djangocms_page_tags.egg-info/SOURCES.txt` & `djangocms-page-tags-1.1.0/djangocms_page_tags.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -40,8 +40,11 @@
 djangocms_page_tags/migrations/0001_initial.py
 djangocms_page_tags/migrations/__init__.py
 djangocms_page_tags/static/djangocms_page_tags/css/djangocms_page_tags_admin.css
 djangocms_page_tags/templates/djangocms_page_tags/base.html
 djangocms_page_tags/templates/djangocms_page_tags/templatetags/page_tags.html
 djangocms_page_tags/templates/djangocms_page_tags/templatetags/title_tags.html
 djangocms_page_tags/templatetags/__init__.py
-djangocms_page_tags/templatetags/page_tags.py
+djangocms_page_tags/templatetags/page_tags.py
+tests/test_general.py
+tests/test_templatetags.py
+tests/test_toolbar.py
```

### Comparing `djangocms-page-tags-1.0.0/setup.cfg` & `djangocms-page-tags-1.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-[bumpversion]
-current_version = 1.0.0
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
-[bumpversion:file:djangocms_page_tags/__init__.py]
-
 [metadata]
 name = djangocms-page-tags
 version = attr: djangocms_page_tags.__version__
 url = https://github.com/nephila/djangocms-page-tags
 project_urls = 
 	Documentation = https://djangocms-page-tags.readthedocs.io/
 author = Iacopo Spalletti
@@ -38,20 +15,23 @@
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
 	django-taggit>=0.11.2
 	django-taggit-autosuggest
@@ -65,18 +45,15 @@
 
 [options.package_data]
 * = *.txt, *.rst
 djangocms_page_tags = *.html *.png *.gif *js *jpg *jpeg *svg *py *mo *po
 
 [options.extras_require]
 docs = 
-	django<4.0
-
-[upload]
-repository = https://upload.pypi.org/legacy/
+	django<5.0
 
 [sdist]
 formats = zip
 
 [bdist_wheel]
 universal = 1
```


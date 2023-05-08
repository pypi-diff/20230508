# Comparing `tmp/django-htmx-viewsets-0.0.7.tar.gz` & `tmp/django-htmx-viewsets-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-viewsets-0.0.7.tar", last modified: Mon Apr 10 10:06:11 2023, max compression
+gzip compressed data, was "django-htmx-viewsets-0.0.8.tar", last modified: Mon May  8 06:58:24 2023, max compression
```

## Comparing `django-htmx-viewsets-0.0.7.tar` & `django-htmx-viewsets-0.0.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 10:06:03.000000 django-htmx-viewsets-0.0.7/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.770650 django-htmx-viewsets-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.778651 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.782651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 10:06:03.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.782651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.786651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.786651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/1.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/full.html
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/partial.html
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/htmx_viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 06:58:18.000000 django-htmx-viewsets-0.0.8/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 06:58:18.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/full.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/partial.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/htmx_viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/viewsets.py
```

### Comparing `django-htmx-viewsets-0.0.7/LICENSE` & `django-htmx-viewsets-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/PKG-INFO` & `django-htmx-viewsets-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.7
+Version: 0.0.8
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
+Home-page: https://github.com/snake-soft/django-htmx-viewsets
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
@@ -22,23 +23,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE
 
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml)
-[![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
+[![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/master/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
 [![Maintainability](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 django-htmx-viewsets
 ========================
-Viewsets for Django using HTMX and DataTables
+Viewsets for Django using HTMX and DataTables.
+Currently in early state.
 
 
 Built with
 ------------------------
 + [htmx](https://htmx.org/)
 + [chart.js](https://www.chartjs.org/)
 + [jQuery](https://jquery.com/)
@@ -69,25 +71,30 @@
 + Auto create mixed chart with AJAX loading
 + Auto create table with AJAX loading
 + Customizable architecture[^1]
 
 [^1]: Things may change while in early state (<1.0.0)
 
 
+Demo
+------------------------
+[Live demo](https://www.snake-soft.com/django-htmx-viewsets/)
+
+
 Screenshot
 ------------------------
 ![django-htmx-viewsets_screenshot1](https://raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/screenshot1.png)
 
 Quick-Start
 ========================
 
 Installation
 ------------------------
 ```
-pip install django-htmx-viewset
+pip install django-htmx-viewsets
 ```
 
 views.py
 ------------------------
 Create a ModelViewset by passing the model
 ```python
 MainViewSet = modelviewset_factory(model=Main)
@@ -154,19 +161,18 @@
 cd django-htmx-viewsets
 virtualenv -p python3 venv
 source venv/bin/activate
 pip install -e .[test]
 ./manage.py migrate
 ./manage.py runserver_plus
 # To create maaaany objects:
-./manage.py create_objects
+./manage.py create_objects -w
 ```
 
 The purpose of the 'create_objects'-command is to create a huge database to analyze the behavior in scenarios with a bigger amount of data.
-On a fast machine it takes about an hour to create the ~4gb database.
 To create a smaller db use the command like this:
 
 ```
 ./manage.py create_objects -c 100 -w
 # Create 100 of every object (Main, Parent, Child, Attribute and AttributeValues).
 # w is needed when using custom parameters to confirm writing to db.
 ```
```

### Comparing `django-htmx-viewsets-0.0.7/README.md` & `django-htmx-viewsets-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml)
-[![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
+[![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/master/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
 [![Maintainability](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 django-htmx-viewsets
 ========================
-Viewsets for Django using HTMX and DataTables
+Viewsets for Django using HTMX and DataTables.
+Currently in early state.
 
 
 Built with
 ------------------------
 + [htmx](https://htmx.org/)
 + [chart.js](https://www.chartjs.org/)
 + [jQuery](https://jquery.com/)
@@ -42,25 +43,30 @@
 + Auto create mixed chart with AJAX loading
 + Auto create table with AJAX loading
 + Customizable architecture[^1]
 
 [^1]: Things may change while in early state (<1.0.0)
 
 
+Demo
+------------------------
+[Live demo](https://www.snake-soft.com/django-htmx-viewsets/)
+
+
 Screenshot
 ------------------------
 ![django-htmx-viewsets_screenshot1](https://raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/screenshot1.png)
 
 Quick-Start
 ========================
 
 Installation
 ------------------------
 ```
-pip install django-htmx-viewset
+pip install django-htmx-viewsets
 ```
 
 views.py
 ------------------------
 Create a ModelViewset by passing the model
 ```python
 MainViewSet = modelviewset_factory(model=Main)
@@ -127,19 +133,18 @@
 cd django-htmx-viewsets
 virtualenv -p python3 venv
 source venv/bin/activate
 pip install -e .[test]
 ./manage.py migrate
 ./manage.py runserver_plus
 # To create maaaany objects:
-./manage.py create_objects
+./manage.py create_objects -w
 ```
 
 The purpose of the 'create_objects'-command is to create a huge database to analyze the behavior in scenarios with a bigger amount of data.
-On a fast machine it takes about an hour to create the ~4gb database.
 To create a smaller db use the command like this:
 
 ```
 ./manage.py create_objects -c 100 -w
 # Create 100 of every object (Main, Parent, Child, Attribute and AttributeValues).
 # w is needed when using custom parameters to confirm writing to db.
 ```
```

#### html2text {}

```diff
@@ -1,74 +1,75 @@
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/
 workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-
 viewsets/actions/workflows/django.yml) [![codecov](https://codecov.io/gh/snake-
-soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https:
-//codecov.io/gh/snake-soft/django-htmx-viewsets) [![Maintainability](https://
-api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://
-codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability) [![Test
-Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/
-test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/
-test_coverage) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-
-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) django-htmx-viewsets
-======================== Viewsets for Django using HTMX and DataTables Built
-with ------------------------ + [htmx](https://htmx.org/) + [chart.js](https://
-www.chartjs.org/) + [jQuery](https://jquery.com/) + [Bootstrap 5](https://
-getbootstrap.com/docs/5.0/getting-started/introduction/) + [Datatables](https:/
-/datatables.net/) + [Select2](https://select2.org/) + [Font Awesome](https://
-fontawesome.com/) Description ------------------------ When working with Django
-REST framework you will stumble upon so called ViewSets. They allow you to
-combine a set of related Views without repeating yourself. This aproach has no
-counterpart in Django itself. Therefore I created this package. It comes to its
-full power in projects where you have to create basic CRUD with listing and
-chart for many models. Eg. you can use it for building a powerful statistics
-page for online shops. Features ------------------------ + Create a viewset
-with one line + Dynamic loading of DetailView, UpdateView, CreateView and
-DeleteView + Urls are auto created + Queryset group by, filter and exclude by
-all possible date and time transform lookups + Auto create mixed chart with
-AJAX loading + Auto create table with AJAX loading + Customizable architecture
-[^1] [^1]: Things may change while in early state (<1.0.0) Screenshot ---------
---------------- ![django-htmx-viewsets_screenshot1](https://
-raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/
-screenshot1.png) Quick-Start ======================== Installation ------------
------------- ``` pip install django-htmx-viewset ``` views.py -----------------
-------- Create a ModelViewset by passing the model ```python MainViewSet =
-modelviewset_factory(model=Main) ``` or a queryset ```python MainViewSet =
-modelviewset_factory(queryset=Main.objects.all(), permissions=[]) # Remove
-permissions kwarg if you want to use django default model permissions for the
-views. ``` urls.py ------------------------ ```python urlpatterns = [ path
-('main/', include(MainViewSet.urls)), ] ``` Settings -----------------------
-- ```python MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware']
-INSTALLED_APPS += ['django_htmx', 'htmx_viewsets'] ``` Template ---------------
---------- Project contains a full template. If you want to use your own
-template, you can overwrite the template (htmx_viewsets/full.html) or pass the
-full_template_name as kwarg to modelviewset_factory. The template should
-contain the following tags and blocks: ```html {% load htmx_viewsets %}
+soft/django-htmx-viewsets/branch/master/graph/badge.svg?token=Tyfji4Pe6Q)]
+(https://codecov.io/gh/snake-soft/django-htmx-viewsets) [![Maintainability]
+(https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)]
+(https://codeclimate.com/github/snake-soft/django-htmx-viewsets/
+maintainability) [![Test Coverage](https://api.codeclimate.com/v1/badges/
+bf8a8ff519a38147e922/test_coverage)](https://codeclimate.com/github/snake-soft/
+django-htmx-viewsets/test_coverage) [![License: GPL v3](https://img.shields.io/
+badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) django-
+htmx-viewsets ======================== Viewsets for Django using HTMX and
+DataTables. Currently in early state. Built with ------------------------ +
+[htmx](https://htmx.org/) + [chart.js](https://www.chartjs.org/) + [jQuery]
+(https://jquery.com/) + [Bootstrap 5](https://getbootstrap.com/docs/5.0/
+getting-started/introduction/) + [Datatables](https://datatables.net/) +
+[Select2](https://select2.org/) + [Font Awesome](https://fontawesome.com/
+) Description ------------------------ When working with Django REST framework
+you will stumble upon so called ViewSets. They allow you to combine a set of
+related Views without repeating yourself. This aproach has no counterpart in
+Django itself. Therefore I created this package. It comes to its full power in
+projects where you have to create basic CRUD with listing and chart for many
+models. Eg. you can use it for building a powerful statistics page for online
+shops. Features ------------------------ + Create a viewset with one line +
+Dynamic loading of DetailView, UpdateView, CreateView and DeleteView + Urls are
+auto created + Queryset group by, filter and exclude by all possible date and
+time transform lookups + Auto create mixed chart with AJAX loading + Auto
+create table with AJAX loading + Customizable architecture[^1] [^1]: Things may
+change while in early state (<1.0.0) Demo ------------------------ [Live demo]
+(https://www.snake-soft.com/django-htmx-viewsets/) Screenshot -----------------
+------- ![django-htmx-viewsets_screenshot1](https://raw.githubusercontent.com/
+snake-soft/django-htmx-viewsets/master/docs/screenshot1.png) Quick-Start
+======================== Installation ------------------------ ``` pip install
+django-htmx-viewsets ``` views.py ------------------------ Create a
+ModelViewset by passing the model ```python MainViewSet = modelviewset_factory
+(model=Main) ``` or a queryset ```python MainViewSet = modelviewset_factory
+(queryset=Main.objects.all(), permissions=[]) # Remove permissions kwarg if you
+want to use django default model permissions for the views. ``` urls.py -------
+----------------- ```python urlpatterns = [ path('main/', include
+(MainViewSet.urls)), ] ``` Settings ------------------------ ```python
+MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware'] INSTALLED_APPS +=
+['django_htmx', 'htmx_viewsets'] ``` Template ------------------------ Project
+contains a full template. If you want to use your own template, you can
+overwrite the template (htmx_viewsets/full.html) or pass the full_template_name
+as kwarg to modelviewset_factory. The template should contain the following
+tags and blocks: ```html {% load htmx_viewsets %}
 {% htmx_viewsets_static_all %}
 {% block main %}{% endblock main %} {% htmx_viewsets_fixed_content %}
 ``` htmx_viewsets_static_all can be splitted by using htmx_viewsets_static_js
 and htmx_viewsets_static_css. htmx_viewsets_fixed_content can be splitted by
 using htmx_viewsets_modal and htmx_viewsets_messages. Development
 ======================== Sandbox ------------------------ The sandbox has
 multiple models containing almost all oob Django fields and relations.
 Currently only BinaryField, FileField, FilePathField and ImageField are
 missing. ``` git clone git@github.com:snake-soft/django-htmx-viewsets.git cd
 django-htmx-viewsets virtualenv -p python3 venv source venv/bin/activate pip
 install -e .[test] ./manage.py migrate ./manage.py runserver_plus # To create
-maaaany objects: ./manage.py create_objects ``` The purpose of the
+maaaany objects: ./manage.py create_objects -w ``` The purpose of the
 'create_objects'-command is to create a huge database to analyze the behavior
-in scenarios with a bigger amount of data. On a fast machine it takes about an
-hour to create the ~4gb database. To create a smaller db use the command like
-this: ``` ./manage.py create_objects -c 100 -w # Create 100 of every object
-(Main, Parent, Child, Attribute and AttributeValues). # w is needed when using
-custom parameters to confirm writing to db. ``` Status -----------------------
-- This project is currently under heavy development but the main architecture
-is finished. All described interfaces (-> Quick-Start) will be kept but there
-may be changes under the hood. Versioning ------------------------ We use
-[semver](https://semver.org/). + Major: Huge steps to make incompatible changes
-that change the documented behaviour + Minor: Changes in undocumented
-functionalities + Micro: Patches to fix smaller problems without changing
-interfaces Code Style ------------------------ + [PEP-8](https://
+in scenarios with a bigger amount of data. To create a smaller db use the
+command like this: ``` ./manage.py create_objects -c 100 -w # Create 100 of
+every object (Main, Parent, Child, Attribute and AttributeValues). # w is
+needed when using custom parameters to confirm writing to db. ``` Status ------
+------------------ This project is currently under heavy development but the
+main architecture is finished. All described interfaces (-> Quick-Start) will
+be kept but there may be changes under the hood. Versioning -------------------
+----- We use [semver](https://semver.org/). + Major: Huge steps to make
+incompatible changes that change the documented behaviour + Minor: Changes in
+undocumented functionalities + Micro: Patches to fix smaller problems without
+changing interfaces Code Style ------------------------ + [PEP-8](https://
 peps.python.org/pep-0008/) + Default line length of 80 chars Contribution -----
 ------------------- Feel free to create a [pull request](https://github.com/
 snake-soft/django-htmx-viewsets/pulls). If you find any errors, please [create
 an issue here](https://github.com/snake-soft/django-htmx-viewsets/issues) with
 all neccessary details.
```

### Comparing `django-htmx-viewsets-0.0.7/setup.py` & `django-htmx-viewsets-0.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     *tests_require,
     'build==0.10.0',
 ]
 
 
 setup(
     name='django-htmx-viewsets',
+    url='https://github.com/snake-soft/django-htmx-viewsets',
     version=version,
     author="Snake-Soft",
     author_email="info@snake-soft.com",
     description="Viewsets for Django using HTMX, Chartjs and DataTables",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='GPL3',
```

### Comparing `django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/PKG-INFO` & `django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.7
+Version: 0.0.8
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
+Home-page: https://github.com/snake-soft/django-htmx-viewsets
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
@@ -22,23 +23,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE
 
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml)
-[![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
+[![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/master/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
 [![Maintainability](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 django-htmx-viewsets
 ========================
-Viewsets for Django using HTMX and DataTables
+Viewsets for Django using HTMX and DataTables.
+Currently in early state.
 
 
 Built with
 ------------------------
 + [htmx](https://htmx.org/)
 + [chart.js](https://www.chartjs.org/)
 + [jQuery](https://jquery.com/)
@@ -69,25 +71,30 @@
 + Auto create mixed chart with AJAX loading
 + Auto create table with AJAX loading
 + Customizable architecture[^1]
 
 [^1]: Things may change while in early state (<1.0.0)
 
 
+Demo
+------------------------
+[Live demo](https://www.snake-soft.com/django-htmx-viewsets/)
+
+
 Screenshot
 ------------------------
 ![django-htmx-viewsets_screenshot1](https://raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/screenshot1.png)
 
 Quick-Start
 ========================
 
 Installation
 ------------------------
 ```
-pip install django-htmx-viewset
+pip install django-htmx-viewsets
 ```
 
 views.py
 ------------------------
 Create a ModelViewset by passing the model
 ```python
 MainViewSet = modelviewset_factory(model=Main)
@@ -154,19 +161,18 @@
 cd django-htmx-viewsets
 virtualenv -p python3 venv
 source venv/bin/activate
 pip install -e .[test]
 ./manage.py migrate
 ./manage.py runserver_plus
 # To create maaaany objects:
-./manage.py create_objects
+./manage.py create_objects -w
 ```
 
 The purpose of the 'create_objects'-command is to create a huge database to analyze the behavior in scenarios with a bigger amount of data.
-On a fast machine it takes about an hour to create the ~4gb database.
 To create a smaller db use the command like this:
 
 ```
 ./manage.py create_objects -c 100 -w
 # Create 100 of every object (Main, Parent, Child, Attribute and AttributeValues).
 # w is needed when using custom parameters to confirm writing to db.
 ```
```

### Comparing `django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/SOURCES.txt` & `django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/chart.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/chart.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/color.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/color.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/fields.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/fields.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/forms.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/forms.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/action.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/action.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/cell.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/cell.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/column.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/column.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/row.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/row.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/table.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/table.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/delete.html` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/delete.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/form.html` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/form.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/list.html` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/list.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal.html` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/partial.html` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/partial.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/table.html` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/table.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/htmx_viewsets.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/htmx_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/views.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/views.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.7/src/htmx_viewsets/viewsets.py` & `django-htmx-viewsets-0.0.8/src/htmx_viewsets/viewsets.py`

 * *Files identical despite different names*


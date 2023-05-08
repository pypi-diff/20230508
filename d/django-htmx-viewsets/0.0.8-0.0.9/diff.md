# Comparing `tmp/django-htmx-viewsets-0.0.8.tar.gz` & `tmp/django-htmx-viewsets-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-viewsets-0.0.8.tar", last modified: Mon May  8 06:58:24 2023, max compression
+gzip compressed data, was "django-htmx-viewsets-0.0.9.tar", last modified: Mon May  8 09:39:45 2023, max compression
```

## Comparing `django-htmx-viewsets-0.0.8.tar` & `django-htmx-viewsets-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 06:58:18.000000 django-htmx-viewsets-0.0.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 06:58:24.000000 django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 06:58:18.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/1.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.542660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.550660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.546660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/full.html
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/partial.html
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:24.554660 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/htmx_viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-08 06:58:06.000000 django-htmx-viewsets-0.0.8/src/htmx_viewsets/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 09:39:39.000000 django-htmx-viewsets-0.0.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.821756 django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 09:39:45.000000 django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-08 09:39:45.000000 django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:39:45.000000 django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 09:39:45.000000 django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 09:39:45.000000 django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.821756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 09:39:39.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.821756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/bootstrap/5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.821756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/datatables/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.821756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/htmx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/htmx/1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/jquery/3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/select2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/select2/4.1.0-rc.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.817756 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/full.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/partial.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:45.825755 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/templatetags/htmx_viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-08 09:39:25.000000 django-htmx-viewsets-0.0.9/src/htmx_viewsets/viewsets.py
```

### Comparing `django-htmx-viewsets-0.0.8/LICENSE` & `django-htmx-viewsets-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/PKG-INFO` & `django-htmx-viewsets-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.8
+Version: 0.0.9
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
 Home-page: https://github.com/snake-soft/django-htmx-viewsets
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-htmx-viewsets-0.0.8/README.md` & `django-htmx-viewsets-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/setup.py` & `django-htmx-viewsets-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/PKG-INFO` & `django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.8
+Version: 0.0.9
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
 Home-page: https://github.com/snake-soft/django-htmx-viewsets
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-htmx-viewsets-0.0.8/src/django_htmx_viewsets.egg-info/SOURCES.txt` & `django-htmx-viewsets-0.0.9/src/django_htmx_viewsets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/chart.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/chart.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/color.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/color.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/fields.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/fields.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/forms.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/forms.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/action.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/action.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/cell.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/cell.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/column.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/column.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/row.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/row.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/table/table.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/table/table.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/delete.html` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/delete.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/form.html` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/form.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/list.html` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/list.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends './dispatch.html' %}
+{% load i18n %}
 
 {% block htmx_main %}
 <div class="row mt-3">
   <div class="col-12">
     <h2>{{ verbose_name_plural }}</h2>
   </div>
   <form method="POST" action="{{ request.path }}?{{ request.GET.urlencode }}">{% csrf_token %}
@@ -76,14 +77,17 @@
     </div>
   </div>
   <div class="col-12">
     <hr>
   </div>
 {% endif %}
 <div class="row mt-3">
+  <div class="col-12 mb-3">
+    <a class="btn btn-link text-decoration-none" href="{% url create_url %}" hx-get="{% url create_url %}" hx-swap="none">&#43; {% trans 'Erstelle' %} {{ verbose_name }}</a>
+  </div>
   <div class="col-12">
     <div class="table-responsive">
       {% include table %}{{ table_id }}
     </div>
   </div>
 </div>
 <style>
```

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/modal.html` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/modal.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+{% load i18n %}
+
+
 <div id="modal-content" hx-swap="innerHTML" hx-swap-oob=true class="modal-content">
   {% block modal_content %}
     <div id="modal-header" class="modal-header">
       {% block modal_header %}
         <h5 class="modal-title" class="modal-title">
           {% block modal_title %}{{ modal_title }}{% endblock modal_title %}
         </h5>
@@ -19,15 +22,15 @@
       {% block modal_body %}{{ modal_body }}{% endblock modal_body %}
       {% block modal_body_post %}{{ modal_body_post }}{% endblock modal_body_post %}
     </div>
     <div id="modal-footer" class="modal-footer">
       {% block modal_footer %}
         {{ modal_footer }}
         {% block modal_submit_button %}{% endblock modal_submit_button %}
-        <button type="button" class="btn btn-secondary modal-close-button" data-dismiss="modal">Schließen</button>
+        <button type="button" class="btn btn-secondary modal-close-button" data-dismiss="modal">{% trans 'Schließen' %}</button>
       {% endblock modal_footer %}
     </div>
   {% endblock modal_content %}
   {% block modal_scripts_wrapper %}
     <script>
     	$(function(){
   			$('#modal').modal('show');
```

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/partial.html` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/partial.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templates/htmx_viewsets/table.html` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templates/htmx_viewsets/table.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/templatetags/htmx_viewsets.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/templatetags/htmx_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/views.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/views.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.8/src/htmx_viewsets/viewsets.py` & `django-htmx-viewsets-0.0.9/src/htmx_viewsets/viewsets.py`

 * *Files identical despite different names*


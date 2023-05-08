# Comparing `tmp/djangorestframework-verbose-errors-0.0.3.tar.gz` & `tmp/djangorestframework-verbose-errors-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangorestframework-verbose-errors-0.0.3.tar", last modified: Mon May  8 14:54:37 2023, max compression
+gzip compressed data, was "dist/djangorestframework-verbose-errors-0.0.4.tar", last modified: Mon May  8 18:42:28 2023, max compression
```

## Comparing `djangorestframework-verbose-errors-0.0.3.tar` & `djangorestframework-verbose-errors-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      821 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/PKG-INFO
-drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/djangorestframework_verbose_errors.egg-info/
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      821 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/djangorestframework_verbose_errors.egg-info/PKG-INFO
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      331 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/djangorestframework_verbose_errors.egg-info/SOURCES.txt
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)       30 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/djangorestframework_verbose_errors.egg-info/top_level.txt
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)        1 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/djangorestframework_verbose_errors.egg-info/dependency_links.txt
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      317 2023-05-08 14:50:07.000000 djangorestframework-verbose-errors-0.0.3/README.md
-drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/rest_framework_verbose_errors/
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)       80 2023-05-08 14:51:05.000000 djangorestframework-verbose-errors-0.0.3/rest_framework_verbose_errors/__init__.py
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      801 2023-05-07 13:20:45.000000 djangorestframework-verbose-errors-0.0.3/rest_framework_verbose_errors/views.py
--rwxr-xr-x   0 mikhaileremeev   (501) staff       (20)      619 2023-05-08 14:51:59.000000 djangorestframework-verbose-errors-0.0.3/setup.py
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)       38 2023-05-08 14:54:37.000000 djangorestframework-verbose-errors-0.0.3/setup.cfg
+drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)     1751 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/PKG-INFO
+drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/djangorestframework_verbose_errors.egg-info/
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)     1751 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/djangorestframework_verbose_errors.egg-info/PKG-INFO
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      331 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/djangorestframework_verbose_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)       30 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/djangorestframework_verbose_errors.egg-info/top_level.txt
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)        1 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/djangorestframework_verbose_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      935 2023-05-08 18:41:05.000000 djangorestframework-verbose-errors-0.0.4/README.md
+drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/rest_framework_verbose_errors/
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)       80 2023-05-08 18:41:38.000000 djangorestframework-verbose-errors-0.0.4/rest_framework_verbose_errors/__init__.py
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      801 2023-05-07 13:20:45.000000 djangorestframework-verbose-errors-0.0.4/rest_framework_verbose_errors/views.py
+-rwxr-xr-x   0 mikhaileremeev   (501) staff       (20)      619 2023-05-08 14:51:59.000000 djangorestframework-verbose-errors-0.0.4/setup.py
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)       38 2023-05-08 18:42:28.000000 djangorestframework-verbose-errors-0.0.4/setup.cfg
```

### Comparing `djangorestframework-verbose-errors-0.0.3/rest_framework_verbose_errors/views.py` & `djangorestframework-verbose-errors-0.0.4/rest_framework_verbose_errors/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-verbose-errors-0.0.3/setup.py` & `djangorestframework-verbose-errors-0.0.4/setup.py`

 * *Files identical despite different names*


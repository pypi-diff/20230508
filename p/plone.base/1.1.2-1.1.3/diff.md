# Comparing `tmp/plone.base-1.1.2.tar.gz` & `tmp/plone.base-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.base-1.1.2.tar", last modified: Wed Apr 19 07:21:34 2023, max compression
+gzip compressed data, was "plone.base-1.1.3.tar", last modified: Mon May  8 19:42:14 2023, max compression
```

## Comparing `plone.base-1.1.2.tar` & `plone.base-1.1.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.009000 plone.base-1.1.2/
--rw-r--r--   0 gil       (1000) gil       (1000)     4115 2023-04-19 07:21:33.000000 plone.base-1.1.2/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      105 2023-04-19 07:21:33.000000 plone.base-1.1.2/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)     7097 2023-04-19 07:21:34.009000 plone.base-1.1.2/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     2025 2023-04-19 07:21:33.000000 plone.base-1.1.2/README.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     2834 2023-04-19 07:21:33.000000 plone.base-1.1.2/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)     1623 2023-04-19 07:21:34.009000 plone.base-1.1.2/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)       39 2023-04-19 07:21:33.000000 plone.base-1.1.2/setup.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.003000 plone.base-1.1.2/src/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.004000 plone.base-1.1.2/src/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.006000 plone.base-1.1.2/src/plone/base/
--rw-r--r--   0 gil       (1000) gil       (1000)      238 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2894 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/batch.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5502 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/defaultpage.py
--rw-r--r--   0 gil       (1000) gil       (1000)    12074 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/i18nl10n.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.008000 plone.base-1.1.2/src/plone/base/interfaces/
--rw-r--r--   0 gil       (1000) gil       (1000)     2622 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      305 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/atd.py
--rw-r--r--   0 gil       (1000) gil       (1000)      289 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/basetool.py
--rw-r--r--   0 gil       (1000) gil       (1000)      151 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/breadcrumbs.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3060 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/constrains.py
--rw-r--r--   0 gil       (1000) gil       (1000)    63997 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/controlpanel.py
--rw-r--r--   0 gil       (1000) gil       (1000)      403 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/defaultpage.py
--rw-r--r--   0 gil       (1000) gil       (1000)      652 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/events.py
--rw-r--r--   0 gil       (1000) gil       (1000)      776 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/images.py
--rw-r--r--   0 gil       (1000) gil       (1000)      529 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/installable.py
--rw-r--r--   0 gil       (1000) gil       (1000)      697 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/interface.py
--rw-r--r--   0 gil       (1000) gil       (1000)      229 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/language.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1993 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/login.py
--rw-r--r--   0 gil       (1000) gil       (1000)      853 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/migration.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1471 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/password_reset.py
--rw-r--r--   0 gil       (1000) gil       (1000)      243 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/patterns.py
--rw-r--r--   0 gil       (1000) gil       (1000)      496 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/properties.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4824 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/resources.py
--rw-r--r--   0 gil       (1000) gil       (1000)      585 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/siteroot.py
--rw-r--r--   0 gil       (1000) gil       (1000)      453 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/structure.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6328 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/syndication.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1499 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/translationservice.py
--rw-r--r--   0 gil       (1000) gil       (1000)      159 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/workflow.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2196 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/navigationroot.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2267 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/permissions.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.009000 plone.base-1.1.2/src/plone/base/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3507 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/messages.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1387 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_batch.py
--rw-r--r--   0 gil       (1000) gil       (1000)      226 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_doctests.py
--rw-r--r--   0 gil       (1000) gil       (1000)    17956 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_i18nl10n.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6869 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_utils.py
--rw-r--r--   0 gil       (1000) gil       (1000)    20346 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/utils.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.005000 plone.base-1.1.2/src/plone.base.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)     7097 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     1673 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      152 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:14.500874 plone.base-1.1.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     4269 2023-05-08 19:42:13.000000 plone.base-1.1.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      105 2023-05-08 19:42:13.000000 plone.base-1.1.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     7251 2023-05-08 19:42:14.501077 plone.base-1.1.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2025 2023-05-08 19:42:13.000000 plone.base-1.1.3/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2834 2023-05-08 19:42:13.000000 plone.base-1.1.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1623 2023-05-08 19:42:14.502071 plone.base-1.1.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       39 2023-05-08 19:42:13.000000 plone.base-1.1.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:14.478049 plone.base-1.1.3/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:14.481610 plone.base-1.1.3/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:14.487615 plone.base-1.1.3/src/plone/base/
+-rw-r--r--   0 maurits    (501) staff       (20)      238 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2894 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/batch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5502 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12074 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/i18nl10n.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:14.497645 plone.base-1.1.3/src/plone/base/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)     2622 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      305 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/atd.py
+-rw-r--r--   0 maurits    (501) staff       (20)      289 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/basetool.py
+-rw-r--r--   0 maurits    (501) staff       (20)      151 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/breadcrumbs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3060 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)    63997 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      403 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      652 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/images.py
+-rw-r--r--   0 maurits    (501) staff       (20)      529 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/installable.py
+-rw-r--r--   0 maurits    (501) staff       (20)      697 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1993 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/login.py
+-rw-r--r--   0 maurits    (501) staff       (20)      853 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/migration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1471 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/password_reset.py
+-rw-r--r--   0 maurits    (501) staff       (20)      243 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)      496 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/properties.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4824 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/resources.py
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/siteroot.py
+-rw-r--r--   0 maurits    (501) staff       (20)      453 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/structure.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6328 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/syndication.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1499 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/translationservice.py
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/interfaces/workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2196 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/navigationroot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2267 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:14.500518 plone.base-1.1.3/src/plone/base/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3507 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/tests/messages.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1387 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/tests/test_batch.py
+-rw-r--r--   0 maurits    (501) staff       (20)      226 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17956 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/tests/test_i18nl10n.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2286 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/tests/test_root.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6869 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20346 2023-05-08 19:42:13.000000 plone.base-1.1.3/src/plone/base/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:42:14.484579 plone.base-1.1.3/src/plone.base.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     7251 2023-05-08 19:42:14.000000 plone.base-1.1.3/src/plone.base.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1707 2023-05-08 19:42:14.000000 plone.base-1.1.3/src/plone.base.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:42:14.000000 plone.base-1.1.3/src/plone.base.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:42:14.000000 plone.base-1.1.3/src/plone.base.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:42:14.000000 plone.base-1.1.3/src/plone.base.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2023-05-08 19:42:14.000000 plone.base-1.1.3/src/plone.base.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:42:14.000000 plone.base-1.1.3/src/plone.base.egg-info/top_level.txt
```

### Comparing `plone.base-1.1.2/CHANGES.rst` & `plone.base-1.1.3/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.3 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Move test for navigationroot from plone.app.layout und refactor.
+  [@jensens] (move-navroot-test)
+
+
 1.1.2 (2023-04-19)
 ------------------
 
 Bug fixes:
 
 
 - Check for container field / attribute when trying to create content with same id [laulaz] (#35)
```

### Comparing `plone.base-1.1.2/PKG-INFO` & `plone.base-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.1.2
+Version: 1.1.3
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -80,14 +80,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.3 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Move test for navigationroot from plone.app.layout und refactor.
+  [@jensens] (move-navroot-test)
+
+
 1.1.2 (2023-04-19)
 ------------------
 
 Bug fixes:
 
 
 - Check for container field / attribute when trying to create content with same id [laulaz] (#35)
```

### Comparing `plone.base-1.1.2/README.rst` & `plone.base-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/pyproject.toml` & `plone.base-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/setup.cfg` & `plone.base-1.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.1.2
+version = 1.1.3
 name = plone.base
 description = Plone Interface contracts, plus basic features and utilities
 long_description = file: README.rst, CHANGES.rst
 keywords = plone
 author = Jens W. Klein
 author_email = jk@kleinundpartner.at
 maintainer = Plone Release Team
```

### Comparing `plone.base-1.1.2/src/plone/base/batch.py` & `plone.base-1.1.3/src/plone/base/batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/defaultpage.py` & `plone.base-1.1.3/src/plone/base/defaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/i18nl10n.py` & `plone.base-1.1.3/src/plone/base/i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/__init__.py` & `plone.base-1.1.3/src/plone/base/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/constrains.py` & `plone.base-1.1.3/src/plone/base/interfaces/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/controlpanel.py` & `plone.base-1.1.3/src/plone/base/interfaces/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/events.py` & `plone.base-1.1.3/src/plone/base/interfaces/events.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/images.py` & `plone.base-1.1.3/src/plone/base/interfaces/images.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/installable.py` & `plone.base-1.1.3/src/plone/base/interfaces/installable.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/interface.py` & `plone.base-1.1.3/src/plone/base/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/login.py` & `plone.base-1.1.3/src/plone/base/interfaces/login.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/migration.py` & `plone.base-1.1.3/src/plone/base/interfaces/migration.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/password_reset.py` & `plone.base-1.1.3/src/plone/base/interfaces/password_reset.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/resources.py` & `plone.base-1.1.3/src/plone/base/interfaces/resources.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/siteroot.py` & `plone.base-1.1.3/src/plone/base/interfaces/siteroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/syndication.py` & `plone.base-1.1.3/src/plone/base/interfaces/syndication.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/interfaces/translationservice.py` & `plone.base-1.1.3/src/plone/base/interfaces/translationservice.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/navigationroot.py` & `plone.base-1.1.3/src/plone/base/navigationroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/permissions.py` & `plone.base-1.1.3/src/plone/base/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/tests/messages.rst` & `plone.base-1.1.3/src/plone/base/tests/messages.rst`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/tests/test_batch.py` & `plone.base-1.1.3/src/plone/base/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/tests/test_i18nl10n.py` & `plone.base-1.1.3/src/plone/base/tests/test_i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/tests/test_utils.py` & `plone.base-1.1.3/src/plone/base/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone/base/utils.py` & `plone.base-1.1.3/src/plone/base/utils.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.2/src/plone.base.egg-info/PKG-INFO` & `plone.base-1.1.3/src/plone.base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.1.2
+Version: 1.1.3
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -80,14 +80,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.3 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Move test for navigationroot from plone.app.layout und refactor.
+  [@jensens] (move-navroot-test)
+
+
 1.1.2 (2023-04-19)
 ------------------
 
 Bug fixes:
 
 
 - Check for container field / attribute when trying to create content with same id [laulaz] (#35)
```

### Comparing `plone.base-1.1.2/src/plone.base.egg-info/SOURCES.txt` & `plone.base-1.1.3/src/plone.base.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 src/plone/base/interfaces/translationservice.py
 src/plone/base/interfaces/workflow.py
 src/plone/base/tests/__init__.py
 src/plone/base/tests/messages.rst
 src/plone/base/tests/test_batch.py
 src/plone/base/tests/test_doctests.py
 src/plone/base/tests/test_i18nl10n.py
+src/plone/base/tests/test_root.py
 src/plone/base/tests/test_utils.py
```


# Comparing `tmp/plone.versioncheck-1.8.0.tar.gz` & `tmp/plone.versioncheck-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.versioncheck-1.8.0.tar", last modified: Sat Apr 15 08:35:47 2023, max compression
+gzip compressed data, was "plone.versioncheck-1.8.1.tar", last modified: Mon May  8 19:49:41 2023, max compression
```

## Comparing `plone.versioncheck-1.8.0.tar` & `plone.versioncheck-1.8.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/
--rw-r--r--   0 gil       (1000) gil       (1000)      144 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/.coveragerc
--rw-r--r--   0 gil       (1000) gil       (1000)     5069 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      138 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)    17507 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)    11084 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/README.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       52 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/bar.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)       84 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/baz.cfg
--rwxr-xr-x   0 gil       (1000) gil       (1000)      231 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/bootstrap.sh
--rw-r--r--   0 gil       (1000) gil       (1000)      979 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/buildout.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)      105 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/foo.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)      615 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     2330 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/setup.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.486667 plone.versioncheck-1.8.0/src/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.488667 plone.versioncheck-1.8.0/src/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       80 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.489667 plone.versioncheck-1.8.0/src/plone/versioncheck/
--rw-r--r--   0 gil       (1000) gil       (1000)       24 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1565 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/analyser.py
--rw-r--r--   0 gil       (1000) gil       (1000)     9526 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/formatter.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5980 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/parser.py
--rw-r--r--   0 gil       (1000) gil       (1000)    10048 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/pypi.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4590 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/script.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.489667 plone.versioncheck-1.8.0/src/plone/versioncheck/tpl/
--rw-r--r--   0 gil       (1000) gil       (1000)     3059 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/tpl/browser.jinja
--rw-r--r--   0 gil       (1000) gil       (1000)     3319 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/tracking.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4949 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/utils.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.488667 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)    17507 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      986 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      134 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/entry_points.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      164 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/zip-safe
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)     3777 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_analyser.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6164 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_formatter.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1695 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_parser.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4859 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_script.py
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_utils.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2357 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_version_compare.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1797 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.472212 plone.versioncheck-1.8.1/
+-rw-r--r--   0 maurits    (501) staff       (20)      144 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/.coveragerc
+-rw-r--r--   0 maurits    (501) staff       (20)      237 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)     5272 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    17710 2023-05-08 19:49:41.472415 plone.versioncheck-1.8.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    11084 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       52 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/bar.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       84 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/baz.cfg
+-rwxr-xr-x   0 maurits    (501) staff       (20)      231 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/bootstrap.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      979 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.461777 plone.versioncheck-1.8.1/buildout.d/
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/buildout.d/spam.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      105 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/foo.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      615 2023-05-08 19:49:41.473428 plone.versioncheck-1.8.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2330 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.454952 plone.versioncheck-1.8.1/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.462183 plone.versioncheck-1.8.1/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.469080 plone.versioncheck-1.8.1/src/plone/versioncheck/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1565 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/analyser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9526 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/formatter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5980 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/parser.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10312 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/pypi.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4590 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/script.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.469503 plone.versioncheck-1.8.1/src/plone/versioncheck/tpl/
+-rw-r--r--   0 maurits    (501) staff       (20)     3059 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/tpl/browser.jinja
+-rw-r--r--   0 maurits    (501) staff       (20)     3319 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/tracking.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4949 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/src/plone/versioncheck/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.465763 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    17710 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      134 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      164 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:49:41.000000 plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/zip-safe
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:41.471870 plone.versioncheck-1.8.1/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)     3777 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/tests/test_analyser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6164 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/tests/test_formatter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1695 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/tests/test_parser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4859 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/tests/test_script.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2357 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/tests/test_version_compare.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1797 2023-05-08 19:49:40.000000 plone.versioncheck-1.8.1/tox.ini
```

### Comparing `plone.versioncheck-1.8.0/CHANGES.rst` & `plone.versioncheck-1.8.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+1.8.1 (2023-05-08)
+------------------
+
+Bug fixes:
+
+- Catch empty version and ignore invalid versions in more places.
+  Needed when a package is explicitly unpinned, for example ``Zope =``.
+  [maurits]
+
+
 1.8.0 (2023-04-15)
 ------------------
 
 - Ignore invalid versions.
   Needed for ``setuptools`` 66 and higher when checking a package that has invalid versions on PyPI.
   Fixes `issue 52 <https://github.com/plone/plone.versioncheck/issues/52>`_.
   [maurits]
```

### Comparing `plone.versioncheck-1.8.0/PKG-INFO` & `plone.versioncheck-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.versioncheck
-Version: 1.8.0
+Version: 1.8.1
 Summary: Checks pinned versions with overrides in a cascaded buildout
 Home-page: https://github.com/plone/plone.versioncheck
 Author: Jens W. Klein
 Author-email: jens@bluedynamics.com
 License: GPL version 2
 Keywords: plone buildout version
 Classifier: Development Status :: 5 - Production/Stable
@@ -361,14 +361,24 @@
 
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
+1.8.1 (2023-05-08)
+------------------
+
+Bug fixes:
+
+- Catch empty version and ignore invalid versions in more places.
+  Needed when a package is explicitly unpinned, for example ``Zope =``.
+  [maurits]
+
+
 1.8.0 (2023-04-15)
 ------------------
 
 - Ignore invalid versions.
   Needed for ``setuptools`` 66 and higher when checking a package that has invalid versions on PyPI.
   Fixes `issue 52 <https://github.com/plone/plone.versioncheck/issues/52>`_.
   [maurits]
```

### Comparing `plone.versioncheck-1.8.0/README.rst` & `plone.versioncheck-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/buildout.cfg` & `plone.versioncheck-1.8.1/buildout.cfg`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/setup.cfg` & `plone.versioncheck-1.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/setup.py` & `plone.versioncheck-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "1.8.0"
+version = "1.8.1"
 
 long_description = "{0}\n\n{1}".format(
     open("README.rst").read(), open("CHANGES.rst").read()
 )
 
 setup(
     name="plone.versioncheck",
```

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/analyser.py` & `plone.versioncheck-1.8.1/src/plone/versioncheck/analyser.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/formatter.py` & `plone.versioncheck-1.8.1/src/plone/versioncheck/formatter.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/parser.py` & `plone.versioncheck-1.8.1/src/plone/versioncheck/parser.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/pypi.py` & `plone.versioncheck-1.8.1/src/plone/versioncheck/pypi.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,24 @@
             ("bugfix", FLOOR_RELEASE),
             ("majorpre", FLOOR_RELEASE),
             ("minorpre", FLOOR_RELEASE),
             ("bugfixpre", FLOOR_RELEASE),
         ]
     )
 
+    if not version:
+        return False, "Empty version."
+
     # parse version to test against:
     try:
         version = parse_version(version)
-    except TypeError:
+    except Exception:
+        # likely pkg_resources.extern.packaging.version.InvalidVersion
+        # or TypeError, but really any exception can be ignored.
+        # See https://github.com/plone/plone.versioncheck/issues/52
         return False, "Version broken/ not checkable."
     try:
         vtuple = mmbp_tuple(version)
     except ValueError:
         return False, "Can not check legacy version number."
 
     # fetch pkgs json info from pypi
```

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/script.py` & `plone.versioncheck-1.8.1/src/plone/versioncheck/script.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/tpl/browser.jinja` & `plone.versioncheck-1.8.1/src/plone/versioncheck/tpl/browser.jinja`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/tracking.py` & `plone.versioncheck-1.8.1/src/plone/versioncheck/tracking.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/src/plone/versioncheck/utils.py` & `plone.versioncheck-1.8.1/src/plone/versioncheck/utils.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/PKG-INFO` & `plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.versioncheck
-Version: 1.8.0
+Version: 1.8.1
 Summary: Checks pinned versions with overrides in a cascaded buildout
 Home-page: https://github.com/plone/plone.versioncheck
 Author: Jens W. Klein
 Author-email: jens@bluedynamics.com
 License: GPL version 2
 Keywords: plone buildout version
 Classifier: Development Status :: 5 - Production/Stable
@@ -361,14 +361,24 @@
 
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
+1.8.1 (2023-05-08)
+------------------
+
+Bug fixes:
+
+- Catch empty version and ignore invalid versions in more places.
+  Needed when a package is explicitly unpinned, for example ``Zope =``.
+  [maurits]
+
+
 1.8.0 (2023-04-15)
 ------------------
 
 - Ignore invalid versions.
   Needed for ``setuptools`` 66 and higher when checking a package that has invalid versions on PyPI.
   Fixes `issue 52 <https://github.com/plone/plone.versioncheck/issues/52>`_.
   [maurits]
```

### Comparing `plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/SOURCES.txt` & `plone.versioncheck-1.8.1/src/plone.versioncheck.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 .coveragerc
+.editorconfig
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 bar.cfg
 baz.cfg
 bootstrap.sh
 buildout.cfg
 foo.cfg
 setup.cfg
 setup.py
 tox.ini
+buildout.d/spam.cfg
 src/plone/__init__.py
 src/plone.versioncheck.egg-info/PKG-INFO
 src/plone.versioncheck.egg-info/SOURCES.txt
 src/plone.versioncheck.egg-info/dependency_links.txt
 src/plone.versioncheck.egg-info/entry_points.txt
 src/plone.versioncheck.egg-info/namespace_packages.txt
 src/plone.versioncheck.egg-info/requires.txt
```

### Comparing `plone.versioncheck-1.8.0/tests/test_analyser.py` & `plone.versioncheck-1.8.1/tests/test_analyser.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/tests/test_formatter.py` & `plone.versioncheck-1.8.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/tests/test_parser.py` & `plone.versioncheck-1.8.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/tests/test_script.py` & `plone.versioncheck-1.8.1/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/tests/test_version_compare.py` & `plone.versioncheck-1.8.1/tests/test_version_compare.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.8.0/tox.ini` & `plone.versioncheck-1.8.1/tox.ini`

 * *Files identical despite different names*


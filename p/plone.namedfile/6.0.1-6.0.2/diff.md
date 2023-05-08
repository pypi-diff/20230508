# Comparing `tmp/plone.namedfile-6.0.1.tar.gz` & `tmp/plone.namedfile-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.namedfile-6.0.1.tar", last modified: Tue Mar 14 22:28:02 2023, max compression
+gzip compressed data, was "plone.namedfile-6.0.2.tar", last modified: Mon May  8 19:44:43 2023, max compression
```

## Comparing `plone.namedfile-6.0.1.tar` & `plone.namedfile-6.0.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:28:02.983278 plone.namedfile-6.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    20194 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    36386 2023-03-14 22:28:02.983412 plone.namedfile-6.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      777 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:28:02.963017 plone.namedfile-6.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1217 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1481 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      457 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/docs/ZPL.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:28:02.963249 plone.namedfile-6.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:28:02.975362 plone.namedfile-6.0.1/plone/namedfile/
--rw-r--r--   0 maurits    (501) staff       (20)      214 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5087 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)     7145 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     1233 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      959 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     2388 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/editor.py
--rw-r--r--   0 maurits    (501) staff       (20)      522 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/editor.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3754 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/field.py
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/field.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    12410 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/file.py
--rw-r--r--   0 maurits    (501) staff       (20)      519 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     6201 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/handler.rst
--rw-r--r--   0 maurits    (501) staff       (20)      609 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/handler.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3040 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/marshaler.py
--rw-r--r--   0 maurits    (501) staff       (20)     8283 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/marshaler.rst
--rw-r--r--   0 maurits    (501) staff       (20)      313 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/marshaler.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5748 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/picture.py
--rw-r--r--   0 maurits    (501) staff       (20)    28292 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/scaling.py
--rw-r--r--   0 maurits    (501) staff       (20)     1853 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/scaling.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2870 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/storages.py
--rw-r--r--   0 maurits    (501) staff       (20)     6976 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/test.pt
--rw-r--r--   0 maurits    (501) staff       (20)      881 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      636 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:28:02.981949 plone.namedfile-6.0.1/plone/namedfile/tests/
--rw-r--r--   0 maurits    (501) staff       (20)   160651 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/900.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      234 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1279 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/dummy.py
--rw-r--r--   0 maurits    (501) staff       (20)     8351 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)      303 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/image.gif
--rw-r--r--   0 maurits    (501) staff       (20)     3641 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      290 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/image.png
--rw-r--r--   0 maurits    (501) staff       (20)     3823 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/image.svg
--rw-r--r--   0 maurits    (501) staff       (20)   300316 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/image.tif
--rw-r--r--   0 maurits    (501) staff       (20)    13824 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/notimage.doc
--rw-r--r--   0 maurits    (501) staff       (20)     5205 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)     4054 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_blobfile.py
--rw-r--r--   0 maurits    (501) staff       (20)     5736 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_display_file.py
--rw-r--r--   0 maurits    (501) staff       (20)      617 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     4381 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_image.py
--rw-r--r--   0 maurits    (501) staff       (20)    37468 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_scaling.py
--rw-r--r--   0 maurits    (501) staff       (20)     8577 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_scaling_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     2039 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_storable.py
--rw-r--r--   0 maurits    (501) staff       (20)     1427 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/test_svg.py
--rw-r--r--   0 maurits    (501) staff       (20)      168 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/tests/tool.gif
--rw-r--r--   0 maurits    (501) staff       (20)    14414 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/usage.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:28:02.983077 plone.namedfile-6.0.1/plone/namedfile/utils/
--rw-r--r--   0 maurits    (501) staff       (20)    11763 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/utils/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1092 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/utils/jpeg_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      866 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/utils/png_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1159 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/utils/svg_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      417 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/utils.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1381 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone/namedfile/z3c-blobfile.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:28:02.965575 plone.namedfile-6.0.1/plone.namedfile.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    36386 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone.namedfile.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2027 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone.namedfile.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone.namedfile.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone.namedfile.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone.namedfile.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      283 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone.namedfile.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/plone.namedfile.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      658 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-03-14 22:28:02.983909 plone.namedfile-6.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2073 2023-03-14 22:28:02.000000 plone.namedfile-6.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:44:43.679590 plone.namedfile-6.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    20333 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    36525 2023-05-08 19:44:43.679807 plone.namedfile-6.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      777 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:44:43.653917 plone.namedfile-6.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1217 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1481 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      457 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/docs/ZPL.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:44:43.654312 plone.namedfile-6.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:44:43.668390 plone.namedfile-6.0.2/plone/namedfile/
+-rw-r--r--   0 maurits    (501) staff       (20)      214 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5087 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7145 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1233 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      959 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/copy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2388 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/editor.py
+-rw-r--r--   0 maurits    (501) staff       (20)      522 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/editor.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3754 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/field.py
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/field.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    12410 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      519 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6201 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/handler.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      609 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/handler.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3040 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/marshaler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8283 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/marshaler.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      313 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/marshaler.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6218 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/picture.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28292 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/scaling.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1853 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/scaling.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2870 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/storages.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6976 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/test.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      881 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      636 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:44:43.677629 plone.namedfile-6.0.2/plone/namedfile/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)   160651 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/900.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1279 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/dummy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8351 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)      303 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/image.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     3641 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)      290 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/image.png
+-rw-r--r--   0 maurits    (501) staff       (20)     3823 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/image.svg
+-rw-r--r--   0 maurits    (501) staff       (20)   300316 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/image.tif
+-rw-r--r--   0 maurits    (501) staff       (20)    13824 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/notimage.doc
+-rw-r--r--   0 maurits    (501) staff       (20)     5205 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4054 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_blobfile.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5736 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_display_file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      617 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4381 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)    38372 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_scaling.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8577 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_scaling_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2039 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_storable.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1427 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/test_svg.py
+-rw-r--r--   0 maurits    (501) staff       (20)      168 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/tests/tool.gif
+-rw-r--r--   0 maurits    (501) staff       (20)    14414 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/usage.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:44:43.679255 plone.namedfile-6.0.2/plone/namedfile/utils/
+-rw-r--r--   0 maurits    (501) staff       (20)    11763 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/utils/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1092 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/utils/jpeg_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      866 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/utils/png_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1159 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/utils/svg_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      417 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/utils.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1381 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/plone/namedfile/z3c-blobfile.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:44:43.657274 plone.namedfile-6.0.2/plone.namedfile.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    36525 2023-05-08 19:44:43.000000 plone.namedfile-6.0.2/plone.namedfile.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2027 2023-05-08 19:44:43.000000 plone.namedfile-6.0.2/plone.namedfile.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:44:43.000000 plone.namedfile-6.0.2/plone.namedfile.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:44:43.000000 plone.namedfile-6.0.2/plone.namedfile.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:44:43.000000 plone.namedfile-6.0.2/plone.namedfile.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      283 2023-05-08 19:44:43.000000 plone.namedfile-6.0.2/plone.namedfile.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:44:43.000000 plone.namedfile-6.0.2/plone.namedfile.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      658 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2023-05-08 19:44:43.680559 plone.namedfile-6.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2073 2023-05-08 19:44:42.000000 plone.namedfile-6.0.2/setup.py
```

### Comparing `plone.namedfile-6.0.1/CHANGES.rst` & `plone.namedfile-6.0.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.0.2 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Fix picture tag when original image is used instead of a scale.
+  [maurits] (#142)
+
+
 6.0.1 (2023-03-14)
 ------------------
 
 Tests
 
 
 - Tox: explicitly test only the ``plone.namedfile`` package.  [maurits] (#50)
```

### Comparing `plone.namedfile-6.0.1/PKG-INFO` & `plone.namedfile-6.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.namedfile
-Version: 6.0.1
+Version: 6.0.2
 Summary: File types and fields for images, files and blob files with filenames
 Home-page: https://pypi.org/project/plone.namedfile
 Author: Laurence Rowe, Martin Aspeli
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: plone named file image blob
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,14 +57,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.0.2 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Fix picture tag when original image is used instead of a scale.
+  [maurits] (#142)
+
+
 6.0.1 (2023-03-14)
 ------------------
 
 Tests
 
 
 - Tox: explicitly test only the ``plone.namedfile`` package.  [maurits] (#50)
```

### Comparing `plone.namedfile-6.0.1/README.rst` & `plone.namedfile-6.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/docs/INSTALL.txt` & `plone.namedfile-6.0.2/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/docs/LICENSE.txt` & `plone.namedfile-6.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/adapters.py` & `plone.namedfile-6.0.2/plone/namedfile/adapters.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/browser.py` & `plone.namedfile-6.0.2/plone/namedfile/browser.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/configure.zcml` & `plone.namedfile-6.0.2/plone/namedfile/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/copy.py` & `plone.namedfile-6.0.2/plone/namedfile/copy.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/editor.py` & `plone.namedfile-6.0.2/plone/namedfile/editor.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/editor.zcml` & `plone.namedfile-6.0.2/plone/namedfile/editor.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/field.py` & `plone.namedfile-6.0.2/plone/namedfile/field.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/file.py` & `plone.namedfile-6.0.2/plone/namedfile/file.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/handler.py` & `plone.namedfile-6.0.2/plone/namedfile/handler.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/handler.rst` & `plone.namedfile-6.0.2/plone/namedfile/handler.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/handler.zcml` & `plone.namedfile-6.0.2/plone/namedfile/handler.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/interfaces.py` & `plone.namedfile-6.0.2/plone/namedfile/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/marshaler.py` & `plone.namedfile-6.0.2/plone/namedfile/marshaler.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/marshaler.rst` & `plone.namedfile-6.0.2/plone/namedfile/marshaler.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/picture.py` & `plone.namedfile-6.0.2/plone/namedfile/picture.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,9 +141,19 @@
     def update_src_scale(self, src, scale):
         parts = src.split("/")
         if "." in parts[-1]:
             field_name = parts[-1].split("-")[0]
             src_scale = "/".join(parts[:-1]) + f"/{field_name}/{scale}"
             src_scale
         else:
-            src_scale = "/".join(parts[:-1]) + f"/{scale}"
+            # Usually the url has '@@images/fieldname/other_scale',
+            # and then we replace the other scale.
+            # But the url may use the original image, e.g. @@images/image.
+            # Then we want to keep the fieldname and return '.../image/scale'.
+            try:
+                full = len(parts) - parts.index("@@images") == 2
+            except ValueError:
+                full = False
+            if not full:
+                parts = parts[:-1]
+            src_scale = "/".join(parts) + f"/{scale}"
         return src_scale
```

### Comparing `plone.namedfile-6.0.1/plone/namedfile/scaling.py` & `plone.namedfile-6.0.2/plone/namedfile/scaling.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/scaling.zcml` & `plone.namedfile-6.0.2/plone/namedfile/scaling.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/storages.py` & `plone.namedfile-6.0.2/plone/namedfile/storages.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/test.pt` & `plone.namedfile-6.0.2/plone/namedfile/test.pt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/testing.py` & `plone.namedfile-6.0.2/plone/namedfile/testing.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/testing.zcml` & `plone.namedfile-6.0.2/plone/namedfile/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/900.jpg` & `plone.namedfile-6.0.2/plone/namedfile/tests/900.jpg`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/dummy.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/file.pdf` & `plone.namedfile-6.0.2/plone/namedfile/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/image.jpg` & `plone.namedfile-6.0.2/plone/namedfile/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/image.svg` & `plone.namedfile-6.0.2/plone/namedfile/tests/image.svg`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/image.tif` & `plone.namedfile-6.0.2/plone/namedfile/tests/image.tif`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/notimage.doc` & `plone.namedfile-6.0.2/plone/namedfile/tests/notimage.doc`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_adapters.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_blobfile.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_blobfile.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_display_file.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_display_file.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_doctests.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_image.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_scaling.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -976,11 +976,39 @@
         )
         self.assertEqual(
             scaling.tag("image", alt="own alt", title="own title"),
             '<img src="http://fake.image/@@images/image.jpeg" alt="own alt" title="own title" height="4" width="6" />'
         )
 
 
+class Img2PictureTagTests(unittest.TestCase):
+    """Low level tests for Img2PictureTag."""
+
+    def _makeOne(self):
+        return plone.namedfile.picture.Img2PictureTag()
+
+    def test_update_src_scale(self):
+        update_src_scale = self._makeOne().update_src_scale
+        self.assertEqual(
+            update_src_scale("foo/fieldname/old", "new"),
+            "foo/fieldname/new"
+        )
+        self.assertEqual(
+            update_src_scale("@@images/fieldname/old", "mini"),
+            "@@images/fieldname/mini"
+        )
+        self.assertEqual(
+            update_src_scale("@@images/fieldname", "preview"),
+            "@@images/fieldname/preview"
+        )
+        self.assertEqual(
+            update_src_scale(
+                "photo.jpg/@@images/image-1200-4a03b0a8227d28737f5d9e3e481bdbd6.jpeg",
+                "teaser"),
+            "photo.jpg/@@images/image/teaser",
+        )
+
+
 def test_suite():
     from unittest import defaultTestLoader
 
     return defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_scaling_functional.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_scaling_functional.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_storable.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_storable.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/tests/test_svg.py` & `plone.namedfile-6.0.2/plone/namedfile/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/usage.rst` & `plone.namedfile-6.0.2/plone/namedfile/usage.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/utils/__init__.py` & `plone.namedfile-6.0.2/plone/namedfile/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/utils/jpeg_utils.py` & `plone.namedfile-6.0.2/plone/namedfile/utils/jpeg_utils.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/utils/png_utils.py` & `plone.namedfile-6.0.2/plone/namedfile/utils/png_utils.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/utils/svg_utils.py` & `plone.namedfile-6.0.2/plone/namedfile/utils/svg_utils.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone/namedfile/z3c-blobfile.zcml` & `plone.namedfile-6.0.2/plone/namedfile/z3c-blobfile.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/plone.namedfile.egg-info/PKG-INFO` & `plone.namedfile-6.0.2/plone.namedfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.namedfile
-Version: 6.0.1
+Version: 6.0.2
 Summary: File types and fields for images, files and blob files with filenames
 Home-page: https://pypi.org/project/plone.namedfile
 Author: Laurence Rowe, Martin Aspeli
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: plone named file image blob
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,14 +57,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.0.2 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Fix picture tag when original image is used instead of a scale.
+  [maurits] (#142)
+
+
 6.0.1 (2023-03-14)
 ------------------
 
 Tests
 
 
 - Tox: explicitly test only the ``plone.namedfile`` package.  [maurits] (#50)
```

### Comparing `plone.namedfile-6.0.1/plone.namedfile.egg-info/SOURCES.txt` & `plone.namedfile-6.0.2/plone.namedfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/pyproject.toml` & `plone.namedfile-6.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.0.1/setup.py` & `plone.namedfile-6.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "6.0.1"
+version = "6.0.2"
 
 description = "File types and fields for images, files and blob files with " "filenames"
 long_description = "\n\n".join(
     [
         open("README.rst").read(),
         open("CHANGES.rst").read(),
         open(os.path.join("plone", "namedfile", "usage.rst")).read(),
```


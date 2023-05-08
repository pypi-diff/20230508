# Comparing `tmp/i18ndude-5.5.0.tar.gz` & `tmp/i18ndude-6.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/i18ndude-5.5.0.tar", last modified: Mon Sep 19 09:27:04 2022, max compression
+gzip compressed data, was "i18ndude-6.0.0a1.tar", last modified: Mon May  8 20:57:57 2023, max compression
```

## Comparing `i18ndude-5.5.0.tar` & `i18ndude-6.0.0a1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/
--rw-r--r--   0 maurits    (501) staff       (20)    34394 2022-09-19 09:27:04.000000 i18ndude-5.5.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-09-19 09:27:04.000000 i18ndude-5.5.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      136 2022-09-19 09:27:04.000000 i18ndude-5.5.0/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      439 2022-09-19 09:27:04.000000 i18ndude-5.5.0/docs/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12296 2022-09-19 09:27:04.000000 i18ndude-5.5.0/docs/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)    15880 2022-09-19 09:27:04.000000 i18ndude-5.5.0/docs/ChangeLog
--rw-r--r--   0 maurits    (501) staff       (20)    10284 2022-09-19 09:27:04.000000 i18ndude-5.5.0/docs/command.rst
--rw-r--r--   0 maurits    (501) staff       (20)      825 2022-09-19 09:27:04.000000 i18ndude-5.5.0/docs/COPYRIGHT
--rw-r--r--   0 maurits    (501) staff       (20)     2235 2022-09-19 09:27:04.000000 i18ndude-5.5.0/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      269 2022-09-19 09:27:04.000000 i18ndude-5.5.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1628 2022-09-19 09:27:04.000000 i18ndude-5.5.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)    13952 2022-09-19 09:27:04.000000 i18ndude-5.5.0/CHANGES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/
--rw-r--r--   0 maurits    (501) staff       (20)    32873 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1831 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/empty-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      893 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test2_expected-en.po
--rw-r--r--   0 maurits    (501) staff       (20)     1917 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      728 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test3.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2361 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      778 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/synctest-de.po
--rw-r--r--   0 maurits    (501) staff       (20)      392 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test2.py
--rw-r--r--   0 maurits    (501) staff       (20)     1375 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test.xml
--rw-r--r--   0 maurits    (501) staff       (20)      820 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/synctest.pot
--rw-r--r--   0 maurits    (501) staff       (20)      510 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test4.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2779 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test1.pt
--rw-r--r--   0 maurits    (501) staff       (20)      916 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test2-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      522 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/chameleon.pt
--rw-r--r--   0 maurits    (501) staff       (20)      882 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/input/test5.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/output/
--rw-r--r--   0 maurits    (501) staff       (20)       38 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/testdata/output/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     5558 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    34684 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/test_catalog.py
--rwxr-xr-x   0 maurits    (501) staff       (20)     1524 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/tox-check-i18ndude-command.sh
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7921 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/test_untranslated.py
--rw-r--r--   0 maurits    (501) staff       (20)      829 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      252 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/tests/test_extract.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     6119 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/visualisation.py
--rw-r--r--   0 maurits    (501) staff       (20)     3237 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/zcmlextract.py
--rw-r--r--   0 maurits    (501) staff       (20)    10947 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/generator.py
--rw-r--r--   0 maurits    (501) staff       (20)     3805 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    11113 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     9723 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/untranslated.py
--rw-r--r--   0 maurits    (501) staff       (20)     2985 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/gsextract.py
--rwxr-xr-x   0 maurits    (501) staff       (20)    28016 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/script.py
--rw-r--r--   0 maurits    (501) staff       (20)    20834 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/extract.py
--rw-r--r--   0 maurits    (501) staff       (20)    22287 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude/pygettext.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    34394 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)     1572 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)      143 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       85 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-09-19 09:27:04.000000 i18ndude-5.5.0/src/i18ndude.egg-info/dependency_links.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.655965 i18ndude-6.0.0a1/
+-rw-r--r--   0 maurits    (501) staff       (20)    14343 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      136 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    27562 2023-05-08 20:57:57.656198 i18ndude-6.0.0a1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.637197 i18ndude-6.0.0a1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      825 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/docs/COPYRIGHT
+-rw-r--r--   0 maurits    (501) staff       (20)    15880 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/docs/ChangeLog
+-rw-r--r--   0 maurits    (501) staff       (20)    12296 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      439 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    10185 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/command.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      293 2023-05-08 20:57:57.656996 i18ndude-6.0.0a1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2122 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.631591 i18ndude-6.0.0a1/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.643047 i18ndude-6.0.0a1/src/i18ndude/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    32873 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20834 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/extract.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2985 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/gsextract.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1831 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22287 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/pygettext.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)    28016 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/script.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.632302 i18ndude-6.0.0a1/src/i18ndude/testdata/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.652132 i18ndude-6.0.0a1/src/i18ndude/testdata/input/
+-rw-r--r--   0 maurits    (501) staff       (20)      522 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/chameleon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/empty-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      778 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest-de.po
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest.pot
+-rw-r--r--   0 maurits    (501) staff       (20)     2361 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1917 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2779 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test1.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      916 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      392 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2.py
+-rw-r--r--   0 maurits    (501) staff       (20)      893 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2_expected-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test3.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test4.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      882 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test5.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.652604 i18ndude-6.0.0a1/src/i18ndude/testdata/output/
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/output/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.655631 i18ndude-6.0.0a1/src/i18ndude/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    34684 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      252 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_extract.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7921 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_untranslated.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5558 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_utils.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1524 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/tox-check-i18ndude-command.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9723 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/untranslated.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11122 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6119 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/visualisation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3237 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/zcmlextract.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.646149 i18ndude-6.0.0a1/src/i18ndude.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    27562 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1572 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `i18ndude-5.5.0/docs/LICENSE` & `i18ndude-6.0.0a1/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/docs/ChangeLog` & `i18ndude-6.0.0a1/docs/ChangeLog`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/docs/command.rst` & `i18ndude-6.0.0a1/docs/command.rst`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   Its main task is to extract translation strings (msgids) into a
   .pot file (with the 'rebuild-pot' command), and sync the .pot file
   with .po files (with the 'sync' command).
 
   Call i18ndude with one of the listed subcommands followed by
   --help to get help for that subcommand.
 
-  optional arguments:
+  options:
     -h, --help            show this help message and exit
 
   subcommands:
     {find-untranslated,rebuild-pot,merge,sync,filter,admix,list,trmerge}
 
 find-untranslated
 -----------------
@@ -53,15 +53,15 @@
       to render a template containing those ignore hints.  You need
       Chameleon 2.23 or higher, or the to be released zope.tal 4.1.2.
       
 
   positional arguments:
     files            list of ZPT filenames
 
-  optional arguments:
+  options:
     -h, --help       show this help message and exit
     -s, --silent     The report will only contain a summary of errors and
                      warnings for each file (or no output if there are no errors
                      or warnings).
     -n, --nosummary  The report will contain only the errors for each file.
 
 rebuild-pot
@@ -120,15 +120,15 @@
       add --line-numbers to be sure you keep them when you get a newer version
       of i18ndude.  If you specify both options, the last one wins.
       
 
   positional arguments:
     path
 
-  optional arguments:
+  options:
     -h, --help            show this help message and exit
     --wrap                Wrap long lines.
     --no-wrap             Do not wrap long lines. This is the default.
     --width NUMBER        Set output page width. Default is 79.
     -p filename, --pot filename
     -c domain, --create domain
     -m filename, --merge filename
@@ -150,15 +150,15 @@
       these msgids into the target-pot file. If a msgid already
       exists, I'll warn you and ignore that msgid.
 
       If you provide a --merge2 <filename> I'll first merge this one
       in addition to the first one.
       
 
-  optional arguments:
+  options:
     -h, --help            show this help message and exit
     --wrap                Wrap long lines.
     --no-wrap             Do not wrap long lines. This is the default.
     --width NUMBER        Set output page width. Default is 79.
     -p filename, --pot filename
     -m filename, --merge filename
     --merge2 filename
@@ -176,15 +176,15 @@
       msgids are not in the pot-file and add messages that the pot-file has
       but the po-file doesn't.
       
 
   positional arguments:
     pofilename
 
-  optional arguments:
+  options:
     -h, --help            show this help message and exit
     --wrap                Wrap long lines.
     --no-wrap             Do not wrap long lines. This is the default.
     --width NUMBER        Set output page width. Default is 79.
     -p potfilename, --pot potfilename
 
 filter
@@ -198,15 +198,15 @@
       messages removed that are also in file2, i.e. where msgids match.
       
 
   positional arguments:
     file1
     file2
 
-  optional arguments:
+  options:
     -h, --help      show this help message and exit
     --wrap          Wrap long lines.
     --no-wrap       Do not wrap long lines. This is the default.
     --width NUMBER  Set output page width. Default is 79.
 
 admix
 -----
@@ -221,15 +221,15 @@
       The result will be on stdout.
       
 
   positional arguments:
     file1
     file2
 
-  optional arguments:
+  options:
     -h, --help      show this help message and exit
     --wrap          Wrap long lines.
     --no-wrap       Do not wrap long lines. This is the default.
     --width NUMBER  Set output page width. Default is 79.
 
 list
 ----
@@ -248,15 +248,15 @@
 
       With the --tiered option, we split the languages in three tiers or groups,
       the first two with languages that Plone was traditionally translated in,
       in a hardcoded order, followed by other languages.
       This was the default output for years.
       
 
-  optional arguments:
+  options:
     -h, --help            show this help message and exit
     -p product [product ...], --products product [product ...]
     -t, --table           Output as html table
     --tiered              Show in traditional three-tiered order
 
 trmerge
 -------
@@ -281,15 +281,15 @@
         i18ndude trmerge file1.po file2.po > tmp_merge && mv tmp_merge file1.po
       
 
   positional arguments:
     file1
     file2
 
-  optional arguments:
+  options:
     -h, --help          show this help message and exit
     --wrap              Wrap long lines.
     --no-wrap           Do not wrap long lines. This is the default.
     --width NUMBER      Set output page width. Default is 79.
     -i, --ignore-extra  Ignore extra messages: do not add msgids that are not in
                         the original po-file. Only update translations for
                         existing msgids.
```

### Comparing `i18ndude-5.5.0/docs/COPYRIGHT` & `i18ndude-6.0.0a1/docs/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/setup.py` & `i18ndude-6.0.0a1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 
 from setuptools import setup, find_packages
 
-version = '5.5.0'
+version = '6.0.0a1'
 
 install_requires = [
     'lxml',
     'zope.i18nmessageid >= 3.3',
     'zope.interface >= 3.3',
     'zope.tal >= 4.3.0',
 ]
@@ -22,22 +22,19 @@
                       open("CHANGES.rst").read()),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Utilities',
     ],
     keywords='Plone i18n zpt',
     author='Daniel Nouri',
@@ -47,14 +44,15 @@
     url='https://github.com/collective/i18ndude',
     license='GPL',
     package_dir={'': 'src'},
     packages=find_packages('src', ),
     include_package_data=True,
     zip_safe=False,
     test_suite='i18ndude.tests',
+    python_requires=">=3.8",
     install_requires=install_requires,
     extras_require={
         'plone': ['plone.i18n'],
     },
     entry_points={
         'console_scripts': [
             'i18ndude=i18ndude.script:main',
```

### Comparing `i18ndude-5.5.0/README.rst` & `i18ndude-6.0.0a1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     :alt: GitHub Actions badge
     :target: https://github.com/collective/i18ndude/actions
 
 
 Compatibility
 -------------
 
-i18ndude works with Python 2.7, 3.6, 3.7, pypy and pypy3.
-Older versions are not supported anymore, use the i18ndude 4.x series
+i18ndude works with Python 3.8-3.11, and PyPy3.
+Older versions are not supported anymore, use the i18ndude 5.x series
 if you need that.
 
 You can install ``i18ndude`` with Buildout or ``pip``.
 With ``pip`` you may want to look at our `requirements.txt <https://github.com/collective/i18ndude/blob/master/requirements.txt>`_.
 
 ``UnicodeEncodeError``
 ----------------------
@@ -37,7 +37,19 @@
     export PYTHONIOENCODING=utf-8
 
 This fixes UnicodeEncodeErrors when piping or redirecting output that contains non-ascii.
 I (Maurits) have this line in my bash profile now.
 
 Note: if you get a ``UnicodeDecodeError``, so 'decode' instead of 'encode', then it may be something that needs fixing in ``i18ndude``.
 Please `report <https://github.com/collective/i18ndude/issues>`_ it then.
+
+Pre commit hook
+---------------
+
+Since version 6 we have a ``pre-commit`` hook available::
+
+    -   repo: https://github.com/collective/i18ndude
+        rev: "master"
+        hooks:
+        -   id: i18ndude
+
+For now it only finds the strings not marked for translation.
```

### Comparing `i18ndude-5.5.0/CHANGES.rst` & `i18ndude-6.0.0a1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,39 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.0.0a1 (2023-05-08)
+--------------------
+
+Breaking changes:
+
+
+- Drop support for Python 2.
+  Require Python 3.8+ (works with PyPy3 as well).
+  [gforcada, maurits] (#50)
+
+
+New features:
+
+
+- Add pre-commit hook, for now only to find the strings not marked for translation.
+  [gforcada] (#50)
+
+
+Bug fixes:
+
+
+- Fix encoding problem on `prepare_cli_documentation` command.
+  [gforcada] (#101)
+
+
 5.5.0 (2022-09-19)
 ------------------
 
 New features:
 
 
 - Add boolean ``--no-line-numbers`` option to ``rebuild-pot``.
```

### Comparing `i18ndude-5.5.0/src/i18ndude/catalog.py` & `i18ndude-6.0.0a1/src/i18ndude/catalog.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/interfaces.py` & `i18ndude-6.0.0a1/src/i18ndude/interfaces.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test2_expected-en.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2_expected-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test.zcml` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.zcml`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test3.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test3.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test-en.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/synctest-de.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest-de.po`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test.xml` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.xml`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/synctest.pot` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest.pot`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test1.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test1.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test2-en.po` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/chameleon.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/chameleon.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/testdata/input/test5.pt` & `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test5.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/tests/test_utils.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/tests/test_catalog.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/tests/tox-check-i18ndude-command.sh` & `i18ndude-6.0.0a1/src/i18ndude/tests/tox-check-i18ndude-command.sh`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/tests/test_untranslated.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/test_untranslated.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/tests/utils.py` & `i18ndude-6.0.0a1/src/i18ndude/tests/utils.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/visualisation.py` & `i18ndude-6.0.0a1/src/i18ndude/visualisation.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/zcmlextract.py` & `i18ndude-6.0.0a1/src/i18ndude/zcmlextract.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/generator.py` & `i18ndude-6.0.0a1/src/i18ndude/generator.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/common.py` & `i18ndude-6.0.0a1/src/i18ndude/common.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/utils.py` & `i18ndude-6.0.0a1/src/i18ndude/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     result.append(marker)
     result.append('')
 
     def indent(text):
         result = []
         for line in text.splitlines():
             if line:
-                result.append('  ' + line)
+                result.append('  ' + line.decode())
             else:
                 result.append('')
         return result
 
     base_cmd = 'bin/i18ndude'
     # Add result off calling bin/i18ndude --help
     result.append('i18ndude')
```

### Comparing `i18ndude-5.5.0/src/i18ndude/untranslated.py` & `i18ndude-6.0.0a1/src/i18ndude/untranslated.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/gsextract.py` & `i18ndude-6.0.0a1/src/i18ndude/gsextract.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/script.py` & `i18ndude-6.0.0a1/src/i18ndude/script.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/extract.py` & `i18ndude-6.0.0a1/src/i18ndude/extract.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude/pygettext.py` & `i18ndude-6.0.0a1/src/i18ndude/pygettext.py`

 * *Files identical despite different names*

### Comparing `i18ndude-5.5.0/src/i18ndude.egg-info/SOURCES.txt` & `i18ndude-6.0.0a1/src/i18ndude.egg-info/SOURCES.txt`

 * *Files identical despite different names*


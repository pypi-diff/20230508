# Comparing `tmp/transmogrify.dexterity-2.0.0.tar.gz` & `tmp/transmogrify.dexterity-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transmogrify.dexterity-2.0.0.tar", last modified: Tue Sep 28 06:15:28 2021, max compression
+gzip compressed data, was "transmogrify.dexterity-3.0.0.tar", last modified: Mon May  8 15:52:28 2023, max compression
```

## Comparing `transmogrify.dexterity-2.0.0.tar` & `transmogrify.dexterity-3.0.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.626926 transmogrify.dexterity-2.0.0/
--rw-r--r--   0 maethu     (501) staff       (20)     3772 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/CHANGES.rst
--rw-r--r--   0 maethu     (501) staff       (20)       98 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/CONTRIBUTORS.rst
--rw-r--r--   0 maethu     (501) staff       (20)      586 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/DEVELOP.rst
--rw-r--r--   0 maethu     (501) staff       (20)      665 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/LICENSE.rst
--rw-r--r--   0 maethu     (501) staff       (20)       69 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/MANIFEST.in
--rw-r--r--   0 maethu     (501) staff       (20)     9905 2021-09-28 06:15:28.627117 transmogrify.dexterity-2.0.0/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)     2477 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/README.rst
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.617984 transmogrify.dexterity-2.0.0/docs/
--rw-r--r--   0 maethu     (501) staff       (20)     7980 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/docs/conf.py
--rw-r--r--   0 maethu     (501) staff       (20)       89 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/docs/index.rst
--rw-r--r--   0 maethu     (501) staff       (20)      302 2021-09-28 06:15:28.627646 transmogrify.dexterity-2.0.0/setup.cfg
--rw-r--r--   0 maethu     (501) staff       (20)     2848 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/setup.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.614705 transmogrify.dexterity-2.0.0/src/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.618258 transmogrify.dexterity-2.0.0/src/transmogrify/
--rw-r--r--   0 maethu     (501) staff       (20)      269 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/__init__.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.623243 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/
--rw-r--r--   0 maethu     (501) staff       (20)      192 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      931 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)    16444 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/converters.py
--rw-r--r--   0 maethu     (501) staff       (20)     1119 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/converters.zcml
--rw-r--r--   0 maethu     (501) staff       (20)      309 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/interfaces.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.624626 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/
--rw-r--r--   0 maethu     (501) staff       (20)       24 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)     1136 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)     1772 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/csvimport.cfg
--rw-r--r--   0 maethu     (501) staff       (20)      537 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/export.cfg
--rw-r--r--   0 maethu     (501) staff       (20)     1190 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/import.cfg
--rw-r--r--   0 maethu     (501) staff       (20)     2487 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/schemareader.py
--rw-r--r--   0 maethu     (501) staff       (20)     9074 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/schemaupdater.py
--rw-r--r--   0 maethu     (501) staff       (20)     2822 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/serializer.py
--rw-r--r--   0 maethu     (501) staff       (20)     8119 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/testing.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.626691 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)     3326 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/pipelinescsvsource.txt
--rw-r--r--   0 maethu     (501) staff       (20)     3156 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/schemaupdater.txt
--rw-r--r--   0 maethu     (501) staff       (20)     1517 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/test_doctests.py
--rw-r--r--   0 maethu     (501) staff       (20)    11067 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/testconverters.py
--rw-r--r--   0 maethu     (501) staff       (20)     6224 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/testconverters_object.py
--rw-r--r--   0 maethu     (501) staff       (20)      361 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/tests.cfg
--rw-r--r--   0 maethu     (501) staff       (20)      587 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/tests.zcml
--rw-r--r--   0 maethu     (501) staff       (20)     2400 2021-09-28 06:15:27.000000 transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/translation.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2021-09-28 06:15:28.620454 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/
--rw-r--r--   0 maethu     (501) staff       (20)     9905 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)     1621 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/SOURCES.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/dependency_links.txt
--rw-r--r--   0 maethu     (501) staff       (20)      147 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/entry_points.txt
--rw-r--r--   0 maethu     (501) staff       (20)       13 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/namespace_packages.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/not-zip-safe
--rw-r--r--   0 maethu     (501) staff       (20)      367 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/requires.txt
--rw-r--r--   0 maethu     (501) staff       (20)       13 2021-09-28 06:15:28.000000 transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/top_level.txt
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.316126 transmogrify.dexterity-3.0.0/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     3834 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/CHANGES.md
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      122 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/CONTRIBUTORS.md
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)    18092 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/LICENSE.GPL
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      144 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/MANIFEST.in
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     9964 2023-05-08 15:52:28.316126 transmogrify.dexterity-3.0.0/PKG-INFO
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     4328 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/README.md
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.304126 transmogrify.dexterity-3.0.0/docs/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     7975 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/docs/conf.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       89 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/docs/index.rst
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.304126 transmogrify.dexterity-3.0.0/examples/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      537 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/examples/export.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      615 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/examples/import.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      760 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/pyproject.toml
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       38 2023-05-08 15:52:28.316126 transmogrify.dexterity-3.0.0/setup.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     2615 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/setup.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.304126 transmogrify.dexterity-3.0.0/src/
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.304126 transmogrify.dexterity-3.0.0/src/transmogrify/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      245 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/__init__.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.312126 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       30 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/__init__.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      990 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/configure.zcml
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)    14486 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/converters.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      961 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/converters.zcml
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      285 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/interfaces.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.316126 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/__init__.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1181 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/configure.zcml
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1772 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/csvimport.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      537 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/export.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1190 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/import.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     2455 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/schemareader.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     7957 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/schemaupdater.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     2776 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/serializer.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     7763 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/testing.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.316126 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/__init__.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     3320 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/pipelinescsvsource.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     3067 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/schemaupdater.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      699 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/test_doctests.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)    10284 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/testconverters.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     6159 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/testconverters_object.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      361 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/tests.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      604 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/tests.zcml
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     2171 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/translation.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-05-08 15:52:28.312126 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     9964 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/PKG-INFO
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1651 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/SOURCES.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)        1 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/dependency_links.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       53 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/entry_points.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       13 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/namespace_packages.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)        1 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/not-zip-safe
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      163 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/requires.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       13 2023-05-08 15:52:28.000000 transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/top_level.txt
```

### Comparing `transmogrify.dexterity-2.0.0/CHANGES.rst` & `transmogrify.dexterity-3.0.0/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,147 @@
-Changelog
-=========
+## Changelog
 
+## 3.0.0 (2023-05-08)
 
-2.0.0 (2021-09-28)
-------------------
+- Doesn't try to convert byte to string. Python converts to string when json is loaded. @wesleybl
 
-- Import relations fields that were exported as UID.
-  [wesleybl]
+- Add Python 3.10 and 3.11 support @wesleybl
 
-- Update plone.dublincore behavior fields, even if the object doesn't have
-  this behavior.
-  [wesleybl]
+- Implement plone/code-analysis-action @ericof
 
-- Add suport to Python 3.7 and 3.8
-  [wesleybl]
+- Add support to Plone 6.0 @ericof
 
-- Add suport to Plone 4.3, 5.0, 5.1 and 5.2
-  [wesleybl]
+- Drop support to Plone versions 4.3, 5.0 and 5.1 @ericof
 
+- Drop support to Python 2.7 @ericof
 
-1.6.4 (2018-12-14)
-------------------
 
-- Fix date deserialization to work with any kind of separator or when it is None.
-  [gbastien]
+### 2.0.0 (2021-09-28)
 
-- DatetimeDeserializer: check for the case when value is an empty string.
-  [erral]
+- Import relations fields that were exported as UID. @wesleybl
 
-1.6.3 (2016-10-11)
-------------------
+- Update plone.dublincore behavior fields, even if the object doesn't have this behavior. @wesleybl
 
-- Refactor DexterityUpdateSection: Factor out determining default value,
-  getting value from pipeline and updating fields into their own methods.
-  [lgraf]
+- Add suport to Python 3.7 and 3.8 @wesleybl
 
+- Add suport to Plone 4.3, 5.0, 5.1 and 5.2 @wesleybl
 
-1.6.2 (2016-05-24)
-------------------
 
-- Fix blueprint context for support with ``transmogrifier`` package (not ``collective.transmogrifier``), which does not have dependencies to CMFPlone and thus doesn't provide a useful context.
-  [thet]
+### 1.6.4 (2018-12-14)
 
+- Fix date deserialization to work with any kind of separator or when it is None. @gbastien
 
-1.6.1 (2015-09-30)
-------------------
+- DatetimeDeserializer: check for the case when value is an empty string. @erral
 
-- Do not import from deprecated zope.app.intid anymore, use zope.intid instead
-  [jensens]
+### 1.6.3 (2016-10-11)
 
-- Fix deserializer if datetime is string "None".
-  [elioschmutz]
+- Refactor DexterityUpdateSection: Factor out determining default value, getting value from pipeline and updating fields into their own methods. @lgraf
 
 
-1.6.0 (2015-08-28)
-------------------
+### 1.6.2 (2016-05-24)
 
-- Implement new deserializer for datetime fields.
-  [mbaechtold]
+- Fix blueprint context for support with ``transmogrifier`` package (not ``collective.transmogrifier``), which does not have dependencies to CMFPlone and thus doesn't provide a useful context. @thet
 
 
-1.5.2 (2015-07-13)
-------------------
+### 1.6.1 (2015-09-30)
 
-- Fix default container description to be unicode, not bytestring.
-  See https://github.com/plone/plone.dexterity/pull/33
-  [jone]
+- Do not import from deprecated zope.app.intid anymore, use zope.intid instead @jensens
 
+- Fix deserializer if datetime is string "None". @elioschmutz
 
-1.5.1 (2015-05-27)
-------------------
 
-- Make z3c.relationfield imports conditional.
-  [jone]
+### 1.6.0 (2015-08-28)
+
+- Implement new deserializer for datetime fields. @mbaechtold
+
+
+### 1.5.2 (2015-07-13)
+
+- Fix default container description to be unicode, not bytestring. See https://github.com/plone/plone.dexterity/pull/33 @jone
+
+
+### 1.5.1 (2015-05-27)
+
+- Make z3c.relationfield imports conditional. @jone
 
 
 1.5 (2015-05-26)
 ----------------
 
 - When retrieving the object via traversal from the path, check if it provides
   IDexterityContent. Traversal can also return attributes of objects, if no
-  object can be found but the path element is named like an attribute.
-  [thet]
+  object can be found but the path element is named like an attribute. @thet
 
-- Handle collective.jsonify structures, specifically _datafield_FIELDNAME and
-  _content_type_FIELDNAME keys.
-  [thet]
+- Handle collective.jsonify structures, specifically _datafield_FIELDNAME and _content_type_FIELDNAME keys. @thet
 
-- PEP8.
-  [thet]
+- PEP8. @thet
 
-- Add value converters for z3c.relationfield relation(-lists).
-  [deiferni]
+- Add value converters for z3c.relationfield relation(-lists). @deiferni
 
 
 1.4 (2014-11-06)
 ----------------
 
-- Add blueprint for managing plone.app.multilingual translations
-  [rnix]
+- Add blueprint for managing plone.app.multilingual translations @rnix
 
 
 1.3 (2014-07-25)
 ----------------
 
-- Use zope.dottedname.resolve to find class
-  [lentinj]
+- Use zope.dottedname.resolve to find class @lentinj
 
-- Serialize/Deserialize zope.schema.IObjects
-  [lentinj]
+- Serialize/Deserialize zope.schema.IObjects @lentinj
 
-- Add 'logger' and 'loglevel' options so invalid fields are logged when
-  disable-constraints is True
-  [ebrehault]
+- Add 'logger' and 'loglevel' options so invalid fields are logged when disable-constraints is True @ebrehault
 
 
 1.2 (2013-08-29)
 ----------------
 
 - Only update with a default value if there isn't a value already set
   on the field. (NB: before a default value would be set, regardless
-  of the current field value).
-  [lentinj]
+  of the current field value). @lentinj
 
 
 1.1 (2013-07-23)
 ----------------
 
-- Don't try to write readonly fields
-  [djowett]
+- Don't try to write readonly fields @djowett
 
-- Added in a generic CSV -> content pipeline
-  [lentinj]
+- Added in a generic CSV -> content pipeline @lentinj
 
 
 1.0 (2011-11-17)
 ----------------
 
-- Updated changelog to be zest releaser compatible
-  [lgraf]
+- Updated changelog to be zest releaser compatible @lgraf
 
 
-1.0a5 (2011-07-18)
-------------------
+### 1.0a5 (2011-07-18)
 
 - Added check-constraints option to schemaupdater section.
   If set to False, field values that are set in the schemaupdater section won't
-  be validated against the field's constraints.
-  [lgraf]
+  be validated against the field's constraints. @lgraf
 
-- Made CollectionDeserializer cast None and empty string to an empty list
-  [lgraf]
+- Made CollectionDeserializer cast None and empty string to an empty list @lgraf
 
-- Added a basic DateDeserializer
-  [lgraf]
+- Added a basic DateDeserializer @lgraf
 
-- Using new-style classes for [de]serializers
-  [lgraf]
+- Using new-style classes for [de]serializers @lgraf
 
 
-1.0a4 (2011-06-07)
-------------------
+### 1.0a4 (2011-06-07)
 
-- Ensure RichTextValue gets a decoded unicode string, add tests
-  [lentinj]
+- Ensure RichTextValue gets a decoded unicode string, add tests @lentinj
 
-- Refactor to support more field types.
-  [elro]
+- Refactor to support more field types. @elro
 
 
-1.0a3 (2010-03-12)
-------------------
+### 1.0a3 (2010-03-12)
 
-- Fixed bug in typechecking of values for Boolean fields
-  [lgraf]
+- Fixed bug in typechecking of values for Boolean fields @lgraf
 
-- fixed dateconverting
-  [phgross]
+- fixed dateconverting @phgross
 
-- fixed value check: so that it works correctly with an empty string
-  [phgross]
+- fixed value check: so that it works correctly with an empty string @phgross
 
-- fixed handling for list and bool fields
-  [phgross]
+- fixed handling for list and bool fields @phgross
```

### Comparing `transmogrify.dexterity-2.0.0/docs/conf.py` & `transmogrify.dexterity-3.0.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,26 +39,26 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"transmogrify.dexterity"
-copyright = u"4teamwork AG ()"
-author = u"4teamwork AG ()"
+project = "transmogrify.dexterity"
+copyright = "4teamwork AG ()"
+author = "4teamwork AG ()"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u"3.0"
+version = "3.0"
 # The full version, including alpha/beta/rc tags.
-release = u"3.0"
+release = "3.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `transmogrify.dexterity-2.0.0/setup.py` & `transmogrify.dexterity-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,76 @@
-# -*- coding: utf-8 -*-
 """Installer for the transmogrify.dexterity package."""
-
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-long_description = "\n\n".join(
-    [
-        open("README.rst").read(),
-        open("CONTRIBUTORS.rst").read(),
-        open("CHANGES.rst").read(),
-    ]
-)
+long_description = f"""
+{Path("README.md").read_text()}\n
+{Path("CONTRIBUTORS.md").read_text()}\n
+{Path("CHANGES.md").read_text()}\n
+"""
 
 
 setup(
     name="transmogrify.dexterity",
-    version="2.0.0",
+    version="3.0.0",
     description="A transmogrifier blueprint for updating dexterity objects",
     long_description=long_description,
-    # Get more from https://pypi.org/classifiers/
+    long_description_content_type="text/markdown",
     classifiers=[
+        "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
-        "Framework :: Plone",
-        "Framework :: Plone :: Addon",
-        "Framework :: Plone :: 4.3",
-        "Framework :: Plone :: 5.0",
-        "Framework :: Plone :: 5.1",
         "Framework :: Plone :: 5.2",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
+        "Framework :: Plone :: 6.0",
+        "Framework :: Plone :: Addon",
+        "Framework :: Plone",
+        "Framework :: Zope2",
+        "Framework :: Zope3",
+        "License :: OSI Approved :: GNU General Public License (GPL)",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="Python Plone CMS",
     author="4teamwork AG",
     author_email="info@4teamwork.ch",
     url="https://github.com/collective/transmogrify.dexterity",
     project_urls={
         "PyPI": "https://pypi.python.org/pypi/transmogrify.dexterity",
         "Source": "https://github.com/collective/transmogrify.dexterity",
         "Tracker": "https://github.com/collective/transmogrify.dexterity/issues",
-        # 'Documentation': 'https://transmogrify.dexterity.readthedocs.io/en/latest/',
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["transmogrify"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7, >=3.7",
+    python_requires=">=3.7",
     install_requires=[
         "collective.transmogrifier",
-        "plone.app.textfield",
         "plone.app.transmogrifier",
-        "plone.app.uuid",
-        "plone.dexterity",
-        "plone.namedfile",
-        "plone.supermodel",
-        "plone.uuid",
         "Products.CMFPlone",
         "setuptools",
-        "six",
-        "z3c.form",
-        "zope.component",
     ],
     extras_require={
         "test": [
-            "ftw.builder",
-            "plone.api",
-            "plone.app.dexterity",
-            "plone.app.intid",
+            "zope.testrunner",
             "plone.app.testing",
             "plone.formwidget.contenttree",
-            "plone.namedfile[blobs]",
-            "unittest2",
-            "z3c.relationfield",
+            "ftw.builder",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
-    [console_scripts]
-    update_locale = transmogrify.dexterity.locales.update:update_locale
     """,
 )
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/configure.zcml` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/configure.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:zcml="http://namespaces.zope.org/zcml"
-  i18n_domain="transmogrify.dexterity">
-
-  <include package="collective.transmogrifier" file="meta.zcml" />
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="transmogrify.dexterity"
+    >
+
+  <include
+      package="collective.transmogrifier"
+      file="meta.zcml"
+      />
   <include package="collective.transmogrifier" />
 
   <include file="converters.zcml" />
   <include package=".pipelines" />
 
   <utility
+      name="transmogrify.dexterity.schemaupdater"
       component=".schemaupdater.DexterityUpdateSection"
-      name="transmogrify.dexterity.schemaupdater" />
+      />
 
   <utility
+      name="transmogrify.dexterity.schemareader"
       component=".schemareader.DexterityReaderSection"
-      name="transmogrify.dexterity.schemareader" />
+      />
 
   <utility
+      name="transmogrify.dexterity.translation"
       component=".translation.DexterityTranslationSection"
-      name="transmogrify.dexterity.translation" />
+      />
 
   <utility
+      name="transmogrify.dexterity.serializer"
       component=".serializer.SerializerSection"
-      name="transmogrify.dexterity.serializer" />
+      />
 
   <utility
+      name="transmogrify.dexterity.deserializer"
       component=".serializer.DeserializerSection"
-      name="transmogrify.dexterity.deserializer" />
+      />
 
 </configure>
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/converters.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/converters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,62 @@
-# -*- coding: utf-8 -*-
 from datetime import datetime
 from DateTime import DateTime
 from plone.app.textfield.interfaces import IRichText
 from plone.app.textfield.value import RichTextValue
 from plone.app.uuid.utils import uuidToObject
 from plone.namedfile.interfaces import INamedField
 from plone.supermodel.interfaces import IToUnicode
 from transmogrify.dexterity.interfaces import IDeserializer
 from transmogrify.dexterity.interfaces import ISerializer
+from z3c.relationfield.interfaces import IRelation
+from z3c.relationfield.interfaces import IRelationList
+from z3c.relationfield.relation import RelationValue
 from zope.component import adapter
 from zope.component import queryUtility
 from zope.dottedname.resolve import resolve
 from zope.interface import implementer
+from zope.intid.interfaces import IIntIds
 from zope.schema.interfaces import ICollection
 from zope.schema.interfaces import IDate
 from zope.schema.interfaces import IDatetime
 from zope.schema.interfaces import IField
 from zope.schema.interfaces import IFromUnicode
 from zope.schema.interfaces import IObject
 
 import base64
 import mimetypes
-import pkg_resources
-import six
 
 
-try:
-    pkg_resources.get_distribution("plone.app.intid")
-except pkg_resources.DistributionNotFound:
-    INTID_AVAILABLE = False
-else:
-    INTID_AVAILABLE = True
-    from zope.intid.interfaces import IIntIds
-
-try:
-    pkg_resources.get_distribution("z3c.relationfield")
-except pkg_resources.DistributionNotFound:
-    RELATIONFIELD_AVAILABLE = False
-else:
-    RELATIONFIELD_AVAILABLE = True
-    from z3c.relationfield.interfaces import IRelation
-    from z3c.relationfield.interfaces import IRelationList
-    from z3c.relationfield.relation import RelationValue
-
-
-def get_site_encoding():
-    # getSiteEncoding was in plone.app.textfield.utils but is not gone. Like
-    # ``Products.CMFPlone.browser.ploneview``, it always returned 'utf-8',
-    # something we can do ourselves here.
-    # TODO: use some sane getSiteEncoding from CMFPlone, once there is one.
-    return "utf-8"
+ENCODING = "utf-8"
 
 
 @implementer(ISerializer)
 @adapter(INamedField)
-class NamedFileSerializer(object):
+class NamedFileSerializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, extra=None):
         if extra is None:
             extra = ""
         else:
-            extra = "_%s" % extra
+            extra = f"_{extra}"
         fieldname = self.field.__name__
         if hasattr(value, "open"):
             data = value.open().read()
         else:
             data = value.data
-        name = "_field_%s%s_%s" % (fieldname, extra, value.filename)
+        name = f"_field_{fieldname}{extra}_{value.filename}"
         filestore[name] = dict(data=data, name=name, contenttype=value.contentType)
         return dict(file=name, filename=value.filename, contenttype=value.contentType)
 
 
 @implementer(IDeserializer)
 @adapter(INamedField)
-class NamedFileDeserializer(object):
+class NamedFileDeserializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
         if isinstance(value, dict):
             filename = value.get("filename", None)
             contenttype = str(value.get("contenttype", ""))
@@ -98,87 +75,73 @@
 
         elif isinstance(value, str):
             data = value
             filename = item.get("_filename", None)
             contenttype = ""
         else:
             raise ValueError("Unable to convert to named file")
-        if six.PY2 and isinstance(filename, str):
-            filename = filename.decode("utf-8")
         instance = self.field._type(
             data=data,
             filename=filename,
             contentType=contenttype,
         )
         try:
             self.field.validate(instance)
         except Exception as e:
             if not disable_constraints:
                 raise e
             else:
                 if logger:
+                    field_name = self.field.__name__
+                    path = item["_path"]
                     logger(
-                        "NamedFileDeserializer: %s is invalid in %s: %s"
-                        % (self.field.__name__, item["_path"], e)
+                        f"NamedFileDeserializer: {field_name} is invalid in {path}: {e}"
                     )
         return instance
 
 
 @implementer(ISerializer)
 @adapter(IRichText)
-class RichTextSerializer(object):
+class RichTextSerializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, extra=None):
-        if extra is None:
-            extra = ""
-        else:
-            extra = "_%s" % extra
+        extra = "" if extra is None else f"_{extra}"
         extension = mimetypes.guess_extension(value.mimeType) or ""
         fieldname = self.field.__name__
-        name = "_field_%s%s%s" % (fieldname, extra, extension)
+        name = f"_field_{fieldname}{extra}{extension}"
         filestore[name] = dict(
             data=value.raw_encoded, name=name, contenttype=value.mimeType
         )
         return dict(file=name, contenttype=value.mimeType, encoding=value.encoding)
 
 
 @implementer(IDeserializer)
 @adapter(IRichText)
-class RichTextDeserializer(object):
+class RichTextDeserializer:
     _type = RichTextValue
 
     def __init__(self, field):
         self.field = field
 
-    def _convert_object(self, obj, encoding):
-        """Decode binary strings into unicode objects"""
-        if not six.PY2 and isinstance(obj, str):
-            return obj
-        if isinstance(obj, str):
-            return obj.decode(encoding)
-        if isinstance(obj, unicode):
-            return obj
-        raise ValueError("Unable to convert value to unicode string")
-
     def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
         if isinstance(value, dict):
-            encoding = value.get("encoding", get_site_encoding())
+            encoding = value.get("encoding", ENCODING)
             contenttype = value.get("contenttype", None)
             if contenttype is not None:
                 contenttype = str(contenttype)
             file = value.get("file", None)
             if file is not None:
-                data = self._convert_object(filestore[file]["data"], encoding)
+                data = filestore[file]["data"]
             else:
-                data = self._convert_object(value["data"], encoding)
+                data = value["data"]
         else:
-            encoding = get_site_encoding()
-            data = self._convert_object(value, encoding)
+            encoding = ENCODING
+            data = value
             contenttype = None
         if contenttype is None:
             contenttype = self.field.default_mime_type
         instance = self._type(
             raw=data,
             mimeType=contenttype,
             outputMimeType=self.field.output_mime_type,
@@ -187,24 +150,25 @@
         try:
             self.field.validate(instance)
         except Exception as e:
             if not disable_constraints:
                 raise e
             else:
                 if logger:
+                    field_name = self.field.__name__
+                    path = item["_path"]
                     logger(
-                        "RichTextDeserializer: %s is invalid in %s: %s"
-                        % (self.field.__name__, item["_path"], e)
+                        f"RichTextDeserializer: {field_name} is invalid in {path}: {e}"
                     )
         return instance
 
 
 @implementer(ISerializer)
 @adapter(IObject)
-class ObjectSerializer(object):
+class ObjectSerializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, extra=""):
         out = {
             "_class": "%s.%s"
             % (
@@ -216,15 +180,15 @@
             serializer = ISerializer(self.field.schema[k])
             out[k] = serializer(getattr(value, k), filestore, extra + k)
         return out
 
 
 @implementer(IDeserializer)
 @adapter(IObject)
-class ObjectDeserializer(object):
+class ObjectDeserializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
         if not isinstance(value, dict):
             raise ValueError("Need a dict to convert")
         if not value.get("_class", None):
@@ -289,38 +253,38 @@
         if not disable_constraints:
             self.field.validate(instance)
         return instance
 
 
 @implementer(ISerializer)
 @adapter(ICollection)
-class CollectionSerializer(object):
+class CollectionSerializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, extra=None):
         field = self.field
         if field.value_type is not None:
             serializer = ISerializer(self.field.value_type)
         else:
             serializer = DefaultSerializer()
         return [serializer(v, filestore, str(i)) for i, v in enumerate(value)]
 
 
 @implementer(IDeserializer)
 @adapter(ICollection)
-class CollectionDeserializer(object):
+class CollectionDeserializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
         field = self.field
         if value in (None, ""):
             return []
-        if isinstance(value, six.string_types):
+        if isinstance(value, str):
             value = [v for v in (v.strip() for v in value.split(";")) if v]
         if field.value_type is not None:
             deserializer = IDeserializer(self.field.value_type)
         else:
             deserializer = DefaultDeserializer(None)
         value = [
             deserializer(v, filestore, item, disable_constraints, logger=logger)
@@ -330,167 +294,154 @@
         try:
             self.field.validate(value)
         except Exception as e:
             if not disable_constraints:
                 raise e
             else:
                 if logger:
+                    field_name = self.field.__name__
+                    path = item["_path"]
                     logger(
-                        "CollectionDeserializer: %s is invalid in %s: %s"
-                        % (self.field.__name__, item["_path"], e)
+                        f"CollectionDeserializer: {field_name} is invalid in {path}: {e}"
                     )
         return value
 
 
 @implementer(IDeserializer)
 @adapter(IDate)
-class DateDeserializer(object):
+class DateDeserializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
-        if isinstance(value, six.string_types):
-            if value in ("", "None"):
-                value = None
-            else:
-                value = DateTime(value).asdatetime().date()
+        if isinstance(value, str):
+            value = None if value in ("", "None") else DateTime(value).asdatetime()
         if isinstance(value, datetime):
             value = value.date()
         try:
             self.field.validate(value)
         except Exception as e:
             if not disable_constraints:
                 raise e
             else:
                 if logger:
-                    logger(
-                        "DateDeserializer: %s is invalid in %s: %s"
-                        % (self.field.__name__, item["_path"], e)
-                    )
+                    field_name = self.field.__name__
+                    path = item["_path"]
+                    logger(f"DateDeserializer: {field_name} is invalid in {path}: {e}")
         return value
 
 
 @implementer(IDeserializer)
 @adapter(IDatetime)
-class DatetimeDeserializer(object):
+class DatetimeDeserializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
-        if isinstance(value, six.string_types):
-            if value in ("", "None"):
-                value = None
-            else:
-                value = DateTime(value).asdatetime()
+        if isinstance(value, str):
+            value = None if value in ("", "None") else DateTime(value).asdatetime()
         try:
             self.field.validate(value)
         except Exception as e:
             if not disable_constraints:
                 raise e
             else:
                 if logger:
+                    field_name = self.field.__name__
+                    path = item["_path"]
                     logger(
-                        "DatetimeDeserializer: %s is invalid in %s: %s"
-                        % (self.field.__name__, item["_path"], e)
+                        f"DatetimeDeserializer: {field_name} is invalid in {path}: {e}"
                     )
         return value
 
 
 @implementer(ISerializer)
 @adapter(IField)
-class DefaultSerializer(object):
+class DefaultSerializer:
     def __init__(self, field=None):
         self.field = field
 
     def __call__(self, value, filestore, extra=None):
-        BASIC_TYPES = (six.text_type, int, int, float, bool, type(None))
+        BASIC_TYPES = (str, int, float, bool, type(None))
         if type(value) in BASIC_TYPES:
             pass
         elif self.field is not None:
             value = IToUnicode(self.field).toUnicode(value)
         else:
             raise ValueError("Unable to serialize field value")
         return value
 
 
 @implementer(IDeserializer)
 @adapter(IField)
-class DefaultDeserializer(object):
+class DefaultDeserializer:
     def __init__(self, field):
         self.field = field
 
     def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
         field = self.field
         if field is not None:
             try:
-                if six.PY2:
-                    if isinstance(value, str):
-                        value = value.decode("utf-8")
-                    if isinstance(value, unicode):
-                        value = IFromUnicode(field).fromUnicode(value)
-                else:
-                    if isinstance(value, str):
-                        value = IFromUnicode(field).fromUnicode(value)
+                if isinstance(value, str):
+                    value = IFromUnicode(field).fromUnicode(value)
                 self.field.validate(value)
             except Exception as e:
                 if not disable_constraints:
                     raise e
                 else:
                     if logger:
+                        field_name = self.field.__name__
+                        path = item["_path"]
                         logger(
-                            "DefaultDeserializer: %s is invalid in %s: %s"
-                            % (self.field.__name__, item["_path"], e.__repr__())
+                            f"DefaultDeserializer: {field_name} is invalid in {path}: {e}"
                         )
         return value
 
 
-if INTID_AVAILABLE and RELATIONFIELD_AVAILABLE:
+@implementer(IDeserializer)
+@adapter(IRelation)
+class RelationDeserializer:
 
-    @implementer(IDeserializer)
-    @adapter(IRelation)
-    class RelationDeserializer(object):
-
-        default_value = None
-
-        def __init__(self, field):
-            self.field = field
-
-        def __call__(
-            self, value, filestore, item, disable_constraints=False, logger=None
-        ):
-            field = self.field
-            if field is None:
-                return None
-
-            if not value:
-                return self.default_value
-
-            self.intids = queryUtility(IIntIds)
-            if self.intids is None:
-                return value
-
-            return self.deserialize(value)
-
-        def deserialize(self, value):
-            if isinstance(value, str):
-                content = uuidToObject(value)
-                if content:
-                    return RelationValue(self.intids.getId(content))
-                else:
-                    return
-            int_id = self.intids.queryId(value)
-            if int_id is None:
-                return value
-
-            return RelationValue(int_id)
-
-    @implementer(IDeserializer)
-    @adapter(IRelationList)
-    class RelationListDeserializer(RelationDeserializer):
-
-        default_value = []
-
-        def deserialize(self, value):
-            result = []
-            for obj in value:
-                result.append(super(RelationListDeserializer, self).deserialize(obj))
-            return result
+    default_value = None
+
+    def __init__(self, field):
+        self.field = field
+
+    def __call__(self, value, filestore, item, disable_constraints=False, logger=None):
+        field = self.field
+        if field is None:
+            return None
+
+        if not value:
+            return self.default_value
+
+        self.intids = queryUtility(IIntIds)
+        if self.intids is None:
+            return value
+
+        return self.deserialize(value)
+
+    def deserialize(self, value):
+        if isinstance(value, str):
+            content = uuidToObject(value)
+            if content:
+                return RelationValue(self.intids.getId(content))
+            else:
+                return
+        int_id = self.intids.queryId(value)
+        if int_id is None:
+            return value
+
+        return RelationValue(int_id)
+
+
+@implementer(IDeserializer)
+@adapter(IRelationList)
+class RelationListDeserializer(RelationDeserializer):
+
+    default_value = []
+
+    def deserialize(self, value):
+        result = []
+        for obj in value:
+            result.append(super().deserialize(obj))
+        return result
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/converters.zcml` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/converters.zcml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  i18n_domain="transmogrify.dexterity"
-  xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="transmogrify.dexterity"
+    >
 
   <adapter factory=".converters.NamedFileSerializer" />
   <adapter factory=".converters.NamedFileDeserializer" />
 
   <adapter factory=".converters.RichTextSerializer" />
   <adapter factory=".converters.RichTextDeserializer" />
 
@@ -17,15 +18,12 @@
 
   <adapter factory=".converters.DateDeserializer" />
   <adapter factory=".converters.DatetimeDeserializer" />
 
   <adapter factory=".converters.DefaultSerializer" />
   <adapter factory=".converters.DefaultDeserializer" />
 
-  <configure zcml:condition="installed plone.app.intid">
-      <configure zcml:condition="installed z3c.relationfield">
-          <adapter factory=".converters.RelationDeserializer" />
-          <adapter factory=".converters.RelationListDeserializer" />
-      </configure>
-  </configure>
+
+  <adapter factory=".converters.RelationDeserializer" />
+  <adapter factory=".converters.RelationListDeserializer" />
 
 </configure>
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/csvimport.cfg` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/csvimport.cfg`

 * *Files identical despite different names*

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/export.cfg` & `transmogrify.dexterity-3.0.0/examples/export.cfg`

 * *Files identical despite different names*

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/pipelines/import.cfg` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/pipelines/import.cfg`

 * *Files identical despite different names*

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/schemareader.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/schemareader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from collective.transmogrifier.interfaces import ISection
 from collective.transmogrifier.interfaces import ISectionBlueprint
 from collective.transmogrifier.utils import defaultMatcher
 from plone.dexterity.interfaces import IDexterityContent
 from plone.dexterity.utils import iterSchemata
 from plone.uuid.interfaces import IUUID
 from transmogrify.dexterity.interfaces import ISerializer
@@ -10,15 +9,15 @@
 from zope.interface import implementer
 from zope.interface import provider
 from zope.schema import getFieldsInOrder
 
 
 @provider(ISectionBlueprint)
 @implementer(ISection)
-class DexterityReaderSection(object):
+class DexterityReaderSection:
     def __init__(self, transmogrifier, name, options, previous):
         self.previous = previous
         self.context = (
             transmogrifier.context if transmogrifier.context else getSite()
         )  # noqa
         self.name = name
         self.pathkey = defaultMatcher(options, "path-key", name, "path")
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/schemaupdater.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/schemaupdater.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,46 @@
-# -*- coding: utf-8 -*-
 from collective.transmogrifier.interfaces import ISection
 from collective.transmogrifier.interfaces import ISectionBlueprint
 from collective.transmogrifier.utils import defaultMatcher
 from collective.transmogrifier.utils import Expression
 from plone.app.dexterity.behaviors.metadata import DublinCore
 from plone.app.dexterity.behaviors.metadata import IDublinCore
 from plone.app.textfield.interfaces import IRichText
 from plone.dexterity.interfaces import IDexterityContent
 from plone.dexterity.utils import iterSchemata
 from plone.uuid.interfaces import IMutableUUID
-from transmogrify.dexterity import PLONE_VERSION
 from transmogrify.dexterity.interfaces import IDeserializer
 from z3c.form import interfaces
 from zope.component import getMultiAdapter
 from zope.component import queryMultiAdapter
 from zope.component.hooks import getSite
 from zope.event import notify
 from zope.interface import implementer
 from zope.interface import provider
 from zope.lifecycleevent import ObjectModifiedEvent
 from zope.schema import getFieldsInOrder
 
 import logging
-import six
 
 
 _marker = object()
 
 
-PLONE_43 = PLONE_VERSION == 4.3
-
-
 dublin_core_fields = [
     (
         name,
         field,
     )
     for name, field in getFieldsInOrder(IDublinCore)
 ]
 
 
 @provider(ISectionBlueprint)
 @implementer(ISection)
-class DexterityUpdateSection(object):
+class DexterityUpdateSection:
     def __init__(self, transmogrifier, name, options, previous):
         self.previous = previous
         self.context = (
             transmogrifier.context if transmogrifier.context else getSite()
         )  # noqa
         self.name = name
         self.pathkey = defaultMatcher(options, "path-key", name, "path")
@@ -150,28 +144,27 @@
         # Get the field's current value, if it has one then leave it alone
         value = getMultiAdapter((obj, field), interfaces.IDataManager).query()
 
         # Fix default description to be an empty unicode instead of
         # an empty bytestring because of this bug:
         # https://github.com/plone/plone.dexterity/pull/33
         if name == "description" and value == "":
-            field.set(field.interface(obj), u"")
+            field.set(field.interface(obj), "")
             return
 
         if not (value is field.missing_value or value is interfaces.NO_VALUE):
             return
 
         # Finally, set a default value if nothing is set so far
         default = self.determine_default_value(obj, field)
         field.set(field.interface(obj), default)
 
     def get_fields(self, obj):
         for schemata in iterSchemata(obj):
-            for name, field in getFieldsInOrder(schemata):
-                yield name, field
+            yield from getFieldsInOrder(schemata)
 
     def get_extras_dublin_core_fields(self, obj):
         """Returns fields of IDublinCore interface, which are not in the
         object's behaviors.
         """
         fields = list(self.get_fields(obj))
         for name_field in dublin_core_fields:
@@ -188,59 +181,33 @@
 
             path = item[pathkey]
             # Skip the Plone site object itself
             if not path:
                 yield item
                 continue
 
-            if six.PY2:
-                path = path.encode()
-
             obj = self.context.unrestrictedTraverse(path.lstrip("/"), None)
 
             if not IDexterityContent.providedBy(obj):
                 # Path doesn't exist
                 # obj can not only be None, but also the value of an attribute,
                 # which is returned by traversal.
                 yield item
                 continue
 
             uuid = item.get("plone.uuid")
             if uuid is not None:
                 IMutableUUID(obj).set(str(uuid))
 
-            creators = None
-
             # For all fields in the schema, update in roughly the same way
             # z3c.form.widget.py would
             for name, field in self.get_fields(obj):
-                if PLONE_43 and name == "creators":
-                    creators = field
-                    continue
                 self.update_field(obj, field, item)
 
-            extra_creators = None
-
             # Updates fields of IDublinCore interface, which are not in the
             # object's behaviors.
             for name, field in self.get_extras_dublin_core_fields(obj):
-                if PLONE_43 and name == "creators":
-                    extra_creators = field
-                    continue
                 self.update_field(obj, field, item, extra_dublin_core=True)
 
             notify(ObjectModifiedEvent(obj))
 
-            # BBB:In Plone 4.3 the notify(ObjectModifiedEvent(obj)) causes the
-            # user runing the migration to be added to the creators. So we need
-            # to set the creators after the event call, so the creators only
-            # have the values that are in json.
-            if creators:
-                self.update_field(obj, creators, item)
-            if extra_creators:
-                self.update_field(
-                    obj,
-                    extra_creators,
-                    item,
-                    extra_dublin_core=True,
-                )
             yield item
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/serializer.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: utf-8 -*-
 from collective.transmogrifier.interfaces import ISection
 from collective.transmogrifier.interfaces import ISectionBlueprint
 from collective.transmogrifier.utils import defaultMatcher
 from zope.component.hooks import getSite
 from zope.interface import implementer
 from zope.interface import provider
 
 import json
 
 
 @provider(ISectionBlueprint)
 @implementer(ISection)
-class SerializerSection(object):
+class SerializerSection:
     def __init__(self, transmogrifier, name, options, previous):
         self.previous = previous
         self.context = (
             transmogrifier.context if transmogrifier.context else getSite()
         )  # noqa
 
         self.pathkey = defaultMatcher(options, "path-key", name, "path")
@@ -34,19 +33,19 @@
 
             path = item.get(pathkey)
             # not enough info
             if not path:
                 yield item
                 continue
 
-            data = dict(
-                (key, value)
+            data = {
+                key: value
                 for key, value in list(item.items())
                 if not key.startswith("_")
-            )
+            }
             if not data:
                 yield item
                 continue
 
             files = item.setdefault(fileskey, {})
             files[self.key] = dict(
                 name="_content.json",
@@ -55,15 +54,15 @@
             )
 
             yield item
 
 
 @provider(ISectionBlueprint)
 @implementer(ISection)
-class DeserializerSection(object):
+class DeserializerSection:
     def __init__(self, transmogrifier, name, options, previous):
         self.previous = previous
         self.context = (
             transmogrifier.context if transmogrifier.context else getSite()
         )  # noqa
 
         self.fileskey = defaultMatcher(options, "files-key", name, "files")
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/testing.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from collective.transmogrifier.interfaces import ISection
 from collective.transmogrifier.interfaces import ISectionBlueprint
 from collective.transmogrifier.sections.tests import SampleSource
 from datetime import date
 from datetime import datetime
 from ftw.builder.testing import BUILDER_LAYER
 from ftw.builder.testing import functional_session_factory
@@ -15,23 +14,20 @@
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.textfield import RichText
 from plone.dexterity.fti import DexterityFTI
 from plone.dexterity.fti import register
 from plone.namedfile.field import NamedFile
 from plone.supermodel import model
-from transmogrify.dexterity import PLONE_VERSION
 from zope import schema
 from zope.component import provideUtility
 from zope.configuration import xmlconfig
 from zope.interface import implementer
 from zope.interface import provider
 
-import six
-
 
 zptlogo = (
     "GIF89a\x10\x00\x10\x00\xd5\x00\x00\xff\xff\xff\xff\xff\xfe\xfc\xfd\xfd"
     "\xfa\xfb\xfc\xf7\xf9\xfa\xf5\xf8\xf9\xf3\xf6\xf8\xf2\xf5\xf7\xf0\xf4\xf6"
     "\xeb\xf1\xf3\xe5\xed\xef\xde\xe8\xeb\xdc\xe6\xea\xd9\xe4\xe8\xd7\xe2\xe6"
     "\xd2\xdf\xe3\xd0\xdd\xe3\xcd\xdc\xe1\xcb\xda\xdf\xc9\xd9\xdf\xc8\xd8\xdd"
     "\xc6\xd7\xdc\xc4\xd6\xdc\xc3\xd4\xda\xc2\xd3\xd9\xc1\xd3\xd9\xc0\xd2\xd9"
@@ -43,23 +39,18 @@
     "\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
     "\x00,\x00\x00\x00\x00\x10\x00\x10\x00\x00\x06z@\x80pH,\x12k\xc8$\xd2f\x04"
     "\xd4\x84\x01\x01\xe1\xf0d\x16\x9f\x80A\x01\x91\xc0ZmL\xb0\xcd\x00V\xd4"
     "\xc4a\x87z\xed\xb0-\x1a\xb3\xb8\x95\xbdf8\x1e\x11\xca,MoC$\x15\x18{"
     "\x006}m\x13\x16\x1a\x1f\x83\x85}6\x17\x1b $\x83\x00\x86\x19\x1d!%)\x8c"
     "\x866#'+.\x8ca`\x1c`(,/1\x94B5\x19\x1e\"&*-024\xacNq\xba\xbb\xb8h\xbeb"
     "\x00A\x00;"
-)
-
-if six.PY2:
-    zptlogo_converted = zptlogo
-else:
-    zptlogo_converted = bytes(zptlogo, "utf-8")
+).encode()
 
 
-class FakeImportContext(object):
+class FakeImportContext:
     def __init__(self, filename, contents):
         self.filename = filename
         self.contents = contents
 
     def readDataFile(self, filename, subdir=None):
         if subdir is not None:
             return None
@@ -67,31 +58,31 @@
             return None
         return self.contents
 
 
 class ITestSchema(model.Schema):
 
     foo = schema.TextLine(
-        title=u"Foo",
+        title="Foo",
     )
 
     test_file = NamedFile(
-        title=u"File",
+        title="File",
     )
 
     test_date = schema.Date(
-        title=u"test_date",
+        title="test_date",
     )
 
     test_datetime = schema.Datetime(
-        title=u"test_datetime",
+        title="test_datetime",
     )
 
     fancy_text = RichText(
-        title=u"Fancy text",
+        title="Fancy text",
     )
 
 
 class TransmogrifyDexterityLayer(PloneSandboxLayer):
 
     defaultBases = (PLONE_FIXTURE, BUILDER_LAYER)
 
@@ -100,18 +91,14 @@
         import transmogrify.dexterity
 
         xmlconfig.file(
             "tests.zcml", transmogrify.dexterity.tests, context=configurationContext
         )
 
     def setUpPloneSite(self, portal):
-        # BBB: In tests of Plone 5.0 and 5.1, the plone.app.contenttypes
-        # profile is not applied by default
-        if PLONE_VERSION in (5.0, 5.1):
-            applyProfile(portal, "plone.app.contenttypes:default")
         applyProfile(portal, "plone.app.intid:default")
         # Install into Plone site using portal_setup
         setRoles(portal, TEST_USER_ID, ["Member", "Contributor", "Manager"])
 
         # portal workaround
         self.portal = portal
 
@@ -127,27 +114,28 @@
         register(fti)
 
         # create test schema source and provide it
         @provider(ISectionBlueprint)
         @implementer(ISection)
         class SchemaSource(SampleSource):
             def __init__(self, transmogrifier, name, options, previous):
-                super(SchemaSource, self).__init__(
-                    transmogrifier, name, options, previous
-                )
+                super().__init__(transmogrifier, name, options, previous)
                 sourcecontent = options.get("source-content", "full")
                 if sourcecontent == "full":
                     self.sample = (
                         dict(
                             _path="/spam",
                             foo="one value",
                             _type="TransmogrifyDexterityFTI",
                             title="Spam",
                             description="Lorem Ipsum bla bla!",
-                            test_file={"data": zptlogo, "filename": "zptlogo.gif"},
+                            test_file={
+                                "data": zptlogo.decode(),
+                                "filename": "zptlogo.gif",
+                            },
                             test_date="2010-10-12",
                             test_datetime="2010-10-12 17:59:59",
                             fieldnotchanged="nochange",
                             creators=["user1"],
                             contributors=["user2"],
                             language="en",
                             effective="2020-07-10 10:24:00.000000 UTC",
@@ -156,15 +144,15 @@
                         dict(
                             _path="/two",
                             foo="Bla",
                             _type="TransmogrifyDexterityFTI",
                             title="My Second Object",
                             # description=None, # None is not valid for this
                             # field.
-                            test_file=zptlogo,
+                            test_file=zptlogo.decode(),
                             _filename="testlogo.gif",
                             test_date=date(
                                 2010,
                                 0o1,
                                 0o1,
                             ),
                             test_datetime=datetime(2010, 0o1, 0o1, 17, 59, 59),
@@ -188,15 +176,15 @@
                         dict(
                             _path="/two",
                             _type="TransmogrifyDexterityFTI",
                             title="My Awesome Second Object",
                         ),
                     )
 
-        provideUtility(SchemaSource, name=u"transmogrify.dexterity.testsource")
+        provideUtility(SchemaSource, name="transmogrify.dexterity.testsource")
 
 
 TRANSMOGRIFY_DEXTERITY_FIXTURE = TransmogrifyDexterityLayer()
 TRANSMOGRIFY_DEXTERITY_INTEGRATION_TESTING = IntegrationTesting(
     bases=(TRANSMOGRIFY_DEXTERITY_FIXTURE,), name="TransmogrifyDexterity:Integration"
 )
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/pipelinescsvsource.txt` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/pipelinescsvsource.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,11 +84,11 @@
     >>> transmogrifier = Transmogrifier(portal)
     >>> IAnnotations(transmogrifier)[IMPORT_CONTEXT] = FakeImportContext('entries.csv',
     ... """_type,_path,fancy_text
     ... TransmogrifyDexterityFTI,content-1,"<b>Ooo</b>, la la!"
     ... TransmogrifyDexterityFTI,content-2,"<em>Amazing</em>"
     ... """)
     >>> output = transmogrifier(u'transmogrify.dexterity.csvimport')
-    >>> portal['content-1'].fancy_text.output
+    >>> portal['content-1'].fancy_text.raw
     '<b>Ooo</b>, la la!'
-    >>> portal['content-2'].fancy_text.output
+    >>> portal['content-2'].fancy_text.raw
     '<em>Amazing</em>'
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/schemaupdater.txt` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/schemaupdater.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
     >>> from plone import api
     >>> from collective.transmogrifier.meta import registerConfig
     >>> from collective.transmogrifier.transmogrifier import Transmogrifier
     >>> from DateTime import DateTime
     >>> from plone.app.dexterity.behaviors.metadata import IBasic
     >>> from transmogrify.dexterity.testing import zptlogo
-    >>> from transmogrify.dexterity.testing import zptlogo_converted
 
 Create object
 
     >>> api.content.create(portal, 'TransmogrifyDexterityFTI', 'existent')
     <Container at /plone/existent>
 
 Run transmogrifier pipeline with default settings (pipeline in tests.cfg)
@@ -55,23 +54,23 @@
 NameFileFields:
 
 Values from a dict:
     >>> spam.test_file
     <plone.namedfile.file.NamedFile object at ...>
     >>> spam.test_file.filename
     'zptlogo.gif'
-    >>> spam.test_file.data == zptlogo_converted
+    >>> spam.test_file.data == zptlogo
     True
 
 get the filename in a seperated value from the pipeline:
     >>> two.test_file
     <plone.namedfile.file.NamedFile object at ...>
     >>> two.test_file.filename
     'testlogo.gif'
-    >>> two.test_file.data == zptlogo_converted
+    >>> two.test_file.data == zptlogo
     True
 
 empty default value is of type unicode:
 
     >>> two.description
     ''
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/testconverters.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/testconverters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from datetime import datetime
 from ftw.builder import Builder
 from ftw.builder import create
 from plone.app.textfield import RichText
 from plone.formwidget.contenttree import ObjPathSourceBinder
 from transmogrify.dexterity import converters
 from transmogrify.dexterity.interfaces import IDeserializer
@@ -10,33 +9,32 @@
 from z3c.relationfield.relation import RelationValue
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope.schema import Date
 from zope.schema import Datetime
 
 import pprint
-import six
 import unittest
 import zope.component
 
 
 class TestRelationDeserializer(unittest.TestCase):
 
     layer = TRANSMOGRIFY_DEXTERITY_FUNCTIONAL_TESTING
 
     relation = RelationChoice(
-        title=u"Relation",
+        title="Relation",
         source=ObjPathSourceBinder(),
         required=False,
     )
 
     relation_list = RelationList(
-        title=u"Relation List",
+        title="Relation List",
         default=[],
-        value_type=RelationChoice(title=u"Relation", source=ObjPathSourceBinder()),
+        value_type=RelationChoice(title="Relation", source=ObjPathSourceBinder()),
         required=False,
     )
 
     def test_deserialize_relation(self):
         folder = create(Builder("folder"))
         deserializer = IDeserializer(self.relation)
         value = deserializer(folder, None, None)
@@ -102,89 +100,77 @@
         deserializer = IDeserializer(self.relation)
         value = deserializer("09ca9f4fe9304123b05656d9c449b1ad", None, None)
         self.assertIsNone(value)
 
     def test_deserialize_non_uid_relation_list(self):
         deserializer = IDeserializer(self.relation_list)
         value = deserializer(["f3d11fdbf5a9471796290df759adaab8"], None, None)
-        self.assertEquals([None], value)
+        self.assertEqual([None], value)
 
 
 class TestRichTextDeserializer(unittest.TestCase):
     def setUp(self):
         self.pp = pprint.PrettyPrinter(indent=4)
         # TODO: This should read the zcml instead
         zope.component.provideAdapter(converters.RichTextDeserializer)
 
     def test_string(self):
         """Test default options, should be able to produce an encoded UTF-8
         string of bytes"""
         rtd = IDeserializer(RichText())
         rtv = rtd("café culture", None, None)
 
-        self.assertEqual(rtv.raw, u"café culture")
-        if six.PY2:
-            self.assertEqual(rtv.raw_encoded, "caf\xc3\xa9 culture")
-        else:
-            self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
+        self.assertEqual(rtv.raw, "café culture")
+        self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
         self.assertEqual(rtv.outputMimeType, "text/x-html-safe")
         self.assertEqual(rtv.mimeType, "text/html")
         self.assertEqual(rtv.encoding, "utf-8")
 
     def test_unicode_string(self):
         """Test that a unicode value gets passed through without
         additional decoding"""
         rtd = IDeserializer(RichText())
-        rtv = rtd(u"café culture", None, None)
+        rtv = rtd("café culture", None, None)
 
-        self.assertEqual(rtv.raw, u"café culture")
-        if six.PY2:
-            self.assertEqual(rtv.raw_encoded, "caf\xc3\xa9 culture")
-        else:
-            self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
+        self.assertEqual(rtv.raw, "café culture")
+        self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
         self.assertEqual(rtv.outputMimeType, "text/x-html-safe")
         self.assertEqual(rtv.mimeType, "text/html")
         self.assertEqual(rtv.encoding, "utf-8")
 
     def test_setting_mime_type(self):
         """Test that RichText mime type options affect the RichTextValue"""
         rtd = IDeserializer(
             RichText(
                 default_mime_type="text/xml", output_mime_type="x-application/pony"
             )
         )
         rtv = rtd("café culture", None, None)
 
-        self.assertEqual(rtv.raw, u"café culture")
-        if six.PY2:
-            self.assertEqual(rtv.raw_encoded, "caf\xc3\xa9 culture")
-        else:
-            self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
+        self.assertEqual(rtv.raw, "café culture")
+        self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
         self.assertEqual(rtv.outputMimeType, "x-application/pony")
         self.assertEqual(rtv.mimeType, "text/xml")
         self.assertEqual(rtv.encoding, "utf-8")
 
     def test_dict_overrides(self):
         """Try using a dict value, ensure that we can override the MIME type,
         and that the MIME type is converted to a string"""
         rtd = IDeserializer(RichText(default_mime_type="text/csv"))
         rtv = rtd(
             {
-                "contenttype": u"x-application/pony",
+                "contenttype": "x-application/pony",
                 "data": "café culture",
             },
             None,
             None,
         )
 
-        self.assertEqual(rtv.raw, u"café culture")
-        if six.PY2:
-            self.assertEqual(rtv.raw_encoded, "caf\xc3\xa9 culture")
-        else:
-            self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
+        self.assertEqual(rtv.raw, "café culture")
+        self.assertEqual(rtv.raw_encoded, b"caf\xc3\xa9 culture")
         self.assertEqual(rtv.outputMimeType, "text/x-html-safe")
         self.assertEqual(
             rtv.mimeType,
             "x-application/pony",
             "Content type from dict should override default",
         )
         self.assertEqual(rtv.encoding, "utf-8")
@@ -197,41 +183,35 @@
                 "data": "caf\xe9 culture",
                 "encoding": "latin-1",
             },
             None,
             None,
         )
 
-        self.assertEqual(rtv.raw, u"café culture")
-        if six.PY2:
-            self.assertEqual(rtv.raw_encoded, "caf\xe9 culture")
-        else:
-            self.assertEqual(rtv.raw_encoded, b"caf\xe9 culture")
+        self.assertEqual(rtv.raw, "café culture")
+        self.assertEqual(rtv.raw_encoded, b"caf\xe9 culture")
         self.assertEqual(rtv.outputMimeType, "text/x-html-safe")
         self.assertEqual(rtv.mimeType, "text/csv")
         self.assertEqual(rtv.encoding, "latin-1")
 
     def test_dict_unicode(self):
         """Try using a dict value, ensure that a unicode string passed through
         and can be decoded properly"""
         rtd = IDeserializer(RichText(default_mime_type="text/csv"))
         rtv = rtd(
             {
-                "data": u"café culture",
+                "data": "café culture",
                 "encoding": "latin-1",
             },
             None,
             None,
         )
 
-        self.assertEqual(rtv.raw, u"café culture")
-        if six.PY2:
-            self.assertEqual(rtv.raw_encoded, "caf\xe9 culture")
-        else:
-            self.assertEqual(rtv.raw_encoded, b"caf\xe9 culture")
+        self.assertEqual(rtv.raw, "café culture")
+        self.assertEqual(rtv.raw_encoded, b"caf\xe9 culture")
         self.assertEqual(rtv.outputMimeType, "text/x-html-safe")
         self.assertEqual(rtv.mimeType, "text/csv")
         self.assertEqual(rtv.encoding, "latin-1")
 
     def test_filestore(self):
         """Try using a dict with a filestore"""
         rtd = IDeserializer(RichText(default_mime_type="text/csv"))
@@ -244,19 +224,16 @@
             },
             {
                 "my-lovely-file": {"data": "greasy spoon"},
             },
             None,
         )
 
-        self.assertEqual(rtv.raw, u"greasy spoon")
-        if six.PY2:
-            self.assertEqual(rtv.raw_encoded, "greasy spoon")
-        else:
-            self.assertEqual(rtv.raw_encoded, b"greasy spoon")
+        self.assertEqual(rtv.raw, "greasy spoon")
+        self.assertEqual(rtv.raw_encoded, b"greasy spoon")
         self.assertEqual(rtv.outputMimeType, "text/x-html-safe")
         self.assertEqual(
             rtv.mimeType,
             "x-application/cow",
             "Content type from dict should override default",
         )
         self.assertEqual(rtv.encoding, "latin-1")
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/testconverters_object.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/testconverters_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-# -*- coding: utf-8 -*-
 from plone.app.textfield import RichText
 from plone.app.textfield import RichTextValue
 from plone.supermodel import model
 from transmogrify.dexterity.interfaces import IDeserializer
 from transmogrify.dexterity.interfaces import ISerializer
 from z3c.form.object import registerFactoryAdapter
 from zope import interface
 from zope import schema
 
 import unittest
 import zope.component
 
 
 class ITestObjectA(model.Schema):
-    fish = schema.TextLine(title=u"Fish", default=u"", required=False)
+    fish = schema.TextLine(title="Fish", default="", required=False)
 
 
 @interface.implementer(ITestObjectA)
-class TestObjectA(object):
+class TestObjectA:
     fish = schema.fieldproperty.FieldProperty(ITestObjectA["fish"])
 
 
 registerFactoryAdapter(ITestObjectA, TestObjectA)
 
 
 class ITestObjectB(model.Schema):
-    title = schema.TextLine(title=u"Title", default=u"", required=False)
+    title = schema.TextLine(title="Title", default="", required=False)
     cowtent = RichText(
-        title=u"Text",
+        title="Text",
         default_mime_type="text/html",
         output_mime_type="text/html",
         allowed_mime_types=("text/html", "scroll/dead-sea"),
-        default=u"",
+        default="",
         required=False,
     )
 
 
 @interface.implementer(ITestObjectB)
-class TestObjectB(object):
+class TestObjectB:
     title = schema.fieldproperty.FieldProperty(ITestObjectB["title"])
     cowtent = schema.fieldproperty.FieldProperty(ITestObjectB["cowtent"])
 
 
 registerFactoryAdapter(ITestObjectB, TestObjectB)
 
 
@@ -65,68 +64,68 @@
             ] = "transmogrify.dexterity.tests.testconverters_object.TestObjectB"  # noqa
         return des(_input, None, None)
 
     def test_failures(self):
         desA = IDeserializer(schema.Object(schema=ITestObjectA))
 
         # Have to provide something
-        with self.assertRaisesRegexp(ValueError, "dict"):
+        with self.assertRaisesRegex(ValueError, "dict"):
             desA(None, None, None)
 
         # Dict needs to provide class
-        with self.assertRaisesRegexp(ValueError, "_class"):
+        with self.assertRaisesRegex(ValueError, "_class"):
             desA(dict(), None, None)
 
         # _class needs to implement ITestObjectA
-        with self.assertRaisesRegexp(ValueError, "TestObjectDeserializer"):
+        with self.assertRaisesRegex(ValueError, "TestObjectDeserializer"):
             desA(
                 dict(
                     _class="transmogrify.dexterity.tests.testconverters_object.TestObjectDeserializer"
                 ),
                 None,
                 None,
             )  # noqa
 
         # Extra values not allowed
-        with self.assertRaisesRegexp(ValueError, "fart"):
-            self.deserialize(desA, dict(fish=u"moo", fart="yes"))
+        with self.assertRaisesRegex(ValueError, "fart"):
+            self.deserialize(desA, dict(fish="moo", fart="yes"))
 
     def test_deserialise(self):
         desA = IDeserializer(schema.Object(schema=ITestObjectA))
         desB = IDeserializer(schema.Object(schema=ITestObjectB))
 
-        obj = self.deserialize(desA, dict(fish=u"moo"))
+        obj = self.deserialize(desA, dict(fish="moo"))
         self.assertEqual(obj.__class__, TestObjectA)
-        self.assertEqual(obj.fish, u"moo")
+        self.assertEqual(obj.fish, "moo")
 
         # We recurseivly deserialize
         obj = self.deserialize(
             desB,
             dict(
-                title=u"A nice section",
-                cowtent=dict(data=u"Some nice text", contenttype="scroll/dead-sea"),
+                title="A nice section",
+                cowtent=dict(data="Some nice text", contenttype="scroll/dead-sea"),
             ),
         )
         self.assertEqual(obj.__class__, TestObjectB)
-        self.assertEqual(obj.title, u"A nice section")
+        self.assertEqual(obj.title, "A nice section")
         self.assertEqual(obj.cowtent.__class__, RichTextValue)
-        self.assertEqual(obj.cowtent.raw, u"Some nice text")
+        self.assertEqual(obj.cowtent.raw, "Some nice text")
         self.assertEqual(obj.cowtent.mimeType, "scroll/dead-sea")
 
         # Missing values are okay
         obj = self.deserialize(
             desB,
             dict(
-                title=u"Another section",
+                title="Another section",
             ),
         )
         self.assertEqual(obj.__class__, TestObjectB)
-        self.assertEqual(obj.title, u"Another section")
+        self.assertEqual(obj.title, "Another section")
         self.assertEqual(obj.cowtent.__class__, RichTextValue)
-        self.assertEqual(obj.cowtent.raw, u"")
+        self.assertEqual(obj.cowtent.raw, "")
         self.assertEqual(obj.cowtent.mimeType, "text/html")
 
 
 class TestObjectSerializer(unittest.TestCase):
     def setUp(self):
         # TODO: Should be importing ZCML
         from transmogrify.dexterity import converters
@@ -140,39 +139,39 @@
 
     def test_serialize(self):
         desB = IDeserializer(schema.Object(schema=ITestObjectB))
         serA = ISerializer(schema.Object(schema=ITestObjectA))
         serB = ISerializer(schema.Object(schema=ITestObjectB))
 
         obj = TestObjectA()
-        obj.fish = u"haddock"
+        obj.fish = "haddock"
         self.assertEqual(
             serA(obj, None),
             dict(
                 _class="transmogrify.dexterity.tests.testconverters_object.TestObjectA",  # noqa
-                fish=u"haddock",
+                fish="haddock",
             ),
         )
 
         # Recurse into attributes
         filestore = {}
         obj = desB(
             dict(
-                title=u"A hairy section",
-                cowtent=dict(data=u"Some nice text", contenttype="scroll/dead-sea"),
+                title="A hairy section",
+                cowtent=dict(data="Some nice text", contenttype="scroll/dead-sea"),
                 _class="transmogrify.dexterity.tests.testconverters_object.TestObjectB",  # noqa
             ),
             filestore,
             None,
         )
         self.assertEqual(
             serB(obj, filestore),
             dict(
                 _class="transmogrify.dexterity.tests.testconverters_object.TestObjectB",  # noqa
-                title=u"A hairy section",
+                title="A hairy section",
                 cowtent=dict(
                     file="_field_cowtent_cowtent",
                     encoding="utf-8",
                     contenttype="scroll/dead-sea",
                 ),
             ),
         )
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/tests/tests.zcml` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/tests/tests.zcml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:transmogrifier="http://namespaces.plone.org/transmogrifier"
-  i18n_domain="transmogrify.dexterity">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:transmogrifier="http://namespaces.plone.org/transmogrifier"
+    i18n_domain="transmogrify.dexterity"
+    >
 
   <include package="collective.transmogrifier" />
   <include package="plone.app.dexterity" />
   <include package="transmogrify.dexterity" />
   <include package="plone.app.intid" />
 
   <transmogrifier:registerConfig
       name="transmogrify.dexterity.testconfiguration"
       title="Example pipeline configuration"
       description="This is an example pipeline configuration"
-      configuration="tests.cfg" />
+      configuration="tests.cfg"
+      />
 
 </configure>
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify/dexterity/translation.py` & `transmogrify.dexterity-3.0.0/src/transmogrify/dexterity/translation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-# -*- coding: utf-8 -*-
 from collective.transmogrifier.interfaces import ISection
 from collective.transmogrifier.interfaces import ISectionBlueprint
 from collective.transmogrifier.utils import defaultMatcher
+from plone.app.multilingual.interfaces import IMutableTG
 from plone.dexterity.interfaces import IDexterityContent
+from Products.CMFPlone.interfaces import ILanguage
 from zope.component.hooks import getSite
 from zope.interface import implementer
 from zope.interface import provider
 
 
-try:
-    from plone.app.multilingual.interfaces import ILanguage
-    from plone.app.multilingual.interfaces import IMutableTG
-
-    PAM_AVAILABLE = True
-except ImportError:
-    PAM_AVAILABLE = False
-
-
 @provider(ISectionBlueprint)
 @implementer(ISection)
-class DexterityTranslationSection(object):
+class DexterityTranslationSection:
     def __init__(self, transmogrifier, name, options, previous):
-        if not PAM_AVAILABLE:
-            raise RuntimeError("``plone.app.multilingual`` not installed")
         self.previous = previous
         self.context = (
             transmogrifier.context if transmogrifier.context else getSite()
         )  # noqa
         self.name = name
         self.pathkey = defaultMatcher(options, "path-key", name, "path")
         self.langkey = options.get("lang-key", "_lang").strip()
```

### Comparing `transmogrify.dexterity-2.0.0/src/transmogrify.dexterity.egg-info/SOURCES.txt` & `transmogrify.dexterity-3.0.0/src/transmogrify.dexterity.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-CHANGES.rst
-CONTRIBUTORS.rst
-DEVELOP.rst
-LICENSE.rst
+CHANGES.md
+CONTRIBUTORS.md
+LICENSE.GPL
 MANIFEST.in
-README.rst
-setup.cfg
+README.md
+pyproject.toml
 setup.py
 docs/conf.py
 docs/index.rst
+examples/export.cfg
+examples/import.cfg
 src/transmogrify/__init__.py
 src/transmogrify.dexterity.egg-info/PKG-INFO
 src/transmogrify.dexterity.egg-info/SOURCES.txt
 src/transmogrify.dexterity.egg-info/dependency_links.txt
 src/transmogrify.dexterity.egg-info/entry_points.txt
 src/transmogrify.dexterity.egg-info/namespace_packages.txt
 src/transmogrify.dexterity.egg-info/not-zip-safe
```


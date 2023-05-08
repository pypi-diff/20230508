# Comparing `tmp/pyatlan-0.0.26.tar.gz` & `tmp/pyatlan-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.26.tar", last modified: Thu May  4 15:48:25 2023, max compression
+gzip compressed data, was "pyatlan-0.0.27.tar", last modified: Mon May  8 16:54:22 2023, max compression
```

## Comparing `pyatlan-0.0.26.tar` & `pyatlan-0.0.27.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.281848 pyatlan-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-04 15:48:12.000000 pyatlan-0.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 15:48:12.000000 pyatlan-0.0.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-04 15:48:12.000000 pyatlan-0.0.26/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 15:48:25.281848 pyatlan-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-04 15:48:12.000000 pyatlan-0.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.273848 pyatlan-0.0.26/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.273848 pyatlan-0.0.26/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   866175 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.273848 pyatlan-0.0.26/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:48:25.281848 pyatlan-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 15:48:12.000000 pyatlan-0.0.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.281848 pyatlan-0.0.26/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.281848 pyatlan-0.0.26/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    51397 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.193591 pyatlan-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-08 16:54:11.000000 pyatlan-0.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 16:54:11.000000 pyatlan-0.0.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 16:54:11.000000 pyatlan-0.0.27/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-08 16:54:22.193591 pyatlan-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-08 16:54:11.000000 pyatlan-0.0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.189591 pyatlan-0.0.27/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.189591 pyatlan-0.0.27/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.189591 pyatlan-0.0.27/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.189591 pyatlan-0.0.27/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.189591 pyatlan-0.0.27/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.189591 pyatlan-0.0.27/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   869422 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 16:54:11.000000 pyatlan-0.0.27/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.189591 pyatlan-0.0.27/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-08 16:54:22.000000 pyatlan-0.0.27/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-08 16:54:22.000000 pyatlan-0.0.27/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:54:22.000000 pyatlan-0.0.27/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:54:22.000000 pyatlan-0.0.27/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 16:54:22.000000 pyatlan-0.0.27/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 16:54:22.000000 pyatlan-0.0.27/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:54:22.193591 pyatlan-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-08 16:54:11.000000 pyatlan-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.193591 pyatlan-0.0.27/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.193591 pyatlan-0.0.27/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33620 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:54:22.193591 pyatlan-0.0.27/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 16:54:11.000000 pyatlan-0.0.27/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.26/LICENSE` & `pyatlan-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/PKG-INFO` & `pyatlan-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.26
+Version: 0.0.27
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.26/README.md` & `pyatlan-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.27/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.27/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/cache/role_cache.py` & `pyatlan-0.0.27/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/client/atlan.py` & `pyatlan-0.0.27/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/client/constants.py` & `pyatlan-0.0.27/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/error.py` & `pyatlan-0.0.27/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/exceptions.py` & `pyatlan-0.0.27/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.27/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/model/assets.py` & `pyatlan-0.0.27/pyatlan/model/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
 from __future__ import annotations
 
+import hashlib
 import sys
 from datetime import datetime
+from io import StringIO
 from typing import Any, ClassVar, Dict, List, Optional, TypeVar
 from urllib.parse import quote, unquote
 
 from pydantic import Field, StrictStr, root_validator, validator
 
 from pyatlan.model.core import (
     Announcement,
@@ -75,14 +77,16 @@
 
 def validate_required_fields(field_names: list[str], values: list[Any]):
     for field_name, value in zip(field_names, values):
         if value is None:
             raise ValueError(f"{field_name} is required")
         if isinstance(value, str) and not value.strip():
             raise ValueError(f"{field_name} cannot be blank")
+        if isinstance(value, list) and len(value) == 0:
+            raise ValueError(f"{field_name} cannot be an empty list")
 
 
 SelfAsset = TypeVar("SelfAsset", bound="Asset")
 
 
 class Referenceable(AtlanObject):
     """Description"""
@@ -3077,20 +3081,105 @@
         column_processes: Optional[list[ColumnProcess]] = Field(
             None, description="", alias="columnProcesses"
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
 
+        @staticmethod
+        def generate_qualified_name(
+            name: str,
+            connection_qualified_name: str,
+            inputs: list["Catalog"],
+            outputs: list["Catalog"],
+            parent: Optional["Process"] = None,
+            process_id: Optional[str] = None,
+        ) -> str:
+            def append_relationship(output: StringIO, relationship: Asset):
+                if relationship.guid:
+                    output.write(relationship.guid)
+
+            def append_relationships(output: StringIO, relationships: list["Catalog"]):
+                for catalog in relationships:
+                    append_relationship(output, catalog)
+
+            validate_required_fields(
+                ["name", "connection_qualified_name", "inputs", "outputs"],
+                [name, connection_qualified_name, inputs, outputs],
+            )
+            if process_id and process_id.strip():
+                return f"{connection_qualified_name}/{process_id}"
+            buffer = StringIO()
+            buffer.write(name)
+            buffer.write(connection_qualified_name)
+            if parent:
+                append_relationship(buffer, parent)
+            append_relationships(buffer, inputs)
+            append_relationships(buffer, outputs)
+            ret_value = hashlib.md5(
+                buffer.getvalue().encode(), usedforsecurity=False
+            ).hexdigest()
+            buffer.close()
+            return ret_value
+
+        @classmethod
+        def create(
+            cls,
+            name: str,
+            connection_qualified_name: str,
+            inputs: list["Catalog"],
+            outputs: list["Catalog"],
+            process_id: Optional[str] = None,
+            parent: Optional[Process] = None,
+        ) -> Process.Attributes:
+            qualified_name = Process.Attributes.generate_qualified_name(
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                process_id=process_id,
+                inputs=inputs,
+                outputs=outputs,
+                parent=parent,
+            )
+            connector_name = connection_qualified_name.split("/")[1]
+            return Process.Attributes(
+                name=name,
+                qualified_name=qualified_name,
+                connector_name=connector_name,
+                connection_qualified_name=connection_qualified_name,
+                inputs=inputs,
+                outputs=outputs,
+            )
+
     attributes: "Process.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @classmethod
+    def create(
+        cls,
+        name: str,
+        connection_qualified_name: str,
+        inputs: list["Catalog"],
+        outputs: list["Catalog"],
+        process_id: Optional[str] = None,
+        parent: Optional[Process] = None,
+    ) -> Process:
+        return Process(
+            attributes=Process.Attributes.create(
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                process_id=process_id,
+                inputs=inputs,
+                outputs=outputs,
+                parent=parent,
+            )
+        )
+
 
 class AtlasGlossaryCategory(Asset, type_name="AtlasGlossaryCategory"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in AtlasGlossaryCategory._convience_properties:
             return object.__setattr__(self, name, value)
```

### Comparing `pyatlan-0.0.26/pyatlan/model/core.py` & `pyatlan-0.0.27/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/model/enums.py` & `pyatlan-0.0.27/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/model/response.py` & `pyatlan-0.0.27/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/model/role.py` & `pyatlan-0.0.27/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/model/search.py` & `pyatlan-0.0.27/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/model/structs.py` & `pyatlan-0.0.27/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/model/typedef.py` & `pyatlan-0.0.27/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan/utils.py` & `pyatlan-0.0.27/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.27/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.26
+Version: 0.0.27
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.26/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.27/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/setup.py` & `pyatlan-0.0.27/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/integration/classification_test.py` & `pyatlan-0.0.27/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.27/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/integration/role_test.py` & `pyatlan-0.0.27/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/integration/test_client.py` & `pyatlan-0.0.27/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/integration/test_entity_model.py` & `pyatlan-0.0.27/tests/integration/test_entity_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import os
 import random
 import string
+from typing import Callable, Generator
 
 import pytest
 import requests
 
 from pyatlan.cache.role_cache import RoleCache
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.error import NotFoundError
@@ -14,15 +15,17 @@
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     Column,
     Connection,
     Database,
+    Process,
     Readme,
+    S3Object,
     Schema,
     Table,
     View,
 )
 from pyatlan.model.core import Announcement
 from pyatlan.model.enums import AnnouncementType, AtlanConnectorType, CertificateStatus
 
@@ -39,14 +42,15 @@
     "34d8106a-1478-4816-bfe1-97814ffff78e",
     "04a4eca5-b7d5-4659-bbad-1dc2306ea9c3",
     "619daa76-ab3c-4f29-836a-6ec0ddefbe0c",
     "4af8d57c-61ef-4b57-983c-eff20e6d08b5",
     "57f5463d-cc2a-4859-bf28-e4fa52002e8e",
 }
 TEMP_CONNECTION_GUID = "b3a5c49a-0c7c-4e66-8453-f4da8d9ce222"
+S3_CONNECTION_GUID = "25f2dc21-cd53-47fe-bbed-be10759d087a"
 
 
 @pytest.fixture(scope="module")
 def client() -> AtlanClient:
     return AtlanClient()
 
 
@@ -185,14 +189,15 @@
         "AtlasGlossary",
         "Table",
         "Schema",
         "Database",
         "Connection",
         "View",
         "Column",
+        "Process",
         "Readme",
     ]
     for type_name in type_names:
         print()
         delete_assets(atlan_host, headers, type_name)
     yield
     for type_name in type_names:
@@ -821,7 +826,52 @@
     glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
     readme = Readme.create(asset=glossary, content="<h1>Important</h1>")
     response = client.upsert(readme)
     assert (reaadmes := response.assets_created(asset_type=Readme))
     assert len(reaadmes) == 1
     assert (glossaries := response.assets_updated(asset_type=AtlasGlossary))
     assert len(glossaries) == 1
+
+
+@pytest.fixture()
+def make_s3_object(
+    client: AtlanClient,
+) -> Generator[Callable[[str], S3Object], None, None]:
+    created_guids = []
+    connection = client.get_asset_by_guid(S3_CONNECTION_GUID, Connection)
+
+    def _make_s3_object(name: str) -> S3Object:
+        s3_object = S3Object.create(
+            connection_qualified_name=connection.qualified_name,
+            name=name,
+            aws_arn=f"arn:aws:s3:::{name}",
+        )
+        s3_object = client.upsert(s3_object).assets_created(S3Object)[0]
+        created_guids.append(s3_object.guid)
+        return s3_object
+
+    yield _make_s3_object
+
+    for guid in created_guids:
+        client.purge_entity_by_guid(guid=guid)
+
+
+def test_process_create(client: AtlanClient, make_s3_object: Callable[[str], S3Object]):
+    connection = client.get_asset_by_guid(S3_CONNECTION_GUID, Connection)
+
+    input_object = make_s3_object("Integration Source")
+
+    output_object = make_s3_object("Integration Target")
+
+    process = Process.create(
+        name="Integration Process Test",
+        connection_qualified_name=connection.qualified_name,
+        process_id="doit",
+        inputs=[input_object],
+        outputs=[output_object],
+    )
+
+    response = client.upsert(process)
+    assert (processes := response.assets_created(Process))
+    assert len(processes) == 1
+    assert (assets := response.assets_updated(S3Object))
+    assert len(assets) == 2
```

### Comparing `pyatlan-0.0.26/tests/integration/test_index_search.py` & `pyatlan-0.0.27/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/unit/test_classification_name.py` & `pyatlan-0.0.27/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/unit/test_client.py` & `pyatlan-0.0.27/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/unit/test_glossary_term.py` & `pyatlan-0.0.27/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/unit/test_model.py` & `pyatlan-0.0.27/tests/unit/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import json
 from datetime import datetime
+from hashlib import md5
 from inspect import signature
 from pathlib import Path
 from unittest.mock import create_autospec, patch
 
 import pytest
 from deepdiff import DeepDiff
 from pydantic.error_wrappers import ValidationError
@@ -20,22 +21,24 @@
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     AtlasServer,
     AwsTag,
     AzureTag,
     BadgeCondition,
+    Catalog,
     ColumnValueFrequencyMap,
     Connection,
     Database,
     DbtMetricFilter,
     GoogleLabel,
     GoogleTag,
     Histogram,
     PopularityInsights,
+    Process,
     Readme,
     S3Bucket,
     S3Object,
     Schema,
     Table,
     View,
     validate_single_required_field,
@@ -1449,7 +1452,211 @@
 )
 def test_create_readme(asset, content, asset_name, expected_name):
     readme = Readme.create(asset=asset, content=content, asset_name=asset_name)
     assert readme.qualified_name == f"{asset.guid}/readme"
     assert readme.name == f"{expected_name} Readme"
     assert readme.attributes.asset == asset
     assert readme.description == content
+
+
+@pytest.mark.parametrize(
+    "name, connection_qualified_name, process_id, inputs,outputs, parent, message",
+    [
+        (None, "133/s3", None, [Catalog()], [Catalog()], None, "name is required"),
+        (
+            "bob",
+            None,
+            None,
+            [Catalog()],
+            [Catalog()],
+            None,
+            "connection_qualified_name is required",
+        ),
+        ("bob", "133/s3", None, None, [Catalog()], None, "inputs is required"),
+        (
+            "bob",
+            "133/s3",
+            None,
+            [],
+            [Catalog()],
+            None,
+            "inputs cannot be an empty list",
+        ),
+        ("bob", "133/s3", None, [Catalog()], None, None, "outputs is required"),
+        (
+            "bob",
+            "133/s3",
+            None,
+            [Catalog()],
+            [],
+            None,
+            "outputs cannot be an empty list",
+        ),
+    ],
+)
+def test_process_attributes_generate_qualified_name_without_required_parameter_raises_value_error(
+    name, connection_qualified_name, process_id, inputs, outputs, parent, message
+):
+    with pytest.raises(ValueError, match=message):
+        Process.Attributes.generate_qualified_name(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            process_id=process_id,
+            inputs=inputs,
+            outputs=outputs,
+            parent=parent,
+        )
+
+
+@pytest.mark.parametrize(
+    "name, connection_qualified_name, process_id, inputs,outputs, parent, expected_value",
+    [
+        (
+            "doit",
+            "default/s3/1678379436102",
+            "123",
+            [Catalog()],
+            [Catalog()],
+            None,
+            "default/s3/1678379436102/123",
+        ),
+        (
+            "doit",
+            "default/s3/1678379436102",
+            None,
+            [Catalog(guid="123")],
+            [Catalog(guid="456")],
+            None,
+            "doitdefault/s3/1678379436102123456",
+        ),
+        (
+            "doit",
+            "default/s3/1678379436102",
+            None,
+            [Catalog(guid="456")],
+            [Catalog(guid="789")],
+            Catalog(guid="123"),
+            "doitdefault/s3/1678379436102123456789",
+        ),
+    ],
+)
+def test_process_attributes_generate_qualified_name(
+    name, connection_qualified_name, process_id, inputs, outputs, parent, expected_value
+):
+    if not process_id:
+        expected_value = md5(expected_value.encode()).hexdigest()
+
+    assert (
+        Process.Attributes.generate_qualified_name(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            process_id=process_id,
+            inputs=inputs,
+            outputs=outputs,
+            parent=parent,
+        )
+        == expected_value
+    )
+
+
+@pytest.mark.parametrize(
+    "name, connection_qualified_name, process_id, inputs,outputs, parent, message",
+    [
+        (None, "133/s3", None, [Catalog()], [Catalog()], None, "name is required"),
+        (
+            "bob",
+            None,
+            None,
+            [Catalog()],
+            [Catalog()],
+            None,
+            "connection_qualified_name is required",
+        ),
+        ("bob", "133/s3", None, None, [Catalog()], None, "inputs is required"),
+        (
+            "bob",
+            "133/s3",
+            None,
+            [],
+            [Catalog()],
+            None,
+            "inputs cannot be an empty list",
+        ),
+        ("bob", "133/s3", None, [Catalog()], None, None, "outputs is required"),
+        (
+            "bob",
+            "133/s3",
+            None,
+            [Catalog()],
+            [],
+            None,
+            "outputs cannot be an empty list",
+        ),
+    ],
+)
+def test_process_attributes_create_without_required_parameter_raises_value_error(
+    name, connection_qualified_name, process_id, inputs, outputs, parent, message
+):
+    with pytest.raises(ValueError, match=message):
+        Process.Attributes.create(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            process_id=process_id,
+            inputs=inputs,
+            outputs=outputs,
+            parent=parent,
+        )
+
+
+@pytest.mark.parametrize(
+    "name, connection_qualified_name, process_id, inputs,outputs, parent, expected_value",
+    [
+        (
+            "doit",
+            "default/s3/1678379436102",
+            "123",
+            [Catalog()],
+            [Catalog()],
+            None,
+            "default/s3/1678379436102/123",
+        ),
+        (
+            "doit",
+            "default/s3/1678379436102",
+            None,
+            [Catalog(guid="123")],
+            [Catalog(guid="456")],
+            None,
+            "doitdefault/s3/1678379436102123456",
+        ),
+        (
+            "doit",
+            "default/s3/1678379436102",
+            None,
+            [Catalog(guid="456")],
+            [Catalog(guid="789")],
+            Catalog(guid="123"),
+            "doitdefault/s3/1678379436102123456789",
+        ),
+    ],
+)
+def test_process_attributes_create(
+    name, connection_qualified_name, process_id, inputs, outputs, parent, expected_value
+):
+    if not process_id:
+        expected_value = md5(expected_value.encode()).hexdigest()
+
+    process = Process.create(
+        name=name,
+        connection_qualified_name=connection_qualified_name,
+        process_id=process_id,
+        inputs=inputs,
+        outputs=outputs,
+        parent=parent,
+    )
+
+    assert process.name == name
+    assert process.connection_qualified_name == connection_qualified_name
+    assert process.qualified_name == expected_value
+    assert process_id == process_id
+    assert process.inputs == inputs
+    assert process.outputs == outputs
```

### Comparing `pyatlan-0.0.26/tests/unit/test_search_model.py` & `pyatlan-0.0.27/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.26/tests/unit/test_typedef_model.py` & `pyatlan-0.0.27/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*


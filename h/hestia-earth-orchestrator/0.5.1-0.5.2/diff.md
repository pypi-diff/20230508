# Comparing `tmp/hestia-earth-orchestrator-0.5.1.tar.gz` & `tmp/hestia-earth-orchestrator-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-orchestrator-0.5.1.tar", last modified: Fri Mar 17 08:32:46 2023, max compression
+gzip compressed data, was "hestia-earth-orchestrator-0.5.2.tar", last modified: Mon May  8 14:42:41 2023, max compression
```

## Comparing `hestia-earth-orchestrator-0.5.1.tar` & `hestia-earth-orchestrator-0.5.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.747064 hestia-earth-orchestrator-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2380 2023-03-17 08:32:46.747064 hestia-earth-orchestrator-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.736063 hestia-earth-orchestrator-0.5.1/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.736980 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.736980 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/config/
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.738813 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.738813 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/emissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/emissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/emissions/deleted.py
--rw-rw-rw-   0 root         (0) root         (0)     4427 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.739730 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.740647 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/
--rw-rw-rw-   0 root         (0) root         (0)     1416 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/merge_append.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/merge_default.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/merge_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2659 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/merge_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.741564 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/run/
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2875 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/run/add_key_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/run/always.py
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.743397 hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2380 2023-03-17 08:32:46.000000 hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-03-17 08:32:46.000000 hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 08:32:46.000000 hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-17 08:32:46.000000 hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-17 08:32:46.000000 hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-17 08:32:46.747064 hestia-earth-orchestrator-0.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.734230 hestia-earth-orchestrator-0.5.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.743397 hestia-earth-orchestrator-0.5.1/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.744314 hestia-earth-orchestrator-0.5.1/tests/models/emissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/models/emissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/models/emissions/test_deleted.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/models/test_transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.744314 hestia-earth-orchestrator-0.5.1/tests/strategies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.746147 hestia-earth-orchestrator-0.5.1/tests/strategies/merge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/merge/test_merge_append.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/merge/test_merge_default.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/merge/test_merge_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3207 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/merge/test_merge_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:32:46.747064 hestia-earth-orchestrator-0.5.1/tests/strategies/run/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3236 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/run/test_add_blank_node_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/run/test_add_key_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-17 08:32:31.000000 hestia-earth-orchestrator-0.5.1/tests/strategies/run/test_always.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.733764 hestia-earth-orchestrator-0.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-05-08 14:42:41.733764 hestia-earth-orchestrator-0.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.720761 hestia-earth-orchestrator-0.5.2/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.722762 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.722762 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/config/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.723762 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.723762 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/emissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/emissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/emissions/deleted.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.723762 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.725762 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/merge_append.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/merge_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/merge_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/merge_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.726762 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/run/
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/run/add_key_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/run/always.py
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.728763 hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-05-08 14:42:41.000000 hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-08 14:42:41.000000 hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 14:42:41.000000 hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-08 14:42:41.000000 hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-08 14:42:41.000000 hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 14:42:41.733764 hestia-earth-orchestrator-0.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.718761 hestia-earth-orchestrator-0.5.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.729763 hestia-earth-orchestrator-0.5.2/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.729763 hestia-earth-orchestrator-0.5.2/tests/models/emissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/models/emissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/models/emissions/test_deleted.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/models/test_transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.730763 hestia-earth-orchestrator-0.5.2/tests/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.731763 hestia-earth-orchestrator-0.5.2/tests/strategies/merge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/merge/test_merge_append.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/merge/test_merge_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/merge/test_merge_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/merge/test_merge_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:42:41.732763 hestia-earth-orchestrator-0.5.2/tests/strategies/run/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/run/test_add_blank_node_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/run/test_add_key_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-08 14:42:25.000000 hestia-earth-orchestrator-0.5.2/tests/strategies/run/test_always.py
```

### Comparing `hestia-earth-orchestrator-0.5.1/LICENSE` & `hestia-earth-orchestrator-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/PKG-INFO` & `hestia-earth-orchestrator-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-orchestrator
-Version: 0.5.1
+Version: 0.5.2
 Summary: Hestia's module to orchestrate the models.
 Home-page: https://gitlab.com/hestia-earth/hestia-engine-orchestrator
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-orchestrator-0.5.1/README.md` & `hestia-earth-orchestrator-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/__init__.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/log.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/__init__.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/emissions/deleted.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/emissions/deleted.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/models/transformations.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/models/transformations.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,23 +22,28 @@
     term_type = term.get('termType')
     term_id = term.get('@id')
     lookup = download_lookup(f"{term_type}.csv")
     value = get_table_value(lookup, 'termid', term_id, column_name('includeForTransformation'))
     return False if value is None or value == '' or not value else True
 
 
-def _convert_transformation(cycle: dict, transformation: dict):
+def _copy_from_cycle(cycle: dict, transformation: dict, keys: list):
     data = deepcopy(transformation)
-    # copy data from previous transformation
+    for key in keys:
+        data[key] = transformation.get(key.replace('cycle', 'transformation')) or \
+            transformation.get(key) or \
+            cycle.get(key)
+    return data
+
+
+def _convert_transformation(cycle: dict, transformation: dict):
+    data = _copy_from_cycle(cycle, transformation, [
+        'functionalUnit', 'site', 'otherSites', 'cycleDuration', 'startDate', 'endDate'
+    ])
     data['completeness'] = _full_completeness()
-    data['functionalUnit'] = cycle.get('functionalUnit')
-    data['site'] = cycle.get('site')
-    data['cycleDuration'] = transformation.get('transformationDuration', cycle.get('cycleDuration'))
-    data['startDate'] = transformation.get('startDate', cycle.get('startDate'))
-    data['endDate'] = transformation.get('endDate', cycle.get('endDate'))
     data['practices'] = [
         _new_practice(transformation.get('term'))  # add `term` as a Practice
     ] + transformation.get('practices', []) + [
         p for p in cycle.get('practices', []) if _include_practice(p)  # some practices need to be copied over
     ]
     return data
```

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/__init__.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/merge_append.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/merge_append.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/merge_list.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/merge_list.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/merge/merge_node.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/merge/merge_node.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth/orchestrator/utils.py` & `hestia-earth-orchestrator-0.5.2/hestia_earth/orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/PKG-INFO` & `hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-orchestrator
-Version: 0.5.1
+Version: 0.5.2
 Summary: Hestia's module to orchestrate the models.
 Home-page: https://gitlab.com/hestia-earth/hestia-engine-orchestrator
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-orchestrator-0.5.1/hestia_earth_orchestrator.egg-info/SOURCES.txt` & `hestia-earth-orchestrator-0.5.2/hestia_earth_orchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/setup.py` & `hestia-earth-orchestrator-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/tests/models/emissions/test_deleted.py` & `hestia-earth-orchestrator-0.5.2/tests/models/emissions/test_deleted.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/tests/models/test_transformations.py` & `hestia-earth-orchestrator-0.5.2/tests/models/test_transformations.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/tests/strategies/merge/test_merge_append.py` & `hestia-earth-orchestrator-0.5.2/tests/strategies/merge/test_merge_append.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/tests/strategies/merge/test_merge_list.py` & `hestia-earth-orchestrator-0.5.2/tests/strategies/merge/test_merge_list.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/tests/strategies/merge/test_merge_node.py` & `hestia-earth-orchestrator-0.5.2/tests/strategies/merge/test_merge_node.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.1/tests/strategies/run/test_add_blank_node_if_missing.py` & `hestia-earth-orchestrator-0.5.2/tests/strategies/run/test_add_blank_node_if_missing.py`

 * *Files identical despite different names*


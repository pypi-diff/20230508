# Comparing `tmp/SeisMonitor-0.0.8.tar.gz` & `tmp/SeisMonitor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeisMonitor-0.0.8.tar", last modified: Tue Nov 15 12:06:32 2022, max compression
+gzip compressed data, was "SeisMonitor-0.0.9.tar", last modified: Tue Jan 17 00:23:31 2023, max compression
```

## Comparing `SeisMonitor-0.0.8.tar` & `SeisMonitor-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.659468 SeisMonitor-0.0.8/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1071 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/LICENSE
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      782 2022-11-15 12:06:32.659468 SeisMonitor-0.0.8/PKG-INFO
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.651468 SeisMonitor-0.0.8/SeisMonitor/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/__init__.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.651468 SeisMonitor-0.0.8/SeisMonitor/core/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/core/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     6337 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/core/client.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     4350 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/core/objects.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    10616 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/core/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.651468 SeisMonitor-0.0.8/SeisMonitor/monitor/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/__init__.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.651468 SeisMonitor-0.0.8/SeisMonitor/monitor/associator/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/associator/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    13959 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/associator/ai.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    12299 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/associator/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.655468 SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      583 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/bmnh.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    11412 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/obspy_mdl.py
--rwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)    12831 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/seismonitor copy.py
--rwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)     9262 2022-11-15 02:04:56.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/seismonitor.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    23588 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.655468 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/__init__.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.655468 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypoDD/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypoDD/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     2147 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypoDD/core.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    22079 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypoDD/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.655468 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypocenter/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypocenter/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1435 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypocenter/core.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    16556 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypocenter/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.655468 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    18627 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/_utils.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    13815 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/nlloc.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    15600 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/utils.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     6853 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/locator/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.655468 SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    28609 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/_magnitude.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    21022 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/mag.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      136 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/t.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    13748 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.659468 SeisMonitor-0.0.8/SeisMonitor/monitor/picker/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/picker/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    11190 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/picker/ai.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    27357 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/picker/utils.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1498 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/picker/x.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    12363 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/monitor/seismonitor.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.659468 SeisMonitor-0.0.8/SeisMonitor/plot/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/plot/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        2 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/plot/associator.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     4313 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/plot/picks copy.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     3704 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/plot/picks.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    15443 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/SeisMonitor/plot/utils.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     2811 2022-11-15 12:05:41.000000 SeisMonitor-0.0.8/SeisMonitor/utils.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.651468 SeisMonitor-0.0.8/SeisMonitor.egg-info/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      782 2022-11-15 12:06:32.000000 SeisMonitor-0.0.8/SeisMonitor.egg-info/PKG-INFO
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1850 2022-11-15 12:06:32.000000 SeisMonitor-0.0.8/SeisMonitor.egg-info/SOURCES.txt
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        1 2022-11-15 12:06:32.000000 SeisMonitor-0.0.8/SeisMonitor.egg-info/dependency_links.txt
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)       53 2022-11-15 12:06:32.000000 SeisMonitor-0.0.8/SeisMonitor.egg-info/requires.txt
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)       17 2022-11-15 12:06:32.000000 SeisMonitor-0.0.8/SeisMonitor.egg-info/top_level.txt
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.659468 SeisMonitor-0.0.8/data/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/data/__init__.py
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)       38 2022-11-15 12:06:32.659468 SeisMonitor-0.0.8/setup.cfg
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1617 2022-11-15 12:06:04.000000 SeisMonitor-0.0.8/setup.py
-drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-15 12:06:32.659468 SeisMonitor-0.0.8/test/
--rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     4675 2022-11-09 03:05:20.000000 SeisMonitor-0.0.8/test/test_seismonitor.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1071 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/LICENSE
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      782 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/PKG-INFO
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.852852 SeisMonitor-0.0.9/SeisMonitor/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/__init__.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/core/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/core/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     6337 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/core/client.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     4350 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/core/objects.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    10616 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/core/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/__init__.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/associator/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/associator/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    13959 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/associator/ai.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    12299 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/associator/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      583 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/bmnh.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    11412 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/obspy_mdl.py
+-rwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)    12831 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/seismonitor copy.py
+-rwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)     9262 2022-11-15 02:04:56.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/seismonitor.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    23584 2022-11-24 12:11:58.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/__init__.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypoDD/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypoDD/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     2147 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypoDD/core.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    22079 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypoDD/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypocenter/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypocenter/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1435 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypocenter/core.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    16556 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypocenter/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    18627 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/_utils.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    13815 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/nlloc.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    15600 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/utils.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     6853 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/locator/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    28609 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/_magnitude.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    21024 2022-12-14 11:40:58.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/mag.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      136 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/t.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    13748 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/monitor/picker/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/picker/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    11190 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/picker/ai.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    27357 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/picker/utils.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1498 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/picker/x.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    12369 2022-12-14 13:49:20.000000 SeisMonitor-0.0.9/SeisMonitor/monitor/seismonitor.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/SeisMonitor/plot/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/plot/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        2 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/plot/associator.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     4313 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/plot/picks copy.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     3704 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/plot/picks.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)    15443 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/SeisMonitor/plot/utils.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     2811 2022-11-15 12:05:41.000000 SeisMonitor-0.0.9/SeisMonitor/utils.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.852852 SeisMonitor-0.0.9/SeisMonitor.egg-info/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)      782 2023-01-17 00:23:31.000000 SeisMonitor-0.0.9/SeisMonitor.egg-info/PKG-INFO
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1850 2023-01-17 00:23:31.000000 SeisMonitor-0.0.9/SeisMonitor.egg-info/SOURCES.txt
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        1 2023-01-17 00:23:31.000000 SeisMonitor-0.0.9/SeisMonitor.egg-info/dependency_links.txt
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)       53 2023-01-17 00:23:31.000000 SeisMonitor-0.0.9/SeisMonitor.egg-info/requires.txt
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)       17 2023-01-17 00:23:31.000000 SeisMonitor-0.0.9/SeisMonitor.egg-info/top_level.txt
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/data/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)        0 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/data/__init__.py
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)       38 2023-01-17 00:23:31.860851 SeisMonitor-0.0.9/setup.cfg
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     1617 2023-01-17 00:22:56.000000 SeisMonitor-0.0.9/setup.py
+drwxrwxr-x   0 emmanuel  (1000) emmanuel  (1000)        0 2023-01-17 00:23:31.856852 SeisMonitor-0.0.9/test/
+-rw-rw-r--   0 emmanuel  (1000) emmanuel  (1000)     4675 2022-11-09 03:05:20.000000 SeisMonitor-0.0.9/test/test_seismonitor.py
```

### Comparing `SeisMonitor-0.0.8/LICENSE` & `SeisMonitor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/PKG-INFO` & `SeisMonitor-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeisMonitor
-Version: 0.0.8
+Version: 0.0.9
 Summary: To monitor seismic activity
 Home-page: https://github.com/ecastillot/SeisMonitor
 Author: ecastillot (Emmanuel Castillo)
 Author-email: <ecastillot@unal.edu.co>
 License: UNKNOWN
 Keywords: python,seismonitor,earthquakes,seismology
 Platform: UNKNOWN
```

### Comparing `SeisMonitor-0.0.8/SeisMonitor/core/client.py` & `SeisMonitor-0.0.9/SeisMonitor/core/client.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/core/objects.py` & `SeisMonitor-0.0.9/SeisMonitor/core/objects.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/core/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/core/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/associator/ai.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/associator/ai.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/associator/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/associator/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/bmnh.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/bmnh.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/obspy_mdl.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/obspy_mdl.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/seismonitor copy.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/seismonitor copy.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/seismonitor.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/seismonitor.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/downloader/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/downloader/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,16 +170,16 @@
 	channel=tr.stats.channel
 	starttime=tr.stats.starttime 
 	_starttime=starttime.strftime(strftime) 
 	endtime=tr.stats.endtime
 	_endtime=endtime.strftime(strftime)
 	year = starttime.year
 	month = starttime.month
-	day = starttime.day
-	julday = starttime.julday
+	day = endtime.day
+	julday = endtime.julday
 	path = _str.format(
                     network=network, station=station, location=location,
                     channel=channel, year=year, month=month, 
                     day=day, julday=julday,starttime=_starttime,endtime=_endtime)
 	if ppc:
 		path = path + ".ppc"
```

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypoDD/core.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypoDD/core.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypoDD/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypoDD/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypocenter/core.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypocenter/core.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/hypocenter/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/hypocenter/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/_utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/_utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/nlloc.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/nlloc.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/nlloc/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/nlloc/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/locator/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/locator/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/_magnitude.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/_magnitude.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/mag.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/mag.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from obspy.core.event import Catalog
 from obspy.core.event import read_events, Comment
 from SeisMonitor.utils import isfile
 from SeisMonitor.core import utils as scut
 from obspy.core.event.base import CreationInfo
 import concurrent.futures as cf
 from obspy import UTCDateTime
-import mtspec
+# import mtspec
 import numpy as np
 import scipy
 import os
 from SeisMonitor.utils import printlog
 from . import utils as ut
 
 class MwPhysicalMagParams():
```

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/magnitude/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/magnitude/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/picker/ai.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/picker/ai.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/picker/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/picker/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/picker/x.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/picker/x.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/monitor/seismonitor.py` & `SeisMonitor-0.0.9/SeisMonitor/monitor/seismonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,26 +237,26 @@
                         if picker == "EQTransformer":
                             _picker = ai_picker.EQTransformer(picker_args)
                             result = _picker.pick(folders["downloads"],
                                                 folders["metadata"],
                                                 out_path)
                             if result.empty:
                                 print("No picks")
-                                exit()
+                                continue
                             del _picker
                             del result
 
                         elif picker == "PhaseNet":
                             _picker = ai_picker.PhaseNet(picker_args)
                             result = _picker.pick(folders["downloads"],
                                                 folders["metadata"],
                                                 out_path)
                             if result.empty:
                                 print("No picks")
-                                exit()
+                                continue
                             del _picker
                             del result
                             
                 elif process == "associator":
                     inv = os.path.join(folders["metadata"],"inv.xml")
 
                     for picker in self.associator_input:
@@ -268,15 +268,15 @@
                             out_folder = os.path.join(folders["associations"],out_name)
                             if associator == "GaMMA":
                                 _associator = ai_asso.GaMMA(associator_args)
                                 _,result,_ = _associator.associate(picks_path,
                                                             inv,out_folder)
                                 if result.empty:
                                     print("No associated picks")
-                                    exit()
+                                    continue
 
                 elif process == "locator":
                     for locator,locator_args in process_args.items():
                         for task,project in self.locator_input.items():
                             catalog = os.path.join(folders[task],project[0],project[1],task+".xml")
                             nlloc_folder = os.path.join(folders["locations"],locator,project[0],project[1])
                             locator_args.locate(catalog,nlloc_folder)
```

### Comparing `SeisMonitor-0.0.8/SeisMonitor/plot/picks copy.py` & `SeisMonitor-0.0.9/SeisMonitor/plot/picks copy.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/plot/picks.py` & `SeisMonitor-0.0.9/SeisMonitor/plot/picks.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/plot/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/plot/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor/utils.py` & `SeisMonitor-0.0.9/SeisMonitor/utils.py`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/SeisMonitor.egg-info/PKG-INFO` & `SeisMonitor-0.0.9/SeisMonitor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeisMonitor
-Version: 0.0.8
+Version: 0.0.9
 Summary: To monitor seismic activity
 Home-page: https://github.com/ecastillot/SeisMonitor
 Author: ecastillot (Emmanuel Castillo)
 Author-email: <ecastillot@unal.edu.co>
 License: UNKNOWN
 Keywords: python,seismonitor,earthquakes,seismology
 Platform: UNKNOWN
```

### Comparing `SeisMonitor-0.0.8/SeisMonitor.egg-info/SOURCES.txt` & `SeisMonitor-0.0.9/SeisMonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SeisMonitor-0.0.8/setup.py` & `SeisMonitor-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 # here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'To monitor seismic activity'
 LONG_DESCRIPTION = 'A package that allows to monitor the seismic activity through main steps in the monitoring workflow: earthquake detection and phase picking -> phase associator -> earthquake locator -> magnitude estimation.'
 
 req_path = os.path.join(os.path.dirname(__file__),"requirements.txt")
 with pathlib.Path('requirements.txt').open() as requirements_txt:
     install_requires = [
         str(requirement)
```

### Comparing `SeisMonitor-0.0.8/test/test_seismonitor.py` & `SeisMonitor-0.0.9/test/test_seismonitor.py`

 * *Files identical despite different names*


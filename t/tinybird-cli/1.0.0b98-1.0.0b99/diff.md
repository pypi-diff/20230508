# Comparing `tmp/tinybird-cli-1.0.0b98.tar.gz` & `tmp/tinybird-cli-1.0.0b99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tinybird-cli-1.0.0b98.tar", last modified: Fri Feb 25 08:50:18 2022, max compression
+gzip compressed data, was "dist/tinybird-cli-1.0.0b99.tar", last modified: Mon Feb 28 11:30:12 2022, max compression
```

## Comparing `tinybird-cli-1.0.0b98.tar` & `tinybird-cli-1.0.0b99.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 08:50:18.647825 tinybird-cli-1.0.0b98/
--rw-r--r--   0 root         (0) root         (0)    17925 2022-02-25 08:50:18.647825 tinybird-cli-1.0.0b98/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    24927 2022-02-23 14:33:10.000000 tinybird-cli-1.0.0b98/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-25 08:50:18.647825 tinybird-cli-1.0.0b98/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2249 2022-02-10 11:11:41.000000 tinybird-cli-1.0.0b98/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3697 2022-02-22 08:02:29.000000 tinybird-cli-1.0.0b98/setup_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 08:50:18.647825 tinybird-cli-1.0.0b98/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      237 2022-02-25 08:50:16.000000 tinybird-cli-1.0.0b98/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 08:50:18.647825 tinybird-cli-1.0.0b98/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)    23405 2022-01-12 11:16:16.000000 tinybird-cli-1.0.0b98/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2021-11-19 14:15:14.000000 tinybird-cli-1.0.0b98/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    18170 2022-02-22 08:53:54.000000 tinybird-cli-1.0.0b98/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2021-12-17 08:47:03.000000 tinybird-cli-1.0.0b98/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    14738 2021-11-19 14:15:14.000000 tinybird-cli-1.0.0b98/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)    60460 2022-02-24 10:35:54.000000 tinybird-cli-1.0.0b98/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     5137 2022-02-23 14:33:10.000000 tinybird-cli-1.0.0b98/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    19405 2022-02-24 10:35:54.000000 tinybird-cli-1.0.0b98/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    30413 2022-02-22 08:02:29.000000 tinybird-cli-1.0.0b98/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    38921 2022-02-23 14:33:11.000000 tinybird-cli-1.0.0b98/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)     7341 2022-02-24 10:35:54.000000 tinybird-cli-1.0.0b98/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    28052 2021-11-19 14:15:14.000000 tinybird-cli-1.0.0b98/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)    88063 2022-02-25 08:49:55.000000 tinybird-cli-1.0.0b98/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 08:50:18.647825 tinybird-cli-1.0.0b98/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17925 2022-02-25 08:50:18.000000 tinybird-cli-1.0.0b98/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2022-02-25 08:50:18.000000 tinybird-cli-1.0.0b98/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-25 08:50:18.000000 tinybird-cli-1.0.0b98/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-02-25 08:50:18.000000 tinybird-cli-1.0.0b98/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      575 2022-02-25 08:50:18.000000 tinybird-cli-1.0.0b98/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-02-25 08:50:18.000000 tinybird-cli-1.0.0b98/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 11:30:12.371667 tinybird-cli-1.0.0b99/
+-rw-r--r--   0 root         (0) root         (0)    18086 2022-02-28 11:30:12.371667 tinybird-cli-1.0.0b99/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    24927 2022-02-23 14:33:10.000000 tinybird-cli-1.0.0b99/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-02-28 11:30:12.371667 tinybird-cli-1.0.0b99/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2022-02-10 11:11:41.000000 tinybird-cli-1.0.0b99/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3735 2022-02-28 11:29:48.000000 tinybird-cli-1.0.0b99/setup_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 11:30:12.367667 tinybird-cli-1.0.0b99/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2022-02-28 11:30:10.000000 tinybird-cli-1.0.0b99/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 11:30:12.367667 tinybird-cli-1.0.0b99/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2022-02-17 18:49:29.000000 tinybird-cli-1.0.0b99/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    23405 2022-02-25 13:30:22.000000 tinybird-cli-1.0.0b99/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2021-11-19 14:15:14.000000 tinybird-cli-1.0.0b99/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    18170 2022-02-22 08:53:54.000000 tinybird-cli-1.0.0b99/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2021-12-17 08:47:03.000000 tinybird-cli-1.0.0b99/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    14738 2021-11-19 14:15:14.000000 tinybird-cli-1.0.0b99/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)    60460 2022-02-24 10:35:54.000000 tinybird-cli-1.0.0b99/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     5137 2022-02-23 14:33:10.000000 tinybird-cli-1.0.0b99/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    19405 2022-02-24 10:35:54.000000 tinybird-cli-1.0.0b99/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    30413 2022-02-22 08:02:29.000000 tinybird-cli-1.0.0b99/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    38921 2022-02-23 14:33:11.000000 tinybird-cli-1.0.0b99/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     7341 2022-02-24 10:35:54.000000 tinybird-cli-1.0.0b99/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    28052 2021-11-19 14:15:14.000000 tinybird-cli-1.0.0b99/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)    88063 2022-02-25 13:30:22.000000 tinybird-cli-1.0.0b99/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 11:30:12.367667 tinybird-cli-1.0.0b99/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18086 2022-02-28 11:30:12.000000 tinybird-cli-1.0.0b99/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      590 2022-02-28 11:30:12.000000 tinybird-cli-1.0.0b99/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-28 11:30:12.000000 tinybird-cli-1.0.0b99/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-02-28 11:30:12.000000 tinybird-cli-1.0.0b99/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      575 2022-02-28 11:30:12.000000 tinybird-cli-1.0.0b99/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-02-28 11:30:12.000000 tinybird-cli-1.0.0b99/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-1.0.0b98/PKG-INFO` & `tinybird-cli-1.0.0b99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 1.0.0b98
+Version: 1.0.0b99
 Summary: Tinybird Command Line Tool
 Home-page: https://docs.tinybird.co/cli.html
 Author: Tinybird
 Author-email: support@tinybird.co
 License: UNKNOWN
 Description: 
         Tinybird CLI
         ============
         
         The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
         
         Changelog
         ---------
         
+        1.0.0b99
+        ********
+        
+        - Fix broken release 1.0.0b98. The published package missed one dependency required for some commands.
+        
         1.0.0b98
         ********
         
-        - `tb auth --interactive` now supports custom regions 
+        - `tb auth --interactive` now supports custom regions
         
         1.0.0b97
         ********
         
         - Add `--sample` option for `--populate`
         
         1.0.0b96
@@ -34,15 +39,15 @@
         ********
         
         - Fix broken release 1.0.0b94.
         
         1.0.0b94
         ********
         
-        - Changed the name for workspace plans. 
+        - Changed the name for workspace plans.
         
         1.0.0b93
         ********
         
         - Improved error message format pushing a pipe.
         
         1.0.0b92
```

### Comparing `tinybird-cli-1.0.0b98/README.md` & `tinybird-cli-1.0.0b99/README.md`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/setup.py` & `tinybird-cli-1.0.0b99/setup.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/setup_cli.py` & `tinybird-cli-1.0.0b99/setup_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 with open(path.join(here, 'cli_changelog.rst')) as f:
     readme = f.read()
 
 # if you change any of these remember to change .gitlab-ci
 included = [
     'tinybird/check_pypi.py',
+    'tinybird/ch_utils/constants.py',
     'tinybird/ch_utils/engine.py',
     'tinybird/client.py',
     'tinybird/__cli__.py',
     'tinybird/config.py',
     'tinybird/connectors.py',
     'tinybird/datafile.py',
     'tinybird/datatypes.py',
```

### Comparing `tinybird-cli-1.0.0b98/tinybird/ch_utils/engine.py` & `tinybird-cli-1.0.0b99/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/check_pypi.py` & `tinybird-cli-1.0.0b99/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/client.py` & `tinybird-cli-1.0.0b99/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/config.py` & `tinybird-cli-1.0.0b99/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/connectors.py` & `tinybird-cli-1.0.0b99/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/datafile.py` & `tinybird-cli-1.0.0b99/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/datatypes.py` & `tinybird-cli-1.0.0b99/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/feedback_manager.py` & `tinybird-cli-1.0.0b99/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/sql.py` & `tinybird-cli-1.0.0b99/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/sql_template.py` & `tinybird-cli-1.0.0b99/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/sql_toolset.py` & `tinybird-cli-1.0.0b99/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/syncasync.py` & `tinybird-cli-1.0.0b99/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird/tb_cli.py` & `tinybird-cli-1.0.0b99/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-1.0.0b98/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-1.0.0b99/tinybird_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 1.0.0b98
+Version: 1.0.0b99
 Summary: Tinybird Command Line Tool
 Home-page: https://docs.tinybird.co/cli.html
 Author: Tinybird
 Author-email: support@tinybird.co
 License: UNKNOWN
 Description: 
         Tinybird CLI
         ============
         
         The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
         
         Changelog
         ---------
         
+        1.0.0b99
+        ********
+        
+        - Fix broken release 1.0.0b98. The published package missed one dependency required for some commands.
+        
         1.0.0b98
         ********
         
-        - `tb auth --interactive` now supports custom regions 
+        - `tb auth --interactive` now supports custom regions
         
         1.0.0b97
         ********
         
         - Add `--sample` option for `--populate`
         
         1.0.0b96
@@ -34,15 +39,15 @@
         ********
         
         - Fix broken release 1.0.0b94.
         
         1.0.0b94
         ********
         
-        - Changed the name for workspace plans. 
+        - Changed the name for workspace plans.
         
         1.0.0b93
         ********
         
         - Improved error message format pushing a pipe.
         
         1.0.0b92
```

### Comparing `tinybird-cli-1.0.0b98/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-1.0.0b99/tinybird_cli.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 tinybird/datatypes.py
 tinybird/feedback_manager.py
 tinybird/sql.py
 tinybird/sql_template.py
 tinybird/sql_toolset.py
 tinybird/syncasync.py
 tinybird/tb_cli.py
+tinybird/ch_utils/constants.py
 tinybird/ch_utils/engine.py
 tinybird_cli.egg-info/PKG-INFO
 tinybird_cli.egg-info/SOURCES.txt
 tinybird_cli.egg-info/dependency_links.txt
 tinybird_cli.egg-info/entry_points.txt
 tinybird_cli.egg-info/requires.txt
 tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-1.0.0b98/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-1.0.0b99/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*


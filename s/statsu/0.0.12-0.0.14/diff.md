# Comparing `tmp/statsu-0.0.12.tar.gz` & `tmp/statsu-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsu-0.0.12.tar", last modified: Wed Jan 11 08:18:55 2023, max compression
+gzip compressed data, was "statsu-0.0.14.tar", last modified: Mon May  8 02:02:06 2023, max compression
```

## Comparing `statsu-0.0.12.tar` & `statsu-0.0.14.tar`

### file list

```diff
@@ -1,37 +1,81 @@
-drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-01-11 08:18:55.164142 statsu-0.0.12/
--rw-r--r--   0 sbyim      (501) staff       (20)     1069 2022-09-28 23:49:55.000000 statsu-0.0.12/LICENSE
--rw-r--r--   0 sbyim      (501) staff       (20)     3878 2023-01-11 08:18:55.163889 statsu-0.0.12/PKG-INFO
--rw-r--r--   0 sbyim      (501) staff       (20)     2394 2023-01-11 08:11:43.000000 statsu-0.0.12/README.md
--rw-r--r--   0 sbyim      (501) staff       (20)       38 2023-01-11 08:18:55.164186 statsu-0.0.12/setup.cfg
--rw-r--r--   0 sbyim      (501) staff       (20)      607 2023-01-11 08:18:51.000000 statsu-0.0.12/setup.py
-drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-01-11 08:18:55.161147 statsu-0.0.12/statsu/
--rw-r--r--   0 sbyim      (501) staff       (20)       73 2023-01-03 03:53:44.000000 statsu-0.0.12/statsu/__init__.py
--rw-r--r--   0 sbyim      (501) staff       (20)      824 2022-10-25 06:11:55.000000 statsu-0.0.12/statsu/__main__.py
-drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-01-11 08:18:55.162437 statsu-0.0.12/statsu/actions/
--rw-r--r--   0 sbyim      (501) staff       (20)        0 2023-01-06 05:47:50.000000 statsu-0.0.12/statsu/actions/__init__.py
--rw-r--r--   0 sbyim      (501) staff       (20)      323 2023-01-04 02:06:31.000000 statsu-0.0.12/statsu/actions/action_base.py
--rw-r--r--   0 sbyim      (501) staff       (20)     2369 2023-01-10 02:15:59.000000 statsu-0.0.12/statsu/actions/action_edit.py
--rw-r--r--   0 sbyim      (501) staff       (20)     2965 2022-12-01 04:07:22.000000 statsu-0.0.12/statsu/actions/action_file.py
--rw-r--r--   0 sbyim      (501) staff       (20)      122 2022-12-14 08:27:01.000000 statsu-0.0.12/statsu/actions/settings.py
--rw-r--r--   0 sbyim      (501) staff       (20)     4093 2023-01-06 07:59:38.000000 statsu-0.0.12/statsu/core.py
-drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-01-11 08:18:55.162759 statsu-0.0.12/statsu/data/
--rw-r--r--   0 sbyim      (501) staff       (20)        0 2022-10-25 02:07:21.000000 statsu-0.0.12/statsu/data/__init__.py
--rw-r--r--   0 sbyim      (501) staff       (20)     5508 2023-01-10 02:07:13.000000 statsu-0.0.12/statsu/data/data_model.py
--rw-r--r--   0 sbyim      (501) staff       (20)     1455 2023-01-06 06:45:23.000000 statsu-0.0.12/statsu/data/file_manager.py
-drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-01-11 08:18:55.163287 statsu-0.0.12/statsu/ui/
--rw-r--r--   0 sbyim      (501) staff       (20)        0 2022-10-25 02:07:31.000000 statsu-0.0.12/statsu/ui/__init__.py
--rw-r--r--   0 sbyim      (501) staff       (20)     4342 2023-01-10 02:21:15.000000 statsu-0.0.12/statsu/ui/data_container.py
-drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-01-11 08:18:55.163684 statsu-0.0.12/statsu/ui/design/
--rw-r--r--   0 sbyim      (501) staff       (20)        0 2022-10-25 02:07:52.000000 statsu-0.0.12/statsu/ui/design/__init__.py
--rw-r--r--   0 sbyim      (501) staff       (20)     1680 2022-10-14 06:19:52.000000 statsu-0.0.12/statsu/ui/design/data_container.py
--rw-r--r--   0 sbyim      (501) staff       (20)     7729 2023-01-06 04:41:39.000000 statsu-0.0.12/statsu/ui/design/main_window.py
--rw-r--r--   0 sbyim      (501) staff       (20)     6524 2022-10-13 09:07:20.000000 statsu-0.0.12/statsu/ui/design/open_csv_dialog.py
--rw-r--r--   0 sbyim      (501) staff       (20)     1890 2022-10-25 02:27:49.000000 statsu-0.0.12/statsu/ui/dialog.py
--rw-r--r--   0 sbyim      (501) staff       (20)      858 2023-01-06 07:59:38.000000 statsu-0.0.12/statsu/ui/main_window.py
--rw-r--r--   0 sbyim      (501) staff       (20)     1035 2023-01-06 06:15:50.000000 statsu-0.0.12/statsu/ui/user_command.py
-drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-01-11 08:18:55.161717 statsu-0.0.12/statsu.egg-info/
--rw-r--r--   0 sbyim      (501) staff       (20)     3878 2023-01-11 08:18:55.000000 statsu-0.0.12/statsu.egg-info/PKG-INFO
--rw-r--r--   0 sbyim      (501) staff       (20)      703 2023-01-11 08:18:55.000000 statsu-0.0.12/statsu.egg-info/SOURCES.txt
--rw-r--r--   0 sbyim      (501) staff       (20)        1 2023-01-11 08:18:55.000000 statsu-0.0.12/statsu.egg-info/dependency_links.txt
--rw-r--r--   0 sbyim      (501) staff       (20)       24 2023-01-11 08:18:55.000000 statsu-0.0.12/statsu.egg-info/requires.txt
--rw-r--r--   0 sbyim      (501) staff       (20)        7 2023-01-11 08:18:55.000000 statsu-0.0.12/statsu.egg-info/top_level.txt
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.498447 statsu-0.0.14/
+-rw-r--r--   0 sbyim      (501) staff       (20)     1918 2023-04-17 01:01:37.000000 statsu-0.0.14/.gitignore
+-rw-r--r--   0 sbyim      (501) staff       (20)     1069 2023-04-17 01:01:37.000000 statsu-0.0.14/LICENSE
+-rw-r--r--   0 sbyim      (501) staff       (20)     3484 2023-05-08 02:02:06.498287 statsu-0.0.14/PKG-INFO
+-rw-r--r--   0 sbyim      (501) staff       (20)      222 2023-04-17 01:01:37.000000 statsu-0.0.14/Pipfile
+-rw-r--r--   0 sbyim      (501) staff       (20)    30385 2023-05-08 01:41:06.000000 statsu-0.0.14/Pipfile.lock
+-rw-r--r--   0 sbyim      (501) staff       (20)     2000 2023-05-08 02:01:07.000000 statsu-0.0.14/README.md
+-rw-r--r--   0 sbyim      (501) staff       (20)      522 2023-04-17 01:01:37.000000 statsu-0.0.14/debug_run.py
+-rw-r--r--   0 sbyim      (501) staff       (20)       38 2023-05-08 02:02:06.498490 statsu-0.0.14/setup.cfg
+-rw-r--r--   0 sbyim      (501) staff       (20)      607 2023-05-08 01:39:17.000000 statsu-0.0.14/setup.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.491289 statsu-0.0.14/statsu/
+-rw-r--r--   0 sbyim      (501) staff       (20)       79 2023-04-25 08:22:25.000000 statsu-0.0.14/statsu/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)      824 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/__main__.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.492844 statsu-0.0.14/statsu/actions/
+-rw-r--r--   0 sbyim      (501) staff       (20)        0 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/actions/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)      323 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/actions/action_base.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     2369 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/actions/action_edit.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     2965 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/actions/action_file.py
+-rw-r--r--   0 sbyim      (501) staff       (20)      122 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/actions/settings.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     4545 2023-04-25 08:22:05.000000 statsu-0.0.14/statsu/core.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.493168 statsu-0.0.14/statsu/data/
+-rw-r--r--   0 sbyim      (501) staff       (20)        0 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/data/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     5508 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/data/data_model.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     1455 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/data/file_manager.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.493731 statsu-0.0.14/statsu/ui/
+-rw-r--r--   0 sbyim      (501) staff       (20)        0 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/ui/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     4291 2023-04-18 00:58:52.000000 statsu-0.0.14/statsu/ui/data_container.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.494556 statsu-0.0.14/statsu/ui/design/
+-rw-r--r--   0 sbyim      (501) staff       (20)        0 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/ui/design/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     1680 2023-04-17 02:58:50.000000 statsu-0.0.14/statsu/ui/design/data_container.py
+-rw-r--r--   0 sbyim      (501) staff       (20)      650 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/ui/design/data_container.ui
+-rw-r--r--   0 sbyim      (501) staff       (20)     9069 2023-04-17 02:58:31.000000 statsu-0.0.14/statsu/ui/design/main_window.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     5540 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/ui/design/main_window.ui
+-rw-r--r--   0 sbyim      (501) staff       (20)     6524 2023-04-17 02:59:10.000000 statsu-0.0.14/statsu/ui/design/open_csv_dialog.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     5003 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/ui/design/open_csv_dialog.ui
+-rw-r--r--   0 sbyim      (501) staff       (20)     1890 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/ui/dialog.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     1344 2023-04-18 01:15:14.000000 statsu-0.0.14/statsu/ui/main_window.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     1035 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu/ui/user_command.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.491988 statsu-0.0.14/statsu.egg-info/
+-rw-r--r--   0 sbyim      (501) staff       (20)     3484 2023-05-08 02:02:06.000000 statsu-0.0.14/statsu.egg-info/PKG-INFO
+-rw-r--r--   0 sbyim      (501) staff       (20)     1904 2023-05-08 02:02:06.000000 statsu-0.0.14/statsu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbyim      (501) staff       (20)        1 2023-05-08 02:02:06.000000 statsu-0.0.14/statsu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbyim      (501) staff       (20)       24 2023-05-08 02:02:06.000000 statsu-0.0.14/statsu.egg-info/requires.txt
+-rw-r--r--   0 sbyim      (501) staff       (20)        7 2023-05-08 02:02:06.000000 statsu-0.0.14/statsu.egg-info/top_level.txt
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.489601 statsu-0.0.14/statsu_legacy/
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.494678 statsu-0.0.14/statsu_legacy/v1/
+-rw-r--r--   0 sbyim      (501) staff       (20)     1599 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/__init__.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.494800 statsu-0.0.14/statsu_legacy/v1/actions/
+-rw-r--r--   0 sbyim      (501) staff       (20)      479 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/actions/__init__.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.495259 statsu-0.0.14/statsu_legacy/v1/actions/menu_action/
+-rw-r--r--   0 sbyim      (501) staff       (20)      172 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/actions/menu_action/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)      472 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/actions/menu_action/analysis.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     2377 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/actions/menu_action/file.py
+-rw-r--r--   0 sbyim      (501) staff       (20)      250 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/actions/menu_action/tools.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.495499 statsu-0.0.14/statsu_legacy/v1/statistics/
+-rw-r--r--   0 sbyim      (501) staff       (20)      814 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/statistics/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)       93 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/statistics/descriptive_statistics.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.496212 statsu-0.0.14/statsu_legacy/v1/widgets/
+-rw-r--r--   0 sbyim      (501) staff       (20)        0 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/__init__.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.496484 statsu-0.0.14/statsu_legacy/v1/widgets/analysis/
+-rw-r--r--   0 sbyim      (501) staff       (20)     2905 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/analysis/general_bridge.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     2182 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/analysis/general_bridge.ui
+-rw-r--r--   0 sbyim      (501) staff       (20)     3485 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/datasheet.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     2146 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/datasheet.ui
+-rw-r--r--   0 sbyim      (501) staff       (20)     4763 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/datasheet_old.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     2057 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/main_window.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     5835 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v1/widgets/main_window.ui
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.496630 statsu-0.0.14/statsu_legacy/v2/
+-rw-r--r--   0 sbyim      (501) staff       (20)      359 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/__init__.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.497271 statsu-0.0.14/statsu_legacy/v2/actions/
+-rw-r--r--   0 sbyim      (501) staff       (20)     1427 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/actions/__init__.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     1066 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/actions/analysis.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     1496 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/actions/file.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.497390 statsu-0.0.14/statsu_legacy/v2/widgets/
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.497923 statsu-0.0.14/statsu_legacy/v2/widgets/analysis/
+-rw-r--r--   0 sbyim      (501) staff       (20)     3066 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/widgets/analysis/general_bridge.py
+-rw-r--r--   0 sbyim      (501) staff       (20)     2240 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/widgets/analysis/run_function_dialog.ui
+-rw-r--r--   0 sbyim      (501) staff       (20)     4068 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/widgets/analysis/select_function_dialog.ui
+-rw-r--r--   0 sbyim      (501) staff       (20)      667 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_legacy/v2/widgets/pgui_window.py
+drwxr-xr-x   0 sbyim      (501) staff       (20)        0 2023-05-08 02:02:06.498037 statsu-0.0.14/statsu_test/
+-rw-r--r--   0 sbyim      (501) staff       (20)      453 2023-04-17 01:01:37.000000 statsu-0.0.14/statsu_test/test.py
```

### Comparing `statsu-0.0.12/LICENSE` & `statsu-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `statsu-0.0.12/setup.py` & `statsu-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("LICENSE", "r") as fh:
     lsc = fh.read()
 
 setup(
     name='statsu',
-    version='0.0.12',
+    version='0.0.14',
     author='sbyim',
     author_email='ysb06@hotmail.com',
     description='Pandas Dataframe Editor',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['statsu_test']),
     url='https://github.com/ysb06/statsu',
```

### Comparing `statsu-0.0.12/statsu/__main__.py` & `statsu-0.0.14/statsu/__main__.py`

 * *Files identical despite different names*

### Comparing `statsu-0.0.12/statsu/actions/action_edit.py` & `statsu-0.0.14/statsu/actions/action_edit.py`

 * *Files identical despite different names*

### Comparing `statsu-0.0.12/statsu/actions/action_file.py` & `statsu-0.0.14/statsu/actions/action_file.py`

 * *Files identical despite different names*

### Comparing `statsu-0.0.12/statsu/core.py` & `statsu-0.0.14/statsu/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 from PySide6.QtGui import QKeySequence
 from PySide6.QtWidgets import QApplication
 
 from statsu.actions.action_edit import ActionEdit
 from statsu.actions.action_file import ActionFile
 from statsu.ui.data_container import DataContainer
 from statsu.ui.main_window import MainWindow
-from statsu.ui.user_command import UserCommandManager
 
 logging.basicConfig(
     format='%(asctime)s %(name)s [%(levelname)s] %(message)s',
     datefmt='%Y/%m/%d %H:%M:%S',
     level=logging.INFO
 )
 
 logger = logging.getLogger(__name__)
-app = QApplication(sys.argv)
 
 @dataclass
 class DataObject:
     data_frame_origin: pd.DataFrame
     name: str = 'Data'
 
     def __post_init__(self):
@@ -76,29 +74,49 @@
 
     def show(self) -> None:
         self.main_window.show()
 
     def update(self) -> None:
         self.main_window.update()
 
+def load(input_data: pd.DataFrame = None, name: str = None) -> WindowUnit:
+    if input_data is not None:
+        window = WindowUnit(
+            in_memory_data=[DataObject(input_data, name=name if name is not None else 'Data')]
+        )
+    else:
+        window = WindowUnit()
+
+    return window
 
 def show(input_data: pd.DataFrame = None, name: str = None) -> pd.DataFrame:
+    app = QApplication.instance()
+    if app is None: 
+        app = QApplication(sys.argv)
+
     if input_data is not None:
         window = WindowUnit(
             in_memory_data=[DataObject(input_data, name=name if name is not None else 'Data')]
         )
     else:
         window = WindowUnit()
 
     window.show()
     app.exec()
 
 def show_list(input_data: List[pd.DataFrame]):
+    app = QApplication.instance()
+    if app is None: 
+        app = QApplication(sys.argv)
+
     window = WindowUnit([DataObject(data) for data in input_data])
     window.show()
     app.exec()
 
 def show_list_with_name(input_data: List[DataObject]):
+    app = QApplication.instance()
+    app.exec()
+
     window = WindowUnit(input_data)
     window.show()
     app.exec()
```

### Comparing `statsu-0.0.12/statsu/data/data_model.py` & `statsu-0.0.14/statsu/data/data_model.py`

 * *Files identical despite different names*

### Comparing `statsu-0.0.12/statsu/data/file_manager.py` & `statsu-0.0.14/statsu/data/file_manager.py`

 * *Files identical despite different names*

### Comparing `statsu-0.0.12/statsu/ui/data_container.py` & `statsu-0.0.14/statsu/ui/data_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 
 class DataContainer(QWidget, Ui_DataContainer):
     def __init__(
             self,
             data: pd.DataFrame = None,
             name: str = 'Sheet',
             data_path: Optional[str] = None,
-            parent: Optional[QWidget] = None
         ) -> None:
-        super().__init__(parent)
+        super().__init__()
         self.setupUi(self)
 
         self.command_manager: UserCommandManager = None
 
         if data is None:
             data = pd.DataFrame()
         self.raw_data = data
```

### Comparing `statsu-0.0.12/statsu/ui/design/data_container.py` & `statsu-0.0.14/statsu/ui/design/data_container.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'data_container.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.3.2
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `statsu-0.0.12/statsu/ui/design/main_window.py` & `statsu-0.0.14/statsu/ui/design/main_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'main_window.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.1
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
     QCursor, QFont, QFontDatabase, QGradient,
     QIcon, QImage, QKeySequence, QLinearGradient,
     QPainter, QPalette, QPixmap, QRadialGradient,
     QTransform)
-from PySide6.QtWidgets import (QApplication, QGridLayout, QMainWindow, QMenu,
-    QMenuBar, QSizePolicy, QStatusBar, QTabWidget,
-    QWidget)
+from PySide6.QtWidgets import (QApplication, QHBoxLayout, QMainWindow, QMenu,
+    QMenuBar, QPushButton, QSizePolicy, QStatusBar,
+    QTabWidget, QToolBar, QVBoxLayout, QWidget)
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
         MainWindow.resize(640, 480)
         self.action_file_new = QAction(MainWindow)
@@ -51,35 +51,57 @@
         self.action_edit_paste.setObjectName(u"action_edit_paste")
         self.action_edit_undo = QAction(MainWindow)
         self.action_edit_undo.setObjectName(u"action_edit_undo")
         self.action_edit_redo = QAction(MainWindow)
         self.action_edit_redo.setObjectName(u"action_edit_redo")
         self.central_widget = QWidget(MainWindow)
         self.central_widget.setObjectName(u"central_widget")
-        self.gridLayout_2 = QGridLayout(self.central_widget)
-        self.gridLayout_2.setObjectName(u"gridLayout_2")
+        self.verticalLayout = QVBoxLayout(self.central_widget)
+        self.verticalLayout.setObjectName(u"verticalLayout")
         self.main_data_tab_widget = QTabWidget(self.central_widget)
         self.main_data_tab_widget.setObjectName(u"main_data_tab_widget")
         self.main_data_tab_widget.setTabPosition(QTabWidget.South)
         self.main_data_tab_widget.setTabShape(QTabWidget.Rounded)
 
-        self.gridLayout_2.addWidget(self.main_data_tab_widget, 0, 0, 1, 1)
+        self.verticalLayout.addWidget(self.main_data_tab_widget)
+
+        self.container_controller = QWidget(self.central_widget)
+        self.container_controller.setObjectName(u"container_controller")
+        self.horizontalLayout = QHBoxLayout(self.container_controller)
+        self.horizontalLayout.setObjectName(u"horizontalLayout")
+        self.horizontalLayout.setContentsMargins(0, 0, 0, 0)
+        self.prev_page_button = QPushButton(self.container_controller)
+        self.prev_page_button.setObjectName(u"prev_page_button")
+        self.prev_page_button.setCheckable(False)
+
+        self.horizontalLayout.addWidget(self.prev_page_button)
+
+        self.next_page_button = QPushButton(self.container_controller)
+        self.next_page_button.setObjectName(u"next_page_button")
+
+        self.horizontalLayout.addWidget(self.next_page_button)
+
+
+        self.verticalLayout.addWidget(self.container_controller)
 
         MainWindow.setCentralWidget(self.central_widget)
         self.main_menubar = QMenuBar(MainWindow)
         self.main_menubar.setObjectName(u"main_menubar")
         self.main_menubar.setGeometry(QRect(0, 0, 640, 37))
         self.menuFile_F = QMenu(self.main_menubar)
         self.menuFile_F.setObjectName(u"menuFile_F")
         self.menuEdit_E = QMenu(self.main_menubar)
         self.menuEdit_E.setObjectName(u"menuEdit_E")
         MainWindow.setMenuBar(self.main_menubar)
         self.statusbar = QStatusBar(MainWindow)
         self.statusbar.setObjectName(u"statusbar")
         MainWindow.setStatusBar(self.statusbar)
+        self.toolBar = QToolBar(MainWindow)
+        self.toolBar.setObjectName(u"toolBar")
+        MainWindow.addToolBar(Qt.TopToolBarArea, self.toolBar)
 
         self.main_menubar.addAction(self.menuFile_F.menuAction())
         self.main_menubar.addAction(self.menuEdit_E.menuAction())
         self.menuFile_F.addAction(self.action_file_new)
         self.menuFile_F.addAction(self.action_file_open)
         self.menuFile_F.addSeparator()
         self.menuFile_F.addAction(self.action_file_save)
@@ -136,11 +158,14 @@
 #endif // QT_CONFIG(shortcut)
         self.action_edit_paste.setText(QCoreApplication.translate("MainWindow", u"Paste (&V)", None))
 #if QT_CONFIG(shortcut)
         self.action_edit_paste.setShortcut(QCoreApplication.translate("MainWindow", u"Ctrl+V", None))
 #endif // QT_CONFIG(shortcut)
         self.action_edit_undo.setText(QCoreApplication.translate("MainWindow", u"Undo", None))
         self.action_edit_redo.setText(QCoreApplication.translate("MainWindow", u"Redo", None))
+        self.prev_page_button.setText(QCoreApplication.translate("MainWindow", u"< Prev Page", None))
+        self.next_page_button.setText(QCoreApplication.translate("MainWindow", u"Next Page >", None))
         self.menuFile_F.setTitle(QCoreApplication.translate("MainWindow", u"File (&F)", None))
         self.menuEdit_E.setTitle(QCoreApplication.translate("MainWindow", u"Edit", None))
+        self.toolBar.setWindowTitle(QCoreApplication.translate("MainWindow", u"toolBar", None))
     # retranslateUi
```

### Comparing `statsu-0.0.12/statsu/ui/design/open_csv_dialog.py` & `statsu-0.0.14/statsu/ui/design/open_csv_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'open_csv_dialog.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.3.2
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `statsu-0.0.12/statsu/ui/dialog.py` & `statsu-0.0.14/statsu/ui/dialog.py`

 * *Files identical despite different names*

### Comparing `statsu-0.0.12/statsu/ui/user_command.py` & `statsu-0.0.14/statsu/ui/user_command.py`

 * *Files identical despite different names*


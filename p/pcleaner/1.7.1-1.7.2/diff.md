# Comparing `tmp/pcleaner-1.7.1.tar.gz` & `tmp/pcleaner-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.7.1.tar", last modified: Sun May  7 15:40:57 2023, max compression
+gzip compressed data, was "pcleaner-1.7.2.tar", last modified: Mon May  8 16:48:50 2023, max compression
```

## Comparing `pcleaner-1.7.1.tar` & `pcleaner-1.7.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.637381 pcleaner-1.7.1/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.7.1/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-07 15:40:57.637381 pcleaner-1.7.1/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11599 2023-05-04 21:07:46.000000 pcleaner-1.7.1/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-05-07 15:40:17.000000 pcleaner-1.7.1/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-05-04 21:08:14.000000 pcleaner-1.7.1/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6380 2023-05-04 21:08:14.000000 pcleaner-1.7.1/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.630714 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    45416 2023-05-05 16:06:03.000000 pcleaner-1.7.1/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6333 2023-05-07 15:38:48.000000 pcleaner-1.7.1/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.7.1/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.7.1/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.7.1/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.7.1/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2600 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/CColorButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3323 2023-05-05 21:26:07.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.7.1/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1094 2023-05-05 20:27:29.000000 pcleaner-1.7.1/pcleaner/gui/gui_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1958 2023-04-22 17:01:16.000000 pcleaner-1.7.1/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    42594 2023-05-05 21:40:55.000000 pcleaner-1.7.1/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4457 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/new_profile_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16468 2023-05-05 21:36:36.000000 pcleaner-1.7.1/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10008 2023-04-22 16:59:47.000000 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/icons_rc.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    75061 2023-04-22 17:01:02.000000 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/theme_icons_rc.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.637381 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    29795 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7464 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1828 2023-04-21 20:13:16.000000 pcleaner-1.7.1/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23467 2023-05-05 14:10:21.000000 pcleaner-1.7.1/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27027 2023-05-06 17:47:48.000000 pcleaner-1.7.1/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-05-06 17:47:48.000000 pcleaner-1.7.1/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.7.1/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8817 2023-05-06 17:51:16.000000 pcleaner-1.7.1/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7581 2023-05-04 21:08:14.000000 pcleaner-1.7.1/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-05-06 17:51:42.000000 pcleaner-1.7.1/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2218 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.7.1/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-05-07 15:40:57.637381 pcleaner-1.7.1/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.7.1/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.614474 pcleaner-1.7.2/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.7.2/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-08 16:48:50.614474 pcleaner-1.7.2/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11599 2023-05-04 21:07:46.000000 pcleaner-1.7.2/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.604474 pcleaner-1.7.2/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-05-08 16:48:42.000000 pcleaner-1.7.2/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-05-04 21:08:14.000000 pcleaner-1.7.2/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6380 2023-05-04 21:08:14.000000 pcleaner-1.7.2/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.607807 pcleaner-1.7.2/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.607807 pcleaner-1.7.2/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.607807 pcleaner-1.7.2/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.611141 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.7.2/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    45878 2023-05-08 00:59:00.000000 pcleaner-1.7.2/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6237 2023-05-08 16:47:38.000000 pcleaner-1.7.2/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.611141 pcleaner-1.7.2/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.7.2/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.7.2/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.7.2/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.7.2/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.614474 pcleaner-1.7.2/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.614474 pcleaner-1.7.2/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2600 2023-05-05 16:04:17.000000 pcleaner-1.7.2/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3651 2023-05-08 16:20:55.000000 pcleaner-1.7.2/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.7.2/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.7.2/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.7.2/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-05-05 16:04:17.000000 pcleaner-1.7.2/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1094 2023-05-05 20:27:29.000000 pcleaner-1.7.2/pcleaner/gui/gui_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1958 2023-04-22 17:01:16.000000 pcleaner-1.7.2/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    48840 2023-05-08 16:25:13.000000 pcleaner-1.7.2/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4457 2023-05-05 16:04:17.000000 pcleaner-1.7.2/pcleaner/gui/new_profile_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16366 2023-05-08 02:27:17.000000 pcleaner-1.7.2/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.614474 pcleaner-1.7.2/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.7.2/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10008 2023-04-22 16:59:47.000000 pcleaner-1.7.2/pcleaner/gui/rc_generated_files/icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    75061 2023-04-22 17:01:02.000000 pcleaner-1.7.2/pcleaner/gui/rc_generated_files/theme_icons_rc.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.614474 pcleaner-1.7.2/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.7.2/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.7.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    30265 2023-05-08 02:51:16.000000 pcleaner-1.7.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7464 2023-05-05 16:04:17.000000 pcleaner-1.7.2/pcleaner/gui/ui_generated_files/ui_NewProfile.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-05-05 16:04:17.000000 pcleaner-1.7.2/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1828 2023-04-21 20:13:16.000000 pcleaner-1.7.2/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23467 2023-05-05 14:10:21.000000 pcleaner-1.7.2/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27106 2023-05-08 01:47:32.000000 pcleaner-1.7.2/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-05-06 17:47:48.000000 pcleaner-1.7.2/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.7.2/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8817 2023-05-06 17:51:16.000000 pcleaner-1.7.2/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7989 2023-05-08 02:36:30.000000 pcleaner-1.7.2/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-05-06 17:51:42.000000 pcleaner-1.7.2/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:48:50.607807 pcleaner-1.7.2/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-08 16:48:50.000000 pcleaner-1.7.2/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2218 2023-05-08 16:48:50.000000 pcleaner-1.7.2/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-05-08 16:48:50.000000 pcleaner-1.7.2/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-05-08 16:48:50.000000 pcleaner-1.7.2/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-05-08 16:48:50.000000 pcleaner-1.7.2/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-05-08 16:48:50.000000 pcleaner-1.7.2/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.7.2/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-05-08 16:48:50.614474 pcleaner-1.7.2/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.7.2/setup.py
```

### Comparing `pcleaner-1.7.1/LICENSE` & `pcleaner-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/PKG-INFO` & `pcleaner-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.7.1
+Version: 1.7.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pcleaner-1.7.1/README.md` & `pcleaner-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/analytics.py` & `pcleaner-1.7.2/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/cli_utils.py` & `pcleaner-1.7.2/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.7.2/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/config.py` & `pcleaner-1.7.2/pcleaner/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 import configupdater as cu
 from logzero import logger
 
 from pcleaner import cli_utils as cli
 from pcleaner import model_downloader as md
 from pcleaner import helpers as hp
 
-RESERVED_PROFILE_NAMES = ["builtin", "none", "default"]
+RESERVED_PROFILE_NAMES = ["default", "builtin", "none"]
+
+DEFAULT_PROFILE_NAME = RESERVED_PROFILE_NAMES[0].capitalize()
 
 # Supported image suffixes.
 SUPPORTED_IMG_TYPES = [
     ".jpeg",
     ".jpg",
     ".png",
     ".bmp",
@@ -792,14 +794,24 @@
         try_to_load(config, conf_updater, section, Path | None, "cache_dir")
         config.saved_profiles = {
             k: Path(v.value) for k, v in conf_updater["Saved Profiles"].items()
         }
         try_to_load(config, conf_updater, section, Path | None, "default_torch_model_path")
         try_to_load(config, conf_updater, section, Path | None, "default_cv2_model_path")
 
+        # If the default profile isn't in the saved profiles, clear it.
+        if (
+            config.default_profile is not None
+            and config.default_profile not in config.saved_profiles
+        ):
+            logger.error(
+                f"Default profile {config.default_profile} not found in saved profiles. Clearing entry."
+            )
+            config.default_profile = None
+
         if config.default_torch_model_path is not None:
             # Verify that the model exists and has the correct hash.
             if not config.default_torch_model_path.is_file():
                 print("Configured torch model does not exist. Clearing entry.")
                 config.default_torch_model_path = None
             elif not md.check_hash(config.default_torch_model_path, md.TORCH_SHA256):
                 print("Configured torch model has the wrong hash. Clearing entry.")
```

### Comparing `pcleaner-1.7.1/pcleaner/ctd_interface.py` & `pcleaner-1.7.2/pcleaner/ctd_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 import json
 import uuid
 from pathlib import Path
 import multiprocessing as mp
 
 from tqdm import tqdm
-from PIL import Image
 import torch
 import numpy as np
 import cv2
 from logzero import logger
 
 import pcleaner.config as cfg
 from .comic_text_detector.inference import TextDetector
@@ -162,19 +161,16 @@
     Then return an array of the image.
 
     :param path: Image path
     :param scale: Scale factor
     :return: Image array
     """
 
-    img = Image.open(str(path))
-
-    if img.mode == "CMYK":
-        logger.warning(f"Image {path} is in CMYK mode. Converting to RGB.")
-        img = img.convert("RGB")
+    img = cv2.imdecode(np.fromfile(str(path), dtype=np.uint8), cv2.IMREAD_COLOR)
 
     if scale != 1.0:
-        new_width = int(img.width * scale)
-        new_height = int(img.height * scale)
-        img = img.resize((new_width, new_height), Image.ANTIALIAS)
+        height, width, channels = img.shape
+        new_width = int(width * scale)
+        new_height = int(height * scale)
+        img = cv2.resize(img, (new_width, new_height))
 
-    return np.array(img)
+    return img
```

### Comparing `pcleaner-1.7.1/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner-1.7.2/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner-1.7.2/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/denoiser.py` & `pcleaner-1.7.2/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/CustomQ/CColorButton.py` & `pcleaner-1.7.2/pcleaner/gui/CustomQ/CColorButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-1.7.2/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,20 +80,31 @@
         Qw.QComboBox.clear(self)
         self._linked_data.clear()
 
     def addTextItemLinkedData(self, text: str, data: any):
         self.addItem(text)
         self._linked_data.append(data)
 
+    def setCurrentIndexByText(self, text: str):
+        self.setCurrentIndex(self.findText(text))
+
     def setCurrentIndexByLinkedData(self, data: any):
         self.setCurrentIndex(self._linked_data.index(data))
 
     def indexLinkedData(self, data: any):
         return self._linked_data.index(data)
 
+    @Slot(int)
+    def setCurrentIndex(self, index: int) -> None:
+        """
+        Ensure the index is valid.
+        :param index:
+        """
+        Qw.QComboBox.setCurrentIndex(self, min(max(index, 0), self.count() - 1))
+
     def currentLinkedData(self):
         try:
             return self._linked_data[self.currentIndex()]
         except IndexError:
             logger.error("No linked data found for current index")
             logger.error("Current index:", self.currentIndex())
             logger.error("Linked data:", self._linked_data)
```

### Comparing `pcleaner-1.7.1/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-1.7.2/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/file_table.py` & `pcleaner-1.7.2/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/gui_utils.py` & `pcleaner-1.7.2/pcleaner/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/launcher.py` & `pcleaner-1.7.2/pcleaner/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/mainwindow_driver.py` & `pcleaner-1.7.2/pcleaner/gui/mainwindow_driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from logzero import logger
 
 import pcleaner.cli_utils as cu
 import pcleaner.helpers as hp
 import pcleaner.config as cfg
 import pcleaner.gui.profile_parser as pp
 import pcleaner.gui.gui_utils as gu
+import pcleaner.profile_cli as pc
 from pcleaner.gui.ui_generated_files.ui_Mainwindow import Ui_MainWindow
 from pcleaner.gui.file_table import Column
 from pcleaner import __display_name__, __version__
 from pcleaner import data
 import pcleaner.gui.new_profile_driver as npd
 
 
@@ -61,15 +62,15 @@
         #
         # self.load_glossary()
 
     def initialize_ui(self):
         self.hide_progress()
         self.start_button_enabled(False)
         self.show_button_start()
-        self.update_input_buttons()
+        # self.update_input_buttons()
         self.set_up_statusbar()
         self.initialize_profiles()
         self.initialize_analytics_view()
 
         # Allow the table to accept file drops and hide the ID column.
         self.file_table.setAcceptDrops(True)
         self.file_table.setColumnHidden(Column.ID, True)
@@ -149,227 +150,227 @@
         Disconnect the combobox slots. This prevents erroneous signals from being sent during
         setup of new language options.
         """
         # self.comboBox_lang_from.currentIndexChanged.disconnect()
         # self.comboBox_lang_to.currentIndexChanged.disconnect()
         pass
 
-    """
-    Config interactions
-    """
-
-    def load_config_to_ui(self):
-        """
-        Apply data from config to ui widgets.
-        """
-        logger.debug("Loading config to UI.")
-
-        self.checkBox_file_fixed_dir.setChecked(self.config.use_fixed_output_path)
-        self.lineEdit_file_out_dir.setText(self.config.fixed_output_path)
-
-        self.lineEdit_glossary_file.setText(self.config.glossary_path)
-        self.checkBox_use_glossary.setChecked(self.config.use_glossary)
-        self.checkBox_extra_quote_protection.setChecked(self.config.use_quote_protection)
-
-        self.fixed_output_dir_enabled(self.config.use_fixed_output_path)
-        self.glossary_enabled(self.config.use_glossary)
-
-        # Ignore the mock because it cannot give language options. It is only to be used for translation.
-        translator = self.open_translator(use_mock=False)
-
-        self.show_api_status(translator is not None)
-        self.update_current_usage(translator)
-
-        if translator is not None:
-            # Disconnect the slots to prevent signals from being sent during setup of new language options.
-            self.disconnect_combobox_slots()  # vvv
-            # Load language options from API.
-            self.comboBox_lang_from.clear()
-            self.comboBox_lang_to.clear()
-
-            # Add automatic option.
-            self.comboBox_lang_from.addTextItemLinkedData("Detect", "")
-
-            for lang in translator.get_source_languages():
-                self.comboBox_lang_from.addTextItemLinkedData(lang.name, lang.code)
-
-            for lang in translator.get_target_languages():
-                self.comboBox_lang_to.addTextItemLinkedData(lang.name, lang.code)
-
-            self.connect_combobox_slots()  # ^^^
-
-            # Try to select the configured languages.
-            try:
-                self.comboBox_lang_from.setCurrentIndexByLinkedData(self.config.lang_from)
-            except ValueError:
-                logger.debug(f"Configured lang_from '{self.config.lang_from}' not found")
-
-            try:
-                self.comboBox_lang_to.setCurrentIndexByLinkedData(self.config.lang_to)
-            except ValueError:
-                logger.debug(f"Configured lang_to '{self.config.lang_to}' not found")
-        else:
-            self.statusbar.showMessage("Error connecting to the API.")
-
-    def lang_from_updated(self):
-        """
-        Copy lang_from from the combobox into the config and save it.
-        """
-        self.config.lang_from = self.comboBox_lang_from.currentLinkedData()
-        logger.debug(f"Saving lang_from: {self.config.lang_from}")
-        self.config.save()
-
-    def lang_to_updated(self):
-        """
-        Copy lang_to from the combobox into the config and save it.
-        """
-        self.config.lang_to = self.comboBox_lang_to.currentLinkedData()
-        logger.debug(f"Saving lang_to: {self.config.lang_to}")
-        self.text_output_changed.emit()
-        self.config.save()
-
-    def fixed_output_dir_toggled(self):
-        """
-        Enable or disable the fixed output directory checkbox and save it to the config.
-        """
-        self.config.use_fixed_output_path = self.checkBox_file_fixed_dir.isChecked()
-        self.fixed_output_dir_enabled(self.config.use_fixed_output_path)
-        self.text_output_changed.emit()
-        self.config.save()
-
-    def browse_file_out_dir(self):
-        """
-        Browse for a directory to save files to.
-        """
-        dir_path = Qw.QFileDialog.getExistingDirectory(
-            self, "Select output directory", self.config.fixed_output_path
-        )
-        if dir_path:
-            self.lineEdit_file_out_dir.setText(dir_path)
-            self.config.fixed_output_path = dir_path
-            self.text_output_changed.emit()
-            self.config.save()
-
-    def fixed_file_out_updated(self, save: bool, *_):
-        """
-        Copy fixed_file_out from the lineedit into the config and save it.
-        Don't save until the line edit signals the end of editing.
-        Throw away the text in the line edit that the signal passes along by using *_.
-        This is because the signal for editing finished does not pass along the text,
-        making it unreliable.
-
-        :param save: Whether to save the config.
-        """
-        self.config.fixed_output_path = self.lineEdit_file_out_dir.text()
-        if save:
-            self.config.save()
-        self.text_output_changed.emit()
-
-    def use_glossary_toggled(self):
-        """
-        Enable or disable the glossary checkbox and save it to the config.
-        """
-        self.config.use_glossary = self.checkBox_use_glossary.isChecked()
-        self.glossary_enabled(self.config.use_glossary)
-        self.config.save()
-        if self.config.use_glossary:
-            self.load_glossary()
-        self.text_params_changed.emit(self.glossary)
-
-    def browse_glossary_file(self):
-        """
-        Browse for a glossary file.
-        Accepts whatever pyexcel can handle.
-        """
-        file_path = Qw.QFileDialog.getOpenFileName(
-            self, "Select glossary file", self.config.glossary_path
-        )
-        if file_path:
-            self.lineEdit_glossary_file.setText(file_path[0])
-            self.config.glossary_path = file_path[0]
-            self.config.save()
-            self.load_glossary()
-
-    def glossary_file_updated(self, save: bool, *_):
-        """
-        Copy glossary_file from the lineedit into the config and save it.
-        Don't save until the line edit signals the end of editing.
-        Throw away the text in the line edit that the signal passes along by using *_.
-        This is because the signal for editing finished does not pass along the text,
-        making it unreliable.
-
-        :param save: Whether to save the config.
-        """
-        self.config.glossary_path = self.lineEdit_glossary_file.text()
-        if save:
-            self.config.save()
-            self.load_glossary()
-
-    def extra_quote_protection_toggled(self):
-        """
-        Enable or disable the extra quote protection checkbox and save it to the config.
-        """
-        self.config.use_quote_protection = self.checkBox_extra_quote_protection.isChecked()
-        self.config.save()
-        self.text_params_changed.emit(self.glossary)
-
-    """
-    Dialogs
-    """
-
-    def configure_api(self):
-        """
-        Configure the DeepL API.
-        """
-        api_conf_dialog = ConfigureAccount(self, self.config)
-        response = api_conf_dialog.exec()
-        if response == Qw.QDialog.Accepted:
-            # Adopt changes from the dialog.
-            self.config.api_key = api_conf_dialog.lineEdit_api_key.text()
-            self.config.save()
-            self.load_config_to_ui()
-
-    """
-    Misc helpers
-    """
-
-    # def open_translator(self, use_mock: bool = True) -> deepl.Translator | None:
+    # """
+    # Config interactions
+    # """
+    #
+    # def load_config_to_ui(self):
     #     """
-    #     Open a translator instance.
+    #     Apply data from config to ui widgets.
+    #     """
+    #     logger.debug("Loading config to UI.")
+    #
+    #     self.checkBox_file_fixed_dir.setChecked(self.config.use_fixed_output_path)
+    #     self.lineEdit_file_out_dir.setText(self.config.fixed_output_path)
+    #
+    #     self.lineEdit_glossary_file.setText(self.config.glossary_path)
+    #     self.checkBox_use_glossary.setChecked(self.config.use_glossary)
+    #     self.checkBox_extra_quote_protection.setChecked(self.config.use_quote_protection)
+    #
+    #     self.fixed_output_dir_enabled(self.config.use_fixed_output_path)
+    #     self.glossary_enabled(self.config.use_glossary)
+    #
+    #     # Ignore the mock because it cannot give language options. It is only to be used for translation.
+    #     translator = self.open_translator(use_mock=False)
+    #
+    #     self.show_api_status(translator is not None)
+    #     self.update_current_usage(translator)
+    #
+    #     if translator is not None:
+    #         # Disconnect the slots to prevent signals from being sent during setup of new language options.
+    #         self.disconnect_combobox_slots()  # vvv
+    #         # Load language options from API.
+    #         self.comboBox_lang_from.clear()
+    #         self.comboBox_lang_to.clear()
+    #
+    #         # Add automatic option.
+    #         self.comboBox_lang_from.addTextItemLinkedData("Detect", "")
+    #
+    #         for lang in translator.get_source_languages():
+    #             self.comboBox_lang_from.addTextItemLinkedData(lang.name, lang.code)
     #
-    #     :return: translator instance and whether it was successful
+    #         for lang in translator.get_target_languages():
+    #             self.comboBox_lang_to.addTextItemLinkedData(lang.name, lang.code)
+    #
+    #         self.connect_combobox_slots()  # ^^^
+    #
+    #         # Try to select the configured languages.
+    #         try:
+    #             self.comboBox_lang_from.setCurrentIndexByLinkedData(self.config.lang_from)
+    #         except ValueError:
+    #             logger.debug(f"Configured lang_from '{self.config.lang_from}' not found")
+    #
+    #         try:
+    #             self.comboBox_lang_to.setCurrentIndexByLinkedData(self.config.lang_to)
+    #         except ValueError:
+    #             logger.debug(f"Configured lang_to '{self.config.lang_to}' not found")
+    #     else:
+    #         self.statusbar.showMessage("Error connecting to the API.")
+    #
+    # def lang_from_updated(self):
+    #     """
+    #     Copy lang_from from the combobox into the config and save it.
     #     """
+    #     self.config.lang_from = self.comboBox_lang_from.currentLinkedData()
+    #     logger.debug(f"Saving lang_from: {self.config.lang_from}")
+    #     self.config.save()
+    #
+    # def lang_to_updated(self):
+    #     """
+    #     Copy lang_to from the combobox into the config and save it.
+    #     """
+    #     self.config.lang_to = self.comboBox_lang_to.currentLinkedData()
+    #     logger.debug(f"Saving lang_to: {self.config.lang_to}")
+    #     self.text_output_changed.emit()
+    #     self.config.save()
+    #
+    # def fixed_output_dir_toggled(self):
+    #     """
+    #     Enable or disable the fixed output directory checkbox and save it to the config.
+    #     """
+    #     self.config.use_fixed_output_path = self.checkBox_file_fixed_dir.isChecked()
+    #     self.fixed_output_dir_enabled(self.config.use_fixed_output_path)
+    #     self.text_output_changed.emit()
+    #     self.config.save()
+    #
+    # def browse_file_out_dir(self):
+    #     """
+    #     Browse for a directory to save files to.
+    #     """
+    #     dir_path = Qw.QFileDialog.getExistingDirectory(
+    #         self, "Select output directory", self.config.fixed_output_path
+    #     )
+    #     if dir_path:
+    #         self.lineEdit_file_out_dir.setText(dir_path)
+    #         self.config.fixed_output_path = dir_path
+    #         self.text_output_changed.emit()
+    #         self.config.save()
+    #
+    # def fixed_file_out_updated(self, save: bool, *_):
+    #     """
+    #     Copy fixed_file_out from the lineedit into the config and save it.
+    #     Don't save until the line edit signals the end of editing.
+    #     Throw away the text in the line edit that the signal passes along by using *_.
+    #     This is because the signal for editing finished does not pass along the text,
+    #     making it unreliable.
+    #
+    #     :param save: Whether to save the config.
+    #     """
+    #     self.config.fixed_output_path = self.lineEdit_file_out_dir.text()
+    #     if save:
+    #         self.config.save()
+    #     self.text_output_changed.emit()
+    #
+    # def use_glossary_toggled(self):
+    #     """
+    #     Enable or disable the glossary checkbox and save it to the config.
+    #     """
+    #     self.config.use_glossary = self.checkBox_use_glossary.isChecked()
+    #     self.glossary_enabled(self.config.use_glossary)
+    #     self.config.save()
+    #     if self.config.use_glossary:
+    #         self.load_glossary()
+    #     self.text_params_changed.emit(self.glossary)
+    #
+    # def browse_glossary_file(self):
+    #     """
+    #     Browse for a glossary file.
+    #     Accepts whatever pyexcel can handle.
+    #     """
+    #     file_path = Qw.QFileDialog.getOpenFileName(
+    #         self, "Select glossary file", self.config.glossary_path
+    #     )
+    #     if file_path:
+    #         self.lineEdit_glossary_file.setText(file_path[0])
+    #         self.config.glossary_path = file_path[0]
+    #         self.config.save()
+    #         self.load_glossary()
+    #
+    # def glossary_file_updated(self, save: bool, *_):
+    #     """
+    #     Copy glossary_file from the lineedit into the config and save it.
+    #     Don't save until the line edit signals the end of editing.
+    #     Throw away the text in the line edit that the signal passes along by using *_.
+    #     This is because the signal for editing finished does not pass along the text,
+    #     making it unreliable.
+    #
+    #     :param save: Whether to save the config.
+    #     """
+    #     self.config.glossary_path = self.lineEdit_glossary_file.text()
+    #     if save:
+    #         self.config.save()
+    #         self.load_glossary()
+    #
+    # def extra_quote_protection_toggled(self):
+    #     """
+    #     Enable or disable the extra quote protection checkbox and save it to the config.
+    #     """
+    #     self.config.use_quote_protection = self.checkBox_extra_quote_protection.isChecked()
+    #     self.config.save()
+    #     self.text_params_changed.emit(self.glossary)
+    #
+    # """
+    # Dialogs
+    # """
+    #
+    # def configure_api(self):
+    #     """
+    #     Configure the DeepL API.
+    #     """
+    #     api_conf_dialog = ConfigureAccount(self, self.config)
+    #     response = api_conf_dialog.exec()
+    #     if response == Qw.QDialog.Accepted:
+    #         # Adopt changes from the dialog.
+    #         self.config.api_key = api_conf_dialog.lineEdit_api_key.text()
+    #         self.config.save()
+    #         self.load_config_to_ui()
+    #
+    # """
+    # Misc helpers
+    # """
+    #
+    # # def open_translator(self, use_mock: bool = True) -> deepl.Translator | None:
+    # #     """
+    # #     Open a translator instance.
+    # #
+    # #     :return: translator instance and whether it was successful
+    # #     """
+    # #
+    # #     if self.config.api_key == "":
+    # #         # Fail silently if no API key is set, since this is the default value.
+    # #         logger.warning("No API key set")
+    # #         return None
+    # #     try:
+    # #         if self.config.tl_mock and use_mock:
+    # #             logger.info("Opening mock translator.")
+    # #             return deepl.Translator(
+    # #                 auth_key="1234567890",
+    # #                 server_url="http://localhost:3000",
+    # #             )
+    # #         else:
+    # #             logger.info("Opening translator.")
+    # #             translator = deepl.Translator(auth_key=self.config.api_key)
+    # #             # Test the api, since initialization doesn't mean success.
+    # #             translator.get_source_languages()
+    # #             return translator
+    # #     except Exception as e:
+    # #         show_warning(self, "API Error", f"Failed connect to DeepL API\n\n{e}")
+    # #         return None
+    #
+    # def update_file_table_params(self):
+    #     """
+    #     Update the file table with the current parameters.
+    #     """
+    #     self.text_params_changed.emit(self.glossary)
     #
-    #     if self.config.api_key == "":
-    #         # Fail silently if no API key is set, since this is the default value.
-    #         logger.warning("No API key set")
-    #         return None
-    #     try:
-    #         if self.config.tl_mock and use_mock:
-    #             logger.info("Opening mock translator.")
-    #             return deepl.Translator(
-    #                 auth_key="1234567890",
-    #                 server_url="http://localhost:3000",
-    #             )
-    #         else:
-    #             logger.info("Opening translator.")
-    #             translator = deepl.Translator(auth_key=self.config.api_key)
-    #             # Test the api, since initialization doesn't mean success.
-    #             translator.get_source_languages()
-    #             return translator
-    #     except Exception as e:
-    #         show_warning(self, "API Error", f"Failed connect to DeepL API\n\n{e}")
-    #         return None
-
-    def update_file_table_params(self):
-        """
-        Update the file table with the current parameters.
-        """
-        self.text_params_changed.emit(self.glossary)
-
     def initialize_analytics_view(self):
         """
         Set up the text edit for analytics.
         """
         # Set the font to monospace, using the included font.
         # The font is stored in the data module. Noto Mono is a free font.
         # Load it from file to be cross platform.
@@ -386,54 +387,164 @@
     Profiles
     """
 
     def initialize_profiles(self):
         """
         Load the available profiles and display the default profile.
         """
-        all_profiles: list[tuple[str, Path | None]] = [(cfg.RESERVED_PROFILE_NAMES[0], None)]
+        all_profiles: list[tuple[str, Path | None]] = [(cfg.DEFAULT_PROFILE_NAME, None)]
         for profile_name, profile_path in self.config.saved_profiles.items():
             all_profiles.append((profile_name, profile_path))
 
+        logger.debug(f"Found profiles: {all_profiles}")
+
         self.comboBox_current_profile.clear()
         for profile_name, profile_path in all_profiles:
             self.comboBox_current_profile.addTextItemLinkedData(profile_name, profile_path)
 
+        # Set the current profile to the default profile.
+        # If this is the default profile, then staying on the 0th index is fine.
+        if self.config.default_profile:
+            self.comboBox_current_profile.setCurrentIndexByText(self.config.default_profile)
+
+        # Populate default profile list.
+        self.menu_set_default_profile.clear()
+        for profile_name, profile_path in all_profiles:
+            action = Qg.QAction(profile_name, self)
+            action.setCheckable(True)
+            action.triggered.connect(partial(self.handle_set_default_profile, profile_name))
+            self.menu_set_default_profile.addAction(action)
+            action.setChecked(
+                profile_name
+                == (
+                    self.config.default_profile
+                    if self.config.default_profile
+                    else cfg.DEFAULT_PROFILE_NAME
+                )
+            )
+
         # Load the ProfileToolBox widget.
         self.toolBox_profile = pp.ProfileToolBox(self)
         inner_layout = Qw.QVBoxLayout()
         inner_layout.setContentsMargins(0, 0, 0, 0)
         inner_layout.addWidget(self.toolBox_profile)
         self.toolBox_profile_frame.setLayout(inner_layout)
-        self.config.load_profile(self.comboBox_current_profile.currentText())
+        self.config.load_profile(self.config.default_profile)
 
         # Load the structure.
         structure = pp.parse_profile_structure(self.config.current_profile)
         self.toolBox_profile.load_profile_structure(structure)
 
         self.load_current_profile()
         self.comboBox_current_profile.set_pre_change_hook(self.profile_change_check)
 
         # Connect signals.
         self.toolBox_profile.values_changed.connect(self.handle_profile_values_changed)
         self.pushButton_reset_profile.clicked.connect(self.reset_profile)
         self.pushButton_save_profile.clicked.connect(self.save_profile)
+        self.action_save_profile.triggered.connect(self.save_profile)
+        self.action_save_profile_as.triggered.connect(partial(self.save_profile, save_as=True))
+        self.action_import_profile.triggered.connect(self.import_profile)
+        self.action_new_profile.triggered.connect(partial(self.save_profile, make_new=True))
+        self.action_delete_profile.triggered.connect(self.delete_profile)
+
+    def handle_set_default_profile(self, profile_name: str):
+        """
+        Set the default profile in the config.
+        """
+        logger.debug(f"Setting default profile to {profile_name}")
+        self.config.default_profile = (
+            profile_name if profile_name != cfg.DEFAULT_PROFILE_NAME else None
+        )
+        self.config.save()
+        # Update the menu.
+        for action in self.menu_set_default_profile.actions():
+            action.setChecked(action.text() == profile_name)
+
+    def import_profile(self):
+        """
+        Open a file picker and add the profile to the profile list.
+        """
+        logger.debug("Importing profile.")
+        file_path = Qw.QFileDialog.getOpenFileName(
+            self,
+            "Import Profile",
+            "",
+            "Profile Files (*.conf)",
+        )[0]
+        if file_path:
+            logger.debug(f"Importing profile from {file_path}")
+            profile_name = Path(file_path).stem
+            success, msg = pc.add_profile(self.config, profile_name, file_path)
+            if success:
+                gu.show_info(self, "Profile Imported", msg)
+            else:
+                gu.show_warning(self, "Import Error", msg)
+                return
+
+            self.add_new_profile_to_gui(profile_name, file_path)
+
+    def delete_profile(self):
+        """
+        Ask and then delete the current profile.
+        Of course, the default profile cannot be deleted.
+        :return:
+        """
+        # if not self.profile_change_check():
+        #     return
+        logger.debug("Deleting profile.")
+        profile_name = self.comboBox_current_profile.currentText()
+
+        if self.comboBox_current_profile.currentText() == cfg.DEFAULT_PROFILE_NAME:
+            gu.show_warning(self, "Failed to Delete", "The default profile cannot be deleted.")
+            return
+        response = gu.show_question(
+            self, "Delete Profile", f"Are you sure you want to delete the profile {profile_name}?"
+        )
+        if response == Qw.QMessageBox.Yes:
+            profile_file = self.config.saved_profiles[profile_name]
+            self.config.remove_profile(profile_name)
+            self.config.save()
+            if profile_file.is_file():
+                try:
+                    profile_file.unlink()
+                except OSError as e:
+                    gu.show_warning(
+                        self, "Delete Error", "Failed to delete the profile\n" + e.what()
+                    )
+
+            self.toolBox_profile.reset_all()  # To suppress the change check.
+            self.comboBox_current_profile.removeItem(self.comboBox_current_profile.currentIndex())
+            for action in self.menu_set_default_profile.actions():
+                if action.text() == profile_name:
+                    self.menu_set_default_profile.removeAction(action)
+                    break
 
     def load_current_profile(self):
         """
         Load the current profile.
         """
         logger.debug("Loading current profile.")
         self.toolBox_profile.set_profile_values(self.config.current_profile)
 
     def profile_change_check(self) -> bool:
         """
         Check if the current profile has unsaved changes.
+
+        :return: True if the profile is ready to be changed, False otherwise.
         """
         logger.warning("Profile change check")
+        # Check if the profile is still in the list.
+        if self.comboBox_current_profile.currentText() not in list(
+            self.config.saved_profiles.keys()
+        ) + [cfg.DEFAULT_PROFILE_NAME]:
+            logger.debug("Profile not in list.")
+            # The profile is not in the list, so it must have been deleted.
+            return True
+
         if self.toolBox_profile.is_modified():
             logger.debug(
                 f"Previous profile {self.comboBox_current_profile.currentText()} has unsaved changes."
             )
             # Warn the user that he will lose unsaved changes.
             message = (
                 f"The profile '{self.comboBox_current_profile.currentText()}' has unsaved changes.\n"
@@ -465,85 +576,104 @@
         """
         Set the config option to match the current profile selector, then load it.
         """
         profile_name = self.comboBox_current_profile.currentText()
         self.config.load_profile(profile_name)
         self.load_current_profile()
 
-    @Slot(bool)
-    def handle_profile_values_changed(self, all_default: bool):
+    @Slot()
+    def handle_profile_values_changed(self):
         """
         Handle the profile values changing.
-
-        :param all_default: Whether all values are default now.
         """
-        self.pushButton_save_profile.setEnabled(not all_default)
-        self.pushButton_reset_profile.setEnabled(not all_default)
-        self.pushButton_apply_profile.setEnabled(not all_default)
+        dirty = self.toolBox_profile.is_modified()
+        self.pushButton_save_profile.setEnabled(dirty)
+        self.pushButton_reset_profile.setEnabled(dirty)
+        self.pushButton_apply_profile.setEnabled(dirty)
+        self.action_save_profile.setEnabled(dirty)
 
     def reset_profile(self):
         """
         Reset the current profile.
         """
         self.toolBox_profile.reset_all()
-        self.handle_profile_values_changed(True)
+        self.handle_profile_values_changed()
 
-    def save_profile(self, save_as: bool = False):
+    def save_profile(self, save_as: bool = False, make_new: bool = False):
         """
         Save the current profile.
 
         :param save_as: Whether to save as a new profile.
+        :param make_new: Whether to make a new profile.
         """
         # Grab the path from the combobox's linked data. If it is none, this is the
         # default profile, so we need to save it as a new profile.
         profile_path = self.comboBox_current_profile.currentLinkedData()
         profile_name = self.comboBox_current_profile.currentText()
-        if profile_path is None:
+        if profile_path is None or make_new:
             save_as = True
 
-        if profile_path is None:
+        if profile_path is None and not make_new:
             # Trying to save over the default profile.
             profile_path, profile_name = self.get_new_profile_path(show_protection_hint=True)
         elif save_as:
             profile_path, profile_name = self.get_new_profile_path()
 
         # If the path is still none, the dialog was canceled.
         if profile_path is None:
             logger.info("User canceled profile save.")
             return
 
-        # Proceed to write the profile.
-        logger.info(f"Saving profile to {profile_path}")
-        self.toolBox_profile.get_profile_values(self.config.current_profile)
-        success = self.config.current_profile.write(profile_path)
-        if not success:
-            logger.error("Failed to save profile.")
-            self.statusbar.showMessage(f"Failed to save profile to {profile_path}")
-            gu.show_critical(self, "Save Error", "Failed to save profile.")
-            return
-
-        logger.info("Profile saved successfully.")
-        self.statusbar.showMessage(f"Profile saved to {profile_path}")
-        if save_as:
-            self.config.add_profile(profile_name, profile_path)
-            if not self.config.save():
-                logger.error("Failed to save config.")
-                self.statusbar.showMessage("Failed to save config.")
-                gu.show_critical(
-                    self,
-                    "Save Error",
-                    "Failed to save the new profile to the configuration file.",
-                )
+        if make_new:
+            success, msg = pc.new_profile(self.config, profile_name, profile_path)
+            if success:
+                gu.show_info(self, "Profile Created", msg)
+                self.add_new_profile_to_gui(profile_name, profile_path)
+            else:
+                gu.show_warning(self, "Create Error", msg)
                 return
-            # Add the new profile to the combobox.
-            self.comboBox_current_profile.addTextItemLinkedData(profile_name, profile_path)
-            self.comboBox_current_profile.setCurrentText(profile_name)
+        else:
+            # Proceed to write the profile.
+            logger.info(f"Saving profile to {profile_path}")
+            self.toolBox_profile.get_profile_values(self.config.current_profile)
+            success = self.config.current_profile.write(profile_path)
+            if not success:
+                logger.error("Failed to save profile.")
+                self.statusbar.showMessage(f"Failed to save profile to {profile_path}")
+                gu.show_critical(self, "Save Error", "Failed to save profile.")
+                return
+
+            logger.info("Profile saved successfully.")
+            self.statusbar.showMessage(f"Profile saved to {profile_path}")
+            if save_as:
+                self.config.add_profile(profile_name, profile_path)
+                if not self.config.save():
+                    logger.error("Failed to save config.")
+                    self.statusbar.showMessage("Failed to save config.")
+                    gu.show_critical(
+                        self,
+                        "Save Error",
+                        "Failed to save the new profile to the configuration file.",
+                    )
+                    return
+                # Add the new profile to the combobox.
+                self.add_new_profile_to_gui(profile_name, profile_path)
+
         self.config.load_profile(profile_name)
         self.load_current_profile()
-        self.handle_profile_values_changed(True)
+        self.handle_profile_values_changed()
+
+    def add_new_profile_to_gui(self, profile_name: str, profile_path: Path):
+        self.comboBox_current_profile.addTextItemLinkedData(profile_name, profile_path)
+        self.comboBox_current_profile.setCurrentIndexByLinkedData(profile_path)
+        self.menu_set_default_profile.addAction(profile_name)
+        self.menu_set_default_profile.actions()[-1].triggered.connect(
+            partial(self.handle_set_default_profile, profile_name)
+        )
+        self.menu_set_default_profile.actions()[-1].setCheckable(True)
 
     def get_new_profile_path(
         self, show_protection_hint: bool = False
     ) -> tuple[Path, str] | tuple[None, None]:
         """
         Open a save dialog to save the current profile.
 
@@ -919,24 +1049,24 @@
 
     def show_api_status(self, good: bool):
         self.label_api_status_good.setVisible(good)
         self.label_api_status_good_icon.setVisible(good)
         self.label_api_status_bad.setVisible(not good)
         self.label_api_status_bad_icon.setVisible(not good)
 
-    def update_input_buttons(self):
-        logger.debug("Updating input buttons")
-
-        if self.processing:
-            self.action_Open_Files.setEnabled(False)
-            self.action_Clear_Files.setEnabled(False)
-        else:
-            self.action_Open_Files.setEnabled(True)
-            self.action_Clear_Files.setEnabled(self.file_table.rowCount() > 0)
-
+    # def update_input_buttons(self):
+    #     logger.debug("Updating input buttons")
+    #
+    #     if self.processing:
+    #         self.action_Open_Files.setEnabled(False)
+    #         self.action_Clear_Files.setEnabled(False)
+    #     else:
+    #         self.action_Open_Files.setEnabled(True)
+    #         self.action_Clear_Files.setEnabled(self.file_table.rowCount() > 0)
+    #
     # def update_current_usage(self, translator: deepl.Translator | None):
     #     if translator is None:
     #         self.label_api_usage.setText("—")
     #         self.label_api_usage_warn_icon.hide()
     #         self.label_api_usage_error_icon.hide()
     #         return
     #
```

### Comparing `pcleaner-1.7.1/pcleaner/gui/new_profile_driver.py` & `pcleaner-1.7.2/pcleaner/gui/new_profile_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/profile_parser.py` & `pcleaner-1.7.2/pcleaner/gui/profile_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,16 @@
                 self._data_widget.setMinimum(1)
             self._data_widget.valueChanged.connect(self._value_changed)
 
         elif entry_type == EntryTypes.Float or entry_type == EntryTypes.FloatGreater0:
             self._data_widget: qw.QDoubleSpinBox = qw.QDoubleSpinBox()
             self._data_widget.setStepType(qw.QAbstractSpinBox.AdaptiveDecimalStepType)
             self._data_setter = self._data_widget.setValue
-            self._data_getter = self._data_widget.value
+            # Round to 2 decimal places.
+            self._data_getter = lambda: round(self._data_widget.value(), 2)
             if entry_type == EntryTypes.FloatGreater0:
                 self._data_widget.setMinimum(0.01)
             self._data_widget.valueChanged.connect(self._value_changed)
 
         elif entry_type == EntryTypes.Str:
             self._data_widget: qw.QLineEdit = qw.QLineEdit()
             self._data_widget.textChanged.connect(self._value_changed)
@@ -292,15 +293,15 @@
 
 
 class ProfileToolBox(qw.QToolBox):
 
     # A subclass that tracks the mapping of widgets to profile options.
     # This is used to save/load the values of the widgets to the profile.
 
-    values_changed = qc.Signal(bool)  # When False, all values are default.
+    values_changed = qc.Signal()  # When False, all values are default.
     values_initialized: bool = (
         False  # This prevents lookups to the default values before they are set.
     )
 
     def __init__(self, parent=None):
         qw.QToolBox.__init__(self, parent)
         self._widgets: dict[str, dict[str, ProfileOptionWidget]] = {}
@@ -377,18 +378,15 @@
     def _on_value_changed(self) -> None:
         """
         Check if all values are default, then re-emit the signal.
         """
         if not self.values_initialized:
             return
 
-        all_values_default = all(
-            w.value_is_default() for section in self._widgets.values() for w in section.values()
-        )
-        self.values_changed.emit(all_values_default)
+        self.values_changed.emit()
 
     def reset_all(self) -> None:
         """
         Reset all widgets to their default values.
         """
         for section in self._widgets.values():
             for widget in section.values():
```

### Comparing `pcleaner-1.7.1/pcleaner/gui/rc_generated_files/icons_rc.py` & `pcleaner-1.7.2/pcleaner/gui/rc_generated_files/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/rc_generated_files/theme_icons_rc.py` & `pcleaner-1.7.2/pcleaner/gui/rc_generated_files/theme_icons_rc.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-1.7.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-1.7.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,48 +28,62 @@
 from pcleaner.gui.file_table import FileTable
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
         MainWindow.resize(1701, 720)
-        self.action_Open_Files = QAction(MainWindow)
-        self.action_Open_Files.setObjectName(u"action_Open_Files")
-        self.action_Clear_Files = QAction(MainWindow)
-        self.action_Clear_Files.setObjectName(u"action_Clear_Files")
-        self.action_New_Profile_2 = QAction(MainWindow)
-        self.action_New_Profile_2.setObjectName(u"action_New_Profile_2")
-        self.action_Delete_Profile = QAction(MainWindow)
-        self.action_Delete_Profile.setObjectName(u"action_Delete_Profile")
-        self.action_Import_Profile = QAction(MainWindow)
-        self.action_Import_Profile.setObjectName(u"action_Import_Profile")
-        self.action_Open_Log = QAction(MainWindow)
-        self.action_Open_Log.setObjectName(u"action_Open_Log")
-        self.action_Panel_Cleaner_Documentation = QAction(MainWindow)
-        self.action_Panel_Cleaner_Documentation.setObjectName(u"action_Panel_Cleaner_Documentation")
-        self.action_Source_Code = QAction(MainWindow)
-        self.action_Source_Code.setObjectName(u"action_Source_Code")
+        self.action_open_files = QAction(MainWindow)
+        self.action_open_files.setObjectName(u"action_open_files")
+        icon = QIcon(QIcon.fromTheme(u"document-open"))
+        self.action_open_files.setIcon(icon)
+        self.action_clear_files = QAction(MainWindow)
+        self.action_clear_files.setObjectName(u"action_clear_files")
+        icon1 = QIcon(QIcon.fromTheme(u"edit-clear-history"))
+        self.action_clear_files.setIcon(icon1)
+        self.action_new_profile = QAction(MainWindow)
+        self.action_new_profile.setObjectName(u"action_new_profile")
+        icon2 = QIcon(QIcon.fromTheme(u"document-new"))
+        self.action_new_profile.setIcon(icon2)
+        self.action_delete_profile = QAction(MainWindow)
+        self.action_delete_profile.setObjectName(u"action_delete_profile")
+        icon3 = QIcon(QIcon.fromTheme(u"edit-delete"))
+        self.action_delete_profile.setIcon(icon3)
+        self.action_import_profile = QAction(MainWindow)
+        self.action_import_profile.setObjectName(u"action_import_profile")
+        icon4 = QIcon(QIcon.fromTheme(u"document-import"))
+        self.action_import_profile.setIcon(icon4)
+        self.action_open_log = QAction(MainWindow)
+        self.action_open_log.setObjectName(u"action_open_log")
+        self.action_panel_cleaner_documentation = QAction(MainWindow)
+        self.action_panel_cleaner_documentation.setObjectName(u"action_panel_cleaner_documentation")
+        self.action_source_code = QAction(MainWindow)
+        self.action_source_code.setObjectName(u"action_source_code")
         self.actionView_License = QAction(MainWindow)
         self.actionView_License.setObjectName(u"actionView_License")
-        self.action_Save = QAction(MainWindow)
-        self.action_Save.setObjectName(u"action_Save")
-        self.action_Save_as = QAction(MainWindow)
-        self.action_Save_as.setObjectName(u"action_Save_as")
+        self.action_save_profile = QAction(MainWindow)
+        self.action_save_profile.setObjectName(u"action_save_profile")
+        icon5 = QIcon(QIcon.fromTheme(u"document-save"))
+        self.action_save_profile.setIcon(icon5)
+        self.action_save_profile_as = QAction(MainWindow)
+        self.action_save_profile_as.setObjectName(u"action_save_profile_as")
+        icon6 = QIcon(QIcon.fromTheme(u"document-save-as"))
+        self.action_save_profile_as.setIcon(icon6)
         self.action_Apply_Denoising = QAction(MainWindow)
         self.action_Apply_Denoising.setObjectName(u"action_Apply_Denoising")
         self.action_Apply_Denoising.setCheckable(True)
         self.action_Apply_Denoising.setChecked(True)
-        self.actionShow_Terminal_Command = QAction(MainWindow)
-        self.actionShow_Terminal_Command.setObjectName(u"actionShow_Terminal_Command")
-        self.action_System_Theme = QAction(MainWindow)
-        self.action_System_Theme.setObjectName(u"action_System_Theme")
-        self.action_Dark = QAction(MainWindow)
-        self.action_Dark.setObjectName(u"action_Dark")
-        self.action_Light = QAction(MainWindow)
-        self.action_Light.setObjectName(u"action_Light")
+        self.action_show_terminal_command = QAction(MainWindow)
+        self.action_show_terminal_command.setObjectName(u"action_show_terminal_command")
+        self.action_system_theme = QAction(MainWindow)
+        self.action_system_theme.setObjectName(u"action_system_theme")
+        self.action_dark = QAction(MainWindow)
+        self.action_dark.setObjectName(u"action_dark")
+        self.action_light = QAction(MainWindow)
+        self.action_light.setObjectName(u"action_light")
         self.action_temp = QAction(MainWindow)
         self.action_temp.setObjectName(u"action_temp")
         self.action_temp_2 = QAction(MainWindow)
         self.action_temp_2.setObjectName(u"action_temp_2")
         self.centralwidget = QWidget(MainWindow)
         self.centralwidget.setObjectName(u"centralwidget")
         self.verticalLayout = QVBoxLayout(self.centralwidget)
@@ -96,50 +110,50 @@
         self.comboBox_current_profile.setMinimumSize(QSize(48, 0))
 
         self.horizontalLayout_2.addWidget(self.comboBox_current_profile)
 
         self.pushButton_save_profile = QPushButton(self.groupBox)
         self.pushButton_save_profile.setObjectName(u"pushButton_save_profile")
         self.pushButton_save_profile.setEnabled(False)
-        icon = QIcon()
+        icon7 = QIcon()
         iconThemeName = u"document-save"
         if QIcon.hasThemeIcon(iconThemeName):
-            icon = QIcon.fromTheme(iconThemeName)
+            icon7 = QIcon.fromTheme(iconThemeName)
         else:
-            icon.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
+            icon7.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
-        self.pushButton_save_profile.setIcon(icon)
+        self.pushButton_save_profile.setIcon(icon7)
 
         self.horizontalLayout_2.addWidget(self.pushButton_save_profile)
 
         self.pushButton_reset_profile = QPushButton(self.groupBox)
         self.pushButton_reset_profile.setObjectName(u"pushButton_reset_profile")
         self.pushButton_reset_profile.setEnabled(False)
-        icon1 = QIcon()
+        icon8 = QIcon()
         iconThemeName = u"document-revert"
         if QIcon.hasThemeIcon(iconThemeName):
-            icon1 = QIcon.fromTheme(iconThemeName)
+            icon8 = QIcon.fromTheme(iconThemeName)
         else:
-            icon1.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
+            icon8.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
-        self.pushButton_reset_profile.setIcon(icon1)
+        self.pushButton_reset_profile.setIcon(icon8)
 
         self.horizontalLayout_2.addWidget(self.pushButton_reset_profile)
 
         self.pushButton_apply_profile = QPushButton(self.groupBox)
         self.pushButton_apply_profile.setObjectName(u"pushButton_apply_profile")
         self.pushButton_apply_profile.setEnabled(False)
-        icon2 = QIcon()
+        icon9 = QIcon()
         iconThemeName = u"dialog-ok-apply"
         if QIcon.hasThemeIcon(iconThemeName):
-            icon2 = QIcon.fromTheme(iconThemeName)
+            icon9 = QIcon.fromTheme(iconThemeName)
         else:
-            icon2.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
+            icon9.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
-        self.pushButton_apply_profile.setIcon(icon2)
+        self.pushButton_apply_profile.setIcon(icon9)
 
         self.horizontalLayout_2.addWidget(self.pushButton_apply_profile)
 
 
         self.verticalLayout_2.addLayout(self.horizontalLayout_2)
 
         self.toolBox_profile_frame = QWidget(self.groupBox)
@@ -227,35 +241,35 @@
         sizePolicy2.setHeightForWidth(self.label_warning.sizePolicy().hasHeightForWidth())
         self.label_warning.setSizePolicy(sizePolicy2)
 
         self.verticalLayout_7.addWidget(self.label_warning)
 
         self.pushButton_start = QPushButton(self.groupBox_4)
         self.pushButton_start.setObjectName(u"pushButton_start")
-        icon3 = QIcon()
+        icon10 = QIcon()
         iconThemeName = u"media-playback-start"
         if QIcon.hasThemeIcon(iconThemeName):
-            icon3 = QIcon.fromTheme(iconThemeName)
+            icon10 = QIcon.fromTheme(iconThemeName)
         else:
-            icon3.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
+            icon10.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
-        self.pushButton_start.setIcon(icon3)
+        self.pushButton_start.setIcon(icon10)
 
         self.verticalLayout_7.addWidget(self.pushButton_start)
 
         self.pushButton_abort = QPushButton(self.groupBox_4)
         self.pushButton_abort.setObjectName(u"pushButton_abort")
-        icon4 = QIcon()
+        icon11 = QIcon()
         iconThemeName = u"process-stop"
         if QIcon.hasThemeIcon(iconThemeName):
-            icon4 = QIcon.fromTheme(iconThemeName)
+            icon11 = QIcon.fromTheme(iconThemeName)
         else:
-            icon4.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
+            icon11.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
-        self.pushButton_abort.setIcon(icon4)
+        self.pushButton_abort.setIcon(icon11)
 
         self.verticalLayout_7.addWidget(self.pushButton_abort)
 
 
         self.verticalLayout_9.addLayout(self.verticalLayout_7)
 
 
@@ -297,22 +311,22 @@
         self.lineEdit_out_directory = QLineEdit(self.groupBox_3)
         self.lineEdit_out_directory.setObjectName(u"lineEdit_out_directory")
 
         self.horizontalLayout.addWidget(self.lineEdit_out_directory)
 
         self.pushButton_browse_out_dir = QPushButton(self.groupBox_3)
         self.pushButton_browse_out_dir.setObjectName(u"pushButton_browse_out_dir")
-        icon5 = QIcon()
+        icon12 = QIcon()
         iconThemeName = u"document-open-folder"
         if QIcon.hasThemeIcon(iconThemeName):
-            icon5 = QIcon.fromTheme(iconThemeName)
+            icon12 = QIcon.fromTheme(iconThemeName)
         else:
-            icon5.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
+            icon12.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
-        self.pushButton_browse_out_dir.setIcon(icon5)
+        self.pushButton_browse_out_dir.setIcon(icon12)
 
         self.horizontalLayout.addWidget(self.pushButton_browse_out_dir)
 
 
         self.verticalLayout_5.addLayout(self.horizontalLayout)
 
 
@@ -373,85 +387,80 @@
         self.menubar = QMenuBar(MainWindow)
         self.menubar.setObjectName(u"menubar")
         self.menubar.setGeometry(QRect(0, 0, 1701, 34))
         self.menu_File = QMenu(self.menubar)
         self.menu_File.setObjectName(u"menu_File")
         self.menu_Profile = QMenu(self.menubar)
         self.menu_Profile.setObjectName(u"menu_Profile")
-        self.menuCurrent_Profile = QMenu(self.menu_Profile)
-        self.menuCurrent_Profile.setObjectName(u"menuCurrent_Profile")
-        self.menuSet_Default = QMenu(self.menu_Profile)
-        self.menuSet_Default.setObjectName(u"menuSet_Default")
-        self.menu_Settings = QMenu(self.menubar)
-        self.menu_Settings.setObjectName(u"menu_Settings")
-        self.menu_Theme = QMenu(self.menu_Settings)
-        self.menu_Theme.setObjectName(u"menu_Theme")
+        self.menu_set_default_profile = QMenu(self.menu_Profile)
+        self.menu_set_default_profile.setObjectName(u"menu_set_default_profile")
+        self.menu_settings = QMenu(self.menubar)
+        self.menu_settings.setObjectName(u"menu_settings")
+        self.menu_theme = QMenu(self.menu_settings)
+        self.menu_theme.setObjectName(u"menu_theme")
         self.menu_Help = QMenu(self.menubar)
         self.menu_Help.setObjectName(u"menu_Help")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QStatusBar(MainWindow)
         self.statusbar.setObjectName(u"statusbar")
         MainWindow.setStatusBar(self.statusbar)
 #if QT_CONFIG(shortcut)
         self.label_4.setBuddy(self.lineEdit_out_directory)
 #endif // QT_CONFIG(shortcut)
 
         self.menubar.addAction(self.menu_File.menuAction())
         self.menubar.addAction(self.menu_Profile.menuAction())
-        self.menubar.addAction(self.menu_Settings.menuAction())
+        self.menubar.addAction(self.menu_settings.menuAction())
         self.menubar.addAction(self.menu_Help.menuAction())
-        self.menu_File.addAction(self.action_Open_Files)
-        self.menu_File.addAction(self.action_Clear_Files)
-        self.menu_Profile.addAction(self.menuCurrent_Profile.menuAction())
+        self.menu_File.addAction(self.action_open_files)
+        self.menu_File.addAction(self.action_clear_files)
+        self.menu_Profile.addAction(self.action_new_profile)
+        self.menu_Profile.addAction(self.action_import_profile)
         self.menu_Profile.addSeparator()
-        self.menu_Profile.addAction(self.action_New_Profile_2)
-        self.menu_Profile.addAction(self.action_Import_Profile)
+        self.menu_Profile.addAction(self.action_save_profile)
+        self.menu_Profile.addAction(self.action_save_profile_as)
         self.menu_Profile.addSeparator()
-        self.menu_Profile.addAction(self.action_Save)
-        self.menu_Profile.addAction(self.action_Save_as)
+        self.menu_Profile.addAction(self.action_delete_profile)
         self.menu_Profile.addSeparator()
-        self.menu_Profile.addAction(self.action_Delete_Profile)
-        self.menu_Profile.addSeparator()
-        self.menu_Profile.addAction(self.menuSet_Default.menuAction())
-        self.menuCurrent_Profile.addAction(self.action_temp)
-        self.menuSet_Default.addAction(self.action_temp_2)
-        self.menu_Settings.addAction(self.menu_Theme.menuAction())
-        self.menu_Settings.addAction(self.action_Open_Log)
-        self.menu_Theme.addAction(self.action_System_Theme)
-        self.menu_Theme.addSeparator()
-        self.menu_Theme.addAction(self.action_Dark)
-        self.menu_Theme.addAction(self.action_Light)
-        self.menu_Help.addAction(self.action_Panel_Cleaner_Documentation)
-        self.menu_Help.addAction(self.action_Source_Code)
+        self.menu_Profile.addAction(self.menu_set_default_profile.menuAction())
+        self.menu_set_default_profile.addAction(self.action_temp_2)
+        self.menu_settings.addAction(self.menu_theme.menuAction())
+        self.menu_settings.addAction(self.action_open_log)
+        self.menu_theme.addAction(self.action_system_theme)
+        self.menu_theme.addSeparator()
+        self.menu_theme.addAction(self.action_dark)
+        self.menu_theme.addAction(self.action_light)
+        self.menu_Help.addAction(self.action_panel_cleaner_documentation)
+        self.menu_Help.addAction(self.action_source_code)
         self.menu_Help.addSeparator()
-        self.menu_Help.addAction(self.actionShow_Terminal_Command)
+        self.menu_Help.addAction(self.action_show_terminal_command)
 
         self.retranslateUi(MainWindow)
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
         MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"Panel Cleaner", None))
-        self.action_Open_Files.setText(QCoreApplication.translate("MainWindow", u"Open Files", None))
-        self.action_Clear_Files.setText(QCoreApplication.translate("MainWindow", u"Clear Files", None))
-        self.action_New_Profile_2.setText(QCoreApplication.translate("MainWindow", u"New", None))
-        self.action_Delete_Profile.setText(QCoreApplication.translate("MainWindow", u"Delete", None))
-        self.action_Import_Profile.setText(QCoreApplication.translate("MainWindow", u"Import...", None))
-        self.action_Open_Log.setText(QCoreApplication.translate("MainWindow", u"Open Log", None))
-        self.action_Panel_Cleaner_Documentation.setText(QCoreApplication.translate("MainWindow", u"Online Documentation", None))
-        self.action_Source_Code.setText(QCoreApplication.translate("MainWindow", u"About Panel Cleaner", None))
+        self.action_open_files.setText(QCoreApplication.translate("MainWindow", u"Open Files", None))
+        self.action_clear_files.setText(QCoreApplication.translate("MainWindow", u"Clear Files", None))
+        self.action_new_profile.setText(QCoreApplication.translate("MainWindow", u"New", None))
+        self.action_delete_profile.setText(QCoreApplication.translate("MainWindow", u"Delete", None))
+        self.action_import_profile.setText(QCoreApplication.translate("MainWindow", u"Import...", None))
+        self.action_open_log.setText(QCoreApplication.translate("MainWindow", u"Open Log", None))
+        self.action_panel_cleaner_documentation.setText(QCoreApplication.translate("MainWindow", u"Online Documentation", None))
+        self.action_source_code.setText(QCoreApplication.translate("MainWindow", u"About Panel Cleaner", None))
         self.actionView_License.setText(QCoreApplication.translate("MainWindow", u"View License", None))
-        self.action_Save.setText(QCoreApplication.translate("MainWindow", u"Save", None))
-        self.action_Save_as.setText(QCoreApplication.translate("MainWindow", u"Save as...", None))
+        self.action_save_profile.setText(QCoreApplication.translate("MainWindow", u"Save", None))
+        self.action_save_profile_as.setText(QCoreApplication.translate("MainWindow", u"Save as...", None))
         self.action_Apply_Denoising.setText(QCoreApplication.translate("MainWindow", u"Apply Denoising", None))
-        self.actionShow_Terminal_Command.setText(QCoreApplication.translate("MainWindow", u"Show Terminal Command", None))
-        self.action_System_Theme.setText(QCoreApplication.translate("MainWindow", u"System", None))
-        self.action_Dark.setText(QCoreApplication.translate("MainWindow", u"Dark", None))
-        self.action_Light.setText(QCoreApplication.translate("MainWindow", u"Light", None))
+        self.action_show_terminal_command.setText(QCoreApplication.translate("MainWindow", u"Show Terminal Command", None))
+        self.action_system_theme.setText(QCoreApplication.translate("MainWindow", u"System", None))
+        self.action_dark.setText(QCoreApplication.translate("MainWindow", u"Dark", None))
+        self.action_light.setText(QCoreApplication.translate("MainWindow", u"Light", None))
         self.action_temp.setText(QCoreApplication.translate("MainWindow", u"<temp>", None))
         self.action_temp_2.setText(QCoreApplication.translate("MainWindow", u"<temp>", None))
         self.groupBox.setTitle(QCoreApplication.translate("MainWindow", u"Profile", None))
         self.comboBox_current_profile.setItemText(0, QCoreApplication.translate("MainWindow", u"Default", None))
 
         self.pushButton_save_profile.setText(QCoreApplication.translate("MainWindow", u"Save", None))
         self.pushButton_reset_profile.setText(QCoreApplication.translate("MainWindow", u"Reset All", None))
@@ -487,14 +496,13 @@
                         ": <br />Mask 0  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 1  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 2  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 3  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 4  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 5  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 6  : </span><span style=\" font-family:'Noto Mono','"
                         "Monospace'; color:#18b2b2;\">\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588</span><span style=\" font-family:'Noto Mono','Monospace';\"> </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">1</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 1 <br />Mask 7  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 8  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 9  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 10 :  </span><span style=\" font-family:'Noto Mono','Monospa"
                         "ce'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Box mask: </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588</span><span style=\" font-family:'Noto Mono','Monospace';\"> </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">4</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 4 <br /><br /></span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">\u2588 Perfect</span><span style=\" font-family:'Noto Mono','Monospace';\"> | \u2588 Total<br /><br /></span></p></body></html>", None))
         self.label_progress_step.setText(QCoreApplication.translate("MainWindow", u"Current Step:", None))
         self.label_2.setText(QCoreApplication.translate("MainWindow", u"Total Progress:", None))
         self.menu_File.setTitle(QCoreApplication.translate("MainWindow", u"File", None))
         self.menu_Profile.setTitle(QCoreApplication.translate("MainWindow", u"Profile", None))
-        self.menuCurrent_Profile.setTitle(QCoreApplication.translate("MainWindow", u"Current Profile", None))
-        self.menuSet_Default.setTitle(QCoreApplication.translate("MainWindow", u"Set Default", None))
-        self.menu_Settings.setTitle(QCoreApplication.translate("MainWindow", u"Settings", None))
-        self.menu_Theme.setTitle(QCoreApplication.translate("MainWindow", u"Theme", None))
+        self.menu_set_default_profile.setTitle(QCoreApplication.translate("MainWindow", u"Set Default", None))
+        self.menu_settings.setTitle(QCoreApplication.translate("MainWindow", u"Settings", None))
+        self.menu_theme.setTitle(QCoreApplication.translate("MainWindow", u"Theme", None))
         self.menu_Help.setTitle(QCoreApplication.translate("MainWindow", u"Help", None))
     # retranslateUi
```

### Comparing `pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py` & `pcleaner-1.7.2/pcleaner/gui/ui_generated_files/ui_NewProfile.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/gui/worker_thread.py` & `pcleaner-1.7.2/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/helpers.py` & `pcleaner-1.7.2/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/image_ops.py` & `pcleaner-1.7.2/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/main.py` & `pcleaner-1.7.2/pcleaner/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,17 +159,19 @@
     if args.profile:
         # Handle profile subcommands.
         config = cfg.load_config()
 
         if args.list:
             pc.list_profiles(config)
         elif args.new:
-            pc.new_profile(config, args.profile_name, args.profile_path)
+            _, msg = pc.new_profile(config, args.profile_name, args.profile_path, cli_mode=True)
+            print(msg)
         elif args.add:
-            pc.add_profile(config, args.profile_name, args.profile_path)
+            _, msg = pc.add_profile(config, args.profile_name, args.profile_path)
+            print(msg)
         elif args.open:
             pc.open_profile(config, args.profile_name)
         elif args.delete:
             pc.delete_profile(config, args.profile_name)
         elif args.set_default:
             pc.set_default_profile(config, args.profile_name)
         elif args.repair:
```

### Comparing `pcleaner-1.7.1/pcleaner/masker.py` & `pcleaner-1.7.2/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/model_downloader.py` & `pcleaner-1.7.2/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/pre_processor.py` & `pcleaner-1.7.2/pcleaner/pre_processor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner/profile_cli.py` & `pcleaner-1.7.2/pcleaner/profile_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,75 +51,84 @@
     for profile_name, profile_path in config.saved_profiles.items():
         table.add_row(
             [profile_name, profile_path, check_path(profile_path), check_default(profile_name)]
         )
     print(table)
 
 
-def new_profile(config: cfg.Config, profile_name: str, profile_path: str | None):
+def new_profile(
+    config: cfg.Config, profile_name: str, profile_path: str | None, cli_mode: bool = False
+) -> tuple[bool, str]:
     """
     Create a new profile with the given name and path.
 
     :param config: The config object.
     :param profile_name: The name of the profile.
     :param profile_path: The path to the profile.
+    :param cli_mode: Whether to ask to overwrite an existing file. Only applicable in CLI mode.
     """
-    if not is_valid_profile_name(config, profile_name):
-        return
+    valid, msg = is_valid_profile_name(config, profile_name)
+    if not valid:
+        return False, msg
 
     # If no path is given, use the default path.
     if profile_path is None:
         profile_path = cli.get_default_profile_path(profile_name)
     else:
         profile_path = Path(profile_path)
         # If the path is a directory, append a default filename.
         if profile_path.is_dir():
             profile_path = profile_path / f"{profile_name}.conf"
 
     # Check if overwriting an existing file.
     if profile_path.exists():
+        if not cli_mode:
+            return False, f"Profile file {profile_path} already exists."
         if not cli.get_confirmation(f"Overwrite existing file {profile_path}?"):
-            print("Aborting.")
-            return
+            return False, "Aborted."
 
     profile_path.parent.mkdir(parents=True, exist_ok=True)
     # Create the profile file from the built-in default.
     profile = cfg.Profile()
     profile.write(profile_path)
-    print(f"Profile {profile_name} created at {profile_path}.")
 
     # Add the profile to the config.
     config.add_profile(profile_name, profile_path)
     config.save()
 
-    open_profile(config, profile_name)
+    if cli_mode:
+        print(f"Profile {profile_name} created at {profile_path}.")
+        open_profile(config, profile_name)
+        return True, ""
 
+    return True, f"Profile {profile_name} created."
 
-def add_profile(config: cfg.Config, profile_name: str, profile_path: str):
+
+def add_profile(config: cfg.Config, profile_name: str, profile_path: str) -> tuple[bool, str]:
     """
     Add a profile to the config.
 
     :param config: The config object.
     :param profile_name: The name of the profile.
     :param profile_path: The path to the profile file.
     """
-    if not is_valid_profile_name(config, profile_name):
-        return
+    valid, msg = is_valid_profile_name(config, profile_name)
+    if not valid:
+        return False, msg
 
     # Verify the profile path exists.
     profile_path = Path(profile_path)
     if not profile_path.is_file():
-        print("Profile file not found.")
-        return
+        return False, "Profile file not found."
 
     # Add the profile to the config.
     config.add_profile(profile_name, profile_path)
     config.save()
 
-    print(f"Profile {profile_name} added.")
+    return True, f"Profile {profile_name} added."
 
 
 def open_profile(config: cfg.Config, profile_name: str):
     """
     Open the profile in the default editor, unless specified in the config.
 
     :param config: The config object.
@@ -207,34 +216,31 @@
 
     profile.write(profile_path)
     print(f"Profile {closest_match} repaired.")
 
 
 def is_valid_profile_name(
     config: cfg.Config, profile_name: str, allow_reserved: bool = False
-) -> bool:
+) -> tuple[bool, str]:
     """
     Verify the profile name isn't empty or already in use.
     Normally reject reserved names, but allow them if specified.
 
     :param config: The config object.
     :param profile_name: The name of the profile.
     :param allow_reserved: Allow reserved names.
-    :return: True if valid, False otherwise.
+    :return: True if valid, False otherwise, and a message.
     """
     if not profile_name:
-        print("Profile name cannot be empty.")
-        return False
+        return False, "Profile name cannot be empty."
     if profile_name in config.saved_profiles.keys():
-        print("Profile name already in use.")
-        return False
+        return False, "Profile name already in use."
     if profile_name.lower() in cfg.RESERVED_PROFILE_NAMES and not allow_reserved:
-        print("Profile name is reserved.")
-        return False
-    return True
+        return False, "Profile name is reserved."
+    return True, ""
 
 
 def purge_missing_profiles(config: cfg.Config):
     """
     Remove profiles from the config that no longer exist.
 
     :param config: The config object.
```

### Comparing `pcleaner-1.7.1/pcleaner/structures.py` & `pcleaner-1.7.2/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.7.2/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.7.1
+Version: 1.7.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pcleaner-1.7.1/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.7.2/pcleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.1/setup.cfg` & `pcleaner-1.7.2/setup.cfg`

 * *Files identical despite different names*


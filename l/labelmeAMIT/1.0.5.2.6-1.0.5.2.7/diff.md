# Comparing `tmp/labelmeAMIT-1.0.5.2.6.tar.gz` & `tmp/labelmeAMIT-1.0.5.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelmeAMIT-1.0.5.2.6.tar", last modified: Thu Mar 23 07:15:57 2023, max compression
+gzip compressed data, was "labelmeAMIT-1.0.5.2.7.tar", last modified: Mon May  8 03:10:50 2023, max compression
```

## Comparing `labelmeAMIT-1.0.5.2.6.tar` & `labelmeAMIT-1.0.5.2.7.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.880187 labelmeAMIT-1.0.5.2.6/
--rw-rw-r--   0 amit      (1000) amit      (1000)      692 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/LICENSE
--rw-rw-r--   0 amit      (1000) amit      (1000)       18 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/MANIFEST.in
--rw-rw-r--   0 amit      (1000) amit      (1000)     9673 2023-03-23 07:15:57.880187 labelmeAMIT-1.0.5.2.6/PKG-INFO
--rw-rw-r--   0 amit      (1000) amit      (1000)     8749 2023-02-08 09:42:54.000000 labelmeAMIT-1.0.5.2.6/README.md
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.868187 labelmeAMIT-1.0.5.2.6/labelme/
--rw-rw-r--   0 amit      (1000) amit      (1000)      612 2023-03-23 07:13:00.000000 labelmeAMIT-1.0.5.2.6/labelme/__init__.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     6660 2023-02-13 03:17:11.000000 labelmeAMIT-1.0.5.2.6/labelme/__main__.py
--rw-rw-r--   0 amit      (1000) amit      (1000)    92152 2023-03-23 06:59:23.000000 labelmeAMIT-1.0.5.2.6/labelme/app.py
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.868187 labelmeAMIT-1.0.5.2.6/labelme/cli/
--rw-rw-r--   0 amit      (1000) amit      (1000)      123 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/cli/__init__.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     1345 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/cli/draw_json.py
--rw-rw-r--   0 amit      (1000) amit      (1000)      636 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/cli/draw_label_png.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     2388 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/cli/json_to_dataset.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     2749 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/cli/on_docker.py
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.868187 labelmeAMIT-1.0.5.2.6/labelme/config/
--rw-rw-r--   0 amit      (1000) amit      (1000)     2698 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/config/__init__.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     2341 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/config/default_config.yaml
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.880187 labelmeAMIT-1.0.5.2.6/labelme/icons/
--rw-rw-r--   0 amit      (1000) amit      (1000)     2136 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/cancel.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     3111 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/close.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     2368 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/color-line.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1461 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/color.png
--rw-rw-r--   0 amit      (1000) amit      (1000)      646 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/copy.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1486 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/delete.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     2198 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/done.png
--rw-rw-r--   0 amit      (1000) amit      (1000)    22232 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/done.svg
--rw-rw-r--   0 amit      (1000) amit      (1000)     1092 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/edit.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     7718 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/expert.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1264 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/eye.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     8059 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/feBlend-icon.png
--rw-rw-r--   0 amit      (1000) amit      (1000)      765 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/file.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1365 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/fit-width.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1102 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/fit-window.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     2262 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/fit.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1587 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/help.png
--rw-rw-r--   0 amit      (1000) amit      (1000)  1128131 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/icon.icns
--rw-rw-r--   0 amit      (1000) amit      (1000)   183198 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/icon.ico
--rw-rw-r--   0 amit      (1000) amit      (1000)    44771 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/icon.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     2381 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/labels.png
--rw-rw-r--   0 amit      (1000) amit      (1000)    36694 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/labels.svg
--rw-rw-r--   0 amit      (1000) amit      (1000)      977 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/new.png
--rw-rw-r--   0 amit      (1000) amit      (1000)    30288 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/next.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1103 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/objects.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     2073 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/open.png
--rw-rw-r--   0 amit      (1000) amit      (1000)    18197 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/open.svg
--rw-rw-r--   0 amit      (1000) amit      (1000)    30665 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/prev.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1915 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/quit.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     2811 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/save-as.png
--rw-rw-r--   0 amit      (1000) amit      (1000)    64005 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/save-as.svg
--rw-rw-r--   0 amit      (1000) amit      (1000)     1187 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/save.png
--rw-rw-r--   0 amit      (1000) amit      (1000)    30613 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/save.svg
--rw-rw-r--   0 amit      (1000) amit      (1000)     2004 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/undo-cross.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     2018 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/undo.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1099 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/zoom-in.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1074 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/zoom-out.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     1139 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/icons/zoom.png
--rw-rw-r--   0 amit      (1000) amit      (1000)     6354 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/label_file.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     1836 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/logger.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     9968 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/shape.py
--rw-rw-r--   0 amit      (1000) amit      (1000)      849 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/testing.py
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.880187 labelmeAMIT-1.0.5.2.6/labelme/utils/
--rw-rw-r--   0 amit      (1000) amit      (1000)      722 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/utils/__init__.py
--rw-rw-r--   0 amit      (1000) amit      (1000)      675 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/utils/_io.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     2367 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/utils/image.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     2392 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/utils/qt.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     3929 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/utils/shape.py
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.880187 labelmeAMIT-1.0.5.2.6/labelme/widgets/
--rw-rw-r--   0 amit      (1000) amit      (1000)      510 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/__init__.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     1468 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/brightness_contrast_dialog.py
--rw-rw-r--   0 amit      (1000) amit      (1000)    38300 2023-02-09 06:24:55.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/canvas.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     1200 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/color_dialog.py
--rw-rw-r--   0 amit      (1000) amit      (1000)      281 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/escapable_qlist_widget.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     2434 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/file_dialog_preview.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     8150 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/label_dialog.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     5792 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/label_list_widget.py
--rw-rw-r--   0 amit      (1000) amit      (1000)      970 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/tool_bar.py
--rw-rw-r--   0 amit      (1000) amit      (1000)     1374 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/unique_label_qlist_widget.py
--rw-rw-r--   0 amit      (1000) amit      (1000)      712 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/labelme/widgets/zoom_widget.py
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-03-23 07:15:57.880187 labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/
--rw-rw-r--   0 amit      (1000) amit      (1000)     9673 2023-03-23 07:15:57.000000 labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/PKG-INFO
--rw-rw-r--   0 amit      (1000) amit      (1000)     2008 2023-03-23 07:15:57.000000 labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/SOURCES.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)        1 2023-03-23 07:15:57.000000 labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/dependency_links.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)      260 2023-03-23 07:15:57.000000 labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/entry_points.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)       87 2023-03-23 07:15:57.000000 labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/requires.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)        8 2023-03-23 07:15:57.000000 labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/top_level.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)       38 2023-03-23 07:15:57.880187 labelmeAMIT-1.0.5.2.6/setup.cfg
--rw-rw-r--   0 amit      (1000) amit      (1000)     4537 2023-02-08 08:15:20.000000 labelmeAMIT-1.0.5.2.6/setup.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.449612 labelmeAMIT-1.0.5.2.7/
+-rw-rw-r--   0 amit      (1000) amit      (1000)      692 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/LICENSE
+-rw-rw-r--   0 amit      (1000) amit      (1000)       18 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/MANIFEST.in
+-rw-rw-r--   0 amit      (1000) amit      (1000)     9673 2023-05-08 03:10:50.449612 labelmeAMIT-1.0.5.2.7/PKG-INFO
+-rw-rw-r--   0 amit      (1000) amit      (1000)     8749 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/README.md
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.445612 labelmeAMIT-1.0.5.2.7/labelme/
+-rw-rw-r--   0 amit      (1000) amit      (1000)      612 2023-05-08 02:55:32.000000 labelmeAMIT-1.0.5.2.7/labelme/__init__.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     6660 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/__main__.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)   100617 2023-05-06 07:09:22.000000 labelmeAMIT-1.0.5.2.7/labelme/app.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.445612 labelmeAMIT-1.0.5.2.7/labelme/cli/
+-rw-rw-r--   0 amit      (1000) amit      (1000)      123 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/cli/__init__.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1345 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/cli/draw_json.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)      636 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/cli/draw_label_png.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2388 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/cli/json_to_dataset.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2749 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/cli/on_docker.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.445612 labelmeAMIT-1.0.5.2.7/labelme/config/
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2698 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/config/__init__.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2362 2023-04-27 11:51:17.000000 labelmeAMIT-1.0.5.2.7/labelme/config/default_config.yaml
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.449612 labelmeAMIT-1.0.5.2.7/labelme/icons/
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2136 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/cancel.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     3111 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/close.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2368 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/color-line.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1461 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/color.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)      646 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/copy.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1486 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/delete.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2198 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/done.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)    22232 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/done.svg
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1092 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/edit.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     7718 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/expert.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1264 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/eye.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     8059 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/feBlend-icon.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)      765 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/file.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1365 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/fit-width.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1102 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/fit-window.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2262 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/fit.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1587 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/help.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)  1128131 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/icon.icns
+-rw-rw-r--   0 amit      (1000) amit      (1000)   183198 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/icon.ico
+-rw-rw-r--   0 amit      (1000) amit      (1000)    44771 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/icon.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2381 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/labels.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)    36694 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/labels.svg
+-rw-rw-r--   0 amit      (1000) amit      (1000)      977 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/new.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)    30288 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/next.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1103 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/objects.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2073 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/open.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)    18197 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/open.svg
+-rw-rw-r--   0 amit      (1000) amit      (1000)    30665 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/prev.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1915 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/quit.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2811 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/save-as.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)    64005 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/save-as.svg
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1187 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/save.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)    30613 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/save.svg
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2004 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/undo-cross.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2018 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/undo.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1099 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/zoom-in.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1074 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/zoom-out.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1139 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/icons/zoom.png
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2475 2023-05-06 08:36:15.000000 labelmeAMIT-1.0.5.2.7/labelme/imageProcessing.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     6354 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/label_file.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1836 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/logger.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)    11224 2023-05-05 09:01:55.000000 labelmeAMIT-1.0.5.2.7/labelme/shape.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)      849 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/testing.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.449612 labelmeAMIT-1.0.5.2.7/labelme/utils/
+-rw-rw-r--   0 amit      (1000) amit      (1000)      722 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/utils/__init__.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)      675 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/utils/_io.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2367 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/utils/image.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2392 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/utils/qt.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     4092 2023-04-27 11:09:27.000000 labelmeAMIT-1.0.5.2.7/labelme/utils/shape.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.449612 labelmeAMIT-1.0.5.2.7/labelme/widgets/
+-rw-rw-r--   0 amit      (1000) amit      (1000)      510 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/__init__.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1468 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/brightness_contrast_dialog.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)    40930 2023-05-05 08:53:01.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/canvas.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1200 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/color_dialog.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)      281 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/escapable_qlist_widget.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2434 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/file_dialog_preview.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     8150 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/label_dialog.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     5792 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/label_list_widget.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)      970 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/tool_bar.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)     1374 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/unique_label_qlist_widget.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)      712 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/labelme/widgets/zoom_widget.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-05-08 03:10:50.449612 labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/
+-rw-rw-r--   0 amit      (1000) amit      (1000)     9673 2023-05-08 03:10:50.000000 labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/PKG-INFO
+-rw-rw-r--   0 amit      (1000) amit      (1000)     2035 2023-05-08 03:10:50.000000 labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/SOURCES.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)        1 2023-05-08 03:10:50.000000 labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/dependency_links.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)      260 2023-05-08 03:10:50.000000 labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/entry_points.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)       87 2023-05-08 03:10:50.000000 labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/requires.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)        8 2023-05-08 03:10:50.000000 labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/top_level.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)       38 2023-05-08 03:10:50.449612 labelmeAMIT-1.0.5.2.7/setup.cfg
+-rw-rw-r--   0 amit      (1000) amit      (1000)     4537 2023-04-27 08:56:39.000000 labelmeAMIT-1.0.5.2.7/setup.py
```

### Comparing `labelmeAMIT-1.0.5.2.6/LICENSE` & `labelmeAMIT-1.0.5.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/PKG-INFO` & `labelmeAMIT-1.0.5.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelmeAMIT
-Version: 1.0.5.2.6
+Version: 1.0.5.2.7
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada
 Author-email: www.kentaro.wada@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labelmeAMIT Version: 1.0.5.2.6 Summary: Image
+Metadata-Version: 2.1 Name: labelmeAMIT Version: 1.0.5.2.7 Summary: Image
 Polygonal Annotation with Python Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada Author-email: www.kentaro.wada@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `labelmeAMIT-1.0.5.2.6/README.md` & `labelmeAMIT-1.0.5.2.7/README.md`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/__init__.py` & `labelmeAMIT-1.0.5.2.7/labelme/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __appname__ = "labelmeAMIT"
 
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
-__version__ = "1.0.5.2.6"
+__version__ = "1.0.5.2.7"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
 
 PY2 = sys.version[0] == "2"
 PY3 = sys.version[0] == "3"
```

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/__main__.py` & `labelmeAMIT-1.0.5.2.7/labelme/__main__.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/app.py` & `labelmeAMIT-1.0.5.2.7/labelme/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 import re
 
 # FIXME
 # - [medium] Set max zoom value to something big enough for FitWidth/Window
 
 # TODO(unknown):
 # - Zoom is too "steppy".
+#image process
+import cv2
+import numpy as np
+import imageProcessing
 
 
 LABEL_COLORMAP = imgviz.label_colormap()
 
 
 class MainWindow(QtWidgets.QMainWindow):
 
@@ -205,14 +209,19 @@
         self.canvas.scrollRequest.connect(self.scrollRequest)
 
         self.canvas.newShape.connect(self.newShape)
         self.canvas.modifyShape.connect(self.modifyShape)
         self.canvas.shapeMoved.connect(self.setDirty)
         self.canvas.selectionChanged.connect(self.shapeSelectionChanged)
         self.canvas.drawingPolygon.connect(self.toggleDrawingSensitive)
+        
+        # Amit
+        self.canvas.getRectanglePoints.connect(self.imgProscess)
+        self.canvas.getMorePoints.connect(self.imgProscess2)
+        
 
         self.setCentralWidget(scrollArea)
 
         features = QtWidgets.QDockWidget.DockWidgetFeatures()
         for dock in ["flag_dock", "label_dock", "shape_dock", "file_dock"]:
             if self._config[dock]["closable"]:
                 features = features | QtWidgets.QDockWidget.DockWidgetClosable
@@ -367,14 +376,22 @@
             self.tr("Create Rectangle"),
             lambda: self.toggleDrawMode(False, createMode="rectangle"),
             shortcuts["create_rectangle"],
             "objects",
             self.tr("Start drawing rectangles"),
             enabled=False,
         )
+        createRectangleMode2 = action(
+            self.tr("Create Rectangle2"),
+            lambda: self.toggleDrawMode(False, createMode="rectangle2"),
+            shortcuts["create_rectangle"],
+            "objects",
+            self.tr("Start drawing rectangles2"),
+            enabled=False,
+        )
         createCircleMode = action(
             self.tr("Create Circle"),
             lambda: self.toggleDrawMode(False, createMode="circle"),
             shortcuts["create_circle"],
             "objects",
             self.tr("Start drawing circles"),
             enabled=False,
@@ -643,14 +660,15 @@
             undo=undo,
             removePoint=removePoint,
             createMode=createMode,
             editMode=editMode,
             drawLineMode=drawLineMode,
             modifyLineMode=modifyLineMode,
             createRectangleMode=createRectangleMode,
+            createRectangleMode2=createRectangleMode2,
             createCircleMode=createCircleMode,
             createLineMode=createLineMode,
             createPointMode=createPointMode,
             createLineStripMode=createLineStripMode,
             zoom=zoom,
             zoomIn=zoomIn,
             zoomOut=zoomOut,
@@ -679,14 +697,15 @@
             ),
             # menu shown at right click
             menu=(
                 drawLineMode,
                 modifyLineMode,
                 createMode,
                 createRectangleMode,
+                createRectangleMode2,
                 createCircleMode,
                 createLineMode,
                 createPointMode,
                 createLineStripMode,
                 editMode,
                 edit,
                 duplicate,
@@ -699,14 +718,15 @@
             ),
             onLoadActive=(
                 close,
                 drawLineMode,
                 modifyLineMode,
                 createMode,
                 createRectangleMode,
+                createRectangleMode2,
                 createCircleMode,
                 createLineMode,
                 createPointMode,
                 createLineStripMode,
                 editMode,
                 brightnessContrast,
             ),
@@ -900,14 +920,15 @@
         utils.addActions(self.canvas.menus[0], menu)
         self.menus.edit.clear()
         actions = (
             self.actions.drawLineMode,
             self.actions.modifyLineMode,
             self.actions.createMode,
             self.actions.createRectangleMode,
+            self.actions.createRectangleMode2,
             self.actions.createCircleMode,
             self.actions.createLineMode,
             self.actions.createPointMode,
             self.actions.createLineStripMode,
             self.actions.editMode,
         )
         utils.addActions(self.menus.edit, actions + self.actions.editMenu)
@@ -933,14 +954,15 @@
     def setClean(self):
         self.dirty = False
         self.actions.save.setEnabled(False)
         self.actions.drawLineMode.setEnabled(True)
         self.actions.modifyLineMode.setEnabled(True)
         self.actions.createMode.setEnabled(True)
         self.actions.createRectangleMode.setEnabled(True)
+        self.actions.createRectangleMode2.setEnabled(True)
         self.actions.createCircleMode.setEnabled(True)
         self.actions.createLineMode.setEnabled(True)
         self.actions.createPointMode.setEnabled(True)
         self.actions.createLineStripMode.setEnabled(True)
         title = __appname__
         if self.filename is not None:
             title = "{} - {}".format(title, self.filename)
@@ -1003,96 +1025,299 @@
 
         In the middle of drawing, toggling between modes should be disabled.
         """
         self.actions.editMode.setEnabled(not drawing)
         self.actions.undoLastPoint.setEnabled(drawing)
         self.actions.undo.setEnabled(not drawing)
         self.actions.delete.setEnabled(not drawing)
+    
+    def imgProscess(self,x1,y1,x2,y2):
+        print("")
+        width=x2-x1
+        height=y2-y1
+        
+        self.image
+        imageCV=self.QImage2CV(self.image)
+        imgCrop=imageCV[y1:y2,x1:x2] 
+        # cv2.imwrite("imgGrayhist.jpg",imgGrayhist)  
+        # imageCV=image1.convertToFormat(QImage::Format_RGB888)  
+        grayimgAll = cv2.cvtColor(imageCV, cv2.COLOR_BGR2GRAY)
+
+        imgGrayhistAll=self.imgGrayhist(grayimgAll)
+        imgGrayhistCrop=imgGrayhistAll[y1:y2,x1:x2] 
+        # cv2.imwrite("imgGrayhist1.jpg",imgGrayhistCrop)
+        # cv2.imwrite("imgGrayhistAll.jpg",imgGrayhistAll) 
+        thresholdImg=imageProcessing.thresholdProcess(imgGrayhistCrop)
+        sobelImg=imageProcessing.sobelProcess(thresholdImg)
+        cannyImg=imageProcessing.sobelProcess(thresholdImg)
+        preImg=imageProcessing.sobelProcess(thresholdImg)
+        
+        # cv2.imwrite("sobelImg.jpg",sobelImg)
+        # cv2.imwrite("cannyImg.jpg",cannyImg)
+        # cv2.imwrite("preImg.jpg",preImg)
+        
+        
+        contours=imageProcessing.getContour(sobelImg)
+        contourlist1=list(contours)
+        # max_value_mirror = max(list(contourlist1.values())) 
+        i=0
+        listLen=len(contourlist1)
+        sizeList=[]
+        for i in range(listLen):
+            sizeList.append(len(contourlist1[i]))
+            
+            
+        maxIndex=sizeList.index(max(sizeList))
+        contoursList = contourlist1[maxIndex]
+        self.canvas.myContourPoints=contoursList
+        cv2.drawContours(sobelImg,contours,-1,(255,255,0),1)
+        cv2.imwrite("sobelImgContour.jpg",sobelImg)
+    def imgProscess2(self,pointslist):
+        print("imgProscess2")
+
+        
+        self.image
+        imageCV=self.QImage2CV(self.image)
+        
+        # imgCrop=imageCV[y1:y2,x1:x2] 
+        # # cv2.imwrite("imgGrayhist.jpg",imgGrayhist)  
+        # # imageCV=image1.convertToFormat(QImage::Format_RGB888)  
+        grayimgAll = cv2.cvtColor(imageCV, cv2.COLOR_BGR2GRAY)
+
+        imgGrayhistAll=self.imgGrayhist(grayimgAll)
+        imgGrayhistCrop,x1,y1=self.imageCrop2(imgGrayhistAll,pointslist)
+        cv2.imwrite("imgGrayhistCrop.jpg",imgGrayhistCrop)
+        # imgGrayhistCrop=imgGrayhistAll[y1:y2,x1:x2] 
+        # cv2.imwrite("imgGrayhist1.jpg",imgGrayhistCrop)
+        # cv2.imwrite("imgGrayhistAll.jpg",imgGrayhistAll)
+        
+        
+        mean , stddv= cv2.meanStdDev(imgGrayhistCrop)
+        min_val,max_val,min_indx,max_indx=cv2.minMaxLoc(imgGrayhistCrop) 
+        thresholdImg=imageProcessing.thresholdProcess(imgGrayhistCrop,min_val,max_val,mean,stddv)
+        sobelImg=imageProcessing.sobelProcess(thresholdImg)
+        cannyImg=imageProcessing.sobelProcess(thresholdImg)
+        preImg=imageProcessing.sobelProcess(thresholdImg)
+        
+        cv2.imwrite("sobelImg.jpg",sobelImg)
+        cv2.imwrite("cannyImg.jpg",cannyImg)
+        cv2.imwrite("preImg.jpg",preImg)
+        
+        
+        contours=imageProcessing.getContour(sobelImg)
+        #contours=imageProcessing.getContour(cannyImg)
+        print("contours",contours)
+        contourlist1=list(contours)
+        # max_value_mirror = max(list(contourlist1.values())) 
+        i=0
+        listLen=len(contourlist1)
+        sizeList=[]
+        for i in range(listLen):
+            sizeList.append(len(contourlist1[i]))
+            
+        if  sizeList!=[]:   
+            maxIndex=sizeList.index(max(sizeList))
+            contoursList = contourlist1[maxIndex]
+            contoursListQPointF=[]
+            for item in contoursList:
+                # xPoint=QtCore.QPointF()
+                # yPoint=QtCore.QPointF()
+                qpoint=QtCore.QPointF(item[0][0]+x1,item[0][1]+y1)
+                contoursListQPointF.append(qpoint)
+            self.canvas.myContourPoints=contoursListQPointF
+            cv2.drawContours(sobelImg,contours,-1,(255,255,0),1)
+            cv2.imwrite("sobelImgContour.jpg",sobelImg) 
+          
+        
+         
+    
+    def imgGrayhist(self,image):
+        
+        imageHist=cv2.equalizeHist(image)
+        cv2.imwrite("imageHist.jpg",imageHist)  
+        return imageHist
+    
+    def QImage2CV(self,qimg):
+        
+    
+        tmp = qimg
+        
+        #使用numpy创建空的图象
+        cv_image = np.zeros((tmp.height(), tmp.width(), 3), dtype=np.uint8)
+        
+        for row in range(0, tmp.height()):
+            for col in range(0,tmp.width()):
+                r = QtGui.qRed(tmp.pixel(col, row))
+                g = QtGui.qGreen(tmp.pixel(col, row))
+                b = QtGui.qBlue(tmp.pixel(col, row))
+                cv_image[row,col,0] = b
+                cv_image[row,col,1] = g
+                cv_image[row,col,2] = r
+        
+        return cv_image
+
+    
+    
+    def imageCrop(self,image,pts):
+        pts_int=0
+        pts_intList=[]
+        # pts_int = list(map(int, pts))
+        i=0
+        for item in pts:
+            
+            pts_int=(item.toPoint())
+            points=[pts_int.x(),pts_int.y()]
+            a=1
+            pts_intList.append(points)
+            i=i+1
+            # a=1
+        mask = np.zeros(image.shape, np.uint8)
+        # pts_int=list(map(pts_int))
+        points = np.array(pts_intList, np.int32)
+        points = points.reshape((-1, 1, 2))
+        # 画多边形
+        mask = cv2.polylines(mask, [points], True, (0, 0, 0), 2)
+        # mask = cv2.polylines(mask, [points], True, (255, 255, 255), 2)
+        # mask2 = cv2.fillPoly(mask.copy(), [points], (255, 255, 255))  # 用于求 ROI
+        mask2 = cv2.fillPoly(mask.copy(), [points], (0, 0, 0))  # 用于求 ROI
+        mask3 = cv2.fillPoly(mask.copy(), [points], (0, 255, 0))  # 用于 显示在桌面的图像
+
+        show_image = cv2.addWeighted(src1=image, alpha=0.8, src2=mask3, beta=0.2, gamma=0)
+
+        # cv2.imshow("mask", mask2)
+        # cv2.imshow("show_img", show_image)
+
+        ROI = cv2.bitwise_and(mask2, image)
+
+        
+        
+        
+        
+        return ROI 
+      
+    def imageCrop2(self,image,pts):
+        pts_int=0
+        pts_intList=[]
+        # pts_int = list(map(int, pts))
+        i=0
+        for item in pts:
+            
+            pts_int=(item.toPoint())
+            points=[pts_int.x(),pts_int.y()]
+            a=1
+            pts_intList.append(points)
+            i=i+1
+            # a=1
+        x1=pts_intList[0][0]
+        x2=pts_intList[1][0]
+        y1=pts_intList[0][1]
+        y2=pts_intList[1][1] 
+        imageCrop=image[y1:y2,x1:x2] 
+        return imageCrop,x1,y1 
 
     def toggleDrawMode(self, edit=True, createMode="polygon"):
         self.canvas.setEditing(edit)
         self.canvas.createMode = createMode
         if edit:
             self.actions.drawLineMode.setEnabled(True)
             self.actions.modifyLineMode.setEnabled(True)
             self.actions.createMode.setEnabled(True)
             self.actions.createRectangleMode.setEnabled(True)
+            self.actions.createRectangleMode2.setEnabled(True)
             self.actions.createCircleMode.setEnabled(True)
             self.actions.createLineMode.setEnabled(True)
             self.actions.createPointMode.setEnabled(True)
             self.actions.createLineStripMode.setEnabled(True)
         else:
             if createMode == "drawline":
                 self.actions.drawLineMode.setEnabled(False)
                 self.actions.modifyLineMode.setEnabled(True)
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
             elif createMode == "modifyline":
                 self.actions.drawLineMode.setEnabled(True)
                 self.actions.modifyLineMode.setEnabled(False)
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
             elif createMode == "polygon":
                 self.actions.drawLineMode.setEnabled(True)
                 self.actions.modifyLineMode.setEnabled(True)
                 self.actions.createMode.setEnabled(False)
                 self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
             elif createMode == "rectangle":
                 self.actions.drawLineMode.setEnabled(True)
                 self.actions.modifyLineMode.setEnabled(True)
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(False)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
+            elif createMode == "rectangle2":
+                self.actions.drawLineMode.setEnabled(True)
+                self.actions.modifyLineMode.setEnabled(True)
+                self.actions.createMode.setEnabled(True)
+                self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(False)
+                self.actions.createCircleMode.setEnabled(True)
+                self.actions.createLineMode.setEnabled(True)
+                self.actions.createPointMode.setEnabled(True)
+                self.actions.createLineStripMode.setEnabled(True)    
             elif createMode == "line":
                 self.actions.drawLineMode.setEnabled(True)
                 self.actions.modifyLineMode.setEnabled(True)
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(False)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
             elif createMode == "point":
                 self.actions.drawLineMode.setEnabled(True)
                 self.actions.modifyLineMode.setEnabled(True)
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(False)
                 self.actions.createLineStripMode.setEnabled(True)
             elif createMode == "circle":
                 self.actions.drawLineMode.setEnabled(True)
                 self.actions.modifyLineMode.setEnabled(True)
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(False)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
             elif createMode == "linestrip":
                 self.actions.drawLineMode.setEnabled(True)
                 self.actions.modifyLineMode.setEnabled(True)
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createRectangleMode2.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(False)
             else:
                 raise ValueError("Unsupported createMode: %s" % createMode)
         self.actions.editMode.setEnabled(not edit)
```

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/cli/draw_json.py` & `labelmeAMIT-1.0.5.2.7/labelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/cli/draw_label_png.py` & `labelmeAMIT-1.0.5.2.7/labelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/cli/json_to_dataset.py` & `labelmeAMIT-1.0.5.2.7/labelme/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/cli/on_docker.py` & `labelmeAMIT-1.0.5.2.7/labelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/config/__init__.py` & `labelmeAMIT-1.0.5.2.7/labelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/config/default_config.yaml` & `labelmeAMIT-1.0.5.2.7/labelme/config/default_config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
   num_backups: 10
   # show crosshair
   crosshair:
     drawline: false
     modifyline: false
     polygon: false
     rectangle: true
+    rectangle2: true
     circle: false
     line: false
     point: false
     linestrip: false
 
 shortcuts:
   close: Ctrl+W
```

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/cancel.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/close.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/color-line.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/color.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/copy.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/delete.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/done.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/done.svg` & `labelmeAMIT-1.0.5.2.7/labelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/edit.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/expert.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/eye.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/feBlend-icon.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/file.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/fit-width.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/fit-window.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/fit.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/help.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/icon.icns` & `labelmeAMIT-1.0.5.2.7/labelme/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/icon.ico` & `labelmeAMIT-1.0.5.2.7/labelme/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/icon.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/icon.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/labels.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/labels.svg` & `labelmeAMIT-1.0.5.2.7/labelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/new.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/next.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/objects.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/open.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/open.svg` & `labelmeAMIT-1.0.5.2.7/labelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/prev.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/quit.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/save-as.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/save-as.svg` & `labelmeAMIT-1.0.5.2.7/labelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/save.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/save.svg` & `labelmeAMIT-1.0.5.2.7/labelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/undo-cross.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/undo.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/zoom-in.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/zoom-out.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/icons/zoom.png` & `labelmeAMIT-1.0.5.2.7/labelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/label_file.py` & `labelmeAMIT-1.0.5.2.7/labelme/label_file.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/logger.py` & `labelmeAMIT-1.0.5.2.7/labelme/logger.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/shape.py` & `labelmeAMIT-1.0.5.2.7/labelme/shape.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         if value is None:
             value = "polygon"
         if value not in [
             "drawline",
             "modifyline",
             "polygon",
             "rectangle",
+            "rectangle2",
             "point",
             "line",
             "circle",
             "linestrip",
         ]:
             raise ValueError("Unexpected shape_type: {}".format(value))
         self._shape_type = value
@@ -130,15 +131,16 @@
 
     def getRectFromLine(self, pt1, pt2):
         x1, y1 = pt1.x(), pt1.y()
         x2, y2 = pt2.x(), pt2.y()
         return QtCore.QRectF(x1, y1, x2 - x1, y2 - y1)
 
     def paint(self, painter):
-        if self.points:
+        a =self.points
+        if True:
             color = (
                 self.select_line_color if self.selected else self.line_color
             )
             pen = QtGui.QPen(color)
             # Try using integer sizes for smoother drawing(?)
             pen.setWidth(max(1, int(round(2.0 / self.scale))))
             painter.setPen(pen)
@@ -149,14 +151,34 @@
             if self.shape_type == "rectangle":
                 assert len(self.points) in [1, 2]
                 if len(self.points) == 2:
                     rectangle = self.getRectFromLine(*self.points)
                     line_path.addRect(rectangle)
                 for i in range(len(self.points)):
                     self.drawVertex(vrtx_path, i)
+            elif self.shape_type == "rectangle2":
+                
+                # assert len(self.points) in [1, 2]
+                if len(self.points) == 2:
+                    rectangle = self.getRectFromLine(*self.points)
+                    line_path.addRect(rectangle)
+                for i in range(len(self.points)):
+                    self.drawVertex(vrtx_path, i)
+                #################################################
+                # line_path.moveTo(self.points[0])
+                # # Uncommenting the following line will draw 2 paths
+                # # for the 1st vertex, and make it non-filled, which
+                # # may be desirable.
+                # # self.drawVertex(vrtx_path, 0)
+
+                # for i, p in enumerate(self.points):
+                #     line_path.lineTo(p)
+                #     self.drawVertex(vrtx_path, i)
+                # if self.isClosed():
+                #     line_path.lineTo(self.points[0])       
             elif self.shape_type == "circle":
                 assert len(self.points) in [1, 2]
                 if len(self.points) == 2:
                     rectangle = self.getCircleRectFromLine(self.points)
                     line_path.addEllipse(rectangle)
                 for i in range(len(self.points)):
                     self.drawVertex(vrtx_path, i)
@@ -250,14 +272,19 @@
 
     def makePath(self):
         if self.shape_type == "rectangle":
             path = QtGui.QPainterPath()
             if len(self.points) == 2:
                 rectangle = self.getRectFromLine(*self.points)
                 path.addRect(rectangle)
+        elif self.shape_type == "rectangle2":
+            path = QtGui.QPainterPath()
+            if len(self.points) == 2:
+                rectangle = self.getRectFromLine(*self.points)
+                path.addRect(rectangle)                
         elif self.shape_type == "circle":
             path = QtGui.QPainterPath()
             if len(self.points) == 2:
                 rectangle = self.getCircleRectFromLine(self.points)
                 path.addEllipse(rectangle)
         elif self.shape_type == "modifyline":
             path = QtGui.QPainterPath()
```

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/testing.py` & `labelmeAMIT-1.0.5.2.7/labelme/testing.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/utils/__init__.py` & `labelmeAMIT-1.0.5.2.7/labelme/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/utils/_io.py` & `labelmeAMIT-1.0.5.2.7/labelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/utils/image.py` & `labelmeAMIT-1.0.5.2.7/labelme/utils/image.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/utils/qt.py` & `labelmeAMIT-1.0.5.2.7/labelme/utils/qt.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/utils/shape.py` & `labelmeAMIT-1.0.5.2.7/labelme/utils/shape.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,17 @@
         assert len(xy) == 2, "Shape of shape_type=circle must have 2 points"
         (cx, cy), (px, py) = xy
         d = math.sqrt((cx - px) ** 2 + (cy - py) ** 2)
         draw.ellipse([cx - d, cy - d, cx + d, cy + d], outline=1, fill=1)
     elif shape_type == "rectangle":
         assert len(xy) == 2, "Shape of shape_type=rectangle must have 2 points"
         draw.rectangle(xy, outline=1, fill=1)
+    elif shape_type == "rectangle2":
+        assert len(xy) == 2, "Shape of shape_type=rectangle must have 2 points"
+        draw.rectangle(xy, outline=1, fill=1)
     elif shape_type == "line":
         assert len(xy) == 2, "Shape of shape_type=line must have 2 points"
         draw.line(xy=xy, fill=1, width=line_width)
     elif shape_type == "linestrip":
         draw.line(xy=xy, fill=1, width=line_width)
     elif shape_type == "point":
         assert len(xy) == 1, "Shape of shape_type=point must have 1 points"
```

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/brightness_contrast_dialog.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/canvas.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,44 +22,51 @@
 
 
 class Canvas(QtWidgets.QWidget):
 
     zoomRequest = QtCore.Signal(int, QtCore.QPoint)
     scrollRequest = QtCore.Signal(int, int)
     newShape = QtCore.Signal()
-    modifyShape = QtCore.Signal()
+    
+    getRectanglePoints=QtCore.Signal(int,int,int,int)
+    getMorePoints=QtCore.Signal(list)
+    
     selectionChanged = QtCore.Signal(list)
+    modifyShape = QtCore.Signal()
     shapeMoved = QtCore.Signal()
     drawingPolygon = QtCore.Signal(bool)
     vertexSelected = QtCore.Signal(bool)
 
     CREATE, EDIT = 0, 1
 
     # polygon, rectangle, line, or point
     _createMode = "polygon"
 
     _fill_drawing = False
+    myContourPoints=''
 
     def __init__(self, *args, **kwargs):
         self.epsilon = kwargs.pop("epsilon", 10.0)
         self.double_click = kwargs.pop("double_click", "close")
         if self.double_click not in [None, "close"]:
             raise ValueError(
                 "Unexpected value for double_click event: {}".format(
                     self.double_click
                 )
             )
         self.num_backups = kwargs.pop("num_backups", 10)
+        # print("self._crosshair",self._crosshair)
         self._crosshair = kwargs.pop(
             "crosshair",
             {
                 "drawline": False,
                 "modifyline": False,
                 "polygon": False,
-                "rectangle": True,
+                "rectangle2": False,
+                "rectangle2": True,
                 "circle": False,
                 "line": False,
                 "point": False,
                 "linestrip": False,
             },
         )
         super(Canvas, self).__init__(*args, **kwargs)
@@ -116,14 +123,15 @@
     @createMode.setter
     def createMode(self, value):
         if value not in [
             "drawline",
             "modifyline",
             "polygon",
             "rectangle",
+            "rectangle2",
             "circle",
             "line",
             "point",
             "linestrip",
         ]:
             raise ValueError("Unsupported createMode: %s" % value)
         self._createMode = value
@@ -231,28 +239,35 @@
             if self.outOfPixmap(pos):
                 # Don't allow the user to draw outside the pixmap.
                 # Project the point to the pixmap's edges.
                 pos = self.intersectionPoint(self.current[-1], pos)
             elif (
                 self.snapping
                 and len(self.current) > 1
-                and self.createMode == "polygon"
+                # and (self.createMode == "polygon" or self.createMode == "rectangle2")
+                and self.createMode == "polygon" 
                 and self.closeEnough(pos, self.current[0])
             ):
                 # Attract line to starting point and
                 # colorise to alert the user.
                 pos = self.current[0]
                 self.overrideCursor(CURSOR_POINT)
                 self.current.highlightVertex(0, Shape.NEAR_VERTEX)
             if self.createMode in ["polygon", "linestrip"]:
                 self.line[0] = self.current[-1]
                 self.line[1] = pos
             elif self.createMode == "rectangle":
                 self.line.points = [self.current[0], pos]
                 self.line.close()
+            elif self.createMode == "rectangle2":
+                 self.line.points = [self.current[0], pos]
+                 self.line.close()
+                #######################
+                # self.line[0] = self.current[-1]
+                # self.line[1] = pos
             elif self.createMode == "circle":
                 self.line.points = [self.current[0], pos]
                 self.line.shape_type = "circle"
             elif self.createMode == "line":
                 self.line.points = [self.current[0], pos]
                 self.line.close()
             elif self.createMode == "point":
@@ -389,14 +404,48 @@
                         self.line[0] = self.current[-1]
                         if self.current.isClosed():
                             self.finalise()
                     elif self.createMode in ["rectangle", "circle", "line"]:
                         assert len(self.current.points) == 1
                         self.current.points = self.line.points
                         self.finalise()
+                    
+                    elif self.createMode in ["rectangle2"]:
+                        # assert len(self.current.points) == 1
+                        # self.current.points = self.line.points
+
+                        # # self.pixmap
+                        # self.current.points=self.myContourPoints
+                        # self.finalise()
+                        # #####polygon
+                        assert len(self.current.points) == 1
+                        self.current.points = self.line.points
+                        point1x=self.current.points[0].x()
+                        point1y=self.current.points[0].y()
+                        point2x=self.current.points[1].x()
+                        point2y=self.current.points[1].y()
+                        # self.getRectanglePoints.emit(int(point1x),int(point1y),int(point2x),int(point2y))
+                        self.getMorePoints.emit(self.current.points)
+                        self.current.points=self.myContourPoints
+                        self.line.points=self.myContourPoints
+                        Shape.points=self.myContourPoints
+                        self.finalise()
+                        
+                        #####
+                        # self.current.addPoint(self.line[1])
+                        # self.line[0] = self.current[-1]
+                        # if self.current.isClosed():
+                        #     self.getMorePoints.emit(self.current.points)
+                        #     self.current.points=self.myContourPoints
+                        #     self.line.points=self.myContourPoints
+                        #     Shape.points=self.myContourPoints
+                        #     self.finalise()
+
+                        
+                            
                     elif self.createMode == "linestrip":
                         self.current.addPoint(self.line[1])
                         self.line[0] = self.current[-1]
                         if int(ev.modifiers()) == QtCore.Qt.ControlModifier:
                             self.finalise()
                     elif self.createMode == "drawline":
                         self.current.addPoint(self.line[1])
@@ -767,14 +816,15 @@
             self.line.paint(p)
         if self.selectedShapesCopy:
             for s in self.selectedShapesCopy:
                 s.paint(p)
 
         if (
             self.fillDrawing()
+            #and (self.createMode == "polygon" or self.createMode == "rectangle2")
             and self.createMode == "polygon"
             and self.current is not None
             and len(self.current.points) >= 2
         ):
             drawing_shape = self.current.copy()
             drawing_shape.addPoint(self.line[1])
             drawing_shape.fill = True
@@ -979,14 +1029,17 @@
         assert self.shapes
         self.current = self.shapes.pop()
         self.current.setOpen()
         if self.createMode in ["polygon", "linestrip"]:
             self.line.points = [self.current[-1], self.current[0]]
         elif self.createMode in ["rectangle", "line", "circle"]:
             self.current.points = self.current.points[0:1]
+        elif self.createMode in ["rectangle2"]:
+            self.current.points = self.current.points[0:1] 
+            #self.line.points = [self.current[-1], self.current[0]]   
         elif self.createMode == "point":
             self.current = None
         self.drawingPolygon.emit(True)
 
     def undoLastPoint(self):
         if not self.current or self.current.isClosed():
             return
```

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/color_dialog.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/file_dialog_preview.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/label_dialog.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/label_list_widget.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/tool_bar.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/unique_label_qlist_widget.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelme/widgets/zoom_widget.py` & `labelmeAMIT-1.0.5.2.7/labelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/PKG-INFO` & `labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelmeAMIT
-Version: 1.0.5.2.6
+Version: 1.0.5.2.7
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada
 Author-email: www.kentaro.wada@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labelmeAMIT Version: 1.0.5.2.6 Summary: Image
+Metadata-Version: 2.1 Name: labelmeAMIT Version: 1.0.5.2.7 Summary: Image
 Polygonal Annotation with Python Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada Author-email: www.kentaro.wada@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `labelmeAMIT-1.0.5.2.6/labelmeAMIT.egg-info/SOURCES.txt` & `labelmeAMIT-1.0.5.2.7/labelmeAMIT.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 labelme/__init__.py
 labelme/__main__.py
 labelme/app.py
+labelme/imageProcessing.py
 labelme/label_file.py
 labelme/logger.py
 labelme/shape.py
 labelme/testing.py
 labelme/cli/__init__.py
 labelme/cli/draw_json.py
 labelme/cli/draw_label_png.py
```

### Comparing `labelmeAMIT-1.0.5.2.6/setup.py` & `labelmeAMIT-1.0.5.2.7/setup.py`

 * *Files identical despite different names*


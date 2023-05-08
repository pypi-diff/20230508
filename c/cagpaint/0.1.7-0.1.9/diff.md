# Comparing `tmp/cagpaint-0.1.7.tar.gz` & `tmp/cagpaint-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagpaint-0.1.7.tar", last modified: Thu May  4 15:23:04 2023, max compression
+gzip compressed data, was "cagpaint-0.1.9.tar", last modified: Mon May  8 10:59:09 2023, max compression
```

## Comparing `cagpaint-0.1.7.tar` & `cagpaint-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.846233 cagpaint-0.1.7/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.1.7/LICENSE
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 15:23:04.846233 cagpaint-0.1.7/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.1.7/README.md
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.838233 cagpaint-0.1.7/cagpaint/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:53:02.000000 cagpaint-0.1.7/cagpaint/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.838233 cagpaint-0.1.7/cagpaint/painter/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:49.000000 cagpaint-0.1.7/cagpaint/painter/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3932 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/install_fixes.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.842233 cagpaint-0.1.7/cagpaint/painter/src/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:53.000000 cagpaint-0.1.7/cagpaint/painter/src/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    43783 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/about.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6548 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/contrast_slider.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12206 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/create_project.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6631 2022-09-20 07:43:51.000000 cagpaint-0.1.7/cagpaint/painter/src/file_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15984 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/graphics_scene.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2853 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/graphics_view.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12990 2023-05-03 08:00:12.000000 cagpaint-0.1.7/cagpaint/painter/src/im_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    23982 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/im_viewer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3161 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/instructions.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2347 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/lock.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3412 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/main.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13121 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/menus.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1649 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/name_edit_widget.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5400 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/nav.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3620 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/palette.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8541 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/patch_seg.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1808 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/progress_widget.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    36880 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/root_painter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1304 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/segment.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8409 2022-11-17 19:02:25.000000 cagpaint-0.1.7/cagpaint/painter/src/segment_folder.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4572 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/slice_nav.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3039 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/tcp_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       85 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/view_state.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3080 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/visibility_widget.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.842233 cagpaint-0.1.7/cagpaint/trainer/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      972 2023-05-04 15:22:42.000000 cagpaint-0.1.7/cagpaint/trainer/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1204 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/trainer/data_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    19205 2023-05-03 14:16:20.000000 cagpaint-0.1.7/cagpaint/trainer/datasets.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2650 2022-11-26 14:08:31.000000 cagpaint-0.1.7/cagpaint/trainer/file_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    21190 2023-05-03 08:05:58.000000 cagpaint-0.1.7/cagpaint/trainer/im_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1789 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/instructions.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7388 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/loss.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2196 2023-05-04 15:03:08.000000 cagpaint-0.1.7/cagpaint/trainer/main.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2922 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/trainer/metrics.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15203 2023-05-03 08:07:17.000000 cagpaint-0.1.7/cagpaint/trainer/model_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7463 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/patch_seg.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1373 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/trainer/scp_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2587 2022-11-17 08:42:24.000000 cagpaint-0.1.7/cagpaint/trainer/startup.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    29553 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/trainer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7698 2022-09-20 07:47:16.000000 cagpaint-0.1.7/cagpaint/trainer/unet3d.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.838233 cagpaint-0.1.7/cagpaint.egg-info/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1547 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/SOURCES.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/dependency_links.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        9 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/top_level.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-04 15:23:04.846233 cagpaint-0.1.7/setup.cfg
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-04 15:23:02.000000 cagpaint-0.1.7/setup.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.455272 cagpaint-0.1.9/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.1.9/LICENSE
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-08 10:59:09.455272 cagpaint-0.1.9/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.1.9/README.md
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.451272 cagpaint-0.1.9/cagpaint/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:53:02.000000 cagpaint-0.1.9/cagpaint/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.451272 cagpaint-0.1.9/cagpaint/painter/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:49.000000 cagpaint-0.1.9/cagpaint/painter/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3932 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/install_fixes.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.455272 cagpaint-0.1.9/cagpaint/painter/src/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:53.000000 cagpaint-0.1.9/cagpaint/painter/src/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    43783 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/about.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6548 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/contrast_slider.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12269 2023-05-08 08:52:37.000000 cagpaint-0.1.9/cagpaint/painter/src/create_project.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6657 2023-05-08 09:04:20.000000 cagpaint-0.1.9/cagpaint/painter/src/file_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    16052 2023-05-08 09:05:33.000000 cagpaint-0.1.9/cagpaint/painter/src/graphics_scene.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2853 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/graphics_view.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12990 2023-05-03 08:00:12.000000 cagpaint-0.1.9/cagpaint/painter/src/im_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    24174 2023-05-08 09:03:45.000000 cagpaint-0.1.9/cagpaint/painter/src/im_viewer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3161 2022-11-29 09:34:29.000000 cagpaint-0.1.9/cagpaint/painter/src/instructions.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2347 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/lock.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3433 2023-05-08 08:49:26.000000 cagpaint-0.1.9/cagpaint/painter/src/main.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13163 2023-05-08 08:54:38.000000 cagpaint-0.1.9/cagpaint/painter/src/menus.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1649 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/name_edit_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5421 2023-05-08 08:54:45.000000 cagpaint-0.1.9/cagpaint/painter/src/nav.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3620 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/palette.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8583 2023-05-08 08:54:54.000000 cagpaint-0.1.9/cagpaint/painter/src/patch_seg.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1808 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/progress_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    37257 2023-05-08 09:02:57.000000 cagpaint-0.1.9/cagpaint/painter/src/root_painter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1304 2022-11-29 09:34:29.000000 cagpaint-0.1.9/cagpaint/painter/src/segment.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8471 2023-05-08 08:55:19.000000 cagpaint-0.1.9/cagpaint/painter/src/segment_folder.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4572 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/slice_nav.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3039 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/tcp_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       85 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/view_state.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3080 2023-05-04 16:09:47.000000 cagpaint-0.1.9/cagpaint/painter/src/visibility_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      124 2023-05-08 08:30:21.000000 cagpaint-0.1.9/cagpaint/setup.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.455272 cagpaint-0.1.9/cagpaint/trainer/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       30 2023-05-08 08:38:36.000000 cagpaint-0.1.9/cagpaint/trainer/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1204 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/trainer/data_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    19244 2023-05-08 09:09:39.000000 cagpaint-0.1.9/cagpaint/trainer/datasets.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2650 2022-11-26 14:08:31.000000 cagpaint-0.1.9/cagpaint/trainer/file_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    21207 2023-05-08 08:42:35.000000 cagpaint-0.1.9/cagpaint/trainer/im_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1789 2022-11-29 09:34:29.000000 cagpaint-0.1.9/cagpaint/trainer/instructions.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7422 2023-05-08 10:04:33.000000 cagpaint-0.1.9/cagpaint/trainer/loss.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2213 2023-05-08 08:46:32.000000 cagpaint-0.1.9/cagpaint/trainer/main.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2922 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/trainer/metrics.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15276 2023-05-08 09:33:38.000000 cagpaint-0.1.9/cagpaint/trainer/model_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7463 2023-05-08 07:44:59.000000 cagpaint-0.1.9/cagpaint/trainer/patch_seg.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1373 2023-05-05 17:55:24.000000 cagpaint-0.1.9/cagpaint/trainer/scp_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2587 2022-11-17 08:42:24.000000 cagpaint-0.1.9/cagpaint/trainer/startup.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    29805 2023-05-08 09:09:02.000000 cagpaint-0.1.9/cagpaint/trainer/trainer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7698 2023-05-08 09:33:09.000000 cagpaint-0.1.9/cagpaint/trainer/unet3d.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.451272 cagpaint-0.1.9/cagpaint.egg-info/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1565 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        9 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/top_level.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-08 10:59:09.455272 cagpaint-0.1.9/setup.cfg
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-08 10:58:15.000000 cagpaint-0.1.9/setup.py
```

### Comparing `cagpaint-0.1.7/LICENSE` & `cagpaint-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/install_fixes.py` & `cagpaint-0.1.9/cagpaint/painter/install_fixes.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/about.py` & `cagpaint-0.1.9/cagpaint/painter/src/about.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/contrast_slider.py` & `cagpaint-0.1.9/cagpaint/painter/src/contrast_slider.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/create_project.py` & `cagpaint-0.1.9/cagpaint/painter/src/create_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 import shutil
 import json
 
 from pathlib import Path, PurePosixPath
 from PyQt5 import QtWidgets
 from PyQt5 import QtCore
 
-from im_utils import is_image, get_recursive_files, getDataFromDatabase
-from palette import PaletteEditWidget
-from name_edit_widget import NameEditWidget
+from cagpaint.painter.src.im_utils import is_image, get_recursive_files, getDataFromDatabase
+from cagpaint.painter.src.palette import PaletteEditWidget
+from cagpaint.painter.src.name_edit_widget import NameEditWidget
 
 class CreateProjectWidget(QtWidgets.QWidget):
 
     created = QtCore.pyqtSignal(Path)
 
     def __init__(self, sync_dir):
         super().__init__()
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/file_utils.py` & `cagpaint-0.1.9/cagpaint/painter/src/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import os
 from os.path import splitext
 import filecmp
 import numpy as np
 from skimage.io import imread
 import nibabel as nib
-import im_utils
+from cagpaint.painter.src import im_utils
 from pathlib import Path
 
 
 def penultimate_fname_with_segmentation(fnames, seg_dir):
     """
     Go through fnames and return the last one with a segmentation
     If no segmentations are found return None.
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/graphics_scene.py` & `cagpaint-0.1.9/cagpaint/painter/src/graphics_scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 from PyQt5 import QtGui
 from PyQt5 import QtCore
 from PyQt5.QtCore import Qt
 import nibabel as nib
 import time
 import qimage2ndarray
 from skimage.segmentation import flood
-import im_utils
-from view_state import ViewState
-from patch_seg import SegmentPatchThread, PatchSegmentor
+from cagpaint.painter.src import im_utils
+from cagpaint.painter.src.view_state import ViewState
+from cagpaint.painter.src.patch_seg import SegmentPatchThread, PatchSegmentor
 
 class GraphicsScene(QtWidgets.QGraphicsScene):
     """
     Canvas where image and lines will be drawn
     """
     def __init__(self, parent):
         super().__init__()
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/graphics_view.py` & `cagpaint-0.1.9/cagpaint/painter/src/graphics_view.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/im_utils.py` & `cagpaint-0.1.9/cagpaint/painter/src/im_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/im_viewer.py` & `cagpaint-0.1.9/cagpaint/painter/src/im_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 
 import qimage2ndarray
 from PyQt5 import QtWidgets
 from PyQt5 import QtCore
 from PyQt5 import QtGui
 from PyQt5.QtCore import Qt
 
-from view_state import ViewState
-from graphics_scene import GraphicsScene
-from graphics_view import CustomGraphicsView
-from slice_nav import SliceNav
-from visibility_widget import VisibilityWidget
-
-import im_utils
-import menus
+from cagpaint.painter.src.view_state import ViewState
+from cagpaint.painter.src.graphics_scene import GraphicsScene
+from cagpaint.painter.src.graphics_view import CustomGraphicsView
+from cagpaint.painter.src.slice_nav import SliceNav
+from cagpaint.painter.src.visibility_widget import VisibilityWidget
+
+from cagpaint.painter.src import im_utils
+#import cagpaint.painter.src.menus
+from cagpaint.painter.src import menus
 
 
 class ImViewer(QtWidgets.QWidget):
     """ Show image, annotation and segmentation data and allow interaction
         Contains graphics scene which is where the image will be drawn
     """
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/instructions.py` & `cagpaint-0.1.9/cagpaint/painter/src/instructions.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/lock.py` & `cagpaint-0.1.9/cagpaint/painter/src/lock.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/main.py` & `cagpaint-0.1.9/cagpaint/painter/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import sys
 import os
 from pathlib import Path
 import json
 import traceback
 
 from PyQt5 import QtWidgets
-from root_painter import RootPainter
+from cagpaint.painter.src.root_painter import RootPainter
 import yaml
 import argparse
 
 
 def init_root_painter(config):
     sys.argv = [sys.argv[0]]
     app = QtWidgets.QApplication(sys.argv)
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/menus.py` & `cagpaint-0.1.9/cagpaint/painter/src/menus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 
 from PyQt5 import QtWidgets
 from PyQt5 import QtGui
 from PyQt5 import QtCore
 from PyQt5.QtCore import Qt
-from segment_folder import SegmentFolderWidget
-from segment import segment_full_image
+from cagpaint.painter.src.segment_folder import SegmentFolderWidget
+from cagpaint.painter.src.segment import segment_full_image
 
 def add_network_menu(window, menu_bar):
     """ Not in use right now as training happens automatically when the 
         annotation is saved
     """
     network_menu = menu_bar.addMenu('Network')
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/name_edit_widget.py` & `cagpaint-0.1.9/cagpaint/painter/src/name_edit_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/nav.py` & `cagpaint-0.1.9/cagpaint/painter/src/nav.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 
 from PyQt5 import QtWidgets
 from PyQt5 import QtCore
 from PyQt5.QtCore import Qt
 import json
 from pathlib import Path, PurePosixPath
-from im_utils import getDataFromDatabase
+from cagpaint.painter.src.im_utils import getDataFromDatabase
 
 class NavWidget(QtWidgets.QWidget):
     """ Shows next and previous buttons as well as image position in folder.
     """
     file_change = QtCore.pyqtSignal(str)
     class_change = QtCore.pyqtSignal(str)
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/palette.py` & `cagpaint-0.1.9/cagpaint/painter/src/palette.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/patch_seg.py` & `cagpaint-0.1.9/cagpaint/painter/src/patch_seg.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import time
 import numpy as np
 from functools import partial
 from PyQt5 import QtCore
 from enum import Enum
 
 
-from tcp_utils import request_patch_seg, establish_connection
-from instructions import fix_instruction_paths
+from cagpaint.painter.src.tcp_utils import request_patch_seg, establish_connection
+from cagpaint.painter.src.instructions import fix_instruction_paths
 
 
 class SegmentPatchThread(QtCore.QThread):
 
     complete = QtCore.pyqtSignal(np.ndarray)
 
     def __init__(self, annot_patch, content, server_ip, server_port):
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/progress_widget.py` & `cagpaint-0.1.9/cagpaint/painter/src/progress_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/root_painter.py` & `cagpaint-0.1.9/cagpaint/painter/src/root_painter.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,32 @@
 
 from skimage.io import use_plugin
 from PyQt5 import QtWidgets
 from PyQt5 import QtGui
 from PyQt5 import QtCore
 from PyQt5.QtCore import Qt
 
-from view_state import ViewState
-from about import AboutWindow, LicenseWindow, ShortcutWindow
-from create_project import CreateProjectWidget
-from im_viewer import ImViewer, ImViewerWindow
-from nav import NavWidget
-from file_utils import penultimate_fname_with_segmentation
-from file_utils import get_annot_path
-from file_utils import maybe_save_annotation_3d
-from instructions import send_instruction
-from contrast_slider import ContrastSlider
-import im_utils
-import menus
-from segment import segment_full_image
-from lock import create_lock_file, delete_lock_files_for_current_user, get_lock_file_path, show_locked_message
+from cagpaint.painter.src.view_state import ViewState
+from cagpaint.painter.src.about import AboutWindow, LicenseWindow, ShortcutWindow
+from cagpaint.painter.src.create_project import CreateProjectWidget
+from cagpaint.painter.src.im_viewer import ImViewer, ImViewerWindow
+from cagpaint.painter.src.nav import NavWidget
+from cagpaint.painter.src.file_utils import penultimate_fname_with_segmentation
+from cagpaint.painter.src.file_utils import get_annot_path
+from cagpaint.painter.src.file_utils import maybe_save_annotation_3d
+from cagpaint.painter.src.instructions import send_instruction
+from cagpaint.painter.src.contrast_slider import ContrastSlider
+from cagpaint.painter.src import im_utils
+from cagpaint.painter.src import menus
+#import menus
+from cagpaint.painter.src import menus
+from cagpaint.painter.src.segment import segment_full_image
+from cagpaint.painter.src.lock import create_lock_file, delete_lock_files_for_current_user, get_lock_file_path, show_locked_message
 from pathlib import Path
-from im_utils import getDataFromDatabase
-
+from cagpaint.painter.src.im_utils import getDataFromDatabase
 
 use_plugin("pil")
 
 class RootPainter(QtWidgets.QMainWindow):
 
     closed = QtCore.pyqtSignal()
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/segment.py` & `cagpaint-0.1.9/cagpaint/painter/src/segment.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/segment_folder.py` & `cagpaint-0.1.9/cagpaint/painter/src/segment_folder.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,20 @@
 
 #pylint: disable=I1101,C0111,W0201,R0903,E0611, R0902, R0914
 import os
 import time
 import copy
 from PyQt5 import QtWidgets
 from PyQt5 import QtCore
-from progress_widget import BaseProgressWidget
-from instructions import send_instruction
-from im_utils import is_image, getDataFromDatabase
+from cagpaint.painter.src.progress_widget import BaseProgressWidget
+from cagpaint.painter.src.instructions import send_instruction
+from cagpaint.painter.src.im_utils import is_image, getDataFromDatabase
 from pathlib import Path
 import json
 
-
 class SegmentWatchThread(QtCore.QThread):
     """
     Runs another thread.
     """
     progress_change = QtCore.pyqtSignal(int, int)
     done = QtCore.pyqtSignal()
```

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/slice_nav.py` & `cagpaint-0.1.9/cagpaint/painter/src/slice_nav.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/tcp_utils.py` & `cagpaint-0.1.9/cagpaint/painter/src/tcp_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/painter/src/visibility_widget.py` & `cagpaint-0.1.9/cagpaint/painter/src/visibility_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/data_utils.py` & `cagpaint-0.1.9/cagpaint/trainer/data_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/datasets.py` & `cagpaint-0.1.9/cagpaint/trainer/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 from pathlib import Path
 
 import torch
 import numpy as np
 from skimage import img_as_float32
 from torch.utils.data import Dataset
 
-from im_utils import load_train_image_and_annot
-import im_utils
+from cagpaint.trainer.im_utils import load_train_image_and_annot
+from cagpaint.trainer import im_utils
 # from monai.transforms import (
 #     AddChanneld,
 #     Compose,
 #     LoadImaged,
 #     RandAffined,
 #     RepeatChanneld,
 #     MapTransform,
```

### Comparing `cagpaint-0.1.7/cagpaint/trainer/file_utils.py` & `cagpaint-0.1.9/cagpaint/trainer/file_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/im_utils.py` & `cagpaint-0.1.9/cagpaint/trainer/im_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from functools import partial
 from math import ceil
 import random
 import numpy as np
 import skimage.util as skim_util
 from skimage.exposure import rescale_intensity
 import nibabel as nib
-from file_utils import ls, ls_annotations
+from cagpaint.trainer.file_utils import ls, ls_annotations
 #import nrrd
 from pathlib import Path
 import traceback
 import SimpleITK as sitk
 from scipy.ndimage import zoom
 import pandas as pd
 import psycopg2
```

### Comparing `cagpaint-0.1.7/cagpaint/trainer/instructions.py` & `cagpaint-0.1.9/cagpaint/trainer/instructions.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/loss.py` & `cagpaint-0.1.9/cagpaint/trainer/loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,16 @@
 
                     masks.append(mask)
                     fg_tiles.append(fg_tile)
                     class_outputs.append(class_output)
 
                     seg_tile = batch_seg_tiles[im_idx][i]
                     if seg_tile is not None:
-                        seg_tile = torch.from_numpy(seg_tile[17:-17,17:-17,17:-17]).to(device)
+                        seg_tile = torch.from_numpy(seg_tile).to(device)
+                       # seg_tile = seg_tile.to(device)
                         # for this purpose we ensure segmentation never disagrees with annotation.
                         seg_tile[fg_tile] = 1
                         seg_tile[bg_tile] = 0
                         seg_tiles.append(seg_tile)
                         seg_class_outputs.append(class_output)
```

### Comparing `cagpaint-0.1.7/cagpaint/trainer/main.py` & `cagpaint-0.1.9/cagpaint/trainer/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 from pathlib import Path
 import os
 import json
 import argparse
 from cagpaint.trainer import Trainer
-from startup import startup_setup
+from cagpaint.trainer.startup import startup_setup
 import yaml
 # Import all the necessary submodules
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('--syncdir',
                         help=('location of directory where data is'
```

### Comparing `cagpaint-0.1.7/cagpaint/trainer/metrics.py` & `cagpaint-0.1.9/cagpaint/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/model_utils.py` & `cagpaint-0.1.9/cagpaint/trainer/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 import time
 import math
 import traceback
 import numpy as np
 import torch
 import copy
 from skimage import img_as_float32
-import im_utils
-from unet3d import UNet3D, SmallUNet3D
-from file_utils import ls
+from cagpaint.trainer import im_utils
+from cagpaint.trainer.unet3d import UNet3D, SmallUNet3D
+from cagpaint.trainer.file_utils import ls
 from torch.nn.functional import softmax
 import torch.nn.functional as F
-from loss import get_batch_loss
+from cagpaint.trainer.loss import get_batch_loss
 
 cached_model = None
 cached_model_path = None
 use_fake_cnn = False
 
 def fake_cnn(tiles_for_gpu):
     """ Useful debug function for checking tile layout etc """
```

### Comparing `cagpaint-0.1.7/cagpaint/trainer/patch_seg.py` & `cagpaint-0.1.9/cagpaint/trainer/patch_seg.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/scp_utils.py` & `cagpaint-0.1.9/cagpaint/trainer/scp_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/startup.py` & `cagpaint-0.1.9/cagpaint/trainer/startup.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint/trainer/trainer.py` & `cagpaint-0.1.9/cagpaint/trainer/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,32 +30,31 @@
 import multiprocessing
 
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 import torch.nn.functional as F
-from loss import get_batch_loss
-from instructions import fix_config_paths
+from cagpaint.trainer.loss import get_batch_loss
+from cagpaint.trainer.instructions import fix_config_paths
 
-from datasets import RPDataset
-from metrics import get_metrics, get_metrics_str, get_metric_csv_row
-from model_utils import ensemble_segment_3d
-from model_utils import create_first_model_with_random_weights
-from model_utils import random_model
-import model_utils
-from model_utils import save_if_better, save_model
-from metrics import metrics_from_val_tile_refs
-import data_utils
+from cagpaint.trainer.datasets import RPDataset
+from cagpaint.trainer.metrics import get_metrics, get_metrics_str, get_metric_csv_row
+from cagpaint.trainer.model_utils import ensemble_segment_3d
+from cagpaint.trainer.model_utils import create_first_model_with_random_weights
+from cagpaint.trainer.model_utils import random_model
+from cagpaint.trainer import model_utils
+from cagpaint.trainer.model_utils import save_if_better, save_model
+from cagpaint.trainer.metrics import metrics_from_val_tile_refs
+from cagpaint.trainer import data_utils
 #import patch_seg
 
-from im_utils import is_image, load_image, save_then_move, save
-import im_utils
-from file_utils import ls
-
+from cagpaint.trainer.im_utils import is_image, load_image, save_then_move, save
+from cagpaint.trainer import im_utils
+from cagpaint.trainer.file_utils import ls
 
 class Trainer():
 
     def __init__(self, sync_dir, config, ip=None, port=None):
         self.sync_dir = sync_dir
         self.ip = ip
         self.port = port
```

### Comparing `cagpaint-0.1.7/cagpaint/trainer/unet3d.py` & `cagpaint-0.1.9/cagpaint/trainer/unet3d.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.7/cagpaint.egg-info/SOURCES.txt` & `cagpaint-0.1.9/cagpaint.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 cagpaint/__init__.py
+cagpaint/setup.py
 cagpaint.egg-info/PKG-INFO
 cagpaint.egg-info/SOURCES.txt
 cagpaint.egg-info/dependency_links.txt
 cagpaint.egg-info/top_level.txt
 cagpaint/painter/__init__.py
 cagpaint/painter/install_fixes.py
 cagpaint/painter/src/__init__.py
```


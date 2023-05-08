# Comparing `tmp/aps_common_libraries-1.0.3.tar.gz` & `tmp/aps_common_libraries-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps_common_libraries-1.0.3.tar", last modified: Wed May  3 22:26:21 2023, max compression
+gzip compressed data, was "aps_common_libraries-1.0.4.tar", last modified: Mon May  8 17:40:57 2023, max compression
```

## Comparing `aps_common_libraries-1.0.3.tar` & `aps_common_libraries-1.0.4.tar`

### file list

```diff
@@ -1,78 +1,85 @@
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.450199 aps_common_libraries-1.0.3/
--rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.3/LICENSE
--rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.3/LICENSE.pdf
--rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.3/MANIFEST.in
--rw-r--r--   0 bishop    (1601)      907      876 2023-05-03 22:26:21.449545 aps_common_libraries-1.0.3/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.3/README.md
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.388129 aps_common_libraries-1.0.3/aps/
--rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.3/aps/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.394898 aps_common_libraries-1.0.3/aps/common/
--rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.3/aps/common/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.396389 aps_common_libraries-1.0.3/aps/common/__test/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.3/aps/common/__test/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.3/aps/common/__test/test.py
--rw-rw-rw-   0 bishop    (1601)      907    10103 2022-11-23 21:10:21.000000 aps_common_libraries-1.0.3/aps/common/initializer.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.399582 aps_common_libraries-1.0.3/aps/common/io/
--rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.3/aps/common/io/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.3/aps/common/io/printout.py
--rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.3/aps/common/io/tcp_client.py
--rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.3/aps/common/io/tiff_file.py
--rw-rw-rw-   0 bishop    (1601)      907    20742 2023-02-17 23:08:47.000000 aps_common_libraries-1.0.3/aps/common/logger.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.400336 aps_common_libraries-1.0.3/aps/common/measurment/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.3/aps/common/measurment/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.403180 aps_common_libraries-1.0.3/aps/common/measurment/beamline/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/__init__.py
--rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_collector.py
--rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_processor.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.418203 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/
--rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/SPINNet_estimate.py
--rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/WXST.py
--rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/diffraction_process.py
--rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/euclidean_dist.py
--rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func.py
--rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func_light.py
--rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/gui_func.py
--rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/integration.py
--rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/main.py
--rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_find.py
--rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_propagate.py
--rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/utils.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.421613 aps_common_libraries-1.0.3/aps/common/ml/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.3/aps/common/ml/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.3/aps/common/ml/data_structures.py
--rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.3/aps/common/ml/mocks.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.426529 aps_common_libraries-1.0.3/aps/common/plot/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.3/aps/common/plot/__init__.py
--rw-r--r--   0 bishop    (1601)      907    44717 2023-04-08 13:27:45.000000 aps_common_libraries-1.0.3/aps/common/plot/gui.py
--rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.3/aps/common/plot/image.py
--rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.3/aps/common/plot/qt_application.py
--rw-rw-rw-   0 bishop    (1601)      907    16718 2023-02-16 16:35:31.000000 aps_common_libraries-1.0.3/aps/common/plotter.py
--rw-r--r--   0 bishop    (1601)      907     5229 2023-05-02 21:11:06.000000 aps_common_libraries-1.0.3/aps/common/reflection.py
--rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.3/aps/common/registry.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.433643 aps_common_libraries-1.0.3/aps/common/scripts/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.3/aps/common/scripts/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.3/aps/common/scripts/abstract_command_line_script.py
--rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.3/aps/common/scripts/generic_process_manager.py
--rw-rw-rw-   0 bishop    (1601)      907     7941 2023-02-17 23:04:17.000000 aps_common_libraries-1.0.3/aps/common/scripts/generic_qt_script.py
--rw-rw-rw-   0 bishop    (1601)      907     4121 2023-02-07 23:10:48.000000 aps_common_libraries-1.0.3/aps/common/scripts/script_data.py
--rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.3/aps/common/scripts/script_registry.py
--rw-rw-rw-   0 bishop    (1601)      907     4333 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.3/aps/common/singleton.py
--rw-rw-rw-   0 bishop    (1601)      907    10071 2022-11-28 18:33:01.000000 aps_common_libraries-1.0.3/aps/common/traffic_light.py
--rw-r--r--   0 bishop    (1601)      907     3543 2023-05-03 14:01:58.000000 aps_common_libraries-1.0.3/aps/common/utilities.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.441075 aps_common_libraries-1.0.3/aps/common/widgets/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.3/aps/common/widgets/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.3/aps/common/widgets/close_app_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.3/aps/common/widgets/context_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.3/aps/common/widgets/generic_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.3/aps/common/widgets/log_stream_widget.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.448412 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/
--rw-rw-rw-   0 bishop    (1601)      907      876 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907     2179 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/SOURCES.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/dependency_links.txt
--rw-rw-rw-   0 bishop    (1601)      907       15 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/namespace_packages.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/not-zip-safe
--rw-rw-rw-   0 bishop    (1601)      907      150 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/requires.txt
--rw-rw-rw-   0 bishop    (1601)      907        4 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/top_level.txt
--rw-r--r--   0 bishop    (1601)      907       38 2023-05-03 22:26:21.451750 aps_common_libraries-1.0.3/setup.cfg
--rw-r--r--   0 bishop    (1601)      907     5571 2023-05-02 20:51:39.000000 aps_common_libraries-1.0.3/setup.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.532944 aps_common_libraries-1.0.4/
+-rw-------   0 rook       (505) staff       (20)     1080 2022-10-18 15:33:45.000000 aps_common_libraries-1.0.4/LICENSE
+-rw-------   0 rook       (505) staff       (20)    10366 2022-10-18 15:33:45.000000 aps_common_libraries-1.0.4/LICENSE.pdf
+-rw-------   0 rook       (505) staff       (20)       66 2022-10-18 15:33:45.000000 aps_common_libraries-1.0.4/MANIFEST.in
+-rw-r--r--   0 rook       (505) staff       (20)      851 2023-05-08 17:40:57.532745 aps_common_libraries-1.0.4/PKG-INFO
+-rw-------   0 rook       (505) staff       (20)       46 2022-10-18 15:33:45.000000 aps_common_libraries-1.0.4/README.md
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.511594 aps_common_libraries-1.0.4/__test/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2022-10-18 19:31:39.000000 aps_common_libraries-1.0.4/__test/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)     3721 2022-10-18 19:37:21.000000 aps_common_libraries-1.0.4/__test/test.py
+-rw-r--r--   0 rook       (505) staff       (20)     3711 2022-10-18 19:37:21.000000 aps_common_libraries-1.0.4/__test/test2.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.511992 aps_common_libraries-1.0.4/aps/
+-rw-------   0 rook       (505) staff       (20)     3471 2022-10-18 15:33:45.000000 aps_common_libraries-1.0.4/aps/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.514638 aps_common_libraries-1.0.4/aps/common/
+-rw-r--r--   0 rook       (505) staff       (20)     3426 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.515620 aps_common_libraries-1.0.4/aps/common/__test/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/__test/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)     3683 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/__test/singletons.py
+-rw-r--r--   0 rook       (505) staff       (20)      548 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/__test/test.py
+-rw-r--r--   0 rook       (505) staff       (20)     5739 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/__test/test2.py
+-rw-r--r--   0 rook       (505) staff       (20)    10116 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/initializer.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.517291 aps_common_libraries-1.0.4/aps/common/io/
+-rw-r--r--   0 rook       (505) staff       (20)     3344 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/io/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)     4627 2023-02-10 21:12:46.000000 aps_common_libraries-1.0.4/aps/common/io/printout.py
+-rw-r--r--   0 rook       (505) staff       (20)     3693 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/io/sys_commands.py
+-rw-r--r--   0 rook       (505) staff       (20)     4434 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/io/tcp_client.py
+-rw-r--r--   0 rook       (505) staff       (20)     8754 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/io/tiff_file.py
+-rw-r--r--   0 rook       (505) staff       (20)    20774 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/logger.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.517597 aps_common_libraries-1.0.4/aps/common/measurment/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.518403 aps_common_libraries-1.0.4/aps/common/measurment/beamline/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)    10472 2023-03-27 20:18:11.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/image_collector.py
+-rw-r--r--   0 rook       (505) staff       (20)    32561 2023-03-31 19:33:20.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/image_processor.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.523998 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/
+-rw-r--r--   0 rook       (505) staff       (20)     5136 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/SPINNet_estimate.py
+-rw-r--r--   0 rook       (505) staff       (20)    45615 2022-11-26 21:02:19.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/WXST.py
+-rw-r--r--   0 rook       (505) staff       (20)     3453 2022-11-26 21:02:19.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)    14796 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/diffraction_process.py
+-rw-r--r--   0 rook       (505) staff       (20)      840 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/euclidean_dist.py
+-rw-r--r--   0 rook       (505) staff       (20)    19167 2022-11-26 21:02:19.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/func.py
+-rw-r--r--   0 rook       (505) staff       (20)    22780 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/func_light.py
+-rw-r--r--   0 rook       (505) staff       (20)     2234 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/gui_func.py
+-rw-r--r--   0 rook       (505) staff       (20)     6630 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/integration.py
+-rw-r--r--   0 rook       (505) staff       (20)    77489 2023-03-31 19:33:20.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/main.py
+-rw-r--r--   0 rook       (505) staff       (20)     5787 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/pattern_find.py
+-rw-r--r--   0 rook       (505) staff       (20)     7058 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/pattern_propagate.py
+-rw-r--r--   0 rook       (505) staff       (20)      178 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/utils.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.524825 aps_common_libraries-1.0.4/aps/common/ml/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/ml/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)     6469 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/ml/data_structures.py
+-rw-r--r--   0 rook       (505) staff       (20)     4889 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/ml/mocks.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.526388 aps_common_libraries-1.0.4/aps/common/plot/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/plot/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)    44717 2023-04-06 21:26:23.000000 aps_common_libraries-1.0.4/aps/common/plot/gui.py
+-rw-r--r--   0 rook       (505) staff       (20)     4639 2022-11-21 18:08:48.000000 aps_common_libraries-1.0.4/aps/common/plot/image.py
+-rw-r--r--   0 rook       (505) staff       (20)     6365 2023-02-20 16:38:55.000000 aps_common_libraries-1.0.4/aps/common/plot/qt_application.py
+-rw-r--r--   0 rook       (505) staff       (20)    16735 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/plotter.py
+-rw-r--r--   0 rook       (505) staff       (20)     5229 2023-05-04 16:48:05.000000 aps_common_libraries-1.0.4/aps/common/reflection.py
+-rw-r--r--   0 rook       (505) staff       (20)     5129 2023-03-01 18:43:25.000000 aps_common_libraries-1.0.4/aps/common/registry.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.529185 aps_common_libraries-1.0.4/aps/common/scripts/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2022-11-16 16:15:33.000000 aps_common_libraries-1.0.4/aps/common/scripts/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)     3533 2023-02-08 19:15:29.000000 aps_common_libraries-1.0.4/aps/common/scripts/abstract_command_line_script.py
+-rw-------   0 rook       (505) staff       (20)     3430 2022-10-18 15:35:47.000000 aps_common_libraries-1.0.4/aps/common/scripts/generic_process_manager.py
+-rw-r--r--   0 rook       (505) staff       (20)     7941 2023-02-20 16:38:55.000000 aps_common_libraries-1.0.4/aps/common/scripts/generic_qt_script.py
+-rw-r--r--   0 rook       (505) staff       (20)     4121 2023-02-08 19:15:29.000000 aps_common_libraries-1.0.4/aps/common/scripts/script_data.py
+-rw-r--r--   0 rook       (505) staff       (20)     4576 2022-11-16 16:15:33.000000 aps_common_libraries-1.0.4/aps/common/scripts/script_registry.py
+-rw-r--r--   0 rook       (505) staff       (20)     4677 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/singleton.py
+-rw-r--r--   0 rook       (505) staff       (20)    10093 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/aps/common/traffic_light.py
+-rw-r--r--   0 rook       (505) staff       (20)     3543 2023-05-04 16:48:05.000000 aps_common_libraries-1.0.4/aps/common/utilities.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.530685 aps_common_libraries-1.0.4/aps/common/widgets/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/widgets/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)     4081 2022-11-08 20:45:37.000000 aps_common_libraries-1.0.4/aps/common/widgets/close_app_widget.py
+-rw-r--r--   0 rook       (505) staff       (20)     5532 2023-03-01 18:43:25.000000 aps_common_libraries-1.0.4/aps/common/widgets/context_widget.py
+-rw-r--r--   0 rook       (505) staff       (20)     8506 2023-02-13 20:12:14.000000 aps_common_libraries-1.0.4/aps/common/widgets/generic_widget.py
+-rw-r--r--   0 rook       (505) staff       (20)     6095 2023-02-20 16:38:55.000000 aps_common_libraries-1.0.4/aps/common/widgets/log_stream_widget.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-05-08 17:40:57.532457 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/
+-rw-r--r--   0 rook       (505) staff       (20)      851 2023-05-08 17:40:57.000000 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/PKG-INFO
+-rw-r--r--   0 rook       (505) staff       (20)     2318 2023-05-08 17:40:57.000000 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/SOURCES.txt
+-rw-r--r--   0 rook       (505) staff       (20)        1 2023-05-08 17:40:57.000000 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/dependency_links.txt
+-rw-r--r--   0 rook       (505) staff       (20)       15 2023-05-08 17:40:57.000000 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/namespace_packages.txt
+-rw-r--r--   0 rook       (505) staff       (20)        1 2022-10-18 16:03:55.000000 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/not-zip-safe
+-rw-r--r--   0 rook       (505) staff       (20)      150 2023-05-08 17:40:57.000000 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/requires.txt
+-rw-r--r--   0 rook       (505) staff       (20)       11 2023-05-08 17:40:57.000000 aps_common_libraries-1.0.4/aps_common_libraries.egg-info/top_level.txt
+-rw-r--r--   0 rook       (505) staff       (20)       38 2023-05-08 17:40:57.533011 aps_common_libraries-1.0.4/setup.cfg
+-rw-r--r--   0 rook       (505) staff       (20)     5571 2023-05-05 15:05:12.000000 aps_common_libraries-1.0.4/setup.py
```

### Comparing `aps_common_libraries-1.0.3/LICENSE` & `aps_common_libraries-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/LICENSE.pdf` & `aps_common_libraries-1.0.4/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/PKG-INFO` & `aps_common_libraries-1.0.4/aps_common_libraries.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 1.2
-Name: aps_common_libraries
-Version: 1.0.3
+Metadata-Version: 2.1
+Name: aps-common-libraries
+Version: 1.0.4
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
+Download-URL: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
-Download-URL: https://github.com/APS-XSD-OPT-Group/Common-Libraries
-Description: # Common-Libraries
-        General Purpose Libraries 
-        
 Keywords: dictionary,glossary,synchrotronsimulation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
+License-File: LICENSE
+
+# Common-Libraries
+General Purpose Libraries
```

### Comparing `aps_common_libraries-1.0.3/aps/__init__.py` & `aps_common_libraries-1.0.4/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/__init__.py` & `aps_common_libraries-1.0.4/aps/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/__test/__init__.py` & `aps_common_libraries-1.0.4/aps/common/__test/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/__test/test.py` & `aps_common_libraries-1.0.4/aps/common/__test/test.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/initializer.py` & `aps_common_libraries-1.0.4/aps/common/initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,12 +188,12 @@
 # Factory Methods
 
 def register_ini_instance(ini_mode=IniMode.LOCAL_FILE, reset=False, application_name=None, **kwargs):
     if reset: __IniRegistry.Instance().reset(application_name)
     if ini_mode == IniMode.LOCAL_FILE: __IniRegistry.Instance().register_ini(__LocalIniFile(**kwargs), application_name)
     elif ini_mode == IniMode.NONE:     __IniRegistry.Instance().register_ini(__NullIni(), application_name)
 
-def get_registered_ini_instance(application_name=None):
+def get_registered_ini_instance(application_name=None) -> IniFacade:
     return __IniRegistry.Instance().get_ini_instance(application_name)
```

### Comparing `aps_common_libraries-1.0.3/aps/common/io/__init__.py` & `aps_common_libraries-1.0.4/aps/common/io/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/io/printout.py` & `aps_common_libraries-1.0.4/aps/common/io/printout.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/io/tcp_client.py` & `aps_common_libraries-1.0.4/aps/common/io/tcp_client.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/io/tiff_file.py` & `aps_common_libraries-1.0.4/aps/common/io/tiff_file.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/logger.py` & `aps_common_libraries-1.0.4/aps/common/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,19 +407,19 @@
 def register_logger_single_instance(stream=DEFAULT_STREAM, logger_mode=LoggerMode.FULL, reset=False, application_name=None, replace=False):
     if reset: __LoggerRegistry.Instance().reset(application_name)
     if logger_mode==LoggerMode.FULL:      __LoggerRegistry.Instance().register_logger(__FullLogger(stream), application_name, replace)
     elif logger_mode==LoggerMode.NONE:    __LoggerRegistry.Instance().register_logger(__NullLogger(stream), application_name, replace)
     elif logger_mode==LoggerMode.WARNING: __LoggerRegistry.Instance().register_logger(__WarningLogger(stream), application_name, replace)
     elif logger_mode==LoggerMode.ERROR:   __LoggerRegistry.Instance().register_logger(__ErrorLogger(stream), application_name, replace)
 
-def get_registered_logger_instance(application_name=None):
+def get_registered_logger_instance(application_name=None) -> LoggerFacade:
     return __LoggerRegistry.Instance().get_logger_instance(application_name)
 
 def register_secondary_logger(stream=DEFAULT_STREAM, logger_mode=LoggerMode.FULL, logger_name=SECONDARY_LOGGER, application_name=None):
     if logger_mode==LoggerMode.FULL:      __SecondaryLoggerRegistry.Instance().register_logger(__FullLogger(stream), logger_name, application_name)
     elif logger_mode==LoggerMode.NONE:    __SecondaryLoggerRegistry.Instance().register_logger(__NullLogger(stream), logger_name, application_name)
     elif logger_mode==LoggerMode.WARNING: __SecondaryLoggerRegistry.Instance().register_logger(__WarningLogger(stream), logger_name, application_name)
     elif logger_mode==LoggerMode.ERROR:   __SecondaryLoggerRegistry.Instance().register_logger(__ErrorLogger(stream), logger_name, application_name)
     
-def get_registered_secondary_logger(logger_name=SECONDARY_LOGGER, application_name=None):
+def get_registered_secondary_logger(logger_name=SECONDARY_LOGGER, application_name=None) -> LoggerFacade:
     return __SecondaryLoggerRegistry.Instance().get_logger_instance(logger_name, application_name)
```

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/__init__.py` & `aps_common_libraries-1.0.4/__test/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/__init__.py` & `aps_common_libraries-1.0.4/aps/common/measurment/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_collector.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/image_collector.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_processor.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/image_processor.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/SPINNet_estimate.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/SPINNet_estimate.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-'''
-@Time    	: 08 / 19 / 2022
-@Author  	: Zhi Qiao
-@Contact	: z.qiao1989@gmail.com
-@File    	: SPINNet_estimate.py
-@Software	: AbsolutePhase
-@Desc		: use SPINNet to get the phase based on the simulated reference and measured sample images.
-'''
-
-import torch
-import math
-import numpy as np
-import os
-import json
-import h5py
-import sys
-
-# adding SPINNet folder to the system path
-sys.path.insert(0, '../SPINNet/PhaseOnly/')
-from DS_network import Network
-
-
-##########################################################
-def write_h5(result_path, file_name, data_dict):
-    ''' this function is used to save the variables in *args to hdf5 file
-        args are in format: {'name': data}
-    '''
-    if not os.path.exists(result_path):
-        os.makedirs(result_path)
-    with h5py.File(os.path.join(result_path, file_name+'.hdf5'), 'w') as f:
-        for key_name in data_dict:
-            f.create_dataset(key_name, data=data_dict[key_name], compression="gzip", compression_opts=9)
-    print('result hdf5 file : {} saved'.format(file_name+'.hdf5'))
-
-class args_setting:
-    def __init__(self, dict_para):
-
-        self.device = dict_para['device']
-        self.OutputFolder = dict_para['OutputFolder']
-        self.DataFolder = dict_para['DataFolder']
-        self.TestFolder = dict_para['TestFolder']
-        self.num_workers = dict_para['num_workers']
-        self.batch_size = dict_para['batch_size']
-        self.epoch = dict_para['epoch']
-        self.lr = dict_para['lr']
-        self.lv_chs = dict_para['lv_chs']
-        self.output_level = dict_para['output_level']
-        self.batch_norm = dict_para['batch_norm']
-        self.corr = dict_para['corr']
-        self.corr_activation = dict_para['corr_activation']
-        self.search_range = dict_para['search_range']
-        self.residual = dict_para['residual']
-        self.fp16 = dict_para['fp16']
-        self.with_refiner = dict_para['with_refiner']
-        self.load_all_data = dict_para['load_all_data']
-        self.load_check_point = dict_para['load_check_point']
-        self.device_type = torch.device(self.device)
-        self.num_levels = len(self.lv_chs)
-
-
-def estimate(img_stack, model, args):
-    """
-    inference function of SPINNet using the trained model
-
-    Args:
-        img_stack (ndarray): input ref and sample image stack
-        model (torch.model): loaded trained torch model
-        args (dict): parameters of the trained model
-
-    Returns:
-        _type_: _description_
-    """
-    intWidth = img_stack[0].shape[-1]
-    intHeight = img_stack[0].shape[-2]
-
-    intPreprocessedWidth = int(math.floor(math.ceil(intWidth / 64.0) * 64.0))
-    intPreprocessedHeight = int(math.floor(math.ceil(intHeight / 64.0) * 64.0))
-
-    img_stack = np.array(img_stack)
-    img_stack = torch.FloatTensor(
-        np.ascontiguousarray(
-            img_stack[:, :, :].astype(np.float32)))
-
-    img_stack = torch.nn.functional.interpolate(
-                            input=img_stack,
-                            size=(intPreprocessedHeight, intPreprocessedWidth),
-                            mode='bilinear',
-                            align_corners=True)
-
-
-    with torch.no_grad():
-        # Transfer to GPU
-        img_stack = img_stack.to(args.device_type)
-        flow_predict = model(img_stack)
-        
-        tenFlow = torch.nn.functional.interpolate(
-                        input=flow_predict,
-                        size=(intHeight, intWidth),
-                        mode='bilinear',
-                        align_corners=True)
-        
-        tenFlow = tenFlow.cpu().detach().numpy()
-        
-        tenFlow[:, 0, :, :] *= float(intWidth) / float(intPreprocessedWidth)
-        tenFlow[:, 1, :, :] *= float(intHeight) / float(intPreprocessedHeight)
-
-        return tenFlow[0, :, :, :]
-
-
-def SPINNet_estimate(ref, img, model_path, setting_path, device):
-    """
-    SPINNet_estimate to predict the phase according to ref and img
-
-    Args:
-        ref (ndarray): ref image
-        img (ndarray): sample image
-        model_path (str): saved model path
-        setting_path (str): saved setting path of the trained model
-        device (srt): use cuda or cpu
-    """
-
-    # load the setting from the trained model
-    with open(setting_path) as f:
-        setting_dict = json.load(f)
-
-    setting_dict['device'] = device
-
-    args = args_setting(setting_dict)
-
-    # print(args.__dict__)
-    
-    torch.manual_seed(42)
-    model = Network(args).to(args.device_type)
-    checkpoint = torch.load(model_path, map_location=args.device_type)
-    print('load checkpoint from file: {}'.format(model_path))
-    
-    model.load_state_dict(checkpoint['model_state_dict'])
-
-    model.eval()
-
-    # load data
-    
-    f_max = np.amax([ref, img])
-    img = img / f_max
-    ref = ref / f_max
-
-    img_stack = []
-    img_stack.append(np.array([ref, img]))
-
-    tenFlow = estimate(img_stack, model, args)
-    # print(tenFlow.shape)
-    displace_x = tenFlow[0, :, :] - np.mean(tenFlow[0, 0:50, 0:50])
-    displace_y = tenFlow[1, :, ] - np.mean(tenFlow[1, 0:50, 0:50])
-
-    return displace_y, displace_x
-        
-
-        
-    
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+'''
+@Time    	: 08 / 19 / 2022
+@Author  	: Zhi Qiao
+@Contact	: z.qiao1989@gmail.com
+@File    	: SPINNet_estimate.py
+@Software	: AbsolutePhase
+@Desc		: use SPINNet to get the phase based on the simulated reference and measured sample images.
+'''
+
+import torch
+import math
+import numpy as np
+import os
+import json
+import h5py
+import sys
+
+# adding SPINNet folder to the system path
+sys.path.insert(0, '../SPINNet/PhaseOnly/')
+from DS_network import Network
+
+
+##########################################################
+def write_h5(result_path, file_name, data_dict):
+    ''' this function is used to save the variables in *args to hdf5 file
+        args are in format: {'name': data}
+    '''
+    if not os.path.exists(result_path):
+        os.makedirs(result_path)
+    with h5py.File(os.path.join(result_path, file_name+'.hdf5'), 'w') as f:
+        for key_name in data_dict:
+            f.create_dataset(key_name, data=data_dict[key_name], compression="gzip", compression_opts=9)
+    print('result hdf5 file : {} saved'.format(file_name+'.hdf5'))
+
+class args_setting:
+    def __init__(self, dict_para):
+
+        self.device = dict_para['device']
+        self.OutputFolder = dict_para['OutputFolder']
+        self.DataFolder = dict_para['DataFolder']
+        self.TestFolder = dict_para['TestFolder']
+        self.num_workers = dict_para['num_workers']
+        self.batch_size = dict_para['batch_size']
+        self.epoch = dict_para['epoch']
+        self.lr = dict_para['lr']
+        self.lv_chs = dict_para['lv_chs']
+        self.output_level = dict_para['output_level']
+        self.batch_norm = dict_para['batch_norm']
+        self.corr = dict_para['corr']
+        self.corr_activation = dict_para['corr_activation']
+        self.search_range = dict_para['search_range']
+        self.residual = dict_para['residual']
+        self.fp16 = dict_para['fp16']
+        self.with_refiner = dict_para['with_refiner']
+        self.load_all_data = dict_para['load_all_data']
+        self.load_check_point = dict_para['load_check_point']
+        self.device_type = torch.device(self.device)
+        self.num_levels = len(self.lv_chs)
+
+
+def estimate(img_stack, model, args):
+    """
+    inference function of SPINNet using the trained model
+
+    Args:
+        img_stack (ndarray): input ref and sample image stack
+        model (torch.model): loaded trained torch model
+        args (dict): parameters of the trained model
+
+    Returns:
+        _type_: _description_
+    """
+    intWidth = img_stack[0].shape[-1]
+    intHeight = img_stack[0].shape[-2]
+
+    intPreprocessedWidth = int(math.floor(math.ceil(intWidth / 64.0) * 64.0))
+    intPreprocessedHeight = int(math.floor(math.ceil(intHeight / 64.0) * 64.0))
+
+    img_stack = np.array(img_stack)
+    img_stack = torch.FloatTensor(
+        np.ascontiguousarray(
+            img_stack[:, :, :].astype(np.float32)))
+
+    img_stack = torch.nn.functional.interpolate(
+                            input=img_stack,
+                            size=(intPreprocessedHeight, intPreprocessedWidth),
+                            mode='bilinear',
+                            align_corners=True)
+
+
+    with torch.no_grad():
+        # Transfer to GPU
+        img_stack = img_stack.to(args.device_type)
+        flow_predict = model(img_stack)
+        
+        tenFlow = torch.nn.functional.interpolate(
+                        input=flow_predict,
+                        size=(intHeight, intWidth),
+                        mode='bilinear',
+                        align_corners=True)
+        
+        tenFlow = tenFlow.cpu().detach().numpy()
+        
+        tenFlow[:, 0, :, :] *= float(intWidth) / float(intPreprocessedWidth)
+        tenFlow[:, 1, :, :] *= float(intHeight) / float(intPreprocessedHeight)
+
+        return tenFlow[0, :, :, :]
+
+
+def SPINNet_estimate(ref, img, model_path, setting_path, device):
+    """
+    SPINNet_estimate to predict the phase according to ref and img
+
+    Args:
+        ref (ndarray): ref image
+        img (ndarray): sample image
+        model_path (str): saved model path
+        setting_path (str): saved setting path of the trained model
+        device (srt): use cuda or cpu
+    """
+
+    # load the setting from the trained model
+    with open(setting_path) as f:
+        setting_dict = json.load(f)
+
+    setting_dict['device'] = device
+
+    args = args_setting(setting_dict)
+
+    # print(args.__dict__)
+    
+    torch.manual_seed(42)
+    model = Network(args).to(args.device_type)
+    checkpoint = torch.load(model_path, map_location=args.device_type)
+    print('load checkpoint from file: {}'.format(model_path))
+    
+    model.load_state_dict(checkpoint['model_state_dict'])
+
+    model.eval()
+
+    # load data
+    
+    f_max = np.amax([ref, img])
+    img = img / f_max
+    ref = ref / f_max
+
+    img_stack = []
+    img_stack.append(np.array([ref, img]))
+
+    tenFlow = estimate(img_stack, model, args)
+    # print(tenFlow.shape)
+    displace_x = tenFlow[0, :, :] - np.mean(tenFlow[0, 0:50, 0:50])
+    displace_y = tenFlow[1, :, ] - np.mean(tenFlow[1, 0:50, 0:50])
+
+    return displace_y, displace_x
+        
+
+        
+
```

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/WXST.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/WXST.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/__init__.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/diffraction_process.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/diffraction_process.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,422 +1,422 @@
-'''
-This is the python version code for diffraction
-                dxy             the pixel pitch of the object
-                z               the distance of the propagation
-                wavelength      the wave length
-                X,Y             meshgrid of coordinate
-                data            input object
-                diff_method     calculation method:
-                                QPF: quadratic phase fresnel diffraction
-                                IR:  convolution transfer methord (for far field)
-                                TF: spectral transfer method    (for near field)
-                                RS: Rayleigh-Sommerfield method
-                                default: use IR(far) and TF(near)
-'''
-import numpy as np
-import sys
-import scipy.interpolate as sfit
-from skimage.restoration import unwrap_phase
-
-
-def diffraction_prop(data, dxy, z, wavelength, diff_method='default'):
-    '''
-    This is the python version code for diffraction
-        dxy             the pixel pitch of the object
-        z               the distance of the propagation
-        wavelength      the wave length
-        X,Y             meshgrid of coordinate
-        data            input object
-        diff_method     calculation method:
-                        QPF: quadratic phase fresnel diffraction
-                        IR:  convolution transfer methord (for far field)
-                        TF: spectral transfer method    (for near field)
-                        RS: Rayleigh-Sommerfield method
-                        GS: phase gradient shift, approximation of near field diffraction
-                        default: use IR(far) and TF(near)
-        if donot specify, the method will be determined by dxy and L(source length)
-    '''
-    if diff_method == 'default':
-        # the method is not defined
-        # the array size
-        M = data.shape[0]
-        # the source plane size
-        L = M * dxy
-        if dxy > wavelength * z / L:
-            # use TF method for near field
-            diff, L_out = prop_TF(data, dxy, z, wavelength)
-        else:
-            # use IR method for far field
-            diff, L_out = prop_IR(data, dxy, z, wavelength)
-
-    elif diff_method == 'QPF':
-        # the method is defined
-        # use QPF method
-        diff, L_out = prop_QPF(data, dxy, z, wavelength)
-    elif diff_method == 'IR':
-        # use IR method
-        diff, L_out = prop_IR(data, dxy, z, wavelength)
-    elif diff_method == 'TF':
-        # use TF method
-        diff, L_out = prop_TF(data, dxy, z, wavelength)
-    elif diff_method == 'RS':
-        # use RS method
-        diff, L_out = prop_RS(data, dxy, z, wavelength)
-    elif diff_method == 'GS':
-        # use phase gradient shift method
-        diff, L_out = prop_GS(data, dxy, z, wavelength)
-    elif diff_method == 'GeoFlow':
-        # use phase gradient shift method
-        diff, L_out = prop_GeoFlow(np.abs(data)**2, np.angle(data), dxy, z, wavelength)
-    else:
-        sys.exit('Error: no such diffraction method; must be TF, IR, RS, QPF')
-
-    return diff, L_out
-
-
-def prop_GeoFlow(I_ref, phi, dxy, z, wavelength):
-    '''
-        here use the Geometric flow method to calculate the img after propagation
-        input:
-            I_ref:                  the ref intensity, I_ref=abs(A_ref)**2
-            phi:                    the phase
-            dxy:                    pixel size
-            z:                      the propagation distance
-            wavelength:             the wavelength
-        output:
-            I_img:                  the intensity after propagation
-        Formula:    I_ref - I_img = diff_T(I_ref * D_T(x, y))
-                    D_T(x, y) is the displacement along x and y axis
-    '''
-    dim = I_ref.shape
-    k_wave = 2 * np.pi / wavelength
-
-    x_axis = dxy * (np.arange(dim[1]) - round(dim[1]/2))
-    y_axis = dxy * (np.arange(dim[0]) - round(dim[0]/2))
-    dk_x = 2*np.pi / (dim[1]*dxy)
-    dk_y = 2*np.pi / (dim[0]*dxy)
-    # dk_x = 1 / (dim[1]*dxy)
-    # dk_y = 1 / (dim[0]*dxy)
-
-    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
-    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
-
-    k_YY, k_XX = np.meshgrid(ky, kx, indexing='ij')
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    '''
-        to calculate the diff_T:
-            diff_T = 1j * F^(-1){(kx, ky) * F{}}
-    '''
-    # axis=1 direction deviation
-    # nabla_x_kern = np.array([[0, 0, 0], [-1, 1, 0], [0, 0, 0]])
-    # # axis=0 direction deviation
-    # nabla_y_kern = np.array([[0, -1, 0], [0, 1, 0], [0, 0, 0]])
-    # # 2nd nabla deviation
-    # nabla_2_kern = np.array([[0, 1, 0], [1, -4, 1], [0, 1, 0]])
-    # bc = 'reflect'
-    # nabla = lambda phi: np.array([sf.correlate(phi, nabla_x_kern, mode=bc), sf.correlate(phi, nabla_y_kern, mode=bc)]) / (dxy)
-    # nabla2 = lambda phi: sf.correlate(phi, nabla_2_kern, mode=bc) / dxy**2
-    nabla_T = lambda x: 1j * np.array([ifft2(k_YY * fft2(x)), ifft2(k_XX * fft2(x))])
-    # nabla_times = lambda x, y: x[0]*y[0] + x[1]*y[1]
-    # nabla2 = lambda vec: ifft2(-(k_XX**2 + k_YY**2) * fft2(vec))
-
-    # I_img = I_ref - (z/k_wave * (nabla_times(nabla(I_ref), nabla(phi)) + I_ref * nabla2(phi)))
-    # D_T = np.real(diff_T(z / k_wave * phi))
-    
-    # D_x = np.real(ifft2((1j*k_XX - k_YY) * fft2(phi * z / k_wave)))
-    # D_y = np.imag(ifft2((1j*k_XX - k_YY) * fft2(phi * z / k_wave)))
-    [D_y, D_x] = np.real(nabla_T(phi * z / k_wave))
-    # use the formula to calculate intensity after propagation
-    # I_ref - I_img = diff_T(I_ref * D_T(x, y))
-
-    I_img = I_ref - np.real(1j*ifft2(k_XX * fft2(I_ref * D_x) + k_YY * fft2(I_ref * D_y)))
-
-    return I_img, dxy * I_ref.shape[0]
-
-
-def prop_GS(data, dxy, z , wavelength):
-    '''
-    Use phase gradient shift method for the diffraction. Assume same x and y lengthss and uniform sampling
-        data:        source plane field
-        dxy:         source and observation plane pixel size
-        wavelength:  wavelength
-        z:           propagation distance
-        GS method
-        dx, dy = -lambda*z/2/pi * nabla(phase)
-
-    '''
-    # phase of the data
-    L = dxy * data.shape[0]
-    phi = unwrap_phase(np.angle(data))
-    I_amp = np.abs(data) ** 2
-    
-    cons = wavelength * z / (2 * np.pi)
-
-    x_axis = range(I_amp.shape[1])
-    y_axis = range(I_amp.shape[0])
-    YY_axis, XX_axis = np.meshgrid(y_axis, x_axis, indexing='ij')
-
-    wx = np.gradient(phi, axis=1) * cons / dxy**2
-    wy = np.gradient(phi, axis=0) * cons / dxy**2
-    YY_axis = YY_axis - wy
-    XX_axis = XX_axis - wx
-
-    f_amp = sfit.RegularGridInterpolator((y_axis, x_axis), I_amp, 
-                                                  bounds_error = False, 
-                                                  method = 'nearest', 
-                                                  fill_value = np.mean(I_amp))
-    f_phase = sfit.RegularGridInterpolator((y_axis, x_axis), phi, 
-                                                  bounds_error = False, 
-                                                  method = 'nearest', 
-                                                  fill_value = np.mean(phi))
-    # recently inverted this line
-    pts = (np.array([np.ndarray.flatten(YY_axis), np.ndarray.flatten(XX_axis)])
-           .transpose())
-
-    I_new = np.reshape(f_amp(pts), I_amp.shape)
-    phi_new = np.reshape(f_phase(pts), phi.shape)
-
-    Amp_new = np.sqrt(I_new) * np.exp(1j * phi_new)
-
-    return Amp_new, L
-
-
-
-def prop_RS(data, dxy, z, wavelength):
-    '''
-    Use Rayleigh-Sommerfield method for the diffraction. Assume same x and y lengthss and uniform sampling
-        data:        source plane field
-        dxy:         source and observation plane pixel size
-        wavelength:  wavelength
-        z:           propagation distance
-        RS method
-        u2(x,y)=ifft(fft(u1)*H); H=exp(jkz(1-(lambdafx)^2-(lambdafy)^2)^0.5)
-
-    '''
-    # the array size
-    M = data.shape[0]
-    N = data.shape[1]
-    # source plane size
-    L_y = dxy * M
-    L_x = dxy * N
-    # wavenumber
-    k = 2 * np.pi / wavelength
-    # frequency resolution
-    dfx = 1/L_x
-    dfy = 1/L_y
-    fy = np.arange(-M/2, M/2) * dfy
-    fx = np.arange(-N/2, N/2) * dfx
-    FX, FY = np.meshgrid(fx, fy)
-
-    L_out = [L_y, L_x]
-    if z > 0:
-        # transform function
-        H = np.exp(1j*k*z*np.sqrt(1-(wavelength*FX)**2-(wavelength*FY)**2))
-        # u2(x,y)=ifft(fft(u1)*H)
-        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
-    else:
-        # transform function
-        H = np.exp(1j*k*z*np.sqrt(1-(wavelength*FX)**2-(wavelength*FY)**2))
-        # u2(x,y)=ifft(fft(u1)*H)
-        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
-
-    return diff, L_out
-
-
-def prop_QPF(data, dxy, z, wavelength):
-    '''
-    this method use the quadratic phase method to calculate fresnel diffraction
-        data:        source plane field
-        dxy:         source and observation plane pixel size
-        wavelength:  wavelength
-        z:           propagation distance
-        QPF:
-            U2(x,y) = exp(jkz)/(j*lambda*z)*exp(jk/2z*(x^2+y^2))*int(U1(xx,yy)exp(jk/2z*(xx^2+yy^2))*exp(-jk/z(x*xx+y*yy))dxxdyy)
-
-    '''
-    # the array size
-    M = data.shape[0]
-    N = data.shape[1]
-    # source plane size
-    L_y = dxy * M
-    L_x = dxy * N
-    # wavenumber
-    k = 2 * np.pi / wavelength
-    # spatial resolution
-    y = np.arange(-N/2, N/2) * dxy
-    x = np.arange(-M/2, M/2) * dxy
-    XX, YY = np.meshgrid(x, y)
-    # frequency resolution
-    dfx = 1/L_x * wavelength * z
-    dfy = 1/L_y * wavelength * z
-    fy = np.arange(-M/2, M/2) * dfy
-    fx = np.arange(-N/2, N/2) * dfx
-
-    FX, FY = np.meshgrid(fx, fy)
-
-    # the out plane size
-    L_out = wavelength * z / dxy
-
-    if z > 0:
-        pf = np.exp(1j*k*z) * np.exp(1j*k/(2*z)*(FX**2 + FY**2))
-        kern = data * np.exp(1j*k/(2*z)*(XX**2 + YY**2))
-        cgh = np.fft.fft2(np.fft.ifftshift(kern))
-        diff = np.fft.fftshift(cgh * np.fft.ifftshift(pf))
-    else:
-        pf = np.exp(1j*k*z) * np.exp(1j*k/(2*z)*(XX**2 + YY**2))
-        kern = data * np.exp(1j*k/(2*z)*(FX**2 + FY**2))
-        cgh = np.fft.ifft2(np.fft.ifftshift(kern))
-        diff = np.fft.fftshift(cgh)*pf
-
-    return diff, L_out
-
-
-def prop_TF(data, dxy, wavelength, z):
-    '''
-    this method use the transfer function approach to calculate fresnel diffraction
-        data:        source plane field
-        dxy:         source and observation plane pixel size
-        wavelength:  wavelength
-        z:           propagation distance
-        TF:
-            U2(x,y)=ifft(fft(u1)*H); H=exp(jkz)*exp(-j*pi*lambda*z*(fx^2+fy^2))
-
-    '''
-    # the array size
-    M = data.shape[0]
-    N = data.shape[1]
-    # source plane size
-    L_x = dxy * N
-    L_y = dxy * M
-    # wavenumber
-    k = 2 * np.pi / wavelength
-    # frequency resolution
-    dfx = 1/L_x
-    dfy = 1/L_y
-    fy = np.arange(-M/2, M/2) * dfy
-    fx = np.arange(-N/2, N/2) * dfx
-
-    FX, FY = np.meshgrid(fx, fy)
-
-    L_out = [L_y, L_x]
-
-    if z > 0:
-        # transfer function
-        H = np.exp(1j*k*z) * np.exp(-1j*wavelength*z*np.pi*(FX**2 + FY**2))
-        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
-    else:
-        # transfer function
-        H = np.exp(1j*k*z) * np.exp(-1j*wavelength*z*np.pi*(FX**2 + FY**2))
-        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
-
-    return diff, L_out
-
-
-def prop_IR(data, dxy, wavelength, z):
-    '''
-    this method use the impulse response approach to calculate fresnel diffraction
-        data:        source plane field
-        dxy:         source and observation plane pixel size
-        wavelength:  wavelength
-        z:           propagation distance
-        IR:
-            U2(x,y)=ifft(fft(u1)*H); H=fft(exp(jkz)/(jlambda*z)*exp(j*k/2z*(x^2+y^2)))
-
-    '''
-    # the array size
-    M = data.shape[0]
-    # source plane size
-    L = dxy * M
-    # wavenumber
-    k = 2 * np.pi / wavelength
-    # spatial resolution
-    x = np.arange(-M/2, M/2) * dxy
-    XX, YY = np.meshgrid(x, x)
-
-    L_out = L
-
-    if z > 0:
-        # impule response
-        h = 1/(1j*wavelength*z) * np.exp(1j*k/(2*z)*(XX**2 + YY**2))
-        # transfer function
-        H = np.fft.fft2(np.fft.ifftshift(h)) * dxy**2
-        U1 = np.fft.fft2(np.fft.ifftshift(data))
-        diff = np.fft.fftshift(np.fft.ifft2(U1 * H))
-    else:
-        # impule response
-        h = 1/(-1j*wavelength*z) * np.exp(1j*k/(-2*z)*(XX**2 + YY**2))
-        # transfer function
-        H = np.fft.fft2(np.fft.ifftshift(h)) * dxy**2
-        U1 = np.fft.fft2(np.fft.ifftshift(data))
-        diff = np.fft.fftshift(np.fft.ifft2(U1 / H))
-
-    return diff, L_out
-
-
-# here is the old propagation function for Fresnel diffraction
-def fresnel_propagation(data, dxy, z, wavelength):
-
-    (M, N) = data.shape
-    k = 2 * np.pi / wavelength
-    # the coordinate grid
-    if M % 2 == 0:
-        M_grid = np.arange(-M/2, M/2)
-    else:
-        M_grid = np.arange(-(M-1)/2, (M-1)/2+1)
-    lx = M_grid * dxy
-    XX, YY = np.meshgrid(lx, lx)
-
-    # the coordinate grid on the output plane
-    fc = 1/dxy
-    fu = wavelength * z * fc
-    lu = M_grid * fu / M
-    Fx, Fy = np.meshgrid(lu, lu)
-
-    if z > 0:
-        pf = np.exp(1j*k*z) * np.exp(1j*k*(Fx**2 + Fy**2)/2/z)
-        kern = data * np.exp(1j*k*(XX**2 + YY**2)/2/z)
-        cgh = np.fft.fft2(np.fft.fftshift(kern))
-        OUT = np.fft.fftshift(cgh * np.fft.fftshift(pf))
-    else:
-        pf = np.exp(1j*k*z) * np.exp(1j*k*(XX**2 + YY**2)/2/z)
-        cgh = np.fft.ifft2(np.fft.fftshift(data*np.exp(1j*k*(Fx**2+Fy**2)/2/z)))
-        OUT = np.fft.fftshift(cgh)*pf
-
-    return OUT
-
-
-
-def prop_TF_2d(data, dxy, wavelength, z):
-    '''
-    this method use the transfer function approach to calculate fresnel diffraction
-        data:        source plane field
-        dxy:         source and observation plane pixel size
-        wavelength:  wavelength
-        z:           propagation distance, [zx, zy]
-        TF:
-            U2(x,y)=ifft(fft(u1)*H); H=exp(jkz)*exp(-j*pi*lambda*z*(fx^2+fy^2))
-
-    '''
-    # the array size
-    M = data.shape[0]
-    N = data.shape[1]
-    # source plane size
-    L_x = dxy * N
-    L_y = dxy * M
-    # wavenumber
-    k = 2 * np.pi / wavelength
-    # frequency resolution
-    dfx = 1/L_x
-    dfy = 1/L_y
-    fy = np.arange(-M/2, M/2) * dfy
-    fx = np.arange(-N/2, N/2) * dfx
-
-    FX, FY = np.meshgrid(fx, fy)
-
-    L_out = [L_y, L_x]
-
-    H = np.exp(-1j*wavelength*np.pi*(z[0] * FX**2 + z[1] * FY**2))
-    diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
-
-    return diff, L_out
-
+'''
+This is the python version code for diffraction
+                dxy             the pixel pitch of the object
+                z               the distance of the propagation
+                wavelength      the wave length
+                X,Y             meshgrid of coordinate
+                data            input object
+                diff_method     calculation method:
+                                QPF: quadratic phase fresnel diffraction
+                                IR:  convolution transfer methord (for far field)
+                                TF: spectral transfer method    (for near field)
+                                RS: Rayleigh-Sommerfield method
+                                default: use IR(far) and TF(near)
+'''
+import numpy as np
+import sys
+import scipy.interpolate as sfit
+from skimage.restoration import unwrap_phase
+
+
+def diffraction_prop(data, dxy, z, wavelength, diff_method='default'):
+    '''
+    This is the python version code for diffraction
+        dxy             the pixel pitch of the object
+        z               the distance of the propagation
+        wavelength      the wave length
+        X,Y             meshgrid of coordinate
+        data            input object
+        diff_method     calculation method:
+                        QPF: quadratic phase fresnel diffraction
+                        IR:  convolution transfer methord (for far field)
+                        TF: spectral transfer method    (for near field)
+                        RS: Rayleigh-Sommerfield method
+                        GS: phase gradient shift, approximation of near field diffraction
+                        default: use IR(far) and TF(near)
+        if donot specify, the method will be determined by dxy and L(source length)
+    '''
+    if diff_method == 'default':
+        # the method is not defined
+        # the array size
+        M = data.shape[0]
+        # the source plane size
+        L = M * dxy
+        if dxy > wavelength * z / L:
+            # use TF method for near field
+            diff, L_out = prop_TF(data, dxy, z, wavelength)
+        else:
+            # use IR method for far field
+            diff, L_out = prop_IR(data, dxy, z, wavelength)
+
+    elif diff_method == 'QPF':
+        # the method is defined
+        # use QPF method
+        diff, L_out = prop_QPF(data, dxy, z, wavelength)
+    elif diff_method == 'IR':
+        # use IR method
+        diff, L_out = prop_IR(data, dxy, z, wavelength)
+    elif diff_method == 'TF':
+        # use TF method
+        diff, L_out = prop_TF(data, dxy, z, wavelength)
+    elif diff_method == 'RS':
+        # use RS method
+        diff, L_out = prop_RS(data, dxy, z, wavelength)
+    elif diff_method == 'GS':
+        # use phase gradient shift method
+        diff, L_out = prop_GS(data, dxy, z, wavelength)
+    elif diff_method == 'GeoFlow':
+        # use phase gradient shift method
+        diff, L_out = prop_GeoFlow(np.abs(data)**2, np.angle(data), dxy, z, wavelength)
+    else:
+        sys.exit('Error: no such diffraction method; must be TF, IR, RS, QPF')
+
+    return diff, L_out
+
+
+def prop_GeoFlow(I_ref, phi, dxy, z, wavelength):
+    '''
+        here use the Geometric flow method to calculate the img after propagation
+        input:
+            I_ref:                  the ref intensity, I_ref=abs(A_ref)**2
+            phi:                    the phase
+            dxy:                    pixel size
+            z:                      the propagation distance
+            wavelength:             the wavelength
+        output:
+            I_img:                  the intensity after propagation
+        Formula:    I_ref - I_img = diff_T(I_ref * D_T(x, y))
+                    D_T(x, y) is the displacement along x and y axis
+    '''
+    dim = I_ref.shape
+    k_wave = 2 * np.pi / wavelength
+
+    x_axis = dxy * (np.arange(dim[1]) - round(dim[1]/2))
+    y_axis = dxy * (np.arange(dim[0]) - round(dim[0]/2))
+    dk_x = 2*np.pi / (dim[1]*dxy)
+    dk_y = 2*np.pi / (dim[0]*dxy)
+    # dk_x = 1 / (dim[1]*dxy)
+    # dk_y = 1 / (dim[0]*dxy)
+
+    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
+    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
+
+    k_YY, k_XX = np.meshgrid(ky, kx, indexing='ij')
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    '''
+        to calculate the diff_T:
+            diff_T = 1j * F^(-1){(kx, ky) * F{}}
+    '''
+    # axis=1 direction deviation
+    # nabla_x_kern = np.array([[0, 0, 0], [-1, 1, 0], [0, 0, 0]])
+    # # axis=0 direction deviation
+    # nabla_y_kern = np.array([[0, -1, 0], [0, 1, 0], [0, 0, 0]])
+    # # 2nd nabla deviation
+    # nabla_2_kern = np.array([[0, 1, 0], [1, -4, 1], [0, 1, 0]])
+    # bc = 'reflect'
+    # nabla = lambda phi: np.array([sf.correlate(phi, nabla_x_kern, mode=bc), sf.correlate(phi, nabla_y_kern, mode=bc)]) / (dxy)
+    # nabla2 = lambda phi: sf.correlate(phi, nabla_2_kern, mode=bc) / dxy**2
+    nabla_T = lambda x: 1j * np.array([ifft2(k_YY * fft2(x)), ifft2(k_XX * fft2(x))])
+    # nabla_times = lambda x, y: x[0]*y[0] + x[1]*y[1]
+    # nabla2 = lambda vec: ifft2(-(k_XX**2 + k_YY**2) * fft2(vec))
+
+    # I_img = I_ref - (z/k_wave * (nabla_times(nabla(I_ref), nabla(phi)) + I_ref * nabla2(phi)))
+    # D_T = np.real(diff_T(z / k_wave * phi))
+    
+    # D_x = np.real(ifft2((1j*k_XX - k_YY) * fft2(phi * z / k_wave)))
+    # D_y = np.imag(ifft2((1j*k_XX - k_YY) * fft2(phi * z / k_wave)))
+    [D_y, D_x] = np.real(nabla_T(phi * z / k_wave))
+    # use the formula to calculate intensity after propagation
+    # I_ref - I_img = diff_T(I_ref * D_T(x, y))
+
+    I_img = I_ref - np.real(1j*ifft2(k_XX * fft2(I_ref * D_x) + k_YY * fft2(I_ref * D_y)))
+
+    return I_img, dxy * I_ref.shape[0]
+
+
+def prop_GS(data, dxy, z , wavelength):
+    '''
+    Use phase gradient shift method for the diffraction. Assume same x and y lengthss and uniform sampling
+        data:        source plane field
+        dxy:         source and observation plane pixel size
+        wavelength:  wavelength
+        z:           propagation distance
+        GS method
+        dx, dy = -lambda*z/2/pi * nabla(phase)
+
+    '''
+    # phase of the data
+    L = dxy * data.shape[0]
+    phi = unwrap_phase(np.angle(data))
+    I_amp = np.abs(data) ** 2
+    
+    cons = wavelength * z / (2 * np.pi)
+
+    x_axis = range(I_amp.shape[1])
+    y_axis = range(I_amp.shape[0])
+    YY_axis, XX_axis = np.meshgrid(y_axis, x_axis, indexing='ij')
+
+    wx = np.gradient(phi, axis=1) * cons / dxy**2
+    wy = np.gradient(phi, axis=0) * cons / dxy**2
+    YY_axis = YY_axis - wy
+    XX_axis = XX_axis - wx
+
+    f_amp = sfit.RegularGridInterpolator((y_axis, x_axis), I_amp, 
+                                                  bounds_error = False, 
+                                                  method = 'nearest', 
+                                                  fill_value = np.mean(I_amp))
+    f_phase = sfit.RegularGridInterpolator((y_axis, x_axis), phi, 
+                                                  bounds_error = False, 
+                                                  method = 'nearest', 
+                                                  fill_value = np.mean(phi))
+    # recently inverted this line
+    pts = (np.array([np.ndarray.flatten(YY_axis), np.ndarray.flatten(XX_axis)])
+           .transpose())
+
+    I_new = np.reshape(f_amp(pts), I_amp.shape)
+    phi_new = np.reshape(f_phase(pts), phi.shape)
+
+    Amp_new = np.sqrt(I_new) * np.exp(1j * phi_new)
+
+    return Amp_new, L
+
+
+
+def prop_RS(data, dxy, z, wavelength):
+    '''
+    Use Rayleigh-Sommerfield method for the diffraction. Assume same x and y lengthss and uniform sampling
+        data:        source plane field
+        dxy:         source and observation plane pixel size
+        wavelength:  wavelength
+        z:           propagation distance
+        RS method
+        u2(x,y)=ifft(fft(u1)*H); H=exp(jkz(1-(lambdafx)^2-(lambdafy)^2)^0.5)
+
+    '''
+    # the array size
+    M = data.shape[0]
+    N = data.shape[1]
+    # source plane size
+    L_y = dxy * M
+    L_x = dxy * N
+    # wavenumber
+    k = 2 * np.pi / wavelength
+    # frequency resolution
+    dfx = 1/L_x
+    dfy = 1/L_y
+    fy = np.arange(-M/2, M/2) * dfy
+    fx = np.arange(-N/2, N/2) * dfx
+    FX, FY = np.meshgrid(fx, fy)
+
+    L_out = [L_y, L_x]
+    if z > 0:
+        # transform function
+        H = np.exp(1j*k*z*np.sqrt(1-(wavelength*FX)**2-(wavelength*FY)**2))
+        # u2(x,y)=ifft(fft(u1)*H)
+        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
+    else:
+        # transform function
+        H = np.exp(1j*k*z*np.sqrt(1-(wavelength*FX)**2-(wavelength*FY)**2))
+        # u2(x,y)=ifft(fft(u1)*H)
+        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
+
+    return diff, L_out
+
+
+def prop_QPF(data, dxy, z, wavelength):
+    '''
+    this method use the quadratic phase method to calculate fresnel diffraction
+        data:        source plane field
+        dxy:         source and observation plane pixel size
+        wavelength:  wavelength
+        z:           propagation distance
+        QPF:
+            U2(x,y) = exp(jkz)/(j*lambda*z)*exp(jk/2z*(x^2+y^2))*int(U1(xx,yy)exp(jk/2z*(xx^2+yy^2))*exp(-jk/z(x*xx+y*yy))dxxdyy)
+
+    '''
+    # the array size
+    M = data.shape[0]
+    N = data.shape[1]
+    # source plane size
+    L_y = dxy * M
+    L_x = dxy * N
+    # wavenumber
+    k = 2 * np.pi / wavelength
+    # spatial resolution
+    y = np.arange(-N/2, N/2) * dxy
+    x = np.arange(-M/2, M/2) * dxy
+    XX, YY = np.meshgrid(x, y)
+    # frequency resolution
+    dfx = 1/L_x * wavelength * z
+    dfy = 1/L_y * wavelength * z
+    fy = np.arange(-M/2, M/2) * dfy
+    fx = np.arange(-N/2, N/2) * dfx
+
+    FX, FY = np.meshgrid(fx, fy)
+
+    # the out plane size
+    L_out = wavelength * z / dxy
+
+    if z > 0:
+        pf = np.exp(1j*k*z) * np.exp(1j*k/(2*z)*(FX**2 + FY**2))
+        kern = data * np.exp(1j*k/(2*z)*(XX**2 + YY**2))
+        cgh = np.fft.fft2(np.fft.ifftshift(kern))
+        diff = np.fft.fftshift(cgh * np.fft.ifftshift(pf))
+    else:
+        pf = np.exp(1j*k*z) * np.exp(1j*k/(2*z)*(XX**2 + YY**2))
+        kern = data * np.exp(1j*k/(2*z)*(FX**2 + FY**2))
+        cgh = np.fft.ifft2(np.fft.ifftshift(kern))
+        diff = np.fft.fftshift(cgh)*pf
+
+    return diff, L_out
+
+
+def prop_TF(data, dxy, wavelength, z):
+    '''
+    this method use the transfer function approach to calculate fresnel diffraction
+        data:        source plane field
+        dxy:         source and observation plane pixel size
+        wavelength:  wavelength
+        z:           propagation distance
+        TF:
+            U2(x,y)=ifft(fft(u1)*H); H=exp(jkz)*exp(-j*pi*lambda*z*(fx^2+fy^2))
+
+    '''
+    # the array size
+    M = data.shape[0]
+    N = data.shape[1]
+    # source plane size
+    L_x = dxy * N
+    L_y = dxy * M
+    # wavenumber
+    k = 2 * np.pi / wavelength
+    # frequency resolution
+    dfx = 1/L_x
+    dfy = 1/L_y
+    fy = np.arange(-M/2, M/2) * dfy
+    fx = np.arange(-N/2, N/2) * dfx
+
+    FX, FY = np.meshgrid(fx, fy)
+
+    L_out = [L_y, L_x]
+
+    if z > 0:
+        # transfer function
+        H = np.exp(1j*k*z) * np.exp(-1j*wavelength*z*np.pi*(FX**2 + FY**2))
+        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
+    else:
+        # transfer function
+        H = np.exp(1j*k*z) * np.exp(-1j*wavelength*z*np.pi*(FX**2 + FY**2))
+        diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
+
+    return diff, L_out
+
+
+def prop_IR(data, dxy, wavelength, z):
+    '''
+    this method use the impulse response approach to calculate fresnel diffraction
+        data:        source plane field
+        dxy:         source and observation plane pixel size
+        wavelength:  wavelength
+        z:           propagation distance
+        IR:
+            U2(x,y)=ifft(fft(u1)*H); H=fft(exp(jkz)/(jlambda*z)*exp(j*k/2z*(x^2+y^2)))
+
+    '''
+    # the array size
+    M = data.shape[0]
+    # source plane size
+    L = dxy * M
+    # wavenumber
+    k = 2 * np.pi / wavelength
+    # spatial resolution
+    x = np.arange(-M/2, M/2) * dxy
+    XX, YY = np.meshgrid(x, x)
+
+    L_out = L
+
+    if z > 0:
+        # impule response
+        h = 1/(1j*wavelength*z) * np.exp(1j*k/(2*z)*(XX**2 + YY**2))
+        # transfer function
+        H = np.fft.fft2(np.fft.ifftshift(h)) * dxy**2
+        U1 = np.fft.fft2(np.fft.ifftshift(data))
+        diff = np.fft.fftshift(np.fft.ifft2(U1 * H))
+    else:
+        # impule response
+        h = 1/(-1j*wavelength*z) * np.exp(1j*k/(-2*z)*(XX**2 + YY**2))
+        # transfer function
+        H = np.fft.fft2(np.fft.ifftshift(h)) * dxy**2
+        U1 = np.fft.fft2(np.fft.ifftshift(data))
+        diff = np.fft.fftshift(np.fft.ifft2(U1 / H))
+
+    return diff, L_out
+
+
+# here is the old propagation function for Fresnel diffraction
+def fresnel_propagation(data, dxy, z, wavelength):
+
+    (M, N) = data.shape
+    k = 2 * np.pi / wavelength
+    # the coordinate grid
+    if M % 2 == 0:
+        M_grid = np.arange(-M/2, M/2)
+    else:
+        M_grid = np.arange(-(M-1)/2, (M-1)/2+1)
+    lx = M_grid * dxy
+    XX, YY = np.meshgrid(lx, lx)
+
+    # the coordinate grid on the output plane
+    fc = 1/dxy
+    fu = wavelength * z * fc
+    lu = M_grid * fu / M
+    Fx, Fy = np.meshgrid(lu, lu)
+
+    if z > 0:
+        pf = np.exp(1j*k*z) * np.exp(1j*k*(Fx**2 + Fy**2)/2/z)
+        kern = data * np.exp(1j*k*(XX**2 + YY**2)/2/z)
+        cgh = np.fft.fft2(np.fft.fftshift(kern))
+        OUT = np.fft.fftshift(cgh * np.fft.fftshift(pf))
+    else:
+        pf = np.exp(1j*k*z) * np.exp(1j*k*(XX**2 + YY**2)/2/z)
+        cgh = np.fft.ifft2(np.fft.fftshift(data*np.exp(1j*k*(Fx**2+Fy**2)/2/z)))
+        OUT = np.fft.fftshift(cgh)*pf
+
+    return OUT
+
+
+
+def prop_TF_2d(data, dxy, wavelength, z):
+    '''
+    this method use the transfer function approach to calculate fresnel diffraction
+        data:        source plane field
+        dxy:         source and observation plane pixel size
+        wavelength:  wavelength
+        z:           propagation distance, [zx, zy]
+        TF:
+            U2(x,y)=ifft(fft(u1)*H); H=exp(jkz)*exp(-j*pi*lambda*z*(fx^2+fy^2))
+
+    '''
+    # the array size
+    M = data.shape[0]
+    N = data.shape[1]
+    # source plane size
+    L_x = dxy * N
+    L_y = dxy * M
+    # wavenumber
+    k = 2 * np.pi / wavelength
+    # frequency resolution
+    dfx = 1/L_x
+    dfy = 1/L_y
+    fy = np.arange(-M/2, M/2) * dfy
+    fx = np.arange(-N/2, N/2) * dfx
+
+    FX, FY = np.meshgrid(fx, fy)
+
+    L_out = [L_y, L_x]
+
+    H = np.exp(-1j*wavelength*np.pi*(z[0] * FX**2 + z[1] * FY**2))
+    diff = np.fft.fftshift(np.fft.ifft2(np.fft.fft2(np.fft.ifftshift(data)) * np.fft.ifftshift(H)))
+
+    return diff, L_out
+
```

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func_light.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/func_light.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,646 +1,646 @@
-'''
-This file contains all the small functions needed for the program
-'''
-import numpy as np
-import sys
-import scipy.ndimage as sf
-
-
-def write_h5(result_path, file_name, data_dict):
-    ''' this function is used to save the variables in *args to hdf5 file
-        args are in format: {'name': data}
-    '''
-    import h5py
-    import os
-    if not os.path.exists(result_path):
-        os.makedirs(result_path)
-    with h5py.File(os.path.join(result_path, file_name+'.hdf5'), 'w') as f:
-        for key_name in data_dict:
-            f.create_dataset(key_name, data=data_dict[key_name], compression="gzip", compression_opts=9)
-    prColor('result hdf5 file : {} saved'.format(file_name+'.hdf5'), 'green')
-
-
-def read_h5(file_path, key_name, print_key=False):
-    '''
-        read the data with the key_name in the h5 file
-    '''
-    import h5py
-    import os
-    if not os.path.exists(file_path):
-        prColor('Wrong file path: {}'.format(file_path), 'red')
-        sys.exit()
-
-    with h5py.File(file_path, 'r') as f:
-        # List all groups
-        if print_key:
-            prColor("Keys: {}".format(list(f.keys())), 'green')
-
-        # Get the data
-        if isinstance(key_name, list):
-            data = []
-            for each_key in key_name:
-                data.append(f[each_key][:])
-        elif isinstance(key_name, str):
-            data = f[key_name][:]
-        else:
-            prColor('Wrong h5 key name', 'red')
-    return data
-
-
-def write_json(result_path, file_name, data_dict):
-    import os
-    import json
-    if not os.path.exists(result_path):
-        os.makedirs(result_path)
-    file_name_para = os.path.join(result_path, file_name+'.json')
-    with open(file_name_para, 'w') as fp:
-        json.dump(data_dict, fp, indent=0)
-    
-    prColor('result json file : {} saved'.format(file_name+'.json'), 'green')
-
-
-def read_json(filepath, print_para=False):
-    import os
-    import json
-    if not os.path.exists(filepath):
-        prColor('Wrong file path: {}'.format(filepath), 'red')
-        sys.exit()
-    # file_name_para = os.path.join(result_path, file_name+'.json')
-    with open(filepath, 'r') as fp:
-        data = json.load(fp)
-        if print_para:
-            prColor('parameters: {}'.format(data), 'green')
-    
-    return data
-
-
-def noise_poisson(data, noise_level):
-    '''
-        here's function to add noise to the intensity
-        input:
-            data:               the original image
-            noise_level:        the poisson noise level
-        output:
-            data_new:           the data with poisson noise
-    '''
-    noise = np.random.poisson(noise_level, data.shape)
-    if data.dtype == 'complex128':
-        I = np.abs(data)**2
-        noisy_img = I+noise
-        noisy_img = np.sqrt(noisy_img) * np.exp(1j*np.angle(data))
-    else:
-        noisy_img = data + noise
-    return noisy_img
-
-
-def spherical_wave(M, dx, beam_dia, L_focal, wavelength, amp_type):
-    '''
-    this function can generate spherical wavefront and amplitude
-        M:              the matrix size
-        dx:             pixel size
-        beam_dia:       beam diameter, FWHM (gaussain) or whole size (plane)
-        wavelength:     the wavelength of the light
-        L_focal:        focal length of wavefront, negtive: diverged; positive: focused
-        amp_type:       the amplitude initilization type, Gaussian or circle plane
-    '''
-    x = np.arange(-M/2, M/2) * dx
-    y = np.arange(-M/2, M/2) * dx
-    XX, YY = np.meshgrid(x, y)
-    k = 2 * np.pi / wavelength
-
-    phase = np.exp(-1j * k / (2 * L_focal) * (XX**2 + YY ** 2))
-
-    if amp_type == 'Gaussian':
-        # Gaussian amplitude distribution
-        amp = np.exp(-(XX**2 + YY**2)/(beam_dia ** 2 / 4 / (np.log(2)))) * phase
-    elif amp_type == 'plane':
-        amp = np.ones(phase.shape, dtype=float) * (XX ** 2 + YY ** 2 < (beam_dia/2)**2) * phase
-    else:
-        sys.exit('wrong amplitude initialization type, Gaussian or plane')
-
-    return amp
-
-
-def phase_plate(M, dxy, period, dis_type, phase_value):
-    '''
-    To generate 2D phase distribution
-        M:              array size
-        dxy:            pixel size
-        period:         the size of structure, for random phase plate, it's point size;
-                        for grating, it's structure period
-        dis_type:       random plate or 2D grating
-        phase_value:    the max-min phase value of the distribution
-    '''
-    cluster_size_random = np.int64(round(period/dxy))
-    cluster_size_grating = np.int64(round(period/2/dxy))
-    # size of the initial matrix, then expand the matrix to make it larger than M
-
-    if dis_type == 'random plate':
-        '''
-            use random plate as the initial matrix
-        '''
-        ini_size = int(M//cluster_size_random + 1)
-        ini_array = np.random.rand(ini_size, ini_size)
-        ini_array = np.ones(ini_array.shape) * (ini_array > 0.5)
-        expande_array = np.repeat(np.repeat(ini_array, cluster_size_random, axis=0), cluster_size_random, axis=1)
-
-    elif dis_type == '2D grating':
-        '''
-            use 2D grating as the initial matrix
-        '''
-        ini_size = int(M//cluster_size_grating + 1)
-        ini_array_row = np.tile(np.arange(ini_size) % 2, (ini_size, 1))
-        ini_array_col = np.transpose(ini_array_row)
-        ini_array = ini_array_row * ini_array_col
-        expande_array = np.repeat(np.repeat(ini_array, cluster_size_grating, axis=0), cluster_size_grating, axis=1)
-
-    return np.exp(1j * phase_value * expande_array[0:M, 0:M])
-
-
-def amp_plate(M, dxy, period, dis_type, absorption):
-    '''
-    To generate 2D amplitude distribution
-        M:              array size
-        dxy:            pixel size
-        period:         the size of structure, for random phase plate, it's point size;
-                        for grating, it's structure period
-        dis_type:       random plate or 2D grating
-        phase_value:    the max-min phase value of the distribution
-    '''
-    cluster_size_random = np.int64(round(period/dxy))
-    cluster_size_grating = np.int64(round(period/2/dxy))
-    # size of the initial matrix, then expand the matrix to make it larger than M
-
-    if dis_type == 'random plate':
-        '''
-            use random plate as the initial matrix
-        '''
-        ini_size = int(M//cluster_size_random + 1)
-        ini_array = np.random.rand(ini_size, ini_size)
-        ini_array = np.ones(ini_array.shape) * (ini_array > 0.5)
-        expande_array = np.repeat(np.repeat(ini_array, cluster_size_random, axis=0), cluster_size_random, axis=1)
-
-    elif dis_type == '2D grating':
-        '''
-            use 2D grating as the initial matrix
-        '''
-        ini_size = int(M//cluster_size_grating + 1)
-        ini_array_row = np.tile(np.arange(ini_size) % 2, (ini_size, 1))
-        ini_array_col = np.transpose(ini_array_row)
-        ini_array = ini_array_row * ini_array_col
-        expande_array = np.repeat(np.repeat(ini_array, cluster_size_grating, axis=0), cluster_size_grating, axis=1)
-
-    return 1 - absorption * expande_array[0:M, 0:M]
-
-def image_roi(img, M):
-    '''
-        take out the interested area of the all data.
-        input:
-            img:            image data, 2D or 3D array
-            M:              the interested array size
-                            if M = 0, use the whole size of the data
-        output:
-            img_data:       the area of the data
-    '''
-    img_size = img.shape
-    if M == 0:
-        return img
-    elif len(img_size) == 2:
-        if M > min(img_size):
-            return img
-        else:
-            pos_0 = np.arange(M) - np.round(M/2) + np.round(img_size[0]/2)
-            pos_0 = pos_0.astype('int')
-            pos_1 = np.arange(M) - np.round(M/2) + np.round(img_size[1]/2)
-            pos_1 = pos_1.astype('int')
-            img_data = img[pos_0[0]:pos_0[-1]+1, pos_1[0]:pos_1[-1]+1]
-    elif len(img_size) == 3:
-        if M > min(img_size[1:]):
-            return img
-        else:
-            pos_0 = np.arange(M) - np.round(M/2) + np.round(img_size[1]/2)
-            pos_0 = pos_0.astype('int')
-            pos_1 = np.arange(M) - np.round(M/2) + np.round(img_size[2]/2)
-            pos_1 = pos_1.astype('int')
-            img_data = np.zeros((img_size[0], M, M))
-            for kk, pp in enumerate(img):
-                img_data[kk] = pp[pos_0[0]:pos_0[-1]+1, pos_1[0]:pos_1[-1]+1]
-
-    return img_data
-
-
-def prColor(word, color_type):
-    ''' function to print color text in terminal
-        input:
-            word:           word to print
-            color_type:     which color
-                            'red', 'green', 'yellow'
-                            'light_purple', 'purple'
-                            'cyan', 'light_gray'
-                            'black'
-    '''
-    end_c = '\033[00m'
-    if color_type == 'red':
-        start_c = '\033[91m'
-    elif color_type == 'green':
-        start_c = '\033[92m'
-    elif color_type == 'yellow':
-        start_c = '\033[93m'
-    elif color_type == 'light_purple':
-        start_c = '\033[94m'
-    elif color_type == 'purple':
-        start_c = '\033[95m'
-    elif color_type == 'cyan':
-        start_c = '\033[96m'
-    elif color_type == 'light_gray':
-        start_c = '\033[97m'
-    elif color_type == 'black':
-        start_c = '\033[98m'
-    else:
-        print('color not right')
-        sys.exit()
-
-    print(start_c + str(word) + end_c)
-
-
-def normalize(data, b_min=0, b_max=1):
-    '''
-        this function is used to normalize the data to [0, 1]
-        input:
-            data:           the initial data
-            b_min:          the minimum after normalization
-            b_max:          the maximum after normalization
-    '''
-    return (data - np.amin(data)) / (np.amax(data) - np.amin(data)) * (b_max-b_min) + b_min
-
-'''
-    the 2D integration method here. fourier_integreation1 and 2 and frankotchellappa method
-'''
-def fourier_integration2DShift(dpc_x, del_x,
-                               dpc_y, del_y):
-
-    '''
-    This function is the direct use of the CONTINOUS formulation of
-    Frankot-Chellappa, eq 21 in the article:
-
-    T. Frankot and R. Chellappa
-        A Method for Enforcing Integrability in Shape from Shading Algorithms,
-        IEEE Transactions On Pattern Analysis And Machine Intelligence, Vol 10,
-        No 4, Jul 1988
-
-    In addition, it uses the CONTINOUS shift property to avoid singularities
-    at zero frequencies
-    input:
-        dpc_x:              the differential phase along x
-        del_x:              pixel size along x
-        dpc_y:              the differential phase along y 
-        del_y:              pixel size along y         
-    output:
-        phi:                phase calculated from the dpc
-    '''
-    dpc_x = dpc_x / del_x
-    dpc_y = dpc_y / del_y
-
-    dim = dpc_x.shape
-    x_axis = del_x * (np.arange(dim[1]) - round(dim[1]/2))
-    y_axis = del_y * (np.arange(dim[0]) - round(dim[0]/2))
-
-    xx, yy = np.meshgrid(x_axis, y_axis)
-
-    dk_x = 2*np.pi / (dim[1]*del_x)
-    dk_y = 2*np.pi / (dim[0]*del_y)
-
-    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
-    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
-
-    fy, fx = np.meshgrid(ky/2/np.pi, kx/2/np.pi, indexing='ij')
-
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    # fftshift = lambda x: np.fft.fftshift(x)
-    # ifftshift = lambda x: np.fft.ifftshift(x)
-
-    # fx, fy = np.meshgrid(np.fft.fftfreq(dpc_x.shape[1], delx),
-    #                      np.fft.fftfreq(dpc_x.shape[0], dely))
-
-    # xx, yy = wpu.realcoordmatrix(dpc_x.shape[1], delx,
-    #                              dpc_x.shape[0], dely)
-
-    fo_x = np.abs(fx[0,1]*0.33) # shift fx value
-    fo_y = np.abs(fy[1,0]*0.33) # shift fy value
-
-
-    phaseShift = np.exp(2*np.pi*1j*(fo_x*xx + fo_y*yy))  # exp factor for shift
-
-    mult_factor = 1/(2*np.pi*1j)/(fx - fo_x - 1j*fy + 1j*fo_y )
-
-
-    bigGprime = fft2((dpc_x - 1j*dpc_y)*phaseShift)
-    bigG = bigGprime*mult_factor
-
-    phi = ifft2(bigG) / phaseShift
-
-    phi -= np.min(np.real(phi))  # since the integral have and undefined constant,
-                         # here it is applied an arbritary offset
-
-
-    return phi
-
-
-def gradient_nabla(phi):
-    '''
-        use fourier transfrom to calculate the displacement from the phase
-        here phase is in a unit of [1/(k_wave)/p_x^2*z]
-    '''
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    fftshift = lambda x: np.fft.fftshift(x)
-    # ifftshift = lambda x: np.fft.ifftshift(x)
-    
-    NN, MM = phi.shape
-
-    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
-                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
-    wx = fftshift(wx)
-    wy = fftshift(wy)
-
-
-    displace_x = np.real(ifft2(1j*wx*fft2(phi)))
-    displace_y = np.real(ifft2(1j*wy*fft2(phi)))
-
-    return [displace_x, displace_y]
-
-
-def frankotchellappa(dpc_x,dpc_y):
-    '''
-        Frankt-Chellappa Algrotihm
-        input:
-            dpc_x:              the differential phase along x
-            dpc_y:              the differential phase along y       
-        output:
-            phi:                phase calculated from the dpc
-    '''
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    fftshift = lambda x: np.fft.fftshift(x)
-    # ifftshift = lambda x: np.fft.ifftshift(x)
-    
-    NN, MM = dpc_x.shape
-
-    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
-                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
-    wx = fftshift(wx)
-    wy = fftshift(wy)
-    numerator = -1j*wx*fft2(dpc_x) -1j*wy*fft2(dpc_y)
-    # here use the numpy.fmax method to eliminate the zero point of the division
-    denominator = np.fmax((wx)**2 + (wy)**2, np.finfo(float).eps)
-
-    div = numerator/denominator
-
-
-    phi = np.real(ifft2(div))
-
-    phi -= np.mean(np.real(phi))
-
-    return phi
-
-
-'''
-    here is the data pre-processing, normalization and the de-noise process.s
-'''
-def Denoise_rof(img, theta=1/8, n_iter=100, alpha=0.95):
-    '''
-        here use the Rudin-Osher-Fatemi method to reduce the noise.
-        and then normalize the data
-        input:
-            img:                speckle image data
-            theta:              parameter for the ROF method
-            n_iter:             iteration for the ROF method
-            alpha:              parameter for the ROF method
-        output:
-            img_out:            the processed image data
-    '''
-    dim = img.shape
-    if len(dim) > 2:
-        # if the data is a combination of multiple data, use loop to process
-        n_data = dim[0]
-        multi_flag = True
-    else:
-        n_data = 1
-        multi_flag = False
-    img_out = np.zeros(dim)
-    # do the process of the data
-    if not multi_flag:
-        # normalize the data to [-1, 1]
-        temp = normalize(img, -1, 1)
-        temp_denoise = fista_l1_denoiseing(temp, theta, n_iter)
-        img_out = normalize(temp - alpha * temp_denoise, 0, 255)
-
-    elif multi_flag:
-        # for multiple images
-        for kk in range(n_data):
-            # normalize the data to [-1, 1]
-            temp = normalize(img[kk], -1, 1)
-            temp_denoise = fista_l1_denoiseing(temp, theta, n_iter)
-            img_out[kk] = normalize(temp - alpha * temp_denoise, 0, 255)
-    return img_out
-
-
-def fista_l1_denoiseing(data, theta, n_iter):
-    '''
-        Rudin-Osher-Fatemi method, L1 denoising
-        input:
-            data:           initial data, 2D array
-            theta:          parameter
-            n_iter:         iteration number
-        output:
-            data_new:       data after denoising
-    '''
-    bc = 'reflect'
-    # axis=1 direction deviation
-    nabla_x_kern = np.array([[0, 0, 0], [1, -1, 0], [0, 0, 0]])
-    # axis=0 direction deviation
-    nabla_y_kern = np.array([[0, 1, 0], [0, -1, 0], [0, 0, 0]])
-    
-    # calculate the gradient along x, and y axis
-    nabla = lambda x: np.array([sf.correlate(x, nabla_x_kern, mode=bc), sf.correlate(x, nabla_y_kern, mode=bc)])
-    # calculate the nabla transpose
-    nablaT = lambda x: sf.correlate(x[0], np.flip(nabla_x_kern), mode=bc) + sf.correlate(x[1], np.flip(nabla_y_kern), mode=bc)
-
-    # define proximal operator of ||x||_{\infty} <= 1
-    prox_linf = lambda x: np.fmin(np.fmax(x, -1), 1)
-    # the objective
-    obj = lambda x: np.sum(np.abs(nablaT(x) - data/theta)**2)
-    # the step size
-    tau = 1/4
-    # start
-    ini_data = np.zeros((2, data.shape[0], data.shape[1]))
-    # gradient descent
-    for kk in range(n_iter):
-        # tt = obj(ini_data)
-        # print('k={}, obj={:.2f}'.format(kk, tt))
-        ini_data = prox_linf(ini_data - tau * nabla(nablaT(ini_data) - data/theta))
-    print('data preprocess ends. obj={:.2f}'.format(obj(ini_data)))
-    data_new = data - nablaT(ini_data) * theta
-    return data_new
-
-
-def grad_fourier(img, dxy=1, z=1, wavelength=2*np.pi):
-    '''
-        here use the fourier method to calculate the gradient along x and y
-        here's the method: nabla(x) = ifft2(1j(kx, ky)fft2(x))
-        if dxy, z, wavelength is not defined, it's the no unit gradient
-        input:
-            img:           the input intensity
-            dxy:            pixel size
-        output:
-            D_y:            gradient along y or displacement
-            D_x:            gradient along x or displacement
-            
-    '''
-    dim = img.shape
-    k_wave = 2 * np.pi / wavelength
-    dk_x = 2*np.pi / (dim[1]*dxy)
-    dk_y = 2*np.pi / (dim[0]*dxy)
-
-    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
-    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
-
-    k_YY, k_XX = np.meshgrid(ky, kx, indexing='ij')
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    '''
-        to calculate the diff_T:
-            diff_T = 1j * F^(-1){(kx, ky) * F{}}
-    '''
-    
-    nabla_T = lambda x: 1j * np.array([ifft2(k_YY * fft2(x)), ifft2(k_XX * fft2(x))])
-   
-    [D_y, D_x] = np.real(nabla_T(img * z / k_wave))
-    return D_y, D_x
-
-
-def grad_conv(img, method=2):
-    '''
-        use convolution to calculate the gradient
-        method:             2 for O(h^4) and 1 for O(h2)
-    '''
-    if method == 2:
-        h = np.array([[0, 0, 0, 0, 0], [1, -8, 0, 8, -1], [0, 0, 0, 0, 0]])/12
-    elif method == 1:
-        h = np.array([[0, 0, 0], [-1, 0, 1], [0, 0, 0]])/2
-    else:
-        print('no defined method, should be 1 or 2 for grad_conv')
-    
-    wx = sf.correlate(img, h, mode='reflect')
-    wy = sf.correlate(img, h.transpose(), mode='reflect')
-
-    return wy, wx
-
-
-def subpixel_shift(img, Sprow, Spcol):
-    ''' input array: numpy.ndarray
-        output array: numpy.ndarray
-    '''
-    if len(img.shape) > 2:
-        print('subpixel_shift function cannot deal with 3D matrix')
-        return
-    N_row = img.shape[0]
-    N_col = img.shape[1]
-    if N_row % 2 != 0 or N_col % 2 != 0:
-        print('The size of data is better to be 2^N for higher accuracy!')
-
-    dk_row = 1/N_row
-    dk_col = 1/N_col
-
-    k_row = dk_row * np.fft.ifftshift(np.arange(-N_row/2, N_row/2) if N_row % 2 == 0 else np.arange(-(N_row-1)/2, (N_row+1)/2))
-    k_col = dk_col * np.fft.ifftshift(np.arange(-N_col/2, N_col/2) if N_col % 2 == 0 else np.arange(-(N_col-1)/2, (N_col+1)/2))
-
-    KK_row, KK_col = np.meshgrid(k_row, k_col)
-
-    Fr = np.fft.fft2(np.fft.ifftshift(img))
-
-    Fr = Fr * np.exp(-2j * np.pi * Spcol * KK_col) * np.exp(-2j * np.pi * Sprow * KK_row)
-    output = np.fft.fftshift(np.fft.ifft2(Fr))
-
-    return np.real(output)
-
-
-def image_shift(img, Spy, Spx):
-    '''
-        here's the function to shift the images x and y pixels
-        the pixel number can be sub-pixels
-        input:
-            img:            original data
-            spy:            shift pixels along y axis
-                            spy>0: down, spy<0: up
-            spx:            shift pixels along x axis
-                            spx>0: right, spx<0: left
-    '''
-    # integer part of the position shifting
-    n_spy = np.round(Spy)
-    n_spx = np.round(Spx)
-    x_axis = (np.arange(img.shape[1]) + n_spx) % img.shape[1]
-    x_axis = x_axis.astype('int')
-    y_axis = (np.arange(img.shape[0]) + n_spy) % img.shape[0]
-    y_axis = y_axis.astype('int')
-
-    img_int = img[y_axis][x_axis] + 0
-
-    s_y = Spy - n_spy
-    s_x = Spx - n_spx
-
-    img_new = subpixel_shift(img_int, s_y, s_x)
-
-    return img_new
-
-
-def image_align(image, offset_image):
-    '''
-        here's a function to do the alignment of two images.
-        the offset_image is shifted relatively to image to find the best position
-        and return the shifted back offset_image
-        input:
-            image:              the first image
-            offset_image:       the second image
-        output:
-            pos:                best shift postion to maximize the correlation
-            image_back:         the image after alignment
-    '''
-    from skimage.feature import register_translation
-    from skimage.feature.register_translation import _upsampled_dft
-    # from skimage.registration import phase_cross_correlation
-    from scipy.ndimage import fourier_shift
-    # roi = lambda x: x[0:100][0:100]
-    shift, error, diffphase = register_translation(image, offset_image, 100)
-    # shift, error, diffphase = phase_cross_correlation(image, offset_image, 100)
-    # shift, error, diffphase = register_translation(roi(image), roi(offset_image), 100)
-
-    print('shift dist: {}, alignment error: {} and phase difference: {}'.format(shift, error, diffphase))
-    # image_back = image_shift(offset_image, shift[0], shift[1])
-    image_back = fourier_shift(np.fft.fftn(offset_image), shift)
-    image_back = np.real(np.fft.ifftn(image_back))
-    return shift, image_back
-
-
-def image_preprocess(image, have_dark, dark_img, have_flat, flat_img):
-    '''
-        do the flat or dark correction for the images
-        img:            image to be corrected
-        have_dark:      if there is dark
-        dark_img:           dark image
-        have_flat:      if there is flat
-        flat_img:           flat image        
-    '''
-    if (have_flat != 0 and have_dark != 0):
-        numerator = (flat_img - dark_img).clip(0.00000001)
-        # numerator = numerator / np.amax(numerator)
-        image = ((image - dark_img) / numerator ) * np.amax(image)
-    elif (have_dark != 0):
-        image = (image - dark_img).clip(0.00000001)
-    elif (have_flat != 0):
-        flat_img[flat_img == 0] = 0.00000001
-        # flat_img = flat_img / np.amax(flat_img)
-        image = (image / flat_img)  * np.amax(image)
-                
-    return image
+'''
+This file contains all the small functions needed for the program
+'''
+import numpy as np
+import sys
+import scipy.ndimage as sf
+
+
+def write_h5(result_path, file_name, data_dict):
+    ''' this function is used to save the variables in *args to hdf5 file
+        args are in format: {'name': data}
+    '''
+    import h5py
+    import os
+    if not os.path.exists(result_path):
+        os.makedirs(result_path)
+    with h5py.File(os.path.join(result_path, file_name+'.hdf5'), 'w') as f:
+        for key_name in data_dict:
+            f.create_dataset(key_name, data=data_dict[key_name], compression="gzip", compression_opts=9)
+    prColor('result hdf5 file : {} saved'.format(file_name+'.hdf5'), 'green')
+
+
+def read_h5(file_path, key_name, print_key=False):
+    '''
+        read the data with the key_name in the h5 file
+    '''
+    import h5py
+    import os
+    if not os.path.exists(file_path):
+        prColor('Wrong file path: {}'.format(file_path), 'red')
+        sys.exit()
+
+    with h5py.File(file_path, 'r') as f:
+        # List all groups
+        if print_key:
+            prColor("Keys: {}".format(list(f.keys())), 'green')
+
+        # Get the data
+        if isinstance(key_name, list):
+            data = []
+            for each_key in key_name:
+                data.append(f[each_key][:])
+        elif isinstance(key_name, str):
+            data = f[key_name][:]
+        else:
+            prColor('Wrong h5 key name', 'red')
+    return data
+
+
+def write_json(result_path, file_name, data_dict):
+    import os
+    import json
+    if not os.path.exists(result_path):
+        os.makedirs(result_path)
+    file_name_para = os.path.join(result_path, file_name+'.json')
+    with open(file_name_para, 'w') as fp:
+        json.dump(data_dict, fp, indent=0)
+    
+    prColor('result json file : {} saved'.format(file_name+'.json'), 'green')
+
+
+def read_json(filepath, print_para=False):
+    import os
+    import json
+    if not os.path.exists(filepath):
+        prColor('Wrong file path: {}'.format(filepath), 'red')
+        sys.exit()
+    # file_name_para = os.path.join(result_path, file_name+'.json')
+    with open(filepath, 'r') as fp:
+        data = json.load(fp)
+        if print_para:
+            prColor('parameters: {}'.format(data), 'green')
+    
+    return data
+
+
+def noise_poisson(data, noise_level):
+    '''
+        here's function to add noise to the intensity
+        input:
+            data:               the original image
+            noise_level:        the poisson noise level
+        output:
+            data_new:           the data with poisson noise
+    '''
+    noise = np.random.poisson(noise_level, data.shape)
+    if data.dtype == 'complex128':
+        I = np.abs(data)**2
+        noisy_img = I+noise
+        noisy_img = np.sqrt(noisy_img) * np.exp(1j*np.angle(data))
+    else:
+        noisy_img = data + noise
+    return noisy_img
+
+
+def spherical_wave(M, dx, beam_dia, L_focal, wavelength, amp_type):
+    '''
+    this function can generate spherical wavefront and amplitude
+        M:              the matrix size
+        dx:             pixel size
+        beam_dia:       beam diameter, FWHM (gaussain) or whole size (plane)
+        wavelength:     the wavelength of the light
+        L_focal:        focal length of wavefront, negtive: diverged; positive: focused
+        amp_type:       the amplitude initilization type, Gaussian or circle plane
+    '''
+    x = np.arange(-M/2, M/2) * dx
+    y = np.arange(-M/2, M/2) * dx
+    XX, YY = np.meshgrid(x, y)
+    k = 2 * np.pi / wavelength
+
+    phase = np.exp(-1j * k / (2 * L_focal) * (XX**2 + YY ** 2))
+
+    if amp_type == 'Gaussian':
+        # Gaussian amplitude distribution
+        amp = np.exp(-(XX**2 + YY**2)/(beam_dia ** 2 / 4 / (np.log(2)))) * phase
+    elif amp_type == 'plane':
+        amp = np.ones(phase.shape, dtype=float) * (XX ** 2 + YY ** 2 < (beam_dia/2)**2) * phase
+    else:
+        sys.exit('wrong amplitude initialization type, Gaussian or plane')
+
+    return amp
+
+
+def phase_plate(M, dxy, period, dis_type, phase_value):
+    '''
+    To generate 2D phase distribution
+        M:              array size
+        dxy:            pixel size
+        period:         the size of structure, for random phase plate, it's point size;
+                        for grating, it's structure period
+        dis_type:       random plate or 2D grating
+        phase_value:    the max-min phase value of the distribution
+    '''
+    cluster_size_random = np.int64(round(period/dxy))
+    cluster_size_grating = np.int64(round(period/2/dxy))
+    # size of the initial matrix, then expand the matrix to make it larger than M
+
+    if dis_type == 'random plate':
+        '''
+            use random plate as the initial matrix
+        '''
+        ini_size = int(M//cluster_size_random + 1)
+        ini_array = np.random.rand(ini_size, ini_size)
+        ini_array = np.ones(ini_array.shape) * (ini_array > 0.5)
+        expande_array = np.repeat(np.repeat(ini_array, cluster_size_random, axis=0), cluster_size_random, axis=1)
+
+    elif dis_type == '2D grating':
+        '''
+            use 2D grating as the initial matrix
+        '''
+        ini_size = int(M//cluster_size_grating + 1)
+        ini_array_row = np.tile(np.arange(ini_size) % 2, (ini_size, 1))
+        ini_array_col = np.transpose(ini_array_row)
+        ini_array = ini_array_row * ini_array_col
+        expande_array = np.repeat(np.repeat(ini_array, cluster_size_grating, axis=0), cluster_size_grating, axis=1)
+
+    return np.exp(1j * phase_value * expande_array[0:M, 0:M])
+
+
+def amp_plate(M, dxy, period, dis_type, absorption):
+    '''
+    To generate 2D amplitude distribution
+        M:              array size
+        dxy:            pixel size
+        period:         the size of structure, for random phase plate, it's point size;
+                        for grating, it's structure period
+        dis_type:       random plate or 2D grating
+        phase_value:    the max-min phase value of the distribution
+    '''
+    cluster_size_random = np.int64(round(period/dxy))
+    cluster_size_grating = np.int64(round(period/2/dxy))
+    # size of the initial matrix, then expand the matrix to make it larger than M
+
+    if dis_type == 'random plate':
+        '''
+            use random plate as the initial matrix
+        '''
+        ini_size = int(M//cluster_size_random + 1)
+        ini_array = np.random.rand(ini_size, ini_size)
+        ini_array = np.ones(ini_array.shape) * (ini_array > 0.5)
+        expande_array = np.repeat(np.repeat(ini_array, cluster_size_random, axis=0), cluster_size_random, axis=1)
+
+    elif dis_type == '2D grating':
+        '''
+            use 2D grating as the initial matrix
+        '''
+        ini_size = int(M//cluster_size_grating + 1)
+        ini_array_row = np.tile(np.arange(ini_size) % 2, (ini_size, 1))
+        ini_array_col = np.transpose(ini_array_row)
+        ini_array = ini_array_row * ini_array_col
+        expande_array = np.repeat(np.repeat(ini_array, cluster_size_grating, axis=0), cluster_size_grating, axis=1)
+
+    return 1 - absorption * expande_array[0:M, 0:M]
+
+def image_roi(img, M):
+    '''
+        take out the interested area of the all data.
+        input:
+            img:            image data, 2D or 3D array
+            M:              the interested array size
+                            if M = 0, use the whole size of the data
+        output:
+            img_data:       the area of the data
+    '''
+    img_size = img.shape
+    if M == 0:
+        return img
+    elif len(img_size) == 2:
+        if M > min(img_size):
+            return img
+        else:
+            pos_0 = np.arange(M) - np.round(M/2) + np.round(img_size[0]/2)
+            pos_0 = pos_0.astype('int')
+            pos_1 = np.arange(M) - np.round(M/2) + np.round(img_size[1]/2)
+            pos_1 = pos_1.astype('int')
+            img_data = img[pos_0[0]:pos_0[-1]+1, pos_1[0]:pos_1[-1]+1]
+    elif len(img_size) == 3:
+        if M > min(img_size[1:]):
+            return img
+        else:
+            pos_0 = np.arange(M) - np.round(M/2) + np.round(img_size[1]/2)
+            pos_0 = pos_0.astype('int')
+            pos_1 = np.arange(M) - np.round(M/2) + np.round(img_size[2]/2)
+            pos_1 = pos_1.astype('int')
+            img_data = np.zeros((img_size[0], M, M))
+            for kk, pp in enumerate(img):
+                img_data[kk] = pp[pos_0[0]:pos_0[-1]+1, pos_1[0]:pos_1[-1]+1]
+
+    return img_data
+
+
+def prColor(word, color_type):
+    ''' function to print color text in terminal
+        input:
+            word:           word to print
+            color_type:     which color
+                            'red', 'green', 'yellow'
+                            'light_purple', 'purple'
+                            'cyan', 'light_gray'
+                            'black'
+    '''
+    end_c = '\033[00m'
+    if color_type == 'red':
+        start_c = '\033[91m'
+    elif color_type == 'green':
+        start_c = '\033[92m'
+    elif color_type == 'yellow':
+        start_c = '\033[93m'
+    elif color_type == 'light_purple':
+        start_c = '\033[94m'
+    elif color_type == 'purple':
+        start_c = '\033[95m'
+    elif color_type == 'cyan':
+        start_c = '\033[96m'
+    elif color_type == 'light_gray':
+        start_c = '\033[97m'
+    elif color_type == 'black':
+        start_c = '\033[98m'
+    else:
+        print('color not right')
+        sys.exit()
+
+    print(start_c + str(word) + end_c)
+
+
+def normalize(data, b_min=0, b_max=1):
+    '''
+        this function is used to normalize the data to [0, 1]
+        input:
+            data:           the initial data
+            b_min:          the minimum after normalization
+            b_max:          the maximum after normalization
+    '''
+    return (data - np.amin(data)) / (np.amax(data) - np.amin(data)) * (b_max-b_min) + b_min
+
+'''
+    the 2D integration method here. fourier_integreation1 and 2 and frankotchellappa method
+'''
+def fourier_integration2DShift(dpc_x, del_x,
+                               dpc_y, del_y):
+
+    '''
+    This function is the direct use of the CONTINOUS formulation of
+    Frankot-Chellappa, eq 21 in the article:
+
+    T. Frankot and R. Chellappa
+        A Method for Enforcing Integrability in Shape from Shading Algorithms,
+        IEEE Transactions On Pattern Analysis And Machine Intelligence, Vol 10,
+        No 4, Jul 1988
+
+    In addition, it uses the CONTINOUS shift property to avoid singularities
+    at zero frequencies
+    input:
+        dpc_x:              the differential phase along x
+        del_x:              pixel size along x
+        dpc_y:              the differential phase along y 
+        del_y:              pixel size along y         
+    output:
+        phi:                phase calculated from the dpc
+    '''
+    dpc_x = dpc_x / del_x
+    dpc_y = dpc_y / del_y
+
+    dim = dpc_x.shape
+    x_axis = del_x * (np.arange(dim[1]) - round(dim[1]/2))
+    y_axis = del_y * (np.arange(dim[0]) - round(dim[0]/2))
+
+    xx, yy = np.meshgrid(x_axis, y_axis)
+
+    dk_x = 2*np.pi / (dim[1]*del_x)
+    dk_y = 2*np.pi / (dim[0]*del_y)
+
+    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
+    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
+
+    fy, fx = np.meshgrid(ky/2/np.pi, kx/2/np.pi, indexing='ij')
+
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    # fftshift = lambda x: np.fft.fftshift(x)
+    # ifftshift = lambda x: np.fft.ifftshift(x)
+
+    # fx, fy = np.meshgrid(np.fft.fftfreq(dpc_x.shape[1], delx),
+    #                      np.fft.fftfreq(dpc_x.shape[0], dely))
+
+    # xx, yy = wpu.realcoordmatrix(dpc_x.shape[1], delx,
+    #                              dpc_x.shape[0], dely)
+
+    fo_x = np.abs(fx[0,1]*0.33) # shift fx value
+    fo_y = np.abs(fy[1,0]*0.33) # shift fy value
+
+
+    phaseShift = np.exp(2*np.pi*1j*(fo_x*xx + fo_y*yy))  # exp factor for shift
+
+    mult_factor = 1/(2*np.pi*1j)/(fx - fo_x - 1j*fy + 1j*fo_y )
+
+
+    bigGprime = fft2((dpc_x - 1j*dpc_y)*phaseShift)
+    bigG = bigGprime*mult_factor
+
+    phi = ifft2(bigG) / phaseShift
+
+    phi -= np.min(np.real(phi))  # since the integral have and undefined constant,
+                         # here it is applied an arbritary offset
+
+
+    return phi
+
+
+def gradient_nabla(phi):
+    '''
+        use fourier transfrom to calculate the displacement from the phase
+        here phase is in a unit of [1/(k_wave)/p_x^2*z]
+    '''
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    fftshift = lambda x: np.fft.fftshift(x)
+    # ifftshift = lambda x: np.fft.ifftshift(x)
+    
+    NN, MM = phi.shape
+
+    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
+                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
+    wx = fftshift(wx)
+    wy = fftshift(wy)
+
+
+    displace_x = np.real(ifft2(1j*wx*fft2(phi)))
+    displace_y = np.real(ifft2(1j*wy*fft2(phi)))
+
+    return [displace_x, displace_y]
+
+
+def frankotchellappa(dpc_x,dpc_y):
+    '''
+        Frankt-Chellappa Algrotihm
+        input:
+            dpc_x:              the differential phase along x
+            dpc_y:              the differential phase along y       
+        output:
+            phi:                phase calculated from the dpc
+    '''
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    fftshift = lambda x: np.fft.fftshift(x)
+    # ifftshift = lambda x: np.fft.ifftshift(x)
+    
+    NN, MM = dpc_x.shape
+
+    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
+                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
+    wx = fftshift(wx)
+    wy = fftshift(wy)
+    numerator = -1j*wx*fft2(dpc_x) -1j*wy*fft2(dpc_y)
+    # here use the numpy.fmax method to eliminate the zero point of the division
+    denominator = np.fmax((wx)**2 + (wy)**2, np.finfo(float).eps)
+
+    div = numerator/denominator
+
+
+    phi = np.real(ifft2(div))
+
+    phi -= np.mean(np.real(phi))
+
+    return phi
+
+
+'''
+    here is the data pre-processing, normalization and the de-noise process.s
+'''
+def Denoise_rof(img, theta=1/8, n_iter=100, alpha=0.95):
+    '''
+        here use the Rudin-Osher-Fatemi method to reduce the noise.
+        and then normalize the data
+        input:
+            img:                speckle image data
+            theta:              parameter for the ROF method
+            n_iter:             iteration for the ROF method
+            alpha:              parameter for the ROF method
+        output:
+            img_out:            the processed image data
+    '''
+    dim = img.shape
+    if len(dim) > 2:
+        # if the data is a combination of multiple data, use loop to process
+        n_data = dim[0]
+        multi_flag = True
+    else:
+        n_data = 1
+        multi_flag = False
+    img_out = np.zeros(dim)
+    # do the process of the data
+    if not multi_flag:
+        # normalize the data to [-1, 1]
+        temp = normalize(img, -1, 1)
+        temp_denoise = fista_l1_denoiseing(temp, theta, n_iter)
+        img_out = normalize(temp - alpha * temp_denoise, 0, 255)
+
+    elif multi_flag:
+        # for multiple images
+        for kk in range(n_data):
+            # normalize the data to [-1, 1]
+            temp = normalize(img[kk], -1, 1)
+            temp_denoise = fista_l1_denoiseing(temp, theta, n_iter)
+            img_out[kk] = normalize(temp - alpha * temp_denoise, 0, 255)
+    return img_out
+
+
+def fista_l1_denoiseing(data, theta, n_iter):
+    '''
+        Rudin-Osher-Fatemi method, L1 denoising
+        input:
+            data:           initial data, 2D array
+            theta:          parameter
+            n_iter:         iteration number
+        output:
+            data_new:       data after denoising
+    '''
+    bc = 'reflect'
+    # axis=1 direction deviation
+    nabla_x_kern = np.array([[0, 0, 0], [1, -1, 0], [0, 0, 0]])
+    # axis=0 direction deviation
+    nabla_y_kern = np.array([[0, 1, 0], [0, -1, 0], [0, 0, 0]])
+    
+    # calculate the gradient along x, and y axis
+    nabla = lambda x: np.array([sf.correlate(x, nabla_x_kern, mode=bc), sf.correlate(x, nabla_y_kern, mode=bc)])
+    # calculate the nabla transpose
+    nablaT = lambda x: sf.correlate(x[0], np.flip(nabla_x_kern), mode=bc) + sf.correlate(x[1], np.flip(nabla_y_kern), mode=bc)
+
+    # define proximal operator of ||x||_{\infty} <= 1
+    prox_linf = lambda x: np.fmin(np.fmax(x, -1), 1)
+    # the objective
+    obj = lambda x: np.sum(np.abs(nablaT(x) - data/theta)**2)
+    # the step size
+    tau = 1/4
+    # start
+    ini_data = np.zeros((2, data.shape[0], data.shape[1]))
+    # gradient descent
+    for kk in range(n_iter):
+        # tt = obj(ini_data)
+        # print('k={}, obj={:.2f}'.format(kk, tt))
+        ini_data = prox_linf(ini_data - tau * nabla(nablaT(ini_data) - data/theta))
+    print('data preprocess ends. obj={:.2f}'.format(obj(ini_data)))
+    data_new = data - nablaT(ini_data) * theta
+    return data_new
+
+
+def grad_fourier(img, dxy=1, z=1, wavelength=2*np.pi):
+    '''
+        here use the fourier method to calculate the gradient along x and y
+        here's the method: nabla(x) = ifft2(1j(kx, ky)fft2(x))
+        if dxy, z, wavelength is not defined, it's the no unit gradient
+        input:
+            img:           the input intensity
+            dxy:            pixel size
+        output:
+            D_y:            gradient along y or displacement
+            D_x:            gradient along x or displacement
+            
+    '''
+    dim = img.shape
+    k_wave = 2 * np.pi / wavelength
+    dk_x = 2*np.pi / (dim[1]*dxy)
+    dk_y = 2*np.pi / (dim[0]*dxy)
+
+    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
+    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
+
+    k_YY, k_XX = np.meshgrid(ky, kx, indexing='ij')
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    '''
+        to calculate the diff_T:
+            diff_T = 1j * F^(-1){(kx, ky) * F{}}
+    '''
+    
+    nabla_T = lambda x: 1j * np.array([ifft2(k_YY * fft2(x)), ifft2(k_XX * fft2(x))])
+   
+    [D_y, D_x] = np.real(nabla_T(img * z / k_wave))
+    return D_y, D_x
+
+
+def grad_conv(img, method=2):
+    '''
+        use convolution to calculate the gradient
+        method:             2 for O(h^4) and 1 for O(h2)
+    '''
+    if method == 2:
+        h = np.array([[0, 0, 0, 0, 0], [1, -8, 0, 8, -1], [0, 0, 0, 0, 0]])/12
+    elif method == 1:
+        h = np.array([[0, 0, 0], [-1, 0, 1], [0, 0, 0]])/2
+    else:
+        print('no defined method, should be 1 or 2 for grad_conv')
+    
+    wx = sf.correlate(img, h, mode='reflect')
+    wy = sf.correlate(img, h.transpose(), mode='reflect')
+
+    return wy, wx
+
+
+def subpixel_shift(img, Sprow, Spcol):
+    ''' input array: numpy.ndarray
+        output array: numpy.ndarray
+    '''
+    if len(img.shape) > 2:
+        print('subpixel_shift function cannot deal with 3D matrix')
+        return
+    N_row = img.shape[0]
+    N_col = img.shape[1]
+    if N_row % 2 != 0 or N_col % 2 != 0:
+        print('The size of data is better to be 2^N for higher accuracy!')
+
+    dk_row = 1/N_row
+    dk_col = 1/N_col
+
+    k_row = dk_row * np.fft.ifftshift(np.arange(-N_row/2, N_row/2) if N_row % 2 == 0 else np.arange(-(N_row-1)/2, (N_row+1)/2))
+    k_col = dk_col * np.fft.ifftshift(np.arange(-N_col/2, N_col/2) if N_col % 2 == 0 else np.arange(-(N_col-1)/2, (N_col+1)/2))
+
+    KK_row, KK_col = np.meshgrid(k_row, k_col)
+
+    Fr = np.fft.fft2(np.fft.ifftshift(img))
+
+    Fr = Fr * np.exp(-2j * np.pi * Spcol * KK_col) * np.exp(-2j * np.pi * Sprow * KK_row)
+    output = np.fft.fftshift(np.fft.ifft2(Fr))
+
+    return np.real(output)
+
+
+def image_shift(img, Spy, Spx):
+    '''
+        here's the function to shift the images x and y pixels
+        the pixel number can be sub-pixels
+        input:
+            img:            original data
+            spy:            shift pixels along y axis
+                            spy>0: down, spy<0: up
+            spx:            shift pixels along x axis
+                            spx>0: right, spx<0: left
+    '''
+    # integer part of the position shifting
+    n_spy = np.round(Spy)
+    n_spx = np.round(Spx)
+    x_axis = (np.arange(img.shape[1]) + n_spx) % img.shape[1]
+    x_axis = x_axis.astype('int')
+    y_axis = (np.arange(img.shape[0]) + n_spy) % img.shape[0]
+    y_axis = y_axis.astype('int')
+
+    img_int = img[y_axis][x_axis] + 0
+
+    s_y = Spy - n_spy
+    s_x = Spx - n_spx
+
+    img_new = subpixel_shift(img_int, s_y, s_x)
+
+    return img_new
+
+
+def image_align(image, offset_image):
+    '''
+        here's a function to do the alignment of two images.
+        the offset_image is shifted relatively to image to find the best position
+        and return the shifted back offset_image
+        input:
+            image:              the first image
+            offset_image:       the second image
+        output:
+            pos:                best shift postion to maximize the correlation
+            image_back:         the image after alignment
+    '''
+    from skimage.feature import register_translation
+    from skimage.feature.register_translation import _upsampled_dft
+    # from skimage.registration import phase_cross_correlation
+    from scipy.ndimage import fourier_shift
+    # roi = lambda x: x[0:100][0:100]
+    shift, error, diffphase = register_translation(image, offset_image, 100)
+    # shift, error, diffphase = phase_cross_correlation(image, offset_image, 100)
+    # shift, error, diffphase = register_translation(roi(image), roi(offset_image), 100)
+
+    print('shift dist: {}, alignment error: {} and phase difference: {}'.format(shift, error, diffphase))
+    # image_back = image_shift(offset_image, shift[0], shift[1])
+    image_back = fourier_shift(np.fft.fftn(offset_image), shift)
+    image_back = np.real(np.fft.ifftn(image_back))
+    return shift, image_back
+
+
+def image_preprocess(image, have_dark, dark_img, have_flat, flat_img):
+    '''
+        do the flat or dark correction for the images
+        img:            image to be corrected
+        have_dark:      if there is dark
+        dark_img:           dark image
+        have_flat:      if there is flat
+        flat_img:           flat image        
+    '''
+    if (have_flat != 0 and have_dark != 0):
+        numerator = (flat_img - dark_img).clip(0.00000001)
+        # numerator = numerator / np.amax(numerator)
+        image = ((image - dark_img) / numerator ) * np.amax(image)
+    elif (have_dark != 0):
+        image = (image - dark_img).clip(0.00000001)
+    elif (have_flat != 0):
+        flat_img[flat_img == 0] = 0.00000001
+        # flat_img = flat_img / np.amax(flat_img)
+        image = (image / flat_img)  * np.amax(image)
+                
+    return image
```

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/gui_func.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/gui_func.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import matplotlib.pyplot as plt
-from matplotlib.widgets import RectangleSelector
-import numpy as np
-import tkinter as tk
-import os
-from tkinter import filedialog
-
-class crop_img:
-    def __init__(self, data) -> None:
-        self.data = data
-        self.fig = plt.figure()
-        self.ax1 = self.fig.add_subplot(121)
-        self.ax1.imshow(data)
-        self.ax2 = self.fig.add_subplot(122)
-        self.ax2.imshow(np.zeros_like(data))
-        plt.subplots_adjust()
-
-    def line_select_callback(self, eclick, erelease):
-        """
-        Callback for line selection.
-
-        *eclick* and *erelease* are the press and release events.
-        """
-        x1, y1 = eclick.xdata, eclick.ydata
-        x2, y2 = erelease.xdata, erelease.ydata
-        print(f"({x1:3.2f}, {y1:3.2f}) --> ({x2:3.2f}, {y2:3.2f})")
-        print(f" The buttons you used were: {eclick.button} {erelease.button}")
-
-        self.croped = self.data[int(y1):int(y2), int(x1):int(x2)]
-        self.ax2.imshow(self.croped)
-        self.fig.canvas.draw_idle()
-
-        self.corner1 = [y1, x1]
-        self.corner2 = [y2, x2]
-    
-    def crop(self):
-        rect_crop = RectangleSelector(self.ax1, self.line_select_callback,
-                                        drawtype='box', useblit=True,
-                                        button=[1, 3],  # disable middle button
-                                        minspanx=5, minspany=5,
-                                        spancoords='pixels',
-                                        interactive=True)
-
-        plt.show()
-
-
-
-
-def crop_gui(data):
-
-    data_crop = crop_img(data)
-    
-    data_crop.crop()
-    cropped_img = data_crop.croped
-    corner1 = data_crop.corner1
-    corner2 = data_crop.corner2
-
-    return cropped_img, [corner1, corner2]
-    # plt.figure()
-    # plt.imshow(cropped_img)
-    # plt.colorbar()
-    # plt.show()
-
-def gui_load_data(directory='', title="File name with Data"):
-
-    originalDir = os.getcwd()
-
-    root = tk.Tk(title)
-    # root.withdraw()
-    
-    fname1 = filedialog.askopenfilenames()
-
-    if len(fname1) == 0:
-        fname_last = None
-
-    else:
-        fname_last = fname1
-
-    os.chdir(originalDir)
-    root.destroy()
-    # root.mainloop()
+import matplotlib.pyplot as plt
+from matplotlib.widgets import RectangleSelector
+import numpy as np
+import tkinter as tk
+import os
+from tkinter import filedialog
+
+class crop_img:
+    def __init__(self, data) -> None:
+        self.data = data
+        self.fig = plt.figure()
+        self.ax1 = self.fig.add_subplot(121)
+        self.ax1.imshow(data)
+        self.ax2 = self.fig.add_subplot(122)
+        self.ax2.imshow(np.zeros_like(data))
+        plt.subplots_adjust()
+
+    def line_select_callback(self, eclick, erelease):
+        """
+        Callback for line selection.
+
+        *eclick* and *erelease* are the press and release events.
+        """
+        x1, y1 = eclick.xdata, eclick.ydata
+        x2, y2 = erelease.xdata, erelease.ydata
+        print(f"({x1:3.2f}, {y1:3.2f}) --> ({x2:3.2f}, {y2:3.2f})")
+        print(f" The buttons you used were: {eclick.button} {erelease.button}")
+
+        self.croped = self.data[int(y1):int(y2), int(x1):int(x2)]
+        self.ax2.imshow(self.croped)
+        self.fig.canvas.draw_idle()
+
+        self.corner1 = [y1, x1]
+        self.corner2 = [y2, x2]
+    
+    def crop(self):
+        rect_crop = RectangleSelector(self.ax1, self.line_select_callback,
+                                        drawtype='box', useblit=True,
+                                        button=[1, 3],  # disable middle button
+                                        minspanx=5, minspany=5,
+                                        spancoords='pixels',
+                                        interactive=True)
+
+        plt.show()
+
+
+
+
+def crop_gui(data):
+
+    data_crop = crop_img(data)
+    
+    data_crop.crop()
+    cropped_img = data_crop.croped
+    corner1 = data_crop.corner1
+    corner2 = data_crop.corner2
+
+    return cropped_img, [corner1, corner2]
+    # plt.figure()
+    # plt.imshow(cropped_img)
+    # plt.colorbar()
+    # plt.show()
+
+def gui_load_data(directory='', title="File name with Data"):
+
+    originalDir = os.getcwd()
+
+    root = tk.Tk(title)
+    # root.withdraw()
+    
+    fname1 = filedialog.askopenfilenames()
+
+    if len(fname1) == 0:
+        fname_last = None
+
+    else:
+        fname_last = fname1
+
+    os.chdir(originalDir)
+    root.destroy()
+    # root.mainloop()
     return fname_last[0]
```

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/integration.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/integration.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-from matplotlib.pyplot import axis
-import numpy as np
-
-'''
-    the 2D integration method here. fourier_integreation1 and 2 and frankotchellappa method
-'''
-def fourier_integration2DShift(dpc_x=None, del_x=1,
-                               dpc_y=None, del_y=1):
-
-    '''
-    This function is the direct use of the CONTINOUS formulation of
-    Frankot-Chellappa, eq 21 in the article:
-
-    T. Frankot and R. Chellappa
-        A Method for Enforcing Integrability in Shape from Shading Algorithms,
-        IEEE Transactions On Pattern Analysis And Machine Intelligence, Vol 10,
-        No 4, Jul 1988
-
-    In addition, it uses the CONTINOUS shift property to avoid singularities
-    at zero frequencies
-    input:
-        dpc_x:              the differential phase along x
-        del_x:              pixel size along x
-        dpc_y:              the differential phase along y 
-        del_y:              pixel size along y         
-    output:
-        phi:                phase calculated from the dpc
-    '''
-    dpc_x = dpc_x / del_x
-    dpc_y = dpc_y / del_y
-
-    dim = dpc_x.shape
-    x_axis = del_x * (np.arange(dim[1]) - round(dim[1]/2))
-    y_axis = del_y * (np.arange(dim[0]) - round(dim[0]/2))
-
-    xx, yy = np.meshgrid(x_axis, y_axis)
-
-    dk_x = 2*np.pi / (dim[1]*del_x)
-    dk_y = 2*np.pi / (dim[0]*del_y)
-
-    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
-    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
-
-    fy, fx = np.meshgrid(ky/2/np.pi, kx/2/np.pi, indexing='ij')
-
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    # fftshift = lambda x: np.fft.fftshift(x)
-    # ifftshift = lambda x: np.fft.ifftshift(x)
-
-    # fx, fy = np.meshgrid(np.fft.fftfreq(dpc_x.shape[1], delx),
-    #                      np.fft.fftfreq(dpc_x.shape[0], dely))
-
-    # xx, yy = wpu.realcoordmatrix(dpc_x.shape[1], delx,
-    #                              dpc_x.shape[0], dely)
-
-    fo_x = np.abs(fx[0,1]*0.33) # shift fx value
-    fo_y = np.abs(fy[1,0]*0.33) # shift fy value
-
-
-    phaseShift = np.exp(2*np.pi*1j*(fo_x*xx + fo_y*yy))  # exp factor for shift
-
-    mult_factor = 1/(2*np.pi*1j)/(fx - fo_x - 1j*fy + 1j*fo_y )
-
-
-    bigGprime = fft2((dpc_x - 1j*dpc_y)*phaseShift)
-    bigG = bigGprime*mult_factor
-
-    phi = ifft2(bigG) / phaseShift
-
-    phi = np.real(phi) - np.min(np.real(phi))  # since the integral have and undefined constant,
-                         # here it is applied an arbritary offset
-
-
-    return phi
-
-
-def gradient_nabla(phi, method='FFT'):
-    '''
-        use fourier transfrom to calculate the displacement from the phase
-        here phase is in a unit of [1/(k_wave)/p_x^2*z]
-    '''
-    if method == 'FFT':
-        fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-        ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-        fftshift = lambda x: np.fft.fftshift(x)
-        # ifftshift = lambda x: np.fft.ifftshift(x)
-        
-        NN, MM = phi.shape
-
-        wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
-                            np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
-
-        wx = fftshift(wx)
-        wy = fftshift(wy)
-        # print(wx, wy)
-
-        displace_x = np.real(ifft2(1j*wx*fft2(phi)))
-        displace_y = np.real(ifft2(1j*wy*fft2(phi)))
-    elif method == 'diff':
-        displace_x = np.gradient(phi, axis=1)
-        displace_y = np.gradient(phi, axis=0)
-    else:
-        print('wrong method for subpixel shift, should be FFT or interp')
-        import sys
-        sys.exit()
-
-    return [displace_x, displace_y]
-
-
-def frankotchellappa(dpc_x,dpc_y):
-    '''
-        Frankt-Chellappa Algrotihm
-        input:
-            dpc_x:              the differential phase along x
-            dpc_y:              the differential phase along y       
-        output:
-            phi:                phase calculated from the dpc
-    '''
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    fftshift = lambda x: np.fft.fftshift(x)
-    # ifftshift = lambda x: np.fft.ifftshift(x)
-    
-    NN, MM = dpc_x.shape
-    
-    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
-                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
-    wx = fftshift(wx)
-    wy = fftshift(wy)
-    numerator = -1j*wx*fft2(dpc_x) -1j*wy*fft2(dpc_y)
-    # here use the numpy.fmax method to eliminate the zero point of the division
-    denominator = np.fmax((wx)**2 + (wy)**2, np.finfo(float).eps)
-
-    div = numerator/denominator
-
-
-    phi = np.real(ifft2(div))
-
-    phi -= np.mean(np.real(phi))
-
-    return phi
-
-def frankotchellappa_ord2(dpc_x,dpc_y):
-    '''
-        Frankt-Chellappa Algrotihm
-        input:
-            dpc_x:              the differential phase along x
-            dpc_y:              the differential phase along y       
-        output:
-            phi:                phase calculated from the dpc
-    '''
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-    fftshift = lambda x: np.fft.fftshift(x)
-    # ifftshift = lambda x: np.fft.ifftshift(x)
-    
-    NN, MM = dpc_x.shape
-
-    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
-                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
-    wx = fftshift(wx)
-    wy = fftshift(wy)
-    numerator = fft2(dpc_x) + fft2(dpc_y)
-    # here use the numpy.fmax method to eliminate the zero point of the division
-    denominator = np.fmax((wx)**2 + (wy)**2, np.finfo(float).eps)
-
-    div = numerator/denominator
-
-
-    phi = np.real(ifft2(div))
-
-    phi -= np.mean(np.real(phi))
-
-    return phi
-
-
-
-def frankotchellappa_1D(dpc, axis=0):
-    # do frankotchellappa integration along specific axis
-    fftshift = lambda x: np.fft.fftshift(x, axes=axis)
-    ifftshift = lambda x: np.fft.ifftshift(x, axes=axis)
-    fft = lambda x: fftshift(np.fft.fft(ifftshift(x), axis=axis))
-    ifft = lambda x: fftshift(np.fft.ifft(ifftshift(x), axis=axis))
-
-    NN, MM = dpc.shape
-
-    wx, wy = np.meshgrid(np.fft.fftfreq(MM) * 2 * np.pi,
-                         np.fft.fftfreq(NN) * 2 * np.pi,
-                         indexing='xy')
-    wx = fftshift(wx)
-    wy = fftshift(wy)
-    ww = wx if axis==1 else wy
-
-    numerator = -1j * ww * fft(dpc)
-    # here use the np.fmax method to eliminate the zero point of the division
-    denominator = np.fmax((ww)**2, np.finfo(float).eps)
-
-    div = numerator / denominator
-
-    integ = np.real(ifft(div))
-
-    integ -= np.mean(np.real(integ))
-
+from matplotlib.pyplot import axis
+import numpy as np
+
+'''
+    the 2D integration method here. fourier_integreation1 and 2 and frankotchellappa method
+'''
+def fourier_integration2DShift(dpc_x=None, del_x=1,
+                               dpc_y=None, del_y=1):
+
+    '''
+    This function is the direct use of the CONTINOUS formulation of
+    Frankot-Chellappa, eq 21 in the article:
+
+    T. Frankot and R. Chellappa
+        A Method for Enforcing Integrability in Shape from Shading Algorithms,
+        IEEE Transactions On Pattern Analysis And Machine Intelligence, Vol 10,
+        No 4, Jul 1988
+
+    In addition, it uses the CONTINOUS shift property to avoid singularities
+    at zero frequencies
+    input:
+        dpc_x:              the differential phase along x
+        del_x:              pixel size along x
+        dpc_y:              the differential phase along y 
+        del_y:              pixel size along y         
+    output:
+        phi:                phase calculated from the dpc
+    '''
+    dpc_x = dpc_x / del_x
+    dpc_y = dpc_y / del_y
+
+    dim = dpc_x.shape
+    x_axis = del_x * (np.arange(dim[1]) - round(dim[1]/2))
+    y_axis = del_y * (np.arange(dim[0]) - round(dim[0]/2))
+
+    xx, yy = np.meshgrid(x_axis, y_axis)
+
+    dk_x = 2*np.pi / (dim[1]*del_x)
+    dk_y = 2*np.pi / (dim[0]*del_y)
+
+    kx = dk_x * (np.arange(dim[1]) - round(dim[1]/2))
+    ky = dk_y * (np.arange(dim[0]) - round(dim[0]/2))
+
+    fy, fx = np.meshgrid(ky/2/np.pi, kx/2/np.pi, indexing='ij')
+
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    # fftshift = lambda x: np.fft.fftshift(x)
+    # ifftshift = lambda x: np.fft.ifftshift(x)
+
+    # fx, fy = np.meshgrid(np.fft.fftfreq(dpc_x.shape[1], delx),
+    #                      np.fft.fftfreq(dpc_x.shape[0], dely))
+
+    # xx, yy = wpu.realcoordmatrix(dpc_x.shape[1], delx,
+    #                              dpc_x.shape[0], dely)
+
+    fo_x = np.abs(fx[0,1]*0.33) # shift fx value
+    fo_y = np.abs(fy[1,0]*0.33) # shift fy value
+
+
+    phaseShift = np.exp(2*np.pi*1j*(fo_x*xx + fo_y*yy))  # exp factor for shift
+
+    mult_factor = 1/(2*np.pi*1j)/(fx - fo_x - 1j*fy + 1j*fo_y )
+
+
+    bigGprime = fft2((dpc_x - 1j*dpc_y)*phaseShift)
+    bigG = bigGprime*mult_factor
+
+    phi = ifft2(bigG) / phaseShift
+
+    phi = np.real(phi) - np.min(np.real(phi))  # since the integral have and undefined constant,
+                         # here it is applied an arbritary offset
+
+
+    return phi
+
+
+def gradient_nabla(phi, method='FFT'):
+    '''
+        use fourier transfrom to calculate the displacement from the phase
+        here phase is in a unit of [1/(k_wave)/p_x^2*z]
+    '''
+    if method == 'FFT':
+        fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+        ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+        fftshift = lambda x: np.fft.fftshift(x)
+        # ifftshift = lambda x: np.fft.ifftshift(x)
+        
+        NN, MM = phi.shape
+
+        wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
+                            np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
+
+        wx = fftshift(wx)
+        wy = fftshift(wy)
+        # print(wx, wy)
+
+        displace_x = np.real(ifft2(1j*wx*fft2(phi)))
+        displace_y = np.real(ifft2(1j*wy*fft2(phi)))
+    elif method == 'diff':
+        displace_x = np.gradient(phi, axis=1)
+        displace_y = np.gradient(phi, axis=0)
+    else:
+        print('wrong method for subpixel shift, should be FFT or interp')
+        import sys
+        sys.exit()
+
+    return [displace_x, displace_y]
+
+
+def frankotchellappa(dpc_x,dpc_y):
+    '''
+        Frankt-Chellappa Algrotihm
+        input:
+            dpc_x:              the differential phase along x
+            dpc_y:              the differential phase along y       
+        output:
+            phi:                phase calculated from the dpc
+    '''
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    fftshift = lambda x: np.fft.fftshift(x)
+    # ifftshift = lambda x: np.fft.ifftshift(x)
+    
+    NN, MM = dpc_x.shape
+    
+    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
+                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
+    wx = fftshift(wx)
+    wy = fftshift(wy)
+    numerator = -1j*wx*fft2(dpc_x) -1j*wy*fft2(dpc_y)
+    # here use the numpy.fmax method to eliminate the zero point of the division
+    denominator = np.fmax((wx)**2 + (wy)**2, np.finfo(float).eps)
+
+    div = numerator/denominator
+
+
+    phi = np.real(ifft2(div))
+
+    phi -= np.mean(np.real(phi))
+
+    return phi
+
+def frankotchellappa_ord2(dpc_x,dpc_y):
+    '''
+        Frankt-Chellappa Algrotihm
+        input:
+            dpc_x:              the differential phase along x
+            dpc_y:              the differential phase along y       
+        output:
+            phi:                phase calculated from the dpc
+    '''
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+    fftshift = lambda x: np.fft.fftshift(x)
+    # ifftshift = lambda x: np.fft.ifftshift(x)
+    
+    NN, MM = dpc_x.shape
+
+    wx, wy = np.meshgrid(np.fft.fftfreq(MM)*2*np.pi,
+                         np.fft.fftfreq(NN)*2*np.pi, indexing='xy')
+    wx = fftshift(wx)
+    wy = fftshift(wy)
+    numerator = fft2(dpc_x) + fft2(dpc_y)
+    # here use the numpy.fmax method to eliminate the zero point of the division
+    denominator = np.fmax((wx)**2 + (wy)**2, np.finfo(float).eps)
+
+    div = numerator/denominator
+
+
+    phi = np.real(ifft2(div))
+
+    phi -= np.mean(np.real(phi))
+
+    return phi
+
+
+
+def frankotchellappa_1D(dpc, axis=0):
+    # do frankotchellappa integration along specific axis
+    fftshift = lambda x: np.fft.fftshift(x, axes=axis)
+    ifftshift = lambda x: np.fft.ifftshift(x, axes=axis)
+    fft = lambda x: fftshift(np.fft.fft(ifftshift(x), axis=axis))
+    ifft = lambda x: fftshift(np.fft.ifft(ifftshift(x), axis=axis))
+
+    NN, MM = dpc.shape
+
+    wx, wy = np.meshgrid(np.fft.fftfreq(MM) * 2 * np.pi,
+                         np.fft.fftfreq(NN) * 2 * np.pi,
+                         indexing='xy')
+    wx = fftshift(wx)
+    wy = fftshift(wy)
+    ww = wx if axis==1 else wy
+
+    numerator = -1j * ww * fft(dpc)
+    # here use the np.fmax method to eliminate the zero point of the division
+    denominator = np.fmax((ww)**2, np.finfo(float).eps)
+
+    div = numerator / denominator
+
+    integ = np.real(ifft(div))
+
+    integ -= np.mean(np.real(integ))
+
     return integ
```

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/main.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/main.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_find.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/pattern_find.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-'''
-@Time    	: 08 / 19 / 2022
-@Author  	: Zhi Qiao
-@Contact	: z.qiao1989@gmail.com
-@File    	: pattern_find.py
-@Software	: AbsolutePhase
-@Desc		: code to find the area of the speckle pattern in the calibrated data
-'''
-
-from PIL import Image as tif_image
-import os
-import numpy as np
-from matplotlib import pyplot as plt
-import cv2
-import scipy.io as sio
-
-from aps.common.measurment.beamline.wf.func_light import prColor
-
-def normalize(v):
-    return (v-np.amin(v)) / (np.amax(v) - np.amin(v))
-
-def image_transfer(img, h_flip=0, v_flip=0, transpose=0, direc='forward'):
-    img_new = img.copy()
-    if direc == 'forward':
-        if h_flip:
-            img_new = np.fliplr(img_new)
-        if v_flip:
-            img_new = np.flipud(img_new)
-        if transpose:
-            img_new = img_new.transpose()
-    elif direc == 'backward':
-        if transpose:
-            img_new = img_new.transpose()
-        if v_flip:
-            img_new = np.flipud(img_new)
-        if h_flip:
-            img_new = np.fliplr(img_new)
-        
-        
-    return img_new
-
-
-def pattern_match(pattern_path, img_path, pattern_size, img_trans, show_fig=True):
-    '''
-        use opencv to find matched pattern with the image
-        input:
-            pattern_path:           path to pattern file (npy)
-            img_path:               path to image file (tif)
-            pattern_size:             pattern size
-            img_trans:              pattern transformation to match image
-            show_fig:               show the plot figure or not
-
-    '''
-    file_folder = os.path.dirname(img_path)
-
-    p_x = 0.65e-6
-    # for 5um pattern
-    pattern_pixel = pattern_size
-    scale = pattern_pixel / p_x 
-
-    # region to use as template
-    row_start = 800
-    row_end = 1200
-    col_start = 800
-    col_end = 1200
-
-    H_flip, V_flip, Dia_transpose = img_trans
-
-    # load data
-    prColor('MESSAGE: sample image,  ' + img_path, 'green')
-    I_img = tif_image.open(img_path)
-
-    '''
-    rotate the image to match the design pattern orientation
-    '''
-    I_img_rot = image_transfer(np.array(I_img), H_flip, V_flip, Dia_transpose)
-    I_img = I_img_rot.astype(np.float32)
-
-    prColor('MESSAGE: pattern image,  ' + pattern_path, 'green')
-    I_pattern = np.load(pattern_path)
-
-    I_pattern = normalize(1-I_pattern) * 255
-    I_pattern = I_pattern.astype(np.float32)
-
-    I_img_norm = normalize(I_img[row_start:row_end, col_start:col_end]) * 255
-    I_img_norm = I_img_norm.astype(np.float32)
-    
-    h, w = I_pattern.shape
-
-    # All the 6 methods for comparison in a list
-    # methods = ['cv2.TM_CCOEFF', 'cv2.TM_CCOEFF_NORMED', 'cv2.TM_CCORR',
-    #             'cv2.TM_CCORR_NORMED', 'cv2.TM_SQDIFF', 'cv2.TM_SQDIFF_NORMED']
-    meth = 'cv2.TM_CCOEFF'
-
-    temp = np.copy(I_pattern)
-
-    I_pattern_reshape = cv2.resize(temp, None, fx=scale, fy=scale, interpolation=cv2.INTER_NEAREST )
-    
-    template = I_img_norm
-    
-    n_template_row, n_template_col = template.shape
-
-    method = eval(meth)
-
-    # Apply template Matching
-    res = cv2.matchTemplate(I_pattern_reshape,template,method)
-    min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
-
-    # If the method is TM_SQDIFF or TM_SQDIFF_NORMED, take minimum
-    if method in [cv2.TM_SQDIFF, cv2.TM_SQDIFF_NORMED]:
-        top_left = min_loc
-    else:
-        top_left = max_loc
-    bottom_right = (top_left[0] + n_template_col, top_left[1] + n_template_row)
-    color = (255, 0, 0)
-    print('region position left top: {}, bottom right: {}'.format(top_left, bottom_right))
-    img_small = I_pattern_reshape[top_left[1]:bottom_right[1], top_left[0]:bottom_right[0]]
-    cv2.rectangle(I_pattern_reshape,top_left, bottom_right, color, 1)
-
-    if show_fig:
-        plt.figure()
-        plt.subplot(131)
-        plt.imshow(res,cmap = 'gray')
-        plt.title('Matching Result')
-        plt.subplot(132)
-        plt.imshow(I_pattern_reshape,cmap = 'gray')
-        plt.title('full image')
-        plt.subplot(133)
-        plt.imshow(img_small,cmap = 'gray')
-        plt.title('Detected Point')
-        plt.suptitle(meth)
-
-        plt.figure()
-        plt.subplot(131)
-        plt.imshow(img_small,cmap = 'gray')
-        plt.title('Matching Result')
-        plt.subplot(132)
-        plt.imshow(template,cmap = 'gray')
-        plt.title('full image')
-        plt.subplot(133)
-        plt.imshow(255- img_small + I_img_norm)
-        plt.title('diff image')
-
-        plt.show()
-
-    '''
-        save results
-    '''
-    n_row, n_col = I_img.shape
-    # pad the pattern data to have enough size
-    n_row_pattern, n_col_pattern = I_pattern_reshape.shape
-
-    n_pad = np.amax([0, -(top_left[1]-row_start), -(top_left[0]-col_start),
-                    bottom_right[1]+n_row-row_end-n_row_pattern,
-                    bottom_right[0]+n_col-col_end-n_col_pattern])
-    print('padding size: {}'.format(n_pad))
-
-    I_pattern_reshape = np.pad(I_pattern_reshape, (n_pad, n_pad), 'constant', constant_values=(0, 0))
-
-    Img_pattern = I_pattern_reshape[top_left[1]-row_start+n_pad:bottom_right[1]+n_row-row_end+n_pad, 
-                                    top_left[0]-col_start+n_pad:bottom_right[0]+n_col-col_end+n_pad]
-
-
-    Img_pattern = image_transfer(Img_pattern, H_flip, V_flip, Dia_transpose, direc='backward')
-
-    I_img = image_transfer(I_img, H_flip, V_flip, Dia_transpose, direc='backward')
-
-    im = tif_image.fromarray(Img_pattern*I_img)
-    im.save(os.path.join(file_folder, 'pattern.tif'))
-    prColor('saved pattern image: {}'.format(os.path.join(file_folder, 'pattern.tif')), 'cyan')
-    
-    sio.savemat(os.path.join(file_folder, 'pattern.mat'), {'I_pattern':Img_pattern, 'I_origin':I_img})
-    prColor('saved data: {}'.format(os.path.join(file_folder, 'pattern.mat')), 'cyan')
-
-
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+'''
+@Time    	: 08 / 19 / 2022
+@Author  	: Zhi Qiao
+@Contact	: z.qiao1989@gmail.com
+@File    	: pattern_find.py
+@Software	: AbsolutePhase
+@Desc		: code to find the area of the speckle pattern in the calibrated data
+'''
+
+from PIL import Image as tif_image
+import os
+import numpy as np
+from matplotlib import pyplot as plt
+import cv2
+import scipy.io as sio
+
+from aps.common.measurment.beamline.wf.func_light import prColor
+
+def normalize(v):
+    return (v-np.amin(v)) / (np.amax(v) - np.amin(v))
+
+def image_transfer(img, h_flip=0, v_flip=0, transpose=0, direc='forward'):
+    img_new = img.copy()
+    if direc == 'forward':
+        if h_flip:
+            img_new = np.fliplr(img_new)
+        if v_flip:
+            img_new = np.flipud(img_new)
+        if transpose:
+            img_new = img_new.transpose()
+    elif direc == 'backward':
+        if transpose:
+            img_new = img_new.transpose()
+        if v_flip:
+            img_new = np.flipud(img_new)
+        if h_flip:
+            img_new = np.fliplr(img_new)
+        
+        
+    return img_new
+
+
+def pattern_match(pattern_path, img_path, pattern_size, img_trans, show_fig=True):
+    '''
+        use opencv to find matched pattern with the image
+        input:
+            pattern_path:           path to pattern file (npy)
+            img_path:               path to image file (tif)
+            pattern_size:             pattern size
+            img_trans:              pattern transformation to match image
+            show_fig:               show the plot figure or not
+
+    '''
+    file_folder = os.path.dirname(img_path)
+
+    p_x = 0.65e-6
+    # for 5um pattern
+    pattern_pixel = pattern_size
+    scale = pattern_pixel / p_x 
+
+    # region to use as template
+    row_start = 800
+    row_end = 1200
+    col_start = 800
+    col_end = 1200
+
+    H_flip, V_flip, Dia_transpose = img_trans
+
+    # load data
+    prColor('MESSAGE: sample image,  ' + img_path, 'green')
+    I_img = tif_image.open(img_path)
+
+    '''
+    rotate the image to match the design pattern orientation
+    '''
+    I_img_rot = image_transfer(np.array(I_img), H_flip, V_flip, Dia_transpose)
+    I_img = I_img_rot.astype(np.float32)
+
+    prColor('MESSAGE: pattern image,  ' + pattern_path, 'green')
+    I_pattern = np.load(pattern_path)
+
+    I_pattern = normalize(1-I_pattern) * 255
+    I_pattern = I_pattern.astype(np.float32)
+
+    I_img_norm = normalize(I_img[row_start:row_end, col_start:col_end]) * 255
+    I_img_norm = I_img_norm.astype(np.float32)
+    
+    h, w = I_pattern.shape
+
+    # All the 6 methods for comparison in a list
+    # methods = ['cv2.TM_CCOEFF', 'cv2.TM_CCOEFF_NORMED', 'cv2.TM_CCORR',
+    #             'cv2.TM_CCORR_NORMED', 'cv2.TM_SQDIFF', 'cv2.TM_SQDIFF_NORMED']
+    meth = 'cv2.TM_CCOEFF'
+
+    temp = np.copy(I_pattern)
+
+    I_pattern_reshape = cv2.resize(temp, None, fx=scale, fy=scale, interpolation=cv2.INTER_NEAREST )
+    
+    template = I_img_norm
+    
+    n_template_row, n_template_col = template.shape
+
+    method = eval(meth)
+
+    # Apply template Matching
+    res = cv2.matchTemplate(I_pattern_reshape,template,method)
+    min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
+
+    # If the method is TM_SQDIFF or TM_SQDIFF_NORMED, take minimum
+    if method in [cv2.TM_SQDIFF, cv2.TM_SQDIFF_NORMED]:
+        top_left = min_loc
+    else:
+        top_left = max_loc
+    bottom_right = (top_left[0] + n_template_col, top_left[1] + n_template_row)
+    color = (255, 0, 0)
+    print('region position left top: {}, bottom right: {}'.format(top_left, bottom_right))
+    img_small = I_pattern_reshape[top_left[1]:bottom_right[1], top_left[0]:bottom_right[0]]
+    cv2.rectangle(I_pattern_reshape,top_left, bottom_right, color, 1)
+
+    if show_fig:
+        plt.figure()
+        plt.subplot(131)
+        plt.imshow(res,cmap = 'gray')
+        plt.title('Matching Result')
+        plt.subplot(132)
+        plt.imshow(I_pattern_reshape,cmap = 'gray')
+        plt.title('full image')
+        plt.subplot(133)
+        plt.imshow(img_small,cmap = 'gray')
+        plt.title('Detected Point')
+        plt.suptitle(meth)
+
+        plt.figure()
+        plt.subplot(131)
+        plt.imshow(img_small,cmap = 'gray')
+        plt.title('Matching Result')
+        plt.subplot(132)
+        plt.imshow(template,cmap = 'gray')
+        plt.title('full image')
+        plt.subplot(133)
+        plt.imshow(255- img_small + I_img_norm)
+        plt.title('diff image')
+
+        plt.show()
+
+    '''
+        save results
+    '''
+    n_row, n_col = I_img.shape
+    # pad the pattern data to have enough size
+    n_row_pattern, n_col_pattern = I_pattern_reshape.shape
+
+    n_pad = np.amax([0, -(top_left[1]-row_start), -(top_left[0]-col_start),
+                    bottom_right[1]+n_row-row_end-n_row_pattern,
+                    bottom_right[0]+n_col-col_end-n_col_pattern])
+    print('padding size: {}'.format(n_pad))
+
+    I_pattern_reshape = np.pad(I_pattern_reshape, (n_pad, n_pad), 'constant', constant_values=(0, 0))
+
+    Img_pattern = I_pattern_reshape[top_left[1]-row_start+n_pad:bottom_right[1]+n_row-row_end+n_pad, 
+                                    top_left[0]-col_start+n_pad:bottom_right[0]+n_col-col_end+n_pad]
+
+
+    Img_pattern = image_transfer(Img_pattern, H_flip, V_flip, Dia_transpose, direc='backward')
+
+    I_img = image_transfer(I_img, H_flip, V_flip, Dia_transpose, direc='backward')
+
+    im = tif_image.fromarray(Img_pattern*I_img)
+    im.save(os.path.join(file_folder, 'pattern.tif'))
+    prColor('saved pattern image: {}'.format(os.path.join(file_folder, 'pattern.tif')), 'cyan')
+    
+    sio.savemat(os.path.join(file_folder, 'pattern.mat'), {'I_pattern':Img_pattern, 'I_origin':I_img})
+    prColor('saved data: {}'.format(os.path.join(file_folder, 'pattern.mat')), 'cyan')
+
+
```

### Comparing `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_propagate.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/wf/pattern_propagate.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-'''
-@Time    	: 08 / 19 / 2022
-@Author  	: Zhi Qiao
-@Contact	: z.qiao1989@gmail.com
-@File    	: pattern_propagate.py
-@Software	: AbsolutePhase
-@Desc		: code to propagate the matched pattern
-'''
-
-
-from PIL import Image as tif_image
-import os
-import numpy as np
-from matplotlib import pyplot as plt
-import scipy.io as sio
-import scipy.constants as sc
-from scipy.ndimage import gaussian_filter
-
-from aps.common.measurment.beamline.wf.func_light import prColor
-from aps.common.measurment.beamline.wf.diffraction_process import diffraction_prop
-
-
-def load_pattern(file_path, print_key=True):
-    if os.path.exists(file_path):
-        data_content = sio.loadmat(file_path)
-        prColor('variable name: {}'.format(data_content.keys()), 'light_purple')
-    else:
-        prColor('Error: wrong file path!', 'cyan')
-        os.exit()
-
-    I_pattern = data_content['I_pattern']
-    I_img = data_content['I_origin']
-    return I_pattern, I_img
-
-def load_tiff(file_path):
-    if os.path.exists(file_path):
-        im = tif_image.open(file_path)
-        im = np.array(im)
-    else:
-        prColor('Error: wrong file path!', 'cyan')
-        os.exit()
-
-    return im
-
-def normalize(v):
-    return (v-np.amin(v)) / (np.amax(v) - np.amin(v))
-
-def PSF_detector(d_reso, p_x, I):
-    '''
-        the resolution degrades due to PSF
-        d_reso:
-            detector resolution
-        p_x:
-            pixel size
-        I:
-            the data
-    '''
-    M, N = I.shape
-    y_axis = np.arange(-M//2, M//2) * p_x
-    x_axis = np.arange(-N//2, N//2) * p_x
-    XX, YY = np.meshgrid(x_axis, y_axis)
-
-    sigma = d_reso / (2 * np.sqrt(np.log(2)))
-    PSF = np.exp(-(XX**2 + YY**2)/(sigma)**2)
-
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-
-    return np.abs(ifft2(fft2(I)*fft2(PSF))) 
-
-
-def PSF_coherence(sigma_h, sigma_v, p_x, I):
-    '''
-        the resolution degrades due to temporal or spatial coherence
-        sigma_h:
-            horizontal convolution kernel size
-        sigma_v:
-            vertical convolution kernel size
-        p_x:
-            pixel size
-        I:
-            the data
-    '''
-    M, N = I.shape
-    y_axis = np.arange(-M//2, M//2) * p_x
-    x_axis = np.arange(-N//2, N//2) * p_x
-    XX, YY = np.meshgrid(x_axis, y_axis)
-
-
-    PSF = np.exp(-(XX**2/sigma_h**2 + YY**2/sigma_v**2))
-
-    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
-    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
-
-    return np.abs(ifft2(fft2(I)*fft2(PSF)))
-
-def sphrical_wavefront(n_size, distance, p_x, wavelength):
-    '''
-        n_size:
-            the data shape
-        distance:
-            source distance to speckle
-            [v, h]
-        p_x:
-            pixel size
-        wavelength:
-            wavelength
-    '''
-    # generate the simulated incident wavefront from the source
-    k = 2 * np.pi / wavelength
-    M, N = n_size
-    y_axis = np.arange(-M//2, M//2) * p_x
-    x_axis = np.arange(-N//2, N//2) * p_x
-    XX, YY = np.meshgrid(x_axis, y_axis)
-
-    phase_illum = np.exp(1j*k*(XX**2/(2*distance[1])+YY**2/(2*distance[0])))
-
-    return phase_illum
-
-def pattern_prop(pattern_path, pattern_para=[0.613, 0.5*np.pi], prop_para=[14e3, 200e-3], 
-                source_para=[35, 29], show_fig=True):
-    '''
-        propagate the matched pattern to get pattern-ref image
-        input:
-                pattern_path:           path to matched pattern file, mat
- 
-                pattern_para:           [T_transmission, phase]
-                                        [transmission of pattern, phase shifting of pattern]
-                prop_para:              parameters for propogation
-                                        [energy(eV), distance]
-                source_para:            source distance
-                                        [vertical, horizontal]
-    '''
-    T_transmission, R_phase = pattern_para
-
-    # energy
-    # energy = 14e3
-    energy = prop_para[0]
-    c_w = sc.value('inverse meter-electron volt relationship') / energy
-
-    # pixel size
-    p_x = 0.65e-6
-    # distance
-    d_prop = prop_para[1]
-    # theoretical resolution of the detector
-    det_resolution = np.floor(2.2e-6/p_x + 1) * p_x
-
-    # coherence of the source
-    source_h = 86.9e-9
-    source_v = 39.7e-9
-
-    d_source2pattern_v, d_source2pattern_h = source_para
-
-    d_source2pattern = [d_source2pattern_v, d_source2pattern_h]
-
-    # calculate sigma kernel size for coherence
-    sigma_h = source_h/d_source2pattern_h*d_prop
-    sigma_v = source_v/d_source2pattern_v*d_prop
-
-    # I_pattern:  pattern matched,   I_img: ref image used to find the matched pattern
-    I_pattern, I_ref = load_pattern(pattern_path, print_key=True)
-    I_pattern = normalize(I_pattern)
-
-    # propagation
-    A_pattern = np.sqrt((1-T_transmission)*I_pattern+T_transmission) * np.exp(1j*I_pattern*R_phase) \
-                * sphrical_wavefront(I_pattern.shape, d_source2pattern, p_x, wavelength=c_w)
-
-    N_pad = 1000
-    if N_pad == 0:
-        A_prop, L_out = diffraction_prop(A_pattern, p_x, d_prop, c_w, 'TF')
-    else:
-        A_pattern_pad = np.pad(A_pattern, (N_pad, N_pad), mode='constant', constant_values=(0,0))
-        A_prop, L_out = diffraction_prop(A_pattern_pad, p_x, d_prop, c_w, 'TF')
-        A_prop = A_prop[N_pad:-N_pad, N_pad:-N_pad]
-    
-    I_prop = np.abs(A_prop) ** 2
-
-    # the detector PSF influence
-    I_det = PSF_detector(det_resolution, p_x, I_prop)
-
-    I_coh = PSF_coherence(sigma_h, sigma_v, p_x, I_det)
-
-    # use gaussian fiter for the image
-    I_blur = gaussian_filter(I_coh, sigma=3)
-
-    if show_fig:
-        plt.figure()
-        plt.subplot(221)
-        plt.imshow(I_ref[0:200,0:200])
-        plt.subplot(222)
-        plt.imshow(I_det[0:200,0:200])
-        plt.subplot(223)
-        plt.imshow(I_coh[0:200,0:200])
-        plt.subplot(224)
-        plt.imshow(I_blur[0:200,0:200])
-        plt.show()
-
-        plt.figure(figsize=(15,8))
-        plt.subplot(241)
-        plt.title('top right')
-        plt.imshow(I_ref[0:200,0:200])
-        plt.colorbar()
-        plt.subplot(242)
-        plt.title('top left')
-        plt.imshow(I_ref[0:200,-200:])
-        plt.colorbar()
-        plt.subplot(243)
-        plt.title('bottom right')
-        plt.imshow(I_ref[-200:,0:200])
-        plt.colorbar()
-        plt.subplot(244)
-        plt.title('bottom left')
-        plt.imshow(I_ref[-200:,-200:])
-        plt.colorbar()
-
-        plt.subplot(245)
-        plt.imshow(I_coh[0:200,0:200])
-        plt.title('top right')
-        plt.colorbar()
-        plt.subplot(246)
-        plt.title('top left')
-        plt.imshow(I_coh[0:200,-200:])
-        plt.colorbar()
-        plt.subplot(247)
-        plt.title('bottom right')
-        plt.imshow(I_coh[-200:,0:200])
-        plt.colorbar()
-        plt.subplot(248)
-        plt.title('bottom left')
-        plt.imshow(I_coh[-200:,-200:])
-        plt.colorbar()
-        plt.show()
-
-    return I_blur, I_coh, I_det, I_pattern
-
-
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+'''
+@Time    	: 08 / 19 / 2022
+@Author  	: Zhi Qiao
+@Contact	: z.qiao1989@gmail.com
+@File    	: pattern_propagate.py
+@Software	: AbsolutePhase
+@Desc		: code to propagate the matched pattern
+'''
+
+
+from PIL import Image as tif_image
+import os
+import numpy as np
+from matplotlib import pyplot as plt
+import scipy.io as sio
+import scipy.constants as sc
+from scipy.ndimage import gaussian_filter
+
+from aps.common.measurment.beamline.wf.func_light import prColor
+from aps.common.measurment.beamline.wf.diffraction_process import diffraction_prop
+
+
+def load_pattern(file_path, print_key=True):
+    if os.path.exists(file_path):
+        data_content = sio.loadmat(file_path)
+        prColor('variable name: {}'.format(data_content.keys()), 'light_purple')
+    else:
+        prColor('Error: wrong file path!', 'cyan')
+        os.exit()
+
+    I_pattern = data_content['I_pattern']
+    I_img = data_content['I_origin']
+    return I_pattern, I_img
+
+def load_tiff(file_path):
+    if os.path.exists(file_path):
+        im = tif_image.open(file_path)
+        im = np.array(im)
+    else:
+        prColor('Error: wrong file path!', 'cyan')
+        os.exit()
+
+    return im
+
+def normalize(v):
+    return (v-np.amin(v)) / (np.amax(v) - np.amin(v))
+
+def PSF_detector(d_reso, p_x, I):
+    '''
+        the resolution degrades due to PSF
+        d_reso:
+            detector resolution
+        p_x:
+            pixel size
+        I:
+            the data
+    '''
+    M, N = I.shape
+    y_axis = np.arange(-M//2, M//2) * p_x
+    x_axis = np.arange(-N//2, N//2) * p_x
+    XX, YY = np.meshgrid(x_axis, y_axis)
+
+    sigma = d_reso / (2 * np.sqrt(np.log(2)))
+    PSF = np.exp(-(XX**2 + YY**2)/(sigma)**2)
+
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+
+    return np.abs(ifft2(fft2(I)*fft2(PSF))) 
+
+
+def PSF_coherence(sigma_h, sigma_v, p_x, I):
+    '''
+        the resolution degrades due to temporal or spatial coherence
+        sigma_h:
+            horizontal convolution kernel size
+        sigma_v:
+            vertical convolution kernel size
+        p_x:
+            pixel size
+        I:
+            the data
+    '''
+    M, N = I.shape
+    y_axis = np.arange(-M//2, M//2) * p_x
+    x_axis = np.arange(-N//2, N//2) * p_x
+    XX, YY = np.meshgrid(x_axis, y_axis)
+
+
+    PSF = np.exp(-(XX**2/sigma_h**2 + YY**2/sigma_v**2))
+
+    fft2 = lambda x: np.fft.fftshift(np.fft.fft2(np.fft.ifftshift(x)))
+    ifft2 = lambda x: np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(x)))
+
+    return np.abs(ifft2(fft2(I)*fft2(PSF)))
+
+def sphrical_wavefront(n_size, distance, p_x, wavelength):
+    '''
+        n_size:
+            the data shape
+        distance:
+            source distance to speckle
+            [v, h]
+        p_x:
+            pixel size
+        wavelength:
+            wavelength
+    '''
+    # generate the simulated incident wavefront from the source
+    k = 2 * np.pi / wavelength
+    M, N = n_size
+    y_axis = np.arange(-M//2, M//2) * p_x
+    x_axis = np.arange(-N//2, N//2) * p_x
+    XX, YY = np.meshgrid(x_axis, y_axis)
+
+    phase_illum = np.exp(1j*k*(XX**2/(2*distance[1])+YY**2/(2*distance[0])))
+
+    return phase_illum
+
+def pattern_prop(pattern_path, pattern_para=[0.613, 0.5*np.pi], prop_para=[14e3, 200e-3], 
+                source_para=[35, 29], show_fig=True):
+    '''
+        propagate the matched pattern to get pattern-ref image
+        input:
+                pattern_path:           path to matched pattern file, mat
+ 
+                pattern_para:           [T_transmission, phase]
+                                        [transmission of pattern, phase shifting of pattern]
+                prop_para:              parameters for propogation
+                                        [energy(eV), distance]
+                source_para:            source distance
+                                        [vertical, horizontal]
+    '''
+    T_transmission, R_phase = pattern_para
+
+    # energy
+    # energy = 14e3
+    energy = prop_para[0]
+    c_w = sc.value('inverse meter-electron volt relationship') / energy
+
+    # pixel size
+    p_x = 0.65e-6
+    # distance
+    d_prop = prop_para[1]
+    # theoretical resolution of the detector
+    det_resolution = np.floor(2.2e-6/p_x + 1) * p_x
+
+    # coherence of the source
+    source_h = 86.9e-9
+    source_v = 39.7e-9
+
+    d_source2pattern_v, d_source2pattern_h = source_para
+
+    d_source2pattern = [d_source2pattern_v, d_source2pattern_h]
+
+    # calculate sigma kernel size for coherence
+    sigma_h = source_h/d_source2pattern_h*d_prop
+    sigma_v = source_v/d_source2pattern_v*d_prop
+
+    # I_pattern:  pattern matched,   I_img: ref image used to find the matched pattern
+    I_pattern, I_ref = load_pattern(pattern_path, print_key=True)
+    I_pattern = normalize(I_pattern)
+
+    # propagation
+    A_pattern = np.sqrt((1-T_transmission)*I_pattern+T_transmission) * np.exp(1j*I_pattern*R_phase) \
+                * sphrical_wavefront(I_pattern.shape, d_source2pattern, p_x, wavelength=c_w)
+
+    N_pad = 1000
+    if N_pad == 0:
+        A_prop, L_out = diffraction_prop(A_pattern, p_x, d_prop, c_w, 'TF')
+    else:
+        A_pattern_pad = np.pad(A_pattern, (N_pad, N_pad), mode='constant', constant_values=(0,0))
+        A_prop, L_out = diffraction_prop(A_pattern_pad, p_x, d_prop, c_w, 'TF')
+        A_prop = A_prop[N_pad:-N_pad, N_pad:-N_pad]
+    
+    I_prop = np.abs(A_prop) ** 2
+
+    # the detector PSF influence
+    I_det = PSF_detector(det_resolution, p_x, I_prop)
+
+    I_coh = PSF_coherence(sigma_h, sigma_v, p_x, I_det)
+
+    # use gaussian fiter for the image
+    I_blur = gaussian_filter(I_coh, sigma=3)
+
+    if show_fig:
+        plt.figure()
+        plt.subplot(221)
+        plt.imshow(I_ref[0:200,0:200])
+        plt.subplot(222)
+        plt.imshow(I_det[0:200,0:200])
+        plt.subplot(223)
+        plt.imshow(I_coh[0:200,0:200])
+        plt.subplot(224)
+        plt.imshow(I_blur[0:200,0:200])
+        plt.show()
+
+        plt.figure(figsize=(15,8))
+        plt.subplot(241)
+        plt.title('top right')
+        plt.imshow(I_ref[0:200,0:200])
+        plt.colorbar()
+        plt.subplot(242)
+        plt.title('top left')
+        plt.imshow(I_ref[0:200,-200:])
+        plt.colorbar()
+        plt.subplot(243)
+        plt.title('bottom right')
+        plt.imshow(I_ref[-200:,0:200])
+        plt.colorbar()
+        plt.subplot(244)
+        plt.title('bottom left')
+        plt.imshow(I_ref[-200:,-200:])
+        plt.colorbar()
+
+        plt.subplot(245)
+        plt.imshow(I_coh[0:200,0:200])
+        plt.title('top right')
+        plt.colorbar()
+        plt.subplot(246)
+        plt.title('top left')
+        plt.imshow(I_coh[0:200,-200:])
+        plt.colorbar()
+        plt.subplot(247)
+        plt.title('bottom right')
+        plt.imshow(I_coh[-200:,0:200])
+        plt.colorbar()
+        plt.subplot(248)
+        plt.title('bottom left')
+        plt.imshow(I_coh[-200:,-200:])
+        plt.colorbar()
+        plt.show()
+
+    return I_blur, I_coh, I_det, I_pattern
+
+
```

### Comparing `aps_common_libraries-1.0.3/aps/common/ml/__init__.py` & `aps_common_libraries-1.0.4/aps/common/measurment/beamline/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/ml/data_structures.py` & `aps_common_libraries-1.0.4/aps/common/ml/data_structures.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/ml/mocks.py` & `aps_common_libraries-1.0.4/aps/common/ml/mocks.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/plot/__init__.py` & `aps_common_libraries-1.0.4/aps/common/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/plot/gui.py` & `aps_common_libraries-1.0.4/aps/common/plot/gui.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/plot/image.py` & `aps_common_libraries-1.0.4/aps/common/plot/image.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/plot/qt_application.py` & `aps_common_libraries-1.0.4/aps/common/plot/qt_application.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/plotter.py` & `aps_common_libraries-1.0.4/aps/common/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,10 +289,10 @@
     if reset: PlotterRegistry.Instance().reset()
 
     if plotter_mode   == PlotterMode.FULL:         PlotterRegistry.Instance().register_plotter(FullPlotter(application_name), application_name, replace)
     elif plotter_mode == PlotterMode.DISPLAY_ONLY: PlotterRegistry.Instance().register_plotter(DisplayOnlyPlotter(application_name), application_name, replace)
     elif plotter_mode == PlotterMode.SAVE_ONLY:    PlotterRegistry.Instance().register_plotter(SaveOnlyPlotter(application_name), application_name, replace)
     elif plotter_mode == PlotterMode.NONE:         PlotterRegistry.Instance().register_plotter(NullPlotter(application_name), application_name, replace)
 
-def get_registered_plotter_instance(application_name=None):
+def get_registered_plotter_instance(application_name=None) -> PlotterFacade:
     return PlotterRegistry.Instance().get_plotter_instance(application_name)
```

### Comparing `aps_common_libraries-1.0.3/aps/common/reflection.py` & `aps_common_libraries-1.0.4/aps/common/reflection.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/registry.py` & `aps_common_libraries-1.0.4/aps/common/registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/scripts/__init__.py` & `aps_common_libraries-1.0.4/aps/common/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/scripts/abstract_command_line_script.py` & `aps_common_libraries-1.0.4/aps/common/scripts/abstract_command_line_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/scripts/generic_process_manager.py` & `aps_common_libraries-1.0.4/aps/common/scripts/generic_process_manager.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/scripts/generic_qt_script.py` & `aps_common_libraries-1.0.4/aps/common/scripts/generic_qt_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/scripts/script_data.py` & `aps_common_libraries-1.0.4/aps/common/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/scripts/script_registry.py` & `aps_common_libraries-1.0.4/aps/common/scripts/script_registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/singleton.py` & `aps_common_libraries-1.0.4/aps/common/singleton.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,38 +44,45 @@
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE         #
 # POSSIBILITY OF SUCH DAMAGE.                                             #
 # ----------------------------------------------------------------------- #
 
 import threading
 
 def synchronized_method(method):
-
     outer_lock = threading.Lock()
     lock_name = "__"+method.__name__+"_lock"+"__"
 
     def sync_method(self, *args, **kws):
         with outer_lock:
             if not hasattr(self, lock_name): setattr(self, lock_name, threading.Lock())
             lock = getattr(self, lock_name)
-            with lock:
-                return method(self, *args, **kws)
+            with lock: return method(self, *args, **kws)
 
     return sync_method
 
+# decorator @Singleton
 class Singleton:
-    def __init__(self, decorated):
-        self.__decorated = decorated
+    def __init__(self, decorated): self.__decorated = decorated
 
     @synchronized_method
     def Instance(self, **args):
-        try:
-            return self.__instance
+        try: return self.__instance
         except AttributeError:
             self.__instance = self.__decorated(**args)
             return self.__instance
 
-    def __call__(self):
-        raise TypeError('Singletons must be accessed through `Instance()`.')
+    def __call__(self): raise TypeError('Singletons must be accessed through `Instance()`.')
+    def __instancecheck__(self, inst): return isinstance(inst, self.__decorated)
 
-    def __instancecheck__(self, inst):
-        return isinstance(inst, self.__decorated)
+# Singleton as Metaclass
+from threading import Lock
 
+class SingletonMeta(type):
+    _instances = {}
+    _lock: Lock = Lock()
+
+    def __call__(cls, *args, **kwargs):
+        with cls._lock:
+            if cls not in cls._instances:
+                instance = super().__call__(*args, **kwargs)
+                cls._instances[cls] = instance
+        return cls._instances[cls]
```

### Comparing `aps_common_libraries-1.0.3/aps/common/traffic_light.py` & `aps_common_libraries-1.0.4/aps/common/traffic_light.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,9 +213,9 @@
 # -----------------------------------------------------
 # Factory Methods
 
 def register_traffic_light_instance(reset=False, application_name=None, **kwargs):
     if reset: __TrafficLightRegistry.Instance().reset(application_name)
     __TrafficLightRegistry.Instance().register_traffic_light(__TrafficLightFile(application_name, **kwargs), application_name)
 
-def get_registered_traffic_light_instance(application_name=None):
+def get_registered_traffic_light_instance(application_name=None) -> TrafficLightFacade:
     return __TrafficLightRegistry.Instance().get_traffic_light_instance(application_name)
```

### Comparing `aps_common_libraries-1.0.3/aps/common/utilities.py` & `aps_common_libraries-1.0.4/aps/common/utilities.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/widgets/__init__.py` & `aps_common_libraries-1.0.4/aps/common/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/widgets/close_app_widget.py` & `aps_common_libraries-1.0.4/aps/common/widgets/close_app_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/widgets/context_widget.py` & `aps_common_libraries-1.0.4/aps/common/widgets/context_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/widgets/generic_widget.py` & `aps_common_libraries-1.0.4/aps/common/widgets/generic_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps/common/widgets/log_stream_widget.py` & `aps_common_libraries-1.0.4/aps/common/widgets/log_stream_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.3/aps_common_libraries.egg-info/PKG-INFO` & `aps_common_libraries-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 1.2
-Name: aps-common-libraries
-Version: 1.0.3
+Metadata-Version: 2.1
+Name: aps_common_libraries
+Version: 1.0.4
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
+Download-URL: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
-Download-URL: https://github.com/APS-XSD-OPT-Group/Common-Libraries
-Description: # Common-Libraries
-        General Purpose Libraries 
-        
 Keywords: dictionary,glossary,synchrotronsimulation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
+License-File: LICENSE
+
+# Common-Libraries
+General Purpose Libraries
```

### Comparing `aps_common_libraries-1.0.3/aps_common_libraries.egg-info/SOURCES.txt` & `aps_common_libraries-1.0.4/aps_common_libraries.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 LICENSE
 LICENSE.pdf
 MANIFEST.in
 README.md
 setup.py
+__test/__init__.py
+__test/test.py
+__test/test2.py
 aps/__init__.py
 aps/common/__init__.py
 aps/common/initializer.py
 aps/common/logger.py
 aps/common/plotter.py
 aps/common/reflection.py
 aps/common/registry.py
 aps/common/singleton.py
 aps/common/traffic_light.py
 aps/common/utilities.py
 aps/common/__test/__init__.py
+aps/common/__test/singletons.py
 aps/common/__test/test.py
+aps/common/__test/test2.py
 aps/common/io/__init__.py
 aps/common/io/printout.py
+aps/common/io/sys_commands.py
 aps/common/io/tcp_client.py
 aps/common/io/tiff_file.py
 aps/common/measurment/__init__.py
 aps/common/measurment/beamline/__init__.py
 aps/common/measurment/beamline/image_collector.py
 aps/common/measurment/beamline/image_processor.py
 aps/common/measurment/beamline/wf/SPINNet_estimate.py
```

### Comparing `aps_common_libraries-1.0.3/setup.py` & `aps_common_libraries-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'aps_common_libraries'
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 ISRELEASED = False
 
 DESCRIPTION = 'APS Common Libraries'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
```


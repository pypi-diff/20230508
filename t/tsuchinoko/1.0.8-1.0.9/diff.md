# Comparing `tmp/tsuchinoko-1.0.8.tar.gz` & `tmp/tsuchinoko-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsuchinoko-1.0.8.tar", last modified: Tue Mar 14 18:25:27 2023, max compression
+gzip compressed data, was "tsuchinoko-1.0.9.tar", last modified: Thu Mar 16 18:22:25 2023, max compression
```

## Comparing `tsuchinoko-1.0.8.tar` & `tsuchinoko-1.0.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.839521 tsuchinoko-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 18:25:27.839521 tsuchinoko-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.831521 tsuchinoko-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.831521 tsuchinoko-1.0.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-14 18:25:27.839521 tsuchinoko-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.831521 tsuchinoko-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tests/test_graphics_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tests/test_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.839521 tsuchinoko-1.0.8/tsuchinoko/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 18:25:27.839521 tsuchinoko-1.0.8/tsuchinoko/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.831521 tsuchinoko-1.0.8/tsuchinoko/adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/acquisition_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/quadtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/adaptive/random_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.831521 tsuchinoko-1.0.8/tsuchinoko/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.831521 tsuchinoko-1.0.8/tsuchinoko/core/
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/core/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/IRBL_server_demo_LC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/_launch_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/adaptive_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/client_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/grid_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/headless_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/high_dimensionality_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/ir_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/multi_task_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/quadtree_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/server_demo_bluesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/examples/vector_metric_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/execution/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/execution/bluesky_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/execution/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/execution/threaded_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/graphics_items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/graphics_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/graphics_items/clouditem.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/graphics_items/indicatoritem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/graphics_items/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/graphs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/plan_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/plan_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/utils/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/utils/mutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/utils/runengine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/utils/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.835521 tsuchinoko-1.0.8/tsuchinoko/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/widgets/debugmenubar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/widgets/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/widgets/graph_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/tsuchinoko/widgets/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:27.831521 tsuchinoko-1.0.8/tsuchinoko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 18:25:27.000000 tsuchinoko-1.0.8/tsuchinoko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-14 18:25:27.000000 tsuchinoko-1.0.8/tsuchinoko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:25:27.000000 tsuchinoko-1.0.8/tsuchinoko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-14 18:25:27.000000 tsuchinoko-1.0.8/tsuchinoko.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-14 18:25:27.000000 tsuchinoko-1.0.8/tsuchinoko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-14 18:25:27.000000 tsuchinoko-1.0.8/tsuchinoko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-14 18:25:19.000000 tsuchinoko-1.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tests/test_graphics_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tsuchinoko/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/quadtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/random_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tsuchinoko/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/core/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/IRBL_server_demo_LC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/_launch_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/adaptive_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/client_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/grid_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/headless_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/high_dimensionality_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/ir_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/multi_task_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/quadtree_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/server_demo_bluesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/vector_metric_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/bluesky_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/threaded_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/graphics_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/clouditem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/indicatoritem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/plan_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/mutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/runengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/debugmenubar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/graph_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tsuchinoko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/versioneer.py
```

### Comparing `tsuchinoko-1.0.8/CONTRIBUTING.rst` & `tsuchinoko-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/LICENSE` & `tsuchinoko-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/PKG-INFO` & `tsuchinoko-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsuchinoko
-Version: 1.0.8
+Version: 1.0.9
 Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
 Home-page: https://github.com/lbl-camera/tsuchinoko
 Author: Ronald J Pandolfi
 Author-email: ronpandolfi@lbl.gov
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tsuchinoko-1.0.8/README.md` & `tsuchinoko-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/docs/Makefile` & `tsuchinoko-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/docs/make.bat` & `tsuchinoko-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/docs/source/conf.py` & `tsuchinoko-1.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/legal.txt` & `tsuchinoko-1.0.9/legal.txt`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/setup.py` & `tsuchinoko-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tests/test_core.py` & `tsuchinoko-1.0.9/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tests/test_graphics_items.py` & `tsuchinoko-1.0.9/tests/test_graphics_items.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tests/test_gui.py` & `tsuchinoko-1.0.9/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/__init__.py` & `tsuchinoko-1.0.9/tsuchinoko/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/__init__.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/acquisition_functions.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/acquisition_functions.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/adaptive.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/adaptive.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/gpCAM_in_process.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/gpCAM_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/grid.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/grid.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/quadtree.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/quadtree.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/adaptive/random_in_process.py` & `tsuchinoko-1.0.9/tsuchinoko/adaptive/random_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/core/__init__.py` & `tsuchinoko-1.0.9/tsuchinoko/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/core/messages.py` & `tsuchinoko-1.0.9/tsuchinoko/core/messages.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/IRBL_server_demo_LC.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/IRBL_server_demo_LC.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/adaptive_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/adaptive_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/grid_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/grid_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/headless_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/headless_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/high_dimensionality_server_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/high_dimensionality_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/ir_server_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/ir_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/multi_task_server_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/multi_task_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/quadtree_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/quadtree_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/server_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/server_demo_bluesky.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/server_demo_bluesky.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/examples/vector_metric_demo.py` & `tsuchinoko-1.0.9/tsuchinoko/examples/vector_metric_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/execution/__init__.py` & `tsuchinoko-1.0.9/tsuchinoko/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/execution/bluesky_in_process.py` & `tsuchinoko-1.0.9/tsuchinoko/execution/bluesky_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/execution/simple.py` & `tsuchinoko-1.0.9/tsuchinoko/execution/simple.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/execution/threaded_in_process.py` & `tsuchinoko-1.0.9/tsuchinoko/execution/threaded_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/graphics_items/clouditem.py` & `tsuchinoko-1.0.9/tsuchinoko/graphics_items/clouditem.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/graphics_items/mixins.py` & `tsuchinoko-1.0.9/tsuchinoko/graphics_items/mixins.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/graphs/__init__.py` & `tsuchinoko-1.0.9/tsuchinoko/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/graphs/common.py` & `tsuchinoko-1.0.9/tsuchinoko/graphs/common.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/plan_stubs/__init__.py` & `tsuchinoko-1.0.9/tsuchinoko/plan_stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/utils/__init__.py` & `tsuchinoko-1.0.9/tsuchinoko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/utils/coverage.py` & `tsuchinoko-1.0.9/tsuchinoko/utils/coverage.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/utils/dependencies.py` & `tsuchinoko-1.0.9/tsuchinoko/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/utils/logging.py` & `tsuchinoko-1.0.9/tsuchinoko/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/utils/mutex.py` & `tsuchinoko-1.0.9/tsuchinoko/utils/mutex.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/utils/runengine.py` & `tsuchinoko-1.0.9/tsuchinoko/utils/runengine.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/utils/threads.py` & `tsuchinoko-1.0.9/tsuchinoko/utils/threads.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/widgets/debugmenubar.py` & `tsuchinoko-1.0.9/tsuchinoko/widgets/debugmenubar.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/widgets/displays.py` & `tsuchinoko-1.0.9/tsuchinoko/widgets/displays.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/widgets/graph_widgets.py` & `tsuchinoko-1.0.9/tsuchinoko/widgets/graph_widgets.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/tsuchinoko/widgets/mainwindow.py` & `tsuchinoko-1.0.9/tsuchinoko/widgets/mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,17 @@
             self.socket = None
         if self.context:
             logger.debug('Closing context')
             self.context.term()
             self.context = None
 
     def closeEvent(self, event):
+        if not self.close_demo():
+            event.ignore()
+            return
         if self.data and len(self.data):
             result = QMessageBox.question(self,
                                       'Save data?',
                                       "You have unsaved data in the active experiment. Do you want to save the data?",
                                       buttons=QMessageBox.StandardButtons(QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel),
                                       defaultButton=QMessageBox.Yes)
             if result == QMessageBox.Yes:
@@ -357,35 +360,42 @@
                 self.close_zmq()
             else:
                 event.ignore()
         else:
             event.accept()
             self.close_zmq()
 
+
     def start_demo(self, demo_key):
         # If not communicating with localhost, dump connection to server
         if self.core_address != 'localhost':
             self.core_address = 'localhost'
             self.init_socket()
 
         # if there's a child process server, exit it
+        if not self.close_demo():
+            return
+
+        suffix = Path(sys.executable).suffix 
+        demo_exe = (Path(sys.executable).parent/'tsuchinoko_demo').with_suffix(suffix if suffix=='.exe' else '')
+        print(demo_exe)
+        self._server = subprocess.Popen([demo_exe, demo_key])
+
+    def close_demo(self):
         if self._server:
             self.message_queue.put(ExitRequest())
             try:
                 self._server.wait(3)
 
             except subprocess.TimeoutExpired:
                 result = QMessageBox.question(self,
                                               'Server not responding.',
                                               "The currently running demo server is not responding. Would you like to terminate it?",
                                               buttons=QMessageBox.StandardButtons(
                                                   QMessageBox.Yes | QMessageBox.Cancel),
                                               defaultButton=QMessageBox.Yes)
                 if result == QMessageBox.Yes:
                     self._server.kill()
-                if result == QMessageBox.Cancel:
-                    return
-
-        suffix = Path(sys.executable).suffix 
-        demo_exe = (Path(sys.executable).parent/'tsuchinoko_demo').with_suffix(suffix if suffix=='.exe' else '')
-        print(demo_exe)
-        self._server = subprocess.Popen([demo_exe, demo_key])
+                    return True
+                elif result == QMessageBox.Cancel:
+                    return False
+        return True
```

### Comparing `tsuchinoko-1.0.8/tsuchinoko.egg-info/PKG-INFO` & `tsuchinoko-1.0.9/tsuchinoko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsuchinoko
-Version: 1.0.8
+Version: 1.0.9
 Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
 Home-page: https://github.com/lbl-camera/tsuchinoko
 Author: Ronald J Pandolfi
 Author-email: ronpandolfi@lbl.gov
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tsuchinoko-1.0.8/tsuchinoko.egg-info/SOURCES.txt` & `tsuchinoko-1.0.9/tsuchinoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.8/versioneer.py` & `tsuchinoko-1.0.9/versioneer.py`

 * *Files identical despite different names*


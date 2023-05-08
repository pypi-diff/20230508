# Comparing `tmp/stactools-0.4.6.tar.gz` & `tmp/stactools-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-0.4.6.tar", last modified: Mon Apr 10 17:23:34 2023, max compression
+gzip compressed data, was "stactools-0.4.7.tar", last modified: Mon May  8 19:54:46 2023, max compression
```

## Comparing `stactools-0.4.6.tar` & `stactools-0.4.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.012019 stactools-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-10 17:23:16.000000 stactools-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-04-10 17:23:34.012019 stactools-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-10 17:23:16.000000 stactools-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-10 17:23:16.000000 stactools-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-10 17:23:34.012019 stactools-0.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:33.992018 stactools-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:33.992018 stactools-0.4.6/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.000018 stactools-0.4.6/src/stactools/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.004018 stactools-0.4.6/src/stactools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/update_extent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/update_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.008019 stactools-0.4.6/src/stactools/core/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.008019 stactools-0.4.6/src/stactools/core/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.012019 stactools-0.4.6/src/stactools/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/antimeridian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    40595 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/raster_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/round.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.012019 stactools-0.4.6/src/stactools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:33.996018 stactools-0.4.6/src/stactools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-08 19:54:24.000000 stactools-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-08 19:54:46.140977 stactools-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-08 19:54:24.000000 stactools-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 19:54:24.000000 stactools-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-08 19:54:46.140977 stactools-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.128977 stactools-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.132977 stactools-0.4.7/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.132977 stactools-0.4.7/src/stactools/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.136977 stactools-0.4.7/src/stactools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/update_extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/update_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/antimeridian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40595 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/raster_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.132977 stactools-0.4.7/src/stactools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:54:45.000000 stactools-0.4.7/src/stactools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/top_level.txt
```

### Comparing `stactools-0.4.6/LICENSE` & `stactools-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/PKG-INFO` & `stactools-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.6
+Version: 0.4.7
 Summary: Command line tool and Python library for working with STAC
 Home-page: https://github.com/stac-utils/stactools
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stac-utils/stactools/issues
 Keywords: stactools,pystac,imagery,raster,catalog,STAC
```

### Comparing `stactools-0.4.6/README.md` & `stactools-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/setup.cfg` & `stactools-0.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/__init__.py` & `stactools-0.4.7/src/stactools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/cli.py` & `stactools-0.4.7/src/stactools/cli/cli.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/add.py` & `stactools-0.4.7/src/stactools/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/add_asset.py` & `stactools-0.4.7/src/stactools/cli/commands/add_asset.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/add_raster.py` & `stactools-0.4.7/src/stactools/cli/commands/add_raster.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/copy.py` & `stactools-0.4.7/src/stactools/cli/commands/copy.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/create.py` & `stactools-0.4.7/src/stactools/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/info.py` & `stactools-0.4.7/src/stactools/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/layout.py` & `stactools-0.4.7/src/stactools/cli/commands/layout.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/lint.py` & `stactools-0.4.7/src/stactools/cli/commands/lint.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/merge.py` & `stactools-0.4.7/src/stactools/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/summary.py` & `stactools-0.4.7/src/stactools/cli/commands/summary.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/update_extent.py` & `stactools-0.4.7/src/stactools/cli/commands/update_extent.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/update_geometry.py` & `stactools-0.4.7/src/stactools/cli/commands/update_geometry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/validate.py` & `stactools-0.4.7/src/stactools/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/commands/version.py` & `stactools-0.4.7/src/stactools/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/cli/registry.py` & `stactools-0.4.7/src/stactools/cli/registry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/__init__.py` & `stactools-0.4.7/src/stactools/core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "merge_all_items",
     "merge_items",
     "move_asset_file_to_item",
     "move_assets",
     "move_all_assets",
     "use_fsspec",
 ]
-__version__ = "0.4.6"
+__version__ = "0.4.7"
```

### Comparing `stactools-0.4.6/src/stactools/core/add.py` & `stactools-0.4.7/src/stactools/core/add.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/add_asset.py` & `stactools-0.4.7/src/stactools/core/add_asset.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/add_raster.py` & `stactools-0.4.7/src/stactools/core/add_raster.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/copy.py` & `stactools-0.4.7/src/stactools/core/copy.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/create.py` & `stactools-0.4.7/src/stactools/core/create.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/geometry.py` & `stactools-0.4.7/src/stactools/core/geometry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/io/__init__.py` & `stactools-0.4.7/src/stactools/core/io/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/io/xml.py` & `stactools-0.4.7/src/stactools/core/io/xml.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/layout.py` & `stactools-0.4.7/src/stactools/core/layout.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/merge.py` & `stactools-0.4.7/src/stactools/core/merge.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/projection.py` & `stactools-0.4.7/src/stactools/core/projection.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         coords = list(coords)
         for i in range(0, len(coords)):
             coord = coords[i]
             if isinstance(coord[0], Sequence):
                 coords[i] = fn(coord)
             else:
                 x, y = coord
-                reprojected_coords = list(transformer.transform(x, y))
+                reprojected_coords = list(transformer.transform(x, y, errcheck=True))
                 if precision is not None:
                     reprojected_coords = [
                         round(n, precision) for n in reprojected_coords
                     ]
                 coords[i] = reprojected_coords
         return coords
```

### Comparing `stactools-0.4.6/src/stactools/core/utils/__init__.py` & `stactools-0.4.7/src/stactools/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/utils/antimeridian.py` & `stactools-0.4.7/src/stactools/core/utils/antimeridian.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/utils/convert.py` & `stactools-0.4.7/src/stactools/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/utils/raster_footprint.py` & `stactools-0.4.7/src/stactools/core/utils/raster_footprint.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/utils/round.py` & `stactools-0.4.7/src/stactools/core/utils/round.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/core/utils/subprocess.py` & `stactools-0.4.7/src/stactools/core/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/testing/cli.py` & `stactools-0.4.7/src/stactools/testing/cli.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/testing/cli_test.py` & `stactools-0.4.7/src/stactools/testing/cli_test.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools/testing/test_data.py` & `stactools-0.4.7/src/stactools/testing/test_data.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.6/src/stactools.egg-info/PKG-INFO` & `stactools-0.4.7/src/stactools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.6
+Version: 0.4.7
 Summary: Command line tool and Python library for working with STAC
 Home-page: https://github.com/stac-utils/stactools
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stac-utils/stactools/issues
 Keywords: stactools,pystac,imagery,raster,catalog,STAC
```

### Comparing `stactools-0.4.6/src/stactools.egg-info/SOURCES.txt` & `stactools-0.4.7/src/stactools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


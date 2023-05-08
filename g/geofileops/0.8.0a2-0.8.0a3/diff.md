# Comparing `tmp/geofileops-0.8.0a2.tar.gz` & `tmp/geofileops-0.8.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofileops-0.8.0a2.tar", last modified: Tue Apr 25 13:16:40 2023, max compression
+gzip compressed data, was "geofileops-0.8.0a3.tar", last modified: Fri May  5 11:57:59 2023, max compression
```

## Comparing `geofileops-0.8.0a2.tar` & `geofileops-0.8.0a3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.844609 geofileops-0.8.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-25 13:16:40.844609 geofileops-0.8.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.832609 geofileops-0.8.0a2/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/benchmark_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/benchmark_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/benchmarker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.832609 geofileops-0.8.0a2/benchmark/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/benchmarks/benchmarks_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/benchmarks/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/benchmark/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.832609 geofileops-0.8.0a2/geofileops/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    83155 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)    90643 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/geoops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.836609 geofileops-0.8.0a2/geofileops/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/helpers/_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/helpers/layerstyles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.836609 geofileops-0.8.0a2/geofileops/util/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    71319 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_geoops_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)   101634 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/geodataframe_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/geofiletypes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30107 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/util/test.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/geofileops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.836609 geofileops-0.8.0a2/geofileops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-25 13:16:40.000000 geofileops-0.8.0a2/geofileops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-25 13:16:40.000000 geofileops-0.8.0a2/geofileops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:16:40.000000 geofileops-0.8.0a2/geofileops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-25 13:16:40.000000 geofileops-0.8.0a2/geofileops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 13:16:40.000000 geofileops-0.8.0a2/geofileops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 13:16:40.844609 geofileops-0.8.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.840609 geofileops-0.8.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:16:40.844609 geofileops-0.8.0a2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/BEFL-kbl.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/geofileops_testdata.qgz
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/linestring-row-trees.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/linestring-watercourse.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/linestrings_hedges.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/point.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-invalid.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-no-rows.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-overlappingcircles-all.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-overlappingcircles-one.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-overlappingcircles-two+three.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-parcel.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-simplify-onborder-testcase.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-twolayers.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygon-zone.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygonstyle.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/data/polygonstyle.sld
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    39071 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geofile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geofileops_singlelayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38479 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geofileops_singlelayer_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geofileops_singlelayer_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geofileops_singlelayer_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geofileops_twolayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_spatialite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-25 13:16:29.000000 geofileops-0.8.0a2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.354919 geofileops-0.8.0a3/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmark_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmark_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.354919 geofileops-0.8.0a3/benchmark/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarks/benchmarks_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarks/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.358919 geofileops-0.8.0a3/geofileops/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84479 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90643 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/geoops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.358919 geofileops-0.8.0a3/geofileops/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/helpers/_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/helpers/layerstyles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.362919 geofileops-0.8.0a3/geofileops/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71319 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_geoops_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101634 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geodataframe_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geofiletypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30107 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/test.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.358919 geofileops-0.8.0a3/geofileops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.362919 geofileops-0.8.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/BEFL-kbl.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/geofileops_testdata.qgz
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/linestring-row-trees.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/linestring-watercourse.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/linestrings_hedges.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/point.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-invalid.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-no-rows.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-all.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-one.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-two+three.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-parcel.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-simplify-onborder-testcase.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-twolayers.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-zone.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygonstyle.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygonstyle.sld
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38479 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_twolayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_spatialite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_version.py
```

### Comparing `geofileops-0.8.0a2/LICENSE.txt` & `geofileops-0.8.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/PKG-INFO` & `geofileops-0.8.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a2
+Version: 0.8.0a3
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a2/README.md` & `geofileops-0.8.0a3/README.md`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/benchmark/benchmarker.py` & `geofileops-0.8.0a3/benchmark/benchmarker.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/benchmark/benchmarks/benchmarks_geofileops.py` & `geofileops-0.8.0a3/benchmark/benchmarks/benchmarks_geofileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/benchmark/benchmarks/testdata.py` & `geofileops-0.8.0a3/benchmark/benchmarks/testdata.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/benchmark/reporter.py` & `geofileops-0.8.0a3/benchmark/reporter.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/fileops.py` & `geofileops-0.8.0a3/geofileops/fileops.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,4985 +214,5067 @@
 00000d50: 2020 2020 206f 7220 6461 7461 736f 7572       or datasour
 00000d60: 6365 5f6c 6179 6572 2e47 6574 4765 6f6d  ce_layer.GetGeom
 00000d70: 6574 7279 436f 6c75 6d6e 2829 2021 3d20  etryColumn() != 
 00000d80: 2222 0a20 2020 2020 2020 2020 2020 2029  "".            )
 00000d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00000da0: 2020 6c61 7965 7273 2e61 7070 656e 6428    layers.append(
 00000db0: 6461 7461 736f 7572 6365 5f6c 6179 6572  datasource_layer
-00000dc0: 2e47 6574 4e61 6d65 2829 290a 2020 2020  .GetName()).    
-00000dd0: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
-00000de0: 2069 6620 6461 7461 736f 7572 6365 2069   if datasource i
-00000df0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00000e00: 2020 2020 2020 2020 6465 6c20 6461 7461          del data
-00000e10: 736f 7572 6365 0a0a 2020 2020 7265 7475  source..    retu
-00000e20: 726e 206c 6179 6572 730a 0a0a 636c 6173  rn layers...clas
-00000e30: 7320 436f 6c75 6d6e 496e 666f 3a0a 2020  s ColumnInfo:.  
-00000e40: 2020 2222 220a 2020 2020 4120 6461 7461    """.    A data
-00000e50: 206f 626a 6563 7420 636f 6e74 6169 6e69   object containi
-00000e60: 6e67 206d 6574 612d 696e 666f 726d 6174  ng meta-informat
-00000e70: 696f 6e20 6162 6f75 7420 6120 636f 6c75  ion about a colu
-00000e80: 6d6e 2e0a 0a20 2020 2041 7474 7269 6275  mn...    Attribu
-00000e90: 7465 733a 0a20 2020 2020 2020 206e 616d  tes:.        nam
-00000ea0: 6520 2873 7472 293a 2074 6865 206e 616d  e (str): the nam
-00000eb0: 6520 6f66 2074 6865 2063 6f6c 756d 6e2e  e of the column.
-00000ec0: 0a20 2020 2020 2020 2067 6461 6c5f 7479  .        gdal_ty
-00000ed0: 7065 2028 7374 7229 3a20 7468 6520 7479  pe (str): the ty
-00000ee0: 7065 206f 6620 7468 6520 636f 6c75 6d6e  pe of the column
-00000ef0: 2061 6363 6f72 6469 6e67 2074 6f20 6764   according to gd
-00000f00: 616c 2e0a 2020 2020 2020 2020 7769 6474  al..        widt
-00000f10: 6820 2869 6e74 293a 2074 6865 2077 6964  h (int): the wid
-00000f20: 7468 206f 6620 7468 6520 636f 6c75 6d6e  th of the column
-00000f30: 2c20 6966 2073 7065 6369 6669 6564 2e0a  , if specified..
-00000f40: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-00000f50: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00000f60: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00000f70: 206e 616d 653a 2073 7472 2c0a 2020 2020   name: str,.    
-00000f80: 2020 2020 6764 616c 5f74 7970 653a 2073      gdal_type: s
-00000f90: 7472 2c0a 2020 2020 2020 2020 7769 6474  tr,.        widt
-00000fa0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
-00000fb0: 2c0a 2020 2020 2020 2020 7072 6563 6973  ,.        precis
-00000fc0: 696f 6e3a 204f 7074 696f 6e61 6c5b 696e  ion: Optional[in
-00000fd0: 745d 2c0a 2020 2020 293a 0a20 2020 2020  t],.    ):.     
-00000fe0: 2020 2073 656c 662e 6e61 6d65 203d 206e     self.name = n
-00000ff0: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
-00001000: 2e67 6461 6c5f 7479 7065 203d 2067 6461  .gdal_type = gda
-00001010: 6c5f 7479 7065 0a20 2020 2020 2020 2073  l_type.        s
-00001020: 656c 662e 7769 6474 6820 3d20 7769 6474  elf.width = widt
-00001030: 680a 2020 2020 2020 2020 7365 6c66 2e70  h.        self.p
-00001040: 7265 6369 7369 6f6e 203d 2070 7265 6369  recision = preci
-00001050: 7369 6f6e 0a0a 2020 2020 6465 6620 5f5f  sion..    def __
-00001060: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
-00001070: 2020 2020 2020 7265 7475 726e 2066 227b        return f"{
-00001080: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 7d28  self.__class__}(
-00001090: 7b73 656c 662e 5f5f 6469 6374 5f5f 7d29  {self.__dict__})
-000010a0: 220a 0a0a 636c 6173 7320 4c61 7965 7249  "...class LayerI
-000010b0: 6e66 6f3a 0a20 2020 2022 2222 0a20 2020  nfo:.    """.   
-000010c0: 2041 2064 6174 6120 6f62 6a65 6374 2063   A data object c
-000010d0: 6f6e 7461 696e 696e 6720 6d65 7461 2d69  ontaining meta-i
-000010e0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-000010f0: 2061 206c 6179 6572 2e0a 0a20 2020 2041   a layer...    A
-00001100: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-00001110: 2020 206e 616d 6520 2873 7472 293a 2074     name (str): t
-00001120: 6865 206e 616d 6520 6f66 2074 6865 206c  he name of the l
-00001130: 6179 6572 2e0a 2020 2020 2020 2020 6665  ayer..        fe
-00001140: 6174 7572 6563 6f75 6e74 2028 696e 7429  aturecount (int)
-00001150: 3a20 7468 6520 6e75 6d62 6572 206f 6620  : the number of 
-00001160: 6665 6174 7572 6573 2028 726f 7773 2920  features (rows) 
-00001170: 696e 2074 6865 206c 6179 6572 2e0a 2020  in the layer..  
-00001180: 2020 2020 2020 746f 7461 6c5f 626f 756e        total_boun
-00001190: 6473 2028 5475 706c 655b 666c 6f61 742c  ds (Tuple[float,
-000011a0: 2066 6c6f 6174 2c20 666c 6f61 742c 2066   float, float, f
-000011b0: 6c6f 6174 5d29 3a20 7468 6520 626f 756e  loat]): the boun
-000011c0: 6469 6e67 2062 6f78 206f 660a 2020 2020  ding box of.    
-000011d0: 2020 2020 2020 2020 7468 6520 6c61 7965          the laye
-000011e0: 722e 0a20 2020 2020 2020 2067 656f 6d65  r..        geome
-000011f0: 7472 7963 6f6c 756d 6e20 2873 7472 293a  trycolumn (str):
-00001200: 206e 616d 6520 6f66 2074 6865 2063 6f6c   name of the col
-00001210: 756d 6e20 7468 6174 2063 6f6e 7461 696e  umn that contain
-00001220: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-00001230: 2020 7072 696d 6172 7920 6765 6f6d 6574    primary geomet
-00001240: 7279 2e0a 2020 2020 2020 2020 6765 6f6d  ry..        geom
-00001250: 6574 7279 7479 7065 6e61 6d65 2028 7374  etrytypename (st
-00001260: 7229 3a20 7468 6520 6765 6f6d 6574 7279  r): the geometry
-00001270: 2074 7970 6520 6e61 6d65 206f 6620 7468   type name of th
-00001280: 6520 6765 6f6d 6574 7279 636f 6c75 6d6e  e geometrycolumn
-00001290: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-000012a0: 6520 7479 7065 206e 616d 6520 7265 7475  e type name retu
-000012b0: 726e 6564 2069 7320 6f6e 6520 6f66 2074  rned is one of t
-000012c0: 6865 2066 6f6c 6c6f 7769 6e67 3a20 504f  he following: PO
-000012d0: 494e 542c 204d 554c 5449 504f 494e 542c  INT, MULTIPOINT,
-000012e0: 0a20 2020 2020 2020 2020 2020 204c 494e  .            LIN
-000012f0: 4553 5452 494e 472c 204d 554c 5449 4c49  ESTRING, MULTILI
-00001300: 4e45 5354 5249 4e47 2c20 504f 4c59 474f  NESTRING, POLYGO
-00001310: 4e2c 204d 554c 5449 504f 4c59 474f 4e2c  N, MULTIPOLYGON,
-00001320: 2043 4f4c 4c45 4354 494f 4e2e 0a20 2020   COLLECTION..   
-00001330: 2020 2020 2067 656f 6d65 7472 7974 7970       geometrytyp
-00001340: 6520 2847 656f 6d65 7472 7954 7970 6529  e (GeometryType)
-00001350: 3a20 7468 6520 6765 6f6d 6574 7279 2074  : the geometry t
-00001360: 7970 6520 6f66 2074 6865 2067 656f 6d65  ype of the geome
-00001370: 7472 7963 6f6c 756d 6e2e 0a20 2020 2020  trycolumn..     
-00001380: 2020 2063 6f6c 756d 6e73 2028 6469 6374     columns (dict
-00001390: 293a 2074 6865 2063 6f6c 756d 6e73 2028  ): the columns (
-000013a0: 6f74 6865 7220 7468 616e 2074 6865 2067  other than the g
-000013b0: 656f 6d65 7472 7920 636f 6c75 6d6e 2920  eometry column) 
-000013c0: 7468 6174 0a20 2020 2020 2020 2020 2020  that.           
-000013d0: 2061 7265 2061 7661 696c 6162 6c65 206f   are available o
-000013e0: 6e20 7468 6520 6c61 7965 7220 7769 7468  n the layer with
-000013f0: 2074 6865 6972 2070 726f 7065 7274 6965   their propertie
-00001400: 7320 6173 2061 2064 6963 742e 0a20 2020  s as a dict..   
-00001410: 2020 2020 2066 6964 5f63 6f6c 756d 6e20       fid_column 
-00001420: 2873 7472 293a 2063 6f6c 756d 6e20 6e61  (str): column na
-00001430: 6d65 206f 6620 7468 6520 4649 4420 636f  me of the FID co
-00001440: 6c75 6d6e 2e20 4973 2022 2220 666f 7220  lumn. Is "" for 
-00001450: 6669 6c65 2074 7970 6573 2074 6861 7420  file types that 
-00001460: 646f 6e27 740a 2020 2020 2020 2020 2020  don't.          
-00001470: 2020 6578 706c 6963 6974 6c79 2073 746f    explicitly sto
-00001480: 7265 2061 6e20 4649 442c 206c 696b 6520  re an FID, like 
-00001490: 7368 6170 6566 696c 652e 0a20 2020 2020  shapefile..     
-000014a0: 2020 2063 7273 2028 7079 7072 6f6a 2e43     crs (pyproj.C
-000014b0: 5253 293a 2074 6865 2073 7061 7469 616c  RS): the spatial
-000014c0: 2072 6566 6572 656e 6365 206f 6620 7468   reference of th
-000014d0: 6520 6c61 7965 722e 0a20 2020 2020 2020  e layer..       
-000014e0: 2065 7272 6f72 7320 284c 6973 745b 7374   errors (List[st
-000014f0: 725d 293a 206c 6973 7420 6f66 2065 7272  r]): list of err
-00001500: 6f72 7320 696e 2074 6865 206c 6179 6572  ors in the layer
-00001510: 2c20 6567 2e20 696e 7661 6c69 6420 636f  , eg. invalid co
-00001520: 6c75 6d6e 0a20 2020 2020 2020 2020 2020  lumn.           
-00001530: 206e 616d 6573 2c2e 2e2e 0a20 2020 2022   names,....    "
-00001540: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-00001550: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00001560: 6c66 2c0a 2020 2020 2020 2020 6e61 6d65  lf,.        name
-00001570: 3a20 7374 722c 0a20 2020 2020 2020 2066  : str,.        f
-00001580: 6561 7475 7265 636f 756e 743a 2069 6e74  eaturecount: int
-00001590: 2c0a 2020 2020 2020 2020 746f 7461 6c5f  ,.        total_
-000015a0: 626f 756e 6473 3a20 5475 706c 655b 666c  bounds: Tuple[fl
-000015b0: 6f61 742c 2066 6c6f 6174 2c20 666c 6f61  oat, float, floa
-000015c0: 742c 2066 6c6f 6174 5d2c 0a20 2020 2020  t, float],.     
-000015d0: 2020 2067 656f 6d65 7472 7963 6f6c 756d     geometrycolum
-000015e0: 6e3a 2073 7472 2c0a 2020 2020 2020 2020  n: str,.        
-000015f0: 6765 6f6d 6574 7279 7479 7065 6e61 6d65  geometrytypename
-00001600: 3a20 7374 722c 0a20 2020 2020 2020 2067  : str,.        g
-00001610: 656f 6d65 7472 7974 7970 653a 2047 656f  eometrytype: Geo
-00001620: 6d65 7472 7954 7970 652c 0a20 2020 2020  metryType,.     
-00001630: 2020 2063 6f6c 756d 6e73 3a20 4469 6374     columns: Dict
-00001640: 5b73 7472 2c20 436f 6c75 6d6e 496e 666f  [str, ColumnInfo
-00001650: 5d2c 0a20 2020 2020 2020 2066 6964 5f63  ],.        fid_c
-00001660: 6f6c 756d 6e3a 2073 7472 2c0a 2020 2020  olumn: str,.    
-00001670: 2020 2020 6372 733a 204f 7074 696f 6e61      crs: Optiona
-00001680: 6c5b 7079 7072 6f6a 2e43 5253 5d2c 0a20  l[pyproj.CRS],. 
-00001690: 2020 2020 2020 2065 7272 6f72 733a 204c         errors: L
-000016a0: 6973 745b 7374 725d 2c0a 2020 2020 293a  ist[str],.    ):
-000016b0: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
-000016c0: 6d65 203d 206e 616d 650a 2020 2020 2020  me = name.      
-000016d0: 2020 7365 6c66 2e66 6561 7475 7265 636f    self.featureco
-000016e0: 756e 7420 3d20 6665 6174 7572 6563 6f75  unt = featurecou
-000016f0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
-00001700: 746f 7461 6c5f 626f 756e 6473 203d 2074  total_bounds = t
-00001710: 6f74 616c 5f62 6f75 6e64 730a 2020 2020  otal_bounds.    
-00001720: 2020 2020 7365 6c66 2e67 656f 6d65 7472      self.geometr
-00001730: 7963 6f6c 756d 6e20 3d20 6765 6f6d 6574  ycolumn = geomet
-00001740: 7279 636f 6c75 6d6e 0a20 2020 2020 2020  rycolumn.       
-00001750: 2073 656c 662e 6765 6f6d 6574 7279 7479   self.geometryty
-00001760: 7065 6e61 6d65 203d 2067 656f 6d65 7472  pename = geometr
-00001770: 7974 7970 656e 616d 650a 2020 2020 2020  ytypename.      
-00001780: 2020 7365 6c66 2e67 656f 6d65 7472 7974    self.geometryt
-00001790: 7970 6520 3d20 6765 6f6d 6574 7279 7479  ype = geometryty
-000017a0: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-000017b0: 636f 6c75 6d6e 7320 3d20 636f 6c75 6d6e  columns = column
-000017c0: 730a 2020 2020 2020 2020 7365 6c66 2e66  s.        self.f
-000017d0: 6964 5f63 6f6c 756d 6e20 3d20 6669 645f  id_column = fid_
-000017e0: 636f 6c75 6d6e 0a20 2020 2020 2020 2073  column.        s
-000017f0: 656c 662e 6372 7320 3d20 6372 730a 2020  elf.crs = crs.  
-00001800: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-00001810: 7320 3d20 6572 726f 7273 0a0a 2020 2020  s = errors..    
-00001820: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
-00001830: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00001840: 726e 2066 227b 7365 6c66 2e5f 5f63 6c61  rn f"{self.__cla
-00001850: 7373 5f5f 7d28 7b73 656c 662e 5f5f 6469  ss__}({self.__di
-00001860: 6374 5f5f 7d29 220a 0a0a 6465 6620 6765  ct__})"...def ge
-00001870: 745f 6c61 7965 725f 6765 6f6d 6574 7279  t_layer_geometry
-00001880: 7479 7065 7328 0a20 2020 2070 6174 683a  types(.    path:
-00001890: 2055 6e69 6f6e 5b73 7472 2c20 226f 732e   Union[str, "os.
-000018a0: 5061 7468 4c69 6b65 5b41 6e79 5d22 5d2c  PathLike[Any]"],
-000018b0: 206c 6179 6572 3a20 4f70 7469 6f6e 616c   layer: Optional
-000018c0: 5b73 7472 5d20 3d20 4e6f 6e65 0a29 202d  [str] = None.) -
-000018d0: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-000018e0: 2022 2222 0a20 2020 2047 6574 2074 6865   """.    Get the
-000018f0: 2067 656f 6d65 7472 7920 7479 7065 7320   geometry types 
-00001900: 696e 2074 6865 206c 6179 6572 2062 7920  in the layer by 
-00001910: 6578 616d 696e 696e 6720 6561 6368 2067  examining each g
-00001920: 656f 6d65 7472 7920 696e 2074 6865 206c  eometry in the l
-00001930: 6179 6572 2e0a 0a20 2020 2054 6865 2067  ayer...    The g
-00001940: 656e 6572 616c 2067 656f 6d65 7472 7920  eneral geometry 
-00001950: 7479 7065 206f 6620 7468 6520 6c61 7965  type of the laye
-00001960: 7220 6361 6e20 6265 2064 6574 6572 6d69  r can be determi
-00001970: 6e65 6420 7573 696e 670a 2020 2020 3a6d  ned using.    :m
-00001980: 6574 683a 607e 6765 745f 6c61 7965 7269  eth:`~get_layeri
-00001990: 6e66 6f60 2e0a 0a20 2020 2041 7267 733a  nfo`...    Args:
-000019a0: 0a20 2020 2020 2020 2070 6174 6820 2850  .        path (P
-000019b0: 6174 684c 696b 6529 3a20 7061 7468 2074  athLike): path t
-000019c0: 6f20 7468 6520 6669 6c65 2074 6f20 6765  o the file to ge
-000019d0: 7420 696e 666f 2061 626f 7574 0a20 2020  t info about.   
-000019e0: 2020 2020 206c 6179 6572 2028 7374 7229       layer (str)
-000019f0: 3a20 7468 6520 6c61 7965 7220 796f 7520  : the layer you 
-00001a00: 7761 6e74 2069 6e66 6f20 6162 6f75 742e  want info about.
-00001a10: 2044 6f65 736e 2774 206e 6565 6420 746f   Doesn't need to
-00001a20: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
-00001a30: 7370 6563 6966 6965 6420 6966 2074 6865  specified if the
-00001a40: 7265 2069 7320 6f6e 6c79 206f 6e65 206c  re is only one l
-00001a50: 6179 6572 2069 6e20 7468 6520 6765 6f66  ayer in the geof
-00001a60: 696c 652e 0a0a 2020 2020 5265 7475 726e  ile...    Return
-00001a70: 733a 0a20 2020 2020 2020 204c 6973 745b  s:.        List[
-00001a80: 7374 725d 3a20 7468 6520 6765 6f6d 6574  str]: the geomet
-00001a90: 7279 2074 7970 6573 2069 6e20 7468 6520  ry types in the 
-00001aa0: 6c61 7965 722e 0a20 2020 2022 2222 0a20  layer..    """. 
-00001ab0: 2020 2073 716c 5f73 746d 7420 3d20 2222     sql_stmt = ""
-00001ac0: 220a 2020 2020 2020 2020 5345 4c45 4354  ".        SELECT
-00001ad0: 2044 4953 5449 4e43 540a 2020 2020 2020   DISTINCT.      
-00001ae0: 2020 2020 2020 2020 2043 4153 450a 2020           CASE.  
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2057                 W
-00001b00: 4845 4e20 4361 7374 546f 5369 6e67 6c65  HEN CastToSingle
-00001b10: 287b 6765 6f6d 6574 7279 636f 6c75 6d6e  ({geometrycolumn
-00001b20: 7d29 2049 5320 4e4f 5420 4e55 4c4c 2054  }) IS NOT NULL T
-00001b30: 4845 4e0a 2020 2020 2020 2020 2020 2020  HEN.            
-00001b40: 2020 2020 2020 2020 2053 545f 4765 6f6d           ST_Geom
-00001b50: 6574 7279 5479 7065 2843 6173 7454 6f53  etryType(CastToS
-00001b60: 696e 676c 6528 7b67 656f 6d65 7472 7963  ingle({geometryc
-00001b70: 6f6c 756d 6e7d 2929 0a20 2020 2020 2020  olumn})).       
-00001b80: 2020 2020 2020 2020 2020 454c 5345 2053            ELSE S
-00001b90: 545f 4765 6f6d 6574 7279 5479 7065 287b  T_GeometryType({
-00001ba0: 6765 6f6d 6574 7279 636f 6c75 6d6e 7d29  geometrycolumn})
-00001bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001bc0: 454e 4420 4153 2067 656f 6d5f 7479 7065  END AS geom_type
-00001bd0: 0a20 2020 2020 2020 2020 2046 524f 4d20  .          FROM 
-00001be0: 227b 696e 7075 745f 6c61 7965 727d 2220  "{input_layer}" 
-00001bf0: 6c61 7965 720a 2020 2020 2222 220a 2020  layer.    """.  
-00001c00: 2020 7265 7375 6c74 5f64 6620 3d20 7265    result_df = re
-00001c10: 6164 5f66 696c 6528 7061 7468 2c20 7371  ad_file(path, sq
-00001c20: 6c5f 7374 6d74 3d73 716c 5f73 746d 742c  l_stmt=sql_stmt,
-00001c30: 2073 716c 5f64 6961 6c65 6374 3d22 5351   sql_dialect="SQ
-00001c40: 4c49 5445 2229 0a20 2020 2072 6574 7572  LITE").    retur
-00001c50: 6e20 7265 7375 6c74 5f64 665b 2267 656f  n result_df["geo
-00001c60: 6d5f 7479 7065 225d 2e74 6f5f 6c69 7374  m_type"].to_list
-00001c70: 2829 2020 2320 7479 7065 3a20 6967 6e6f  ()  # type: igno
-00001c80: 7265 0a0a 0a64 6566 2067 6574 5f6c 6179  re...def get_lay
-00001c90: 6572 696e 666f 280a 2020 2020 7061 7468  erinfo(.    path
-00001ca0: 3a20 556e 696f 6e5b 7374 722c 2022 6f73  : Union[str, "os
-00001cb0: 2e50 6174 684c 696b 655b 416e 795d 225d  .PathLike[Any]"]
-00001cc0: 2c20 6c61 7965 723a 204f 7074 696f 6e61  , layer: Optiona
-00001cd0: 6c5b 7374 725d 203d 204e 6f6e 650a 2920  l[str] = None.) 
-00001ce0: 2d3e 204c 6179 6572 496e 666f 3a0a 2020  -> LayerInfo:.  
-00001cf0: 2020 2222 220a 2020 2020 4765 7420 696e    """.    Get in
-00001d00: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-00001d10: 6120 6c61 7965 7220 696e 2074 6865 2067  a layer in the g
-00001d20: 656f 6669 6c65 2e0a 0a20 2020 2052 6169  eofile...    Rai
-00001d30: 7365 7320 616e 2065 7863 6570 7469 6f6e  ses an exception
-00001d40: 2069 6620 7468 6520 6c61 7965 7220 6465   if the layer de
-00001d50: 6669 6e69 7469 6f6e 2068 6173 2065 7272  finition has err
-00001d60: 6f72 7320 6c69 6b65 2069 6e76 616c 6964  ors like invalid
-00001d70: 2063 6f6c 756d 6e0a 2020 2020 6e61 6d65   column.    name
-00001d80: 732c 2e2e 2e0a 0a20 2020 2041 7267 733a  s,.....    Args:
-00001d90: 0a20 2020 2020 2020 2070 6174 6820 2850  .        path (P
-00001da0: 6174 684c 696b 6529 3a20 7061 7468 2074  athLike): path t
-00001db0: 6f20 7468 6520 6669 6c65 2074 6f20 6765  o the file to ge
-00001dc0: 7420 696e 666f 2061 626f 7574 0a20 2020  t info about.   
-00001dd0: 2020 2020 206c 6179 6572 2028 7374 7229       layer (str)
-00001de0: 3a20 7468 6520 6c61 7965 7220 796f 7520  : the layer you 
-00001df0: 7761 6e74 2069 6e66 6f20 6162 6f75 742e  want info about.
-00001e00: 2044 6f65 736e 2774 206e 6565 6420 746f   Doesn't need to
-00001e10: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
-00001e20: 7370 6563 6966 6965 6420 6966 2074 6865  specified if the
-00001e30: 7265 2069 7320 6f6e 6c79 206f 6e65 206c  re is only one l
-00001e40: 6179 6572 2069 6e20 7468 6520 6765 6f66  ayer in the geof
-00001e50: 696c 652e 0a0a 2020 2020 5265 7475 726e  ile...    Return
-00001e60: 733a 0a20 2020 2020 2020 204c 6179 6572  s:.        Layer
-00001e70: 496e 666f 3a20 7468 6520 696e 666f 726d  Info: the inform
-00001e80: 6174 696f 6e20 6162 6f75 7420 7468 6520  ation about the 
-00001e90: 6c61 7965 722e 0a20 2020 2022 2222 0a20  layer..    """. 
-00001ea0: 2020 2023 2049 6e69 740a 2020 2020 7061     # Init.    pa
-00001eb0: 7468 203d 2050 6174 6828 7061 7468 290a  th = Path(path).
-00001ec0: 2020 2020 6966 206e 6f74 2070 6174 682e      if not path.
-00001ed0: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-00001ee0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00001ef0: 6f72 2866 2269 6e70 7574 5f70 6174 6820  or(f"input_path 
-00001f00: 646f 6573 6e27 7420 6578 6973 743a 207b  doesn't exist: {
-00001f10: 7061 7468 7d22 290a 0a20 2020 2069 6620  path}")..    if 
-00001f20: 6c61 7965 7220 6973 204e 6f6e 653a 0a20  layer is None:. 
-00001f30: 2020 2020 2020 206c 6179 6572 203d 2067         layer = g
-00001f40: 6574 5f6f 6e6c 795f 6c61 7965 7228 7061  et_only_layer(pa
-00001f50: 7468 290a 0a20 2020 2064 6174 6173 6f75  th)..    datasou
-00001f60: 7263 6520 3d20 4e6f 6e65 0a20 2020 2074  rce = None.    t
-00001f70: 7279 3a0a 2020 2020 2020 2020 6461 7461  ry:.        data
-00001f80: 736f 7572 6365 203d 2067 6461 6c2e 4f70  source = gdal.Op
-00001f90: 656e 4578 2873 7472 2870 6174 6829 290a  enEx(str(path)).
-00001fa0: 2020 2020 2020 2020 6461 7461 736f 7572          datasour
-00001fb0: 6365 5f6c 6179 6572 203d 2064 6174 6173  ce_layer = datas
-00001fc0: 6f75 7263 652e 4765 744c 6179 6572 286c  ource.GetLayer(l
-00001fd0: 6179 6572 290a 0a20 2020 2020 2020 2023  ayer)..        #
-00001fe0: 2049 6620 7468 6520 6c61 7965 7220 646f   If the layer do
-00001ff0: 6573 6e27 7420 6578 6973 742c 2072 6574  esn't exist, ret
-00002000: 7572 6e0a 2020 2020 2020 2020 6966 2064  urn.        if d
-00002010: 6174 6173 6f75 7263 655f 6c61 7965 7220  atasource_layer 
-00002020: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00002030: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00002040: 4572 726f 7228 6622 4c61 7965 7220 7b6c  Error(f"Layer {l
-00002050: 6179 6572 7d20 6e6f 7420 666f 756e 6420  ayer} not found 
-00002060: 696e 2066 696c 653a 207b 7061 7468 7d22  in file: {path}"
-00002070: 290a 0a20 2020 2020 2020 2023 2047 6574  )..        # Get
-00002080: 2063 6f6c 756d 6e20 696e 666f 0a20 2020   column info.   
-00002090: 2020 2020 2063 6f6c 756d 6e73 203d 207b       columns = {
-000020a0: 7d0a 2020 2020 2020 2020 6572 726f 7273  }.        errors
-000020b0: 203d 205b 5d0a 2020 2020 2020 2020 6765   = [].        ge
-000020c0: 6f66 696c 6574 7970 6520 3d20 4765 6f66  ofiletype = Geof
-000020d0: 696c 6554 7970 6528 7061 7468 290a 2020  ileType(path).  
-000020e0: 2020 2020 2020 6c61 7965 725f 6465 666e        layer_defn
-000020f0: 203d 2064 6174 6173 6f75 7263 655f 6c61   = datasource_la
-00002100: 7965 722e 4765 744c 6179 6572 4465 666e  yer.GetLayerDefn
-00002110: 2829 0a20 2020 2020 2020 2066 6f72 2069  ().        for i
-00002120: 2069 6e20 7261 6e67 6528 6c61 7965 725f   in range(layer_
-00002130: 6465 666e 2e47 6574 4669 656c 6443 6f75  defn.GetFieldCou
-00002140: 6e74 2829 293a 0a20 2020 2020 2020 2020  nt()):.         
-00002150: 2020 206e 616d 6520 3d20 6c61 7965 725f     name = layer_
-00002160: 6465 666e 2e47 6574 4669 656c 6444 6566  defn.GetFieldDef
-00002170: 6e28 6929 2e47 6574 4e61 6d65 2829 0a20  n(i).GetName(). 
-00002180: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-00002190: 4f3a 2074 6869 6e6b 2077 6865 7468 6572  O: think whether
-000021a0: 2074 6865 2074 7970 6520 6e61 6d65 2073   the type name s
-000021b0: 686f 756c 6420 6265 2063 6f6e 7665 7274  hould be convert
-000021c0: 6564 2074 6f20 6f74 6865 7220 6e61 6d65  ed to other name
-000021d0: 730a 2020 2020 2020 2020 2020 2020 6764  s.            gd
-000021e0: 616c 5f74 7970 6520 3d20 6c61 7965 725f  al_type = layer_
-000021f0: 6465 666e 2e47 6574 4669 656c 6444 6566  defn.GetFieldDef
-00002200: 6e28 6929 2e47 6574 5479 7065 4e61 6d65  n(i).GetTypeName
-00002210: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
-00002220: 6964 7468 203d 206c 6179 6572 5f64 6566  idth = layer_def
-00002230: 6e2e 4765 7446 6965 6c64 4465 666e 2869  n.GetFieldDefn(i
-00002240: 292e 4765 7457 6964 7468 2829 0a20 2020  ).GetWidth().   
-00002250: 2020 2020 2020 2020 2077 6964 7468 203d           width =
-00002260: 2077 6964 7468 2069 6620 7769 6474 6820   width if width 
-00002270: 3e20 3020 656c 7365 204e 6f6e 650a 2020  > 0 else None.  
-00002280: 2020 2020 2020 2020 2020 7072 6563 6973            precis
-00002290: 696f 6e20 3d20 6c61 7965 725f 6465 666e  ion = layer_defn
-000022a0: 2e47 6574 4669 656c 6444 6566 6e28 6929  .GetFieldDefn(i)
-000022b0: 2e47 6574 5072 6563 6973 696f 6e28 290a  .GetPrecision().
-000022c0: 2020 2020 2020 2020 2020 2020 7072 6563              prec
-000022d0: 6973 696f 6e20 3d20 7072 6563 6973 696f  ision = precisio
-000022e0: 6e20 6966 2070 7265 6369 7369 6f6e 203e  n if precision >
-000022f0: 2030 2065 6c73 6520 4e6f 6e65 0a20 2020   0 else None.   
-00002300: 2020 2020 2020 2020 2069 6c6c 6567 616c           illegal
-00002310: 5f63 6f6c 756d 6e5f 6368 6172 7320 3d20  _column_chars = 
-00002320: 5b27 2227 5d0a 2020 2020 2020 2020 2020  ['"'].          
-00002330: 2020 666f 7220 696c 6c65 6761 6c5f 6368    for illegal_ch
-00002340: 6172 2069 6e20 696c 6c65 6761 6c5f 636f  ar in illegal_co
-00002350: 6c75 6d6e 5f63 6861 7273 3a0a 2020 2020  lumn_chars:.    
-00002360: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00002370: 6c6c 6567 616c 5f63 6861 7220 696e 206e  llegal_char in n
-00002380: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-00002390: 2020 2020 2020 2020 2065 7272 6f72 732e           errors.
-000023a0: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 6622 436f 6c75 6d6e 206e 616d 6520 7b6e  f"Column name {n
-000023d0: 616d 657d 2063 6f6e 7461 696e 7320 696c  ame} contains il
-000023e0: 6c65 6761 6c20 6368 6172 3a20 7b69 6c6c  legal char: {ill
-000023f0: 6567 616c 5f63 6861 727d 2022 0a20 2020  egal_char} ".   
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2020 2066 2269 6e20 6669 6c65 207b       f"in file {
-00002420: 7061 7468 7d2c 206c 6179 6572 207b 6c61  path}, layer {la
-00002430: 7965 727d 220a 2020 2020 2020 2020 2020  yer}".          
-00002440: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00002450: 2020 2020 2020 2020 636f 6c75 6d6e 5f69          column_i
-00002460: 6e66 6f20 3d20 436f 6c75 6d6e 496e 666f  nfo = ColumnInfo
-00002470: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00002480: 2020 6e61 6d65 3d6e 616d 652c 2067 6461    name=name, gda
-00002490: 6c5f 7479 7065 3d67 6461 6c5f 7479 7065  l_type=gdal_type
-000024a0: 2c20 7769 6474 683d 7769 6474 682c 2070  , width=width, p
-000024b0: 7265 6369 7369 6f6e 3d70 7265 6369 7369  recision=precisi
-000024c0: 6f6e 0a20 2020 2020 2020 2020 2020 2029  on.            )
-000024d0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-000024e0: 756d 6e73 5b6e 616d 655d 203d 2063 6f6c  umns[name] = col
-000024f0: 756d 6e5f 696e 666f 0a20 2020 2020 2020  umn_info.       
-00002500: 2020 2020 2069 6620 6765 6f66 696c 6574       if geofilet
-00002510: 7970 6520 3d3d 2047 656f 6669 6c65 5479  ype == GeofileTy
-00002520: 7065 2e45 5352 4953 6861 7065 6669 6c65  pe.ESRIShapefile
-00002530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002540: 2020 6966 206e 616d 652e 6361 7365 666f    if name.casefo
-00002550: 6c64 2829 203d 3d20 2267 656f 6d65 7472  ld() == "geometr
-00002560: 7922 3a0a 2020 2020 2020 2020 2020 2020  y":.            
-00002570: 2020 2020 2020 2020 6572 726f 7273 2e61          errors.a
-00002580: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-00002590: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000025a0: 416e 2061 7474 7269 6275 7465 2063 6f6c  An attribute col
-000025b0: 756d 6e20 2767 656f 6d65 7472 7927 2069  umn 'geometry' i
-000025c0: 7320 6e6f 7420 7375 7070 6f72 7465 6420  s not supported 
-000025d0: 696e 2061 2073 6861 7065 6669 6c65 220a  in a shapefile".
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-00002600: 2047 6574 2067 656f 6d65 7472 7920 636f   Get geometry co
-00002610: 6c75 6d6e 2069 6e66 6f2e 2e2e 0a20 2020  lumn info....   
-00002620: 2020 2020 2067 656f 6d65 7472 7974 7970       geometrytyp
-00002630: 656e 616d 6520 3d20 6764 616c 2e6f 6772  ename = gdal.ogr
-00002640: 2e47 656f 6d65 7472 7954 7970 6554 6f4e  .GeometryTypeToN
-00002650: 616d 6528 6461 7461 736f 7572 6365 5f6c  ame(datasource_l
-00002660: 6179 6572 2e47 6574 4765 6f6d 5479 7065  ayer.GetGeomType
-00002670: 2829 290a 2020 2020 2020 2020 6765 6f6d  ()).        geom
-00002680: 6574 7279 7479 7065 6e61 6d65 203d 2067  etrytypename = g
-00002690: 656f 6d65 7472 7974 7970 656e 616d 652e  eometrytypename.
-000026a0: 7265 706c 6163 6528 2220 222c 2022 2229  replace(" ", "")
-000026b0: 2e75 7070 6572 2829 0a0a 2020 2020 2020  .upper()..      
-000026c0: 2020 2320 466f 7220 7368 6170 6520 6669    # For shape fi
-000026d0: 6c65 732c 2074 6865 2064 6966 6665 7265  les, the differe
-000026e0: 6e63 6520 6265 7477 6565 6e20 7468 6520  nce between the 
-000026f0: 274d 554c 5449 2720 7661 7269 616e 7420  'MULTI' variant 
-00002700: 616e 6420 7468 650a 2020 2020 2020 2020  and the.        
-00002710: 2320 7369 6e67 6c65 206f 6e65 2064 6f65  # single one doe
-00002720: 736e 2774 2065 7869 7374 732e 2e2e 2073  sn't exists... s
-00002730: 6f20 616c 7761 7973 2072 6570 6f72 7420  o always report 
-00002740: 4d55 4c54 4920 7661 7269 616e 7420 6279  MULTI variant by
-00002750: 2063 6f6e 7665 6e74 696f 6e2e 0a20 2020   convention..   
-00002760: 2020 2020 2069 6620 4765 6f66 696c 6554       if GeofileT
-00002770: 7970 6528 7061 7468 2920 3d3d 2047 656f  ype(path) == Geo
-00002780: 6669 6c65 5479 7065 2e45 5352 4953 6861  fileType.ESRISha
-00002790: 7065 6669 6c65 3a0a 2020 2020 2020 2020  pefile:.        
-000027a0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-000027b0: 2020 2020 2020 2020 2067 656f 6d65 7472           geometr
-000027c0: 7974 7970 656e 616d 652e 7374 6172 7473  ytypename.starts
-000027d0: 7769 7468 2822 504f 4c59 474f 4e22 290a  with("POLYGON").
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 6f72 2067 656f 6d65 7472 7974 7970 656e  or geometrytypen
-00002800: 616d 652e 7374 6172 7473 7769 7468 2822  ame.startswith("
-00002810: 4c49 4e45 5354 5249 4e47 2229 0a20 2020  LINESTRING").   
-00002820: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-00002830: 6765 6f6d 6574 7279 7479 7065 6e61 6d65  geometrytypename
-00002840: 2e73 7461 7274 7377 6974 6828 2250 4f49  .startswith("POI
-00002850: 4e54 2229 0a20 2020 2020 2020 2020 2020  NT").           
-00002860: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00002870: 2020 2020 6765 6f6d 6574 7279 7479 7065      geometrytype
-00002880: 6e61 6d65 203d 2066 224d 554c 5449 7b67  name = f"MULTI{g
-00002890: 656f 6d65 7472 7974 7970 656e 616d 657d  eometrytypename}
-000028a0: 220a 2020 2020 2020 2020 6966 2067 656f  ".        if geo
-000028b0: 6d65 7472 7974 7970 656e 616d 6520 3d3d  metrytypename ==
-000028c0: 2022 554e 4b4e 4f57 4e28 414e 5929 223a   "UNKNOWN(ANY)":
-000028d0: 0a20 2020 2020 2020 2020 2020 2067 656f  .            geo
-000028e0: 6d65 7472 7974 7970 656e 616d 6520 3d20  metrytypename = 
-000028f0: 2247 454f 4d45 5452 5922 0a0a 2020 2020  "GEOMETRY"..    
-00002900: 2020 2020 2320 4765 6f6d 6574 7279 7479      # Geometryty
-00002910: 7065 0a20 2020 2020 2020 2069 6620 6765  pe.        if ge
-00002920: 6f6d 6574 7279 7479 7065 6e61 6d65 2021  ometrytypename !
-00002930: 3d20 224e 4f4e 4522 3a0a 2020 2020 2020  = "NONE":.      
-00002940: 2020 2020 2020 6765 6f6d 6574 7279 7479        geometryty
-00002950: 7065 203d 2047 656f 6d65 7472 7954 7970  pe = GeometryTyp
-00002960: 655b 6765 6f6d 6574 7279 7479 7065 6e61  e[geometrytypena
-00002970: 6d65 5d0a 2020 2020 2020 2020 656c 7365  me].        else
-00002980: 3a0a 2020 2020 2020 2020 2020 2020 6765  :.            ge
-00002990: 6f6d 6574 7279 7479 7065 203d 204e 6f6e  ometrytype = Non
-000029a0: 650a 0a20 2020 2020 2020 2023 2049 6620  e..        # If 
-000029b0: 7468 6520 6765 6f6d 6574 7279 2074 7970  the geometry typ
-000029c0: 6520 6973 206e 6f74 204e 6f6e 652c 2066  e is not None, f
-000029d0: 696c 6c20 6f75 7420 7468 6520 6578 7472  ill out the extr
-000029e0: 6120 7072 6f70 6572 7469 6573 0a20 2020  a properties.   
-000029f0: 2020 2020 2067 656f 6d65 7472 7963 6f6c       geometrycol
-00002a00: 756d 6e20 3d20 4e6f 6e65 0a20 2020 2020  umn = None.     
-00002a10: 2020 2065 7874 656e 7420 3d20 4e6f 6e65     extent = None
-00002a20: 0a20 2020 2020 2020 2063 7273 203d 204e  .        crs = N
-00002a30: 6f6e 650a 2020 2020 2020 2020 746f 7461  one.        tota
-00002a40: 6c5f 626f 756e 6473 203d 204e 6f6e 650a  l_bounds = None.
-00002a50: 2020 2020 2020 2020 6966 2067 656f 6d65          if geome
-00002a60: 7472 7974 7970 6520 6973 206e 6f74 204e  trytype is not N
-00002a70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002a80: 2023 2047 656f 6d65 7472 7920 636f 6c75   # Geometry colu
-00002a90: 6d6e 206e 616d 650a 2020 2020 2020 2020  mn name.        
-00002aa0: 2020 2020 6765 6f6d 6574 7279 636f 6c75      geometrycolu
-00002ab0: 6d6e 203d 2064 6174 6173 6f75 7263 655f  mn = datasource_
-00002ac0: 6c61 7965 722e 4765 7447 656f 6d65 7472  layer.GetGeometr
-00002ad0: 7943 6f6c 756d 6e28 290a 2020 2020 2020  yColumn().      
-00002ae0: 2020 2020 2020 6966 2067 656f 6d65 7472        if geometr
-00002af0: 7963 6f6c 756d 6e20 3d3d 2022 223a 0a20  ycolumn == "":. 
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00002b10: 656f 6d65 7472 7963 6f6c 756d 6e20 3d20  eometrycolumn = 
-00002b20: 2267 656f 6d65 7472 7922 0a20 2020 2020  "geometry".     
-00002b30: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-00002b40: 2065 7874 656e 7420 2878 6d69 6e2c 2078   extent (xmin, x
-00002b50: 6d61 782c 2079 6d69 6e2c 2079 6d61 7829  max, ymin, ymax)
-00002b60: 2074 6f20 626f 756e 6473 2028 786d 696e   to bounds (xmin
-00002b70: 2c20 796d 696e 2c20 786d 6178 2c20 796d  , ymin, xmax, ym
-00002b80: 6178 290a 2020 2020 2020 2020 2020 2020  ax).            
-00002b90: 6578 7465 6e74 203d 2064 6174 6173 6f75  extent = datasou
-00002ba0: 7263 655f 6c61 7965 722e 4765 7445 7874  rce_layer.GetExt
-00002bb0: 656e 7428 290a 2020 2020 2020 2020 2020  ent().          
-00002bc0: 2020 746f 7461 6c5f 626f 756e 6473 203d    total_bounds =
-00002bd0: 2028 6578 7465 6e74 5b30 5d2c 2065 7874   (extent[0], ext
-00002be0: 656e 745b 325d 2c20 6578 7465 6e74 5b31  ent[2], extent[1
-00002bf0: 5d2c 2065 7874 656e 745b 335d 290a 2020  ], extent[3]).  
-00002c00: 2020 2020 2020 2020 2020 2320 4352 530a            # CRS.
-00002c10: 2020 2020 2020 2020 2020 2020 7370 6174              spat
-00002c20: 6961 6c72 6566 203d 2064 6174 6173 6f75  ialref = datasou
-00002c30: 7263 655f 6c61 7965 722e 4765 7453 7061  rce_layer.GetSpa
-00002c40: 7469 616c 5265 6628 290a 2020 2020 2020  tialRef().      
-00002c50: 2020 2020 2020 6966 2073 7061 7469 616c        if spatial
-00002c60: 7265 6620 6973 206e 6f74 204e 6f6e 653a  ref is not None:
-00002c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c80: 2063 7273 203d 2070 7970 726f 6a2e 4352   crs = pyproj.CR
-00002c90: 5328 7370 6174 6961 6c72 6566 2e45 7870  S(spatialref.Exp
-00002ca0: 6f72 7454 6f57 6b74 2829 290a 0a20 2020  ortToWkt())..   
-00002cb0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-00002cc0: 6620 7370 6174 6961 6c20 7265 6620 6861  f spatial ref ha
-00002cd0: 7320 6e6f 2065 7073 672c 2074 7279 2074  s no epsg, try t
-00002ce0: 6f20 6669 6e64 2063 6f72 7265 7370 6f6e  o find correspon
-00002cf0: 6469 6e67 206f 6e65 0a20 2020 2020 2020  ding one.       
-00002d00: 2020 2020 2020 2020 2063 7273 5f65 7073           crs_eps
-00002d10: 6720 3d20 6372 732e 746f 5f65 7073 6728  g = crs.to_epsg(
-00002d20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002d30: 2020 6966 2063 7273 5f65 7073 6720 6973    if crs_epsg is
-00002d40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00002d50: 2020 2020 2020 2020 2020 2069 6620 6372             if cr
-00002d60: 732e 6e61 6d65 2069 6e20 5b0a 2020 2020  s.name in [.    
-00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2020 2242 656c 6765 2031 3937 3220      "Belge 1972 
-00002d90: 2f20 4265 6c67 6961 6e20 4c61 6d62 6572  / Belgian Lamber
-00002da0: 7420 3732 222c 0a20 2020 2020 2020 2020  t 72",.         
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002dc0: 4265 6c67 655f 3139 3732 5f42 656c 6769  Belge_1972_Belgi
-00002dd0: 616e 5f4c 616d 6265 7274 5f37 3222 2c0a  an_Lambert_72",.
-00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002df0: 2020 2020 2020 2020 2242 656c 6765 5f4c          "Belge_L
-00002e00: 616d 6265 7274 5f31 3937 3222 2c0a 2020  ambert_1972",.  
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 2020 2020 2020 2242 4437 3220 2f20 4265        "BD72 / Be
-00002e30: 6c67 6961 6e20 4c61 6d62 6572 7420 3732  lgian Lambert 72
-00002e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002e50: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
-00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e70: 2020 2320 4265 6c67 6961 6e20 4c61 6d62    # Belgian Lamb
-00002e80: 6572 7420 696e 206e 616d 652c 2073 6f20  ert in name, so 
-00002e90: 6173 7375 6d65 2033 3133 3730 0a20 2020  assume 31370.   
+00000dc0: 2e47 6574 4e61 6d65 2829 290a 0a20 2020  .GetName())..   
+00000dd0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00000de0: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
+00000df0: 2065 782e 6172 6773 203d 2028 6622 6c69   ex.args = (f"li
+00000e00: 7374 6c61 7965 7273 2065 7272 6f72 2066  stlayers error f
+00000e10: 6f72 207b 7061 7468 7d3a 5c6e 2020 7b65  or {path}:\n  {e
+00000e20: 787d 222c 290a 2020 2020 2020 2020 7261  x}",).        ra
+00000e30: 6973 650a 2020 2020 6669 6e61 6c6c 793a  ise.    finally:
+00000e40: 0a20 2020 2020 2020 2064 6174 6173 6f75  .        datasou
+00000e50: 7263 6520 3d20 4e6f 6e65 0a0a 2020 2020  rce = None..    
+00000e60: 7265 7475 726e 206c 6179 6572 730a 0a0a  return layers...
+00000e70: 636c 6173 7320 436f 6c75 6d6e 496e 666f  class ColumnInfo
+00000e80: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
+00000e90: 6461 7461 206f 626a 6563 7420 636f 6e74  data object cont
+00000ea0: 6169 6e69 6e67 206d 6574 612d 696e 666f  aining meta-info
+00000eb0: 726d 6174 696f 6e20 6162 6f75 7420 6120  rmation about a 
+00000ec0: 636f 6c75 6d6e 2e0a 0a20 2020 2041 7474  column...    Att
+00000ed0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+00000ee0: 206e 616d 6520 2873 7472 293a 2074 6865   name (str): the
+00000ef0: 206e 616d 6520 6f66 2074 6865 2063 6f6c   name of the col
+00000f00: 756d 6e2e 0a20 2020 2020 2020 2067 6461  umn..        gda
+00000f10: 6c5f 7479 7065 2028 7374 7229 3a20 7468  l_type (str): th
+00000f20: 6520 7479 7065 206f 6620 7468 6520 636f  e type of the co
+00000f30: 6c75 6d6e 2061 6363 6f72 6469 6e67 2074  lumn according t
+00000f40: 6f20 6764 616c 2e0a 2020 2020 2020 2020  o gdal..        
+00000f50: 7769 6474 6820 2869 6e74 293a 2074 6865  width (int): the
+00000f60: 2077 6964 7468 206f 6620 7468 6520 636f   width of the co
+00000f70: 6c75 6d6e 2c20 6966 2073 7065 6369 6669  lumn, if specifi
+00000f80: 6564 2e0a 2020 2020 2222 220a 0a20 2020  ed..    """..   
+00000f90: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00000fa0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00000fb0: 2020 2020 206e 616d 653a 2073 7472 2c0a       name: str,.
+00000fc0: 2020 2020 2020 2020 6764 616c 5f74 7970          gdal_typ
+00000fd0: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00000fe0: 7769 6474 683a 204f 7074 696f 6e61 6c5b  width: Optional[
+00000ff0: 696e 745d 2c0a 2020 2020 2020 2020 7072  int],.        pr
+00001000: 6563 6973 696f 6e3a 204f 7074 696f 6e61  ecision: Optiona
+00001010: 6c5b 696e 745d 2c0a 2020 2020 293a 0a20  l[int],.    ):. 
+00001020: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
+00001030: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
+00001040: 7365 6c66 2e67 6461 6c5f 7479 7065 203d  self.gdal_type =
+00001050: 2067 6461 6c5f 7479 7065 0a20 2020 2020   gdal_type.     
+00001060: 2020 2073 656c 662e 7769 6474 6820 3d20     self.width = 
+00001070: 7769 6474 680a 2020 2020 2020 2020 7365  width.        se
+00001080: 6c66 2e70 7265 6369 7369 6f6e 203d 2070  lf.precision = p
+00001090: 7265 6369 7369 6f6e 0a0a 2020 2020 6465  recision..    de
+000010a0: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
+000010b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000010c0: 2066 227b 7365 6c66 2e5f 5f63 6c61 7373   f"{self.__class
+000010d0: 5f5f 7d28 7b73 656c 662e 5f5f 6469 6374  __}({self.__dict
+000010e0: 5f5f 7d29 220a 0a0a 636c 6173 7320 4c61  __})"...class La
+000010f0: 7965 7249 6e66 6f3a 0a20 2020 2022 2222  yerInfo:.    """
+00001100: 0a20 2020 2041 2064 6174 6120 6f62 6a65  .    A data obje
+00001110: 6374 2063 6f6e 7461 696e 696e 6720 6d65  ct containing me
+00001120: 7461 2d69 6e66 6f72 6d61 7469 6f6e 2061  ta-information a
+00001130: 626f 7574 2061 206c 6179 6572 2e0a 0a20  bout a layer... 
+00001140: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+00001150: 2020 2020 2020 206e 616d 6520 2873 7472         name (str
+00001160: 293a 2074 6865 206e 616d 6520 6f66 2074  ): the name of t
+00001170: 6865 206c 6179 6572 2e0a 2020 2020 2020  he layer..      
+00001180: 2020 6665 6174 7572 6563 6f75 6e74 2028    featurecount (
+00001190: 696e 7429 3a20 7468 6520 6e75 6d62 6572  int): the number
+000011a0: 206f 6620 6665 6174 7572 6573 2028 726f   of features (ro
+000011b0: 7773 2920 696e 2074 6865 206c 6179 6572  ws) in the layer
+000011c0: 2e0a 2020 2020 2020 2020 746f 7461 6c5f  ..        total_
+000011d0: 626f 756e 6473 2028 5475 706c 655b 666c  bounds (Tuple[fl
+000011e0: 6f61 742c 2066 6c6f 6174 2c20 666c 6f61  oat, float, floa
+000011f0: 742c 2066 6c6f 6174 5d29 3a20 7468 6520  t, float]): the 
+00001200: 626f 756e 6469 6e67 2062 6f78 206f 660a  bounding box of.
+00001210: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00001220: 6c61 7965 722e 0a20 2020 2020 2020 2067  layer..        g
+00001230: 656f 6d65 7472 7963 6f6c 756d 6e20 2873  eometrycolumn (s
+00001240: 7472 293a 206e 616d 6520 6f66 2074 6865  tr): name of the
+00001250: 2063 6f6c 756d 6e20 7468 6174 2063 6f6e   column that con
+00001260: 7461 696e 7320 7468 650a 2020 2020 2020  tains the.      
+00001270: 2020 2020 2020 7072 696d 6172 7920 6765        primary ge
+00001280: 6f6d 6574 7279 2e0a 2020 2020 2020 2020  ometry..        
+00001290: 6765 6f6d 6574 7279 7479 7065 6e61 6d65  geometrytypename
+000012a0: 2028 7374 7229 3a20 7468 6520 6765 6f6d   (str): the geom
+000012b0: 6574 7279 2074 7970 6520 6e61 6d65 206f  etry type name o
+000012c0: 6620 7468 6520 6765 6f6d 6574 7279 636f  f the geometryco
+000012d0: 6c75 6d6e 2e0a 2020 2020 2020 2020 2020  lumn..          
+000012e0: 2020 5468 6520 7479 7065 206e 616d 6520    The type name 
+000012f0: 7265 7475 726e 6564 2069 7320 6f6e 6520  returned is one 
+00001300: 6f66 2074 6865 2066 6f6c 6c6f 7769 6e67  of the following
+00001310: 3a20 504f 494e 542c 204d 554c 5449 504f  : POINT, MULTIPO
+00001320: 494e 542c 0a20 2020 2020 2020 2020 2020  INT,.           
+00001330: 204c 494e 4553 5452 494e 472c 204d 554c   LINESTRING, MUL
+00001340: 5449 4c49 4e45 5354 5249 4e47 2c20 504f  TILINESTRING, PO
+00001350: 4c59 474f 4e2c 204d 554c 5449 504f 4c59  LYGON, MULTIPOLY
+00001360: 474f 4e2c 2043 4f4c 4c45 4354 494f 4e2e  GON, COLLECTION.
+00001370: 0a20 2020 2020 2020 2067 656f 6d65 7472  .        geometr
+00001380: 7974 7970 6520 2847 656f 6d65 7472 7954  ytype (GeometryT
+00001390: 7970 6529 3a20 7468 6520 6765 6f6d 6574  ype): the geomet
+000013a0: 7279 2074 7970 6520 6f66 2074 6865 2067  ry type of the g
+000013b0: 656f 6d65 7472 7963 6f6c 756d 6e2e 0a20  eometrycolumn.. 
+000013c0: 2020 2020 2020 2063 6f6c 756d 6e73 2028         columns (
+000013d0: 6469 6374 293a 2074 6865 2063 6f6c 756d  dict): the colum
+000013e0: 6e73 2028 6f74 6865 7220 7468 616e 2074  ns (other than t
+000013f0: 6865 2067 656f 6d65 7472 7920 636f 6c75  he geometry colu
+00001400: 6d6e 2920 7468 6174 0a20 2020 2020 2020  mn) that.       
+00001410: 2020 2020 2061 7265 2061 7661 696c 6162       are availab
+00001420: 6c65 206f 6e20 7468 6520 6c61 7965 7220  le on the layer 
+00001430: 7769 7468 2074 6865 6972 2070 726f 7065  with their prope
+00001440: 7274 6965 7320 6173 2061 2064 6963 742e  rties as a dict.
+00001450: 0a20 2020 2020 2020 2066 6964 5f63 6f6c  .        fid_col
+00001460: 756d 6e20 2873 7472 293a 2063 6f6c 756d  umn (str): colum
+00001470: 6e20 6e61 6d65 206f 6620 7468 6520 4649  n name of the FI
+00001480: 4420 636f 6c75 6d6e 2e20 4973 2022 2220  D column. Is "" 
+00001490: 666f 7220 6669 6c65 2074 7970 6573 2074  for file types t
+000014a0: 6861 7420 646f 6e27 740a 2020 2020 2020  hat don't.      
+000014b0: 2020 2020 2020 6578 706c 6963 6974 6c79        explicitly
+000014c0: 2073 746f 7265 2061 6e20 4649 442c 206c   store an FID, l
+000014d0: 696b 6520 7368 6170 6566 696c 652e 0a20  ike shapefile.. 
+000014e0: 2020 2020 2020 2063 7273 2028 7079 7072         crs (pypr
+000014f0: 6f6a 2e43 5253 293a 2074 6865 2073 7061  oj.CRS): the spa
+00001500: 7469 616c 2072 6566 6572 656e 6365 206f  tial reference o
+00001510: 6620 7468 6520 6c61 7965 722e 0a20 2020  f the layer..   
+00001520: 2020 2020 2065 7272 6f72 7320 284c 6973       errors (Lis
+00001530: 745b 7374 725d 293a 206c 6973 7420 6f66  t[str]): list of
+00001540: 2065 7272 6f72 7320 696e 2074 6865 206c   errors in the l
+00001550: 6179 6572 2c20 6567 2e20 696e 7661 6c69  ayer, eg. invali
+00001560: 6420 636f 6c75 6d6e 0a20 2020 2020 2020  d column.       
+00001570: 2020 2020 206e 616d 6573 2c2e 2e2e 0a20       names,.... 
+00001580: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+00001590: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000015a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000015b0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
+000015c0: 2020 2066 6561 7475 7265 636f 756e 743a     featurecount:
+000015d0: 2069 6e74 2c0a 2020 2020 2020 2020 746f   int,.        to
+000015e0: 7461 6c5f 626f 756e 6473 3a20 5475 706c  tal_bounds: Tupl
+000015f0: 655b 666c 6f61 742c 2066 6c6f 6174 2c20  e[float, float, 
+00001600: 666c 6f61 742c 2066 6c6f 6174 5d2c 0a20  float, float],. 
+00001610: 2020 2020 2020 2067 656f 6d65 7472 7963         geometryc
+00001620: 6f6c 756d 6e3a 2073 7472 2c0a 2020 2020  olumn: str,.    
+00001630: 2020 2020 6765 6f6d 6574 7279 7479 7065      geometrytype
+00001640: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
+00001650: 2020 2067 656f 6d65 7472 7974 7970 653a     geometrytype:
+00001660: 2047 656f 6d65 7472 7954 7970 652c 0a20   GeometryType,. 
+00001670: 2020 2020 2020 2063 6f6c 756d 6e73 3a20         columns: 
+00001680: 4469 6374 5b73 7472 2c20 436f 6c75 6d6e  Dict[str, Column
+00001690: 496e 666f 5d2c 0a20 2020 2020 2020 2066  Info],.        f
+000016a0: 6964 5f63 6f6c 756d 6e3a 2073 7472 2c0a  id_column: str,.
+000016b0: 2020 2020 2020 2020 6372 733a 204f 7074          crs: Opt
+000016c0: 696f 6e61 6c5b 7079 7072 6f6a 2e43 5253  ional[pyproj.CRS
+000016d0: 5d2c 0a20 2020 2020 2020 2065 7272 6f72  ],.        error
+000016e0: 733a 204c 6973 745b 7374 725d 2c0a 2020  s: List[str],.  
+000016f0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00001700: 662e 6e61 6d65 203d 206e 616d 650a 2020  f.name = name.  
+00001710: 2020 2020 2020 7365 6c66 2e66 6561 7475        self.featu
+00001720: 7265 636f 756e 7420 3d20 6665 6174 7572  recount = featur
+00001730: 6563 6f75 6e74 0a20 2020 2020 2020 2073  ecount.        s
+00001740: 656c 662e 746f 7461 6c5f 626f 756e 6473  elf.total_bounds
+00001750: 203d 2074 6f74 616c 5f62 6f75 6e64 730a   = total_bounds.
+00001760: 2020 2020 2020 2020 7365 6c66 2e67 656f          self.geo
+00001770: 6d65 7472 7963 6f6c 756d 6e20 3d20 6765  metrycolumn = ge
+00001780: 6f6d 6574 7279 636f 6c75 6d6e 0a20 2020  ometrycolumn.   
+00001790: 2020 2020 2073 656c 662e 6765 6f6d 6574       self.geomet
+000017a0: 7279 7479 7065 6e61 6d65 203d 2067 656f  rytypename = geo
+000017b0: 6d65 7472 7974 7970 656e 616d 650a 2020  metrytypename.  
+000017c0: 2020 2020 2020 7365 6c66 2e67 656f 6d65        self.geome
+000017d0: 7472 7974 7970 6520 3d20 6765 6f6d 6574  trytype = geomet
+000017e0: 7279 7479 7065 0a20 2020 2020 2020 2073  rytype.        s
+000017f0: 656c 662e 636f 6c75 6d6e 7320 3d20 636f  elf.columns = co
+00001800: 6c75 6d6e 730a 2020 2020 2020 2020 7365  lumns.        se
+00001810: 6c66 2e66 6964 5f63 6f6c 756d 6e20 3d20  lf.fid_column = 
+00001820: 6669 645f 636f 6c75 6d6e 0a20 2020 2020  fid_column.     
+00001830: 2020 2073 656c 662e 6372 7320 3d20 6372     self.crs = cr
+00001840: 730a 2020 2020 2020 2020 7365 6c66 2e65  s.        self.e
+00001850: 7272 6f72 7320 3d20 6572 726f 7273 0a0a  rrors = errors..
+00001860: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00001870: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00001880: 7265 7475 726e 2066 227b 7365 6c66 2e5f  return f"{self._
+00001890: 5f63 6c61 7373 5f5f 7d28 7b73 656c 662e  _class__}({self.
+000018a0: 5f5f 6469 6374 5f5f 7d29 220a 0a0a 6465  __dict__})"...de
+000018b0: 6620 6765 745f 6c61 7965 725f 6765 6f6d  f get_layer_geom
+000018c0: 6574 7279 7479 7065 7328 0a20 2020 2070  etrytypes(.    p
+000018d0: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
+000018e0: 226f 732e 5061 7468 4c69 6b65 5b41 6e79  "os.PathLike[Any
+000018f0: 5d22 5d2c 206c 6179 6572 3a20 4f70 7469  ]"], layer: Opti
+00001900: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00001910: 0a29 202d 3e20 4c69 7374 5b73 7472 5d3a  .) -> List[str]:
+00001920: 0a20 2020 2022 2222 0a20 2020 2047 6574  .    """.    Get
+00001930: 2074 6865 2067 656f 6d65 7472 7920 7479   the geometry ty
+00001940: 7065 7320 696e 2074 6865 206c 6179 6572  pes in the layer
+00001950: 2062 7920 6578 616d 696e 696e 6720 6561   by examining ea
+00001960: 6368 2067 656f 6d65 7472 7920 696e 2074  ch geometry in t
+00001970: 6865 206c 6179 6572 2e0a 0a20 2020 2054  he layer...    T
+00001980: 6865 2067 656e 6572 616c 2067 656f 6d65  he general geome
+00001990: 7472 7920 7479 7065 206f 6620 7468 6520  try type of the 
+000019a0: 6c61 7965 7220 6361 6e20 6265 2064 6574  layer can be det
+000019b0: 6572 6d69 6e65 6420 7573 696e 670a 2020  ermined using.  
+000019c0: 2020 3a6d 6574 683a 607e 6765 745f 6c61    :meth:`~get_la
+000019d0: 7965 7269 6e66 6f60 2e0a 0a20 2020 2041  yerinfo`...    A
+000019e0: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+000019f0: 6820 2850 6174 684c 696b 6529 3a20 7061  h (PathLike): pa
+00001a00: 7468 2074 6f20 7468 6520 6669 6c65 2074  th to the file t
+00001a10: 6f20 6765 7420 696e 666f 2061 626f 7574  o get info about
+00001a20: 0a20 2020 2020 2020 206c 6179 6572 2028  .        layer (
+00001a30: 7374 7229 3a20 7468 6520 6c61 7965 7220  str): the layer 
+00001a40: 796f 7520 7761 6e74 2069 6e66 6f20 6162  you want info ab
+00001a50: 6f75 742e 2044 6f65 736e 2774 206e 6565  out. Doesn't nee
+00001a60: 6420 746f 2062 650a 2020 2020 2020 2020  d to be.        
+00001a70: 2020 2020 7370 6563 6966 6965 6420 6966      specified if
+00001a80: 2074 6865 7265 2069 7320 6f6e 6c79 206f   there is only o
+00001a90: 6e65 206c 6179 6572 2069 6e20 7468 6520  ne layer in the 
+00001aa0: 6765 6f66 696c 652e 0a0a 2020 2020 5265  geofile...    Re
+00001ab0: 7475 726e 733a 0a20 2020 2020 2020 204c  turns:.        L
+00001ac0: 6973 745b 7374 725d 3a20 7468 6520 6765  ist[str]: the ge
+00001ad0: 6f6d 6574 7279 2074 7970 6573 2069 6e20  ometry types in 
+00001ae0: 7468 6520 6c61 7965 722e 0a20 2020 2022  the layer..    "
+00001af0: 2222 0a20 2020 2073 716c 5f73 746d 7420  "".    sql_stmt 
+00001b00: 3d20 2222 220a 2020 2020 2020 2020 5345  = """.        SE
+00001b10: 4c45 4354 2044 4953 5449 4e43 540a 2020  LECT DISTINCT.  
+00001b20: 2020 2020 2020 2020 2020 2020 2043 4153               CAS
+00001b30: 450a 2020 2020 2020 2020 2020 2020 2020  E.              
+00001b40: 2020 2057 4845 4e20 4361 7374 546f 5369     WHEN CastToSi
+00001b50: 6e67 6c65 287b 6765 6f6d 6574 7279 636f  ngle({geometryco
+00001b60: 6c75 6d6e 7d29 2049 5320 4e4f 5420 4e55  lumn}) IS NOT NU
+00001b70: 4c4c 2054 4845 4e0a 2020 2020 2020 2020  LL THEN.        
+00001b80: 2020 2020 2020 2020 2020 2020 2053 545f               ST_
+00001b90: 4765 6f6d 6574 7279 5479 7065 2843 6173  GeometryType(Cas
+00001ba0: 7454 6f53 696e 676c 6528 7b67 656f 6d65  tToSingle({geome
+00001bb0: 7472 7963 6f6c 756d 6e7d 2929 0a20 2020  trycolumn})).   
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 454c                EL
+00001bd0: 5345 2053 545f 4765 6f6d 6574 7279 5479  SE ST_GeometryTy
+00001be0: 7065 287b 6765 6f6d 6574 7279 636f 6c75  pe({geometrycolu
+00001bf0: 6d6e 7d29 0a20 2020 2020 2020 2020 2020  mn}).           
+00001c00: 2020 2020 454e 4420 4153 2067 656f 6d5f      END AS geom_
+00001c10: 7479 7065 0a20 2020 2020 2020 2020 2046  type.          F
+00001c20: 524f 4d20 227b 696e 7075 745f 6c61 7965  ROM "{input_laye
+00001c30: 727d 2220 6c61 7965 720a 2020 2020 2222  r}" layer.    ""
+00001c40: 220a 2020 2020 7265 7375 6c74 5f64 6620  ".    result_df 
+00001c50: 3d20 7265 6164 5f66 696c 6528 7061 7468  = read_file(path
+00001c60: 2c20 7371 6c5f 7374 6d74 3d73 716c 5f73  , sql_stmt=sql_s
+00001c70: 746d 742c 2073 716c 5f64 6961 6c65 6374  tmt, sql_dialect
+00001c80: 3d22 5351 4c49 5445 2229 0a20 2020 2072  ="SQLITE").    r
+00001c90: 6574 7572 6e20 7265 7375 6c74 5f64 665b  eturn result_df[
+00001ca0: 2267 656f 6d5f 7479 7065 225d 2e74 6f5f  "geom_type"].to_
+00001cb0: 6c69 7374 2829 2020 2320 7479 7065 3a20  list()  # type: 
+00001cc0: 6967 6e6f 7265 0a0a 0a64 6566 2067 6574  ignore...def get
+00001cd0: 5f6c 6179 6572 696e 666f 280a 2020 2020  _layerinfo(.    
+00001ce0: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
+00001cf0: 2022 6f73 2e50 6174 684c 696b 655b 416e   "os.PathLike[An
+00001d00: 795d 225d 2c20 6c61 7965 723a 204f 7074  y]"], layer: Opt
+00001d10: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00001d20: 650a 2920 2d3e 204c 6179 6572 496e 666f  e.) -> LayerInfo
+00001d30: 3a0a 2020 2020 2222 220a 2020 2020 4765  :.    """.    Ge
+00001d40: 7420 696e 666f 726d 6174 696f 6e20 6162  t information ab
+00001d50: 6f75 7420 6120 6c61 7965 7220 696e 2074  out a layer in t
+00001d60: 6865 2067 656f 6669 6c65 2e0a 0a20 2020  he geofile...   
+00001d70: 2052 6169 7365 7320 616e 2065 7863 6570   Raises an excep
+00001d80: 7469 6f6e 2069 6620 7468 6520 6c61 7965  tion if the laye
+00001d90: 7220 6465 6669 6e69 7469 6f6e 2068 6173  r definition has
+00001da0: 2065 7272 6f72 7320 6c69 6b65 2069 6e76   errors like inv
+00001db0: 616c 6964 2063 6f6c 756d 6e0a 2020 2020  alid column.    
+00001dc0: 6e61 6d65 732c 2e2e 2e0a 0a20 2020 2041  names,.....    A
+00001dd0: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+00001de0: 6820 2850 6174 684c 696b 6529 3a20 7061  h (PathLike): pa
+00001df0: 7468 2074 6f20 7468 6520 6669 6c65 2074  th to the file t
+00001e00: 6f20 6765 7420 696e 666f 2061 626f 7574  o get info about
+00001e10: 0a20 2020 2020 2020 206c 6179 6572 2028  .        layer (
+00001e20: 7374 7229 3a20 7468 6520 6c61 7965 7220  str): the layer 
+00001e30: 796f 7520 7761 6e74 2069 6e66 6f20 6162  you want info ab
+00001e40: 6f75 742e 2044 6f65 736e 2774 206e 6565  out. Doesn't nee
+00001e50: 6420 746f 2062 650a 2020 2020 2020 2020  d to be.        
+00001e60: 2020 2020 7370 6563 6966 6965 6420 6966      specified if
+00001e70: 2074 6865 7265 2069 7320 6f6e 6c79 206f   there is only o
+00001e80: 6e65 206c 6179 6572 2069 6e20 7468 6520  ne layer in the 
+00001e90: 6765 6f66 696c 652e 0a0a 2020 2020 5265  geofile...    Re
+00001ea0: 7475 726e 733a 0a20 2020 2020 2020 204c  turns:.        L
+00001eb0: 6179 6572 496e 666f 3a20 7468 6520 696e  ayerInfo: the in
+00001ec0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00001ed0: 7468 6520 6c61 7965 722e 0a20 2020 2022  the layer..    "
+00001ee0: 2222 0a20 2020 2023 2049 6e69 740a 2020  "".    # Init.  
+00001ef0: 2020 7061 7468 203d 2050 6174 6828 7061    path = Path(pa
+00001f00: 7468 290a 2020 2020 6966 206e 6f74 2070  th).    if not p
+00001f10: 6174 682e 6578 6973 7473 2829 3a0a 2020  ath.exists():.  
+00001f20: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00001f30: 6545 7272 6f72 2866 2269 6e70 7574 5f70  eError(f"input_p
+00001f40: 6174 6820 646f 6573 6e27 7420 6578 6973  ath doesn't exis
+00001f50: 743a 207b 7061 7468 7d22 290a 0a20 2020  t: {path}")..   
+00001f60: 2069 6620 6c61 7965 7220 6973 204e 6f6e   if layer is Non
+00001f70: 653a 0a20 2020 2020 2020 206c 6179 6572  e:.        layer
+00001f80: 203d 2067 6574 5f6f 6e6c 795f 6c61 7965   = get_only_laye
+00001f90: 7228 7061 7468 290a 0a20 2020 2064 6174  r(path)..    dat
+00001fa0: 6173 6f75 7263 6520 3d20 4e6f 6e65 0a20  asource = None. 
+00001fb0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00001fc0: 6461 7461 736f 7572 6365 203d 2067 6461  datasource = gda
+00001fd0: 6c2e 4f70 656e 4578 2873 7472 2870 6174  l.OpenEx(str(pat
+00001fe0: 6829 290a 2020 2020 2020 2020 6461 7461  h)).        data
+00001ff0: 736f 7572 6365 5f6c 6179 6572 203d 2064  source_layer = d
+00002000: 6174 6173 6f75 7263 652e 4765 744c 6179  atasource.GetLay
+00002010: 6572 286c 6179 6572 290a 0a20 2020 2020  er(layer)..     
+00002020: 2020 2023 2049 6620 7468 6520 6c61 7965     # If the laye
+00002030: 7220 646f 6573 6e27 7420 6578 6973 742c  r doesn't exist,
+00002040: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00002050: 6966 2064 6174 6173 6f75 7263 655f 6c61  if datasource_la
+00002060: 7965 7220 6973 204e 6f6e 653a 0a20 2020  yer is None:.   
+00002070: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00002080: 616c 7565 4572 726f 7228 6622 4c61 7965  alueError(f"Laye
+00002090: 7220 7b6c 6179 6572 7d20 6e6f 7420 666f  r {layer} not fo
+000020a0: 756e 6420 696e 2066 696c 653a 207b 7061  und in file: {pa
+000020b0: 7468 7d22 290a 0a20 2020 2020 2020 2023  th}")..        #
+000020c0: 2047 6574 2063 6f6c 756d 6e20 696e 666f   Get column info
+000020d0: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
+000020e0: 203d 207b 7d0a 2020 2020 2020 2020 6572   = {}.        er
+000020f0: 726f 7273 203d 205b 5d0a 2020 2020 2020  rors = [].      
+00002100: 2020 6765 6f66 696c 6574 7970 6520 3d20    geofiletype = 
+00002110: 4765 6f66 696c 6554 7970 6528 7061 7468  GeofileType(path
+00002120: 290a 2020 2020 2020 2020 6c61 7965 725f  ).        layer_
+00002130: 6465 666e 203d 2064 6174 6173 6f75 7263  defn = datasourc
+00002140: 655f 6c61 7965 722e 4765 744c 6179 6572  e_layer.GetLayer
+00002150: 4465 666e 2829 0a20 2020 2020 2020 2066  Defn().        f
+00002160: 6f72 2069 2069 6e20 7261 6e67 6528 6c61  or i in range(la
+00002170: 7965 725f 6465 666e 2e47 6574 4669 656c  yer_defn.GetFiel
+00002180: 6443 6f75 6e74 2829 293a 0a20 2020 2020  dCount()):.     
+00002190: 2020 2020 2020 206e 616d 6520 3d20 6c61         name = la
+000021a0: 7965 725f 6465 666e 2e47 6574 4669 656c  yer_defn.GetFiel
+000021b0: 6444 6566 6e28 6929 2e47 6574 4e61 6d65  dDefn(i).GetName
+000021c0: 2829 0a20 2020 2020 2020 2020 2020 2023  ().            #
+000021d0: 2054 4f44 4f3a 2074 6869 6e6b 2077 6865   TODO: think whe
+000021e0: 7468 6572 2074 6865 2074 7970 6520 6e61  ther the type na
+000021f0: 6d65 2073 686f 756c 6420 6265 2063 6f6e  me should be con
+00002200: 7665 7274 6564 2074 6f20 6f74 6865 7220  verted to other 
+00002210: 6e61 6d65 730a 2020 2020 2020 2020 2020  names.          
+00002220: 2020 6764 616c 5f74 7970 6520 3d20 6c61    gdal_type = la
+00002230: 7965 725f 6465 666e 2e47 6574 4669 656c  yer_defn.GetFiel
+00002240: 6444 6566 6e28 6929 2e47 6574 5479 7065  dDefn(i).GetType
+00002250: 4e61 6d65 2829 0a20 2020 2020 2020 2020  Name().         
+00002260: 2020 2077 6964 7468 203d 206c 6179 6572     width = layer
+00002270: 5f64 6566 6e2e 4765 7446 6965 6c64 4465  _defn.GetFieldDe
+00002280: 666e 2869 292e 4765 7457 6964 7468 2829  fn(i).GetWidth()
+00002290: 0a20 2020 2020 2020 2020 2020 2077 6964  .            wid
+000022a0: 7468 203d 2077 6964 7468 2069 6620 7769  th = width if wi
+000022b0: 6474 6820 3e20 3020 656c 7365 204e 6f6e  dth > 0 else Non
+000022c0: 650a 2020 2020 2020 2020 2020 2020 7072  e.            pr
+000022d0: 6563 6973 696f 6e20 3d20 6c61 7965 725f  ecision = layer_
+000022e0: 6465 666e 2e47 6574 4669 656c 6444 6566  defn.GetFieldDef
+000022f0: 6e28 6929 2e47 6574 5072 6563 6973 696f  n(i).GetPrecisio
+00002300: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
+00002310: 7072 6563 6973 696f 6e20 3d20 7072 6563  precision = prec
+00002320: 6973 696f 6e20 6966 2070 7265 6369 7369  ision if precisi
+00002330: 6f6e 203e 2030 2065 6c73 6520 4e6f 6e65  on > 0 else None
+00002340: 0a20 2020 2020 2020 2020 2020 2069 6c6c  .            ill
+00002350: 6567 616c 5f63 6f6c 756d 6e5f 6368 6172  egal_column_char
+00002360: 7320 3d20 5b27 2227 5d0a 2020 2020 2020  s = ['"'].      
+00002370: 2020 2020 2020 666f 7220 696c 6c65 6761        for illega
+00002380: 6c5f 6368 6172 2069 6e20 696c 6c65 6761  l_char in illega
+00002390: 6c5f 636f 6c75 6d6e 5f63 6861 7273 3a0a  l_column_chars:.
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 6966 2069 6c6c 6567 616c 5f63 6861 7220  if illegal_char 
+000023c0: 696e 206e 616d 653a 0a20 2020 2020 2020  in name:.       
+000023d0: 2020 2020 2020 2020 2020 2020 2065 7272               err
+000023e0: 6f72 732e 6170 7065 6e64 280a 2020 2020  ors.append(.    
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 2020 2020 6622 436f 6c75 6d6e 206e 616d      f"Column nam
+00002410: 6520 7b6e 616d 657d 2063 6f6e 7461 696e  e {name} contain
+00002420: 7320 696c 6c65 6761 6c20 6368 6172 3a20  s illegal char: 
+00002430: 7b69 6c6c 6567 616c 5f63 6861 727d 2022  {illegal_char} "
+00002440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002450: 2020 2020 2020 2020 2066 2269 6e20 6669           f"in fi
+00002460: 6c65 207b 7061 7468 7d2c 206c 6179 6572  le {path}, layer
+00002470: 207b 6c61 7965 727d 220a 2020 2020 2020   {layer}".      
+00002480: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00002490: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+000024a0: 6d6e 5f69 6e66 6f20 3d20 436f 6c75 6d6e  mn_info = Column
+000024b0: 496e 666f 280a 2020 2020 2020 2020 2020  Info(.          
+000024c0: 2020 2020 2020 6e61 6d65 3d6e 616d 652c        name=name,
+000024d0: 2067 6461 6c5f 7479 7065 3d67 6461 6c5f   gdal_type=gdal_
+000024e0: 7479 7065 2c20 7769 6474 683d 7769 6474  type, width=widt
+000024f0: 682c 2070 7265 6369 7369 6f6e 3d70 7265  h, precision=pre
+00002500: 6369 7369 6f6e 0a20 2020 2020 2020 2020  cision.         
+00002510: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00002520: 2063 6f6c 756d 6e73 5b6e 616d 655d 203d   columns[name] =
+00002530: 2063 6f6c 756d 6e5f 696e 666f 0a20 2020   column_info.   
+00002540: 2020 2020 2020 2020 2069 6620 6765 6f66           if geof
+00002550: 696c 6574 7970 6520 3d3d 2047 656f 6669  iletype == Geofi
+00002560: 6c65 5479 7065 2e45 5352 4953 6861 7065  leType.ESRIShape
+00002570: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00002580: 2020 2020 2020 6966 206e 616d 652e 6361        if name.ca
+00002590: 7365 666f 6c64 2829 203d 3d20 2267 656f  sefold() == "geo
+000025a0: 6d65 7472 7922 3a0a 2020 2020 2020 2020  metry":.        
+000025b0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+000025c0: 7273 2e61 7070 656e 6428 0a20 2020 2020  rs.append(.     
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 2020 2022 416e 2061 7474 7269 6275 7465     "An attribute
+000025f0: 2063 6f6c 756d 6e20 2767 656f 6d65 7472   column 'geometr
+00002600: 7927 2069 7320 6e6f 7420 7375 7070 6f72  y' is not suppor
+00002610: 7465 6420 696e 2061 2073 6861 7065 6669  ted in a shapefi
+00002620: 6c65 220a 2020 2020 2020 2020 2020 2020  le".            
+00002630: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00002640: 2020 2023 2047 6574 2067 656f 6d65 7472     # Get geometr
+00002650: 7920 636f 6c75 6d6e 2069 6e66 6f2e 2e2e  y column info...
+00002660: 0a20 2020 2020 2020 2067 656f 6d65 7472  .        geometr
+00002670: 7974 7970 656e 616d 6520 3d20 6764 616c  ytypename = gdal
+00002680: 2e6f 6772 2e47 656f 6d65 7472 7954 7970  .ogr.GeometryTyp
+00002690: 6554 6f4e 616d 6528 6461 7461 736f 7572  eToName(datasour
+000026a0: 6365 5f6c 6179 6572 2e47 6574 4765 6f6d  ce_layer.GetGeom
+000026b0: 5479 7065 2829 290a 2020 2020 2020 2020  Type()).        
+000026c0: 6765 6f6d 6574 7279 7479 7065 6e61 6d65  geometrytypename
+000026d0: 203d 2067 656f 6d65 7472 7974 7970 656e   = geometrytypen
+000026e0: 616d 652e 7265 706c 6163 6528 2220 222c  ame.replace(" ",
+000026f0: 2022 2229 2e75 7070 6572 2829 0a0a 2020   "").upper()..  
+00002700: 2020 2020 2020 2320 466f 7220 7368 6170        # For shap
+00002710: 6520 6669 6c65 732c 2074 6865 2064 6966  e files, the dif
+00002720: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
+00002730: 7468 6520 274d 554c 5449 2720 7661 7269  the 'MULTI' vari
+00002740: 616e 7420 616e 6420 7468 650a 2020 2020  ant and the.    
+00002750: 2020 2020 2320 7369 6e67 6c65 206f 6e65      # single one
+00002760: 2064 6f65 736e 2774 2065 7869 7374 732e   doesn't exists.
+00002770: 2e2e 2073 6f20 616c 7761 7973 2072 6570  .. so always rep
+00002780: 6f72 7420 4d55 4c54 4920 7661 7269 616e  ort MULTI varian
+00002790: 7420 6279 2063 6f6e 7665 6e74 696f 6e2e  t by convention.
+000027a0: 0a20 2020 2020 2020 2069 6620 4765 6f66  .        if Geof
+000027b0: 696c 6554 7970 6528 7061 7468 2920 3d3d  ileType(path) ==
+000027c0: 2047 656f 6669 6c65 5479 7065 2e45 5352   GeofileType.ESR
+000027d0: 4953 6861 7065 6669 6c65 3a0a 2020 2020  IShapefile:.    
+000027e0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+000027f0: 2020 2020 2020 2020 2020 2020 2067 656f               geo
+00002800: 6d65 7472 7974 7970 656e 616d 652e 7374  metrytypename.st
+00002810: 6172 7473 7769 7468 2822 504f 4c59 474f  artswith("POLYGO
+00002820: 4e22 290a 2020 2020 2020 2020 2020 2020  N").            
+00002830: 2020 2020 6f72 2067 656f 6d65 7472 7974      or geometryt
+00002840: 7970 656e 616d 652e 7374 6172 7473 7769  ypename.startswi
+00002850: 7468 2822 4c49 4e45 5354 5249 4e47 2229  th("LINESTRING")
+00002860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002870: 206f 7220 6765 6f6d 6574 7279 7479 7065   or geometrytype
+00002880: 6e61 6d65 2e73 7461 7274 7377 6974 6828  name.startswith(
+00002890: 2250 4f49 4e54 2229 0a20 2020 2020 2020  "POINT").       
+000028a0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+000028b0: 2020 2020 2020 2020 6765 6f6d 6574 7279          geometry
+000028c0: 7479 7065 6e61 6d65 203d 2066 224d 554c  typename = f"MUL
+000028d0: 5449 7b67 656f 6d65 7472 7974 7970 656e  TI{geometrytypen
+000028e0: 616d 657d 220a 2020 2020 2020 2020 6966  ame}".        if
+000028f0: 2067 656f 6d65 7472 7974 7970 656e 616d   geometrytypenam
+00002900: 6520 3d3d 2022 554e 4b4e 4f57 4e28 414e  e == "UNKNOWN(AN
+00002910: 5929 223a 0a20 2020 2020 2020 2020 2020  Y)":.           
+00002920: 2067 656f 6d65 7472 7974 7970 656e 616d   geometrytypenam
+00002930: 6520 3d20 2247 454f 4d45 5452 5922 0a0a  e = "GEOMETRY"..
+00002940: 2020 2020 2020 2020 2320 4765 6f6d 6574          # Geomet
+00002950: 7279 7479 7065 0a20 2020 2020 2020 2069  rytype.        i
+00002960: 6620 6765 6f6d 6574 7279 7479 7065 6e61  f geometrytypena
+00002970: 6d65 2021 3d20 224e 4f4e 4522 3a0a 2020  me != "NONE":.  
+00002980: 2020 2020 2020 2020 2020 6765 6f6d 6574            geomet
+00002990: 7279 7479 7065 203d 2047 656f 6d65 7472  rytype = Geometr
+000029a0: 7954 7970 655b 6765 6f6d 6574 7279 7479  yType[geometryty
+000029b0: 7065 6e61 6d65 5d0a 2020 2020 2020 2020  pename].        
+000029c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000029d0: 2020 6765 6f6d 6574 7279 7479 7065 203d    geometrytype =
+000029e0: 204e 6f6e 650a 0a20 2020 2020 2020 2023   None..        #
+000029f0: 2049 6620 7468 6520 6765 6f6d 6574 7279   If the geometry
+00002a00: 2074 7970 6520 6973 206e 6f74 204e 6f6e   type is not Non
+00002a10: 652c 2066 696c 6c20 6f75 7420 7468 6520  e, fill out the 
+00002a20: 6578 7472 6120 7072 6f70 6572 7469 6573  extra properties
+00002a30: 0a20 2020 2020 2020 2067 656f 6d65 7472  .        geometr
+00002a40: 7963 6f6c 756d 6e20 3d20 4e6f 6e65 0a20  ycolumn = None. 
+00002a50: 2020 2020 2020 2065 7874 656e 7420 3d20         extent = 
+00002a60: 4e6f 6e65 0a20 2020 2020 2020 2063 7273  None.        crs
+00002a70: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00002a80: 746f 7461 6c5f 626f 756e 6473 203d 204e  total_bounds = N
+00002a90: 6f6e 650a 2020 2020 2020 2020 6966 2067  one.        if g
+00002aa0: 656f 6d65 7472 7974 7970 6520 6973 206e  eometrytype is n
+00002ab0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002ac0: 2020 2020 2023 2047 656f 6d65 7472 7920       # Geometry 
+00002ad0: 636f 6c75 6d6e 206e 616d 650a 2020 2020  column name.    
+00002ae0: 2020 2020 2020 2020 6765 6f6d 6574 7279          geometry
+00002af0: 636f 6c75 6d6e 203d 2064 6174 6173 6f75  column = datasou
+00002b00: 7263 655f 6c61 7965 722e 4765 7447 656f  rce_layer.GetGeo
+00002b10: 6d65 7472 7943 6f6c 756d 6e28 290a 2020  metryColumn().  
+00002b20: 2020 2020 2020 2020 2020 6966 2067 656f            if geo
+00002b30: 6d65 7472 7963 6f6c 756d 6e20 3d3d 2022  metrycolumn == "
+00002b40: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00002b50: 2020 2067 656f 6d65 7472 7963 6f6c 756d     geometrycolum
+00002b60: 6e20 3d20 2267 656f 6d65 7472 7922 0a20  n = "geometry". 
+00002b70: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
+00002b80: 7665 7274 2065 7874 656e 7420 2878 6d69  vert extent (xmi
+00002b90: 6e2c 2078 6d61 782c 2079 6d69 6e2c 2079  n, xmax, ymin, y
+00002ba0: 6d61 7829 2074 6f20 626f 756e 6473 2028  max) to bounds (
+00002bb0: 786d 696e 2c20 796d 696e 2c20 786d 6178  xmin, ymin, xmax
+00002bc0: 2c20 796d 6178 290a 2020 2020 2020 2020  , ymax).        
+00002bd0: 2020 2020 6578 7465 6e74 203d 2064 6174      extent = dat
+00002be0: 6173 6f75 7263 655f 6c61 7965 722e 4765  asource_layer.Ge
+00002bf0: 7445 7874 656e 7428 290a 2020 2020 2020  tExtent().      
+00002c00: 2020 2020 2020 746f 7461 6c5f 626f 756e        total_boun
+00002c10: 6473 203d 2028 6578 7465 6e74 5b30 5d2c  ds = (extent[0],
+00002c20: 2065 7874 656e 745b 325d 2c20 6578 7465   extent[2], exte
+00002c30: 6e74 5b31 5d2c 2065 7874 656e 745b 335d  nt[1], extent[3]
+00002c40: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00002c50: 4352 530a 2020 2020 2020 2020 2020 2020  CRS.            
+00002c60: 7370 6174 6961 6c72 6566 203d 2064 6174  spatialref = dat
+00002c70: 6173 6f75 7263 655f 6c61 7965 722e 4765  asource_layer.Ge
+00002c80: 7453 7061 7469 616c 5265 6628 290a 2020  tSpatialRef().  
+00002c90: 2020 2020 2020 2020 2020 6966 2073 7061            if spa
+00002ca0: 7469 616c 7265 6620 6973 206e 6f74 204e  tialref is not N
+00002cb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00002cc0: 2020 2020 2063 7273 203d 2070 7970 726f       crs = pypro
+00002cd0: 6a2e 4352 5328 7370 6174 6961 6c72 6566  j.CRS(spatialref
+00002ce0: 2e45 7870 6f72 7454 6f57 6b74 2829 290a  .ExportToWkt()).
+00002cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d00: 2023 2049 6620 7370 6174 6961 6c20 7265   # If spatial re
+00002d10: 6620 6861 7320 6e6f 2065 7073 672c 2074  f has no epsg, t
+00002d20: 7279 2074 6f20 6669 6e64 2063 6f72 7265  ry to find corre
+00002d30: 7370 6f6e 6469 6e67 206f 6e65 0a20 2020  sponding one.   
+00002d40: 2020 2020 2020 2020 2020 2020 2063 7273               crs
+00002d50: 5f65 7073 6720 3d20 6372 732e 746f 5f65  _epsg = crs.to_e
+00002d60: 7073 6728 290a 2020 2020 2020 2020 2020  psg().          
+00002d70: 2020 2020 2020 6966 2063 7273 5f65 7073        if crs_eps
+00002d80: 6720 6973 204e 6f6e 653a 0a20 2020 2020  g is None:.     
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002da0: 6620 6372 732e 6e61 6d65 2069 6e20 5b0a  f crs.name in [.
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2020 2020 2020 2020 2242 656c 6765 2031          "Belge 1
+00002dd0: 3937 3220 2f20 4265 6c67 6961 6e20 4c61  972 / Belgian La
+00002de0: 6d62 6572 7420 3732 222c 0a20 2020 2020  mbert 72",.     
+00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e00: 2020 2022 4265 6c67 655f 3139 3732 5f42     "Belge_1972_B
+00002e10: 656c 6769 616e 5f4c 616d 6265 7274 5f37  elgian_Lambert_7
+00002e20: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
+00002e30: 2020 2020 2020 2020 2020 2020 2242 656c              "Bel
+00002e40: 6765 5f4c 616d 6265 7274 5f31 3937 3222  ge_Lambert_1972"
+00002e50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002e60: 2020 2020 2020 2020 2020 2242 4437 3220            "BD72 
+00002e70: 2f20 4265 6c67 6961 6e20 4c61 6d62 6572  / Belgian Lamber
+00002e80: 7420 3732 222c 0a20 2020 2020 2020 2020  t 72",.         
+00002e90: 2020 2020 2020 2020 2020 205d 3a0a 2020             ]:.  
 00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002eb0: 2020 2020 2063 7273 203d 2070 7970 726f       crs = pypro
-00002ec0: 6a2e 4352 532e 6672 6f6d 5f65 7073 6728  j.CRS.from_epsg(
-00002ed0: 3331 3337 3029 0a0a 2020 2020 2020 2020  31370)..        
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ef0: 2320 4966 2073 6861 7065 6669 6c65 2c20  # If shapefile, 
-00002f00: 6164 6420 636f 7272 6563 7420 3331 3337  add correct 3137
-00002f10: 3020 2e70 726a 2066 696c 650a 2020 2020  0 .prj file.    
+00002eb0: 2020 2020 2020 2320 4265 6c67 6961 6e20        # Belgian 
+00002ec0: 4c61 6d62 6572 7420 696e 206e 616d 652c  Lambert in name,
+00002ed0: 2073 6f20 6173 7375 6d65 2033 3133 3730   so assume 31370
+00002ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ef0: 2020 2020 2020 2020 2063 7273 203d 2070           crs = p
+00002f00: 7970 726f 6a2e 4352 532e 6672 6f6d 5f65  yproj.CRS.from_e
+00002f10: 7073 6728 3331 3337 3029 0a0a 2020 2020  psg(31370)..    
 00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 6966 2047 656f 6669 6c65 5479      if GeofileTy
-00002f40: 7065 2870 6174 6829 203d 3d20 4765 6f66  pe(path) == Geof
-00002f50: 696c 6554 7970 652e 4553 5249 5368 6170  ileType.ESRIShap
-00002f60: 6566 696c 653a 0a20 2020 2020 2020 2020  efile:.         
-00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f80: 2020 2070 726a 5f70 6174 6820 3d20 7061     prj_path = pa
-00002f90: 7468 2e70 6172 656e 7420 2f20 6622 7b70  th.parent / f"{p
-00002fa0: 6174 682e 7374 656d 7d2e 7072 6a22 0a20  ath.stem}.prj". 
+00002f30: 2020 2020 2320 4966 2073 6861 7065 6669      # If shapefi
+00002f40: 6c65 2c20 6164 6420 636f 7272 6563 7420  le, add correct 
+00002f50: 3331 3337 3020 2e70 726a 2066 696c 650a  31370 .prj file.
+00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f70: 2020 2020 2020 2020 6966 2047 656f 6669          if Geofi
+00002f80: 6c65 5479 7065 2870 6174 6829 203d 3d20  leType(path) == 
+00002f90: 4765 6f66 696c 6554 7970 652e 4553 5249  GeofileType.ESRI
+00002fa0: 5368 6170 6566 696c 653a 0a20 2020 2020  Shapefile:.     
 00002fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fc0: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
-00002fd0: 6a5f 7061 7468 2e65 7869 7374 7328 293a  j_path.exists():
-00002fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003000: 2070 726a 5f72 656e 616d 655f 7061 7468   prj_rename_path
-00003010: 203d 2070 6174 682e 7061 7265 6e74 202f   = path.parent /
-00003020: 2066 227b 7061 7468 2e73 7465 6d7d 5f6f   f"{path.stem}_o
-00003030: 7269 672e 7072 6a22 0a20 2020 2020 2020  rig.prj".       
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00003060: 7072 6a5f 7265 6e61 6d65 5f70 6174 682e  prj_rename_path.
-00003070: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
+00002fc0: 2020 2020 2020 2070 726a 5f70 6174 6820         prj_path 
+00002fd0: 3d20 7061 7468 2e70 6172 656e 7420 2f20  = path.parent / 
+00002fe0: 6622 7b70 6174 682e 7374 656d 7d2e 7072  f"{path.stem}.pr
+00002ff0: 6a22 0a20 2020 2020 2020 2020 2020 2020  j".             
+00003000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003010: 6620 7072 6a5f 7061 7468 2e65 7869 7374  f prj_path.exist
+00003020: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 2020 2020 2070 726a 5f72 656e 616d 655f       prj_rename_
+00003050: 7061 7468 203d 2070 6174 682e 7061 7265  path = path.pare
+00003060: 6e74 202f 2066 227b 7061 7468 2e73 7465  nt / f"{path.ste
+00003070: 6d7d 5f6f 7269 672e 7072 6a22 0a20 2020  m}_orig.prj".   
 00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003090: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000030a0: 6a5f 7061 7468 2e72 656e 616d 6528 7072  j_path.rename(pr
-000030b0: 6a5f 7265 6e61 6d65 5f70 6174 6829 0a20  j_rename_path). 
+00003090: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000030a0: 6e6f 7420 7072 6a5f 7265 6e61 6d65 5f70  not prj_rename_p
+000030b0: 6174 682e 6578 6973 7473 2829 3a0a 2020  ath.exists():.  
 000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000030e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003100: 2020 2020 2020 2020 2070 726a 5f70 6174           prj_pat
-00003110: 682e 756e 6c69 6e6b 2829 0a20 2020 2020  h.unlink().     
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2020 2020 2020 2020 2070 726a 5f70             prj_p
-00003140: 6174 682e 7772 6974 655f 7465 7874 2850  ath.write_text(P
-00003150: 524a 5f45 5053 475f 3331 3337 3029 0a0a  RJ_EPSG_31370)..
-00003160: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003170: 726e 204c 6179 6572 496e 666f 280a 2020  rn LayerInfo(.  
-00003180: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00003190: 6d65 3d64 6174 6173 6f75 7263 655f 6c61  me=datasource_la
-000031a0: 7965 722e 4765 744e 616d 6528 292c 0a20  yer.GetName(),. 
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000031c0: 6561 7475 7265 636f 756e 743d 6461 7461  eaturecount=data
-000031d0: 736f 7572 6365 5f6c 6179 6572 2e47 6574  source_layer.Get
-000031e0: 4665 6174 7572 6543 6f75 6e74 2829 2c0a  FeatureCount(),.
-000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003200: 746f 7461 6c5f 626f 756e 6473 3d74 6f74  total_bounds=tot
-00003210: 616c 5f62 6f75 6e64 732c 0a20 2020 2020  al_bounds,.     
-00003220: 2020 2020 2020 2020 2020 2067 656f 6d65             geome
-00003230: 7472 7963 6f6c 756d 6e3d 6765 6f6d 6574  trycolumn=geomet
-00003240: 7279 636f 6c75 6d6e 2c0a 2020 2020 2020  rycolumn,.      
-00003250: 2020 2020 2020 2020 2020 6765 6f6d 6574            geomet
-00003260: 7279 7479 7065 6e61 6d65 3d67 656f 6d65  rytypename=geome
-00003270: 7472 7974 7970 656e 616d 652c 0a20 2020  trytypename,.   
-00003280: 2020 2020 2020 2020 2020 2020 2067 656f               geo
-00003290: 6d65 7472 7974 7970 653d 6765 6f6d 6574  metrytype=geomet
-000032a0: 7279 7479 7065 2c0a 2020 2020 2020 2020  rytype,.        
-000032b0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-000032c0: 636f 6c75 6d6e 732c 0a20 2020 2020 2020  columns,.       
-000032d0: 2020 2020 2020 2020 2066 6964 5f63 6f6c           fid_col
-000032e0: 756d 6e3d 6461 7461 736f 7572 6365 5f6c  umn=datasource_l
-000032f0: 6179 6572 2e47 6574 4649 4443 6f6c 756d  ayer.GetFIDColum
-00003300: 6e28 292c 0a20 2020 2020 2020 2020 2020  n(),.           
-00003310: 2020 2020 2063 7273 3d63 7273 2c0a 2020       crs=crs,.  
-00003320: 2020 2020 2020 2020 2020 2020 2020 6572                er
-00003330: 726f 7273 3d65 7272 6f72 732c 0a20 2020  rors=errors,.   
-00003340: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00003350: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003360: 2020 2020 2065 7272 6f72 732e 6170 7065       errors.appe
-00003370: 6e64 2822 4c61 7965 7220 646f 6573 6e27  nd("Layer doesn'
-00003380: 7420 6861 7665 2061 2067 656f 6d65 7472  t have a geometr
-00003390: 7920 636f 6c75 6d6e 2122 290a 0a20 2020  y column!")..   
-000033a0: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-000033b0: 2020 6966 2064 6174 6173 6f75 7263 6520    if datasource 
-000033c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000033d0: 2020 2020 2020 2020 2064 656c 2064 6174           del dat
-000033e0: 6173 6f75 7263 650a 0a20 2020 2023 2049  asource..    # I
-000033f0: 6620 7765 2064 6964 6e27 7420 7265 7475  f we didn't retu
-00003400: 726e 206f 7220 7261 6973 6520 7965 7420  rn or raise yet 
-00003410: 6865 7265 2c20 7468 6572 6520 6d75 7374  here, there must
-00003420: 2068 6176 6520 6265 656e 2065 7272 6f72   have been error
-00003430: 730a 2020 2020 6572 726f 7273 5f73 7472  s.    errors_str
-00003440: 203d 2070 7072 696e 742e 7066 6f72 6d61   = pprint.pforma
-00003450: 7428 6572 726f 7273 290a 2020 2020 7261  t(errors).    ra
-00003460: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
-00003470: 2020 2020 2020 2066 2245 7272 6f72 7320         f"Errors 
-00003480: 696e 206c 6179 6572 2064 6566 696e 6974  in layer definit
-00003490: 696f 6e20 6f66 2066 696c 6520 7b70 6174  ion of file {pat
-000034a0: 687d 2c20 6c61 7965 7220 7b6c 6179 6572  h}, layer {layer
-000034b0: 7d3a 205c 6e7b 6572 726f 7273 5f73 7472  }: \n{errors_str
-000034c0: 7d22 0a20 2020 2029 0a0a 0a64 6566 2067  }".    )...def g
-000034d0: 6574 5f6f 6e6c 795f 6c61 7965 7228 7061  et_only_layer(pa
-000034e0: 7468 3a20 556e 696f 6e5b 7374 722c 2022  th: Union[str, "
-000034f0: 6f73 2e50 6174 684c 696b 655b 416e 795d  os.PathLike[Any]
-00003500: 225d 2920 2d3e 2073 7472 3a0a 2020 2020  "]) -> str:.    
-00003510: 2222 220a 2020 2020 4765 7420 7468 6520  """.    Get the 
-00003520: 6c61 7965 726e 616d 6520 666f 7220 6120  layername for a 
-00003530: 6669 6c65 2074 6861 7420 6f6e 6c79 2063  file that only c
-00003540: 6f6e 7461 696e 7320 6f6e 6520 6c61 7965  ontains one laye
-00003550: 722e 0a0a 2020 2020 4966 2074 6865 2066  r...    If the f
-00003560: 696c 6520 636f 6e74 6169 6e73 206d 756c  ile contains mul
-00003570: 7469 706c 6520 6c61 7965 7273 2c20 616e  tiple layers, an
-00003580: 2065 7863 6570 7469 6f6e 2069 7320 7468   exception is th
-00003590: 726f 776e 2e0a 0a20 2020 2041 7267 733a  rown...    Args:
-000035a0: 0a20 2020 2020 2020 2070 6174 6820 2850  .        path (P
-000035b0: 6174 684c 696b 6529 3a20 7468 6520 6669  athLike): the fi
-000035c0: 6c65 2e0a 0a20 2020 2052 6169 7365 733a  le...    Raises:
-000035d0: 0a20 2020 2020 2020 2056 616c 7565 4572  .        ValueEr
-000035e0: 726f 723a 2061 6e20 696e 7661 6c69 6420  ror: an invalid 
-000035f0: 7061 7261 6d65 7465 7220 7661 6c75 6520  parameter value 
-00003600: 7761 7320 7061 7373 6564 2e0a 0a20 2020  was passed...   
-00003610: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00003620: 2020 7374 723a 2074 6865 206c 6179 6572    str: the layer
-00003630: 206e 616d 650a 2020 2020 2222 220a 2020   name.    """.  
-00003640: 2020 6461 7461 736f 7572 6365 203d 204e    datasource = N
-00003650: 6f6e 650a 2020 2020 7472 793a 0a20 2020  one.    try:.   
-00003660: 2020 2020 2064 6174 6173 6f75 7263 655f       datasource_
-00003670: 6c61 7965 7220 3d20 4e6f 6e65 0a20 2020  layer = None.   
-00003680: 2020 2020 2064 6174 6173 6f75 7263 6520       datasource 
-00003690: 3d20 6764 616c 2e4f 7065 6e45 7828 0a20  = gdal.OpenEx(. 
-000036a0: 2020 2020 2020 2020 2020 2073 7472 2870             str(p
-000036b0: 6174 6829 2c20 6e4f 7065 6e46 6c61 6773  ath), nOpenFlags
-000036c0: 3d67 6461 6c2e 4f46 5f56 4543 544f 5220  =gdal.OF_VECTOR 
-000036d0: 7c20 6764 616c 2e4f 465f 5245 4144 4f4e  | gdal.OF_READON
-000036e0: 4c59 207c 2067 6461 6c2e 4f46 5f53 4841  LY | gdal.OF_SHA
-000036f0: 5245 440a 2020 2020 2020 2020 290a 2020  RED.        ).  
-00003700: 2020 2020 2020 6e62 5f6c 6179 6572 7320        nb_layers 
-00003710: 3d20 6461 7461 736f 7572 6365 2e47 6574  = datasource.Get
-00003720: 4c61 7965 7243 6f75 6e74 2829 0a20 2020  LayerCount().   
-00003730: 2020 2020 2069 6620 6e62 5f6c 6179 6572       if nb_layer
-00003740: 7320 3d3d 2031 3a0a 2020 2020 2020 2020  s == 1:.        
-00003750: 2020 2020 6461 7461 736f 7572 6365 5f6c      datasource_l
-00003760: 6179 6572 203d 2064 6174 6173 6f75 7263  ayer = datasourc
-00003770: 652e 4765 744c 6179 6572 4279 496e 6465  e.GetLayerByInde
-00003780: 7828 3029 0a20 2020 2020 2020 2065 6c69  x(0).        eli
-00003790: 6620 6e62 5f6c 6179 6572 7320 3d3d 2030  f nb_layers == 0
-000037a0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000037b0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-000037c0: 2245 7272 6f72 3a20 4e6f 206c 6179 6572  "Error: No layer
-000037d0: 7320 666f 756e 6420 696e 207b 7061 7468  s found in {path
-000037e0: 7d22 290a 2020 2020 2020 2020 656c 7365  }").        else
-000037f0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00003800: 4368 6563 6b20 6966 2074 6865 7265 2069  Check if there i
-00003810: 7320 6f6e 6c79 206f 6e65 2073 7061 7469  s only one spati
-00003820: 616c 206c 6179 6572 0a20 2020 2020 2020  al layer.       
-00003830: 2020 2020 206c 6179 6572 7320 3d20 6c69       layers = li
-00003840: 7374 6c61 7965 7273 2870 6174 682c 206f  stlayers(path, o
-00003850: 6e6c 795f 7370 6174 6961 6c5f 6c61 7965  nly_spatial_laye
-00003860: 7273 3d54 7275 6529 0a20 2020 2020 2020  rs=True).       
-00003870: 2020 2020 2069 6620 6c65 6e28 6c61 7965       if len(laye
-00003880: 7273 2920 3d3d 2031 3a0a 2020 2020 2020  rs) == 1:.      
-00003890: 2020 2020 2020 2020 2020 6461 7461 736f            dataso
-000038a0: 7572 6365 5f6c 6179 6572 203d 2064 6174  urce_layer = dat
-000038b0: 6173 6f75 7263 652e 4765 744c 6179 6572  asource.GetLayer
-000038c0: 286c 6179 6572 735b 305d 290a 2020 2020  (layers[0]).    
-000038d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000038e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000038f0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-00003900: 224c 6179 6572 2068 6173 203e 2031 206c  "Layer has > 1 l
-00003910: 6179 6572 3a20 7b70 6174 687d 3a20 7b6c  ayer: {path}: {l
-00003920: 6179 6572 737d 2229 0a0a 2020 2020 2020  ayers}")..      
-00003930: 2020 7265 7475 726e 2064 6174 6173 6f75    return datasou
-00003940: 7263 655f 6c61 7965 722e 4765 744e 616d  rce_layer.GetNam
-00003950: 6528 290a 0a20 2020 2066 696e 616c 6c79  e()..    finally
-00003960: 3a0a 2020 2020 2020 2020 6966 2064 6174  :.        if dat
-00003970: 6173 6f75 7263 6520 6973 206e 6f74 204e  asource is not N
-00003980: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00003990: 2064 656c 2064 6174 6173 6f75 7263 650a   del datasource.
-000039a0: 0a0a 6465 6620 6765 745f 6465 6661 756c  ..def get_defaul
-000039b0: 745f 6c61 7965 7228 7061 7468 3a20 556e  t_layer(path: Un
-000039c0: 696f 6e5b 7374 722c 2022 6f73 2e50 6174  ion[str, "os.Pat
-000039d0: 684c 696b 655b 416e 795d 225d 2920 2d3e  hLike[Any]"]) ->
-000039e0: 2073 7472 3a0a 2020 2020 2222 220a 2020   str:.    """.  
-000039f0: 2020 4765 7420 7468 6520 6465 6661 756c    Get the defaul
-00003a00: 7420 6c61 7965 7220 6e61 6d65 2074 6f20  t layer name to 
-00003a10: 6265 2075 7365 6420 666f 7220 6120 6c61  be used for a la
-00003a20: 7965 7220 696e 2074 6869 7320 6669 6c65  yer in this file
-00003a30: 2e0a 0a20 2020 2054 6869 7320 6973 2074  ...    This is t
-00003a40: 6865 2073 7465 6d20 6f66 2074 6865 2066  he stem of the f
-00003a50: 696c 6570 6174 682e 0a0a 2020 2020 4172  ilepath...    Ar
-00003a60: 6773 3a0a 2020 2020 2020 2020 7061 7468  gs:.        path
-00003a70: 2028 556e 696f 6e5b 7374 722c 293a 2054   (Union[str,): T
-00003a80: 6865 2070 6174 6820 746f 2074 6865 2066  he path to the f
-00003a90: 696c 652e 0a0a 2020 2020 5265 7475 726e  ile...    Return
-00003aa0: 733a 0a20 2020 2020 2020 2073 7472 3a20  s:.        str: 
-00003ab0: 5468 6520 6465 6661 756c 7420 6c61 7965  The default laye
-00003ac0: 7220 6e61 6d65 2e0a 2020 2020 2222 220a  r name..    """.
-00003ad0: 2020 2020 7265 7475 726e 2050 6174 6828      return Path(
-00003ae0: 7061 7468 292e 7374 656d 0a0a 0a64 6566  path).stem...def
-00003af0: 2065 7865 6375 7465 5f73 716c 280a 2020   execute_sql(.  
-00003b00: 2020 7061 7468 3a20 556e 696f 6e5b 7374    path: Union[st
-00003b10: 722c 2022 6f73 2e50 6174 684c 696b 655b  r, "os.PathLike[
-00003b20: 416e 795d 225d 2c0a 2020 2020 7371 6c5f  Any]"],.    sql_
-00003b30: 7374 6d74 3a20 7374 722c 0a20 2020 2073  stmt: str,.    s
-00003b40: 716c 5f64 6961 6c65 6374 3a20 4f70 7469  ql_dialect: Opti
-00003b50: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00003b60: 2c0a 293a 0a20 2020 2022 2222 0a20 2020  ,.):.    """.   
-00003b70: 2045 7865 6375 7465 2061 2073 716c 2073   Execute a sql s
-00003b80: 7461 7465 6d65 6e74 2028 444d 4c20 6f72  tatement (DML or
-00003b90: 2044 444c 2920 6f6e 2074 6865 2066 696c   DDL) on the fil
-00003ba0: 652e 0a0a 2020 2020 546f 2072 756e 2053  e...    To run S
-00003bb0: 454c 4543 5420 7371 6c20 7374 6174 656d  ELECT sql statem
-00003bc0: 656e 7473 206f 6e20 6120 6669 6c65 2c20  ents on a file, 
-00003bd0: 7573 6520 3a6d 6574 683a 607e 7265 6164  use :meth:`~read
-00003be0: 5f66 696c 6560 2e0a 0a20 2020 2041 7267  _file`...    Arg
-00003bf0: 733a 0a20 2020 2020 2020 2070 6174 6820  s:.        path 
-00003c00: 2850 6174 684c 696b 6529 3a20 5468 6520  (PathLike): The 
-00003c10: 7061 7468 2074 6f20 7468 6520 6669 6c65  path to the file
-00003c20: 2e0a 2020 2020 2020 2020 7371 6c5f 7374  ..        sql_st
-00003c30: 6d74 2028 7374 7229 3a20 5468 6520 7371  mt (str): The sq
-00003c40: 6c20 7374 6174 656d 656e 7420 746f 2065  l statement to e
-00003c50: 7865 6375 7465 2e0a 2020 2020 2020 2020  xecute..        
-00003c60: 7371 6c5f 6469 616c 6563 7420 2873 7472  sql_dialect (str
-00003c70: 293a 2054 6865 2073 716c 2064 6961 6c65  ): The sql diale
-00003c80: 6374 2074 6f20 7573 653a 0a20 2020 2020  ct to use:.     
-00003c90: 2020 2020 2020 202a 204e 6f6e 653a 2075         * None: u
-00003ca0: 7365 2074 6865 206e 6174 6976 6520 5351  se the native SQ
-00003cb0: 4c20 6469 616c 6563 7420 6f66 2074 6865  L dialect of the
-00003cc0: 2067 656f 6669 6c65 2e0a 2020 2020 2020   geofile..      
-00003cd0: 2020 2020 2020 2a20 274f 4752 5351 4c27        * 'OGRSQL'
-00003ce0: 3a20 666f 7263 6520 7468 6520 7573 6520  : force the use 
-00003cf0: 6f66 2074 6865 204f 4752 2053 514c 2064  of the OGR SQL d
-00003d00: 6961 6c65 6374 2e0a 2020 2020 2020 2020  ialect..        
-00003d10: 2020 2020 2a20 2753 514c 4954 4527 3a20      * 'SQLITE': 
-00003d20: 666f 7263 6520 7468 6520 7573 6520 6f66  force the use of
-00003d30: 2074 6865 2053 514c 4954 4520 6469 616c   the SQLITE dial
-00003d40: 6563 742e 0a20 2020 2020 2020 2020 2020  ect..           
-00003d50: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00003d60: 652e 0a20 2020 2022 2222 0a20 2020 2064  e..    """.    d
-00003d70: 6174 6173 6f75 7263 6520 3d20 4e6f 6e65  atasource = None
-00003d80: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
-00003d90: 2020 6461 7461 736f 7572 6365 203d 2067    datasource = g
-00003da0: 6461 6c2e 4f70 656e 4578 2873 7472 2870  dal.OpenEx(str(p
-00003db0: 6174 6829 2c20 6e4f 7065 6e46 6c61 6773  ath), nOpenFlags
-00003dc0: 3d67 6461 6c2e 4f46 5f55 5044 4154 4529  =gdal.OF_UPDATE)
-00003dd0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00003de0: 3d20 6461 7461 736f 7572 6365 2e45 7865  = datasource.Exe
-00003df0: 6375 7465 5351 4c28 7371 6c5f 7374 6d74  cuteSQL(sql_stmt
-00003e00: 2c20 6469 616c 6563 743d 7371 6c5f 6469  , dialect=sql_di
-00003e10: 616c 6563 7429 0a20 2020 2020 2020 2064  alect).        d
-00003e20: 6174 6173 6f75 7263 652e 5265 6c65 6173  atasource.Releas
-00003e30: 6552 6573 756c 7453 6574 2872 6573 756c  eResultSet(resul
-00003e40: 7429 0a20 2020 2066 696e 616c 6c79 3a0a  t).    finally:.
-00003e50: 2020 2020 2020 2020 6966 2064 6174 6173          if datas
-00003e60: 6f75 7263 6520 6973 206e 6f74 204e 6f6e  ource is not Non
-00003e70: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-00003e80: 656c 2064 6174 6173 6f75 7263 650a 0a0a  el datasource...
-00003e90: 6465 6620 6372 6561 7465 5f73 7061 7469  def create_spati
-00003ea0: 616c 5f69 6e64 6578 280a 2020 2020 7061  al_index(.    pa
-00003eb0: 7468 3a20 556e 696f 6e5b 7374 722c 2022  th: Union[str, "
-00003ec0: 6f73 2e50 6174 684c 696b 655b 416e 795d  os.PathLike[Any]
-00003ed0: 225d 2c0a 2020 2020 6c61 7965 723a 204f  "],.    layer: O
-00003ee0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00003ef0: 6f6e 652c 0a20 2020 2063 6163 6865 5f73  one,.    cache_s
-00003f00: 697a 655f 6d62 3a20 696e 7420 3d20 3132  ize_mb: int = 12
-00003f10: 382c 0a20 2020 2065 7869 7374 5f6f 6b3a  8,.    exist_ok:
-00003f20: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00003f30: 2020 2066 6f72 6365 5f72 6562 7569 6c64     force_rebuild
-00003f40: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00003f50: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
-00003f60: 7265 6174 6520 6120 7370 6174 6961 6c20  reate a spatial 
-00003f70: 696e 6465 7820 6f6e 2074 6865 206c 6179  index on the lay
-00003f80: 6572 2073 7065 6369 6669 6564 2e0a 0a20  er specified... 
-00003f90: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00003fa0: 2070 6174 6820 2850 6174 684c 696b 6529   path (PathLike)
-00003fb0: 3a20 5468 6520 6669 6c65 2070 6174 682e  : The file path.
-00003fc0: 0a20 2020 2020 2020 206c 6179 6572 2028  .        layer (
-00003fd0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00003fe0: 5468 6520 6c61 7965 722e 2049 6620 6e6f  The layer. If no
-00003ff0: 7420 7370 6563 6966 6965 642c 2061 6e64  t specified, and
-00004000: 2074 6865 7265 2069 7320 6f6e 6c79 0a20   there is only. 
-00004010: 2020 2020 2020 2020 2020 206f 6e65 206c             one l
-00004020: 6179 6572 2069 6e20 7468 6520 6669 6c65  ayer in the file
-00004030: 2c20 7468 6973 206c 6179 6572 2069 7320  , this layer is 
-00004040: 7573 6564 2e20 4f74 6865 7277 6973 6520  used. Otherwise 
-00004050: 6578 6365 7074 696f 6e2e 0a20 2020 2020  exception..     
-00004060: 2020 2063 6163 6865 5f73 697a 655f 6d62     cache_size_mb
-00004070: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-00004080: 3a20 6d65 6d6f 7279 2069 6e20 4d42 2074  : memory in MB t
-00004090: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
-000040a0: 7768 696c 650a 2020 2020 2020 2020 2020  while.          
-000040b0: 2020 6372 6561 7469 6e67 2073 7061 7469    creating spati
-000040c0: 616c 2069 6e64 6578 2066 6f72 2073 7061  al index for spa
-000040d0: 7469 616c 6974 6520 6669 6c65 7320 282e  tialite files (.
-000040e0: 6770 6b67 206f 7220 2e73 716c 6974 6529  gpkg or .sqlite)
-000040f0: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-00004100: 6661 756c 7473 2074 6f20 3132 382e 0a20  faults to 128.. 
-00004110: 2020 2020 2020 2065 7869 7374 5f6f 6b20         exist_ok 
-00004120: 2862 6f6f 6c2c 206f 7074 696f 6e73 293a  (bool, options):
-00004130: 2049 6620 5472 7565 2061 6e64 2074 6865   If True and the
-00004140: 2069 6e64 6578 2065 7869 7374 7320 616c   index exists al
-00004150: 7265 6164 792c 2064 6f6e 2774 0a20 2020  ready, don't.   
-00004160: 2020 2020 2020 2020 2074 6872 6f77 2061           throw a
-00004170: 6e20 6572 726f 722e 0a20 2020 2020 2020  n error..       
-00004180: 2066 6f72 6365 5f72 6562 7569 6c64 2028   force_rebuild (
-00004190: 626f 6f6c 2c20 6f70 7469 6f6e 7329 3a20  bool, options): 
-000041a0: 5472 7565 2074 6f20 666f 7263 6520 7265  True to force re
-000041b0: 6275 696c 6420 6576 656e 2069 6620 696e  build even if in
-000041c0: 6465 780a 2020 2020 2020 2020 2020 2020  dex.            
-000041d0: 6578 6973 7473 2061 6c72 6561 6479 2e20  exists already. 
-000041e0: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
-000041f0: 652e 0a20 2020 2022 2222 0a20 2020 2023  e..    """.    #
-00004200: 2049 6e69 740a 2020 2020 7061 7468 203d   Init.    path =
-00004210: 2050 6174 6828 7061 7468 290a 2020 2020   Path(path).    
-00004220: 6966 206c 6179 6572 2069 7320 4e6f 6e65  if layer is None
-00004230: 3a0a 2020 2020 2020 2020 6c61 7965 7220  :.        layer 
-00004240: 3d20 6765 745f 6f6e 6c79 5f6c 6179 6572  = get_only_layer
-00004250: 2870 6174 6829 0a0a 2020 2020 2320 4966  (path)..    # If
-00004260: 2069 6e64 6578 2061 6c72 6561 6479 2065   index already e
-00004270: 7869 7374 732c 2072 656d 6f76 6520 696e  xists, remove in
-00004280: 6465 7820 6f72 2072 6574 7572 6e0a 2020  dex or return.  
-00004290: 2020 6966 2068 6173 5f73 7061 7469 616c    if has_spatial
-000042a0: 5f69 6e64 6578 2870 6174 682c 206c 6179  _index(path, lay
-000042b0: 6572 293a 0a20 2020 2020 2020 2069 6620  er):.        if 
-000042c0: 666f 7263 655f 7265 6275 696c 643a 0a20  force_rebuild:. 
-000042d0: 2020 2020 2020 2020 2020 2072 656d 6f76             remov
-000042e0: 655f 7370 6174 6961 6c5f 696e 6465 7828  e_spatial_index(
-000042f0: 7061 7468 2c20 6c61 7965 7229 0a20 2020  path, layer).   
-00004300: 2020 2020 2065 6c69 6620 6578 6973 745f       elif exist_
-00004310: 6f6b 3a0a 2020 2020 2020 2020 2020 2020  ok:.            
-00004320: 7265 7475 726e 0a20 2020 2020 2020 2065  return.        e
-00004330: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00004340: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00004350: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004360: 2020 6622 4572 726f 7220 6164 6469 6e67    f"Error adding
-00004370: 2073 7061 7469 616c 2069 6e64 6578 2074   spatial index t
-00004380: 6f20 7b70 6174 687d 2e7b 6c61 7965 727d  o {path}.{layer}
-00004390: 2c20 6974 2065 7869 7374 7320 616c 7265  , it exists alre
-000043a0: 6164 7922 0a20 2020 2020 2020 2020 2020  ady".           
-000043b0: 2029 0a0a 2020 2020 2320 4e6f 7720 7265   )..    # Now re
-000043c0: 616c 6c79 2061 6464 2069 6e64 6578 0a20  ally add index. 
-000043d0: 2020 2064 6174 6173 6f75 7263 6520 3d20     datasource = 
-000043e0: 4e6f 6e65 0a20 2020 2074 7279 3a0a 2020  None.    try:.  
-000043f0: 2020 2020 2020 6765 6f66 696c 6574 7970        geofiletyp
-00004400: 6520 3d20 4765 6f66 696c 6554 7970 6528  e = GeofileType(
-00004410: 7061 7468 290a 2020 2020 2020 2020 6966  path).        if
-00004420: 2067 656f 6669 6c65 7479 7065 2e69 735f   geofiletype.is_
-00004430: 7370 6174 6961 6c69 7465 5f62 6173 6564  spatialite_based
-00004440: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00004450: 5468 6520 636f 6e66 6967 206f 7074 696f  The config optio
-00004460: 6e73 206e 6565 6420 746f 2062 6520 7365  ns need to be se
-00004470: 7420 6265 666f 7265 206f 7065 6e69 6e67  t before opening
-00004480: 2074 6865 2066 696c 6521 0a20 2020 2020   the file!.     
-00004490: 2020 2020 2020 206c 6179 6572 696e 666f         layerinfo
-000044a0: 203d 2067 6574 5f6c 6179 6572 696e 666f   = get_layerinfo
-000044b0: 2870 6174 682c 206c 6179 6572 290a 2020  (path, layer).  
-000044c0: 2020 2020 2020 2020 2020 7769 7468 205f            with _
-000044d0: 6f67 725f 7574 696c 2e73 6574 5f63 6f6e  ogr_util.set_con
-000044e0: 6669 675f 6f70 7469 6f6e 7328 7b22 4f47  fig_options({"OG
-000044f0: 525f 5351 4c49 5445 5f43 4143 4845 223a  R_SQLITE_CACHE":
-00004500: 2063 6163 6865 5f73 697a 655f 6d62 7d29   cache_size_mb})
-00004510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004520: 2020 6461 7461 736f 7572 6365 203d 2067    datasource = g
-00004530: 6461 6c2e 4f70 656e 4578 2873 7472 2870  dal.OpenEx(str(p
-00004540: 6174 6829 2c20 6e4f 7065 6e46 6c61 6773  ath), nOpenFlags
-00004550: 3d67 6461 6c2e 4f46 5f55 5044 4154 4529  =gdal.OF_UPDATE)
-00004560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004570: 2067 656f 6d65 7472 7963 6f6c 756d 6e20   geometrycolumn 
-00004580: 3d20 6c61 7965 7269 6e66 6f2e 6765 6f6d  = layerinfo.geom
-00004590: 6574 7279 636f 6c75 6d6e 0a20 2020 2020  etrycolumn.     
-000045a0: 2020 2020 2020 2020 2020 2073 716c 203d             sql =
-000045b0: 2066 2253 454c 4543 5420 4372 6561 7465   f"SELECT Create
-000045c0: 5370 6174 6961 6c49 6e64 6578 2827 7b6c  SpatialIndex('{l
-000045d0: 6179 6572 7d27 2c20 277b 6765 6f6d 6574  ayer}', '{geomet
-000045e0: 7279 636f 6c75 6d6e 7d27 2922 0a20 2020  rycolumn}')".   
-000045f0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00004600: 756c 7420 3d20 6461 7461 736f 7572 6365  ult = datasource
-00004610: 2e45 7865 6375 7465 5351 4c28 7371 6c2c  .ExecuteSQL(sql,
-00004620: 2064 6961 6c65 6374 3d22 5351 4c49 5445   dialect="SQLITE
-00004630: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00004640: 2020 2064 6174 6173 6f75 7263 652e 5265     datasource.Re
-00004650: 6c65 6173 6552 6573 756c 7453 6574 2872  leaseResultSet(r
-00004660: 6573 756c 7429 0a20 2020 2020 2020 2065  esult).        e
-00004670: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00004680: 2064 6174 6173 6f75 7263 6520 3d20 6764   datasource = gd
-00004690: 616c 2e4f 7065 6e45 7828 7374 7228 7061  al.OpenEx(str(pa
-000046a0: 7468 292c 206e 4f70 656e 466c 6167 733d  th), nOpenFlags=
-000046b0: 6764 616c 2e4f 465f 5550 4441 5445 290a  gdal.OF_UPDATE).
-000046c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000046d0: 6c74 203d 2064 6174 6173 6f75 7263 652e  lt = datasource.
-000046e0: 4578 6563 7574 6553 514c 2866 2743 5245  ExecuteSQL(f'CRE
-000046f0: 4154 4520 5350 4154 4941 4c20 494e 4445  ATE SPATIAL INDE
-00004700: 5820 4f4e 2022 7b6c 6179 6572 7d22 2729  X ON "{layer}"')
-00004710: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00004720: 6173 6f75 7263 652e 5265 6c65 6173 6552  asource.ReleaseR
-00004730: 6573 756c 7453 6574 2872 6573 756c 7429  esultSet(result)
-00004740: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
-00004750: 7074 696f 6e20 6173 2065 783a 0a20 2020  ption as ex:.   
-00004760: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00004770: 7469 6f6e 2866 2245 7272 6f72 2061 6464  tion(f"Error add
-00004780: 696e 6720 7370 6174 6961 6c20 696e 6465  ing spatial inde
-00004790: 7820 746f 207b 7061 7468 7d2e 7b6c 6179  x to {path}.{lay
-000047a0: 6572 7d22 2920 6672 6f6d 2065 780a 2020  er}") from ex.  
-000047b0: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
-000047c0: 2020 2069 6620 6461 7461 736f 7572 6365     if datasource
-000047d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000047e0: 2020 2020 2020 2020 2020 6465 6c20 6461            del da
-000047f0: 7461 736f 7572 6365 0a0a 2020 2020 6966  tasource..    if
-00004800: 206e 6f74 2068 6173 5f73 7061 7469 616c   not has_spatial
-00004810: 5f69 6e64 6578 2870 6174 682c 206c 6179  _index(path, lay
-00004820: 6572 293a 0a20 2020 2020 2020 2072 6169  er):.        rai
-00004830: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
-00004840: 6622 6372 6561 7465 5f73 7061 7469 616c  f"create_spatial
-00004850: 5f69 6e64 6578 2066 6169 6c65 6420 6f6e  _index failed on
-00004860: 207b 7061 7468 7d2c 206c 6179 6572 3a20   {path}, layer: 
-00004870: 7b6c 6179 6572 7d22 290a 0a0a 6465 6620  {layer}")...def 
-00004880: 6861 735f 7370 6174 6961 6c5f 696e 6465  has_spatial_inde
-00004890: 7828 0a20 2020 2070 6174 683a 2055 6e69  x(.    path: Uni
-000048a0: 6f6e 5b73 7472 2c20 226f 732e 5061 7468  on[str, "os.Path
-000048b0: 4c69 6b65 5b41 6e79 5d22 5d2c 206c 6179  Like[Any]"], lay
-000048c0: 6572 3a20 4f70 7469 6f6e 616c 5b73 7472  er: Optional[str
-000048d0: 5d20 3d20 4e6f 6e65 0a29 202d 3e20 626f  ] = None.) -> bo
-000048e0: 6f6c 3a0a 2020 2020 2222 220a 2020 2020  ol:.    """.    
-000048f0: 4368 6563 6b20 6966 2074 6865 206c 6179  Check if the lay
-00004900: 6572 2f63 6f6c 756d 6e20 6861 7320 6120  er/column has a 
-00004910: 7370 6174 6961 6c20 696e 6465 782e 0a0a  spatial index...
-00004920: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00004930: 2020 7061 7468 2028 5061 7468 4c69 6b65    path (PathLike
-00004940: 293a 2054 6865 2066 696c 6520 7061 7468  ): The file path
-00004950: 2e0a 2020 2020 2020 2020 6c61 7965 7220  ..        layer 
-00004960: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00004970: 2054 6865 206c 6179 6572 2e20 4465 6661   The layer. Defa
-00004980: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
-00004990: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-000049a0: 2020 2056 616c 7565 4572 726f 723a 2061     ValueError: a
-000049b0: 6e20 696e 7661 6c69 6420 7061 7261 6d65  n invalid parame
-000049c0: 7465 7220 7661 6c75 6520 7761 7320 7061  ter value was pa
-000049d0: 7373 6564 2e0a 0a20 2020 2052 6574 7572  ssed...    Retur
-000049e0: 6e73 3a0a 2020 2020 2020 2020 626f 6f6c  ns:.        bool
-000049f0: 3a20 5472 7565 2069 6620 7468 6520 7370  : True if the sp
-00004a00: 6174 6961 6c20 636f 6c75 6d6e 2065 7869  atial column exi
-00004a10: 7374 732e 0a20 2020 2022 2222 0a20 2020  sts..    """.   
-00004a20: 2023 2049 6e69 740a 2020 2020 7061 7468   # Init.    path
-00004a30: 203d 2050 6174 6828 7061 7468 290a 0a20   = Path(path).. 
-00004a40: 2020 2023 204e 6f77 2063 6865 636b 2074     # Now check t
-00004a50: 6865 2069 6e64 6578 0a20 2020 2064 6174  he index.    dat
-00004a60: 6173 6f75 7263 6520 3d20 4e6f 6e65 0a20  asource = None. 
-00004a70: 2020 2067 656f 6669 6c65 7479 7065 203d     geofiletype =
-00004a80: 2047 656f 6669 6c65 5479 7065 2870 6174   GeofileType(pat
-00004a90: 6829 0a20 2020 2074 7279 3a0a 2020 2020  h).    try:.    
-00004aa0: 2020 2020 6966 2067 656f 6669 6c65 7479      if geofilety
-00004ab0: 7065 2e69 735f 7370 6174 6961 6c69 7465  pe.is_spatialite
-00004ac0: 5f62 6173 6564 3a0a 2020 2020 2020 2020  _based:.        
-00004ad0: 2020 2020 6c61 7965 7269 6e66 6f20 3d20      layerinfo = 
-00004ae0: 6765 745f 6c61 7965 7269 6e66 6f28 7061  get_layerinfo(pa
-00004af0: 7468 2c20 6c61 7965 7229 0a20 2020 2020  th, layer).     
-00004b00: 2020 2020 2020 2064 6174 6173 6f75 7263         datasourc
-00004b10: 6520 3d20 6764 616c 2e4f 7065 6e45 7828  e = gdal.OpenEx(
-00004b20: 7374 7228 7061 7468 292c 206e 4f70 656e  str(path), nOpen
-00004b30: 466c 6167 733d 6764 616c 2e4f 465f 5245  Flags=gdal.OF_RE
-00004b40: 4144 4f4e 4c59 290a 2020 2020 2020 2020  ADONLY).        
-00004b50: 2020 2020 7371 6c20 3d20 6622 2222 0a20      sql = f""". 
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00004b70: 454c 4543 5420 4861 7353 7061 7469 616c  ELECT HasSpatial
-00004b80: 496e 6465 7828 277b 6c61 7965 7269 6e66  Index('{layerinf
-00004b90: 6f2e 6e61 6d65 7d27 2c0a 2020 2020 2020  o.name}',.      
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2027 7b6c 6179 6572 696e 666f 2e67 656f   '{layerinfo.geo
-00004bd0: 6d65 7472 7963 6f6c 756d 6e7d 2729 0a20  metrycolumn}'). 
-00004be0: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-00004bf0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00004c00: 7420 3d20 6461 7461 736f 7572 6365 2e45  t = datasource.E
-00004c10: 7865 6375 7465 5351 4c28 7371 6c2c 2064  xecuteSQL(sql, d
-00004c20: 6961 6c65 6374 3d22 5351 4c49 5445 2229  ialect="SQLITE")
-00004c30: 0a20 2020 2020 2020 2020 2020 2068 6173  .            has
-00004c40: 5f73 7061 7469 616c 5f69 6e64 6578 203d  _spatial_index =
-00004c50: 2072 6573 756c 742e 4765 744e 6578 7446   result.GetNextF
-00004c60: 6561 7475 7265 2829 2e47 6574 4669 656c  eature().GetFiel
-00004c70: 6428 3029 203d 3d20 310a 2020 2020 2020  d(0) == 1.      
-00004c80: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
-00004c90: 2e52 656c 6561 7365 5265 7375 6c74 5365  .ReleaseResultSe
-00004ca0: 7428 7265 7375 6c74 290a 2020 2020 2020  t(result).      
-00004cb0: 2020 2020 2020 7265 7475 726e 2068 6173        return has
-00004cc0: 5f73 7061 7469 616c 5f69 6e64 6578 0a20  _spatial_index. 
-00004cd0: 2020 2020 2020 2065 6c69 6620 6765 6f66         elif geof
-00004ce0: 696c 6574 7970 6520 3d3d 2047 656f 6669  iletype == Geofi
-00004cf0: 6c65 5479 7065 2e45 5352 4953 6861 7065  leType.ESRIShape
-00004d00: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
-00004d10: 2020 696e 6465 785f 7061 7468 203d 2070    index_path = p
-00004d20: 6174 682e 7061 7265 6e74 202f 2066 227b  ath.parent / f"{
-00004d30: 7061 7468 2e73 7465 6d7d 2e71 6978 220a  path.stem}.qix".
-00004d40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004d50: 726e 2069 6e64 6578 5f70 6174 682e 6578  rn index_path.ex
-00004d60: 6973 7473 2829 0a20 2020 2020 2020 2065  ists().        e
-00004d70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00004d80: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00004d90: 7228 6622 6861 735f 7370 6174 6961 6c5f  r(f"has_spatial_
-00004da0: 696e 6465 7820 6e6f 7420 7375 7070 6f72  index not suppor
-00004db0: 7465 6420 666f 7220 7b70 6174 687d 2229  ted for {path}")
-00004dc0: 0a20 2020 2066 696e 616c 6c79 3a0a 2020  .    finally:.  
-00004dd0: 2020 2020 2020 6966 2064 6174 6173 6f75        if datasou
-00004de0: 7263 6520 6973 206e 6f74 204e 6f6e 653a  rce is not None:
-00004df0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00004e00: 6173 6f75 7263 6520 3d20 4e6f 6e65 0a0a  asource = None..
-00004e10: 0a64 6566 2072 656d 6f76 655f 7370 6174  .def remove_spat
-00004e20: 6961 6c5f 696e 6465 7828 0a20 2020 2070  ial_index(.    p
-00004e30: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
-00004e40: 226f 732e 5061 7468 4c69 6b65 5b41 6e79  "os.PathLike[Any
-00004e50: 5d22 5d2c 206c 6179 6572 3a20 4f70 7469  ]"], layer: Opti
-00004e60: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00004e70: 0a29 3a0a 2020 2020 2222 220a 2020 2020  .):.    """.    
-00004e80: 5265 6d6f 7665 2074 6865 2073 7061 7469  Remove the spati
-00004e90: 616c 2069 6e64 6578 2066 726f 6d20 7468  al index from th
-00004ea0: 6520 6c61 7965 7220 7370 6563 6966 6965  e layer specifie
-00004eb0: 642e 0a0a 2020 2020 4172 6773 3a0a 2020  d...    Args:.  
-00004ec0: 2020 2020 2020 7061 7468 2028 5061 7468        path (Path
-00004ed0: 4c69 6b65 293a 2054 6865 2066 696c 6520  Like): The file 
-00004ee0: 7061 7468 2e0a 2020 2020 2020 2020 6c61  path..        la
-00004ef0: 7965 7220 2873 7472 2c20 6f70 7469 6f6e  yer (str, option
-00004f00: 616c 293a 2054 6865 206c 6179 6572 2e20  al): The layer. 
-00004f10: 4966 206e 6f74 2073 7065 6369 6669 6564  If not specified
-00004f20: 2c20 616e 6420 7468 6572 6520 6973 206f  , and there is o
-00004f30: 6e6c 790a 2020 2020 2020 2020 2020 2020  nly.            
-00004f40: 6f6e 6520 6c61 7965 7220 696e 2074 6865  one layer in the
-00004f50: 2066 696c 652c 2074 6869 7320 6c61 7965   file, this laye
-00004f60: 7220 6973 2075 7365 642e 204f 7468 6572  r is used. Other
-00004f70: 7769 7365 2065 7863 6570 7469 6f6e 2e0a  wise exception..
-00004f80: 2020 2020 2222 220a 2020 2020 2320 496e      """.    # In
-00004f90: 6974 0a20 2020 2070 6174 6820 3d20 5061  it.    path = Pa
-00004fa0: 7468 2870 6174 6829 0a0a 2020 2020 2320  th(path)..    # 
-00004fb0: 4e6f 7720 7265 616c 6c79 2072 656d 6f76  Now really remov
-00004fc0: 6520 696e 6465 780a 2020 2020 6461 7461  e index.    data
-00004fd0: 736f 7572 6365 203d 204e 6f6e 650a 2020  source = None.  
-00004fe0: 2020 6765 6f66 696c 6574 7970 6520 3d20    geofiletype = 
-00004ff0: 4765 6f66 696c 6554 7970 6528 7061 7468  GeofileType(path
-00005000: 290a 2020 2020 6c61 7965 7269 6e66 6f20  ).    layerinfo 
-00005010: 3d20 6765 745f 6c61 7965 7269 6e66 6f28  = get_layerinfo(
-00005020: 7061 7468 2c20 6c61 7965 7229 0a20 2020  path, layer).   
-00005030: 2074 7279 3a0a 2020 2020 2020 2020 6966   try:.        if
-00005040: 2067 656f 6669 6c65 7479 7065 2e69 735f   geofiletype.is_
-00005050: 7370 6174 6961 6c69 7465 5f62 6173 6564  spatialite_based
-00005060: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-00005070: 7461 736f 7572 6365 203d 2067 6461 6c2e  tasource = gdal.
-00005080: 4f70 656e 4578 2873 7472 2870 6174 6829  OpenEx(str(path)
-00005090: 2c20 6e4f 7065 6e46 6c61 6773 3d67 6461  , nOpenFlags=gda
-000050a0: 6c2e 4f46 5f55 5044 4154 4529 0a20 2020  l.OF_UPDATE).   
-000050b0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-000050c0: 3d20 6461 7461 736f 7572 6365 2e45 7865  = datasource.Exe
-000050d0: 6375 7465 5351 4c28 0a20 2020 2020 2020  cuteSQL(.       
-000050e0: 2020 2020 2020 2020 2066 2253 454c 4543           f"SELEC
-000050f0: 5420 4469 7361 626c 6553 7061 7469 616c  T DisableSpatial
-00005100: 496e 6465 7828 277b 6c61 7965 7269 6e66  Index('{layerinf
-00005110: 6f2e 6e61 6d65 7d27 2c20 277b 6c61 7965  o.name}', '{laye
-00005120: 7269 6e66 6f2e 6765 6f6d 6574 7279 636f  rinfo.geometryco
-00005130: 6c75 6d6e 7d27 2922 2c20 2023 206e 6f71  lumn}')",  # noq
-00005140: 613a 2045 3530 310a 2020 2020 2020 2020  a: E501.        
-00005150: 2020 2020 2020 2020 6469 616c 6563 743d          dialect=
-00005160: 2253 514c 4954 4522 2c0a 2020 2020 2020  "SQLITE",.      
-00005170: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00005180: 2020 2020 6461 7461 736f 7572 6365 2e52      datasource.R
-00005190: 656c 6561 7365 5265 7375 6c74 5365 7428  eleaseResultSet(
-000051a0: 7265 7375 6c74 290a 2020 2020 2020 2020  result).        
-000051b0: 656c 6966 2067 656f 6669 6c65 7479 7065  elif geofiletype
-000051c0: 203d 3d20 4765 6f66 696c 6554 7970 652e   == GeofileType.
-000051d0: 4553 5249 5368 6170 6566 696c 653a 0a20  ESRIShapefile:. 
-000051e0: 2020 2020 2020 2020 2020 2023 2044 524f             # DRO
-000051f0: 5020 5350 4154 4941 4c20 494e 4445 5820  P SPATIAL INDEX 
-00005200: 4f4e 202e 2e2e 2063 6f6d 6d61 6e64 2067  ON ... command g
-00005210: 6976 6573 2061 6e20 6572 726f 722c 2073  ives an error, s
-00005220: 6f20 6a75 7374 2072 656d 6f76 6520 2e71  o just remove .q
-00005230: 6978 0a20 2020 2020 2020 2020 2020 2069  ix.            i
-00005240: 6e64 6578 5f70 6174 6820 3d20 7061 7468  ndex_path = path
-00005250: 2e70 6172 656e 7420 2f20 6622 7b70 6174  .parent / f"{pat
-00005260: 682e 7374 656d 7d2e 7169 7822 0a20 2020  h.stem}.qix".   
-00005270: 2020 2020 2020 2020 2069 6e64 6578 5f70           index_p
-00005280: 6174 682e 756e 6c69 6e6b 2829 0a20 2020  ath.unlink().   
-00005290: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000052a0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-000052b0: 6570 7469 6f6e 280a 2020 2020 2020 2020  eption(.        
-000052c0: 2020 2020 2020 2020 6622 7265 6d6f 7665          f"remove
-000052d0: 5f73 7061 7469 616c 5f69 6e64 6578 2069  _spatial_index i
-000052e0: 7320 6e6f 7420 7375 7070 6f72 7465 6420  s not supported 
-000052f0: 666f 7220 7b70 6174 682e 7375 6666 6978  for {path.suffix
-00005300: 7d20 6669 6c65 220a 2020 2020 2020 2020  } file".        
-00005310: 2020 2020 290a 2020 2020 6669 6e61 6c6c      ).    finall
-00005320: 793a 0a20 2020 2020 2020 2069 6620 6461  y:.        if da
-00005330: 7461 736f 7572 6365 2069 7320 6e6f 7420  tasource is not 
-00005340: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00005350: 2020 6465 6c20 6461 7461 736f 7572 6365    del datasource
-00005360: 0a0a 0a64 6566 2072 656e 616d 655f 6c61  ...def rename_la
-00005370: 7965 7228 0a20 2020 2070 6174 683a 2055  yer(.    path: U
-00005380: 6e69 6f6e 5b73 7472 2c20 226f 732e 5061  nion[str, "os.Pa
-00005390: 7468 4c69 6b65 5b41 6e79 5d22 5d2c 206e  thLike[Any]"], n
-000053a0: 6577 5f6c 6179 6572 3a20 7374 722c 206c  ew_layer: str, l
-000053b0: 6179 6572 3a20 4f70 7469 6f6e 616c 5b73  ayer: Optional[s
-000053c0: 7472 5d20 3d20 4e6f 6e65 0a29 3a0a 2020  tr] = None.):.  
-000053d0: 2020 2222 220a 2020 2020 5265 6e61 6d65    """.    Rename
-000053e0: 2074 6865 206c 6179 6572 2073 7065 6369   the layer speci
-000053f0: 6669 6564 2e0a 0a20 2020 2041 7267 733a  fied...    Args:
-00005400: 0a20 2020 2020 2020 2070 6174 6820 2850  .        path (P
-00005410: 6174 684c 696b 6529 3a20 5468 6520 6669  athLike): The fi
-00005420: 6c65 2070 6174 682e 0a20 2020 2020 2020  le path..       
-00005430: 206c 6179 6572 2028 4f70 7469 6f6e 616c   layer (Optional
-00005440: 5b73 7472 5d29 3a20 5468 6520 6c61 7965  [str]): The laye
-00005450: 7220 6e61 6d65 2e20 4966 206e 6f74 2073  r name. If not s
-00005460: 7065 6369 6669 6564 2c20 616e 6420 7468  pecified, and th
-00005470: 6572 6520 6973 206f 6e6c 790a 2020 2020  ere is only.    
-00005480: 2020 2020 2020 2020 6f6e 6520 6c61 7965          one laye
-00005490: 7220 696e 2074 6865 2066 696c 652c 2074  r in the file, t
-000054a0: 6869 7320 6c61 7965 7220 6973 2075 7365  his layer is use
-000054b0: 642e 204f 7468 6572 7769 7365 2065 7863  d. Otherwise exc
-000054c0: 6570 7469 6f6e 2e0a 2020 2020 2020 2020  eption..        
-000054d0: 6e65 775f 6c61 7965 7220 2873 7472 293a  new_layer (str):
-000054e0: 2054 6865 206e 6577 206c 6179 6572 206e   The new layer n
-000054f0: 616d 652e 2049 6620 6e6f 7420 7370 6563  ame. If not spec
-00005500: 6966 6965 642c 2061 6e64 2074 6865 7265  ified, and there
-00005510: 2069 7320 6f6e 6c79 0a20 2020 2020 2020   is only.       
-00005520: 2020 2020 206f 6e65 206c 6179 6572 2069       one layer i
-00005530: 6e20 7468 6520 6669 6c65 2c20 7468 6973  n the file, this
-00005540: 206c 6179 6572 2069 7320 7573 6564 2e20   layer is used. 
-00005550: 4f74 6865 7277 6973 6520 6578 6365 7074  Otherwise except
-00005560: 696f 6e2e 0a20 2020 2022 2222 0a20 2020  ion..    """.   
-00005570: 2023 2043 6865 636b 2069 6e70 7574 2070   # Check input p
-00005580: 6172 616d 6574 6572 730a 2020 2020 7061  arameters.    pa
-00005590: 7468 203d 2050 6174 6828 7061 7468 290a  th = Path(path).
-000055a0: 2020 2020 6966 206c 6179 6572 2069 7320      if layer is 
-000055b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6c61  None:.        la
-000055c0: 7965 7220 3d20 6765 745f 6f6e 6c79 5f6c  yer = get_only_l
-000055d0: 6179 6572 2870 6174 6829 0a0a 2020 2020  ayer(path)..    
-000055e0: 2320 4e6f 7720 7265 616c 6c79 2072 656e  # Now really ren
-000055f0: 616d 650a 2020 2020 6461 7461 736f 7572  ame.    datasour
-00005600: 6365 203d 204e 6f6e 650a 2020 2020 6765  ce = None.    ge
-00005610: 6f66 696c 6574 7970 6520 3d20 4765 6f66  ofiletype = Geof
-00005620: 696c 6554 7970 6528 7061 7468 290a 2020  ileType(path).  
-00005630: 2020 7472 793a 0a20 2020 2020 2020 2069    try:.        i
-00005640: 6620 6765 6f66 696c 6574 7970 652e 6973  f geofiletype.is
-00005650: 5f73 7061 7469 616c 6974 655f 6261 7365  _spatialite_base
-00005660: 643a 0a20 2020 2020 2020 2020 2020 2064  d:.            d
-00005670: 6174 6173 6f75 7263 6520 3d20 6764 616c  atasource = gdal
-00005680: 2e4f 7065 6e45 7828 7374 7228 7061 7468  .OpenEx(str(path
-00005690: 292c 206e 4f70 656e 466c 6167 733d 6764  ), nOpenFlags=gd
-000056a0: 616c 2e4f 465f 5550 4441 5445 290a 2020  al.OF_UPDATE).  
-000056b0: 2020 2020 2020 2020 2020 7371 6c5f 7374            sql_st
-000056c0: 6d74 203d 2066 2741 4c54 4552 2054 4142  mt = f'ALTER TAB
-000056d0: 4c45 2022 7b6c 6179 6572 7d22 2052 454e  LE "{layer}" REN
-000056e0: 414d 4520 544f 2022 7b6e 6577 5f6c 6179  AME TO "{new_lay
-000056f0: 6572 7d22 270a 2020 2020 2020 2020 2020  er}"'.          
-00005700: 2020 7265 7375 6c74 203d 2064 6174 6173    result = datas
-00005710: 6f75 7263 652e 4578 6563 7574 6553 514c  ource.ExecuteSQL
-00005720: 2873 716c 5f73 746d 7429 0a20 2020 2020  (sql_stmt).     
-00005730: 2020 2020 2020 2064 6174 6173 6f75 7263         datasourc
-00005740: 652e 5265 6c65 6173 6552 6573 756c 7453  e.ReleaseResultS
-00005750: 6574 2872 6573 756c 7429 0a20 2020 2020  et(result).     
-00005760: 2020 2065 6c69 6620 6765 6f66 696c 6574     elif geofilet
-00005770: 7970 6520 3d3d 2047 656f 6669 6c65 5479  ype == GeofileTy
-00005780: 7065 2e45 5352 4953 6861 7065 6669 6c65  pe.ESRIShapefile
-00005790: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000057a0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-000057b0: 2272 656e 616d 655f 6c61 7965 7220 6973  "rename_layer is
-000057c0: 206e 6f74 2070 6f73 7369 626c 6520 666f   not possible fo
-000057d0: 7220 7b67 656f 6669 6c65 7479 7065 7d20  r {geofiletype} 
-000057e0: 6669 6c65 2229 0a20 2020 2020 2020 2065  file").        e
-000057f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00005800: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00005810: 7228 6622 7265 6e61 6d65 5f6c 6179 6572  r(f"rename_layer
-00005820: 2069 7320 6e6f 7420 696d 706c 656d 656e   is not implemen
-00005830: 7465 6420 666f 7220 7b70 6174 682e 7375  ted for {path.su
-00005840: 6666 6978 7d20 6669 6c65 2229 0a20 2020  ffix} file").   
-00005850: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-00005860: 2020 6966 2064 6174 6173 6f75 7263 6520    if datasource 
-00005870: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005880: 2020 2020 2020 2020 2064 656c 2064 6174           del dat
-00005890: 6173 6f75 7263 650a 0a0a 6465 6620 7265  asource...def re
-000058a0: 6e61 6d65 5f63 6f6c 756d 6e28 0a20 2020  name_column(.   
-000058b0: 2070 6174 683a 2055 6e69 6f6e 5b73 7472   path: Union[str
-000058c0: 2c20 226f 732e 5061 7468 4c69 6b65 5b41  , "os.PathLike[A
-000058d0: 6e79 5d22 5d2c 0a20 2020 2063 6f6c 756d  ny]"],.    colum
-000058e0: 6e5f 6e61 6d65 3a20 7374 722c 0a20 2020  n_name: str,.   
-000058f0: 206e 6577 5f63 6f6c 756d 6e5f 6e61 6d65   new_column_name
-00005900: 3a20 7374 722c 0a20 2020 206c 6179 6572  : str,.    layer
-00005910: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00005920: 3d20 4e6f 6e65 2c0a 293a 0a20 2020 2022  = None,.):.    "
-00005930: 2222 0a20 2020 2052 656e 616d 6520 7468  "".    Rename th
-00005940: 6520 636f 6c75 6d6e 2073 7065 6369 6669  e column specifi
-00005950: 6564 2e0a 0a20 2020 2041 7267 733a 0a20  ed...    Args:. 
-00005960: 2020 2020 2020 2070 6174 6820 2850 6174         path (Pat
-00005970: 684c 696b 6529 3a20 5468 6520 6669 6c65  hLike): The file
-00005980: 2070 6174 682e 0a20 2020 2020 2020 2063   path..        c
-00005990: 6f6c 756d 6e5f 6e61 6d65 2028 7374 7229  olumn_name (str)
-000059a0: 3a20 7468 6520 6375 7272 656e 7420 636f  : the current co
-000059b0: 6c75 6d6e 206e 616d 652e 0a20 2020 2020  lumn name..     
-000059c0: 2020 206e 6577 5f63 6f6c 756d 6e5f 6e61     new_column_na
-000059d0: 6d65 2028 7374 7229 3a20 7468 6520 6e65  me (str): the ne
-000059e0: 7720 636f 6c75 6d6e 206e 616d 652e 0a20  w column name.. 
-000059f0: 2020 2020 2020 206c 6179 6572 2028 4f70         layer (Op
-00005a00: 7469 6f6e 616c 5b73 7472 5d29 3a20 5468  tional[str]): Th
-00005a10: 6520 6c61 7965 7220 6e61 6d65 2e20 4966  e layer name. If
-00005a20: 206e 6f74 2073 7065 6369 6669 6564 2c20   not specified, 
-00005a30: 616e 6420 7468 6572 6520 6973 206f 6e6c  and there is onl
-00005a40: 790a 2020 2020 2020 2020 2020 2020 6f6e  y.            on
-00005a50: 6520 6c61 7965 7220 696e 2074 6865 2066  e layer in the f
-00005a60: 696c 652c 2074 6869 7320 6c61 7965 7220  ile, this layer 
-00005a70: 6973 2075 7365 642e 204f 7468 6572 7769  is used. Otherwi
-00005a80: 7365 2065 7863 6570 7469 6f6e 2e0a 2020  se exception..  
-00005a90: 2020 2222 220a 2020 2020 2320 4368 6563    """.    # Chec
-00005aa0: 6b20 696e 7075 7420 7061 7261 6d65 7465  k input paramete
-00005ab0: 7273 0a20 2020 2070 6174 6820 3d20 5061  rs.    path = Pa
-00005ac0: 7468 2870 6174 6829 0a20 2020 2069 6620  th(path).    if 
-00005ad0: 6c61 7965 7220 6973 204e 6f6e 653a 0a20  layer is None:. 
-00005ae0: 2020 2020 2020 206c 6179 6572 203d 2067         layer = g
-00005af0: 6574 5f6f 6e6c 795f 6c61 7965 7228 7061  et_only_layer(pa
-00005b00: 7468 290a 2020 2020 696e 666f 203d 2067  th).    info = g
-00005b10: 6574 5f6c 6179 6572 696e 666f 2870 6174  et_layerinfo(pat
-00005b20: 6829 0a20 2020 2069 6620 636f 6c75 6d6e  h).    if column
-00005b30: 5f6e 616d 6520 6e6f 7420 696e 2069 6e66  _name not in inf
-00005b40: 6f2e 636f 6c75 6d6e 7320 616e 6420 6e65  o.columns and ne
-00005b50: 775f 636f 6c75 6d6e 5f6e 616d 6520 696e  w_column_name in
-00005b60: 2069 6e66 6f2e 636f 6c75 6d6e 733a 0a20   info.columns:. 
-00005b70: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00005b80: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
-00005b90: 6622 436f 6c75 6d6e 207b 636f 6c75 6d6e  f"Column {column
-00005ba0: 5f6e 616d 657d 2073 6565 6d73 2074 6f20  _name} seems to 
-00005bb0: 6265 2072 656e 616d 6564 2061 6c72 6561  be renamed alrea
-00005bc0: 6479 2074 6f20 7b6e 6577 5f63 6f6c 756d  dy to {new_colum
-00005bd0: 6e5f 6e61 6d65 7d22 0a20 2020 2020 2020  n_name}".       
-00005be0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00005bf0: 6e0a 0a20 2020 2023 204e 6f77 2072 6561  n..    # Now rea
-00005c00: 6c6c 7920 7265 6e61 6d65 0a20 2020 2064  lly rename.    d
-00005c10: 6174 6173 6f75 7263 6520 3d20 4e6f 6e65  atasource = None
-00005c20: 0a20 2020 2067 656f 6669 6c65 7479 7065  .    geofiletype
-00005c30: 203d 2047 656f 6669 6c65 5479 7065 2870   = GeofileType(p
-00005c40: 6174 6829 0a20 2020 2074 7279 3a0a 2020  ath).    try:.  
-00005c50: 2020 2020 2020 6966 2067 656f 6669 6c65        if geofile
-00005c60: 7479 7065 2e69 735f 7370 6174 6961 6c69  type.is_spatiali
-00005c70: 7465 5f62 6173 6564 3a0a 2020 2020 2020  te_based:.      
-00005c80: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
-00005c90: 203d 2067 6461 6c2e 4f70 656e 4578 2873   = gdal.OpenEx(s
-00005ca0: 7472 2870 6174 6829 2c20 6e4f 7065 6e46  tr(path), nOpenF
-00005cb0: 6c61 6773 3d67 6461 6c2e 4f46 5f55 5044  lags=gdal.OF_UPD
-00005cc0: 4154 4529 0a20 2020 2020 2020 2020 2020  ATE).           
-00005cd0: 2073 716c 5f73 746d 7420 3d20 280a 2020   sql_stmt = (.  
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00005cf0: 414c 5445 5220 5441 424c 4520 227b 6c61  ALTER TABLE "{la
-00005d00: 7965 727d 2220 270a 2020 2020 2020 2020  yer}" '.        
-00005d10: 2020 2020 2020 2020 6627 5245 4e41 4d45          f'RENAME
-00005d20: 2043 4f4c 554d 4e20 227b 636f 6c75 6d6e   COLUMN "{column
-00005d30: 5f6e 616d 657d 2220 544f 2022 7b6e 6577  _name}" TO "{new
-00005d40: 5f63 6f6c 756d 6e5f 6e61 6d65 7d22 270a  _column_name}"'.
-00005d50: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00005d60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00005d70: 203d 2064 6174 6173 6f75 7263 652e 4578   = datasource.Ex
-00005d80: 6563 7574 6553 514c 2873 716c 5f73 746d  ecuteSQL(sql_stm
-00005d90: 7429 0a20 2020 2020 2020 2020 2020 2064  t).            d
-00005da0: 6174 6173 6f75 7263 652e 5265 6c65 6173  atasource.Releas
-00005db0: 6552 6573 756c 7453 6574 2872 6573 756c  eResultSet(resul
-00005dc0: 7429 0a20 2020 2020 2020 2065 6c69 6620  t).        elif 
-00005dd0: 6765 6f66 696c 6574 7970 6520 3d3d 2047  geofiletype == G
-00005de0: 656f 6669 6c65 5479 7065 2e45 5352 4953  eofileType.ESRIS
-00005df0: 6861 7065 6669 6c65 3a0a 2020 2020 2020  hapefile:.      
-00005e00: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00005e10: 6545 7272 6f72 2866 2272 656e 616d 655f  eError(f"rename_
-00005e20: 636f 6c75 6d6e 2069 7320 6e6f 7420 706f  column is not po
-00005e30: 7373 6962 6c65 2066 6f72 207b 6765 6f66  ssible for {geof
-00005e40: 696c 6574 7970 657d 2066 696c 6522 290a  iletype} file").
-00005e50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00005e60: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00005e70: 5661 6c75 6545 7272 6f72 2866 2272 656e  ValueError(f"ren
-00005e80: 616d 655f 636f 6c75 6d6e 2069 7320 6e6f  ame_column is no
-00005e90: 7420 696d 706c 656d 656e 7465 6420 666f  t implemented fo
-00005ea0: 7220 7b70 6174 682e 7375 6666 6978 7d20  r {path.suffix} 
-00005eb0: 6669 6c65 2229 0a20 2020 2066 696e 616c  file").    final
-00005ec0: 6c79 3a0a 2020 2020 2020 2020 6966 2064  ly:.        if d
-00005ed0: 6174 6173 6f75 7263 6520 6973 206e 6f74  atasource is not
-00005ee0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00005ef0: 2020 2064 656c 2064 6174 6173 6f75 7263     del datasourc
-00005f00: 650a 0a0a 636c 6173 7320 4461 7461 5479  e...class DataTy
-00005f10: 7065 2865 6e75 6d2e 456e 756d 293a 0a20  pe(enum.Enum):. 
-00005f20: 2020 2022 2222 0a20 2020 2054 6869 7320     """.    This 
-00005f30: 656e 756d 2064 6566 696e 6573 2074 6865  enum defines the
-00005f40: 2073 7461 6e64 6172 6420 6461 7461 2074   standard data t
-00005f50: 7970 6573 2074 6861 7420 6361 6e20 6265  ypes that can be
-00005f60: 2075 7365 6420 666f 7220 636f 6c75 6d6e   used for column
-00005f70: 732e 0a20 2020 2022 2222 0a0a 2020 2020  s..    """..    
-00005f80: 5445 5854 203d 2022 5445 5854 220a 2020  TEXT = "TEXT".  
-00005f90: 2020 2222 2243 6f6c 756d 6e20 7769 7468    """Column with
-00005fa0: 2074 6578 7420 6461 7461 3a20 7e20 7374   text data: ~ st
-00005fb0: 7269 6e67 2c20 6368 6172 2c20 7661 7263  ring, char, varc
-00005fc0: 6861 722c 2063 6c6f 622e 2222 220a 2020  har, clob.""".  
-00005fd0: 2020 494e 5445 4745 5220 3d20 2249 4e54    INTEGER = "INT
-00005fe0: 4547 4552 220a 2020 2020 2222 2243 6f6c  EGER".    """Col
-00005ff0: 756d 6e20 7769 7468 2069 6e74 6567 6572  umn with integer
-00006000: 2064 6174 612e 2222 220a 2020 2020 5245   data.""".    RE
-00006010: 414c 203d 2022 5245 414c 220a 2020 2020  AL = "REAL".    
-00006020: 2222 2243 6f6c 756d 6e20 7769 7468 2066  """Column with f
-00006030: 6c6f 6174 696e 6720 706f 696e 7420 6461  loating point da
-00006040: 7461 3a20 7e20 666c 6f61 742c 2064 6f75  ta: ~ float, dou
-00006050: 626c 652e 2222 220a 2020 2020 4441 5445  ble.""".    DATE
-00006060: 203d 2022 4441 5445 220a 2020 2020 2222   = "DATE".    ""
-00006070: 2243 6f6c 756d 6e20 7769 7468 2064 6174  "Column with dat
-00006080: 6520 6461 7461 2e22 2222 0a20 2020 2054  e data.""".    T
-00006090: 494d 4553 5441 4d50 203d 2022 5449 4d45  IMESTAMP = "TIME
-000060a0: 5354 414d 5022 0a20 2020 2022 2222 436f  STAMP".    """Co
-000060b0: 6c75 6d6e 2077 6974 6820 7469 6d65 7374  lumn with timest
-000060c0: 616d 7020 6461 7461 3a20 7e20 6461 7465  amp data: ~ date
-000060d0: 7469 6d65 2e22 2222 0a20 2020 2042 4f4f  time.""".    BOO
-000060e0: 4c45 414e 203d 2022 424f 4f4c 4541 4e22  LEAN = "BOOLEAN"
-000060f0: 0a20 2020 2022 2222 436f 6c75 6d6e 2077  .    """Column w
-00006100: 6974 6820 626f 6f6c 6561 6e20 6461 7461  ith boolean data
-00006110: 2e22 2222 0a20 2020 2042 4c4f 4220 3d20  .""".    BLOB = 
-00006120: 2242 4c4f 4222 0a20 2020 2022 2222 436f  "BLOB".    """Co
-00006130: 6c75 6d6e 2077 6974 6820 6269 6e61 7279  lumn with binary
-00006140: 2064 6174 612e 2222 220a 2020 2020 4e55   data.""".    NU
-00006150: 4d45 5249 4320 3d20 224e 554d 4552 4943  MERIC = "NUMERIC
-00006160: 220a 2020 2020 2222 2243 6f6c 756d 6e20  ".    """Column 
-00006170: 7769 7468 206e 756d 6572 6963 2064 6174  with numeric dat
-00006180: 613a 2065 7861 6374 2064 6563 696d 616c  a: exact decimal
-00006190: 2064 6174 612e 2222 220a 0a0a 6465 6620   data."""...def 
-000061a0: 6164 645f 636f 6c75 6d6e 280a 2020 2020  add_column(.    
-000061b0: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
-000061c0: 2022 6f73 2e50 6174 684c 696b 655b 416e   "os.PathLike[An
-000061d0: 795d 225d 2c0a 2020 2020 6e61 6d65 3a20  y]"],.    name: 
-000061e0: 7374 722c 0a20 2020 2074 7970 653a 2055  str,.    type: U
-000061f0: 6e69 6f6e 5b44 6174 6154 7970 652c 2073  nion[DataType, s
-00006200: 7472 5d2c 0a20 2020 2065 7870 7265 7373  tr],.    express
-00006210: 696f 6e3a 2055 6e69 6f6e 5b73 7472 2c20  ion: Union[str, 
-00006220: 696e 742c 2066 6c6f 6174 2c20 4e6f 6e65  int, float, None
-00006230: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6578  ] = None,.    ex
-00006240: 7072 6573 7369 6f6e 5f64 6961 6c65 6374  pression_dialect
-00006250: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00006260: 3d20 4e6f 6e65 2c0a 2020 2020 6c61 7965  = None,.    laye
-00006270: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
-00006280: 203d 204e 6f6e 652c 0a20 2020 2066 6f72   = None,.    for
-00006290: 6365 5f75 7064 6174 653a 2062 6f6f 6c20  ce_update: bool 
-000062a0: 3d20 4661 6c73 652c 0a20 2020 2077 6964  = False,.    wid
-000062b0: 7468 3a20 4f70 7469 6f6e 616c 5b69 6e74  th: Optional[int
-000062c0: 5d20 3d20 4e6f 6e65 2c0a 293a 0a20 2020  ] = None,.):.   
-000062d0: 2022 2222 0a20 2020 2041 6464 2061 2063   """.    Add a c
-000062e0: 6f6c 756d 6e20 746f 2061 206c 6179 6572  olumn to a layer
-000062f0: 206f 6620 7468 6520 6765 6f66 696c 652e   of the geofile.
-00006300: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00006310: 2020 2020 7061 7468 2028 5061 7468 4c69      path (PathLi
-00006320: 6b65 293a 2050 6174 6820 746f 2074 6865  ke): Path to the
-00006330: 2067 656f 6669 6c65 2e0a 2020 2020 2020   geofile..      
-00006340: 2020 6e61 6d65 2028 7374 7229 3a20 4e61    name (str): Na
-00006350: 6d65 2066 6f72 2074 6865 206e 6577 2063  me for the new c
-00006360: 6f6c 756d 6e2e 0a20 2020 2020 2020 2074  olumn..        t
-00006370: 7970 6520 2873 7472 293a 2043 6f6c 756d  ype (str): Colum
-00006380: 6e20 7479 7065 206f 6620 7468 6520 6e65  n type of the ne
-00006390: 7720 636f 6c75 6d6e 2e0a 2020 2020 2020  w column..      
-000063a0: 2020 6578 7072 6573 7369 6f6e 2028 7374    expression (st
-000063b0: 722c 206f 7074 696f 6e61 6c29 3a20 5351  r, optional): SQ
-000063c0: 4c69 7465 2065 7870 7265 7373 696f 6e20  Lite expression 
-000063d0: 746f 2075 7365 2074 6f20 7570 6461 7465  to use to update
-000063e0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-000063f0: 2076 616c 7565 2e20 4465 6661 756c 7473   value. Defaults
-00006400: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
-00006410: 2020 6578 7072 6573 7369 6f6e 5f64 6961    expression_dia
-00006420: 6c65 6374 2028 7374 722c 206f 7074 696f  lect (str, optio
-00006430: 6e61 6c29 3a20 5351 4c20 6469 616c 6563  nal): SQL dialec
-00006440: 7420 7573 6564 2066 6f72 2074 6865 2065  t used for the e
-00006450: 7870 7265 7373 696f 6e2e 0a20 2020 2020  xpression..     
-00006460: 2020 206c 6179 6572 2028 7374 722c 206f     layer (str, o
-00006470: 7074 696f 6e61 6c29 3a20 5468 6520 6c61  ptional): The la
-00006480: 7965 7220 6e61 6d65 2e20 4966 204e 6f6e  yer name. If Non
-00006490: 6520 616e 6420 7468 6520 6765 6f66 696c  e and the geofil
-000064a0: 650a 2020 2020 2020 2020 2020 2020 6861  e.            ha
-000064b0: 7320 6f6e 6c79 206f 6e65 206c 6179 6572  s only one layer
-000064c0: 2c20 7468 6174 206c 6179 6572 2069 7320  , that layer is 
-000064d0: 7573 6564 2e20 4465 6661 756c 7473 2074  used. Defaults t
-000064e0: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-000064f0: 666f 7263 655f 7570 6461 7465 2028 626f  force_update (bo
-00006500: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2049  ol, optional): I
-00006510: 6620 7468 6520 636f 6c75 6d6e 2061 6c72  f the column alr
-00006520: 6561 6479 2065 7869 7374 732c 2065 7865  eady exists, exe
-00006530: 6375 7465 0a20 2020 2020 2020 2020 2020  cute.           
-00006540: 2074 6865 2075 7064 6174 6520 616e 7977   the update anyw
-00006550: 6179 2e20 4465 6661 756c 7473 2074 6f20  ay. Defaults to 
-00006560: 4661 6c73 652e 0a20 2020 2020 2020 2077  False..        w
-00006570: 6964 7468 2028 696e 742c 206f 7074 696f  idth (int, optio
-00006580: 6e61 6c29 3a20 7468 6520 7769 6474 6820  nal): the width 
-00006590: 6f66 2074 6865 2066 6965 6c64 2e0a 0a20  of the field... 
-000065a0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-000065b0: 2020 2065 783a 205b 6465 7363 7269 7074     ex: [descript
-000065c0: 696f 6e5d 0a20 2020 2022 2222 0a20 2020  ion].    """.   
-000065d0: 2023 2049 6e69 740a 2020 2020 6966 2069   # Init.    if i
-000065e0: 7369 6e73 7461 6e63 6528 7479 7065 2c20  sinstance(type, 
-000065f0: 4461 7461 5479 7065 293a 0a20 2020 2020  DataType):.     
-00006600: 2020 2074 7970 655f 7374 7220 3d20 7479     type_str = ty
-00006610: 7065 2e76 616c 7565 0a20 2020 2065 6c73  pe.value.    els
-00006620: 653a 0a20 2020 2020 2020 2074 7970 655f  e:.        type_
-00006630: 6c6f 7765 7220 3d20 7479 7065 2e6c 6f77  lower = type.low
-00006640: 6572 2829 0a20 2020 2020 2020 2069 6620  er().        if 
-00006650: 7479 7065 5f6c 6f77 6572 203d 3d20 2273  type_lower == "s
-00006660: 7472 696e 6722 3a0a 2020 2020 2020 2020  tring":.        
-00006670: 2020 2020 2320 544f 444f 3a20 7468 696e      # TODO: thin
-00006680: 6b20 7768 6574 6865 7220 6265 696e 6720  k whether being 
-00006690: 666c 6578 6962 6c65 2068 6572 6520 6973  flexible here is
-000066a0: 2061 2067 6f6f 6420 6964 6561 2e2e 2e0a   a good idea....
-000066b0: 2020 2020 2020 2020 2020 2020 7479 7065              type
-000066c0: 5f73 7472 203d 2022 5445 5854 220a 2020  _str = "TEXT".  
-000066d0: 2020 2020 2020 656c 6966 2074 7970 655f        elif type_
-000066e0: 6c6f 7765 7220 3d3d 2022 6269 6e61 7279  lower == "binary
-000066f0: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
-00006700: 7970 655f 7374 7220 3d20 2242 4c4f 4222  ype_str = "BLOB"
-00006710: 0a20 2020 2020 2020 2065 6c69 6620 7479  .        elif ty
-00006720: 7065 5f6c 6f77 6572 203d 3d20 2274 696d  pe_lower == "tim
-00006730: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
-00006740: 7479 7065 5f73 7472 203d 2022 4441 5445  type_str = "DATE
-00006750: 5449 4d45 220a 2020 2020 2020 2020 656c  TIME".        el
-00006760: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00006770: 7479 7065 5f73 7472 203d 2074 7970 650a  type_str = type.
-00006780: 2020 2020 7061 7468 203d 2050 6174 6828      path = Path(
-00006790: 7061 7468 290a 2020 2020 6966 206c 6179  path).    if lay
-000067a0: 6572 2069 7320 4e6f 6e65 3a0a 2020 2020  er is None:.    
-000067b0: 2020 2020 6c61 7965 7220 3d20 6765 745f      layer = get_
-000067c0: 6f6e 6c79 5f6c 6179 6572 2870 6174 6829  only_layer(path)
-000067d0: 0a20 2020 206c 6179 6572 696e 666f 5f6f  .    layerinfo_o
-000067e0: 7269 6720 3d20 6765 745f 6c61 7965 7269  rig = get_layeri
-000067f0: 6e66 6f28 7061 7468 2c20 6c61 7965 7229  nfo(path, layer)
-00006800: 0a0a 2020 2020 2320 476f 210a 2020 2020  ..    # Go!.    
-00006810: 6461 7461 736f 7572 6365 203d 204e 6f6e  datasource = Non
-00006820: 650a 2020 2020 7472 793a 0a20 2020 2020  e.    try:.     
-00006830: 2020 2023 2049 6620 636f 6c75 6d6e 2064     # If column d
-00006840: 6f65 736e 2774 2065 7869 7374 2079 6574  oesn't exist yet
-00006850: 2c20 6372 6561 7465 2069 740a 2020 2020  , create it.    
-00006860: 2020 2020 636f 6c75 6d6e 735f 7570 7065      columns_uppe
-00006870: 7220 3d20 5b63 6f6c 756d 6e2e 7570 7065  r = [column.uppe
-00006880: 7228 2920 666f 7220 636f 6c75 6d6e 2069  r() for column i
-00006890: 6e20 6c61 7965 7269 6e66 6f5f 6f72 6967  n layerinfo_orig
-000068a0: 2e63 6f6c 756d 6e73 5d0a 2020 2020 2020  .columns].      
-000068b0: 2020 6966 206e 616d 652e 7570 7065 7228    if name.upper(
-000068c0: 2920 6e6f 7420 696e 2063 6f6c 756d 6e73  ) not in columns
-000068d0: 5f75 7070 6572 3a0a 2020 2020 2020 2020  _upper:.        
-000068e0: 2020 2020 7769 6474 685f 7374 7220 3d20      width_str = 
-000068f0: 6622 287b 7769 6474 687d 2922 2069 6620  f"({width})" if 
-00006900: 7769 6474 6820 6973 206e 6f74 204e 6f6e  width is not Non
-00006910: 6520 656c 7365 2022 220a 2020 2020 2020  e else "".      
-00006920: 2020 2020 2020 7371 6c5f 7374 6d74 203d        sql_stmt =
-00006930: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00006940: 2020 2066 2741 4c54 4552 2054 4142 4c45     f'ALTER TABLE
-00006950: 2022 7b6c 6179 6572 7d22 2041 4444 2043   "{layer}" ADD C
-00006960: 4f4c 554d 4e20 227b 6e61 6d65 7d22 207b  OLUMN "{name}" {
-00006970: 7479 7065 5f73 7472 7d7b 7769 6474 685f  type_str}{width_
-00006980: 7374 727d 270a 2020 2020 2020 2020 2020  str}'.          
-00006990: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000069a0: 6461 7461 736f 7572 6365 203d 2067 6461  datasource = gda
-000069b0: 6c2e 4f70 656e 4578 2873 7472 2870 6174  l.OpenEx(str(pat
-000069c0: 6829 2c20 6e4f 7065 6e46 6c61 6773 3d67  h), nOpenFlags=g
-000069d0: 6461 6c2e 4f46 5f55 5044 4154 4529 0a20  dal.OF_UPDATE). 
-000069e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000069f0: 7420 3d20 6461 7461 736f 7572 6365 2e45  t = datasource.E
-00006a00: 7865 6375 7465 5351 4c28 7371 6c5f 7374  xecuteSQL(sql_st
-00006a10: 6d74 290a 2020 2020 2020 2020 2020 2020  mt).            
-00006a20: 6461 7461 736f 7572 6365 2e52 656c 6561  datasource.Relea
-00006a30: 7365 5265 7375 6c74 5365 7428 7265 7375  seResultSet(resu
-00006a40: 6c74 290a 2020 2020 2020 2020 656c 7365  lt).        else
-00006a50: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00006a60: 6767 6572 2e77 6172 6e69 6e67 2866 2243  gger.warning(f"C
-00006a70: 6f6c 756d 6e20 7b6e 616d 657d 2065 7869  olumn {name} exi
-00006a80: 7374 6564 2061 6c72 6561 6479 2069 6e20  sted already in 
-00006a90: 7b70 6174 687d 2c20 6c61 7965 7220 7b6c  {path}, layer {l
-00006aa0: 6179 6572 7d22 290a 0a20 2020 2020 2020  ayer}")..       
-00006ab0: 2023 2049 6620 616e 2065 7870 7265 7373   # If an express
-00006ac0: 696f 6e20 7761 7320 7072 6f76 6964 6564  ion was provided
-00006ad0: 2061 6e64 2075 7064 6174 6520 6361 6e20   and update can 
-00006ae0: 6265 2064 6f6e 652c 2067 6f20 666f 7220  be done, go for 
-00006af0: 6974 2e2e 2e0a 2020 2020 2020 2020 6966  it....        if
-00006b00: 2065 7870 7265 7373 696f 6e20 6973 206e   expression is n
-00006b10: 6f74 204e 6f6e 6520 616e 6420 280a 2020  ot None and (.  
-00006b20: 2020 2020 2020 2020 2020 6e61 6d65 206e            name n
-00006b30: 6f74 2069 6e20 6c61 7965 7269 6e66 6f5f  ot in layerinfo_
-00006b40: 6f72 6967 2e63 6f6c 756d 6e73 206f 7220  orig.columns or 
-00006b50: 666f 7263 655f 7570 6461 7465 2069 7320  force_update is 
-00006b60: 5472 7565 0a20 2020 2020 2020 2029 3a0a  True.        ):.
-00006b70: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00006b80: 6174 6173 6f75 7263 6520 6973 204e 6f6e  atasource is Non
-00006b90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00006ba0: 2020 2064 6174 6173 6f75 7263 6520 3d20     datasource = 
-00006bb0: 6764 616c 2e4f 7065 6e45 7828 7374 7228  gdal.OpenEx(str(
-00006bc0: 7061 7468 292c 206e 4f70 656e 466c 6167  path), nOpenFlag
-00006bd0: 733d 6764 616c 2e4f 465f 5550 4441 5445  s=gdal.OF_UPDATE
-00006be0: 290a 2020 2020 2020 2020 2020 2020 7371  ).            sq
-00006bf0: 6c5f 7374 6d74 203d 2066 2755 5044 4154  l_stmt = f'UPDAT
-00006c00: 4520 227b 6c61 7965 727d 2220 5345 5420  E "{layer}" SET 
-00006c10: 227b 6e61 6d65 7d22 203d 207b 6578 7072  "{name}" = {expr
-00006c20: 6573 7369 6f6e 7d27 0a20 2020 2020 2020  ession}'.       
-00006c30: 2020 2020 2072 6573 756c 7420 3d20 6461       result = da
-00006c40: 7461 736f 7572 6365 2e45 7865 6375 7465  tasource.Execute
-00006c50: 5351 4c28 7371 6c5f 7374 6d74 2c20 6469  SQL(sql_stmt, di
-00006c60: 616c 6563 743d 6578 7072 6573 7369 6f6e  alect=expression
-00006c70: 5f64 6961 6c65 6374 290a 2020 2020 2020  _dialect).      
-00006c80: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
-00006c90: 2e52 656c 6561 7365 5265 7375 6c74 5365  .ReleaseResultSe
-00006ca0: 7428 7265 7375 6c74 290a 2020 2020 6669  t(result).    fi
-00006cb0: 6e61 6c6c 793a 0a20 2020 2020 2020 2069  nally:.        i
-00006cc0: 6620 6461 7461 736f 7572 6365 2069 7320  f datasource is 
-00006cd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00006ce0: 2020 2020 2020 6465 6c20 6461 7461 736f        del dataso
-00006cf0: 7572 6365 0a0a 0a64 6566 2064 726f 705f  urce...def drop_
-00006d00: 636f 6c75 6d6e 280a 2020 2020 7061 7468  column(.    path
-00006d10: 3a20 556e 696f 6e5b 7374 722c 2022 6f73  : Union[str, "os
-00006d20: 2e50 6174 684c 696b 655b 416e 795d 225d  .PathLike[Any]"]
-00006d30: 2c20 636f 6c75 6d6e 5f6e 616d 653a 2073  , column_name: s
-00006d40: 7472 2c20 6c61 7965 723a 204f 7074 696f  tr, layer: Optio
-00006d50: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00006d60: 293a 0a20 2020 2022 2222 0a20 2020 2044  ):.    """.    D
-00006d70: 726f 7020 7468 6520 636f 6c75 6d6e 2073  rop the column s
-00006d80: 7065 6369 6669 6564 2e0a 0a20 2020 2041  pecified...    A
-00006d90: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
-00006da0: 6820 2850 6174 684c 696b 6529 3a20 5468  h (PathLike): Th
-00006db0: 6520 6669 6c65 2070 6174 682e 0a20 2020  e file path..   
-00006dc0: 2020 2020 2063 6f6c 756d 6e5f 6e61 6d65       column_name
-00006dd0: 2028 7374 7229 3a20 7468 6520 636f 6c75   (str): the colu
-00006de0: 6d6e 206e 616d 652e 0a20 2020 2020 2020  mn name..       
-00006df0: 206c 6179 6572 2028 4f70 7469 6f6e 616c   layer (Optional
-00006e00: 5b73 7472 5d29 3a20 5468 6520 6c61 7965  [str]): The laye
-00006e10: 7220 6e61 6d65 2e20 4966 206e 6f74 2073  r name. If not s
-00006e20: 7065 6369 6669 6564 2c20 616e 6420 7468  pecified, and th
-00006e30: 6572 6520 6973 206f 6e6c 790a 2020 2020  ere is only.    
-00006e40: 2020 2020 2020 2020 6f6e 6520 6c61 7965          one laye
-00006e50: 7220 696e 2074 6865 2066 696c 652c 2074  r in the file, t
-00006e60: 6869 7320 6c61 7965 7220 6973 2075 7365  his layer is use
-00006e70: 642e 204f 7468 6572 7769 7365 2061 2056  d. Otherwise a V
-00006e80: 616c 7565 4572 726f 7220 6973 0a20 2020  alueError is.   
-00006e90: 2020 2020 2020 2020 2072 6169 7365 642e           raised.
-00006ea0: 0a20 2020 2022 2222 0a20 2020 2023 2043  .    """.    # C
-00006eb0: 6865 636b 2069 6e70 7574 2070 6172 616d  heck input param
-00006ec0: 6574 6572 730a 2020 2020 7061 7468 203d  eters.    path =
-00006ed0: 2050 6174 6828 7061 7468 290a 2020 2020   Path(path).    
-00006ee0: 6966 206c 6179 6572 2069 7320 4e6f 6e65  if layer is None
-00006ef0: 3a0a 2020 2020 2020 2020 6c61 7965 7220  :.        layer 
-00006f00: 3d20 6765 745f 6f6e 6c79 5f6c 6179 6572  = get_only_layer
-00006f10: 2870 6174 6829 0a20 2020 2069 6e66 6f20  (path).    info 
-00006f20: 3d20 6765 745f 6c61 7965 7269 6e66 6f28  = get_layerinfo(
-00006f30: 7061 7468 2c20 6c61 7965 7229 0a20 2020  path, layer).   
-00006f40: 2069 6620 636f 6c75 6d6e 5f6e 616d 6520   if column_name 
-00006f50: 6e6f 7420 696e 2069 6e66 6f2e 636f 6c75  not in info.colu
-00006f60: 6d6e 733a 0a20 2020 2020 2020 206c 6f67  mns:.        log
-00006f70: 6765 722e 696e 666f 2866 2243 6f6c 756d  ger.info(f"Colum
-00006f80: 6e20 7b63 6f6c 756d 6e5f 6e61 6d65 7d20  n {column_name} 
-00006f90: 6e6f 7420 7072 6573 656e 7420 736f 2063  not present so c
-00006fa0: 616e 6e6f 7420 6265 2064 726f 7070 6564  annot be dropped
-00006fb0: 2e22 290a 2020 2020 2020 2020 7265 7475  .").        retu
-00006fc0: 726e 0a0a 2020 2020 2320 4e6f 7720 7265  rn..    # Now re
-00006fd0: 616c 6c79 2072 656e 616d 650a 2020 2020  ally rename.    
-00006fe0: 6461 7461 736f 7572 6365 203d 204e 6f6e  datasource = Non
-00006ff0: 650a 2020 2020 7472 793a 0a20 2020 2020  e.    try:.     
-00007000: 2020 2064 6174 6173 6f75 7263 6520 3d20     datasource = 
-00007010: 6764 616c 2e4f 7065 6e45 7828 7374 7228  gdal.OpenEx(str(
-00007020: 7061 7468 292c 206e 4f70 656e 466c 6167  path), nOpenFlag
-00007030: 733d 6764 616c 2e4f 465f 5550 4441 5445  s=gdal.OF_UPDATE
-00007040: 290a 2020 2020 2020 2020 7371 6c5f 7374  ).        sql_st
-00007050: 6d74 203d 2066 2741 4c54 4552 2054 4142  mt = f'ALTER TAB
-00007060: 4c45 2022 7b6c 6179 6572 7d22 2044 524f  LE "{layer}" DRO
-00007070: 5020 434f 4c55 4d4e 2022 7b63 6f6c 756d  P COLUMN "{colum
-00007080: 6e5f 6e61 6d65 7d22 270a 2020 2020 2020  n_name}"'.      
-00007090: 2020 7265 7375 6c74 203d 2064 6174 6173    result = datas
-000070a0: 6f75 7263 652e 4578 6563 7574 6553 514c  ource.ExecuteSQL
-000070b0: 2873 716c 5f73 746d 7429 0a20 2020 2020  (sql_stmt).     
-000070c0: 2020 2064 6174 6173 6f75 7263 652e 5265     datasource.Re
-000070d0: 6c65 6173 6552 6573 756c 7453 6574 2872  leaseResultSet(r
-000070e0: 6573 756c 7429 0a20 2020 2066 696e 616c  esult).    final
-000070f0: 6c79 3a0a 2020 2020 2020 2020 6966 2064  ly:.        if d
-00007100: 6174 6173 6f75 7263 6520 6973 206e 6f74  atasource is not
-00007110: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007120: 2020 2064 656c 2064 6174 6173 6f75 7263     del datasourc
-00007130: 650a 0a0a 6465 6620 7570 6461 7465 5f63  e...def update_c
-00007140: 6f6c 756d 6e28 0a20 2020 2070 6174 683a  olumn(.    path:
-00007150: 2055 6e69 6f6e 5b73 7472 2c20 226f 732e   Union[str, "os.
-00007160: 5061 7468 4c69 6b65 5b41 6e79 5d22 5d2c  PathLike[Any]"],
-00007170: 0a20 2020 206e 616d 653a 2073 7472 2c0a  .    name: str,.
-00007180: 2020 2020 6578 7072 6573 7369 6f6e 3a20      expression: 
-00007190: 7374 722c 0a20 2020 206c 6179 6572 3a20  str,.    layer: 
-000071a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000071b0: 4e6f 6e65 2c0a 2020 2020 7768 6572 653a  None,.    where:
-000071c0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-000071d0: 204e 6f6e 652c 0a29 3a0a 2020 2020 2222   None,.):.    ""
-000071e0: 220a 2020 2020 5570 6461 7465 2061 2063  ".    Update a c
-000071f0: 6f6c 756d 6e20 6672 6f6d 2061 206c 6179  olumn from a lay
-00007200: 6572 206f 6620 7468 6520 6765 6f66 696c  er of the geofil
-00007210: 652e 0a0a 2020 2020 4172 6773 3a0a 2020  e...    Args:.  
-00007220: 2020 2020 2020 7061 7468 2028 5061 7468        path (Path
-00007230: 4c69 6b65 293a 2050 6174 6820 746f 2074  Like): Path to t
-00007240: 6865 2067 656f 6669 6c65 0a20 2020 2020  he geofile.     
-00007250: 2020 206e 616d 6520 2873 7472 293a 204e     name (str): N
-00007260: 616d 6520 666f 7220 7468 6520 6e65 7720  ame for the new 
-00007270: 636f 6c75 6d6e 0a20 2020 2020 2020 2065  column.        e
-00007280: 7870 7265 7373 696f 6e20 2873 7472 293a  xpression (str):
-00007290: 2053 514c 6974 6520 6578 7072 6573 7369   SQLite expressi
-000072a0: 6f6e 2074 6f20 7573 6520 746f 2075 7064  on to use to upd
-000072b0: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
-000072c0: 7468 6520 7661 6c75 652e 0a20 2020 2020  the value..     
-000072d0: 2020 206c 6179 6572 2028 7374 722c 206f     layer (str, o
-000072e0: 7074 696f 6e61 6c29 3a20 5468 6520 6c61  ptional): The la
-000072f0: 7965 7220 6e61 6d65 2e20 4966 204e 6f6e  yer name. If Non
-00007300: 6520 616e 6420 7468 6520 6765 6f66 696c  e and the geofil
-00007310: 650a 2020 2020 2020 2020 2020 2020 6861  e.            ha
-00007320: 7320 6f6e 6c79 206f 6e65 206c 6179 6572  s only one layer
-00007330: 2c20 7468 6174 206c 6179 6572 2069 7320  , that layer is 
-00007340: 7573 6564 2e20 4465 6661 756c 7473 2074  used. Defaults t
-00007350: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-00007360: 6c61 7965 7220 2873 7472 2c20 6f70 7469  layer (str, opti
-00007370: 6f6e 616c 293a 2053 514c 2077 6865 7265  onal): SQL where
-00007380: 2063 6c61 7573 6520 746f 2072 6573 7472   clause to restr
-00007390: 6963 7420 7468 6520 726f 7773 2074 6861  ict the rows tha
-000073a0: 7420 7769 6c6c 0a20 2020 2020 2020 2020  t will.         
-000073b0: 2020 2062 6520 7570 6461 7465 642e 2044     be updated. D
-000073c0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-000073d0: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
-000073e0: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
-000073f0: 3a20 616e 2069 6e76 616c 6964 2070 6172  : an invalid par
-00007400: 616d 6574 6572 2076 616c 7565 2077 6173  ameter value was
-00007410: 2070 6173 7365 642e 0a20 2020 2022 2222   passed..    """
-00007420: 0a0a 2020 2020 2320 496e 6974 0a20 2020  ..    # Init.   
-00007430: 2070 6174 6820 3d20 5061 7468 2870 6174   path = Path(pat
-00007440: 6829 0a20 2020 2069 6620 6c61 7965 7220  h).    if layer 
-00007450: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00007460: 206c 6179 6572 203d 2067 6574 5f6f 6e6c   layer = get_onl
-00007470: 795f 6c61 7965 7228 7061 7468 290a 2020  y_layer(path).  
-00007480: 2020 6c61 7965 7269 6e66 6f5f 6f72 6967    layerinfo_orig
-00007490: 203d 2067 6574 5f6c 6179 6572 696e 666f   = get_layerinfo
-000074a0: 2870 6174 682c 206c 6179 6572 290a 2020  (path, layer).  
-000074b0: 2020 636f 6c75 6d6e 735f 7570 7065 7220    columns_upper 
-000074c0: 3d20 5b63 6f6c 756d 6e2e 7570 7065 7228  = [column.upper(
-000074d0: 2920 666f 7220 636f 6c75 6d6e 2069 6e20  ) for column in 
-000074e0: 6c61 7965 7269 6e66 6f5f 6f72 6967 2e63  layerinfo_orig.c
-000074f0: 6f6c 756d 6e73 5d0a 2020 2020 6966 206e  olumns].    if n
-00007500: 616d 652e 7570 7065 7228 2920 6e6f 7420  ame.upper() not 
-00007510: 696e 2063 6f6c 756d 6e73 5f75 7070 6572  in columns_upper
-00007520: 3a0a 2020 2020 2020 2020 2320 4966 2063  :.        # If c
-00007530: 6f6c 756d 6e20 646f 6573 6e27 7420 6578  olumn doesn't ex
-00007540: 6973 7420 7965 742c 2065 7272 6f72 210a  ist yet, error!.
-00007550: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00007560: 6c75 6545 7272 6f72 2866 2243 6f6c 756d  lueError(f"Colum
-00007570: 6e20 7b6e 616d 657d 2064 6f65 736e 2774  n {name} doesn't
-00007580: 2065 7869 7374 2069 6e20 7b70 6174 687d   exist in {path}
-00007590: 2c20 6c61 7965 7220 7b6c 6179 6572 7d22  , layer {layer}"
-000075a0: 290a 0a20 2020 2023 2047 6f21 0a20 2020  )..    # Go!.   
-000075b0: 2064 6174 6173 6f75 7263 6520 3d20 4e6f   datasource = No
-000075c0: 6e65 0a20 2020 2074 7279 3a0a 2020 2020  ne.    try:.    
-000075d0: 2020 2020 6461 7461 736f 7572 6365 203d      datasource =
-000075e0: 2067 6461 6c2e 4f70 656e 4578 2873 7472   gdal.OpenEx(str
-000075f0: 2870 6174 6829 2c20 6e4f 7065 6e46 6c61  (path), nOpenFla
-00007600: 6773 3d67 6461 6c2e 4f46 5f55 5044 4154  gs=gdal.OF_UPDAT
-00007610: 4529 0a20 2020 2020 2020 2073 716c 6974  E).        sqlit
-00007620: 655f 7374 6d74 203d 2066 2755 5044 4154  e_stmt = f'UPDAT
-00007630: 4520 227b 6c61 7965 727d 2220 5345 5420  E "{layer}" SET 
-00007640: 227b 6e61 6d65 7d22 203d 207b 6578 7072  "{name}" = {expr
-00007650: 6573 7369 6f6e 7d27 0a20 2020 2020 2020  ession}'.       
-00007660: 2069 6620 7768 6572 6520 6973 206e 6f74   if where is not
-00007670: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007680: 2020 2073 716c 6974 655f 7374 6d74 202b     sqlite_stmt +
-00007690: 3d20 6622 5c6e 2057 4845 5245 207b 7768  = f"\n WHERE {wh
-000076a0: 6572 657d 220a 2020 2020 2020 2020 7265  ere}".        re
-000076b0: 7375 6c74 203d 2064 6174 6173 6f75 7263  sult = datasourc
-000076c0: 652e 4578 6563 7574 6553 514c 2873 716c  e.ExecuteSQL(sql
-000076d0: 6974 655f 7374 6d74 2c20 6469 616c 6563  ite_stmt, dialec
-000076e0: 743d 2253 514c 4954 4522 290a 2020 2020  t="SQLITE").    
-000076f0: 2020 2020 6461 7461 736f 7572 6365 2e52      datasource.R
-00007700: 656c 6561 7365 5265 7375 6c74 5365 7428  eleaseResultSet(
-00007710: 7265 7375 6c74 290a 2020 2020 6669 6e61  result).    fina
-00007720: 6c6c 793a 0a20 2020 2020 2020 2069 6620  lly:.        if 
-00007730: 6461 7461 736f 7572 6365 2069 7320 6e6f  datasource is no
-00007740: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00007750: 2020 2020 6465 6c20 6461 7461 736f 7572      del datasour
-00007760: 6365 0a0a 0a64 6566 2072 6561 645f 6669  ce...def read_fi
-00007770: 6c65 280a 2020 2020 7061 7468 3a20 556e  le(.    path: Un
-00007780: 696f 6e5b 7374 722c 2022 6f73 2e50 6174  ion[str, "os.Pat
-00007790: 684c 696b 655b 416e 795d 225d 2c0a 2020  hLike[Any]"],.  
-000077a0: 2020 6c61 7965 723a 204f 7074 696f 6e61    layer: Optiona
-000077b0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-000077c0: 2020 2063 6f6c 756d 6e73 3a20 4f70 7469     columns: Opti
-000077d0: 6f6e 616c 5b49 7465 7261 626c 655b 7374  onal[Iterable[st
-000077e0: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-000077f0: 6262 6f78 3d4e 6f6e 652c 0a20 2020 2072  bbox=None,.    r
-00007800: 6f77 733d 4e6f 6e65 2c0a 2020 2020 7371  ows=None,.    sq
-00007810: 6c5f 7374 6d74 3a20 4f70 7469 6f6e 616c  l_stmt: Optional
-00007820: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-00007830: 2020 7371 6c5f 6469 616c 6563 743a 204f    sql_dialect: O
-00007840: 7074 696f 6e61 6c5b 4c69 7465 7261 6c5b  ptional[Literal[
-00007850: 2253 514c 4954 4522 2c20 224f 4752 5351  "SQLITE", "OGRSQ
-00007860: 4c22 5d5d 203d 204e 6f6e 652c 0a20 2020  L"]] = None,.   
-00007870: 2069 676e 6f72 655f 6765 6f6d 6574 7279   ignore_geometry
-00007880: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00007890: 2020 2020 6669 645f 6173 5f69 6e64 6578      fid_as_index
-000078a0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-000078b0: 2920 2d3e 2067 7064 2e47 656f 4461 7461  ) -> gpd.GeoData
-000078c0: 4672 616d 653a 0a20 2020 2022 2222 0a20  Frame:.    """. 
-000078d0: 2020 2052 6561 6473 2061 2066 696c 6520     Reads a file 
-000078e0: 746f 2061 2067 656f 7061 6e64 6173 2047  to a geopandas G
-000078f0: 656f 4461 7461 6672 616d 652e 0a0a 2020  eoDataframe...  
-00007900: 2020 5468 6520 6669 6c65 2066 6f72 6d61    The file forma
-00007910: 7420 6973 2064 6574 6563 7465 6420 6261  t is detected ba
-00007920: 7365 6420 6f6e 2074 6865 2066 696c 6570  sed on the filep
-00007930: 6174 6820 6578 7465 6e73 696f 6e2e 0a0a  ath extension...
-00007940: 2020 2020 4966 2061 6e20 7371 6c5f 7374      If an sql_st
-00007950: 6d74 2069 7320 7370 6563 6966 6965 642c  mt is specified,
-00007960: 2074 6865 2073 716c 6974 6520 7175 6572   the sqlite quer
-00007970: 7920 6361 6e20 636f 6e74 6169 6e20 666f  y can contain fo
-00007980: 6c6c 6f77 696e 6720 706c 6163 6568 6f6c  llowing placehol
-00007990: 6465 7273 0a20 2020 2074 6861 7420 7769  ders.    that wi
-000079a0: 6c6c 2062 6520 6175 746f 6d61 7469 6361  ll be automatica
-000079b0: 6c6c 7920 7265 706c 6163 6564 2066 6f72  lly replaced for
-000079c0: 2079 6f75 3a0a 0a20 2020 2020 202a 207b   you:..      * {
-000079d0: 6765 6f6d 6574 7279 636f 6c75 6d6e 7d3a  geometrycolumn}:
-000079e0: 2074 6865 2063 6f6c 756d 6e20 7768 6572   the column wher
-000079f0: 6520 7468 6520 7072 696d 6172 7920 6765  e the primary ge
-00007a00: 6f6d 6574 7279 2069 7320 7374 6f72 6564  ometry is stored
-00007a10: 2e0a 2020 2020 2020 2a20 7b63 6f6c 756d  ..      * {colum
-00007a20: 6e73 5f74 6f5f 7365 6c65 6374 5f73 7472  ns_to_select_str
-00007a30: 7d3a 2069 6620 2763 6f6c 756d 6e73 2720  }: if 'columns' 
-00007a40: 6973 206e 6f74 204e 6f6e 652c 2074 686f  is not None, tho
-00007a50: 7365 2063 6f6c 756d 6e73 2c0a 2020 2020  se columns,.    
-00007a60: 2020 2020 6f74 6865 7277 6973 6520 616c      otherwise al
-00007a70: 6c20 636f 6c75 6d6e 7320 6f66 2074 6865  l columns of the
-00007a80: 206c 6179 6572 2e0a 2020 2020 2020 2a20   layer..      * 
-00007a90: 7b69 6e70 7574 5f6c 6179 6572 7d3a 2074  {input_layer}: t
-00007aa0: 6865 206c 6179 6572 206e 616d 6520 6f66  he layer name of
-00007ab0: 2074 6865 2069 6e70 7574 206c 6179 6572   the input layer
-00007ac0: 2e0a 0a20 2020 2045 7861 6d70 6c65 2073  ...    Example s
-00007ad0: 716c 2073 7461 7465 6d65 6e74 2077 6974  ql statement wit
-00007ae0: 6820 706c 6163 6568 6f6c 6465 7273 3a0a  h placeholders:.
-00007af0: 2020 2020 3a3a 0a0a 2020 2020 2020 2020      ::..        
-00007b00: 5345 4c45 4354 207b 6765 6f6d 6574 7279  SELECT {geometry
-00007b10: 636f 6c75 6d6e 7d0a 2020 2020 2020 2020  column}.        
-00007b20: 2020 2020 2020 7b63 6f6c 756d 6e73 5f74        {columns_t
-00007b30: 6f5f 7365 6c65 6374 5f73 7472 7d0a 2020  o_select_str}.  
-00007b40: 2020 2020 2020 2020 4652 4f4d 2022 7b69          FROM "{i
-00007b50: 6e70 7574 5f6c 6179 6572 7d22 206c 6179  nput_layer}" lay
-00007b60: 6572 0a0a 2020 2020 5468 6520 756e 6465  er..    The unde
-00007b70: 726c 7969 6e67 206c 6962 7261 7279 2075  rlying library u
-00007b80: 7365 6420 746f 2072 6561 6420 7468 6520  sed to read the 
-00007b90: 6669 6c65 2063 616e 2062 6520 6368 6f6f  file can be choo
-00007ba0: 7365 6e20 7573 696e 6720 7468 650a 2020  sen using the.  
-00007bb0: 2020 2247 464f 5f49 4f5f 454e 4749 4e45    "GFO_IO_ENGINE
-00007bc0: 2220 656e 7669 726f 6e6d 656e 7420 7661  " environment va
-00007bd0: 7269 6162 6c65 2e20 506f 7373 6962 6c65  riable. Possible
-00007be0: 2076 616c 7565 7320 6172 6520 2266 696f   values are "fio
-00007bf0: 6e61 2220 616e 6420 2270 796f 6772 696f  na" and "pyogrio
-00007c00: 222e 0a20 2020 2054 6869 7320 6f70 7469  "..    This opti
-00007c10: 6f6e 2069 7320 6372 6561 7465 6420 6173  on is created as
-00007c20: 2061 2074 656d 706f 7261 7279 2066 616c   a temporary fal
-00007c30: 6c62 6163 6b20 746f 2022 6669 6f6e 6122  lback to "fiona"
-00007c40: 2066 6f72 2063 6173 6573 2077 6865 7265   for cases where
-00007c50: 2022 7079 6f67 7269 6f22 0a20 2020 2067   "pyogrio".    g
-00007c60: 6976 6573 2069 7373 7565 732c 2073 6f20  ives issues, so 
-00007c70: 706c 6561 7365 2072 6570 6f72 7420 6973  please report is
-00007c80: 7375 6573 2069 6620 7468 6579 2061 7265  sues if they are
-00007c90: 2065 6e63 6f75 6e74 6572 6564 2e20 496e   encountered. In
-00007ca0: 2074 6865 2066 7574 7572 6520 7375 7070   the future supp
-00007cb0: 6f72 740a 2020 2020 666f 7220 7468 6520  ort.    for the 
-00007cc0: 2266 696f 6e61 2220 656e 6769 6e65 206d  "fiona" engine m
-00007cd0: 6f73 7420 6c69 6b65 6c79 2077 696c 6c20  ost likely will 
-00007ce0: 6265 2072 656d 6f76 6564 2e20 4465 6661  be removed. Defa
-00007cf0: 756c 7420 656e 6769 6e65 2069 7320 2270  ult engine is "p
-00007d00: 796f 6772 696f 222e 0a0a 2020 2020 4172  yogrio"...    Ar
-00007d10: 6773 3a0a 2020 2020 2020 2020 7061 7468  gs:.        path
-00007d20: 2028 6669 6c65 2070 6174 6829 3a20 7061   (file path): pa
-00007d30: 7468 2074 6f20 7468 6520 6669 6c65 2074  th to the file t
-00007d40: 6f20 7265 6164 2066 726f 6d0a 2020 2020  o read from.    
-00007d50: 2020 2020 6c61 7965 7220 2873 7472 2c20      layer (str, 
-00007d60: 6f70 7469 6f6e 616c 293a 2054 6865 206c  optional): The l
-00007d70: 6179 6572 2074 6f20 7265 6164 2e20 4465  ayer to read. De
-00007d80: 6661 756c 7473 2074 6f20 4e6f 6e65 2c0a  faults to None,.
-00007d90: 2020 2020 2020 2020 2020 2020 7468 656e              then
-00007da0: 2072 6561 6473 2074 6865 206f 6e6c 7920   reads the only 
-00007db0: 6c61 7965 7220 696e 2074 6865 2066 696c  layer in the fil
-00007dc0: 6520 6f72 2074 6872 6f77 7320 6572 726f  e or throws erro
-00007dd0: 722e 0a20 2020 2020 2020 2063 6f6c 756d  r..        colum
-00007de0: 6e73 2028 4974 6572 6162 6c65 5b73 7472  ns (Iterable[str
-00007df0: 5d2c 206f 7074 696f 6e61 6c29 3a20 5468  ], optional): Th
-00007e00: 6520 286e 6f6e 2d67 656f 6d65 7472 7929  e (non-geometry)
-00007e10: 2063 6f6c 756d 6e73 2074 6f20 7265 6164   columns to read
-00007e20: 2077 696c 6c0a 2020 2020 2020 2020 2020   will.          
-00007e30: 2020 6265 2072 6574 7572 6e65 6420 696e    be returned in
-00007e40: 2074 6865 206f 7264 6572 2073 7065 6369   the order speci
-00007e50: 6669 6564 2e20 4966 204e 6f6e 652c 2061  fied. If None, a
-00007e60: 6c6c 2073 7461 6e64 6172 6420 636f 6c75  ll standard colu
-00007e70: 6d6e 7320 6172 6520 7265 6164 2e0a 2020  mns are read..  
-00007e80: 2020 2020 2020 2020 2020 496e 2061 6464            In add
-00007e90: 6974 696f 6e20 746f 2073 7461 6e64 6172  ition to standar
-00007ea0: 6420 636f 6c75 6d6e 732c 2069 7420 6973  d columns, it is
-00007eb0: 2061 6c73 6f20 706f 7373 6962 6c65 0a20   also possible. 
-00007ec0: 2020 2020 2020 2020 2020 2074 6f20 7370             to sp
-00007ed0: 6563 6966 7920 2266 6964 222c 2061 2075  ecify "fid", a u
-00007ee0: 6e69 7175 6520 696e 6465 7820 6176 6169  nique index avai
-00007ef0: 6c61 626c 6520 696e 2061 6c6c 2069 6e70  lable in all inp
-00007f00: 7574 2066 696c 6573 2e20 4e6f 7465 2074  ut files. Note t
-00007f10: 6861 7420 7468 650a 2020 2020 2020 2020  hat the.        
-00007f20: 2020 2020 2266 6964 2220 7769 6c6c 2062      "fid" will b
-00007f30: 6520 616c 6961 7365 6420 6567 2e20 746f  e aliased eg. to
-00007f40: 2022 6669 645f 3122 2e20 4465 6661 756c   "fid_1". Defaul
-00007f50: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-00007f60: 2020 2020 6262 6f78 2028 5b74 7970 655d      bbox ([type]
-00007f70: 2c20 6f70 7469 6f6e 616c 293a 2052 6561  , optional): Rea
-00007f80: 6420 6f6e 6c79 2067 656f 6d65 7472 6965  d only geometrie
-00007f90: 7320 696e 7465 7273 6563 7469 6e67 2074  s intersecting t
-00007fa0: 6869 7320 6262 6f78 2e0a 2020 2020 2020  his bbox..      
-00007fb0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00007fc0: 6f20 4e6f 6e65 2c20 7468 656e 2061 6c6c  o None, then all
-00007fd0: 2072 6f77 7320 6172 6520 7265 6164 2e0a   rows are read..
-00007fe0: 2020 2020 2020 2020 726f 7773 2028 5b74          rows ([t
-00007ff0: 7970 655d 2c20 6f70 7469 6f6e 616c 293a  ype], optional):
-00008000: 2052 6561 6420 6f6e 6c79 2074 6865 2072   Read only the r
-00008010: 6f77 7320 7370 6563 6966 6965 642e 0a20  ows specified.. 
-00008020: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00008030: 6c74 7320 746f 204e 6f6e 652c 2074 6865  lts to None, the
-00008040: 6e20 616c 6c20 726f 7773 2061 7265 2072  n all rows are r
-00008050: 6561 642e 0a20 2020 2020 2020 2073 716c  ead..        sql
-00008060: 5f73 746d 7420 2873 7472 293a 2073 716c  _stmt (str): sql
-00008070: 2073 7461 7465 6d65 6e74 2074 6f20 7573   statement to us
-00008080: 652e 204f 6e6c 7920 7375 7070 6f72 7465  e. Only supporte
-00008090: 6420 7769 7468 2022 7079 6f67 7269 6f22  d with "pyogrio"
-000080a0: 2065 6e67 696e 652e 0a20 2020 2020 2020   engine..       
-000080b0: 2073 716c 5f64 6961 6c65 6374 2028 7374   sql_dialect (st
-000080c0: 722c 206f 7074 696f 6e61 6c29 3a20 5371  r, optional): Sq
-000080d0: 6c20 6469 616c 6563 7420 7573 6564 2e20  l dialect used. 
-000080e0: 4966 204e 6f6e 652c 2066 6f72 2064 6174  If None, for dat
-000080f0: 6120 736f 7572 6365 7320 7769 7468 0a20  a sources with. 
-00008100: 2020 2020 2020 2020 2020 2065 7870 6c69             expli
-00008110: 6369 7420 5351 4c20 7375 7070 6f72 7420  cit SQL support 
-00008120: 7468 6520 7374 6174 656d 656e 7420 6973  the statement is
-00008130: 2070 726f 6365 7373 6564 2062 7920 7468   processed by th
-00008140: 6520 6465 6661 756c 7420 5351 4c20 656e  e default SQL en
-00008150: 6769 6e65 0a20 2020 2020 2020 2020 2020  gine.           
-00008160: 2028 652e 672e 2050 6f73 7447 4953 2c20   (e.g. PostGIS, 
-00008170: 4765 6f70 6163 6b61 6765 2c20 5370 6174  Geopackage, Spat
-00008180: 6961 6c69 7465 2c2e 2e2e 292e 2046 6f72  ialite,...). For
-00008190: 2064 6174 6120 736f 7572 6365 730a 2020   data sources.  
-000081a0: 2020 2020 2020 2020 2020 7769 7468 6f75            withou
-000081b0: 7420 5351 4c20 7375 7070 6f72 742c 2074  t SQL support, t
-000081c0: 6865 2022 4f47 5253 514c 2220 6469 616c  he "OGRSQL" dial
-000081d0: 6563 7420 6973 2074 6865 2064 6566 6175  ect is the defau
-000081e0: 6c74 2e20 4465 6661 756c 7473 2074 6f20  lt. Defaults to 
-000081f0: 4e6f 6e65 2e0a 2020 2020 2020 2020 6967  None..        ig
-00008200: 6e6f 7265 5f67 656f 6d65 7472 7920 2862  nore_geometry (b
-00008210: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-00008220: 5472 7565 206e 6f74 2074 6f20 7265 6164  True not to read
-00008230: 2f72 6574 7572 6e20 7468 6520 6765 6f6d  /return the geom
-00008240: 6574 7279 2e0a 2020 2020 2020 2020 2020  etry..          
-00008250: 2020 4465 6661 756c 7473 2074 6f20 4661    Defaults to Fa
-00008260: 6c73 652e 0a20 2020 2020 2020 2066 6964  lse..        fid
-00008270: 5f61 735f 696e 6465 7820 2862 6f6f 6c2c  _as_index (bool,
-00008280: 206f 7074 696f 6e61 6c29 3a20 4966 2054   optional): If T
-00008290: 7275 652c 2077 696c 6c20 7573 6520 7468  rue, will use th
-000082a0: 6520 4649 4473 206f 6620 7468 6520 6665  e FIDs of the fe
-000082b0: 6174 7572 6573 2074 6861 740a 2020 2020  atures that.    
-000082c0: 2020 2020 2020 2020 7765 7265 2072 6561          were rea
-000082d0: 6420 6173 2074 6865 2069 6e64 6578 206f  d as the index o
-000082e0: 6620 7468 6520 4765 6f44 6174 6146 7261  f the GeoDataFra
-000082f0: 6d65 2e20 4d61 7920 7374 6172 7420 6174  me. May start at
-00008300: 2030 206f 7220 3120 6465 7065 6e64 696e   0 or 1 dependin
-00008310: 6720 6f6e 0a20 2020 2020 2020 2020 2020  g on.           
-00008320: 2074 6865 2064 7269 7665 722e 2044 6566   the driver. Def
-00008330: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
-00008340: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
-00008350: 2020 2020 2056 616c 7565 4572 726f 723a       ValueError:
-00008360: 2061 6e20 696e 7661 6c69 6420 7061 7261   an invalid para
-00008370: 6d65 7465 7220 7661 6c75 6520 7761 7320  meter value was 
-00008380: 7061 7373 6564 2e0a 0a20 2020 2052 6574  passed...    Ret
-00008390: 7572 6e73 3a0a 2020 2020 2020 2020 6770  urns:.        gp
-000083a0: 642e 4765 6f44 6174 6146 7261 6d65 3a20  d.GeoDataFrame: 
-000083b0: 7468 6520 6461 7461 2072 6561 642e 0a20  the data read.. 
-000083c0: 2020 2022 2222 0a20 2020 2072 6573 756c     """.    resul
-000083d0: 745f 6764 6620 3d20 5f72 6561 645f 6669  t_gdf = _read_fi
-000083e0: 6c65 5f62 6173 6528 0a20 2020 2020 2020  le_base(.       
-000083f0: 2070 6174 683d 7061 7468 2c0a 2020 2020   path=path,.    
-00008400: 2020 2020 6c61 7965 723d 6c61 7965 722c      layer=layer,
-00008410: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
-00008420: 3d63 6f6c 756d 6e73 2c0a 2020 2020 2020  =columns,.      
-00008430: 2020 6262 6f78 3d62 626f 782c 0a20 2020    bbox=bbox,.   
-00008440: 2020 2020 2072 6f77 733d 726f 7773 2c0a       rows=rows,.
-00008450: 2020 2020 2020 2020 7371 6c5f 7374 6d74          sql_stmt
-00008460: 3d73 716c 5f73 746d 742c 0a20 2020 2020  =sql_stmt,.     
-00008470: 2020 2073 716c 5f64 6961 6c65 6374 3d73     sql_dialect=s
-00008480: 716c 5f64 6961 6c65 6374 2c0a 2020 2020  ql_dialect,.    
-00008490: 2020 2020 6967 6e6f 7265 5f67 656f 6d65      ignore_geome
-000084a0: 7472 793d 6967 6e6f 7265 5f67 656f 6d65  try=ignore_geome
-000084b0: 7472 792c 0a20 2020 2020 2020 2066 6964  try,.        fid
-000084c0: 5f61 735f 696e 6465 783d 6669 645f 6173  _as_index=fid_as
-000084d0: 5f69 6e64 6578 2c0a 2020 2020 290a 0a20  _index,.    ).. 
-000084e0: 2020 2023 204e 6f20 6173 7365 7274 2074     # No assert t
-000084f0: 6f20 6b65 6570 2062 6163 6b77 6172 6473  o keep backwards
-00008500: 2063 6f6d 7061 7469 6269 6c69 7479 0a20   compatibility. 
-00008510: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00008520: 5f67 6466 2020 2320 7479 7065 3a20 6967  _gdf  # type: ig
-00008530: 6e6f 7265 0a0a 0a64 6566 2072 6561 645f  nore...def read_
-00008540: 6669 6c65 5f6e 6f67 656f 6d28 0a20 2020  file_nogeom(.   
-00008550: 2070 6174 683a 2055 6e69 6f6e 5b73 7472   path: Union[str
-00008560: 2c20 226f 732e 5061 7468 4c69 6b65 5b41  , "os.PathLike[A
-00008570: 6e79 5d22 5d2c 0a20 2020 206c 6179 6572  ny]"],.    layer
-00008580: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00008590: 3d20 4e6f 6e65 2c0a 2020 2020 636f 6c75  = None,.    colu
-000085a0: 6d6e 733a 204f 7074 696f 6e61 6c5b 4974  mns: Optional[It
-000085b0: 6572 6162 6c65 5b73 7472 5d5d 203d 204e  erable[str]] = N
-000085c0: 6f6e 652c 0a20 2020 2062 626f 783d 4e6f  one,.    bbox=No
-000085d0: 6e65 2c0a 2020 2020 726f 7773 3d4e 6f6e  ne,.    rows=Non
-000085e0: 652c 0a20 2020 2073 716c 5f73 746d 743a  e,.    sql_stmt:
-000085f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00008600: 204e 6f6e 652c 0a20 2020 2073 716c 5f64   None,.    sql_d
-00008610: 6961 6c65 6374 3a20 4f70 7469 6f6e 616c  ialect: Optional
-00008620: 5b4c 6974 6572 616c 5b22 5351 4c49 5445  [Literal["SQLITE
-00008630: 222c 2022 4f47 5253 514c 225d 5d20 3d20  ", "OGRSQL"]] = 
-00008640: 4e6f 6e65 2c0a 2020 2020 6669 645f 6173  None,.    fid_as
-00008650: 5f69 6e64 6578 3a20 626f 6f6c 203d 2046  _index: bool = F
-00008660: 616c 7365 2c0a 2920 2d3e 2070 642e 4461  alse,.) -> pd.Da
-00008670: 7461 4672 616d 653a 0a20 2020 2022 2222  taFrame:.    """
-00008680: 0a20 2020 2044 4550 5245 4341 5445 443a  .    DEPRECATED:
-00008690: 2070 6c65 6173 6520 7573 6520 7265 6164   please use read
-000086a0: 5f66 696c 6520 7769 7468 206f 7074 696f  _file with optio
-000086b0: 6e20 6967 6e6f 7265 5f67 656f 6d65 7472  n ignore_geometr
-000086c0: 793d 5472 7565 2e0a 2020 2020 2222 220a  y=True..    """.
-000086d0: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-000086e0: 6e28 0a20 2020 2020 2020 2022 7265 6164  n(.        "read
-000086f0: 5f66 696c 655f 6e6f 6765 6f6d 2069 7320  _file_nogeom is 
-00008700: 6465 7072 6563 6174 6564 3a20 7573 6520  deprecated: use 
-00008710: 7265 6164 5f66 696c 6520 7769 7468 2069  read_file with i
-00008720: 676e 6f72 655f 6765 6f6d 6574 7279 3d54  gnore_geometry=T
-00008730: 7275 6522 2c0a 2020 2020 2020 2020 4675  rue",.        Fu
-00008740: 7475 7265 5761 726e 696e 672c 0a20 2020  tureWarning,.   
-00008750: 2029 0a20 2020 2072 6573 756c 745f 6764   ).    result_gd
-00008760: 6620 3d20 5f72 6561 645f 6669 6c65 5f62  f = _read_file_b
-00008770: 6173 6528 0a20 2020 2020 2020 2070 6174  ase(.        pat
-00008780: 683d 7061 7468 2c0a 2020 2020 2020 2020  h=path,.        
-00008790: 6c61 7965 723d 6c61 7965 722c 0a20 2020  layer=layer,.   
-000087a0: 2020 2020 2063 6f6c 756d 6e73 3d63 6f6c       columns=col
-000087b0: 756d 6e73 2c0a 2020 2020 2020 2020 6262  umns,.        bb
-000087c0: 6f78 3d62 626f 782c 0a20 2020 2020 2020  ox=bbox,.       
-000087d0: 2072 6f77 733d 726f 7773 2c0a 2020 2020   rows=rows,.    
-000087e0: 2020 2020 7371 6c5f 7374 6d74 3d73 716c      sql_stmt=sql
-000087f0: 5f73 746d 742c 0a20 2020 2020 2020 2073  _stmt,.        s
-00008800: 716c 5f64 6961 6c65 6374 3d73 716c 5f64  ql_dialect=sql_d
-00008810: 6961 6c65 6374 2c0a 2020 2020 2020 2020  ialect,.        
-00008820: 6967 6e6f 7265 5f67 656f 6d65 7472 793d  ignore_geometry=
-00008830: 5472 7565 2c0a 2020 2020 2020 2020 6669  True,.        fi
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2020 7072 6a5f 7061 7468 2e72 656e 616d    prj_path.renam
+000030f0: 6528 7072 6a5f 7265 6e61 6d65 5f70 6174  e(prj_rename_pat
+00003100: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003120: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003140: 2020 2020 2020 2020 2020 2020 2070 726a               prj
+00003150: 5f70 6174 682e 756e 6c69 6e6b 2829 0a20  _path.unlink(). 
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003180: 726a 5f70 6174 682e 7772 6974 655f 7465  rj_path.write_te
+00003190: 7874 2850 524a 5f45 5053 475f 3331 3337  xt(PRJ_EPSG_3137
+000031a0: 3029 0a0a 2020 2020 2020 2020 2020 2020  0)..            
+000031b0: 7265 7475 726e 204c 6179 6572 496e 666f  return LayerInfo
+000031c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000031d0: 2020 6e61 6d65 3d64 6174 6173 6f75 7263    name=datasourc
+000031e0: 655f 6c61 7965 722e 4765 744e 616d 6528  e_layer.GetName(
+000031f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00003200: 2020 2066 6561 7475 7265 636f 756e 743d     featurecount=
+00003210: 6461 7461 736f 7572 6365 5f6c 6179 6572  datasource_layer
+00003220: 2e47 6574 4665 6174 7572 6543 6f75 6e74  .GetFeatureCount
+00003230: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00003240: 2020 2020 746f 7461 6c5f 626f 756e 6473      total_bounds
+00003250: 3d74 6f74 616c 5f62 6f75 6e64 732c 0a20  =total_bounds,. 
+00003260: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00003270: 656f 6d65 7472 7963 6f6c 756d 6e3d 6765  eometrycolumn=ge
+00003280: 6f6d 6574 7279 636f 6c75 6d6e 2c0a 2020  ometrycolumn,.  
+00003290: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+000032a0: 6f6d 6574 7279 7479 7065 6e61 6d65 3d67  ometrytypename=g
+000032b0: 656f 6d65 7472 7974 7970 656e 616d 652c  eometrytypename,
+000032c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000032d0: 2067 656f 6d65 7472 7974 7970 653d 6765   geometrytype=ge
+000032e0: 6f6d 6574 7279 7479 7065 2c0a 2020 2020  ometrytype,.    
+000032f0: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00003300: 6d6e 733d 636f 6c75 6d6e 732c 0a20 2020  mns=columns,.   
+00003310: 2020 2020 2020 2020 2020 2020 2066 6964               fid
+00003320: 5f63 6f6c 756d 6e3d 6461 7461 736f 7572  _column=datasour
+00003330: 6365 5f6c 6179 6572 2e47 6574 4649 4443  ce_layer.GetFIDC
+00003340: 6f6c 756d 6e28 292c 0a20 2020 2020 2020  olumn(),.       
+00003350: 2020 2020 2020 2020 2063 7273 3d63 7273           crs=crs
+00003360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003370: 2020 6572 726f 7273 3d65 7272 6f72 732c    errors=errors,
+00003380: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00003390: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000033a0: 2020 2020 2020 2020 2065 7272 6f72 732e           errors.
+000033b0: 6170 7065 6e64 2822 4c61 7965 7220 646f  append("Layer do
+000033c0: 6573 6e27 7420 6861 7665 2061 2067 656f  esn't have a geo
+000033d0: 6d65 7472 7920 636f 6c75 6d6e 2122 290a  metry column!").
+000033e0: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
+000033f0: 7074 696f 6e20 6173 2065 783a 0a20 2020  ption as ex:.   
+00003400: 2020 2020 2065 782e 6172 6773 203d 2028       ex.args = (
+00003410: 6622 6765 745f 6c61 7965 7269 6e66 6f20  f"get_layerinfo 
+00003420: 6572 726f 7220 666f 7220 7b70 6174 687d  error for {path}
+00003430: 2e7b 6c61 7965 727d 3a5c 6e20 207b 6578  .{layer}:\n  {ex
+00003440: 7d22 2c29 0a20 2020 2020 2020 2072 6169  }",).        rai
+00003450: 7365 0a20 2020 2066 696e 616c 6c79 3a0a  se.    finally:.
+00003460: 2020 2020 2020 2020 6461 7461 736f 7572          datasour
+00003470: 6365 203d 204e 6f6e 650a 0a20 2020 2023  ce = None..    #
+00003480: 2049 6620 7765 2064 6964 6e27 7420 7265   If we didn't re
+00003490: 7475 726e 206f 7220 7261 6973 6520 7965  turn or raise ye
+000034a0: 7420 6865 7265 2c20 7468 6572 6520 6d75  t here, there mu
+000034b0: 7374 2068 6176 6520 6265 656e 2065 7272  st have been err
+000034c0: 6f72 730a 2020 2020 6572 726f 7273 5f73  ors.    errors_s
+000034d0: 7472 203d 2070 7072 696e 742e 7066 6f72  tr = pprint.pfor
+000034e0: 6d61 7428 6572 726f 7273 290a 2020 2020  mat(errors).    
+000034f0: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00003500: 0a20 2020 2020 2020 2066 2245 7272 6f72  .        f"Error
+00003510: 7320 696e 206c 6179 6572 2064 6566 696e  s in layer defin
+00003520: 6974 696f 6e20 6f66 2066 696c 6520 7b70  ition of file {p
+00003530: 6174 687d 2c20 6c61 7965 7220 7b6c 6179  ath}, layer {lay
+00003540: 6572 7d3a 205c 6e7b 6572 726f 7273 5f73  er}: \n{errors_s
+00003550: 7472 7d22 0a20 2020 2029 0a0a 0a64 6566  tr}".    )...def
+00003560: 2067 6574 5f6f 6e6c 795f 6c61 7965 7228   get_only_layer(
+00003570: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
+00003580: 2022 6f73 2e50 6174 684c 696b 655b 416e   "os.PathLike[An
+00003590: 795d 225d 2920 2d3e 2073 7472 3a0a 2020  y]"]) -> str:.  
+000035a0: 2020 2222 220a 2020 2020 4765 7420 7468    """.    Get th
+000035b0: 6520 6c61 7965 726e 616d 6520 666f 7220  e layername for 
+000035c0: 6120 6669 6c65 2074 6861 7420 6f6e 6c79  a file that only
+000035d0: 2063 6f6e 7461 696e 7320 6f6e 6520 6c61   contains one la
+000035e0: 7965 722e 0a0a 2020 2020 4966 2074 6865  yer...    If the
+000035f0: 2066 696c 6520 636f 6e74 6169 6e73 206d   file contains m
+00003600: 756c 7469 706c 6520 6c61 7965 7273 2c20  ultiple layers, 
+00003610: 616e 2065 7863 6570 7469 6f6e 2069 7320  an exception is 
+00003620: 7468 726f 776e 2e0a 0a20 2020 2041 7267  thrown...    Arg
+00003630: 733a 0a20 2020 2020 2020 2070 6174 6820  s:.        path 
+00003640: 2850 6174 684c 696b 6529 3a20 7468 6520  (PathLike): the 
+00003650: 6669 6c65 2e0a 0a20 2020 2052 6169 7365  file...    Raise
+00003660: 733a 0a20 2020 2020 2020 2056 616c 7565  s:.        Value
+00003670: 4572 726f 723a 2061 6e20 696e 7661 6c69  Error: an invali
+00003680: 6420 7061 7261 6d65 7465 7220 7661 6c75  d parameter valu
+00003690: 6520 7761 7320 7061 7373 6564 2e0a 0a20  e was passed... 
+000036a0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000036b0: 2020 2020 7374 723a 2074 6865 206c 6179      str: the lay
+000036c0: 6572 206e 616d 650a 2020 2020 2222 220a  er name.    """.
+000036d0: 2020 2020 6461 7461 736f 7572 6365 203d      datasource =
+000036e0: 204e 6f6e 650a 2020 2020 7472 793a 0a20   None.    try:. 
+000036f0: 2020 2020 2020 2064 6174 6173 6f75 7263         datasourc
+00003700: 655f 6c61 7965 7220 3d20 4e6f 6e65 0a20  e_layer = None. 
+00003710: 2020 2020 2020 2064 6174 6173 6f75 7263         datasourc
+00003720: 6520 3d20 6764 616c 2e4f 7065 6e45 7828  e = gdal.OpenEx(
+00003730: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00003740: 2870 6174 6829 2c20 6e4f 7065 6e46 6c61  (path), nOpenFla
+00003750: 6773 3d67 6461 6c2e 4f46 5f56 4543 544f  gs=gdal.OF_VECTO
+00003760: 5220 7c20 6764 616c 2e4f 465f 5245 4144  R | gdal.OF_READ
+00003770: 4f4e 4c59 207c 2067 6461 6c2e 4f46 5f53  ONLY | gdal.OF_S
+00003780: 4841 5245 440a 2020 2020 2020 2020 290a  HARED.        ).
+00003790: 2020 2020 2020 2020 6e62 5f6c 6179 6572          nb_layer
+000037a0: 7320 3d20 6461 7461 736f 7572 6365 2e47  s = datasource.G
+000037b0: 6574 4c61 7965 7243 6f75 6e74 2829 0a20  etLayerCount(). 
+000037c0: 2020 2020 2020 2069 6620 6e62 5f6c 6179         if nb_lay
+000037d0: 6572 7320 3d3d 2031 3a0a 2020 2020 2020  ers == 1:.      
+000037e0: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
+000037f0: 5f6c 6179 6572 203d 2064 6174 6173 6f75  _layer = datasou
+00003800: 7263 652e 4765 744c 6179 6572 4279 496e  rce.GetLayerByIn
+00003810: 6465 7828 3029 0a20 2020 2020 2020 2065  dex(0).        e
+00003820: 6c69 6620 6e62 5f6c 6179 6572 7320 3d3d  lif nb_layers ==
+00003830: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00003840: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00003850: 2866 2245 7272 6f72 3a20 4e6f 206c 6179  (f"Error: No lay
+00003860: 6572 7320 666f 756e 6420 696e 207b 7061  ers found in {pa
+00003870: 7468 7d22 290a 2020 2020 2020 2020 656c  th}").        el
+00003880: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00003890: 2320 4368 6563 6b20 6966 2074 6865 7265  # Check if there
+000038a0: 2069 7320 6f6e 6c79 206f 6e65 2073 7061   is only one spa
+000038b0: 7469 616c 206c 6179 6572 0a20 2020 2020  tial layer.     
+000038c0: 2020 2020 2020 206c 6179 6572 7320 3d20         layers = 
+000038d0: 6c69 7374 6c61 7965 7273 2870 6174 682c  listlayers(path,
+000038e0: 206f 6e6c 795f 7370 6174 6961 6c5f 6c61   only_spatial_la
+000038f0: 7965 7273 3d54 7275 6529 0a20 2020 2020  yers=True).     
+00003900: 2020 2020 2020 2069 6620 6c65 6e28 6c61         if len(la
+00003910: 7965 7273 2920 3d3d 2031 3a0a 2020 2020  yers) == 1:.    
+00003920: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00003930: 736f 7572 6365 5f6c 6179 6572 203d 2064  source_layer = d
+00003940: 6174 6173 6f75 7263 652e 4765 744c 6179  atasource.GetLay
+00003950: 6572 286c 6179 6572 735b 305d 290a 2020  er(layers[0]).  
+00003960: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003980: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00003990: 2866 224c 6179 6572 2068 6173 203e 2031  (f"Layer has > 1
+000039a0: 206c 6179 6572 3a20 7b70 6174 687d 3a20   layer: {path}: 
+000039b0: 7b6c 6179 6572 737d 2229 0a0a 2020 2020  {layers}")..    
+000039c0: 2020 2020 7265 7475 726e 2064 6174 6173      return datas
+000039d0: 6f75 7263 655f 6c61 7965 722e 4765 744e  ource_layer.GetN
+000039e0: 616d 6528 290a 0a20 2020 2065 7863 6570  ame()..    excep
+000039f0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00003a00: 783a 0a20 2020 2020 2020 2065 782e 6172  x:.        ex.ar
+00003a10: 6773 203d 2028 6622 6765 745f 6f6e 6c79  gs = (f"get_only
+00003a20: 5f6c 6179 6572 2065 7272 6f72 2066 6f72  _layer error for
+00003a30: 207b 7061 7468 7d3a 5c6e 2020 7b65 787d   {path}:\n  {ex}
+00003a40: 222c 290a 2020 2020 2020 2020 7261 6973  ",).        rais
+00003a50: 650a 2020 2020 6669 6e61 6c6c 793a 0a20  e.    finally:. 
+00003a60: 2020 2020 2020 2064 6174 6173 6f75 7263         datasourc
+00003a70: 6520 3d20 4e6f 6e65 0a0a 0a64 6566 2067  e = None...def g
+00003a80: 6574 5f64 6566 6175 6c74 5f6c 6179 6572  et_default_layer
+00003a90: 2870 6174 683a 2055 6e69 6f6e 5b73 7472  (path: Union[str
+00003aa0: 2c20 226f 732e 5061 7468 4c69 6b65 5b41  , "os.PathLike[A
+00003ab0: 6e79 5d22 5d29 202d 3e20 7374 723a 0a20  ny]"]) -> str:. 
+00003ac0: 2020 2022 2222 0a20 2020 2047 6574 2074     """.    Get t
+00003ad0: 6865 2064 6566 6175 6c74 206c 6179 6572  he default layer
+00003ae0: 206e 616d 6520 746f 2062 6520 7573 6564   name to be used
+00003af0: 2066 6f72 2061 206c 6179 6572 2069 6e20   for a layer in 
+00003b00: 7468 6973 2066 696c 652e 0a0a 2020 2020  this file...    
+00003b10: 5468 6973 2069 7320 7468 6520 7374 656d  This is the stem
+00003b20: 206f 6620 7468 6520 6669 6c65 7061 7468   of the filepath
+00003b30: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00003b40: 2020 2020 2070 6174 6820 2855 6e69 6f6e       path (Union
+00003b50: 5b73 7472 2c29 3a20 5468 6520 7061 7468  [str,): The path
+00003b60: 2074 6f20 7468 6520 6669 6c65 2e0a 0a20   to the file... 
+00003b70: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00003b80: 2020 2020 7374 723a 2054 6865 2064 6566      str: The def
+00003b90: 6175 6c74 206c 6179 6572 206e 616d 652e  ault layer name.
+00003ba0: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+00003bb0: 7572 6e20 5061 7468 2870 6174 6829 2e73  urn Path(path).s
+00003bc0: 7465 6d0a 0a0a 6465 6620 6578 6563 7574  tem...def execut
+00003bd0: 655f 7371 6c28 0a20 2020 2070 6174 683a  e_sql(.    path:
+00003be0: 2055 6e69 6f6e 5b73 7472 2c20 226f 732e   Union[str, "os.
+00003bf0: 5061 7468 4c69 6b65 5b41 6e79 5d22 5d2c  PathLike[Any]"],
+00003c00: 0a20 2020 2073 716c 5f73 746d 743a 2073  .    sql_stmt: s
+00003c10: 7472 2c0a 2020 2020 7371 6c5f 6469 616c  tr,.    sql_dial
+00003c20: 6563 743a 204f 7074 696f 6e61 6c5b 7374  ect: Optional[st
+00003c30: 725d 203d 204e 6f6e 652c 0a29 3a0a 2020  r] = None,.):.  
+00003c40: 2020 2222 220a 2020 2020 4578 6563 7574    """.    Execut
+00003c50: 6520 6120 7371 6c20 7374 6174 656d 656e  e a sql statemen
+00003c60: 7420 2844 4d4c 206f 7220 4444 4c29 206f  t (DML or DDL) o
+00003c70: 6e20 7468 6520 6669 6c65 2e0a 0a20 2020  n the file...   
+00003c80: 2054 6f20 7275 6e20 5345 4c45 4354 2073   To run SELECT s
+00003c90: 716c 2073 7461 7465 6d65 6e74 7320 6f6e  ql statements on
+00003ca0: 2061 2066 696c 652c 2075 7365 203a 6d65   a file, use :me
+00003cb0: 7468 3a60 7e72 6561 645f 6669 6c65 602e  th:`~read_file`.
+00003cc0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00003cd0: 2020 2020 7061 7468 2028 5061 7468 4c69      path (PathLi
+00003ce0: 6b65 293a 2054 6865 2070 6174 6820 746f  ke): The path to
+00003cf0: 2074 6865 2066 696c 652e 0a20 2020 2020   the file..     
+00003d00: 2020 2073 716c 5f73 746d 7420 2873 7472     sql_stmt (str
+00003d10: 293a 2054 6865 2073 716c 2073 7461 7465  ): The sql state
+00003d20: 6d65 6e74 2074 6f20 6578 6563 7574 652e  ment to execute.
+00003d30: 0a20 2020 2020 2020 2073 716c 5f64 6961  .        sql_dia
+00003d40: 6c65 6374 2028 7374 7229 3a20 5468 6520  lect (str): The 
+00003d50: 7371 6c20 6469 616c 6563 7420 746f 2075  sql dialect to u
+00003d60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00003d70: 2a20 4e6f 6e65 3a20 7573 6520 7468 6520  * None: use the 
+00003d80: 6e61 7469 7665 2053 514c 2064 6961 6c65  native SQL diale
+00003d90: 6374 206f 6620 7468 6520 6765 6f66 696c  ct of the geofil
+00003da0: 652e 0a20 2020 2020 2020 2020 2020 202a  e..            *
+00003db0: 2027 4f47 5253 514c 273a 2066 6f72 6365   'OGRSQL': force
+00003dc0: 2074 6865 2075 7365 206f 6620 7468 6520   the use of the 
+00003dd0: 4f47 5220 5351 4c20 6469 616c 6563 742e  OGR SQL dialect.
+00003de0: 0a20 2020 2020 2020 2020 2020 202a 2027  .            * '
+00003df0: 5351 4c49 5445 273a 2066 6f72 6365 2074  SQLITE': force t
+00003e00: 6865 2075 7365 206f 6620 7468 6520 5351  he use of the SQ
+00003e10: 4c49 5445 2064 6961 6c65 6374 2e0a 2020  LITE dialect..  
+00003e20: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00003e30: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00003e40: 2222 220a 2020 2020 6461 7461 736f 7572  """.    datasour
+00003e50: 6365 203d 204e 6f6e 650a 2020 2020 7472  ce = None.    tr
+00003e60: 793a 0a20 2020 2020 2020 2064 6174 6173  y:.        datas
+00003e70: 6f75 7263 6520 3d20 6764 616c 2e4f 7065  ource = gdal.Ope
+00003e80: 6e45 7828 7374 7228 7061 7468 292c 206e  nEx(str(path), n
+00003e90: 4f70 656e 466c 6167 733d 6764 616c 2e4f  OpenFlags=gdal.O
+00003ea0: 465f 5550 4441 5445 290a 2020 2020 2020  F_UPDATE).      
+00003eb0: 2020 7265 7375 6c74 203d 2064 6174 6173    result = datas
+00003ec0: 6f75 7263 652e 4578 6563 7574 6553 514c  ource.ExecuteSQL
+00003ed0: 2873 716c 5f73 746d 742c 2064 6961 6c65  (sql_stmt, diale
+00003ee0: 6374 3d73 716c 5f64 6961 6c65 6374 290a  ct=sql_dialect).
+00003ef0: 2020 2020 2020 2020 6461 7461 736f 7572          datasour
+00003f00: 6365 2e52 656c 6561 7365 5265 7375 6c74  ce.ReleaseResult
+00003f10: 5365 7428 7265 7375 6c74 290a 0a20 2020  Set(result)..   
+00003f20: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00003f30: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
+00003f40: 2065 782e 6172 6773 203d 2028 6622 6578   ex.args = (f"ex
+00003f50: 6563 7574 655f 7371 6c20 6572 726f 7220  ecute_sql error 
+00003f60: 666f 7220 7b70 6174 687d 5c6e 2020 7b65  for {path}\n  {e
+00003f70: 787d 222c 290a 2020 2020 2020 2020 7261  x}",).        ra
+00003f80: 6973 650a 2020 2020 6669 6e61 6c6c 793a  ise.    finally:
+00003f90: 0a20 2020 2020 2020 2064 6174 6173 6f75  .        datasou
+00003fa0: 7263 6520 3d20 4e6f 6e65 0a0a 0a64 6566  rce = None...def
+00003fb0: 2063 7265 6174 655f 7370 6174 6961 6c5f   create_spatial_
+00003fc0: 696e 6465 7828 0a20 2020 2070 6174 683a  index(.    path:
+00003fd0: 2055 6e69 6f6e 5b73 7472 2c20 226f 732e   Union[str, "os.
+00003fe0: 5061 7468 4c69 6b65 5b41 6e79 5d22 5d2c  PathLike[Any]"],
+00003ff0: 0a20 2020 206c 6179 6572 3a20 4f70 7469  .    layer: Opti
+00004000: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00004010: 2c0a 2020 2020 6361 6368 655f 7369 7a65  ,.    cache_size
+00004020: 5f6d 623a 204f 7074 696f 6e61 6c5b 696e  _mb: Optional[in
+00004030: 745d 203d 2031 3238 2c0a 2020 2020 6578  t] = 128,.    ex
+00004040: 6973 745f 6f6b 3a20 626f 6f6c 203d 2046  ist_ok: bool = F
+00004050: 616c 7365 2c0a 2020 2020 666f 7263 655f  alse,.    force_
+00004060: 7265 6275 696c 643a 2062 6f6f 6c20 3d20  rebuild: bool = 
+00004070: 4661 6c73 652c 0a29 3a0a 2020 2020 2222  False,.):.    ""
+00004080: 220a 2020 2020 4372 6561 7465 2061 2073  ".    Create a s
+00004090: 7061 7469 616c 2069 6e64 6578 206f 6e20  patial index on 
+000040a0: 7468 6520 6c61 7965 7220 7370 6563 6966  the layer specif
+000040b0: 6965 642e 0a0a 2020 2020 4172 6773 3a0a  ied...    Args:.
+000040c0: 2020 2020 2020 2020 7061 7468 2028 5061          path (Pa
+000040d0: 7468 4c69 6b65 293a 2054 6865 2066 696c  thLike): The fil
+000040e0: 6520 7061 7468 2e0a 2020 2020 2020 2020  e path..        
+000040f0: 6c61 7965 7220 2873 7472 2c20 6f70 7469  layer (str, opti
+00004100: 6f6e 616c 293a 2054 6865 206c 6179 6572  onal): The layer
+00004110: 2e20 4966 206e 6f74 2073 7065 6369 6669  . If not specifi
+00004120: 6564 2c20 616e 6420 7468 6572 6520 6973  ed, and there is
+00004130: 206f 6e6c 790a 2020 2020 2020 2020 2020   only.          
+00004140: 2020 6f6e 6520 6c61 7965 7220 696e 2074    one layer in t
+00004150: 6865 2066 696c 652c 2074 6869 7320 6c61  he file, this la
+00004160: 7965 7220 6973 2075 7365 642e 204f 7468  yer is used. Oth
+00004170: 6572 7769 7365 2065 7863 6570 7469 6f6e  erwise exception
+00004180: 2e0a 2020 2020 2020 2020 6361 6368 655f  ..        cache_
+00004190: 7369 7a65 5f6d 6220 2869 6e74 2c20 6f70  size_mb (int, op
+000041a0: 7469 6f6e 616c 293a 2063 6163 6865 206d  tional): cache m
+000041b0: 656d 6f72 7920 696e 204d 4220 7468 6174  emory in MB that
+000041c0: 2063 616e 2062 6520 7573 6564 2077 6869   can be used whi
+000041d0: 6c65 0a20 2020 2020 2020 2020 2020 2063  le.            c
+000041e0: 7265 6174 696e 6720 7370 6174 6961 6c20  reating spatial 
+000041f0: 696e 6465 7820 666f 7220 7370 6174 6961  index for spatia
+00004200: 6c69 7465 2066 696c 6573 2028 2e67 706b  lite files (.gpk
+00004210: 6720 6f72 202e 7371 6c69 7465 292e 2049  g or .sqlite). I
+00004220: 6620 4e6f 6e65 2c0a 2020 2020 2020 2020  f None,.        
+00004230: 2020 2020 7468 6520 6465 6661 756c 7420      the default 
+00004240: 6361 6368 655f 7369 7a65 2066 726f 6d20  cache_size from 
+00004250: 7371 6c69 7465 2069 7320 7573 6564 2e20  sqlite is used. 
+00004260: 4465 6661 756c 7473 2074 6f20 3132 382e  Defaults to 128.
+00004270: 0a20 2020 2020 2020 2065 7869 7374 5f6f  .        exist_o
+00004280: 6b20 2862 6f6f 6c2c 206f 7074 696f 6e73  k (bool, options
+00004290: 293a 2049 6620 5472 7565 2061 6e64 2074  ): If True and t
+000042a0: 6865 2069 6e64 6578 2065 7869 7374 7320  he index exists 
+000042b0: 616c 7265 6164 792c 2064 6f6e 2774 0a20  already, don't. 
+000042c0: 2020 2020 2020 2020 2020 2074 6872 6f77             throw
+000042d0: 2061 6e20 6572 726f 722e 0a20 2020 2020   an error..     
+000042e0: 2020 2066 6f72 6365 5f72 6562 7569 6c64     force_rebuild
+000042f0: 2028 626f 6f6c 2c20 6f70 7469 6f6e 7329   (bool, options)
+00004300: 3a20 5472 7565 2074 6f20 666f 7263 6520  : True to force 
+00004310: 7265 6275 696c 6420 6576 656e 2069 6620  rebuild even if 
+00004320: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
+00004330: 2020 6578 6973 7473 2061 6c72 6561 6479    exists already
+00004340: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
+00004350: 6c73 652e 0a20 2020 2022 2222 0a20 2020  lse..    """.   
+00004360: 2023 2049 6e69 740a 2020 2020 7061 7468   # Init.    path
+00004370: 203d 2050 6174 6828 7061 7468 290a 2020   = Path(path).  
+00004380: 2020 6966 206c 6179 6572 2069 7320 4e6f    if layer is No
+00004390: 6e65 3a0a 2020 2020 2020 2020 6c61 7965  ne:.        laye
+000043a0: 7220 3d20 6765 745f 6f6e 6c79 5f6c 6179  r = get_only_lay
+000043b0: 6572 2870 6174 6829 0a0a 2020 2020 2320  er(path)..    # 
+000043c0: 4966 2069 6e64 6578 2061 6c72 6561 6479  If index already
+000043d0: 2065 7869 7374 732c 2072 656d 6f76 6520   exists, remove 
+000043e0: 696e 6465 7820 6f72 2072 6574 7572 6e0a  index or return.
+000043f0: 2020 2020 6966 2068 6173 5f73 7061 7469      if has_spati
+00004400: 616c 5f69 6e64 6578 2870 6174 682c 206c  al_index(path, l
+00004410: 6179 6572 293a 0a20 2020 2020 2020 2069  ayer):.        i
+00004420: 6620 666f 7263 655f 7265 6275 696c 643a  f force_rebuild:
+00004430: 0a20 2020 2020 2020 2020 2020 2072 656d  .            rem
+00004440: 6f76 655f 7370 6174 6961 6c5f 696e 6465  ove_spatial_inde
+00004450: 7828 7061 7468 2c20 6c61 7965 7229 0a20  x(path, layer). 
+00004460: 2020 2020 2020 2065 6c69 6620 6578 6973         elif exis
+00004470: 745f 6f6b 3a0a 2020 2020 2020 2020 2020  t_ok:.          
+00004480: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00004490: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000044a0: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+000044b0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000044c0: 2020 2020 6622 4572 726f 7220 6164 6469      f"Error addi
+000044d0: 6e67 2073 7061 7469 616c 2069 6e64 6578  ng spatial index
+000044e0: 2074 6f20 7b70 6174 687d 2e7b 6c61 7965   to {path}.{laye
+000044f0: 727d 2c20 6974 2065 7869 7374 7320 616c  r}, it exists al
+00004500: 7265 6164 7922 0a20 2020 2020 2020 2020  ready".         
+00004510: 2020 2029 0a0a 2020 2020 2320 4e6f 7720     )..    # Now 
+00004520: 7265 616c 6c79 2061 6464 2069 6e64 6578  really add index
+00004530: 0a20 2020 2064 6174 6173 6f75 7263 6520  .    datasource 
+00004540: 3d20 4e6f 6e65 0a20 2020 2074 7279 3a0a  = None.    try:.
+00004550: 2020 2020 2020 2020 6765 6f66 696c 6574          geofilet
+00004560: 7970 6520 3d20 4765 6f66 696c 6554 7970  ype = GeofileTyp
+00004570: 6528 7061 7468 290a 2020 2020 2020 2020  e(path).        
+00004580: 6966 2067 656f 6669 6c65 7479 7065 2e69  if geofiletype.i
+00004590: 735f 7370 6174 6961 6c69 7465 5f62 6173  s_spatialite_bas
+000045a0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+000045b0: 2320 5468 6520 636f 6e66 6967 206f 7074  # The config opt
+000045c0: 696f 6e73 206e 6565 6420 746f 2062 6520  ions need to be 
+000045d0: 7365 7420 6265 666f 7265 206f 7065 6e69  set before openi
+000045e0: 6e67 2074 6865 2066 696c 6521 0a20 2020  ng the file!.   
+000045f0: 2020 2020 2020 2020 206c 6179 6572 696e           layerin
+00004600: 666f 203d 2067 6574 5f6c 6179 6572 696e  fo = get_layerin
+00004610: 666f 2870 6174 682c 206c 6179 6572 290a  fo(path, layer).
+00004620: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00004630: 205f 6f67 725f 7574 696c 2e73 6574 5f63   _ogr_util.set_c
+00004640: 6f6e 6669 675f 6f70 7469 6f6e 7328 7b22  onfig_options({"
+00004650: 4f47 525f 5351 4c49 5445 5f43 4143 4845  OGR_SQLITE_CACHE
+00004660: 223a 2063 6163 6865 5f73 697a 655f 6d62  ": cache_size_mb
+00004670: 7d29 3a0a 2020 2020 2020 2020 2020 2020  }):.            
+00004680: 2020 2020 6461 7461 736f 7572 6365 203d      datasource =
+00004690: 2067 6461 6c2e 4f70 656e 4578 2873 7472   gdal.OpenEx(str
+000046a0: 2870 6174 6829 2c20 6e4f 7065 6e46 6c61  (path), nOpenFla
+000046b0: 6773 3d67 6461 6c2e 4f46 5f55 5044 4154  gs=gdal.OF_UPDAT
+000046c0: 4529 0a20 2020 2020 2020 2020 2020 2020  E).             
+000046d0: 2020 2067 656f 6d65 7472 7963 6f6c 756d     geometrycolum
+000046e0: 6e20 3d20 6c61 7965 7269 6e66 6f2e 6765  n = layerinfo.ge
+000046f0: 6f6d 6574 7279 636f 6c75 6d6e 0a20 2020  ometrycolumn.   
+00004700: 2020 2020 2020 2020 2020 2020 2073 716c               sql
+00004710: 203d 2066 2253 454c 4543 5420 4372 6561   = f"SELECT Crea
+00004720: 7465 5370 6174 6961 6c49 6e64 6578 2827  teSpatialIndex('
+00004730: 7b6c 6179 6572 7d27 2c20 277b 6765 6f6d  {layer}', '{geom
+00004740: 6574 7279 636f 6c75 6d6e 7d27 2922 0a20  etrycolumn}')". 
+00004750: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004760: 6573 756c 7420 3d20 6461 7461 736f 7572  esult = datasour
+00004770: 6365 2e45 7865 6375 7465 5351 4c28 7371  ce.ExecuteSQL(sq
+00004780: 6c2c 2064 6961 6c65 6374 3d22 5351 4c49  l, dialect="SQLI
+00004790: 5445 2229 0a20 2020 2020 2020 2020 2020  TE").           
+000047a0: 2020 2020 2064 6174 6173 6f75 7263 652e       datasource.
+000047b0: 5265 6c65 6173 6552 6573 756c 7453 6574  ReleaseResultSet
+000047c0: 2872 6573 756c 7429 0a20 2020 2020 2020  (result).       
+000047d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000047e0: 2020 2064 6174 6173 6f75 7263 6520 3d20     datasource = 
+000047f0: 6764 616c 2e4f 7065 6e45 7828 7374 7228  gdal.OpenEx(str(
+00004800: 7061 7468 292c 206e 4f70 656e 466c 6167  path), nOpenFlag
+00004810: 733d 6764 616c 2e4f 465f 5550 4441 5445  s=gdal.OF_UPDATE
+00004820: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00004830: 7375 6c74 203d 2064 6174 6173 6f75 7263  sult = datasourc
+00004840: 652e 4578 6563 7574 6553 514c 2866 2743  e.ExecuteSQL(f'C
+00004850: 5245 4154 4520 5350 4154 4941 4c20 494e  REATE SPATIAL IN
+00004860: 4445 5820 4f4e 2022 7b6c 6179 6572 7d22  DEX ON "{layer}"
+00004870: 2729 0a20 2020 2020 2020 2020 2020 2064  ').            d
+00004880: 6174 6173 6f75 7263 652e 5265 6c65 6173  atasource.Releas
+00004890: 6552 6573 756c 7453 6574 2872 6573 756c  eResultSet(resul
+000048a0: 7429 0a0a 2020 2020 6578 6365 7074 2045  t)..    except E
+000048b0: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
+000048c0: 2020 2020 2020 2020 6578 2e61 7267 7320          ex.args 
+000048d0: 3d20 2866 2263 7265 6174 655f 7370 6174  = (f"create_spat
+000048e0: 6961 6c5f 696e 6465 7820 6572 726f 7220  ial_index error 
+000048f0: 666f 7220 7b70 6174 687d 2e7b 6c61 7965  for {path}.{laye
+00004900: 727d 3a5c 6e20 207b 6578 7d22 2c29 0a20  r}:\n  {ex}",). 
+00004910: 2020 2020 2020 2072 6169 7365 0a20 2020         raise.   
+00004920: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
+00004930: 2020 6461 7461 736f 7572 6365 203d 204e    datasource = N
+00004940: 6f6e 650a 0a20 2020 2069 6620 6e6f 7420  one..    if not 
+00004950: 6861 735f 7370 6174 6961 6c5f 696e 6465  has_spatial_inde
+00004960: 7828 7061 7468 2c20 6c61 7965 7229 3a0a  x(path, layer):.
+00004970: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+00004980: 6e74 696d 6545 7272 6f72 2866 2263 7265  ntimeError(f"cre
+00004990: 6174 655f 7370 6174 6961 6c5f 696e 6465  ate_spatial_inde
+000049a0: 7820 6661 696c 6564 206f 6e20 7b70 6174  x failed on {pat
+000049b0: 687d 2c20 6c61 7965 723a 207b 6c61 7965  h}, layer: {laye
+000049c0: 727d 2229 0a0a 0a64 6566 2068 6173 5f73  r}")...def has_s
+000049d0: 7061 7469 616c 5f69 6e64 6578 280a 2020  patial_index(.  
+000049e0: 2020 7061 7468 3a20 556e 696f 6e5b 7374    path: Union[st
+000049f0: 722c 2022 6f73 2e50 6174 684c 696b 655b  r, "os.PathLike[
+00004a00: 416e 795d 225d 2c20 6c61 7965 723a 204f  Any]"], layer: O
+00004a10: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00004a20: 6f6e 650a 2920 2d3e 2062 6f6f 6c3a 0a20  one.) -> bool:. 
+00004a30: 2020 2022 2222 0a20 2020 2043 6865 636b     """.    Check
+00004a40: 2069 6620 7468 6520 6c61 7965 722f 636f   if the layer/co
+00004a50: 6c75 6d6e 2068 6173 2061 2073 7061 7469  lumn has a spati
+00004a60: 616c 2069 6e64 6578 2e0a 0a20 2020 2041  al index...    A
+00004a70: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+00004a80: 6820 2850 6174 684c 696b 6529 3a20 5468  h (PathLike): Th
+00004a90: 6520 6669 6c65 2070 6174 682e 0a20 2020  e file path..   
+00004aa0: 2020 2020 206c 6179 6572 2028 7374 722c       layer (str,
+00004ab0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00004ac0: 6c61 7965 722e 2044 6566 6175 6c74 7320  layer. Defaults 
+00004ad0: 746f 204e 6f6e 652e 0a0a 2020 2020 5261  to None...    Ra
+00004ae0: 6973 6573 3a0a 2020 2020 2020 2020 5661  ises:.        Va
+00004af0: 6c75 6545 7272 6f72 3a20 616e 2069 6e76  lueError: an inv
+00004b00: 616c 6964 2070 6172 616d 6574 6572 2076  alid parameter v
+00004b10: 616c 7565 2077 6173 2070 6173 7365 642e  alue was passed.
+00004b20: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00004b30: 2020 2020 2020 2062 6f6f 6c3a 2054 7275         bool: Tru
+00004b40: 6520 6966 2074 6865 2073 7061 7469 616c  e if the spatial
+00004b50: 2063 6f6c 756d 6e20 6578 6973 7473 2e0a   column exists..
+00004b60: 2020 2020 2222 220a 2020 2020 2320 496e      """.    # In
+00004b70: 6974 0a20 2020 2070 6174 6820 3d20 5061  it.    path = Pa
+00004b80: 7468 2870 6174 6829 0a0a 2020 2020 2320  th(path)..    # 
+00004b90: 4e6f 7720 6368 6563 6b20 7468 6520 696e  Now check the in
+00004ba0: 6465 780a 2020 2020 6461 7461 736f 7572  dex.    datasour
+00004bb0: 6365 203d 204e 6f6e 650a 2020 2020 6765  ce = None.    ge
+00004bc0: 6f66 696c 6574 7970 6520 3d20 4765 6f66  ofiletype = Geof
+00004bd0: 696c 6554 7970 6528 7061 7468 290a 2020  ileType(path).  
+00004be0: 2020 7472 793a 0a20 2020 2020 2020 2069    try:.        i
+00004bf0: 6620 6765 6f66 696c 6574 7970 652e 6973  f geofiletype.is
+00004c00: 5f73 7061 7469 616c 6974 655f 6261 7365  _spatialite_base
+00004c10: 643a 0a20 2020 2020 2020 2020 2020 206c  d:.            l
+00004c20: 6179 6572 696e 666f 203d 2067 6574 5f6c  ayerinfo = get_l
+00004c30: 6179 6572 696e 666f 2870 6174 682c 206c  ayerinfo(path, l
+00004c40: 6179 6572 290a 2020 2020 2020 2020 2020  ayer).          
+00004c50: 2020 6461 7461 736f 7572 6365 203d 2067    datasource = g
+00004c60: 6461 6c2e 4f70 656e 4578 2873 7472 2870  dal.OpenEx(str(p
+00004c70: 6174 6829 2c20 6e4f 7065 6e46 6c61 6773  ath), nOpenFlags
+00004c80: 3d67 6461 6c2e 4f46 5f52 4541 444f 4e4c  =gdal.OF_READONL
+00004c90: 5929 0a20 2020 2020 2020 2020 2020 2073  Y).            s
+00004ca0: 716c 203d 2066 2222 220a 2020 2020 2020  ql = f""".      
+00004cb0: 2020 2020 2020 2020 2020 5345 4c45 4354            SELECT
+00004cc0: 2048 6173 5370 6174 6961 6c49 6e64 6578   HasSpatialIndex
+00004cd0: 2827 7b6c 6179 6572 696e 666f 2e6e 616d  ('{layerinfo.nam
+00004ce0: 657d 272c 0a20 2020 2020 2020 2020 2020  e}',.           
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2020 2020 2020 2020 2020 2020 277b 6c61              '{la
+00004d10: 7965 7269 6e66 6f2e 6765 6f6d 6574 7279  yerinfo.geometry
+00004d20: 636f 6c75 6d6e 7d27 290a 2020 2020 2020  column}').      
+00004d30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004d40: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00004d50: 6174 6173 6f75 7263 652e 4578 6563 7574  atasource.Execut
+00004d60: 6553 514c 2873 716c 2c20 6469 616c 6563  eSQL(sql, dialec
+00004d70: 743d 2253 514c 4954 4522 290a 2020 2020  t="SQLITE").    
+00004d80: 2020 2020 2020 2020 6861 735f 7370 6174          has_spat
+00004d90: 6961 6c5f 696e 6465 7820 3d20 7265 7375  ial_index = resu
+00004da0: 6c74 2e47 6574 4e65 7874 4665 6174 7572  lt.GetNextFeatur
+00004db0: 6528 292e 4765 7446 6965 6c64 2830 2920  e().GetField(0) 
+00004dc0: 3d3d 2031 0a20 2020 2020 2020 2020 2020  == 1.           
+00004dd0: 2064 6174 6173 6f75 7263 652e 5265 6c65   datasource.Rele
+00004de0: 6173 6552 6573 756c 7453 6574 2872 6573  aseResultSet(res
+00004df0: 756c 7429 0a20 2020 2020 2020 2020 2020  ult).           
+00004e00: 2072 6574 7572 6e20 6861 735f 7370 6174   return has_spat
+00004e10: 6961 6c5f 696e 6465 780a 2020 2020 2020  ial_index.      
+00004e20: 2020 656c 6966 2067 656f 6669 6c65 7479    elif geofilety
+00004e30: 7065 203d 3d20 4765 6f66 696c 6554 7970  pe == GeofileTyp
+00004e40: 652e 4553 5249 5368 6170 6566 696c 653a  e.ESRIShapefile:
+00004e50: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
+00004e60: 6578 5f70 6174 6820 3d20 7061 7468 2e70  ex_path = path.p
+00004e70: 6172 656e 7420 2f20 6622 7b70 6174 682e  arent / f"{path.
+00004e80: 7374 656d 7d2e 7169 7822 0a20 2020 2020  stem}.qix".     
+00004e90: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
+00004ea0: 6465 785f 7061 7468 2e65 7869 7374 7328  dex_path.exists(
+00004eb0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00004ec0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00004ed0: 6520 5661 6c75 6545 7272 6f72 2866 2268  e ValueError(f"h
+00004ee0: 6173 5f73 7061 7469 616c 5f69 6e64 6578  as_spatial_index
+00004ef0: 206e 6f74 2073 7570 706f 7274 6564 2066   not supported f
+00004f00: 6f72 207b 7061 7468 7d22 290a 0a20 2020  or {path}")..   
+00004f10: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00004f20: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
+00004f30: 2065 782e 6172 6773 203d 2028 6622 6861   ex.args = (f"ha
+00004f40: 735f 7370 6174 6961 6c5f 696e 6465 7820  s_spatial_index 
+00004f50: 6572 726f 7220 666f 7220 7b70 6174 687d  error for {path}
+00004f60: 2e7b 6c61 7965 727d 3a5c 6e20 207b 6578  .{layer}:\n  {ex
+00004f70: 7d22 2c29 0a20 2020 2020 2020 2072 6169  }",).        rai
+00004f80: 7365 0a20 2020 2066 696e 616c 6c79 3a0a  se.    finally:.
+00004f90: 2020 2020 2020 2020 6461 7461 736f 7572          datasour
+00004fa0: 6365 203d 204e 6f6e 650a 0a0a 6465 6620  ce = None...def 
+00004fb0: 7265 6d6f 7665 5f73 7061 7469 616c 5f69  remove_spatial_i
+00004fc0: 6e64 6578 280a 2020 2020 7061 7468 3a20  ndex(.    path: 
+00004fd0: 556e 696f 6e5b 7374 722c 2022 6f73 2e50  Union[str, "os.P
+00004fe0: 6174 684c 696b 655b 416e 795d 225d 2c20  athLike[Any]"], 
+00004ff0: 6c61 7965 723a 204f 7074 696f 6e61 6c5b  layer: Optional[
+00005000: 7374 725d 203d 204e 6f6e 650a 293a 0a20  str] = None.):. 
+00005010: 2020 2022 2222 0a20 2020 2052 656d 6f76     """.    Remov
+00005020: 6520 7468 6520 7370 6174 6961 6c20 696e  e the spatial in
+00005030: 6465 7820 6672 6f6d 2074 6865 206c 6179  dex from the lay
+00005040: 6572 2073 7065 6369 6669 6564 2e0a 0a20  er specified... 
+00005050: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00005060: 2070 6174 6820 2850 6174 684c 696b 6529   path (PathLike)
+00005070: 3a20 5468 6520 6669 6c65 2070 6174 682e  : The file path.
+00005080: 0a20 2020 2020 2020 206c 6179 6572 2028  .        layer (
+00005090: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+000050a0: 5468 6520 6c61 7965 722e 2049 6620 6e6f  The layer. If no
+000050b0: 7420 7370 6563 6966 6965 642c 2061 6e64  t specified, and
+000050c0: 2074 6865 7265 2069 7320 6f6e 6c79 0a20   there is only. 
+000050d0: 2020 2020 2020 2020 2020 206f 6e65 206c             one l
+000050e0: 6179 6572 2069 6e20 7468 6520 6669 6c65  ayer in the file
+000050f0: 2c20 7468 6973 206c 6179 6572 2069 7320  , this layer is 
+00005100: 7573 6564 2e20 4f74 6865 7277 6973 6520  used. Otherwise 
+00005110: 6578 6365 7074 696f 6e2e 0a20 2020 2022  exception..    "
+00005120: 2222 0a20 2020 2023 2049 6e69 740a 2020  "".    # Init.  
+00005130: 2020 7061 7468 203d 2050 6174 6828 7061    path = Path(pa
+00005140: 7468 290a 0a20 2020 2023 204e 6f77 2072  th)..    # Now r
+00005150: 6561 6c6c 7920 7265 6d6f 7665 2069 6e64  eally remove ind
+00005160: 6578 0a20 2020 2064 6174 6173 6f75 7263  ex.    datasourc
+00005170: 6520 3d20 4e6f 6e65 0a20 2020 2067 656f  e = None.    geo
+00005180: 6669 6c65 7479 7065 203d 2047 656f 6669  filetype = Geofi
+00005190: 6c65 5479 7065 2870 6174 6829 0a20 2020  leType(path).   
+000051a0: 206c 6179 6572 696e 666f 203d 2067 6574   layerinfo = get
+000051b0: 5f6c 6179 6572 696e 666f 2870 6174 682c  _layerinfo(path,
+000051c0: 206c 6179 6572 290a 2020 2020 7472 793a   layer).    try:
+000051d0: 0a20 2020 2020 2020 2069 6620 6765 6f66  .        if geof
+000051e0: 696c 6574 7970 652e 6973 5f73 7061 7469  iletype.is_spati
+000051f0: 616c 6974 655f 6261 7365 643a 0a20 2020  alite_based:.   
+00005200: 2020 2020 2020 2020 2064 6174 6173 6f75           datasou
+00005210: 7263 6520 3d20 6764 616c 2e4f 7065 6e45  rce = gdal.OpenE
+00005220: 7828 7374 7228 7061 7468 292c 206e 4f70  x(str(path), nOp
+00005230: 656e 466c 6167 733d 6764 616c 2e4f 465f  enFlags=gdal.OF_
+00005240: 5550 4441 5445 290a 2020 2020 2020 2020  UPDATE).        
+00005250: 2020 2020 7265 7375 6c74 203d 2064 6174      result = dat
+00005260: 6173 6f75 7263 652e 4578 6563 7574 6553  asource.ExecuteS
+00005270: 514c 280a 2020 2020 2020 2020 2020 2020  QL(.            
+00005280: 2020 2020 6622 5345 4c45 4354 2044 6973      f"SELECT Dis
+00005290: 6162 6c65 5370 6174 6961 6c49 6e64 6578  ableSpatialIndex
+000052a0: 2827 7b6c 6179 6572 696e 666f 2e6e 616d  ('{layerinfo.nam
+000052b0: 657d 272c 2027 7b6c 6179 6572 696e 666f  e}', '{layerinfo
+000052c0: 2e67 656f 6d65 7472 7963 6f6c 756d 6e7d  .geometrycolumn}
+000052d0: 2729 222c 2020 2320 6e6f 7161 3a20 4535  ')",  # noqa: E5
+000052e0: 3031 0a20 2020 2020 2020 2020 2020 2020  01.             
+000052f0: 2020 2064 6961 6c65 6374 3d22 5351 4c49     dialect="SQLI
+00005300: 5445 222c 0a20 2020 2020 2020 2020 2020  TE",.           
+00005310: 2029 0a20 2020 2020 2020 2020 2020 2064   ).            d
+00005320: 6174 6173 6f75 7263 652e 5265 6c65 6173  atasource.Releas
+00005330: 6552 6573 756c 7453 6574 2872 6573 756c  eResultSet(resul
+00005340: 7429 0a20 2020 2020 2020 2065 6c69 6620  t).        elif 
+00005350: 6765 6f66 696c 6574 7970 6520 3d3d 2047  geofiletype == G
+00005360: 656f 6669 6c65 5479 7065 2e45 5352 4953  eofileType.ESRIS
+00005370: 6861 7065 6669 6c65 3a0a 2020 2020 2020  hapefile:.      
+00005380: 2020 2020 2020 2320 4452 4f50 2053 5041        # DROP SPA
+00005390: 5449 414c 2049 4e44 4558 204f 4e20 2e2e  TIAL INDEX ON ..
+000053a0: 2e20 636f 6d6d 616e 6420 6769 7665 7320  . command gives 
+000053b0: 616e 2065 7272 6f72 2c20 736f 206a 7573  an error, so jus
+000053c0: 7420 7265 6d6f 7665 202e 7169 780a 2020  t remove .qix.  
+000053d0: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+000053e0: 7061 7468 203d 2070 6174 682e 7061 7265  path = path.pare
+000053f0: 6e74 202f 2066 227b 7061 7468 2e73 7465  nt / f"{path.ste
+00005400: 6d7d 2e71 6978 220a 2020 2020 2020 2020  m}.qix".        
+00005410: 2020 2020 696e 6465 785f 7061 7468 2e75      index_path.u
+00005420: 6e6c 696e 6b28 290a 2020 2020 2020 2020  nlink().        
+00005430: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00005440: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
+00005450: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00005460: 2020 2020 2020 6622 7265 6d6f 7665 5f73        f"remove_s
+00005470: 7061 7469 616c 5f69 6e64 6578 2069 7320  patial_index is 
+00005480: 6e6f 7420 7375 7070 6f72 7465 6420 666f  not supported fo
+00005490: 7220 7b70 6174 682e 7375 6666 6978 7d20  r {path.suffix} 
+000054a0: 6669 6c65 220a 2020 2020 2020 2020 2020  file".          
+000054b0: 2020 290a 0a20 2020 2065 7863 6570 7420    )..    except 
+000054c0: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
+000054d0: 0a20 2020 2020 2020 2065 782e 6172 6773  .        ex.args
+000054e0: 203d 2028 6622 7265 6d6f 7665 5f73 7061   = (f"remove_spa
+000054f0: 7469 616c 5f69 6e64 6578 2065 7272 6f72  tial_index error
+00005500: 2066 6f72 207b 7061 7468 7d2e 7b6c 6179   for {path}.{lay
+00005510: 6572 7d3a 5c6e 2020 7b65 787d 222c 290a  er}:\n  {ex}",).
+00005520: 2020 2020 2020 2020 7261 6973 650a 2020          raise.  
+00005530: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
+00005540: 2020 2064 6174 6173 6f75 7263 6520 3d20     datasource = 
+00005550: 4e6f 6e65 0a0a 0a64 6566 2072 656e 616d  None...def renam
+00005560: 655f 6c61 7965 7228 0a20 2020 2070 6174  e_layer(.    pat
+00005570: 683a 2055 6e69 6f6e 5b73 7472 2c20 226f  h: Union[str, "o
+00005580: 732e 5061 7468 4c69 6b65 5b41 6e79 5d22  s.PathLike[Any]"
+00005590: 5d2c 206e 6577 5f6c 6179 6572 3a20 7374  ], new_layer: st
+000055a0: 722c 206c 6179 6572 3a20 4f70 7469 6f6e  r, layer: Option
+000055b0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a29  al[str] = None.)
+000055c0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+000055d0: 6e61 6d65 2074 6865 206c 6179 6572 2073  name the layer s
+000055e0: 7065 6369 6669 6564 2e0a 0a20 2020 2041  pecified...    A
+000055f0: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+00005600: 6820 2850 6174 684c 696b 6529 3a20 5468  h (PathLike): Th
+00005610: 6520 6669 6c65 2070 6174 682e 0a20 2020  e file path..   
+00005620: 2020 2020 206c 6179 6572 2028 4f70 7469       layer (Opti
+00005630: 6f6e 616c 5b73 7472 5d29 3a20 5468 6520  onal[str]): The 
+00005640: 6c61 7965 7220 6e61 6d65 2e20 4966 206e  layer name. If n
+00005650: 6f74 2073 7065 6369 6669 6564 2c20 616e  ot specified, an
+00005660: 6420 7468 6572 6520 6973 206f 6e6c 790a  d there is only.
+00005670: 2020 2020 2020 2020 2020 2020 6f6e 6520              one 
+00005680: 6c61 7965 7220 696e 2074 6865 2066 696c  layer in the fil
+00005690: 652c 2074 6869 7320 6c61 7965 7220 6973  e, this layer is
+000056a0: 2075 7365 642e 204f 7468 6572 7769 7365   used. Otherwise
+000056b0: 2065 7863 6570 7469 6f6e 2e0a 2020 2020   exception..    
+000056c0: 2020 2020 6e65 775f 6c61 7965 7220 2873      new_layer (s
+000056d0: 7472 293a 2054 6865 206e 6577 206c 6179  tr): The new lay
+000056e0: 6572 206e 616d 652e 2049 6620 6e6f 7420  er name. If not 
+000056f0: 7370 6563 6966 6965 642c 2061 6e64 2074  specified, and t
+00005700: 6865 7265 2069 7320 6f6e 6c79 0a20 2020  here is only.   
+00005710: 2020 2020 2020 2020 206f 6e65 206c 6179           one lay
+00005720: 6572 2069 6e20 7468 6520 6669 6c65 2c20  er in the file, 
+00005730: 7468 6973 206c 6179 6572 2069 7320 7573  this layer is us
+00005740: 6564 2e20 4f74 6865 7277 6973 6520 6578  ed. Otherwise ex
+00005750: 6365 7074 696f 6e2e 0a20 2020 2022 2222  ception..    """
+00005760: 0a20 2020 2023 2043 6865 636b 2069 6e70  .    # Check inp
+00005770: 7574 2070 6172 616d 6574 6572 730a 2020  ut parameters.  
+00005780: 2020 7061 7468 203d 2050 6174 6828 7061    path = Path(pa
+00005790: 7468 290a 2020 2020 6966 206c 6179 6572  th).    if layer
+000057a0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000057b0: 2020 6c61 7965 7220 3d20 6765 745f 6f6e    layer = get_on
+000057c0: 6c79 5f6c 6179 6572 2870 6174 6829 0a0a  ly_layer(path)..
+000057d0: 2020 2020 2320 4e6f 7720 7265 616c 6c79      # Now really
+000057e0: 2072 656e 616d 650a 2020 2020 6461 7461   rename.    data
+000057f0: 736f 7572 6365 203d 204e 6f6e 650a 2020  source = None.  
+00005800: 2020 6765 6f66 696c 6574 7970 6520 3d20    geofiletype = 
+00005810: 4765 6f66 696c 6554 7970 6528 7061 7468  GeofileType(path
+00005820: 290a 2020 2020 6966 2067 656f 6669 6c65  ).    if geofile
+00005830: 7479 7065 2e69 735f 7370 6174 6961 6c69  type.is_spatiali
+00005840: 7465 5f62 6173 6564 3a0a 2020 2020 2020  te_based:.      
+00005850: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00005860: 2020 2064 6174 6173 6f75 7263 6520 3d20     datasource = 
+00005870: 6764 616c 2e4f 7065 6e45 7828 7374 7228  gdal.OpenEx(str(
+00005880: 7061 7468 292c 206e 4f70 656e 466c 6167  path), nOpenFlag
+00005890: 733d 6764 616c 2e4f 465f 5550 4441 5445  s=gdal.OF_UPDATE
+000058a0: 290a 2020 2020 2020 2020 2020 2020 7371  ).            sq
+000058b0: 6c5f 7374 6d74 203d 2066 2741 4c54 4552  l_stmt = f'ALTER
+000058c0: 2054 4142 4c45 2022 7b6c 6179 6572 7d22   TABLE "{layer}"
+000058d0: 2052 454e 414d 4520 544f 2022 7b6e 6577   RENAME TO "{new
+000058e0: 5f6c 6179 6572 7d22 270a 2020 2020 2020  _layer}"'.      
+000058f0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00005900: 6174 6173 6f75 7263 652e 4578 6563 7574  atasource.Execut
+00005910: 6553 514c 2873 716c 5f73 746d 7429 0a20  eSQL(sql_stmt). 
+00005920: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00005930: 6f75 7263 652e 5265 6c65 6173 6552 6573  ource.ReleaseRes
+00005940: 756c 7453 6574 2872 6573 756c 7429 0a20  ultSet(result). 
+00005950: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00005960: 6365 7074 696f 6e20 6173 2065 783a 0a20  ception as ex:. 
+00005970: 2020 2020 2020 2020 2020 2065 782e 6172             ex.ar
+00005980: 6773 203d 2028 6622 7265 6e61 6d65 5f6c  gs = (f"rename_l
+00005990: 6179 6572 2065 7272 6f72 2066 6f72 207b  ayer error for {
+000059a0: 7061 7468 7d2e 7b6c 6179 6572 7d3a 5c6e  path}.{layer}:\n
+000059b0: 2020 7b65 787d 222c 290a 2020 2020 2020    {ex}",).      
+000059c0: 2020 2020 2020 7261 6973 650a 2020 2020        raise.    
+000059d0: 2020 2020 6669 6e61 6c6c 793a 0a20 2020      finally:.   
+000059e0: 2020 2020 2020 2020 2064 6174 6173 6f75           datasou
+000059f0: 7263 6520 3d20 4e6f 6e65 0a20 2020 2065  rce = None.    e
+00005a00: 6c69 6620 6765 6f66 696c 6574 7970 6520  lif geofiletype 
+00005a10: 3d3d 2047 656f 6669 6c65 5479 7065 2e45  == GeofileType.E
+00005a20: 5352 4953 6861 7065 6669 6c65 3a0a 2020  SRIShapefile:.  
+00005a30: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00005a40: 6545 7272 6f72 2866 2272 656e 616d 655f  eError(f"rename_
+00005a50: 6c61 7965 7220 6e6f 7420 706f 7373 6962  layer not possib
+00005a60: 6c65 2066 6f72 207b 6765 6f66 696c 6574  le for {geofilet
+00005a70: 7970 657d 2066 696c 6522 290a 2020 2020  ype} file").    
+00005a80: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
+00005a90: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00005aa0: 2272 656e 616d 655f 6c61 7965 7220 6e6f  "rename_layer no
+00005ab0: 7420 696d 706c 656d 656e 7465 6420 666f  t implemented fo
+00005ac0: 7220 7b70 6174 682e 7375 6666 6978 7d20  r {path.suffix} 
+00005ad0: 6669 6c65 2229 0a0a 0a64 6566 2072 656e  file")...def ren
+00005ae0: 616d 655f 636f 6c75 6d6e 280a 2020 2020  ame_column(.    
+00005af0: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
+00005b00: 2022 6f73 2e50 6174 684c 696b 655b 416e   "os.PathLike[An
+00005b10: 795d 225d 2c0a 2020 2020 636f 6c75 6d6e  y]"],.    column
+00005b20: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
+00005b30: 6e65 775f 636f 6c75 6d6e 5f6e 616d 653a  new_column_name:
+00005b40: 2073 7472 2c0a 2020 2020 6c61 7965 723a   str,.    layer:
+00005b50: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00005b60: 204e 6f6e 652c 0a29 3a0a 2020 2020 2222   None,.):.    ""
+00005b70: 220a 2020 2020 5265 6e61 6d65 2074 6865  ".    Rename the
+00005b80: 2063 6f6c 756d 6e20 7370 6563 6966 6965   column specifie
+00005b90: 642e 0a0a 2020 2020 4172 6773 3a0a 2020  d...    Args:.  
+00005ba0: 2020 2020 2020 7061 7468 2028 5061 7468        path (Path
+00005bb0: 4c69 6b65 293a 2054 6865 2066 696c 6520  Like): The file 
+00005bc0: 7061 7468 2e0a 2020 2020 2020 2020 636f  path..        co
+00005bd0: 6c75 6d6e 5f6e 616d 6520 2873 7472 293a  lumn_name (str):
+00005be0: 2074 6865 2063 7572 7265 6e74 2063 6f6c   the current col
+00005bf0: 756d 6e20 6e61 6d65 2e0a 2020 2020 2020  umn name..      
+00005c00: 2020 6e65 775f 636f 6c75 6d6e 5f6e 616d    new_column_nam
+00005c10: 6520 2873 7472 293a 2074 6865 206e 6577  e (str): the new
+00005c20: 2063 6f6c 756d 6e20 6e61 6d65 2e0a 2020   column name..  
+00005c30: 2020 2020 2020 6c61 7965 7220 284f 7074        layer (Opt
+00005c40: 696f 6e61 6c5b 7374 725d 293a 2054 6865  ional[str]): The
+00005c50: 206c 6179 6572 206e 616d 652e 2049 6620   layer name. If 
+00005c60: 6e6f 7420 7370 6563 6966 6965 642c 2061  not specified, a
+00005c70: 6e64 2074 6865 7265 2069 7320 6f6e 6c79  nd there is only
+00005c80: 0a20 2020 2020 2020 2020 2020 206f 6e65  .            one
+00005c90: 206c 6179 6572 2069 6e20 7468 6520 6669   layer in the fi
+00005ca0: 6c65 2c20 7468 6973 206c 6179 6572 2069  le, this layer i
+00005cb0: 7320 7573 6564 2e20 4f74 6865 7277 6973  s used. Otherwis
+00005cc0: 6520 6578 6365 7074 696f 6e2e 0a20 2020  e exception..   
+00005cd0: 2022 2222 0a20 2020 2023 2043 6865 636b   """.    # Check
+00005ce0: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+00005cf0: 730a 2020 2020 7061 7468 203d 2050 6174  s.    path = Pat
+00005d00: 6828 7061 7468 290a 2020 2020 6966 206c  h(path).    if l
+00005d10: 6179 6572 2069 7320 4e6f 6e65 3a0a 2020  ayer is None:.  
+00005d20: 2020 2020 2020 6c61 7965 7220 3d20 6765        layer = ge
+00005d30: 745f 6f6e 6c79 5f6c 6179 6572 2870 6174  t_only_layer(pat
+00005d40: 6829 0a20 2020 2069 6e66 6f20 3d20 6765  h).    info = ge
+00005d50: 745f 6c61 7965 7269 6e66 6f28 7061 7468  t_layerinfo(path
+00005d60: 2c20 6c61 7965 7229 0a20 2020 2069 6620  , layer).    if 
+00005d70: 636f 6c75 6d6e 5f6e 616d 6520 6e6f 7420  column_name not 
+00005d80: 696e 2069 6e66 6f2e 636f 6c75 6d6e 7320  in info.columns 
+00005d90: 616e 6420 6e65 775f 636f 6c75 6d6e 5f6e  and new_column_n
+00005da0: 616d 6520 696e 2069 6e66 6f2e 636f 6c75  ame in info.colu
+00005db0: 6d6e 733a 0a20 2020 2020 2020 206c 6f67  mns:.        log
+00005dc0: 6765 722e 696e 666f 280a 2020 2020 2020  ger.info(.      
+00005dd0: 2020 2020 2020 6622 436f 6c75 6d6e 207b        f"Column {
+00005de0: 636f 6c75 6d6e 5f6e 616d 657d 2073 6565  column_name} see
+00005df0: 6d73 2074 6f20 6265 2072 656e 616d 6564  ms to be renamed
+00005e00: 2061 6c72 6561 6479 2074 6f20 7b6e 6577   already to {new
+00005e10: 5f63 6f6c 756d 6e5f 6e61 6d65 7d22 0a20  _column_name}". 
+00005e20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005e30: 2072 6574 7572 6e0a 0a20 2020 2023 204e   return..    # N
+00005e40: 6f77 2072 6561 6c6c 7920 7265 6e61 6d65  ow really rename
+00005e50: 0a20 2020 2064 6174 6173 6f75 7263 6520  .    datasource 
+00005e60: 3d20 4e6f 6e65 0a20 2020 2067 656f 6669  = None.    geofi
+00005e70: 6c65 7479 7065 203d 2047 656f 6669 6c65  letype = Geofile
+00005e80: 5479 7065 2870 6174 6829 0a20 2020 2069  Type(path).    i
+00005e90: 6620 6765 6f66 696c 6574 7970 652e 6973  f geofiletype.is
+00005ea0: 5f73 7061 7469 616c 6974 655f 6261 7365  _spatialite_base
+00005eb0: 643a 0a20 2020 2020 2020 2074 7279 3a0a  d:.        try:.
+00005ec0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00005ed0: 736f 7572 6365 203d 2067 6461 6c2e 4f70  source = gdal.Op
+00005ee0: 656e 4578 2873 7472 2870 6174 6829 2c20  enEx(str(path), 
+00005ef0: 6e4f 7065 6e46 6c61 6773 3d67 6461 6c2e  nOpenFlags=gdal.
+00005f00: 4f46 5f55 5044 4154 4529 0a20 2020 2020  OF_UPDATE).     
+00005f10: 2020 2020 2020 2073 716c 5f73 746d 7420         sql_stmt 
+00005f20: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00005f30: 2020 2020 6627 414c 5445 5220 5441 424c      f'ALTER TABL
+00005f40: 4520 227b 6c61 7965 727d 2220 270a 2020  E "{layer}" '.  
+00005f50: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00005f60: 5245 4e41 4d45 2043 4f4c 554d 4e20 227b  RENAME COLUMN "{
+00005f70: 636f 6c75 6d6e 5f6e 616d 657d 2220 544f  column_name}" TO
+00005f80: 2022 7b6e 6577 5f63 6f6c 756d 6e5f 6e61   "{new_column_na
+00005f90: 6d65 7d22 270a 2020 2020 2020 2020 2020  me}"'.          
+00005fa0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00005fb0: 7265 7375 6c74 203d 2064 6174 6173 6f75  result = datasou
+00005fc0: 7263 652e 4578 6563 7574 6553 514c 2873  rce.ExecuteSQL(s
+00005fd0: 716c 5f73 746d 7429 0a20 2020 2020 2020  ql_stmt).       
+00005fe0: 2020 2020 2064 6174 6173 6f75 7263 652e       datasource.
+00005ff0: 5265 6c65 6173 6552 6573 756c 7453 6574  ReleaseResultSet
+00006000: 2872 6573 756c 7429 0a20 2020 2020 2020  (result).       
+00006010: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00006020: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
+00006030: 2020 2020 2065 782e 6172 6773 203d 2028       ex.args = (
+00006040: 6622 7265 6e61 6d65 5f63 6f6c 756d 6e20  f"rename_column 
+00006050: 6572 726f 7220 666f 7220 7b70 6174 687d  error for {path}
+00006060: 2e7b 6c61 7965 727d 3a5c 6e20 207b 6578  .{layer}:\n  {ex
+00006070: 7d22 2c29 0a20 2020 2020 2020 2020 2020  }",).           
+00006080: 2072 6169 7365 0a20 2020 2020 2020 2066   raise.        f
+00006090: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
+000060a0: 2020 2020 6461 7461 736f 7572 6365 203d      datasource =
+000060b0: 204e 6f6e 650a 0a20 2020 2065 6c69 6620   None..    elif 
+000060c0: 6765 6f66 696c 6574 7970 6520 3d3d 2047  geofiletype == G
+000060d0: 656f 6669 6c65 5479 7065 2e45 5352 4953  eofileType.ESRIS
+000060e0: 6861 7065 6669 6c65 3a0a 2020 2020 2020  hapefile:.      
+000060f0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00006100: 6f72 2866 2272 656e 616d 655f 636f 6c75  or(f"rename_colu
+00006110: 6d6e 2069 7320 6e6f 7420 706f 7373 6962  mn is not possib
+00006120: 6c65 2066 6f72 207b 6765 6f66 696c 6574  le for {geofilet
+00006130: 7970 657d 2066 696c 6522 290a 2020 2020  ype} file").    
+00006140: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
+00006150: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00006160: 2272 656e 616d 655f 636f 6c75 6d6e 2069  "rename_column i
+00006170: 7320 6e6f 7420 696d 706c 656d 656e 7465  s not implemente
+00006180: 6420 666f 7220 7b70 6174 682e 7375 6666  d for {path.suff
+00006190: 6978 7d20 6669 6c65 2229 0a0a 0a63 6c61  ix} file")...cla
+000061a0: 7373 2044 6174 6154 7970 6528 656e 756d  ss DataType(enum
+000061b0: 2e45 6e75 6d29 3a0a 2020 2020 2222 220a  .Enum):.    """.
+000061c0: 2020 2020 5468 6973 2065 6e75 6d20 6465      This enum de
+000061d0: 6669 6e65 7320 7468 6520 7374 616e 6461  fines the standa
+000061e0: 7264 2064 6174 6120 7479 7065 7320 7468  rd data types th
+000061f0: 6174 2063 616e 2062 6520 7573 6564 2066  at can be used f
+00006200: 6f72 2063 6f6c 756d 6e73 2e0a 2020 2020  or columns..    
+00006210: 2222 220a 0a20 2020 2054 4558 5420 3d20  """..    TEXT = 
+00006220: 2254 4558 5422 0a20 2020 2022 2222 436f  "TEXT".    """Co
+00006230: 6c75 6d6e 2077 6974 6820 7465 7874 2064  lumn with text d
+00006240: 6174 613a 207e 2073 7472 696e 672c 2063  ata: ~ string, c
+00006250: 6861 722c 2076 6172 6368 6172 2c20 636c  har, varchar, cl
+00006260: 6f62 2e22 2222 0a20 2020 2049 4e54 4547  ob.""".    INTEG
+00006270: 4552 203d 2022 494e 5445 4745 5222 0a20  ER = "INTEGER". 
+00006280: 2020 2022 2222 436f 6c75 6d6e 2077 6974     """Column wit
+00006290: 6820 696e 7465 6765 7220 6461 7461 2e22  h integer data."
+000062a0: 2222 0a20 2020 2052 4541 4c20 3d20 2252  "".    REAL = "R
+000062b0: 4541 4c22 0a20 2020 2022 2222 436f 6c75  EAL".    """Colu
+000062c0: 6d6e 2077 6974 6820 666c 6f61 7469 6e67  mn with floating
+000062d0: 2070 6f69 6e74 2064 6174 613a 207e 2066   point data: ~ f
+000062e0: 6c6f 6174 2c20 646f 7562 6c65 2e22 2222  loat, double."""
+000062f0: 0a20 2020 2044 4154 4520 3d20 2244 4154  .    DATE = "DAT
+00006300: 4522 0a20 2020 2022 2222 436f 6c75 6d6e  E".    """Column
+00006310: 2077 6974 6820 6461 7465 2064 6174 612e   with date data.
+00006320: 2222 220a 2020 2020 5449 4d45 5354 414d  """.    TIMESTAM
+00006330: 5020 3d20 2254 494d 4553 5441 4d50 220a  P = "TIMESTAMP".
+00006340: 2020 2020 2222 2243 6f6c 756d 6e20 7769      """Column wi
+00006350: 7468 2074 696d 6573 7461 6d70 2064 6174  th timestamp dat
+00006360: 613a 207e 2064 6174 6574 696d 652e 2222  a: ~ datetime.""
+00006370: 220a 2020 2020 424f 4f4c 4541 4e20 3d20  ".    BOOLEAN = 
+00006380: 2242 4f4f 4c45 414e 220a 2020 2020 2222  "BOOLEAN".    ""
+00006390: 2243 6f6c 756d 6e20 7769 7468 2062 6f6f  "Column with boo
+000063a0: 6c65 616e 2064 6174 612e 2222 220a 2020  lean data.""".  
+000063b0: 2020 424c 4f42 203d 2022 424c 4f42 220a    BLOB = "BLOB".
+000063c0: 2020 2020 2222 2243 6f6c 756d 6e20 7769      """Column wi
+000063d0: 7468 2062 696e 6172 7920 6461 7461 2e22  th binary data."
+000063e0: 2222 0a20 2020 204e 554d 4552 4943 203d  "".    NUMERIC =
+000063f0: 2022 4e55 4d45 5249 4322 0a20 2020 2022   "NUMERIC".    "
+00006400: 2222 436f 6c75 6d6e 2077 6974 6820 6e75  ""Column with nu
+00006410: 6d65 7269 6320 6461 7461 3a20 6578 6163  meric data: exac
+00006420: 7420 6465 6369 6d61 6c20 6461 7461 2e22  t decimal data."
+00006430: 2222 0a0a 0a64 6566 2061 6464 5f63 6f6c  ""...def add_col
+00006440: 756d 6e28 0a20 2020 2070 6174 683a 2055  umn(.    path: U
+00006450: 6e69 6f6e 5b73 7472 2c20 226f 732e 5061  nion[str, "os.Pa
+00006460: 7468 4c69 6b65 5b41 6e79 5d22 5d2c 0a20  thLike[Any]"],. 
+00006470: 2020 206e 616d 653a 2073 7472 2c0a 2020     name: str,.  
+00006480: 2020 7479 7065 3a20 556e 696f 6e5b 4461    type: Union[Da
+00006490: 7461 5479 7065 2c20 7374 725d 2c0a 2020  taType, str],.  
+000064a0: 2020 6578 7072 6573 7369 6f6e 3a20 556e    expression: Un
+000064b0: 696f 6e5b 7374 722c 2069 6e74 2c20 666c  ion[str, int, fl
+000064c0: 6f61 742c 204e 6f6e 655d 203d 204e 6f6e  oat, None] = Non
+000064d0: 652c 0a20 2020 2065 7870 7265 7373 696f  e,.    expressio
+000064e0: 6e5f 6469 616c 6563 743a 204f 7074 696f  n_dialect: Optio
+000064f0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00006500: 0a20 2020 206c 6179 6572 3a20 4f70 7469  .    layer: Opti
+00006510: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00006520: 2c0a 2020 2020 666f 7263 655f 7570 6461  ,.    force_upda
+00006530: 7465 3a20 626f 6f6c 203d 2046 616c 7365  te: bool = False
+00006540: 2c0a 2020 2020 7769 6474 683a 204f 7074  ,.    width: Opt
+00006550: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00006560: 652c 0a29 3a0a 2020 2020 2222 220a 2020  e,.):.    """.  
+00006570: 2020 4164 6420 6120 636f 6c75 6d6e 2074    Add a column t
+00006580: 6f20 6120 6c61 7965 7220 6f66 2074 6865  o a layer of the
+00006590: 2067 656f 6669 6c65 2e0a 0a20 2020 2041   geofile...    A
+000065a0: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+000065b0: 6820 2850 6174 684c 696b 6529 3a20 5061  h (PathLike): Pa
+000065c0: 7468 2074 6f20 7468 6520 6765 6f66 696c  th to the geofil
+000065d0: 652e 0a20 2020 2020 2020 206e 616d 6520  e..        name 
+000065e0: 2873 7472 293a 204e 616d 6520 666f 7220  (str): Name for 
+000065f0: 7468 6520 6e65 7720 636f 6c75 6d6e 2e0a  the new column..
+00006600: 2020 2020 2020 2020 7479 7065 2028 7374          type (st
+00006610: 7229 3a20 436f 6c75 6d6e 2074 7970 6520  r): Column type 
+00006620: 6f66 2074 6865 206e 6577 2063 6f6c 756d  of the new colum
+00006630: 6e2e 0a20 2020 2020 2020 2065 7870 7265  n..        expre
+00006640: 7373 696f 6e20 2873 7472 2c20 6f70 7469  ssion (str, opti
+00006650: 6f6e 616c 293a 2053 514c 6974 6520 6578  onal): SQLite ex
+00006660: 7072 6573 7369 6f6e 2074 6f20 7573 6520  pression to use 
+00006670: 746f 2075 7064 6174 650a 2020 2020 2020  to update.      
+00006680: 2020 2020 2020 7468 6520 7661 6c75 652e        the value.
+00006690: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+000066a0: 652e 0a20 2020 2020 2020 2065 7870 7265  e..        expre
+000066b0: 7373 696f 6e5f 6469 616c 6563 7420 2873  ssion_dialect (s
+000066c0: 7472 2c20 6f70 7469 6f6e 616c 293a 2053  tr, optional): S
+000066d0: 514c 2064 6961 6c65 6374 2075 7365 6420  QL dialect used 
+000066e0: 666f 7220 7468 6520 6578 7072 6573 7369  for the expressi
+000066f0: 6f6e 2e0a 2020 2020 2020 2020 6c61 7965  on..        laye
+00006700: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
+00006710: 293a 2054 6865 206c 6179 6572 206e 616d  ): The layer nam
+00006720: 652e 2049 6620 4e6f 6e65 2061 6e64 2074  e. If None and t
+00006730: 6865 2067 656f 6669 6c65 0a20 2020 2020  he geofile.     
+00006740: 2020 2020 2020 2068 6173 206f 6e6c 7920         has only 
+00006750: 6f6e 6520 6c61 7965 722c 2074 6861 7420  one layer, that 
+00006760: 6c61 7965 7220 6973 2075 7365 642e 2044  layer is used. D
+00006770: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+00006780: 0a20 2020 2020 2020 2066 6f72 6365 5f75  .        force_u
+00006790: 7064 6174 6520 2862 6f6f 6c2c 206f 7074  pdate (bool, opt
+000067a0: 696f 6e61 6c29 3a20 4966 2074 6865 2063  ional): If the c
+000067b0: 6f6c 756d 6e20 616c 7265 6164 7920 6578  olumn already ex
+000067c0: 6973 7473 2c20 6578 6563 7574 650a 2020  ists, execute.  
+000067d0: 2020 2020 2020 2020 2020 7468 6520 7570            the up
+000067e0: 6461 7465 2061 6e79 7761 792e 2044 6566  date anyway. Def
+000067f0: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
+00006800: 2020 2020 2020 2020 7769 6474 6820 2869          width (i
+00006810: 6e74 2c20 6f70 7469 6f6e 616c 293a 2074  nt, optional): t
+00006820: 6865 2077 6964 7468 206f 6620 7468 6520  he width of the 
+00006830: 6669 656c 642e 0a0a 2020 2020 5261 6973  field...    Rais
+00006840: 6573 3a0a 2020 2020 2020 2020 6578 3a20  es:.        ex: 
+00006850: 5b64 6573 6372 6970 7469 6f6e 5d0a 2020  [description].  
+00006860: 2020 2222 220a 2020 2020 2320 496e 6974    """.    # Init
+00006870: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00006880: 6365 2874 7970 652c 2044 6174 6154 7970  ce(type, DataTyp
+00006890: 6529 3a0a 2020 2020 2020 2020 7479 7065  e):.        type
+000068a0: 5f73 7472 203d 2074 7970 652e 7661 6c75  _str = type.valu
+000068b0: 650a 2020 2020 656c 7365 3a0a 2020 2020  e.    else:.    
+000068c0: 2020 2020 7479 7065 5f6c 6f77 6572 203d      type_lower =
+000068d0: 2074 7970 652e 6c6f 7765 7228 290a 2020   type.lower().  
+000068e0: 2020 2020 2020 6966 2074 7970 655f 6c6f        if type_lo
+000068f0: 7765 7220 3d3d 2022 7374 7269 6e67 223a  wer == "string":
+00006900: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00006910: 4f44 4f3a 2074 6869 6e6b 2077 6865 7468  ODO: think wheth
+00006920: 6572 2062 6569 6e67 2066 6c65 7869 626c  er being flexibl
+00006930: 6520 6865 7265 2069 7320 6120 676f 6f64  e here is a good
+00006940: 2069 6465 612e 2e2e 0a20 2020 2020 2020   idea....       
+00006950: 2020 2020 2074 7970 655f 7374 7220 3d20       type_str = 
+00006960: 2254 4558 5422 0a20 2020 2020 2020 2065  "TEXT".        e
+00006970: 6c69 6620 7479 7065 5f6c 6f77 6572 203d  lif type_lower =
+00006980: 3d20 2262 696e 6172 7922 3a0a 2020 2020  = "binary":.    
+00006990: 2020 2020 2020 2020 7479 7065 5f73 7472          type_str
+000069a0: 203d 2022 424c 4f42 220a 2020 2020 2020   = "BLOB".      
+000069b0: 2020 656c 6966 2074 7970 655f 6c6f 7765    elif type_lowe
+000069c0: 7220 3d3d 2022 7469 6d65 223a 0a20 2020  r == "time":.   
+000069d0: 2020 2020 2020 2020 2074 7970 655f 7374           type_st
+000069e0: 7220 3d20 2244 4154 4554 494d 4522 0a20  r = "DATETIME". 
+000069f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006a00: 2020 2020 2020 2020 2074 7970 655f 7374           type_st
+00006a10: 7220 3d20 7479 7065 0a20 2020 2070 6174  r = type.    pat
+00006a20: 6820 3d20 5061 7468 2870 6174 6829 0a20  h = Path(path). 
+00006a30: 2020 2069 6620 6c61 7965 7220 6973 204e     if layer is N
+00006a40: 6f6e 653a 0a20 2020 2020 2020 206c 6179  one:.        lay
+00006a50: 6572 203d 2067 6574 5f6f 6e6c 795f 6c61  er = get_only_la
+00006a60: 7965 7228 7061 7468 290a 2020 2020 6c61  yer(path).    la
+00006a70: 7965 7269 6e66 6f5f 6f72 6967 203d 2067  yerinfo_orig = g
+00006a80: 6574 5f6c 6179 6572 696e 666f 2870 6174  et_layerinfo(pat
+00006a90: 682c 206c 6179 6572 290a 0a20 2020 2023  h, layer)..    #
+00006aa0: 2047 6f21 0a20 2020 2064 6174 6173 6f75   Go!.    datasou
+00006ab0: 7263 6520 3d20 4e6f 6e65 0a20 2020 2074  rce = None.    t
+00006ac0: 7279 3a0a 2020 2020 2020 2020 2320 4966  ry:.        # If
+00006ad0: 2063 6f6c 756d 6e20 646f 6573 6e27 7420   column doesn't 
+00006ae0: 6578 6973 7420 7965 742c 2063 7265 6174  exist yet, creat
+00006af0: 6520 6974 0a20 2020 2020 2020 2063 6f6c  e it.        col
+00006b00: 756d 6e73 5f75 7070 6572 203d 205b 636f  umns_upper = [co
+00006b10: 6c75 6d6e 2e75 7070 6572 2829 2066 6f72  lumn.upper() for
+00006b20: 2063 6f6c 756d 6e20 696e 206c 6179 6572   column in layer
+00006b30: 696e 666f 5f6f 7269 672e 636f 6c75 6d6e  info_orig.column
+00006b40: 735d 0a20 2020 2020 2020 2069 6620 6e61  s].        if na
+00006b50: 6d65 2e75 7070 6572 2829 206e 6f74 2069  me.upper() not i
+00006b60: 6e20 636f 6c75 6d6e 735f 7570 7065 723a  n columns_upper:
+00006b70: 0a20 2020 2020 2020 2020 2020 2077 6964  .            wid
+00006b80: 7468 5f73 7472 203d 2066 2228 7b77 6964  th_str = f"({wid
+00006b90: 7468 7d29 2220 6966 2077 6964 7468 2069  th})" if width i
+00006ba0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00006bb0: 2222 0a20 2020 2020 2020 2020 2020 2073  "".            s
+00006bc0: 716c 5f73 746d 7420 3d20 280a 2020 2020  ql_stmt = (.    
+00006bd0: 2020 2020 2020 2020 2020 2020 6627 414c              f'AL
+00006be0: 5445 5220 5441 424c 4520 227b 6c61 7965  TER TABLE "{laye
+00006bf0: 727d 2220 4144 4420 434f 4c55 4d4e 2022  r}" ADD COLUMN "
+00006c00: 7b6e 616d 657d 2220 7b74 7970 655f 7374  {name}" {type_st
+00006c10: 727d 7b77 6964 7468 5f73 7472 7d27 0a20  r}{width_str}'. 
+00006c20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006c30: 2020 2020 2020 2020 2064 6174 6173 6f75           datasou
+00006c40: 7263 6520 3d20 6764 616c 2e4f 7065 6e45  rce = gdal.OpenE
+00006c50: 7828 7374 7228 7061 7468 292c 206e 4f70  x(str(path), nOp
+00006c60: 656e 466c 6167 733d 6764 616c 2e4f 465f  enFlags=gdal.OF_
+00006c70: 5550 4441 5445 290a 2020 2020 2020 2020  UPDATE).        
+00006c80: 2020 2020 7265 7375 6c74 203d 2064 6174      result = dat
+00006c90: 6173 6f75 7263 652e 4578 6563 7574 6553  asource.ExecuteS
+00006ca0: 514c 2873 716c 5f73 746d 7429 0a20 2020  QL(sql_stmt).   
+00006cb0: 2020 2020 2020 2020 2064 6174 6173 6f75           datasou
+00006cc0: 7263 652e 5265 6c65 6173 6552 6573 756c  rce.ReleaseResul
+00006cd0: 7453 6574 2872 6573 756c 7429 0a20 2020  tSet(result).   
+00006ce0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00006cf0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+00006d00: 726e 696e 6728 6622 436f 6c75 6d6e 207b  rning(f"Column {
+00006d10: 6e61 6d65 7d20 6578 6973 7465 6420 616c  name} existed al
+00006d20: 7265 6164 7920 696e 207b 7061 7468 7d2c  ready in {path},
+00006d30: 206c 6179 6572 207b 6c61 7965 727d 2229   layer {layer}")
+00006d40: 0a0a 2020 2020 2020 2020 2320 4966 2061  ..        # If a
+00006d50: 6e20 6578 7072 6573 7369 6f6e 2077 6173  n expression was
+00006d60: 2070 726f 7669 6465 6420 616e 6420 7570   provided and up
+00006d70: 6461 7465 2063 616e 2062 6520 646f 6e65  date can be done
+00006d80: 2c20 676f 2066 6f72 2069 742e 2e2e 0a20  , go for it.... 
+00006d90: 2020 2020 2020 2069 6620 6578 7072 6573         if expres
+00006da0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+00006db0: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
+00006dc0: 2020 206e 616d 6520 6e6f 7420 696e 206c     name not in l
+00006dd0: 6179 6572 696e 666f 5f6f 7269 672e 636f  ayerinfo_orig.co
+00006de0: 6c75 6d6e 7320 6f72 2066 6f72 6365 5f75  lumns or force_u
+00006df0: 7064 6174 6520 6973 2054 7275 650a 2020  pdate is True.  
+00006e00: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00006e10: 2020 2020 2069 6620 6461 7461 736f 7572       if datasour
+00006e20: 6365 2069 7320 4e6f 6e65 3a0a 2020 2020  ce is None:.    
+00006e30: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00006e40: 736f 7572 6365 203d 2067 6461 6c2e 4f70  source = gdal.Op
+00006e50: 656e 4578 2873 7472 2870 6174 6829 2c20  enEx(str(path), 
+00006e60: 6e4f 7065 6e46 6c61 6773 3d67 6461 6c2e  nOpenFlags=gdal.
+00006e70: 4f46 5f55 5044 4154 4529 0a20 2020 2020  OF_UPDATE).     
+00006e80: 2020 2020 2020 2073 716c 5f73 746d 7420         sql_stmt 
+00006e90: 3d20 6627 5550 4441 5445 2022 7b6c 6179  = f'UPDATE "{lay
+00006ea0: 6572 7d22 2053 4554 2022 7b6e 616d 657d  er}" SET "{name}
+00006eb0: 2220 3d20 7b65 7870 7265 7373 696f 6e7d  " = {expression}
+00006ec0: 270a 2020 2020 2020 2020 2020 2020 7265  '.            re
+00006ed0: 7375 6c74 203d 2064 6174 6173 6f75 7263  sult = datasourc
+00006ee0: 652e 4578 6563 7574 6553 514c 2873 716c  e.ExecuteSQL(sql
+00006ef0: 5f73 746d 742c 2064 6961 6c65 6374 3d65  _stmt, dialect=e
+00006f00: 7870 7265 7373 696f 6e5f 6469 616c 6563  xpression_dialec
+00006f10: 7429 0a20 2020 2020 2020 2020 2020 2064  t).            d
+00006f20: 6174 6173 6f75 7263 652e 5265 6c65 6173  atasource.Releas
+00006f30: 6552 6573 756c 7453 6574 2872 6573 756c  eResultSet(resul
+00006f40: 7429 0a0a 2020 2020 6578 6365 7074 2045  t)..    except E
+00006f50: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
+00006f60: 2020 2020 2020 2020 6578 2e61 7267 7320          ex.args 
+00006f70: 3d20 2866 2261 6464 5f63 6f6c 756d 6e20  = (f"add_column 
+00006f80: 6572 726f 7220 666f 7220 7b70 6174 687d  error for {path}
+00006f90: 2e7b 6c61 7965 727d 3a5c 6e20 207b 6578  .{layer}:\n  {ex
+00006fa0: 7d22 2c29 0a20 2020 2020 2020 2072 6169  }",).        rai
+00006fb0: 7365 0a20 2020 2066 696e 616c 6c79 3a0a  se.    finally:.
+00006fc0: 2020 2020 2020 2020 6461 7461 736f 7572          datasour
+00006fd0: 6365 203d 204e 6f6e 650a 0a0a 6465 6620  ce = None...def 
+00006fe0: 6472 6f70 5f63 6f6c 756d 6e28 0a20 2020  drop_column(.   
+00006ff0: 2070 6174 683a 2055 6e69 6f6e 5b73 7472   path: Union[str
+00007000: 2c20 226f 732e 5061 7468 4c69 6b65 5b41  , "os.PathLike[A
+00007010: 6e79 5d22 5d2c 2063 6f6c 756d 6e5f 6e61  ny]"], column_na
+00007020: 6d65 3a20 7374 722c 206c 6179 6572 3a20  me: str, layer: 
+00007030: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00007040: 4e6f 6e65 0a29 3a0a 2020 2020 2222 220a  None.):.    """.
+00007050: 2020 2020 4472 6f70 2074 6865 2063 6f6c      Drop the col
+00007060: 756d 6e20 7370 6563 6966 6965 642e 0a0a  umn specified...
+00007070: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00007080: 2020 7061 7468 2028 5061 7468 4c69 6b65    path (PathLike
+00007090: 293a 2054 6865 2066 696c 6520 7061 7468  ): The file path
+000070a0: 2e0a 2020 2020 2020 2020 636f 6c75 6d6e  ..        column
+000070b0: 5f6e 616d 6520 2873 7472 293a 2074 6865  _name (str): the
+000070c0: 2063 6f6c 756d 6e20 6e61 6d65 2e0a 2020   column name..  
+000070d0: 2020 2020 2020 6c61 7965 7220 284f 7074        layer (Opt
+000070e0: 696f 6e61 6c5b 7374 725d 293a 2054 6865  ional[str]): The
+000070f0: 206c 6179 6572 206e 616d 652e 2049 6620   layer name. If 
+00007100: 6e6f 7420 7370 6563 6966 6965 642c 2061  not specified, a
+00007110: 6e64 2074 6865 7265 2069 7320 6f6e 6c79  nd there is only
+00007120: 0a20 2020 2020 2020 2020 2020 206f 6e65  .            one
+00007130: 206c 6179 6572 2069 6e20 7468 6520 6669   layer in the fi
+00007140: 6c65 2c20 7468 6973 206c 6179 6572 2069  le, this layer i
+00007150: 7320 7573 6564 2e20 4f74 6865 7277 6973  s used. Otherwis
+00007160: 6520 6120 5661 6c75 6545 7272 6f72 2069  e a ValueError i
+00007170: 730a 2020 2020 2020 2020 2020 2020 7261  s.            ra
+00007180: 6973 6564 2e0a 2020 2020 2222 220a 2020  ised..    """.  
+00007190: 2020 2320 4368 6563 6b20 696e 7075 7420    # Check input 
+000071a0: 7061 7261 6d65 7465 7273 0a20 2020 2070  parameters.    p
+000071b0: 6174 6820 3d20 5061 7468 2870 6174 6829  ath = Path(path)
+000071c0: 0a20 2020 2069 6620 6c61 7965 7220 6973  .    if layer is
+000071d0: 204e 6f6e 653a 0a20 2020 2020 2020 206c   None:.        l
+000071e0: 6179 6572 203d 2067 6574 5f6f 6e6c 795f  ayer = get_only_
+000071f0: 6c61 7965 7228 7061 7468 290a 2020 2020  layer(path).    
+00007200: 696e 666f 203d 2067 6574 5f6c 6179 6572  info = get_layer
+00007210: 696e 666f 2870 6174 682c 206c 6179 6572  info(path, layer
+00007220: 290a 2020 2020 6966 2063 6f6c 756d 6e5f  ).    if column_
+00007230: 6e61 6d65 206e 6f74 2069 6e20 696e 666f  name not in info
+00007240: 2e63 6f6c 756d 6e73 3a0a 2020 2020 2020  .columns:.      
+00007250: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
+00007260: 436f 6c75 6d6e 207b 636f 6c75 6d6e 5f6e  Column {column_n
+00007270: 616d 657d 206e 6f74 2070 7265 7365 6e74  ame} not present
+00007280: 2073 6f20 6361 6e6e 6f74 2062 6520 6472   so cannot be dr
+00007290: 6f70 7065 642e 2229 0a20 2020 2020 2020  opped.").       
+000072a0: 2072 6574 7572 6e0a 0a20 2020 2023 204e   return..    # N
+000072b0: 6f77 2072 6561 6c6c 7920 7265 6e61 6d65  ow really rename
+000072c0: 0a20 2020 2064 6174 6173 6f75 7263 6520  .    datasource 
+000072d0: 3d20 4e6f 6e65 0a20 2020 2074 7279 3a0a  = None.    try:.
+000072e0: 2020 2020 2020 2020 6461 7461 736f 7572          datasour
+000072f0: 6365 203d 2067 6461 6c2e 4f70 656e 4578  ce = gdal.OpenEx
+00007300: 2873 7472 2870 6174 6829 2c20 6e4f 7065  (str(path), nOpe
+00007310: 6e46 6c61 6773 3d67 6461 6c2e 4f46 5f55  nFlags=gdal.OF_U
+00007320: 5044 4154 4529 0a20 2020 2020 2020 2073  PDATE).        s
+00007330: 716c 5f73 746d 7420 3d20 6627 414c 5445  ql_stmt = f'ALTE
+00007340: 5220 5441 424c 4520 227b 6c61 7965 727d  R TABLE "{layer}
+00007350: 2220 4452 4f50 2043 4f4c 554d 4e20 227b  " DROP COLUMN "{
+00007360: 636f 6c75 6d6e 5f6e 616d 657d 2227 0a20  column_name}"'. 
+00007370: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00007380: 6461 7461 736f 7572 6365 2e45 7865 6375  datasource.Execu
+00007390: 7465 5351 4c28 7371 6c5f 7374 6d74 290a  teSQL(sql_stmt).
+000073a0: 2020 2020 2020 2020 6461 7461 736f 7572          datasour
+000073b0: 6365 2e52 656c 6561 7365 5265 7375 6c74  ce.ReleaseResult
+000073c0: 5365 7428 7265 7375 6c74 290a 0a20 2020  Set(result)..   
+000073d0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000073e0: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
+000073f0: 2065 782e 6172 6773 203d 2028 6622 6472   ex.args = (f"dr
+00007400: 6f70 5f63 6f6c 756d 6e20 6572 726f 7220  op_column error 
+00007410: 666f 7220 7b70 6174 687d 2e7b 6c61 7965  for {path}.{laye
+00007420: 727d 3a5c 6e20 207b 6578 7d22 2c29 0a20  r}:\n  {ex}",). 
+00007430: 2020 2020 2020 2072 6169 7365 0a20 2020         raise.   
+00007440: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
+00007450: 2020 6461 7461 736f 7572 6365 203d 204e    datasource = N
+00007460: 6f6e 650a 0a0a 6465 6620 7570 6461 7465  one...def update
+00007470: 5f63 6f6c 756d 6e28 0a20 2020 2070 6174  _column(.    pat
+00007480: 683a 2055 6e69 6f6e 5b73 7472 2c20 226f  h: Union[str, "o
+00007490: 732e 5061 7468 4c69 6b65 5b41 6e79 5d22  s.PathLike[Any]"
+000074a0: 5d2c 0a20 2020 206e 616d 653a 2073 7472  ],.    name: str
+000074b0: 2c0a 2020 2020 6578 7072 6573 7369 6f6e  ,.    expression
+000074c0: 3a20 7374 722c 0a20 2020 206c 6179 6572  : str,.    layer
+000074d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000074e0: 3d20 4e6f 6e65 2c0a 2020 2020 7768 6572  = None,.    wher
+000074f0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+00007500: 203d 204e 6f6e 652c 0a29 3a0a 2020 2020   = None,.):.    
+00007510: 2222 220a 2020 2020 5570 6461 7465 2061  """.    Update a
+00007520: 2063 6f6c 756d 6e20 6672 6f6d 2061 206c   column from a l
+00007530: 6179 6572 206f 6620 7468 6520 6765 6f66  ayer of the geof
+00007540: 696c 652e 0a0a 2020 2020 4172 6773 3a0a  ile...    Args:.
+00007550: 2020 2020 2020 2020 7061 7468 2028 5061          path (Pa
+00007560: 7468 4c69 6b65 293a 2050 6174 6820 746f  thLike): Path to
+00007570: 2074 6865 2067 656f 6669 6c65 0a20 2020   the geofile.   
+00007580: 2020 2020 206e 616d 6520 2873 7472 293a       name (str):
+00007590: 204e 616d 6520 666f 7220 7468 6520 6e65   Name for the ne
+000075a0: 7720 636f 6c75 6d6e 0a20 2020 2020 2020  w column.       
+000075b0: 2065 7870 7265 7373 696f 6e20 2873 7472   expression (str
+000075c0: 293a 2053 514c 6974 6520 6578 7072 6573  ): SQLite expres
+000075d0: 7369 6f6e 2074 6f20 7573 6520 746f 2075  sion to use to u
+000075e0: 7064 6174 650a 2020 2020 2020 2020 2020  pdate.          
+000075f0: 2020 7468 6520 7661 6c75 652e 0a20 2020    the value..   
+00007600: 2020 2020 206c 6179 6572 2028 7374 722c       layer (str,
+00007610: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00007620: 6c61 7965 7220 6e61 6d65 2e20 4966 204e  layer name. If N
+00007630: 6f6e 6520 616e 6420 7468 6520 6765 6f66  one and the geof
+00007640: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
+00007650: 6861 7320 6f6e 6c79 206f 6e65 206c 6179  has only one lay
+00007660: 6572 2c20 7468 6174 206c 6179 6572 2069  er, that layer i
+00007670: 7320 7573 6564 2e20 4465 6661 756c 7473  s used. Defaults
+00007680: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
+00007690: 2020 6c61 7965 7220 2873 7472 2c20 6f70    layer (str, op
+000076a0: 7469 6f6e 616c 293a 2053 514c 2077 6865  tional): SQL whe
+000076b0: 7265 2063 6c61 7573 6520 746f 2072 6573  re clause to res
+000076c0: 7472 6963 7420 7468 6520 726f 7773 2074  trict the rows t
+000076d0: 6861 7420 7769 6c6c 0a20 2020 2020 2020  hat will.       
+000076e0: 2020 2020 2062 6520 7570 6461 7465 642e       be updated.
+000076f0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00007700: 652e 0a0a 2020 2020 5261 6973 6573 3a0a  e...    Raises:.
+00007710: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+00007720: 6f72 3a20 616e 2069 6e76 616c 6964 2070  or: an invalid p
+00007730: 6172 616d 6574 6572 2076 616c 7565 2077  arameter value w
+00007740: 6173 2070 6173 7365 642e 0a20 2020 2022  as passed..    "
+00007750: 2222 0a0a 2020 2020 2320 496e 6974 0a20  ""..    # Init. 
+00007760: 2020 2070 6174 6820 3d20 5061 7468 2870     path = Path(p
+00007770: 6174 6829 0a20 2020 2069 6620 6c61 7965  ath).    if laye
+00007780: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+00007790: 2020 206c 6179 6572 203d 2067 6574 5f6f     layer = get_o
+000077a0: 6e6c 795f 6c61 7965 7228 7061 7468 290a  nly_layer(path).
+000077b0: 2020 2020 6c61 7965 7269 6e66 6f5f 6f72      layerinfo_or
+000077c0: 6967 203d 2067 6574 5f6c 6179 6572 696e  ig = get_layerin
+000077d0: 666f 2870 6174 682c 206c 6179 6572 290a  fo(path, layer).
+000077e0: 2020 2020 636f 6c75 6d6e 735f 7570 7065      columns_uppe
+000077f0: 7220 3d20 5b63 6f6c 756d 6e2e 7570 7065  r = [column.uppe
+00007800: 7228 2920 666f 7220 636f 6c75 6d6e 2069  r() for column i
+00007810: 6e20 6c61 7965 7269 6e66 6f5f 6f72 6967  n layerinfo_orig
+00007820: 2e63 6f6c 756d 6e73 5d0a 2020 2020 6966  .columns].    if
+00007830: 206e 616d 652e 7570 7065 7228 2920 6e6f   name.upper() no
+00007840: 7420 696e 2063 6f6c 756d 6e73 5f75 7070  t in columns_upp
+00007850: 6572 3a0a 2020 2020 2020 2020 2320 4966  er:.        # If
+00007860: 2063 6f6c 756d 6e20 646f 6573 6e27 7420   column doesn't 
+00007870: 6578 6973 7420 7965 742c 2065 7272 6f72  exist yet, error
+00007880: 210a 2020 2020 2020 2020 7261 6973 6520  !.        raise 
+00007890: 5661 6c75 6545 7272 6f72 2866 2243 6f6c  ValueError(f"Col
+000078a0: 756d 6e20 7b6e 616d 657d 2064 6f65 736e  umn {name} doesn
+000078b0: 2774 2065 7869 7374 2069 6e20 7b70 6174  't exist in {pat
+000078c0: 687d 2c20 6c61 7965 7220 7b6c 6179 6572  h}, layer {layer
+000078d0: 7d22 290a 0a20 2020 2023 2047 6f21 0a20  }")..    # Go!. 
+000078e0: 2020 2064 6174 6173 6f75 7263 6520 3d20     datasource = 
+000078f0: 4e6f 6e65 0a20 2020 2074 7279 3a0a 2020  None.    try:.  
+00007900: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
+00007910: 203d 2067 6461 6c2e 4f70 656e 4578 2873   = gdal.OpenEx(s
+00007920: 7472 2870 6174 6829 2c20 6e4f 7065 6e46  tr(path), nOpenF
+00007930: 6c61 6773 3d67 6461 6c2e 4f46 5f55 5044  lags=gdal.OF_UPD
+00007940: 4154 4529 0a20 2020 2020 2020 2073 716c  ATE).        sql
+00007950: 6974 655f 7374 6d74 203d 2066 2755 5044  ite_stmt = f'UPD
+00007960: 4154 4520 227b 6c61 7965 727d 2220 5345  ATE "{layer}" SE
+00007970: 5420 227b 6e61 6d65 7d22 203d 207b 6578  T "{name}" = {ex
+00007980: 7072 6573 7369 6f6e 7d27 0a20 2020 2020  pression}'.     
+00007990: 2020 2069 6620 7768 6572 6520 6973 206e     if where is n
+000079a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000079b0: 2020 2020 2073 716c 6974 655f 7374 6d74       sqlite_stmt
+000079c0: 202b 3d20 6622 5c6e 2057 4845 5245 207b   += f"\n WHERE {
+000079d0: 7768 6572 657d 220a 2020 2020 2020 2020  where}".        
+000079e0: 7265 7375 6c74 203d 2064 6174 6173 6f75  result = datasou
+000079f0: 7263 652e 4578 6563 7574 6553 514c 2873  rce.ExecuteSQL(s
+00007a00: 716c 6974 655f 7374 6d74 2c20 6469 616c  qlite_stmt, dial
+00007a10: 6563 743d 2253 514c 4954 4522 290a 2020  ect="SQLITE").  
+00007a20: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
+00007a30: 2e52 656c 6561 7365 5265 7375 6c74 5365  .ReleaseResultSe
+00007a40: 7428 7265 7375 6c74 290a 0a20 2020 2065  t(result)..    e
+00007a50: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00007a60: 6173 2065 783a 0a20 2020 2020 2020 2065  as ex:.        e
+00007a70: 782e 6172 6773 203d 2028 6622 7570 6461  x.args = (f"upda
+00007a80: 7465 5f63 6f6c 756d 6e20 6572 726f 7220  te_column error 
+00007a90: 666f 7220 7b70 6174 687d 2e7b 6c61 7965  for {path}.{laye
+00007aa0: 727d 3a5c 6e20 207b 6578 7d22 2c29 0a20  r}:\n  {ex}",). 
+00007ab0: 2020 2020 2020 2072 6169 7365 0a20 2020         raise.   
+00007ac0: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
+00007ad0: 2020 6461 7461 736f 7572 6365 203d 204e    datasource = N
+00007ae0: 6f6e 650a 0a0a 6465 6620 7265 6164 5f66  one...def read_f
+00007af0: 696c 6528 0a20 2020 2070 6174 683a 2055  ile(.    path: U
+00007b00: 6e69 6f6e 5b73 7472 2c20 226f 732e 5061  nion[str, "os.Pa
+00007b10: 7468 4c69 6b65 5b41 6e79 5d22 5d2c 0a20  thLike[Any]"],. 
+00007b20: 2020 206c 6179 6572 3a20 4f70 7469 6f6e     layer: Option
+00007b30: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00007b40: 2020 2020 636f 6c75 6d6e 733a 204f 7074      columns: Opt
+00007b50: 696f 6e61 6c5b 4974 6572 6162 6c65 5b73  ional[Iterable[s
+00007b60: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+00007b70: 2062 626f 783d 4e6f 6e65 2c0a 2020 2020   bbox=None,.    
+00007b80: 726f 7773 3d4e 6f6e 652c 0a20 2020 2073  rows=None,.    s
+00007b90: 716c 5f73 746d 743a 204f 7074 696f 6e61  ql_stmt: Optiona
+00007ba0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00007bb0: 2020 2073 716c 5f64 6961 6c65 6374 3a20     sql_dialect: 
+00007bc0: 4f70 7469 6f6e 616c 5b4c 6974 6572 616c  Optional[Literal
+00007bd0: 5b22 5351 4c49 5445 222c 2022 4f47 5253  ["SQLITE", "OGRS
+00007be0: 514c 225d 5d20 3d20 4e6f 6e65 2c0a 2020  QL"]] = None,.  
+00007bf0: 2020 6967 6e6f 7265 5f67 656f 6d65 7472    ignore_geometr
+00007c00: 793a 2062 6f6f 6c20 3d20 4661 6c73 652c  y: bool = False,
+00007c10: 0a20 2020 2066 6964 5f61 735f 696e 6465  .    fid_as_inde
+00007c20: 783a 2062 6f6f 6c20 3d20 4661 6c73 652c  x: bool = False,
+00007c30: 0a29 202d 3e20 6770 642e 4765 6f44 6174  .) -> gpd.GeoDat
+00007c40: 6146 7261 6d65 3a0a 2020 2020 2222 220a  aFrame:.    """.
+00007c50: 2020 2020 5265 6164 7320 6120 6669 6c65      Reads a file
+00007c60: 2074 6f20 6120 6765 6f70 616e 6461 7320   to a geopandas 
+00007c70: 4765 6f44 6174 6166 7261 6d65 2e0a 0a20  GeoDataframe... 
+00007c80: 2020 2054 6865 2066 696c 6520 666f 726d     The file form
+00007c90: 6174 2069 7320 6465 7465 6374 6564 2062  at is detected b
+00007ca0: 6173 6564 206f 6e20 7468 6520 6669 6c65  ased on the file
+00007cb0: 7061 7468 2065 7874 656e 7369 6f6e 2e0a  path extension..
+00007cc0: 0a20 2020 2049 6620 616e 2073 716c 5f73  .    If an sql_s
+00007cd0: 746d 7420 6973 2073 7065 6369 6669 6564  tmt is specified
+00007ce0: 2c20 7468 6520 7371 6c69 7465 2071 7565  , the sqlite que
+00007cf0: 7279 2063 616e 2063 6f6e 7461 696e 2066  ry can contain f
+00007d00: 6f6c 6c6f 7769 6e67 2070 6c61 6365 686f  ollowing placeho
+00007d10: 6c64 6572 730a 2020 2020 7468 6174 2077  lders.    that w
+00007d20: 696c 6c20 6265 2061 7574 6f6d 6174 6963  ill be automatic
+00007d30: 616c 6c79 2072 6570 6c61 6365 6420 666f  ally replaced fo
+00007d40: 7220 796f 753a 0a0a 2020 2020 2020 2a20  r you:..      * 
+00007d50: 7b67 656f 6d65 7472 7963 6f6c 756d 6e7d  {geometrycolumn}
+00007d60: 3a20 7468 6520 636f 6c75 6d6e 2077 6865  : the column whe
+00007d70: 7265 2074 6865 2070 7269 6d61 7279 2067  re the primary g
+00007d80: 656f 6d65 7472 7920 6973 2073 746f 7265  eometry is store
+00007d90: 642e 0a20 2020 2020 202a 207b 636f 6c75  d..      * {colu
+00007da0: 6d6e 735f 746f 5f73 656c 6563 745f 7374  mns_to_select_st
+00007db0: 727d 3a20 6966 2027 636f 6c75 6d6e 7327  r}: if 'columns'
+00007dc0: 2069 7320 6e6f 7420 4e6f 6e65 2c20 7468   is not None, th
+00007dd0: 6f73 6520 636f 6c75 6d6e 732c 0a20 2020  ose columns,.   
+00007de0: 2020 2020 206f 7468 6572 7769 7365 2061       otherwise a
+00007df0: 6c6c 2063 6f6c 756d 6e73 206f 6620 7468  ll columns of th
+00007e00: 6520 6c61 7965 722e 0a20 2020 2020 202a  e layer..      *
+00007e10: 207b 696e 7075 745f 6c61 7965 727d 3a20   {input_layer}: 
+00007e20: 7468 6520 6c61 7965 7220 6e61 6d65 206f  the layer name o
+00007e30: 6620 7468 6520 696e 7075 7420 6c61 7965  f the input laye
+00007e40: 722e 0a0a 2020 2020 4578 616d 706c 6520  r...    Example 
+00007e50: 7371 6c20 7374 6174 656d 656e 7420 7769  sql statement wi
+00007e60: 7468 2070 6c61 6365 686f 6c64 6572 733a  th placeholders:
+00007e70: 0a20 2020 203a 3a0a 0a20 2020 2020 2020  .    ::..       
+00007e80: 2053 454c 4543 5420 7b67 656f 6d65 7472   SELECT {geometr
+00007e90: 7963 6f6c 756d 6e7d 0a20 2020 2020 2020  ycolumn}.       
+00007ea0: 2020 2020 2020 207b 636f 6c75 6d6e 735f         {columns_
+00007eb0: 746f 5f73 656c 6563 745f 7374 727d 0a20  to_select_str}. 
+00007ec0: 2020 2020 2020 2020 2046 524f 4d20 227b           FROM "{
+00007ed0: 696e 7075 745f 6c61 7965 727d 2220 6c61  input_layer}" la
+00007ee0: 7965 720a 0a20 2020 2054 6865 2075 6e64  yer..    The und
+00007ef0: 6572 6c79 696e 6720 6c69 6272 6172 7920  erlying library 
+00007f00: 7573 6564 2074 6f20 7265 6164 2074 6865  used to read the
+00007f10: 2066 696c 6520 6361 6e20 6265 2063 686f   file can be cho
+00007f20: 6f73 656e 2075 7369 6e67 2074 6865 0a20  osen using the. 
+00007f30: 2020 2022 4746 4f5f 494f 5f45 4e47 494e     "GFO_IO_ENGIN
+00007f40: 4522 2065 6e76 6972 6f6e 6d65 6e74 2076  E" environment v
+00007f50: 6172 6961 626c 652e 2050 6f73 7369 626c  ariable. Possibl
+00007f60: 6520 7661 6c75 6573 2061 7265 2022 6669  e values are "fi
+00007f70: 6f6e 6122 2061 6e64 2022 7079 6f67 7269  ona" and "pyogri
+00007f80: 6f22 2e0a 2020 2020 5468 6973 206f 7074  o"..    This opt
+00007f90: 696f 6e20 6973 2063 7265 6174 6564 2061  ion is created a
+00007fa0: 7320 6120 7465 6d70 6f72 6172 7920 6661  s a temporary fa
+00007fb0: 6c6c 6261 636b 2074 6f20 2266 696f 6e61  llback to "fiona
+00007fc0: 2220 666f 7220 6361 7365 7320 7768 6572  " for cases wher
+00007fd0: 6520 2270 796f 6772 696f 220a 2020 2020  e "pyogrio".    
+00007fe0: 6769 7665 7320 6973 7375 6573 2c20 736f  gives issues, so
+00007ff0: 2070 6c65 6173 6520 7265 706f 7274 2069   please report i
+00008000: 7373 7565 7320 6966 2074 6865 7920 6172  ssues if they ar
+00008010: 6520 656e 636f 756e 7465 7265 642e 2049  e encountered. I
+00008020: 6e20 7468 6520 6675 7475 7265 2073 7570  n the future sup
+00008030: 706f 7274 0a20 2020 2066 6f72 2074 6865  port.    for the
+00008040: 2022 6669 6f6e 6122 2065 6e67 696e 6520   "fiona" engine 
+00008050: 6d6f 7374 206c 696b 656c 7920 7769 6c6c  most likely will
+00008060: 2062 6520 7265 6d6f 7665 642e 2044 6566   be removed. Def
+00008070: 6175 6c74 2065 6e67 696e 6520 6973 2022  ault engine is "
+00008080: 7079 6f67 7269 6f22 2e0a 0a20 2020 2041  pyogrio"...    A
+00008090: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+000080a0: 6820 2866 696c 6520 7061 7468 293a 2070  h (file path): p
+000080b0: 6174 6820 746f 2074 6865 2066 696c 6520  ath to the file 
+000080c0: 746f 2072 6561 6420 6672 6f6d 0a20 2020  to read from.   
+000080d0: 2020 2020 206c 6179 6572 2028 7374 722c       layer (str,
+000080e0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+000080f0: 6c61 7965 7220 746f 2072 6561 642e 2044  layer to read. D
+00008100: 6566 6175 6c74 7320 746f 204e 6f6e 652c  efaults to None,
+00008110: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00008120: 6e20 7265 6164 7320 7468 6520 6f6e 6c79  n reads the only
+00008130: 206c 6179 6572 2069 6e20 7468 6520 6669   layer in the fi
+00008140: 6c65 206f 7220 7468 726f 7773 2065 7272  le or throws err
+00008150: 6f72 2e0a 2020 2020 2020 2020 636f 6c75  or..        colu
+00008160: 6d6e 7320 2849 7465 7261 626c 655b 7374  mns (Iterable[st
+00008170: 725d 2c20 6f70 7469 6f6e 616c 293a 2054  r], optional): T
+00008180: 6865 2028 6e6f 6e2d 6765 6f6d 6574 7279  he (non-geometry
+00008190: 2920 636f 6c75 6d6e 7320 746f 2072 6561  ) columns to rea
+000081a0: 6420 7769 6c6c 0a20 2020 2020 2020 2020  d will.         
+000081b0: 2020 2062 6520 7265 7475 726e 6564 2069     be returned i
+000081c0: 6e20 7468 6520 6f72 6465 7220 7370 6563  n the order spec
+000081d0: 6966 6965 642e 2049 6620 4e6f 6e65 2c20  ified. If None, 
+000081e0: 616c 6c20 7374 616e 6461 7264 2063 6f6c  all standard col
+000081f0: 756d 6e73 2061 7265 2072 6561 642e 0a20  umns are read.. 
+00008200: 2020 2020 2020 2020 2020 2049 6e20 6164             In ad
+00008210: 6469 7469 6f6e 2074 6f20 7374 616e 6461  dition to standa
+00008220: 7264 2063 6f6c 756d 6e73 2c20 6974 2069  rd columns, it i
+00008230: 7320 616c 736f 2070 6f73 7369 626c 650a  s also possible.
+00008240: 2020 2020 2020 2020 2020 2020 746f 2073              to s
+00008250: 7065 6369 6679 2022 6669 6422 2c20 6120  pecify "fid", a 
+00008260: 756e 6971 7565 2069 6e64 6578 2061 7661  unique index ava
+00008270: 696c 6162 6c65 2069 6e20 616c 6c20 696e  ilable in all in
+00008280: 7075 7420 6669 6c65 732e 204e 6f74 6520  put files. Note 
+00008290: 7468 6174 2074 6865 0a20 2020 2020 2020  that the.       
+000082a0: 2020 2020 2022 6669 6422 2077 696c 6c20       "fid" will 
+000082b0: 6265 2061 6c69 6173 6564 2065 672e 2074  be aliased eg. t
+000082c0: 6f20 2266 6964 5f31 222e 2044 6566 6175  o "fid_1". Defau
+000082d0: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
+000082e0: 2020 2020 2062 626f 7820 285b 7479 7065       bbox ([type
+000082f0: 5d2c 206f 7074 696f 6e61 6c29 3a20 5265  ], optional): Re
+00008300: 6164 206f 6e6c 7920 6765 6f6d 6574 7269  ad only geometri
+00008310: 6573 2069 6e74 6572 7365 6374 696e 6720  es intersecting 
+00008320: 7468 6973 2062 626f 782e 0a20 2020 2020  this bbox..     
+00008330: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00008340: 746f 204e 6f6e 652c 2074 6865 6e20 616c  to None, then al
+00008350: 6c20 726f 7773 2061 7265 2072 6561 642e  l rows are read.
+00008360: 0a20 2020 2020 2020 2072 6f77 7320 285b  .        rows ([
+00008370: 7479 7065 5d2c 206f 7074 696f 6e61 6c29  type], optional)
+00008380: 3a20 5265 6164 206f 6e6c 7920 7468 6520  : Read only the 
+00008390: 726f 7773 2073 7065 6369 6669 6564 2e0a  rows specified..
+000083a0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+000083b0: 756c 7473 2074 6f20 4e6f 6e65 2c20 7468  ults to None, th
+000083c0: 656e 2061 6c6c 2072 6f77 7320 6172 6520  en all rows are 
+000083d0: 7265 6164 2e0a 2020 2020 2020 2020 7371  read..        sq
+000083e0: 6c5f 7374 6d74 2028 7374 7229 3a20 7371  l_stmt (str): sq
+000083f0: 6c20 7374 6174 656d 656e 7420 746f 2075  l statement to u
+00008400: 7365 2e20 4f6e 6c79 2073 7570 706f 7274  se. Only support
+00008410: 6564 2077 6974 6820 2270 796f 6772 696f  ed with "pyogrio
+00008420: 2220 656e 6769 6e65 2e0a 2020 2020 2020  " engine..      
+00008430: 2020 7371 6c5f 6469 616c 6563 7420 2873    sql_dialect (s
+00008440: 7472 2c20 6f70 7469 6f6e 616c 293a 2053  tr, optional): S
+00008450: 716c 2064 6961 6c65 6374 2075 7365 642e  ql dialect used.
+00008460: 2049 6620 4e6f 6e65 2c20 666f 7220 6461   If None, for da
+00008470: 7461 2073 6f75 7263 6573 2077 6974 680a  ta sources with.
+00008480: 2020 2020 2020 2020 2020 2020 6578 706c              expl
+00008490: 6963 6974 2053 514c 2073 7570 706f 7274  icit SQL support
+000084a0: 2074 6865 2073 7461 7465 6d65 6e74 2069   the statement i
+000084b0: 7320 7072 6f63 6573 7365 6420 6279 2074  s processed by t
+000084c0: 6865 2064 6566 6175 6c74 2053 514c 2065  he default SQL e
+000084d0: 6e67 696e 650a 2020 2020 2020 2020 2020  ngine.          
+000084e0: 2020 2865 2e67 2e20 506f 7374 4749 532c    (e.g. PostGIS,
+000084f0: 2047 656f 7061 636b 6167 652c 2053 7061   Geopackage, Spa
+00008500: 7469 616c 6974 652c 2e2e 2e29 2e20 466f  tialite,...). Fo
+00008510: 7220 6461 7461 2073 6f75 7263 6573 0a20  r data sources. 
+00008520: 2020 2020 2020 2020 2020 2077 6974 686f             witho
+00008530: 7574 2053 514c 2073 7570 706f 7274 2c20  ut SQL support, 
+00008540: 7468 6520 224f 4752 5351 4c22 2064 6961  the "OGRSQL" dia
+00008550: 6c65 6374 2069 7320 7468 6520 6465 6661  lect is the defa
+00008560: 756c 742e 2044 6566 6175 6c74 7320 746f  ult. Defaults to
+00008570: 204e 6f6e 652e 0a20 2020 2020 2020 2069   None..        i
+00008580: 676e 6f72 655f 6765 6f6d 6574 7279 2028  gnore_geometry (
+00008590: 626f 6f6c 2c20 6f70 7469 6f6e 616c 293a  bool, optional):
+000085a0: 2054 7275 6520 6e6f 7420 746f 2072 6561   True not to rea
+000085b0: 642f 7265 7475 726e 2074 6865 2067 656f  d/return the geo
+000085c0: 6d65 7472 792e 0a20 2020 2020 2020 2020  metry..         
+000085d0: 2020 2044 6566 6175 6c74 7320 746f 2046     Defaults to F
+000085e0: 616c 7365 2e0a 2020 2020 2020 2020 6669  alse..        fi
+000085f0: 645f 6173 5f69 6e64 6578 2028 626f 6f6c  d_as_index (bool
+00008600: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00008610: 5472 7565 2c20 7769 6c6c 2075 7365 2074  True, will use t
+00008620: 6865 2046 4944 7320 6f66 2074 6865 2066  he FIDs of the f
+00008630: 6561 7475 7265 7320 7468 6174 0a20 2020  eatures that.   
+00008640: 2020 2020 2020 2020 2077 6572 6520 7265           were re
+00008650: 6164 2061 7320 7468 6520 696e 6465 7820  ad as the index 
+00008660: 6f66 2074 6865 2047 656f 4461 7461 4672  of the GeoDataFr
+00008670: 616d 652e 204d 6179 2073 7461 7274 2061  ame. May start a
+00008680: 7420 3020 6f72 2031 2064 6570 656e 6469  t 0 or 1 dependi
+00008690: 6e67 206f 6e0a 2020 2020 2020 2020 2020  ng on.          
+000086a0: 2020 7468 6520 6472 6976 6572 2e20 4465    the driver. De
+000086b0: 6661 756c 7473 2074 6f20 4661 6c73 652e  faults to False.
+000086c0: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
+000086d0: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+000086e0: 3a20 616e 2069 6e76 616c 6964 2070 6172  : an invalid par
+000086f0: 616d 6574 6572 2076 616c 7565 2077 6173  ameter value was
+00008700: 2070 6173 7365 642e 0a0a 2020 2020 5265   passed...    Re
+00008710: 7475 726e 733a 0a20 2020 2020 2020 2067  turns:.        g
+00008720: 7064 2e47 656f 4461 7461 4672 616d 653a  pd.GeoDataFrame:
+00008730: 2074 6865 2064 6174 6120 7265 6164 2e0a   the data read..
+00008740: 2020 2020 2222 220a 2020 2020 7265 7375      """.    resu
+00008750: 6c74 5f67 6466 203d 205f 7265 6164 5f66  lt_gdf = _read_f
+00008760: 696c 655f 6261 7365 280a 2020 2020 2020  ile_base(.      
+00008770: 2020 7061 7468 3d70 6174 682c 0a20 2020    path=path,.   
+00008780: 2020 2020 206c 6179 6572 3d6c 6179 6572       layer=layer
+00008790: 2c0a 2020 2020 2020 2020 636f 6c75 6d6e  ,.        column
+000087a0: 733d 636f 6c75 6d6e 732c 0a20 2020 2020  s=columns,.     
+000087b0: 2020 2062 626f 783d 6262 6f78 2c0a 2020     bbox=bbox,.  
+000087c0: 2020 2020 2020 726f 7773 3d72 6f77 732c        rows=rows,
+000087d0: 0a20 2020 2020 2020 2073 716c 5f73 746d  .        sql_stm
+000087e0: 743d 7371 6c5f 7374 6d74 2c0a 2020 2020  t=sql_stmt,.    
+000087f0: 2020 2020 7371 6c5f 6469 616c 6563 743d      sql_dialect=
+00008800: 7371 6c5f 6469 616c 6563 742c 0a20 2020  sql_dialect,.   
+00008810: 2020 2020 2069 676e 6f72 655f 6765 6f6d       ignore_geom
+00008820: 6574 7279 3d69 676e 6f72 655f 6765 6f6d  etry=ignore_geom
+00008830: 6574 7279 2c0a 2020 2020 2020 2020 6669  etry,.        fi
 00008840: 645f 6173 5f69 6e64 6578 3d66 6964 5f61  d_as_index=fid_a
-00008850: 735f 696e 6465 782c 0a20 2020 2029 0a20  s_index,.    ). 
-00008860: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-00008870: 616e 6365 2872 6573 756c 745f 6764 662c  ance(result_gdf,
-00008880: 2070 642e 4461 7461 4672 616d 6529 0a20   pd.DataFrame). 
-00008890: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000088a0: 5f67 6466 0a0a 0a64 6566 205f 7265 6164  _gdf...def _read
-000088b0: 5f66 696c 655f 6261 7365 280a 2020 2020  _file_base(.    
-000088c0: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
-000088d0: 2022 6f73 2e50 6174 684c 696b 655b 416e   "os.PathLike[An
-000088e0: 795d 225d 2c0a 2020 2020 6c61 7965 723a  y]"],.    layer:
-000088f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00008900: 204e 6f6e 652c 0a20 2020 2063 6f6c 756d   None,.    colum
-00008910: 6e73 3a20 4f70 7469 6f6e 616c 5b49 7465  ns: Optional[Ite
-00008920: 7261 626c 655b 7374 725d 5d20 3d20 4e6f  rable[str]] = No
-00008930: 6e65 2c0a 2020 2020 6262 6f78 3d4e 6f6e  ne,.    bbox=Non
-00008940: 652c 0a20 2020 2072 6f77 733d 4e6f 6e65  e,.    rows=None
-00008950: 2c0a 2020 2020 7371 6c5f 7374 6d74 3a20  ,.    sql_stmt: 
-00008960: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00008970: 4e6f 6e65 2c0a 2020 2020 7371 6c5f 6469  None,.    sql_di
-00008980: 616c 6563 743a 204f 7074 696f 6e61 6c5b  alect: Optional[
-00008990: 4c69 7465 7261 6c5b 2253 514c 4954 4522  Literal["SQLITE"
-000089a0: 2c20 224f 4752 5351 4c22 5d5d 203d 204e  , "OGRSQL"]] = N
-000089b0: 6f6e 652c 0a20 2020 2069 676e 6f72 655f  one,.    ignore_
-000089c0: 6765 6f6d 6574 7279 3a20 626f 6f6c 203d  geometry: bool =
-000089d0: 2046 616c 7365 2c0a 2020 2020 6669 645f   False,.    fid_
-000089e0: 6173 5f69 6e64 6578 3a20 626f 6f6c 203d  as_index: bool =
-000089f0: 2046 616c 7365 2c0a 2920 2d3e 2055 6e69   False,.) -> Uni
-00008a00: 6f6e 5b70 642e 4461 7461 4672 616d 652c  on[pd.DataFrame,
-00008a10: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-00008a20: 655d 3a0a 2020 2020 2222 220a 2020 2020  e]:.    """.    
-00008a30: 5265 6164 7320 6120 6669 6c65 2074 6f20  Reads a file to 
-00008a40: 6120 7061 6e64 6173 2044 6174 6166 7261  a pandas Datafra
-00008a50: 6d65 2e0a 2020 2020 2222 220a 2020 2020  me..    """.    
-00008a60: 2320 4368 6563 6b20 6966 2074 6865 2066  # Check if the f
-00008a70: 6964 2063 6f6c 756d 6e20 6e65 6564 7320  id column needs 
-00008a80: 746f 2062 6520 7265 6164 2061 7320 636f  to be read as co
-00008a90: 6c75 6d6e 2076 6961 2074 6865 2063 6f6c  lumn via the col
-00008aa0: 756d 6e73 2070 6172 616d 6574 6572 0a20  umns parameter. 
-00008ab0: 2020 2066 6964 5f61 735f 636f 6c75 6d6e     fid_as_column
-00008ac0: 203d 2046 616c 7365 0a20 2020 2069 6620   = False.    if 
-00008ad0: 636f 6c75 6d6e 7320 6973 206e 6f74 204e  columns is not N
-00008ae0: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-00008af0: 2266 6964 2220 696e 205b 636f 6c75 6d6e  "fid" in [column
-00008b00: 2e6c 6f77 6572 2829 2066 6f72 2063 6f6c  .lower() for col
-00008b10: 756d 6e20 696e 2063 6f6c 756d 6e73 5d3a  umn in columns]:
-00008b20: 0a20 2020 2020 2020 2020 2020 2066 6964  .            fid
-00008b30: 5f61 735f 636f 6c75 6d6e 203d 2054 7275  _as_column = Tru
-00008b40: 650a 0a20 2020 2023 2052 6561 6420 7769  e..    # Read wi
-00008b50: 7468 2074 6865 2065 6e67 696e 6520 7370  th the engine sp
-00008b60: 6563 6966 6965 640a 2020 2020 656e 6769  ecified.    engi
-00008b70: 6e65 203d 205f 6765 745f 656e 6769 6e65  ne = _get_engine
-00008b80: 2829 0a20 2020 2069 6620 656e 6769 6e65  ().    if engine
-00008b90: 203d 3d20 2270 796f 6772 696f 223a 0a20   == "pyogrio":. 
-00008ba0: 2020 2020 2020 2067 6466 203d 205f 7265         gdf = _re
-00008bb0: 6164 5f66 696c 655f 6261 7365 5f70 796f  ad_file_base_pyo
-00008bc0: 6772 696f 280a 2020 2020 2020 2020 2020  grio(.          
-00008bd0: 2020 7061 7468 3d70 6174 682c 0a20 2020    path=path,.   
-00008be0: 2020 2020 2020 2020 206c 6179 6572 3d6c           layer=l
-00008bf0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
-00008c00: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
-00008c10: 732c 0a20 2020 2020 2020 2020 2020 2062  s,.            b
-00008c20: 626f 783d 6262 6f78 2c0a 2020 2020 2020  box=bbox,.      
-00008c30: 2020 2020 2020 726f 7773 3d72 6f77 732c        rows=rows,
-00008c40: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
-00008c50: 5f73 746d 743d 7371 6c5f 7374 6d74 2c0a  _stmt=sql_stmt,.
-00008c60: 2020 2020 2020 2020 2020 2020 7371 6c5f              sql_
-00008c70: 6469 616c 6563 743d 7371 6c5f 6469 616c  dialect=sql_dial
-00008c80: 6563 742c 0a20 2020 2020 2020 2020 2020  ect,.           
-00008c90: 2069 676e 6f72 655f 6765 6f6d 6574 7279   ignore_geometry
-00008ca0: 3d69 676e 6f72 655f 6765 6f6d 6574 7279  =ignore_geometry
-00008cb0: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
-00008cc0: 645f 6173 5f69 6e64 6578 3d66 6964 5f61  d_as_index=fid_a
-00008cd0: 735f 696e 6465 7820 6f72 2066 6964 5f61  s_index or fid_a
-00008ce0: 735f 636f 6c75 6d6e 2c0a 2020 2020 2020  s_column,.      
-00008cf0: 2020 290a 2020 2020 656c 6966 2065 6e67    ).    elif eng
-00008d00: 696e 6520 3d3d 2022 6669 6f6e 6122 3a0a  ine == "fiona":.
-00008d10: 2020 2020 2020 2020 6764 6620 3d20 5f72          gdf = _r
-00008d20: 6561 645f 6669 6c65 5f62 6173 655f 6669  ead_file_base_fi
-00008d30: 6f6e 6128 0a20 2020 2020 2020 2020 2020  ona(.           
-00008d40: 2070 6174 683d 7061 7468 2c0a 2020 2020   path=path,.    
-00008d50: 2020 2020 2020 2020 6c61 7965 723d 6c61          layer=la
-00008d60: 7965 722c 0a20 2020 2020 2020 2020 2020  yer,.           
-00008d70: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
-00008d80: 2c0a 2020 2020 2020 2020 2020 2020 6262  ,.            bb
-00008d90: 6f78 3d62 626f 782c 0a20 2020 2020 2020  ox=bbox,.       
-00008da0: 2020 2020 2072 6f77 733d 726f 7773 2c0a       rows=rows,.
-00008db0: 2020 2020 2020 2020 2020 2020 7371 6c5f              sql_
-00008dc0: 7374 6d74 3d73 716c 5f73 746d 742c 0a20  stmt=sql_stmt,. 
-00008dd0: 2020 2020 2020 2020 2020 2073 716c 5f64             sql_d
-00008de0: 6961 6c65 6374 3d73 716c 5f64 6961 6c65  ialect=sql_diale
-00008df0: 6374 2c0a 2020 2020 2020 2020 2020 2020  ct,.            
-00008e00: 6967 6e6f 7265 5f67 656f 6d65 7472 793d  ignore_geometry=
-00008e10: 6967 6e6f 7265 5f67 656f 6d65 7472 792c  ignore_geometry,
-00008e20: 0a20 2020 2020 2020 2020 2020 2066 6964  .            fid
-00008e30: 5f61 735f 696e 6465 783d 6669 645f 6173  _as_index=fid_as
-00008e40: 5f69 6e64 6578 206f 7220 6669 645f 6173  _index or fid_as
-00008e50: 5f63 6f6c 756d 6e2c 0a20 2020 2020 2020  _column,.       
-00008e60: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
-00008e70: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00008e80: 4572 726f 7228 6622 556e 7375 7070 6f72  Error(f"Unsuppor
-00008e90: 7465 6420 656e 6769 6e65 3a20 7b65 6e67  ted engine: {eng
-00008ea0: 696e 657d 2229 0a0a 2020 2020 2320 436f  ine}")..    # Co
-00008eb0: 7079 2074 6865 2069 6e64 6578 2074 6f20  py the index to 
-00008ec0: 6120 636f 6c75 6d6e 2069 6620 6e65 6564  a column if need
-00008ed0: 6564 2e2e 2e0a 2020 2020 6966 2066 6964  ed....    if fid
-00008ee0: 5f61 735f 636f 6c75 6d6e 3a0a 2020 2020  _as_column:.    
-00008ef0: 2020 2020 6764 665b 2266 6964 225d 203d      gdf["fid"] =
-00008f00: 2067 6466 2e69 6e64 6578 0a20 2020 2020   gdf.index.     
-00008f10: 2020 2069 6620 6e6f 7420 6669 645f 6173     if not fid_as
-00008f20: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
-00008f30: 2020 2020 6764 6620 3d20 6764 662e 7265      gdf = gdf.re
-00008f40: 7365 745f 696e 6465 7828 6472 6f70 3d54  set_index(drop=T
-00008f50: 7275 6529 0a0a 2020 2020 7265 7475 726e  rue)..    return
-00008f60: 2067 6466 0a0a 0a64 6566 205f 7265 6164   gdf...def _read
-00008f70: 5f66 696c 655f 6261 7365 5f66 696f 6e61  _file_base_fiona
-00008f80: 280a 2020 2020 7061 7468 3a20 556e 696f  (.    path: Unio
-00008f90: 6e5b 7374 722c 2022 6f73 2e50 6174 684c  n[str, "os.PathL
-00008fa0: 696b 655b 416e 795d 225d 2c0a 2020 2020  ike[Any]"],.    
-00008fb0: 6c61 7965 723a 204f 7074 696f 6e61 6c5b  layer: Optional[
-00008fc0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00008fd0: 2063 6f6c 756d 6e73 3a20 4f70 7469 6f6e   columns: Option
-00008fe0: 616c 5b49 7465 7261 626c 655b 7374 725d  al[Iterable[str]
-00008ff0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6262  ] = None,.    bb
-00009000: 6f78 3d4e 6f6e 652c 0a20 2020 2072 6f77  ox=None,.    row
-00009010: 733d 4e6f 6e65 2c0a 2020 2020 7371 6c5f  s=None,.    sql_
-00009020: 7374 6d74 3a20 4f70 7469 6f6e 616c 5b73  stmt: Optional[s
-00009030: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00009040: 7371 6c5f 6469 616c 6563 743a 204f 7074  sql_dialect: Opt
-00009050: 696f 6e61 6c5b 4c69 7465 7261 6c5b 2253  ional[Literal["S
-00009060: 514c 4954 4522 2c20 224f 4752 5351 4c22  QLITE", "OGRSQL"
-00009070: 5d5d 203d 204e 6f6e 652c 0a20 2020 2069  ]] = None,.    i
-00009080: 676e 6f72 655f 6765 6f6d 6574 7279 3a20  gnore_geometry: 
-00009090: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-000090a0: 2020 6669 645f 6173 5f69 6e64 6578 3a20    fid_as_index: 
-000090b0: 626f 6f6c 203d 2046 616c 7365 2c0a 2920  bool = False,.) 
-000090c0: 2d3e 2055 6e69 6f6e 5b70 642e 4461 7461  -> Union[pd.Data
-000090d0: 4672 616d 652c 2067 7064 2e47 656f 4461  Frame, gpd.GeoDa
-000090e0: 7461 4672 616d 655d 3a0a 2020 2020 2222  taFrame]:.    ""
-000090f0: 220a 2020 2020 5265 6164 7320 6120 6669  ".    Reads a fi
-00009100: 6c65 2074 6f20 6120 7061 6e64 6173 2044  le to a pandas D
-00009110: 6174 6166 7261 6d65 2075 7369 6e67 2066  ataframe using f
-00009120: 696f 6e61 2e0a 2020 2020 2222 220a 2020  iona..    """.  
-00009130: 2020 6966 2069 676e 6f72 655f 6765 6f6d    if ignore_geom
-00009140: 6574 7279 2061 6e64 2063 6f6c 756d 6e73  etry and columns
-00009150: 203d 3d20 5b5d 3a0a 2020 2020 2020 2020   == []:.        
-00009160: 7265 7475 726e 2070 642e 4461 7461 4672  return pd.DataFr
-00009170: 616d 6528 290a 2020 2020 6966 2073 716c  ame().    if sql
-00009180: 5f73 746d 7420 6973 206e 6f74 204e 6f6e  _stmt is not Non
-00009190: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-000091a0: 2056 616c 7565 4572 726f 7228 2273 716c   ValueError("sql
-000091b0: 5f73 746d 7420 6973 206e 6f74 2073 7570  _stmt is not sup
-000091c0: 706f 7274 6564 2077 6974 6820 6669 6f6e  ported with fion
-000091d0: 6120 656e 6769 6e65 2229 0a0a 2020 2020  a engine")..    
-000091e0: 2320 496e 6974 0a20 2020 2070 6174 6820  # Init.    path 
-000091f0: 3d20 5061 7468 2870 6174 6829 0a20 2020  = Path(path).   
-00009200: 2069 6620 7061 7468 2e65 7869 7374 7328   if path.exists(
-00009210: 2920 6973 2046 616c 7365 3a0a 2020 2020  ) is False:.    
-00009220: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00009230: 7272 6f72 2866 2266 696c 6520 646f 6573  rror(f"file does
-00009240: 6e27 7420 6578 6973 743a 207b 7061 7468  n't exist: {path
-00009250: 7d22 290a 0a20 2020 2023 2049 6620 6e6f  }")..    # If no
-00009260: 206c 6179 6572 206e 616d 6520 7370 6563   layer name spec
-00009270: 6966 6965 642c 2063 6865 636b 2069 6620  ified, check if 
-00009280: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
-00009290: 6520 6c61 7965 7220 696e 2074 6865 2066  e layer in the f
-000092a0: 696c 652e 0a20 2020 2069 6620 6c61 7965  ile..    if laye
-000092b0: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
-000092c0: 2020 206c 6179 6572 203d 2067 6574 5f6f     layer = get_o
-000092d0: 6e6c 795f 6c61 7965 7228 7061 7468 290a  nly_layer(path).
-000092e0: 0a20 2020 2023 2056 4552 5920 4449 5254  .    # VERY DIRT
-000092f0: 5920 6861 636b 2074 6f20 6765 7420 7468  Y hack to get th
-00009300: 6520 6669 640a 2020 2020 6966 2066 6964  e fid.    if fid
-00009310: 5f61 735f 696e 6465 783a 0a20 2020 2020  _as_index:.     
-00009320: 2020 2023 204d 616b 6520 6120 636f 7079     # Make a copy
-00009330: 2f63 6f70 7920 696e 7075 7420 6669 6c65  /copy input file
-00009340: 2074 6f20 6765 6f70 6163 6b61 6765 2c20   to geopackage, 
-00009350: 6173 2077 6520 7769 6c6c 2061 6464 2061  as we will add a
-00009360: 6e20 6669 642f 726f 7764 2063 6f6c 756d  n fid/rowd colum
-00009370: 6e0a 2020 2020 2020 2020 746d 705f 6669  n.        tmp_fi
-00009380: 645f 7061 7468 203d 2050 6174 6828 7465  d_path = Path(te
-00009390: 6d70 6669 6c65 2e6d 6b64 7465 6d70 2829  mpfile.mkdtemp()
-000093a0: 2920 2f20 6622 7b70 6174 682e 7374 656d  ) / f"{path.stem
-000093b0: 7d2e 6770 6b67 220a 2020 2020 2020 2020  }.gpkg".        
-000093c0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000093d0: 2069 6620 4765 6f66 696c 6554 7970 6528   if GeofileType(
-000093e0: 7061 7468 2920 3d3d 2047 656f 6669 6c65  path) == Geofile
-000093f0: 5479 7065 2e47 504b 473a 0a20 2020 2020  Type.GPKG:.     
-00009400: 2020 2020 2020 2020 2020 2063 6f70 7928             copy(
-00009410: 7061 7468 2c20 746d 705f 6669 645f 7061  path, tmp_fid_pa
-00009420: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
-00009430: 2020 2020 6164 645f 636f 6c75 6d6e 2874      add_column(t
-00009440: 6d70 5f66 6964 5f70 6174 682c 2022 5f5f  mp_fid_path, "__
-00009450: 544d 505f 4745 4f46 494c 454f 5053 5f46  TMP_GEOFILEOPS_F
-00009460: 4944 222c 2022 494e 5445 4745 5222 2c20  ID", "INTEGER", 
-00009470: 2266 6964 2229 0a20 2020 2020 2020 2020  "fid").         
-00009480: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00009490: 2020 2020 2020 2020 2063 6f6e 7665 7274           convert
-000094a0: 2870 6174 682c 2074 6d70 5f66 6964 5f70  (path, tmp_fid_p
-000094b0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-000094c0: 2020 2020 2023 2066 6964 2069 6e20 7368       # fid in sh
-000094d0: 6170 6566 696c 6520 6973 2030 2062 6173  apefile is 0 bas
-000094e0: 6564 2c20 736f 2066 6964 2d31 0a20 2020  ed, so fid-1.   
-000094f0: 2020 2020 2020 2020 2020 2020 2061 6464               add
-00009500: 5f63 6f6c 756d 6e28 746d 705f 6669 645f  _column(tmp_fid_
-00009510: 7061 7468 2c20 225f 5f54 4d50 5f47 454f  path, "__TMP_GEO
-00009520: 4649 4c45 4f50 535f 4649 4422 2c20 2249  FILEOPS_FID", "I
-00009530: 4e54 4547 4552 222c 2022 6669 642d 3122  NTEGER", "fid-1"
-00009540: 290a 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00009550: 6174 6820 3d20 746d 705f 6669 645f 7061  ath = tmp_fid_pa
-00009560: 7468 0a20 2020 2020 2020 2066 696e 616c  th.        final
-00009570: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
-00009580: 6966 2074 6d70 5f66 6964 5f70 6174 682e  if tmp_fid_path.
-00009590: 7061 7265 6e74 2e65 7869 7374 7328 293a  parent.exists():
-000095a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000095b0: 2073 6875 7469 6c2e 726d 7472 6565 2874   shutil.rmtree(t
-000095c0: 6d70 5f66 6964 5f70 6174 682c 2069 676e  mp_fid_path, ign
-000095d0: 6f72 655f 6572 726f 7273 3d54 7275 6529  ore_errors=True)
-000095e0: 0a0a 2020 2020 2320 4368 6563 6b69 6e67  ..    # Checking
-000095f0: 2069 6620 6669 656c 642f 636f 6c75 6d6e   if field/column
-00009600: 206e 616d 6573 2073 686f 756c 6420 6265   names should be
-00009610: 2072 6561 6420 6973 2063 6173 6520 7365   read is case se
-00009620: 6e73 6974 6976 6520 696e 2066 696f 6e61  nsitive in fiona
-00009630: 2c20 736f 0a20 2020 2023 206d 616b 6520  , so.    # make 
-00009640: 7375 7265 2074 6865 2063 6f6c 756d 6e20  sure the column 
-00009650: 6e61 6d65 7320 7370 6563 6966 6965 6420  names specified 
-00009660: 6861 7665 2074 6865 2073 616d 6520 6361  have the same ca
-00009670: 7369 6e67 2e0a 2020 2020 636f 6c75 6d6e  sing..    column
-00009680: 735f 7072 6570 6172 6564 203d 204e 6f6e  s_prepared = Non
-00009690: 650a 2020 2020 6966 2063 6f6c 756d 6e73  e.    if columns
-000096a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000096b0: 2020 2020 2020 6c61 7965 7269 6e66 6f20        layerinfo 
-000096c0: 3d20 6765 745f 6c61 7965 7269 6e66 6f28  = get_layerinfo(
-000096d0: 7061 7468 2c20 6c61 7965 723d 6c61 7965  path, layer=laye
-000096e0: 7229 0a20 2020 2020 2020 2063 6f6c 756d  r).        colum
-000096f0: 6e73 5f75 7070 6572 5f6c 6f6f 6b75 7020  ns_upper_lookup 
-00009700: 3d20 7b63 6f6c 756d 6e2e 7570 7065 7228  = {column.upper(
-00009710: 293a 2063 6f6c 756d 6e20 666f 7220 636f  ): column for co
-00009720: 6c75 6d6e 2069 6e20 636f 6c75 6d6e 737d  lumn in columns}
-00009730: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
-00009740: 5f70 7265 7061 7265 6420 3d20 7b0a 2020  _prepared = {.  
-00009750: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-00009760: 3a20 636f 6c75 6d6e 735f 7570 7065 725f  : columns_upper_
-00009770: 6c6f 6f6b 7570 5b63 6f6c 756d 6e2e 7570  lookup[column.up
-00009780: 7065 7228 295d 0a20 2020 2020 2020 2020  per()].         
-00009790: 2020 2066 6f72 2063 6f6c 756d 6e20 696e     for column in
-000097a0: 206c 6179 6572 696e 666f 2e63 6f6c 756d   layerinfo.colum
-000097b0: 6e73 0a20 2020 2020 2020 2020 2020 2069  ns.            i
-000097c0: 6620 636f 6c75 6d6e 2e75 7070 6572 2829  f column.upper()
-000097d0: 2069 6e20 636f 6c75 6d6e 735f 7570 7065   in columns_uppe
-000097e0: 725f 6c6f 6f6b 7570 0a20 2020 2020 2020  r_lookup.       
-000097f0: 207d 0a0a 2020 2020 2320 5265 6164 2e2e   }..    # Read..
-00009800: 2e0a 2020 2020 636f 6c75 6d6e 735f 6c69  ..    columns_li
-00009810: 7374 203d 204e 6f6e 6520 6966 2063 6f6c  st = None if col
-00009820: 756d 6e73 5f70 7265 7061 7265 6420 6973  umns_prepared is
-00009830: 204e 6f6e 6520 656c 7365 206c 6973 7428   None else list(
-00009840: 636f 6c75 6d6e 735f 7072 6570 6172 6564  columns_prepared
-00009850: 290a 2020 2020 7265 7375 6c74 5f67 6466  ).    result_gdf
-00009860: 203d 2067 7064 2e72 6561 645f 6669 6c65   = gpd.read_file
-00009870: 280a 2020 2020 2020 2020 7374 7228 7061  (.        str(pa
-00009880: 7468 292c 0a20 2020 2020 2020 206c 6179  th),.        lay
-00009890: 6572 3d6c 6179 6572 2c0a 2020 2020 2020  er=layer,.      
-000098a0: 2020 6262 6f78 3d62 626f 782c 0a20 2020    bbox=bbox,.   
-000098b0: 2020 2020 2072 6f77 733d 726f 7773 2c0a       rows=rows,.
-000098c0: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-000098d0: 6669 656c 6473 3d63 6f6c 756d 6e73 5f6c  fields=columns_l
-000098e0: 6973 742c 0a20 2020 2020 2020 2073 716c  ist,.        sql
-000098f0: 3d73 716c 5f73 746d 742c 0a20 2020 2020  =sql_stmt,.     
-00009900: 2020 2073 716c 5f64 6961 6c65 6374 3d73     sql_dialect=s
-00009910: 716c 5f64 6961 6c65 6374 2c0a 2020 2020  ql_dialect,.    
-00009920: 2020 2020 6967 6e6f 7265 5f67 656f 6d65      ignore_geome
-00009930: 7472 793d 6967 6e6f 7265 5f67 656f 6d65  try=ignore_geome
-00009940: 7472 792c 0a20 2020 2029 0a0a 2020 2020  try,.    )..    
-00009950: 2320 5365 7420 7468 6520 696e 6465 7820  # Set the index 
-00009960: 746f 2074 6865 2062 6163 6b65 642d 7570  to the backed-up
-00009970: 2066 6964 0a20 2020 2069 6620 6669 645f   fid.    if fid_
-00009980: 6173 5f69 6e64 6578 3a0a 2020 2020 2020  as_index:.      
-00009990: 2020 7265 7375 6c74 5f67 6466 203d 2072    result_gdf = r
-000099a0: 6573 756c 745f 6764 662e 7365 745f 696e  esult_gdf.set_in
-000099b0: 6465 7828 225f 5f54 4d50 5f47 454f 4649  dex("__TMP_GEOFI
-000099c0: 4c45 4f50 535f 4649 4422 290a 0a20 2020  LEOPS_FID")..   
-000099d0: 2023 2052 656f 7264 6572 2063 6f6c 756d   # Reorder colum
-000099e0: 6e73 202b 2063 6861 6e67 6520 6361 7369  ns + change casi
-000099f0: 6e67 2073 6f20 7468 6579 2061 7265 2074  ng so they are t
-00009a00: 6865 2073 616d 6520 6173 2063 6f6c 756d  he same as colum
-00009a10: 6e73 2070 6172 616d 6574 6572 0a20 2020  ns parameter.   
-00009a20: 2069 6620 636f 6c75 6d6e 735f 7072 6570   if columns_prep
-00009a30: 6172 6564 2069 7320 6e6f 7420 4e6f 6e65  ared is not None
-00009a40: 2061 6e64 206c 656e 2863 6f6c 756d 6e73   and len(columns
-00009a50: 5f70 7265 7061 7265 6429 203e 2030 3a0a  _prepared) > 0:.
-00009a60: 2020 2020 2020 2020 7265 7375 6c74 5f67          result_g
-00009a70: 6466 203d 2072 6573 756c 745f 6764 665b  df = result_gdf[
-00009a80: 6c69 7374 2863 6f6c 756d 6e73 5f70 7265  list(columns_pre
-00009a90: 7061 7265 6429 202b 205b 2267 656f 6d65  pared) + ["geome
-00009aa0: 7472 7922 5d5d 0a20 2020 2020 2020 2072  try"]].        r
-00009ab0: 6573 756c 745f 6764 6620 3d20 7265 7375  esult_gdf = resu
-00009ac0: 6c74 5f67 6466 2e72 656e 616d 6528 636f  lt_gdf.rename(co
-00009ad0: 6c75 6d6e 733d 636f 6c75 6d6e 735f 7072  lumns=columns_pr
-00009ae0: 6570 6172 6564 2920 2023 2074 7970 653a  epared)  # type:
-00009af0: 2069 676e 6f72 650a 0a20 2020 2023 2053   ignore..    # S
-00009b00: 7461 7274 696e 6720 6672 6f6d 2066 696f  tarting from fio
-00009b10: 6e61 2031 2e39 2c20 7374 7269 6e67 2063  na 1.9, string c
-00009b20: 6f6c 756d 6e73 2077 6974 6820 616c 6c20  olumns with all 
-00009b30: 4e6f 6e65 2076 616c 7565 7320 6172 6520  None values are 
-00009b40: 7265 6164 2061 7320 6265 696e 670a 2020  read as being.  
-00009b50: 2020 2320 666c 6f61 7420 636f 6c75 6d6e    # float column
-00009b60: 732e 2043 6f6e 7665 7274 2074 6865 6d20  s. Convert them 
-00009b70: 746f 206f 626a 6563 7420 7479 7065 2e0a  to object type..
-00009b80: 2020 2020 666c 6f61 745f 636f 6c73 203d      float_cols =
-00009b90: 206c 6973 7428 7265 7375 6c74 5f67 6466   list(result_gdf
-00009ba0: 2e73 656c 6563 745f 6474 7970 6573 285b  .select_dtypes([
-00009bb0: 2266 6c6f 6174 3634 225d 292e 636f 6c75  "float64"]).colu
-00009bc0: 6d6e 7329 0a20 2020 2069 6620 6c65 6e28  mns).    if len(
-00009bd0: 666c 6f61 745f 636f 6c73 2920 3e20 303a  float_cols) > 0:
-00009be0: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
-00009bf0: 2066 6f72 2061 6c6c 2066 6c6f 6174 2063   for all float c
-00009c00: 6f6c 756d 6e73 2066 6f75 6e64 2069 6620  olumns found if 
-00009c10: 7468 6579 2073 686f 756c 6420 6265 206f  they should be o
-00009c20: 626a 6563 7420 636f 6c75 6d6e 7320 696e  bject columns in
-00009c30: 7374 6561 640a 2020 2020 2020 2020 7769  stead.        wi
-00009c40: 7468 2066 696f 6e61 2e6f 7065 6e28 7061  th fiona.open(pa
-00009c50: 7468 2c20 6c61 7965 723d 6c61 7965 7229  th, layer=layer)
-00009c60: 2061 7320 636f 6c6c 6563 7469 6f6e 3a0a   as collection:.
-00009c70: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00009c80: 7274 2063 6f6c 6c65 6374 696f 6e2e 7363  rt collection.sc
-00009c90: 6865 6d61 2069 7320 6e6f 7420 4e6f 6e65  hema is not None
-00009ca0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00009cb0: 7065 7274 6965 7320 3d20 636f 6c6c 6563  perties = collec
-00009cc0: 7469 6f6e 2e73 6368 656d 615b 2270 726f  tion.schema["pro
-00009cd0: 7065 7274 6965 7322 5d0a 2020 2020 2020  perties"].      
-00009ce0: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
-00009cf0: 2066 6c6f 6174 5f63 6f6c 733a 0a20 2020   float_cols:.   
-00009d00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009d10: 636f 6c20 696e 2070 726f 7065 7274 6965  col in propertie
-00009d20: 7320 616e 6420 7072 6f70 6572 7469 6573  s and properties
-00009d30: 5b63 6f6c 5d2e 7374 6172 7473 7769 7468  [col].startswith
-00009d40: 2822 7374 7222 293a 0a20 2020 2020 2020  ("str"):.       
-00009d50: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00009d60: 756c 745f 6764 665b 636f 6c5d 203d 2028  ult_gdf[col] = (
-00009d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009d80: 2020 2020 2020 2020 2072 6573 756c 745f           result_
-00009d90: 6764 665b 636f 6c5d 2020 2320 7479 7065  gdf[col]  # type
-00009da0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 202e 6173 7479 7065 286f 626a 6563 7429   .astype(object)
-00009dd0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00009de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009df0: 2020 2020 2020 2020 202e 7265 706c 6163           .replac
-00009e00: 6528 6e70 2e6e 616e 2c20 4e6f 6e65 290a  e(np.nan, None).
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 2020 2020 290a 0a20 2020 2023 2061 7373      )..    # ass
-00009e30: 6572 7420 746f 2065 7661 6465 2070 794c  ert to evade pyL
-00009e40: 616e 6365 2077 6172 6e69 6e67 0a20 2020  ance warning.   
-00009e50: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00009e60: 6365 2872 6573 756c 745f 6764 662c 2070  ce(result_gdf, p
-00009e70: 642e 4461 7461 4672 616d 6529 206f 7220  d.DataFrame) or 
-00009e80: 6973 696e 7374 616e 6365 280a 2020 2020  isinstance(.    
-00009e90: 2020 2020 7265 7375 6c74 5f67 6466 2c20      result_gdf, 
-00009ea0: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
-00009eb0: 0a20 2020 2029 0a20 2020 2072 6574 7572  .    ).    retur
-00009ec0: 6e20 7265 7375 6c74 5f67 6466 0a0a 0a64  n result_gdf...d
-00009ed0: 6566 205f 7265 6164 5f66 696c 655f 6261  ef _read_file_ba
-00009ee0: 7365 5f70 796f 6772 696f 280a 2020 2020  se_pyogrio(.    
-00009ef0: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
-00009f00: 2022 6f73 2e50 6174 684c 696b 655b 416e   "os.PathLike[An
-00009f10: 795d 225d 2c0a 2020 2020 6c61 7965 723a  y]"],.    layer:
-00009f20: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00009f30: 204e 6f6e 652c 0a20 2020 2063 6f6c 756d   None,.    colum
-00009f40: 6e73 3a20 4f70 7469 6f6e 616c 5b49 7465  ns: Optional[Ite
-00009f50: 7261 626c 655b 7374 725d 5d20 3d20 4e6f  rable[str]] = No
-00009f60: 6e65 2c0a 2020 2020 6262 6f78 3d4e 6f6e  ne,.    bbox=Non
-00009f70: 652c 0a20 2020 2072 6f77 733d 4e6f 6e65  e,.    rows=None
-00009f80: 2c0a 2020 2020 7371 6c5f 7374 6d74 3a20  ,.    sql_stmt: 
-00009f90: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00009fa0: 4e6f 6e65 2c0a 2020 2020 7371 6c5f 6469  None,.    sql_di
-00009fb0: 616c 6563 743a 204f 7074 696f 6e61 6c5b  alect: Optional[
-00009fc0: 4c69 7465 7261 6c5b 2253 514c 4954 4522  Literal["SQLITE"
-00009fd0: 2c20 224f 4752 5351 4c22 5d5d 203d 204e  , "OGRSQL"]] = N
-00009fe0: 6f6e 652c 0a20 2020 2069 676e 6f72 655f  one,.    ignore_
-00009ff0: 6765 6f6d 6574 7279 3a20 626f 6f6c 203d  geometry: bool =
-0000a000: 2046 616c 7365 2c0a 2020 2020 6669 645f   False,.    fid_
-0000a010: 6173 5f69 6e64 6578 3a20 626f 6f6c 203d  as_index: bool =
-0000a020: 2046 616c 7365 2c0a 2920 2d3e 2055 6e69   False,.) -> Uni
-0000a030: 6f6e 5b70 642e 4461 7461 4672 616d 652c  on[pd.DataFrame,
-0000a040: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-0000a050: 655d 3a0a 2020 2020 2222 220a 2020 2020  e]:.    """.    
-0000a060: 5265 6164 7320 6120 6669 6c65 2074 6f20  Reads a file to 
-0000a070: 6120 7061 6e64 6173 2044 6174 6166 7261  a pandas Datafra
-0000a080: 6d65 2075 7369 6e67 2070 796f 6772 696f  me using pyogrio
-0000a090: 2e0a 2020 2020 2222 220a 2020 2020 2320  ..    """.    # 
-0000a0a0: 496e 6974 0a20 2020 2070 6174 6820 3d20  Init.    path = 
-0000a0b0: 5061 7468 2870 6174 6829 0a20 2020 2069  Path(path).    i
-0000a0c0: 6620 7061 7468 2e65 7869 7374 7328 2920  f path.exists() 
-0000a0d0: 6973 2046 616c 7365 3a0a 2020 2020 2020  is False:.      
-0000a0e0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000a0f0: 6f72 2866 2266 696c 6520 646f 6573 6e27  or(f"file doesn'
-0000a100: 7420 6578 6973 743a 207b 7061 7468 7d22  t exist: {path}"
-0000a110: 290a 0a20 2020 2023 2043 6f6e 7665 7274  )..    # Convert
-0000a120: 2073 6c69 6365 206f 626a 6563 7420 746f   slice object to
-0000a130: 2070 796f 6772 696f 2070 6172 616d 6574   pyogrio paramet
-0000a140: 6572 730a 2020 2020 6966 2072 6f77 7320  ers.    if rows 
-0000a150: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000a160: 2020 2020 2073 6b69 705f 6665 6174 7572       skip_featur
-0000a170: 6573 203d 2072 6f77 732e 7374 6172 740a  es = rows.start.
-0000a180: 2020 2020 2020 2020 6d61 785f 6665 6174          max_feat
-0000a190: 7572 6573 203d 2072 6f77 732e 7374 6f70  ures = rows.stop
-0000a1a0: 202d 2072 6f77 732e 7374 6172 740a 2020   - rows.start.  
-0000a1b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a1c0: 736b 6970 5f66 6561 7475 7265 7320 3d20  skip_features = 
-0000a1d0: 300a 2020 2020 2020 2020 6d61 785f 6665  0.        max_fe
-0000a1e0: 6174 7572 6573 203d 204e 6f6e 650a 0a20  atures = None.. 
-0000a1f0: 2020 2023 2049 6620 6e6f 2073 716c 5f73     # If no sql_s
-0000a200: 746d 7420 7370 6563 6966 6965 640a 2020  tmt specified.  
-0000a210: 2020 636f 6c75 6d6e 735f 7072 6570 6172    columns_prepar
-0000a220: 6564 203d 204e 6f6e 650a 2020 2020 6966  ed = None.    if
-0000a230: 2073 716c 5f73 746d 7420 6973 204e 6f6e   sql_stmt is Non
-0000a240: 653a 0a20 2020 2020 2020 2023 2049 6620  e:.        # If 
-0000a250: 6e6f 206c 6179 6572 2073 7065 6369 6669  no layer specifi
-0000a260: 6564 2c20 7468 6572 6520 7368 6f75 6c64  ed, there should
-0000a270: 2062 6520 6f6e 6c79 206f 6e65 206c 6179   be only one lay
-0000a280: 6572 2069 6e20 7468 6520 6669 6c65 2e0a  er in the file..
-0000a290: 2020 2020 2020 2020 6966 206c 6179 6572          if layer
-0000a2a0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000a2b0: 2020 2020 2020 6c61 7965 7220 3d20 6765        layer = ge
-0000a2c0: 745f 6f6e 6c79 5f6c 6179 6572 2870 6174  t_only_layer(pat
-0000a2d0: 6829 0a0a 2020 2020 2020 2020 2320 4368  h)..        # Ch
-0000a2e0: 6563 6b69 6e67 2069 6620 636f 6c75 6d6e  ecking if column
-0000a2f0: 206e 616d 6573 2073 686f 756c 6420 6265   names should be
-0000a300: 2072 6561 6420 6973 2063 6173 6520 7365   read is case se
-0000a310: 6e73 6974 6976 6520 696e 2070 796f 6772  nsitive in pyogr
-0000a320: 696f 2c20 736f 0a20 2020 2020 2020 2023  io, so.        #
-0000a330: 206d 616b 6520 7375 7265 2074 6865 2063   make sure the c
-0000a340: 6f6c 756d 6e20 6e61 6d65 7320 7370 6563  olumn names spec
-0000a350: 6966 6965 6420 6861 7665 2074 6865 2073  ified have the s
-0000a360: 616d 6520 6361 7369 6e67 2e0a 2020 2020  ame casing..    
-0000a370: 2020 2020 6966 2063 6f6c 756d 6e73 2069      if columns i
-0000a380: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000a390: 2020 2020 2020 2020 6c61 7965 7269 6e66          layerinf
-0000a3a0: 6f20 3d20 6765 745f 6c61 7965 7269 6e66  o = get_layerinf
-0000a3b0: 6f28 7061 7468 2c20 6c61 7965 723d 6c61  o(path, layer=la
-0000a3c0: 7965 7229 0a20 2020 2020 2020 2020 2020  yer).           
-0000a3d0: 2063 6f6c 756d 6e73 5f75 7070 6572 5f6c   columns_upper_l
-0000a3e0: 6f6f 6b75 7020 3d20 7b63 6f6c 756d 6e2e  ookup = {column.
-0000a3f0: 7570 7065 7228 293a 2063 6f6c 756d 6e20  upper(): column 
-0000a400: 666f 7220 636f 6c75 6d6e 2069 6e20 636f  for column in co
-0000a410: 6c75 6d6e 737d 0a20 2020 2020 2020 2020  lumns}.         
-0000a420: 2020 2063 6f6c 756d 6e73 5f70 7265 7061     columns_prepa
-0000a430: 7265 6420 3d20 7b0a 2020 2020 2020 2020  red = {.        
-0000a440: 2020 2020 2020 2020 636f 6c75 6d6e 3a20          column: 
-0000a450: 636f 6c75 6d6e 735f 7570 7065 725f 6c6f  columns_upper_lo
-0000a460: 6f6b 7570 5b63 6f6c 756d 6e2e 7570 7065  okup[column.uppe
-0000a470: 7228 295d 0a20 2020 2020 2020 2020 2020  r()].           
-0000a480: 2020 2020 2066 6f72 2063 6f6c 756d 6e20       for column 
-0000a490: 696e 206c 6179 6572 696e 666f 2e63 6f6c  in layerinfo.col
-0000a4a0: 756d 6e73 0a20 2020 2020 2020 2020 2020  umns.           
-0000a4b0: 2020 2020 2069 6620 636f 6c75 6d6e 2e75       if column.u
-0000a4c0: 7070 6572 2829 2069 6e20 636f 6c75 6d6e  pper() in column
-0000a4d0: 735f 7570 7065 725f 6c6f 6f6b 7570 0a20  s_upper_lookup. 
-0000a4e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0000a4f0: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
-0000a500: 2046 696c 6c20 6f75 7420 706c 6163 6568   Fill out placeh
-0000a510: 6f6c 6465 7273 2c20 6b65 6570 2063 6f6c  olders, keep col
-0000a520: 756d 6e73 5f70 7265 7061 7265 6420 4e6f  umns_prepared No
-0000a530: 6e65 2062 6563 6175 7365 2063 6f6c 756d  ne because colum
-0000a540: 6e20 6669 6c74 6572 696e 670a 2020 2020  n filtering.    
-0000a550: 2020 2020 2320 7368 6f75 6c64 2068 6170      # should hap
-0000a560: 7065 6e20 696e 2073 716c 5f73 746d 742e  pen in sql_stmt.
-0000a570: 0a20 2020 2020 2020 2073 716c 5f73 746d  .        sql_stm
-0000a580: 7420 3d20 5f66 696c 6c5f 6f75 745f 7371  t = _fill_out_sq
-0000a590: 6c5f 706c 6163 6568 6f6c 6465 7273 280a  l_placeholders(.
-0000a5a0: 2020 2020 2020 2020 2020 2020 7061 7468              path
-0000a5b0: 3d70 6174 682c 206c 6179 6572 3d6c 6179  =path, layer=lay
-0000a5c0: 6572 2c20 7371 6c5f 7374 6d74 3d73 716c  er, sql_stmt=sql
-0000a5d0: 5f73 746d 742c 2063 6f6c 756d 6e73 3d63  _stmt, columns=c
-0000a5e0: 6f6c 756d 6e73 0a20 2020 2020 2020 2029  olumns.        )
-0000a5f0: 0a0a 2020 2020 2320 5265 6164 210a 2020  ..    # Read!.  
-0000a600: 2020 636f 6c75 6d6e 735f 6c69 7374 203d    columns_list =
-0000a610: 204e 6f6e 6520 6966 2063 6f6c 756d 6e73   None if columns
-0000a620: 5f70 7265 7061 7265 6420 6973 204e 6f6e  _prepared is Non
-0000a630: 6520 656c 7365 206c 6973 7428 636f 6c75  e else list(colu
-0000a640: 6d6e 735f 7072 6570 6172 6564 290a 2020  mns_prepared).  
-0000a650: 2020 7265 7375 6c74 5f67 6466 203d 2070    result_gdf = p
-0000a660: 796f 6772 696f 2e72 6561 645f 6461 7461  yogrio.read_data
-0000a670: 6672 616d 6528 0a20 2020 2020 2020 2070  frame(.        p
-0000a680: 6174 682c 0a20 2020 2020 2020 206c 6179  ath,.        lay
-0000a690: 6572 3d6c 6179 6572 2c0a 2020 2020 2020  er=layer,.      
-0000a6a0: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
-0000a6b0: 735f 6c69 7374 2c0a 2020 2020 2020 2020  s_list,.        
-0000a6c0: 6262 6f78 3d62 626f 782c 0a20 2020 2020  bbox=bbox,.     
-0000a6d0: 2020 2073 6b69 705f 6665 6174 7572 6573     skip_features
-0000a6e0: 3d73 6b69 705f 6665 6174 7572 6573 2c0a  =skip_features,.
-0000a6f0: 2020 2020 2020 2020 6d61 785f 6665 6174          max_feat
-0000a700: 7572 6573 3d6d 6178 5f66 6561 7475 7265  ures=max_feature
-0000a710: 732c 0a20 2020 2020 2020 2073 716c 3d73  s,.        sql=s
-0000a720: 716c 5f73 746d 742c 0a20 2020 2020 2020  ql_stmt,.       
-0000a730: 2073 716c 5f64 6961 6c65 6374 3d73 716c   sql_dialect=sql
-0000a740: 5f64 6961 6c65 6374 2c0a 2020 2020 2020  _dialect,.      
-0000a750: 2020 7265 6164 5f67 656f 6d65 7472 793d    read_geometry=
-0000a760: 6e6f 7420 6967 6e6f 7265 5f67 656f 6d65  not ignore_geome
-0000a770: 7472 792c 0a20 2020 2020 2020 2066 6964  try,.        fid
-0000a780: 5f61 735f 696e 6465 783d 6669 645f 6173  _as_index=fid_as
-0000a790: 5f69 6e64 6578 2c0a 2020 2020 290a 0a20  _index,.    ).. 
-0000a7a0: 2020 2023 2052 656f 7264 6572 2063 6f6c     # Reorder col
-0000a7b0: 756d 6e73 202b 2063 6861 6e67 6520 6361  umns + change ca
-0000a7c0: 7369 6e67 2073 6f20 7468 6579 2061 7265  sing so they are
-0000a7d0: 2074 6865 2073 616d 6520 6173 2063 6f6c   the same as col
-0000a7e0: 756d 6e73 2070 6172 616d 6574 6572 0a20  umns parameter. 
-0000a7f0: 2020 2069 6620 636f 6c75 6d6e 735f 7072     if columns_pr
-0000a800: 6570 6172 6564 2069 7320 6e6f 7420 4e6f  epared is not No
-0000a810: 6e65 2061 6e64 206c 656e 2863 6f6c 756d  ne and len(colum
-0000a820: 6e73 5f70 7265 7061 7265 6429 203e 2030  ns_prepared) > 0
-0000a830: 3a0a 2020 2020 2020 2020 7265 7375 6c74  :.        result
-0000a840: 5f67 6466 203d 2072 6573 756c 745f 6764  _gdf = result_gd
-0000a850: 665b 6c69 7374 2863 6f6c 756d 6e73 5f70  f[list(columns_p
-0000a860: 7265 7061 7265 6429 202b 205b 2267 656f  repared) + ["geo
-0000a870: 6d65 7472 7922 5d5d 0a20 2020 2020 2020  metry"]].       
-0000a880: 2072 6573 756c 745f 6764 6620 3d20 7265   result_gdf = re
-0000a890: 7375 6c74 5f67 6466 2e72 656e 616d 6528  sult_gdf.rename(
-0000a8a0: 636f 6c75 6d6e 733d 636f 6c75 6d6e 735f  columns=columns_
-0000a8b0: 7072 6570 6172 6564 2920 2023 2074 7970  prepared)  # typ
-0000a8c0: 653a 2069 676e 6f72 650a 0a20 2020 2023  e: ignore..    #
-0000a8d0: 2061 7373 6572 7420 746f 2065 7661 6465   assert to evade
-0000a8e0: 2070 794c 616e 6365 2077 6172 6e69 6e67   pyLance warning
-0000a8f0: 0a20 2020 2061 7373 6572 7420 6973 696e  .    assert isin
-0000a900: 7374 616e 6365 2872 6573 756c 745f 6764  stance(result_gd
-0000a910: 662c 2070 642e 4461 7461 4672 616d 6529  f, pd.DataFrame)
-0000a920: 206f 7220 6973 696e 7374 616e 6365 280a   or isinstance(.
-0000a930: 2020 2020 2020 2020 7265 7375 6c74 5f67          result_g
-0000a940: 6466 2c20 6770 642e 4765 6f44 6174 6146  df, gpd.GeoDataF
-0000a950: 7261 6d65 0a20 2020 2029 0a20 2020 2072  rame.    ).    r
-0000a960: 6574 7572 6e20 7265 7375 6c74 5f67 6466  eturn result_gdf
-0000a970: 0a0a 0a64 6566 205f 6669 6c6c 5f6f 7574  ...def _fill_out
-0000a980: 5f73 716c 5f70 6c61 6365 686f 6c64 6572  _sql_placeholder
-0000a990: 7328 0a20 2020 2070 6174 683a 2050 6174  s(.    path: Pat
-0000a9a0: 682c 206c 6179 6572 3a20 4f70 7469 6f6e  h, layer: Option
-0000a9b0: 616c 5b73 7472 5d2c 2073 716c 5f73 746d  al[str], sql_stm
-0000a9c0: 743a 2073 7472 2c20 636f 6c75 6d6e 733a  t: str, columns:
-0000a9d0: 204f 7074 696f 6e61 6c5b 4974 6572 6162   Optional[Iterab
-0000a9e0: 6c65 5b73 7472 5d5d 0a29 202d 3e20 7374  le[str]].) -> st
-0000a9f0: 723a 0a20 2020 2023 2046 696c 6c20 6f75  r:.    # Fill ou
-0000aa00: 7420 706c 6163 6568 6f6c 6465 7273 2069  t placeholders i
-0000aa10: 6e20 7468 6520 7371 6c5f 7374 6d74 2069  n the sql_stmt i
-0000aa20: 6620 6e65 6564 6564 3a0a 2020 2020 706c  f needed:.    pl
-0000aa30: 6163 6568 6f6c 6465 7273 203d 205b 0a20  aceholders = [. 
-0000aa40: 2020 2020 2020 206e 616d 6520 666f 7220         name for 
-0000aa50: 5f2c 206e 616d 652c 205f 2c20 5f20 696e  _, name, _, _ in
-0000aa60: 2073 7472 696e 672e 466f 726d 6174 7465   string.Formatte
-0000aa70: 7228 292e 7061 7273 6528 7371 6c5f 7374  r().parse(sql_st
-0000aa80: 6d74 2920 6966 206e 616d 650a 2020 2020  mt) if name.    
-0000aa90: 5d0a 2020 2020 6c61 7965 725f 746d 7020  ].    layer_tmp 
-0000aaa0: 3d20 6c61 7965 720a 2020 2020 6c61 7965  = layer.    laye
-0000aab0: 7269 6e66 6f20 3d20 4e6f 6e65 0a20 2020  rinfo = None.   
-0000aac0: 2066 6f72 6d61 745f 6b77 6172 6773 203d   format_kwargs =
-0000aad0: 207b 7d0a 2020 2020 666f 7220 706c 6163   {}.    for plac
-0000aae0: 6568 6f6c 6465 7220 696e 2070 6c61 6365  eholder in place
-0000aaf0: 686f 6c64 6572 733a 0a20 2020 2020 2020  holders:.       
-0000ab00: 2069 6620 6c61 7965 725f 746d 7020 6973   if layer_tmp is
-0000ab10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000ab20: 2020 206c 6179 6572 5f74 6d70 203d 2067     layer_tmp = g
-0000ab30: 6574 5f6f 6e6c 795f 6c61 7965 7228 7061  et_only_layer(pa
-0000ab40: 7468 290a 2020 2020 2020 2020 6966 2070  th).        if p
-0000ab50: 6c61 6365 686f 6c64 6572 203d 3d20 2269  laceholder == "i
-0000ab60: 6e70 7574 5f6c 6179 6572 223a 0a20 2020  nput_layer":.   
-0000ab70: 2020 2020 2020 2020 2066 6f72 6d61 745f           format_
-0000ab80: 6b77 6172 6773 5b70 6c61 6365 686f 6c64  kwargs[placehold
-0000ab90: 6572 5d20 3d20 6c61 7965 725f 746d 700a  er] = layer_tmp.
-0000aba0: 2020 2020 2020 2020 656c 6966 2070 6c61          elif pla
-0000abb0: 6365 686f 6c64 6572 203d 3d20 2267 656f  ceholder == "geo
-0000abc0: 6d65 7472 7963 6f6c 756d 6e22 3a0a 2020  metrycolumn":.  
-0000abd0: 2020 2020 2020 2020 2020 6966 206c 6179            if lay
-0000abe0: 6572 696e 666f 2069 7320 4e6f 6e65 3a0a  erinfo is None:.
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 6c61 7965 7269 6e66 6f20 3d20 6765 745f  layerinfo = get_
-0000ac10: 6c61 7965 7269 6e66 6f28 7061 7468 2c20  layerinfo(path, 
-0000ac20: 6c61 7965 725f 746d 7029 0a20 2020 2020  layer_tmp).     
-0000ac30: 2020 2020 2020 2066 6f72 6d61 745f 6b77         format_kw
-0000ac40: 6172 6773 5b70 6c61 6365 686f 6c64 6572  args[placeholder
-0000ac50: 5d20 3d20 6c61 7965 7269 6e66 6f2e 6765  ] = layerinfo.ge
-0000ac60: 6f6d 6574 7279 636f 6c75 6d6e 0a20 2020  ometrycolumn.   
-0000ac70: 2020 2020 2065 6c69 6620 706c 6163 6568       elif placeh
-0000ac80: 6f6c 6465 7220 3d3d 2022 636f 6c75 6d6e  older == "column
-0000ac90: 735f 746f 5f73 656c 6563 745f 7374 7222  s_to_select_str"
-0000aca0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000acb0: 206c 6179 6572 696e 666f 2069 7320 4e6f   layerinfo is No
-0000acc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000acd0: 2020 2020 6c61 7965 7269 6e66 6f20 3d20      layerinfo = 
-0000ace0: 6765 745f 6c61 7965 7269 6e66 6f28 7061  get_layerinfo(pa
-0000acf0: 7468 2c20 6c61 7965 725f 746d 7029 0a20  th, layer_tmp). 
-0000ad00: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000ad10: 6e73 5f61 736b 6564 203d 204e 6f6e 6520  ns_asked = None 
-0000ad20: 6966 2063 6f6c 756d 6e73 2069 7320 4e6f  if columns is No
-0000ad30: 6e65 2065 6c73 6520 6c69 7374 2863 6f6c  ne else list(col
-0000ad40: 756d 6e73 290a 2020 2020 2020 2020 2020  umns).          
-0000ad50: 2020 666f 726d 6174 7465 7220 3d20 5f6f    formatter = _o
-0000ad60: 6772 5f73 716c 5f75 7469 6c2e 436f 6c75  gr_sql_util.Colu
-0000ad70: 6d6e 466f 726d 6174 7465 7228 0a20 2020  mnFormatter(.   
-0000ad80: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0000ad90: 756d 6e73 5f61 736b 6564 3d63 6f6c 756d  umns_asked=colum
-0000ada0: 6e73 5f61 736b 6564 2c0a 2020 2020 2020  ns_asked,.      
-0000adb0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-0000adc0: 735f 696e 5f6c 6179 6572 3d6c 6179 6572  s_in_layer=layer
-0000add0: 696e 666f 2e63 6f6c 756d 6e73 2c0a 2020  info.columns,.  
-0000ade0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000adf0: 645f 636f 6c75 6d6e 3d6c 6179 6572 696e  d_column=layerin
-0000ae00: 666f 2e66 6964 5f63 6f6c 756d 6e2c 0a20  fo.fid_column,. 
-0000ae10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000ae20: 2020 2020 2020 2020 2066 6f72 6d61 745f           format_
-0000ae30: 6b77 6172 6773 5b70 6c61 6365 686f 6c64  kwargs[placehold
-0000ae40: 6572 5d20 3d20 666f 726d 6174 7465 722e  er] = formatter.
-0000ae50: 7072 6566 6978 6564 5f61 6c69 6173 6564  prefixed_aliased
-0000ae60: 2829 0a0a 2020 2020 2020 2020 656c 7365  ()..        else
-0000ae70: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000ae80: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aea0: 6622 756e 6b6e 6f77 6e20 706c 6163 6568  f"unknown placeh
-0000aeb0: 6f6c 6465 7220 7b70 6c61 6365 686f 6c64  older {placehold
-0000aec0: 6572 7d20 696e 2073 716c 5f73 746d 743a  er} in sql_stmt:
-0000aed0: 207b 7371 6c5f 7374 6d74 7d22 0a20 2020   {sql_stmt}".   
-0000aee0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000aef0: 6966 206c 656e 2866 6f72 6d61 745f 6b77  if len(format_kw
-0000af00: 6172 6773 2920 3e20 303a 0a20 2020 2020  args) > 0:.     
-0000af10: 2020 2073 716c 5f73 746d 7420 3d20 7371     sql_stmt = sq
-0000af20: 6c5f 7374 6d74 2e66 6f72 6d61 7428 2a2a  l_stmt.format(**
-0000af30: 666f 726d 6174 5f6b 7761 7267 7329 0a20  format_kwargs). 
-0000af40: 2020 2072 6574 7572 6e20 7371 6c5f 7374     return sql_st
-0000af50: 6d74 0a0a 0a64 6566 2072 6561 645f 6669  mt...def read_fi
-0000af60: 6c65 5f73 716c 280a 2020 2020 7061 7468  le_sql(.    path
-0000af70: 3a20 556e 696f 6e5b 7374 722c 2022 6f73  : Union[str, "os
-0000af80: 2e50 6174 684c 696b 655b 416e 795d 225d  .PathLike[Any]"]
-0000af90: 2c0a 2020 2020 7371 6c5f 7374 6d74 3a20  ,.    sql_stmt: 
-0000afa0: 7374 722c 0a20 2020 2073 716c 5f64 6961  str,.    sql_dia
-0000afb0: 6c65 6374 3a20 4f70 7469 6f6e 616c 5b4c  lect: Optional[L
-0000afc0: 6974 6572 616c 5b22 5351 4c49 5445 222c  iteral["SQLITE",
-0000afd0: 2022 4f47 5253 514c 225d 5d20 3d20 2253   "OGRSQL"]] = "S
-0000afe0: 514c 4954 4522 2c0a 2020 2020 6c61 7965  QLITE",.    laye
-0000aff0: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
-0000b000: 203d 204e 6f6e 652c 0a20 2020 2069 676e   = None,.    ign
-0000b010: 6f72 655f 6765 6f6d 6574 7279 3a20 626f  ore_geometry: bo
-0000b020: 6f6c 203d 2046 616c 7365 2c0a 2920 2d3e  ol = False,.) ->
-0000b030: 2055 6e69 6f6e 5b70 642e 4461 7461 4672   Union[pd.DataFr
-0000b040: 616d 652c 2067 7064 2e47 656f 4461 7461  ame, gpd.GeoData
-0000b050: 4672 616d 655d 3a0a 2020 2020 2222 220a  Frame]:.    """.
-0000b060: 2020 2020 4445 5052 4543 4154 4544 3a20      DEPRECATED: 
-0000b070: 5265 6164 7320 6120 6669 6c65 2075 7369  Reads a file usi
-0000b080: 6e67 2061 6e20 7371 6c20 7374 6174 656d  ng an sql statem
-0000b090: 656e 742e 0a0a 2020 2020 4172 6773 3a0a  ent...    Args:.
-0000b0a0: 2020 2020 2020 2020 7061 7468 2028 6669          path (fi
-0000b0b0: 6c65 2070 6174 6829 3a20 7061 7468 2074  le path): path t
-0000b0c0: 6f20 7468 6520 6669 6c65 2074 6f20 7265  o the file to re
-0000b0d0: 6164 2066 726f 6d0a 2020 2020 2020 2020  ad from.        
-0000b0e0: 7371 6c5f 7374 6d74 2028 7374 7229 3a20  sql_stmt (str): 
-0000b0f0: 7371 6c20 7374 6174 656d 656e 7420 746f  sql statement to
-0000b100: 2075 7365 0a20 2020 2020 2020 2073 716c   use.        sql
-0000b110: 5f64 6961 6c65 6374 2028 7374 722c 206f  _dialect (str, o
-0000b120: 7074 696f 6e61 6c29 3a20 5371 6c20 6469  ptional): Sql di
-0000b130: 616c 6563 7420 7573 6564 2e20 4465 6661  alect used. Defa
-0000b140: 756c 7473 2074 6f20 2753 514c 4954 4527  ults to 'SQLITE'
-0000b150: 2e0a 2020 2020 2020 2020 6c61 7965 7220  ..        layer 
-0000b160: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-0000b170: 2054 6865 206c 6179 6572 2074 6f20 7265   The layer to re
-0000b180: 6164 2e20 4966 206e 6f20 6c61 7965 7220  ad. If no layer 
-0000b190: 6973 2073 7065 6369 6669 6564 2c0a 2020  is specified,.  
-0000b1a0: 2020 2020 2020 2020 2020 7265 6164 7320            reads 
-0000b1b0: 7468 6520 6f6e 6c79 206c 6179 6572 2069  the only layer i
-0000b1c0: 6e20 7468 6520 6669 6c65 206f 7220 7468  n the file or th
-0000b1d0: 726f 7773 2061 6e20 4578 6365 7074 696f  rows an Exceptio
-0000b1e0: 6e2e 0a20 2020 2020 2020 2069 676e 6f72  n..        ignor
-0000b1f0: 655f 6765 6f6d 6574 7279 2028 626f 6f6c  e_geometry (bool
-0000b200: 2c20 6f70 7469 6f6e 616c 293a 2054 7275  , optional): Tru
-0000b210: 6520 6e6f 7420 746f 2072 6561 642f 7265  e not to read/re
-0000b220: 7475 726e 2074 6865 2067 656f 6d61 7472  turn the geomatr
-0000b230: 792e 0a20 2020 2020 2020 2020 2020 2044  y..            D
-0000b240: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-0000b250: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
-0000b260: 2020 2020 2020 2020 556e 696f 6e5b 7064          Union[pd
-0000b270: 2e44 6174 6146 7261 6d65 2c20 6770 642e  .DataFrame, gpd.
-0000b280: 4765 6f44 6174 6146 7261 6d65 5d3a 2054  GeoDataFrame]: T
-0000b290: 6865 2064 6174 6120 7265 6164 2e0a 2020  he data read..  
-0000b2a0: 2020 2222 220a 2020 2020 7761 726e 696e    """.    warnin
-0000b2b0: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
-0000b2c0: 2027 7265 6164 5f66 696c 655f 7371 6c20   'read_file_sql 
-0000b2d0: 6973 2064 6570 7265 6361 7465 643a 2075  is deprecated: u
-0000b2e0: 7365 2072 6561 645f 6669 6c65 2120 4d69  se read_file! Mi
-0000b2f0: 6e64 3a20 7371 6c5f 6469 616c 6563 7420  nd: sql_dialect 
-0000b300: 6973 206e 6f74 2022 5351 4c49 5445 2220  is not "SQLITE" 
-0000b310: 270a 2020 2020 2020 2020 2262 7920 6465  '.        "by de
-0000b320: 6661 756c 7420 7468 6572 6521 222c 0a20  fault there!",. 
-0000b330: 2020 2020 2020 2046 7574 7572 6557 6172         FutureWar
-0000b340: 6e69 6e67 2c0a 2020 2020 290a 0a20 2020  ning,.    )..   
-0000b350: 2023 2052 756e 0a20 2020 2072 6574 7572   # Run.    retur
-0000b360: 6e20 5f72 6561 645f 6669 6c65 5f62 6173  n _read_file_bas
-0000b370: 6528 0a20 2020 2020 2020 2070 6174 682c  e(.        path,
-0000b380: 0a20 2020 2020 2020 2073 716c 5f73 746d  .        sql_stm
-0000b390: 743d 7371 6c5f 7374 6d74 2c0a 2020 2020  t=sql_stmt,.    
-0000b3a0: 2020 2020 7371 6c5f 6469 616c 6563 743d      sql_dialect=
-0000b3b0: 7371 6c5f 6469 616c 6563 742c 0a20 2020  sql_dialect,.   
-0000b3c0: 2020 2020 206c 6179 6572 3d6c 6179 6572       layer=layer
-0000b3d0: 2c0a 2020 2020 2020 2020 6967 6e6f 7265  ,.        ignore
-0000b3e0: 5f67 656f 6d65 7472 793d 6967 6e6f 7265  _geometry=ignore
-0000b3f0: 5f67 656f 6d65 7472 792c 0a20 2020 2029  _geometry,.    )
-0000b400: 0a0a 0a64 6566 2074 6f5f 6669 6c65 280a  ...def to_file(.
-0000b410: 2020 2020 6764 663a 2055 6e69 6f6e 5b70      gdf: Union[p
-0000b420: 642e 4461 7461 4672 616d 652c 2067 7064  d.DataFrame, gpd
-0000b430: 2e47 656f 4461 7461 4672 616d 655d 2c0a  .GeoDataFrame],.
-0000b440: 2020 2020 7061 7468 3a20 556e 696f 6e5b      path: Union[
-0000b450: 7374 722c 2022 6f73 2e50 6174 684c 696b  str, "os.PathLik
-0000b460: 655b 416e 795d 225d 2c0a 2020 2020 6c61  e[Any]"],.    la
-0000b470: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
-0000b480: 725d 203d 204e 6f6e 652c 0a20 2020 2066  r] = None,.    f
-0000b490: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
-0000b4a0: 6574 7279 7479 7065 3a20 556e 696f 6e5b  etrytype: Union[
-0000b4b0: 4765 6f6d 6574 7279 5479 7065 2c20 7374  GeometryType, st
-0000b4c0: 722c 204e 6f6e 655d 203d 204e 6f6e 652c  r, None] = None,
-0000b4d0: 0a20 2020 2066 6f72 6365 5f6d 756c 7469  .    force_multi
-0000b4e0: 7479 7065 3a20 626f 6f6c 203d 2046 616c  type: bool = Fal
-0000b4f0: 7365 2c0a 2020 2020 6170 7065 6e64 3a20  se,.    append: 
-0000b500: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-0000b510: 2020 6170 7065 6e64 5f74 696d 656f 7574    append_timeout
-0000b520: 5f73 3a20 696e 7420 3d20 3630 302c 0a20  _s: int = 600,. 
-0000b530: 2020 2069 6e64 6578 3a20 626f 6f6c 203d     index: bool =
-0000b540: 2054 7275 652c 0a20 2020 2063 7265 6174   True,.    creat
-0000b550: 655f 7370 6174 6961 6c5f 696e 6465 783a  e_spatial_index:
-0000b560: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-0000b570: 3d20 5472 7565 2c0a 293a 0a20 2020 2022  = True,.):.    "
-0000b580: 2222 0a20 2020 2057 7269 7465 7320 6120  "".    Writes a 
-0000b590: 7061 6e64 6173 2064 6174 6166 7261 6d65  pandas dataframe
-0000b5a0: 2074 6f20 6669 6c65 2e0a 0a20 2020 2054   to file...    T
-0000b5b0: 6865 2066 696c 6566 6f72 6d61 7420 6973  he fileformat is
-0000b5c0: 2064 6574 6563 7465 6420 6261 7365 6420   detected based 
-0000b5d0: 6f6e 2074 6865 2066 696c 6570 6174 6820  on the filepath 
-0000b5e0: 6578 7465 6e73 696f 6e2e 0a0a 2020 2020  extension...    
-0000b5f0: 5468 6520 756e 6465 726c 7969 6e67 206c  The underlying l
-0000b600: 6962 7261 7279 2075 7365 6420 746f 2077  ibrary used to w
-0000b610: 7269 7465 2074 6865 2066 696c 6520 6361  rite the file ca
-0000b620: 6e20 6265 2063 686f 6f73 656e 2075 7369  n be choosen usi
-0000b630: 6e67 2074 6865 0a20 2020 2022 4746 4f5f  ng the.    "GFO_
-0000b640: 494f 5f45 4e47 494e 4522 2065 6e76 6972  IO_ENGINE" envir
-0000b650: 6f6e 6d65 6e74 2076 6172 6961 626c 652e  onment variable.
-0000b660: 2050 6f73 7369 626c 6520 7661 6c75 6573   Possible values
-0000b670: 2061 7265 2022 6669 6f6e 6122 2061 6e64   are "fiona" and
-0000b680: 2022 7079 6f67 7269 6f22 2e0a 2020 2020   "pyogrio"..    
-0000b690: 4465 6661 756c 7420 656e 6769 6e65 2069  Default engine i
-0000b6a0: 7320 2270 796f 6772 696f 222e 0a0a 2020  s "pyogrio"...  
-0000b6b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000b6c0: 6764 6620 2867 7064 2e47 656f 4461 7461  gdf (gpd.GeoData
-0000b6d0: 4672 616d 6529 3a20 5468 6520 4765 6f44  Frame): The GeoD
-0000b6e0: 6174 6146 7261 6d65 2074 6f20 6578 706f  ataFrame to expo
-0000b6f0: 7274 2074 6f20 6669 6c65 2e0a 2020 2020  rt to file..    
-0000b700: 2020 2020 7061 7468 2028 556e 696f 6e5b      path (Union[
-0000b710: 7374 722c 293a 2054 6865 2066 696c 6520  str,): The file 
-0000b720: 7061 7468 2074 6f20 7772 6974 6520 746f  path to write to
-0000b730: 2e0a 2020 2020 2020 2020 6c61 7965 7220  ..        layer 
-0000b740: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-0000b750: 2054 6865 206c 6179 6572 2074 6f20 7265   The layer to re
-0000b760: 6164 2e20 4966 206e 6f20 6c61 7965 7220  ad. If no layer 
-0000b770: 6973 2073 7065 6369 6669 6564 2c0a 2020  is specified,.  
-0000b780: 2020 2020 2020 2020 2020 7265 6164 7320            reads 
-0000b790: 7468 6520 6f6e 6c79 206c 6179 6572 2069  the only layer i
-0000b7a0: 6e20 7468 6520 6669 6c65 206f 7220 7468  n the file or th
-0000b7b0: 726f 7773 2061 6e20 4578 6365 7074 696f  rows an Exceptio
-0000b7c0: 6e2e 0a20 2020 2020 2020 2066 6f72 6365  n..        force
-0000b7d0: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-0000b7e0: 7479 7065 2028 556e 696f 6e5b 4765 6f6d  type (Union[Geom
-0000b7f0: 6574 7279 5479 7065 2c20 7374 725d 2c20  etryType, str], 
-0000b800: 6f70 7469 6f6e 616c 293a 2047 656f 6d65  optional): Geome
-0000b810: 7472 7920 7479 7065 0a20 2020 2020 2020  try type.       
-0000b820: 2020 2020 2074 6f20 2874 7279 2074 6f29       to (try to)
-0000b830: 2066 6f72 6365 2074 6865 206f 7574 7075   force the outpu
-0000b840: 7420 746f 2e20 4465 6661 756c 7473 2074  t to. Defaults t
-0000b850: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-0000b860: 2020 2020 4d61 726b 3a20 636f 6d70 6172      Mark: compar
-0000b870: 6564 2074 6f20 6f74 6865 7220 6675 6e63  ed to other func
-0000b880: 7469 6f6e 7320 696e 2067 666f 2077 6974  tions in gfo wit
-0000b890: 6820 7468 6973 2070 6172 616d 6574 6572  h this parameter
-0000b8a0: 2c20 7468 6520 6265 6861 7669 6f75 720a  , the behaviour.
-0000b8b0: 2020 2020 2020 2020 2020 2020 6865 7265              here
-0000b8c0: 2069 7320 6c69 6d69 7465 6420 746f 2074   is limited to t
-0000b8d0: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 2020  he following:.  
-0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0000b8f0: 666f 7220 656d 7074 7920 696e 7075 7420  for empty input 
-0000b900: 6764 6627 732c 2061 2073 7461 6e64 6172  gdf's, a standar
-0000b910: 6420 6765 6f6d 6574 7279 2074 7970 6520  d geometry type 
-0000b920: 2865 672e 2050 6f6c 7967 6f6e 2c2e 2e2e  (eg. Polygon,...
-0000b930: 2920 6361 6e0a 2020 2020 2020 2020 2020  ) can.          
-0000b940: 2020 2020 2020 2020 6265 2075 7365 6420          be used 
-0000b950: 746f 2066 6f72 6365 2074 6865 2067 656f  to force the geo
-0000b960: 6d65 7472 7920 636f 6c75 6d6e 2074 6f20  metry column to 
-0000b970: 6265 206f 6620 7468 6174 2074 7970 652e  be of that type.
-0000b980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b990: 202d 2069 6620 666f 7263 655f 6f75 7470   - if force_outp
-0000b9a0: 7574 5f67 656f 6d65 7472 7974 7970 6520  ut_geometrytype 
-0000b9b0: 6973 2061 204d 554c 5449 2074 7970 652c  is a MULTI type,
-0000b9c0: 2070 6172 616d 6574 6572 0a20 2020 2020   parameter.     
-0000b9d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000b9e0: 6365 5f6d 756c 7469 7479 7065 2062 6563  ce_multitype bec
-0000b9f0: 6f6d 6573 2054 7275 652e 0a20 2020 2020  omes True..     
-0000ba00: 2020 2066 6f72 6365 5f6d 756c 7469 7479     force_multity
-0000ba10: 7065 2028 626f 6f6c 2c20 6f70 7469 6f6e  pe (bool, option
-0000ba20: 616c 293a 2066 6f72 6365 2074 6865 2067  al): force the g
-0000ba30: 656f 6d65 7472 7920 7479 7065 2074 6f20  eometry type to 
-0000ba40: 6120 6d75 6c74 6974 7970 650a 2020 2020  a multitype.    
-0000ba50: 2020 2020 2020 2020 666f 7220 6669 6c65          for file
-0000ba60: 2074 7970 6573 2074 6861 7420 7265 7175   types that requ
-0000ba70: 6972 6520 6f6e 6520 6765 6f6d 6574 7279  ire one geometry
-0000ba80: 7479 7065 2070 6572 206c 6179 6572 2e0a  type per layer..
-0000ba90: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-0000baa0: 756c 7473 2074 6f20 4661 6c73 652e 0a20  ults to False.. 
-0000bab0: 2020 2020 2020 2061 7070 656e 6420 2862         append (b
-0000bac0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-0000bad0: 5472 7565 2074 6f20 6170 7065 6e64 2074  True to append t
-0000bae0: 6f20 7468 6520 6669 6c65 2f6c 6179 6572  o the file/layer
-0000baf0: 2069 6620 6974 2065 7869 7374 7320 616c   if it exists al
-0000bb00: 7265 6164 792e 0a20 2020 2020 2020 2020  ready..         
-0000bb10: 2020 2049 6620 6974 2064 6f65 736e 2774     If it doesn't
-0000bb20: 2065 7869 7374 2079 6574 2c20 6974 2069   exist yet, it i
-0000bb30: 7320 6372 6561 7465 642e 2044 6566 6175  s created. Defau
-0000bb40: 6c74 7320 746f 2046 616c 7365 2e0a 2020  lts to False..  
-0000bb50: 2020 2020 2020 6170 7065 6e64 5f74 696d        append_tim
-0000bb60: 656f 7574 5f73 2028 696e 742c 206f 7074  eout_s (int, opt
-0000bb70: 696f 6e61 6c29 3a20 5468 6520 6d61 7869  ional): The maxi
-0000bb80: 6d75 6d20 7469 6d65 6f75 7420 746f 2077  mum timeout to w
-0000bb90: 6169 7420 7768 656e 2074 6865 0a20 2020  ait when the.   
-0000bba0: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-0000bbb0: 6669 6c65 2069 7320 616c 7265 6164 7920  file is already 
-0000bbc0: 6265 696e 6720 7772 6974 7465 6e20 746f  being written to
-0000bbd0: 2062 7920 616e 6f74 6865 7220 7072 6f63   by another proc
-0000bbe0: 6573 732e 0a20 2020 2020 2020 2020 2020  ess..           
-0000bbf0: 2044 6566 6175 6c74 7320 746f 2036 3030   Defaults to 600
-0000bc00: 2e0a 2020 2020 2020 2020 696e 6465 7820  ..        index 
-0000bc10: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
-0000bc20: 3a20 5472 7565 2074 6f20 7772 6974 6520  : True to write 
-0000bc30: 7468 6520 7061 6e64 6173 2069 6e64 6578  the pandas index
-0000bc40: 2074 6f20 7468 6520 6669 6c65 2061 730a   to the file as.
-0000bc50: 2020 2020 2020 2020 2020 2020 7765 6c6c              well
-0000bc60: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
-0000bc70: 7565 2e0a 2020 2020 2020 2020 6372 6561  ue..        crea
-0000bc80: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
-0000bc90: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-0000bca0: 293a 2054 7275 6520 746f 2066 6f72 6365  ): True to force
-0000bcb0: 2063 7265 6174 696f 6e20 6f66 2073 7061   creation of spa
-0000bcc0: 7469 616c 2069 6e64 6578 2c0a 2020 2020  tial index,.    
-0000bcd0: 2020 2020 2020 2020 4661 6c73 6520 746f          False to
-0000bce0: 2061 766f 6964 2063 7265 6174 696f 6e2e   avoid creation.
-0000bcf0: 204e 6f6e 6520 6c65 6164 7320 746f 2074   None leads to t
-0000bd00: 6865 2064 6566 6175 6c74 2062 6568 6176  he default behav
-0000bd10: 696f 7572 206f 6620 6764 616c 2e0a 2020  iour of gdal..  
-0000bd20: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-0000bd30: 7473 2074 6f20 5472 7565 2e0a 0a20 2020  ts to True...   
-0000bd40: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-0000bd50: 2056 616c 7565 4572 726f 723a 2061 6e20   ValueError: an 
-0000bd60: 696e 7661 6c69 6420 7061 7261 6d65 7465  invalid paramete
-0000bd70: 7220 7661 6c75 6520 7761 7320 7061 7373  r value was pass
-0000bd80: 6564 2e0a 2020 2020 2020 2020 5275 6e74  ed..        Runt
-0000bd90: 696d 6545 7272 6f72 3a20 7469 6d65 6f75  imeError: timeou
-0000bda0: 7420 7761 7320 7265 6163 6865 6420 7768  t was reached wh
-0000bdb0: 696c 6520 7472 7969 6e67 2074 6f20 6170  ile trying to ap
-0000bdc0: 7065 6e64 2064 6174 6120 746f 2070 6174  pend data to pat
-0000bdd0: 682e 0a20 2020 2022 2222 0a20 2020 2023  h..    """.    #
-0000bde0: 2043 6865 636b 2069 6e70 7574 2070 6172   Check input par
-0000bdf0: 616d 6574 6572 730a 2020 2020 2320 2d2d  ameters.    # --
-0000be00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000be10: 2d2d 2d2d 0a20 2020 2070 6174 6820 3d20  ----.    path = 
-0000be20: 5061 7468 2870 6174 6829 0a0a 2020 2020  Path(path)..    
-0000be30: 2320 4966 206e 6f20 6c61 7965 7220 6e61  # If no layer na
-0000be40: 6d65 2073 7065 6369 6669 6564 2c20 6465  me specified, de
-0000be50: 7465 726d 696e 6520 6f6e 650a 2020 2020  termine one.    
-0000be60: 6966 206c 6179 6572 2069 7320 4e6f 6e65  if layer is None
-0000be70: 3a0a 2020 2020 2020 2020 6966 2061 7070  :.        if app
-0000be80: 656e 6420 616e 6420 7061 7468 2e65 7869  end and path.exi
-0000be90: 7374 7328 293a 0a20 2020 2020 2020 2020  sts():.         
-0000bea0: 2020 206c 6179 6572 203d 2067 6574 5f6f     layer = get_o
-0000beb0: 6e6c 795f 6c61 7965 7228 7061 7468 290a  nly_layer(path).
-0000bec0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000bed0: 2020 2020 2020 2020 2020 6c61 7965 7220            layer 
-0000bee0: 3d20 5061 7468 2870 6174 6829 2e73 7465  = Path(path).ste
-0000bef0: 6d0a 0a20 2020 2023 2049 6620 666f 7263  m..    # If forc
-0000bf00: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
-0000bf10: 7974 7970 6520 6973 2061 2073 7472 696e  ytype is a strin
-0000bf20: 672c 2063 6865 636b 2069 6620 6974 2069  g, check if it i
-0000bf30: 7320 6120 2273 7461 6e64 6172 6422 2067  s a "standard" g
-0000bf40: 656f 6d65 7472 790a 2020 2020 2320 7479  eometry.    # ty
-0000bf50: 7065 2c20 6173 2047 4441 4c20 616c 736f  pe, as GDAL also
-0000bf60: 2073 7570 706f 7274 7320 7370 6563 6961   supports specia
-0000bf70: 6c20 6765 6f6d 6574 7279 2074 7970 6573  l geometry types
-0000bf80: 206c 696b 6520 2250 524f 4d4f 5445 5f54   like "PROMOTE_T
-0000bf90: 4f5f 4d55 4c54 4922 0a20 2020 2069 6620  O_MULTI".    if 
-0000bfa0: 6973 696e 7374 616e 6365 2866 6f72 6365  isinstance(force
-0000bfb0: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-0000bfc0: 7479 7065 2c20 7374 7229 3a0a 2020 2020  type, str):.    
-0000bfd0: 2020 2020 666f 7263 655f 6f75 7470 7574      force_output
-0000bfe0: 5f67 656f 6d65 7472 7974 7970 6520 3d20  _geometrytype = 
-0000bff0: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
-0000c000: 6d65 7472 7974 7970 652e 7570 7065 7228  metrytype.upper(
-0000c010: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-0000c020: 2020 2020 2020 2020 2020 2023 2056 6572             # Ver
-0000c030: 6966 7920 6966 2069 7420 6973 2061 2022  ify if it is a "
-0000c040: 7374 616e 6461 7264 2220 6765 6f6d 6574  standard" geomet
-0000c050: 7279 2074 7970 652c 2061 7320 4744 414c  ry type, as GDAL
-0000c060: 2061 6c73 6f20 7375 7070 6f72 7473 0a20   also supports. 
-0000c070: 2020 2020 2020 2020 2020 2023 2073 7065             # spe
-0000c080: 6369 616c 2067 656f 6d65 7472 7920 7479  cial geometry ty
-0000c090: 7065 7320 6c69 6b65 2022 5052 4f4d 4f54  pes like "PROMOT
-0000c0a0: 455f 544f 5f4d 554c 5449 220a 2020 2020  E_TO_MULTI".    
-0000c0b0: 2020 2020 2020 2020 666f 7263 655f 6f75          force_ou
-0000c0c0: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-0000c0d0: 6520 3d20 4765 6f6d 6574 7279 5479 7065  e = GeometryType
-0000c0e0: 5b66 6f72 6365 5f6f 7574 7075 745f 6765  [force_output_ge
-0000c0f0: 6f6d 6574 7279 7479 7065 5d0a 2020 2020  ometrytype].    
-0000c100: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0000c110: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-0000c120: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000c130: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000c140: 2020 2020 6622 556e 7375 7070 6f72 7465      f"Unsupporte
-0000c150: 6420 666f 7263 655f 6f75 7470 7574 5f67  d force_output_g
-0000c160: 656f 6d65 7472 7974 7970 653a 207b 666f  eometrytype: {fo
-0000c170: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
-0000c180: 7472 7974 7970 657d 220a 2020 2020 2020  trytype}".      
-0000c190: 2020 2020 2020 290a 2020 2020 6966 2066        ).    if f
-0000c1a0: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
-0000c1b0: 6574 7279 7479 7065 2069 7320 6e6f 7420  etrytype is not 
-0000c1c0: 4e6f 6e65 2061 6e64 2066 6f72 6365 5f6f  None and force_o
-0000c1d0: 7574 7075 745f 6765 6f6d 6574 7279 7479  utput_geometryty
-0000c1e0: 7065 2e69 735f 6d75 6c74 6974 7970 653a  pe.is_multitype:
-0000c1f0: 0a20 2020 2020 2020 2066 6f72 6365 5f6d  .        force_m
-0000c200: 756c 7469 7479 7065 203d 2054 7275 650a  ultitype = True.
-0000c210: 0a20 2020 2023 2049 6620 7468 6572 6520  .    # If there 
-0000c220: 6973 206e 6f20 6765 6f6d 6574 7279 2063  is no geometry c
-0000c230: 6f6c 756d 6e20 696e 2074 6865 2069 6e70  olumn in the inp
-0000c240: 7574 2c20 616c 7761 7973 2075 7365 2066  ut, always use f
-0000c250: 696f 6e61 2c20 6173 2070 796f 6772 696f  iona, as pyogrio
-0000c260: 2064 6f65 736e 2774 0a20 2020 2023 2073   doesn't.    # s
-0000c270: 7570 706f 7274 2074 6861 7420 7965 7420  upport that yet 
-0000c280: 6174 2074 696d 6520 6f66 2077 7269 7469  at time of writi
-0000c290: 6e67 2e0a 2020 2020 6966 2069 7369 6e73  ng..    if isins
-0000c2a0: 7461 6e63 6528 6764 662c 2067 7064 2e47  tance(gdf, gpd.G
-0000c2b0: 656f 4461 7461 4672 616d 6529 2069 7320  eoDataFrame) is 
-0000c2c0: 4661 6c73 6520 6f72 2028 0a20 2020 2020  False or (.     
-0000c2d0: 2020 2069 7369 6e73 7461 6e63 6528 6764     isinstance(gd
-0000c2e0: 662c 2067 7064 2e47 656f 4461 7461 4672  f, gpd.GeoDataFr
-0000c2f0: 616d 6529 2061 6e64 2022 6765 6f6d 6574  ame) and "geomet
-0000c300: 7279 2220 6e6f 7420 696e 2067 6466 2e63  ry" not in gdf.c
-0000c310: 6f6c 756d 6e73 0a20 2020 2029 3a0a 2020  olumns.    ):.  
-0000c320: 2020 2020 2020 656e 6769 6e65 203d 2022        engine = "
-0000c330: 6669 6f6e 6122 0a20 2020 2065 6c73 653a  fiona".    else:
-0000c340: 0a20 2020 2020 2020 2065 6e67 696e 6520  .        engine 
-0000c350: 3d20 5f67 6574 5f65 6e67 696e 6528 290a  = _get_engine().
-0000c360: 0a20 2020 2023 204e 6f77 2077 7269 7465  .    # Now write
-0000c370: 2077 6974 6820 7468 6520 636f 7272 6563   with the correc
-0000c380: 7420 656e 6769 6e65 0a20 2020 2069 6620  t engine.    if 
-0000c390: 656e 6769 6e65 203d 3d20 2270 796f 6772  engine == "pyogr
-0000c3a0: 696f 223a 0a20 2020 2020 2020 2072 6574  io":.        ret
-0000c3b0: 7572 6e20 5f74 6f5f 6669 6c65 5f70 796f  urn _to_file_pyo
-0000c3c0: 6772 696f 280a 2020 2020 2020 2020 2020  grio(.          
-0000c3d0: 2020 6764 663d 6764 662c 0a20 2020 2020    gdf=gdf,.     
-0000c3e0: 2020 2020 2020 2070 6174 683d 7061 7468         path=path
-0000c3f0: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
-0000c400: 7965 723d 6c61 7965 722c 0a20 2020 2020  yer=layer,.     
-0000c410: 2020 2020 2020 2066 6f72 6365 5f6f 7574         force_out
-0000c420: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
-0000c430: 3d66 6f72 6365 5f6f 7574 7075 745f 6765  =force_output_ge
-0000c440: 6f6d 6574 7279 7479 7065 2c0a 2020 2020  ometrytype,.    
-0000c450: 2020 2020 2020 2020 666f 7263 655f 6d75          force_mu
-0000c460: 6c74 6974 7970 653d 666f 7263 655f 6d75  ltitype=force_mu
-0000c470: 6c74 6974 7970 652c 0a20 2020 2020 2020  ltitype,.       
-0000c480: 2020 2020 2061 7070 656e 643d 6170 7065       append=appe
-0000c490: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-0000c4a0: 6170 7065 6e64 5f74 696d 656f 7574 5f73  append_timeout_s
-0000c4b0: 3d61 7070 656e 645f 7469 6d65 6f75 745f  =append_timeout_
-0000c4c0: 732c 0a20 2020 2020 2020 2020 2020 2069  s,.            i
-0000c4d0: 6e64 6578 3d69 6e64 6578 2c0a 2020 2020  ndex=index,.    
-0000c4e0: 2020 2020 2020 2020 6372 6561 7465 5f73          create_s
-0000c4f0: 7061 7469 616c 5f69 6e64 6578 3d63 7265  patial_index=cre
-0000c500: 6174 655f 7370 6174 6961 6c5f 696e 6465  ate_spatial_inde
-0000c510: 782c 0a20 2020 2020 2020 2029 0a20 2020  x,.        ).   
-0000c520: 2065 6c69 6620 656e 6769 6e65 203d 3d20   elif engine == 
-0000c530: 2266 696f 6e61 223a 0a20 2020 2020 2020  "fiona":.       
-0000c540: 2072 6574 7572 6e20 5f74 6f5f 6669 6c65   return _to_file
-0000c550: 5f66 696f 6e61 280a 2020 2020 2020 2020  _fiona(.        
-0000c560: 2020 2020 6764 663d 6764 662c 0a20 2020      gdf=gdf,.   
-0000c570: 2020 2020 2020 2020 2070 6174 683d 7061           path=pa
-0000c580: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0000c590: 6c61 7965 723d 6c61 7965 722c 0a20 2020  layer=layer,.   
-0000c5a0: 2020 2020 2020 2020 2066 6f72 6365 5f6f           force_o
-0000c5b0: 7574 7075 745f 6765 6f6d 6574 7279 7479  utput_geometryty
-0000c5c0: 7065 3d66 6f72 6365 5f6f 7574 7075 745f  pe=force_output_
-0000c5d0: 6765 6f6d 6574 7279 7479 7065 2c0a 2020  geometrytype,.  
-0000c5e0: 2020 2020 2020 2020 2020 666f 7263 655f            force_
-0000c5f0: 6d75 6c74 6974 7970 653d 666f 7263 655f  multitype=force_
-0000c600: 6d75 6c74 6974 7970 652c 0a20 2020 2020  multitype,.     
-0000c610: 2020 2020 2020 2061 7070 656e 643d 6170         append=ap
-0000c620: 7065 6e64 2c0a 2020 2020 2020 2020 2020  pend,.          
-0000c630: 2020 6170 7065 6e64 5f74 696d 656f 7574    append_timeout
-0000c640: 5f73 3d61 7070 656e 645f 7469 6d65 6f75  _s=append_timeou
-0000c650: 745f 732c 0a20 2020 2020 2020 2020 2020  t_s,.           
-0000c660: 2069 6e64 6578 3d69 6e64 6578 2c0a 2020   index=index,.  
-0000c670: 2020 2020 2020 2020 2020 6372 6561 7465            create
-0000c680: 5f73 7061 7469 616c 5f69 6e64 6578 3d63  _spatial_index=c
-0000c690: 7265 6174 655f 7370 6174 6961 6c5f 696e  reate_spatial_in
-0000c6a0: 6465 782c 0a20 2020 2020 2020 2029 0a20  dex,.        ). 
-0000c6b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c6c0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000c6d0: 7228 6622 556e 7375 7070 6f72 7465 6420  r(f"Unsupported 
-0000c6e0: 656e 6769 6e65 3a20 7b65 6e67 696e 657d  engine: {engine}
-0000c6f0: 2229 0a0a 0a64 6566 205f 6765 745f 656e  ")...def _get_en
-0000c700: 6769 6e65 2829 3a0a 2020 2020 7265 7475  gine():.    retu
-0000c710: 726e 206f 732e 656e 7669 726f 6e2e 6765  rn os.environ.ge
-0000c720: 7428 2247 464f 5f49 4f5f 454e 4749 4e45  t("GFO_IO_ENGINE
-0000c730: 222c 2022 7079 6f67 7269 6f22 290a 0a0a  ", "pyogrio")...
-0000c740: 6465 6620 5f74 6f5f 6669 6c65 5f66 696f  def _to_file_fio
-0000c750: 6e61 280a 2020 2020 6764 663a 2055 6e69  na(.    gdf: Uni
-0000c760: 6f6e 5b70 642e 4461 7461 4672 616d 652c  on[pd.DataFrame,
-0000c770: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-0000c780: 655d 2c0a 2020 2020 7061 7468 3a20 5061  e],.    path: Pa
-0000c790: 7468 2c0a 2020 2020 6c61 7965 723a 2073  th,.    layer: s
-0000c7a0: 7472 2c0a 2020 2020 666f 7263 655f 6f75  tr,.    force_ou
-0000c7b0: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-0000c7c0: 653a 2055 6e69 6f6e 5b47 656f 6d65 7472  e: Union[Geometr
-0000c7d0: 7954 7970 652c 2073 7472 2c20 4e6f 6e65  yType, str, None
-0000c7e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 666f  ] = None,.    fo
-0000c7f0: 7263 655f 6d75 6c74 6974 7970 653a 2062  rce_multitype: b
-0000c800: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000c810: 2061 7070 656e 643a 2062 6f6f 6c20 3d20   append: bool = 
-0000c820: 4661 6c73 652c 0a20 2020 2061 7070 656e  False,.    appen
-0000c830: 645f 7469 6d65 6f75 745f 733a 2069 6e74  d_timeout_s: int
-0000c840: 203d 2036 3030 2c0a 2020 2020 696e 6465   = 600,.    inde
-0000c850: 783a 2062 6f6f 6c20 3d20 5472 7565 2c0a  x: bool = True,.
-0000c860: 2020 2020 6372 6561 7465 5f73 7061 7469      create_spati
-0000c870: 616c 5f69 6e64 6578 3a20 4f70 7469 6f6e  al_index: Option
-0000c880: 616c 5b62 6f6f 6c5d 203d 2054 7275 652c  al[bool] = True,
-0000c890: 0a29 3a0a 2020 2020 2222 220a 2020 2020  .):.    """.    
-0000c8a0: 5772 6974 6573 2061 2070 616e 6461 7320  Writes a pandas 
-0000c8b0: 6461 7461 6672 616d 6520 746f 2066 696c  dataframe to fil
-0000c8c0: 6520 7573 696e 6720 6669 6f6e 612e 0a20  e using fiona.. 
-0000c8d0: 2020 2022 2222 0a20 2020 2023 2048 616e     """.    # Han
-0000c8e0: 646c 6520 736f 6d65 2073 7065 6369 6669  dle some specifi
-0000c8f0: 6320 6361 7365 7320 7768 6572 6520 7468  c cases where th
-0000c900: 6520 6669 6c65 2073 6368 656d 6120 6e65  e file schema ne
-0000c910: 6564 7320 746f 2062 6520 6d61 6e69 7075  eds to be manipu
-0000c920: 6c61 7465 642e 0a20 2020 2073 6368 656d  lated..    schem
-0000c930: 6120 3d20 4e6f 6e65 0a20 2020 2069 6620  a = None.    if 
-0000c940: 6973 696e 7374 616e 6365 2867 6466 2c20  isinstance(gdf, 
-0000c950: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
-0000c960: 2920 6973 2046 616c 7365 206f 7220 280a  ) is False or (.
-0000c970: 2020 2020 2020 2020 6973 696e 7374 616e          isinstan
-0000c980: 6365 2867 6466 2c20 6770 642e 4765 6f44  ce(gdf, gpd.GeoD
-0000c990: 6174 6146 7261 6d65 2920 616e 6420 2267  ataFrame) and "g
-0000c9a0: 656f 6d65 7472 7922 206e 6f74 2069 6e20  eometry" not in 
-0000c9b0: 6764 662e 636f 6c75 6d6e 730a 2020 2020  gdf.columns.    
-0000c9c0: 293a 0a20 2020 2020 2020 2023 204e 6f20  ):.        # No 
-0000c9d0: 6765 6f6d 6574 7279 2c20 736f 2070 7265  geometry, so pre
-0000c9e0: 7061 7265 2074 6f20 6265 2077 7269 7474  pare to be writt
-0000c9f0: 656e 2061 7320 6174 7472 6962 7574 6520  en as attribute 
-0000ca00: 7461 626c 653a 2061 6464 2067 656f 6d65  table: add geome
-0000ca10: 7472 7920 636f 6c75 6d6e 0a20 2020 2020  try column.     
-0000ca20: 2020 2023 2077 6974 6820 4e6f 6e65 2067     # with None g
-0000ca30: 656f 6d65 7472 7920 7479 7065 2069 6e20  eometry type in 
-0000ca40: 7363 6865 6d61 0a20 2020 2020 2020 2067  schema.        g
-0000ca50: 6466 203d 2067 7064 2e47 656f 4461 7461  df = gpd.GeoData
-0000ca60: 4672 616d 6528 6764 662c 2067 656f 6d65  Frame(gdf, geome
-0000ca70: 7472 793d 5b4e 6f6e 6520 666f 7220 6920  try=[None for i 
-0000ca80: 696e 2067 6466 2e69 6e64 6578 5d29 2020  in gdf.index])  
-0000ca90: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
-0000caa0: 2020 2020 2020 2073 6368 656d 6120 3d20         schema = 
-0000cab0: 6770 645f 696f 5f66 696c 652e 696e 6665  gpd_io_file.infe
-0000cac0: 725f 7363 6865 6d61 2867 6466 290a 2020  r_schema(gdf).  
-0000cad0: 2020 2020 2020 7363 6865 6d61 5b22 6765        schema["ge
-0000cae0: 6f6d 6574 7279 225d 203d 2022 4e6f 6e65  ometry"] = "None
-0000caf0: 220a 2020 2020 656c 6966 2028 0a20 2020  ".    elif (.   
-0000cb00: 2020 2020 206c 656e 2867 6466 2920 3d3d       len(gdf) ==
-0000cb10: 2030 0a20 2020 2020 2020 2061 6e64 2066   0.        and f
-0000cb20: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
-0000cb30: 6574 7279 7479 7065 2069 7320 6e6f 7420  etrytype is not 
-0000cb40: 4e6f 6e65 0a20 2020 2020 2020 2061 6e64  None.        and
-0000cb50: 2069 7369 6e73 7461 6e63 6528 666f 7263   isinstance(forc
-0000cb60: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
-0000cb70: 7974 7970 652c 2047 656f 6d65 7472 7954  ytype, GeometryT
-0000cb80: 7970 6529 0a20 2020 2029 3a0a 2020 2020  ype).    ):.    
-0000cb90: 2020 2020 2320 4966 2074 6865 2067 6466      # If the gdf
-0000cba0: 2069 7320 656d 7074 7920 6275 7420 6120   is empty but a 
-0000cbb0: 6765 6f6d 6574 7279 2074 7970 6520 6973  geometry type is
-0000cbc0: 2073 7065 6369 6669 6564 2c20 7573 6520   specified, use 
-0000cbd0: 7468 6520 7370 6563 6966 6965 6420 7479  the specified ty
-0000cbe0: 7065 0a20 2020 2020 2020 2073 6368 656d  pe.        schem
-0000cbf0: 6120 3d20 6770 645f 696f 5f66 696c 652e  a = gpd_io_file.
-0000cc00: 696e 6665 725f 7363 6865 6d61 2867 6466  infer_schema(gdf
-0000cc10: 290a 2020 2020 2020 2020 2320 4765 6f6d  ).        # Geom
-0000cc20: 6574 7279 2074 7970 6520 6d75 7374 2062  etry type must b
-0000cc30: 6520 696e 2063 616d 656c 6361 7365 2066  e in camelcase f
-0000cc40: 6f72 2066 696f 6e61 0a20 2020 2020 2020  or fiona.       
-0000cc50: 2073 6368 656d 615b 2267 656f 6d65 7472   schema["geometr
-0000cc60: 7922 5d20 3d20 666f 7263 655f 6f75 7470  y"] = force_outp
-0000cc70: 7574 5f67 656f 6d65 7472 7974 7970 652e  ut_geometrytype.
-0000cc80: 6e61 6d65 5f63 616d 656c 6361 7365 0a20  name_camelcase. 
-0000cc90: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-0000cca0: 616e 6365 2867 6466 2c20 6770 642e 4765  ance(gdf, gpd.Ge
-0000ccb0: 6f44 6174 6146 7261 6d65 290a 0a20 2020  oDataFrame)..   
-0000ccc0: 2023 2043 6f6e 7665 7274 2066 6f72 6365   # Convert force
-0000ccd0: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-0000cce0: 7479 7065 2074 6f20 7374 7269 6e67 2074  type to string t
-0000ccf0: 6f20 7369 6d70 6c69 6679 2063 6f64 6520  o simplify code 
-0000cd00: 6166 7465 7277 6172 6473 0a20 2020 2069  afterwards.    i
-0000cd10: 6620 6973 696e 7374 616e 6365 2866 6f72  f isinstance(for
-0000cd20: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
-0000cd30: 7279 7479 7065 2c20 4765 6f6d 6574 7279  rytype, Geometry
-0000cd40: 5479 7065 293a 0a20 2020 2020 2020 2066  Type):.        f
-0000cd50: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
-0000cd60: 6574 7279 7479 7065 203d 2066 6f72 6365  etrytype = force
-0000cd70: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-0000cd80: 7479 7065 2e6e 616d 650a 0a20 2020 2023  type.name..    #
-0000cd90: 204e 6f20 7468 6520 6669 6c65 2063 616e   No the file can
-0000cda0: 2061 6374 7561 6c6c 7920 6265 2077 7269   actually be wri
-0000cdb0: 7474 656e 0a20 2020 2023 202d 2d2d 2d2d  tten.    # -----
-0000cdc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000cdd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-0000cde0: 2020 2023 2046 696f 6e61 2064 6f65 736e     # Fiona doesn
-0000cdf0: 2774 2073 7570 706f 7274 2074 6865 206f  't support the o
-0000ce00: 7574 7075 7420 6765 6f6d 6574 7279 7479  utput geometryty
-0000ce10: 7065 2070 6172 616d 6574 6572 2061 7320  pe parameter as 
-0000ce20: 7573 6564 2069 6e20 6764 616c 2c20 736f  used in gdal, so
-0000ce30: 2061 7320 610a 2020 2020 2320 6c69 6768   as a.    # ligh
-0000ce40: 7477 6569 6768 7420 696d 706c 656d 656e  tweight implemen
-0000ce50: 7461 7469 6f6e 206a 7573 7420 7365 7420  tation just set 
-0000ce60: 666f 7263 650a 2020 2020 6465 6620 7772  force.    def wr
-0000ce70: 6974 655f 746f 5f66 696c 6528 0a20 2020  ite_to_file(.   
-0000ce80: 2020 2020 2067 6466 3a20 6770 642e 4765       gdf: gpd.Ge
-0000ce90: 6f44 6174 6146 7261 6d65 2c0a 2020 2020  oDataFrame,.    
-0000cea0: 2020 2020 7061 7468 3a20 5061 7468 2c0a      path: Path,.
-0000ceb0: 2020 2020 2020 2020 6c61 7965 723a 2073          layer: s
-0000cec0: 7472 2c0a 2020 2020 2020 2020 696e 6465  tr,.        inde
-0000ced0: 783a 2062 6f6f 6c20 3d20 5472 7565 2c0a  x: bool = True,.
-0000cee0: 2020 2020 2020 2020 666f 7263 655f 6f75          force_ou
-0000cef0: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-0000cf00: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-0000cf10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000cf20: 2066 6f72 6365 5f6d 756c 7469 7479 7065   force_multitype
-0000cf30: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-0000cf40: 2020 2020 2020 2020 6170 7065 6e64 3a20          append: 
-0000cf50: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-0000cf60: 2020 2020 2020 7363 6865 6d61 3a20 4f70        schema: Op
-0000cf70: 7469 6f6e 616c 5b64 6963 745d 203d 204e  tional[dict] = N
-0000cf80: 6f6e 652c 0a20 2020 2020 2020 2063 7265  one,.        cre
-0000cf90: 6174 655f 7370 6174 6961 6c5f 696e 6465  ate_spatial_inde
-0000cfa0: 783a 204f 7074 696f 6e61 6c5b 626f 6f6c  x: Optional[bool
-0000cfb0: 5d20 3d20 5472 7565 2c0a 2020 2020 293a  ] = True,.    ):
-0000cfc0: 0a20 2020 2020 2020 2023 2050 7265 7061  .        # Prepa
-0000cfd0: 7265 2061 7267 7320 666f 7220 746f 5f66  re args for to_f
-0000cfe0: 696c 650a 2020 2020 2020 2020 6966 2061  ile.        if a
-0000cff0: 7070 656e 6420 6973 2054 7275 653a 0a20  ppend is True:. 
-0000d000: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
-0000d010: 7468 2e65 7869 7374 7328 293a 0a20 2020  th.exists():.   
-0000d020: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-0000d030: 6520 3d20 2261 220a 2020 2020 2020 2020  e = "a".        
-0000d040: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d050: 2020 2020 2020 2020 2020 6d6f 6465 203d            mode =
-0000d060: 2022 7722 0a20 2020 2020 2020 2065 6c73   "w".        els
-0000d070: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
-0000d080: 6f64 6520 3d20 2277 220a 0a20 2020 2020  ode = "w"..     
-0000d090: 2020 206b 7761 7267 7320 3d20 7b7d 0a20     kwargs = {}. 
-0000d0a0: 2020 2020 2020 206b 7761 7267 735b 226d         kwargs["m
-0000d0b0: 6f64 6522 5d20 3d20 6d6f 6465 0a20 2020  ode"] = mode.   
-0000d0c0: 2020 2020 2067 656f 6669 6c65 7479 7065       geofiletype
-0000d0d0: 203d 2047 656f 6669 6c65 5479 7065 2870   = GeofileType(p
-0000d0e0: 6174 6829 0a20 2020 2020 2020 206b 7761  ath).        kwa
-0000d0f0: 7267 735b 2264 7269 7665 7222 5d20 3d20  rgs["driver"] = 
-0000d100: 6765 6f66 696c 6574 7970 652e 6f67 7264  geofiletype.ogrd
-0000d110: 7269 7665 720a 2020 2020 2020 2020 6966  river.        if
-0000d120: 2063 7265 6174 655f 7370 6174 6961 6c5f   create_spatial_
-0000d130: 696e 6465 7820 6973 206e 6f74 204e 6f6e  index is not Non
-0000d140: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
-0000d150: 7761 7267 735b 2253 5041 5449 414c 5f49  wargs["SPATIAL_I
-0000d160: 4e44 4558 225d 203d 2063 7265 6174 655f  NDEX"] = create_
-0000d170: 7370 6174 6961 6c5f 696e 6465 780a 2020  spatial_index.  
-0000d180: 2020 2020 2020 6966 2066 6f72 6365 5f6f        if force_o
-0000d190: 7574 7075 745f 6765 6f6d 6574 7279 7479  utput_geometryty
-0000d1a0: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-0000d1b0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-0000d1c0: 6773 5b22 6765 6f6d 6574 7279 7479 7065  gs["geometrytype
-0000d1d0: 225d 203d 2066 6f72 6365 5f6f 7574 7075  "] = force_outpu
-0000d1e0: 745f 6765 6f6d 6574 7279 7479 7065 0a20  t_geometrytype. 
-0000d1f0: 2020 2020 2020 2069 6620 7363 6865 6d61         if schema
-0000d200: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000d210: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-0000d220: 5b22 7363 6865 6d61 225d 203d 2073 6368  ["schema"] = sch
-0000d230: 656d 610a 0a20 2020 2020 2020 2023 204e  ema..        # N
-0000d240: 6f77 2077 6520 6361 6e20 7772 6974 650a  ow we can write.
-0000d250: 2020 2020 2020 2020 6966 2067 656f 6669          if geofi
-0000d260: 6c65 7479 7065 203d 3d20 4765 6f66 696c  letype == Geofil
-0000d270: 6554 7970 652e 4553 5249 5368 6170 6566  eType.ESRIShapef
-0000d280: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-0000d290: 2069 6620 696e 6465 7820 6973 2054 7275   if index is Tru
-0000d2a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000d2b0: 2020 2067 6466 5f74 6f5f 7772 6974 6520     gdf_to_write 
-0000d2c0: 3d20 6764 662e 7265 7365 745f 696e 6465  = gdf.reset_inde
-0000d2d0: 7828 6472 6f70 3d54 7275 6529 0a20 2020  x(drop=True).   
-0000d2e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0000d300: 6466 5f74 6f5f 7772 6974 6520 3d20 6764  df_to_write = gd
-0000d310: 660a 2020 2020 2020 2020 2020 2020 6764  f.            gd
-0000d320: 665f 746f 5f77 7269 7465 2e74 6f5f 6669  f_to_write.to_fi
-0000d330: 6c65 2873 7472 2870 6174 6829 2c20 2a2a  le(str(path), **
-0000d340: 6b77 6172 6773 2920 2023 2074 7970 653a  kwargs)  # type:
-0000d350: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
-0000d360: 656c 6966 2067 656f 6669 6c65 7479 7065  elif geofiletype
-0000d370: 203d 3d20 4765 6f66 696c 6554 7970 652e   == GeofileType.
-0000d380: 4750 4b47 3a0a 2020 2020 2020 2020 2020  GPKG:.          
-0000d390: 2020 2320 5472 7920 746f 2068 6172 6d6f    # Try to harmo
-0000d3a0: 6e69 7a65 2074 6865 2067 656f 6d65 7472  nize the geometr
-0000d3b0: 7974 7970 6520 746f 206f 6e65 2028 6d75  ytype to one (mu
-0000d3c0: 6c74 6929 7479 7065 2c20 6173 2047 504b  lti)type, as GPK
-0000d3d0: 470a 2020 2020 2020 2020 2020 2020 2320  G.            # 
-0000d3e0: 646f 6573 6e27 7420 6c69 6b65 203e 2031  doesn't like > 1
-0000d3f0: 2074 7970 6520 696e 2061 206c 6179 6572   type in a layer
-0000d400: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d410: 7363 6865 6d61 2069 7320 4e6f 6e65 206f  schema is None o
-0000d420: 7220 286c 656e 2867 6466 2920 3e20 3020  r (len(gdf) > 0 
-0000d430: 616e 6420 7363 6865 6d61 5b22 6765 6f6d  and schema["geom
-0000d440: 6574 7279 225d 2021 3d20 224e 6f6e 6522  etry"] != "None"
-0000d450: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000d460: 2020 2067 6466 5f74 6f5f 7772 6974 6520     gdf_to_write 
-0000d470: 3d20 6764 662e 636f 7079 2829 0a20 2020  = gdf.copy().   
-0000d480: 2020 2020 2020 2020 2020 2020 2067 6466               gdf
-0000d490: 5f74 6f5f 7772 6974 652e 6765 6f6d 6574  _to_write.geomet
-0000d4a0: 7279 203d 2067 656f 7365 7269 6573 5f75  ry = geoseries_u
-0000d4b0: 7469 6c2e 6861 726d 6f6e 697a 655f 6765  til.harmonize_ge
-0000d4c0: 6f6d 6574 7279 7479 7065 7328 0a20 2020  ometrytypes(.   
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 2067 6466 2e67 656f 6d65 7472 792c 2066   gdf.geometry, f
-0000d4f0: 6f72 6365 5f6d 756c 7469 7479 7065 3d66  orce_multitype=f
-0000d500: 6f72 6365 5f6d 756c 7469 7479 7065 0a20  orce_multitype. 
-0000d510: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000d520: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000d530: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000d540: 2020 2067 6466 5f74 6f5f 7772 6974 6520     gdf_to_write 
-0000d550: 3d20 6764 660a 2020 2020 2020 2020 2020  = gdf.          
-0000d560: 2020 6764 665f 746f 5f77 7269 7465 2e74    gdf_to_write.t
-0000d570: 6f5f 6669 6c65 2873 7472 2870 6174 6829  o_file(str(path)
-0000d580: 2c20 6c61 7965 723d 6c61 7965 722c 202a  , layer=layer, *
-0000d590: 2a6b 7761 7267 7329 2020 2320 7479 7065  *kwargs)  # type
-0000d5a0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-0000d5b0: 2065 6c69 6620 6765 6f66 696c 6574 7970   elif geofiletyp
-0000d5c0: 6520 3d3d 2047 656f 6669 6c65 5479 7065  e == GeofileType
-0000d5d0: 2e53 514c 6974 653a 0a20 2020 2020 2020  .SQLite:.       
-0000d5e0: 2020 2020 2067 6466 2e74 6f5f 6669 6c65       gdf.to_file
-0000d5f0: 2873 7472 2870 6174 6829 2c20 6c61 7965  (str(path), laye
-0000d600: 723d 6c61 7965 722c 202a 2a6b 7761 7267  r=layer, **kwarg
-0000d610: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
-0000d620: 6765 6f66 696c 6574 7970 6520 3d3d 2047  geofiletype == G
-0000d630: 656f 6669 6c65 5479 7065 2e47 656f 4a53  eofileType.GeoJS
-0000d640: 4f4e 3a0a 2020 2020 2020 2020 2020 2020  ON:.            
-0000d650: 6764 662e 746f 5f66 696c 6528 7374 7228  gdf.to_file(str(
-0000d660: 7061 7468 292c 202a 2a6b 7761 7267 7329  path), **kwargs)
-0000d670: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000d680: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000d690: 2056 616c 7565 4572 726f 7228 6622 4e6f   ValueError(f"No
-0000d6a0: 7420 696d 706c 656d 656e 7465 6420 666f  t implemented fo
-0000d6b0: 7220 6765 6f66 696c 6574 7970 6520 7b67  r geofiletype {g
-0000d6c0: 656f 6669 6c65 7479 7065 7d22 290a 0a20  eofiletype}").. 
-0000d6d0: 2020 2023 2049 6620 6e6f 2061 7070 656e     # If no appen
-0000d6e0: 642c 206a 7573 7420 7772 6974 6520 746f  d, just write to
-0000d6f0: 206f 7574 7075 7420 7061 7468 0a20 2020   output path.   
-0000d700: 2069 6620 6e6f 7420 6170 7065 6e64 3a0a   if not append:.
-0000d710: 2020 2020 2020 2020 7772 6974 655f 746f          write_to
-0000d720: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
-0000d730: 2020 2067 6466 3d67 6466 2c0a 2020 2020     gdf=gdf,.    
-0000d740: 2020 2020 2020 2020 7061 7468 3d70 6174          path=pat
-0000d750: 682c 0a20 2020 2020 2020 2020 2020 206c  h,.            l
-0000d760: 6179 6572 3d6c 6179 6572 2c0a 2020 2020  ayer=layer,.    
-0000d770: 2020 2020 2020 2020 696e 6465 783d 696e          index=in
-0000d780: 6465 782c 0a20 2020 2020 2020 2020 2020  dex,.           
-0000d790: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
-0000d7a0: 6f6d 6574 7279 7479 7065 3d66 6f72 6365  ometrytype=force
-0000d7b0: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-0000d7c0: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
-0000d7d0: 2020 666f 7263 655f 6d75 6c74 6974 7970    force_multityp
-0000d7e0: 653d 666f 7263 655f 6d75 6c74 6974 7970  e=force_multityp
-0000d7f0: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
-0000d800: 7070 656e 643d 6170 7065 6e64 2c0a 2020  ppend=append,.  
-0000d810: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-0000d820: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
-0000d830: 2020 2020 2063 7265 6174 655f 7370 6174       create_spat
-0000d840: 6961 6c5f 696e 6465 783d 6372 6561 7465  ial_index=create
-0000d850: 5f73 7061 7469 616c 5f69 6e64 6578 2c0a  _spatial_index,.
-0000d860: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-0000d870: 7365 3a0a 2020 2020 2020 2020 2320 4170  se:.        # Ap
-0000d880: 7065 6e64 2069 7320 6173 6b65 642c 2063  pend is asked, c
-0000d890: 6865 636b 2069 6620 7468 6520 6669 6f6e  heck if the fion
-0000d8a0: 6120 6472 6976 6572 2073 7570 706f 7274  a driver support
-0000d8b0: 7320 6170 7065 6e64 696e 672e 2049 660a  s appending. If.
-0000d8c0: 2020 2020 2020 2020 2320 6e6f 742c 2077          # not, w
-0000d8d0: 7269 7465 2074 6f20 7465 6d70 6f72 6172  rite to temporar
-0000d8e0: 7920 6f75 7470 7574 2066 696c 650a 0a20  y output file.. 
-0000d8f0: 2020 2020 2020 2023 2052 656d 6172 6b3a         # Remark:
-0000d900: 2066 696f 6e61 2070 7265 2d31 2e38 2e31   fiona pre-1.8.1
-0000d910: 3420 6469 646e 2774 2073 7570 706f 7274  4 didn't support
-0000d920: 2061 7070 656e 6469 6e67 2074 6f20 6765   appending to ge
-0000d930: 6f70 6163 6b61 6765 2e20 4f6e 6365 0a20  opackage. Once. 
-0000d940: 2020 2020 2020 2023 206f 6c64 6572 2076         # older v
-0000d950: 6572 7369 6f6e 7320 6265 636f 6d65 7320  ersions becomes 
-0000d960: 7261 7265 2c20 6465 7065 6e64 656e 6379  rare, dependency
-0000d970: 2063 616e 2062 6520 7075 7420 746f 2074   can be put to t
-0000d980: 6869 7320 7665 7273 696f 6e2c 2061 6e64  his version, and
-0000d990: 0a20 2020 2020 2020 2023 2074 6869 7320  .        # this 
-0000d9a0: 636f 6465 2063 616e 2062 6520 636c 6561  code can be clea
-0000d9b0: 6e65 6420 7570 2e2e 2e0a 2020 2020 2020  ned up....      
-0000d9c0: 2020 6765 6f66 696c 6574 7970 6520 3d20    geofiletype = 
-0000d9d0: 4765 6f66 696c 6554 7970 6528 7061 7468  GeofileType(path
-0000d9e0: 290a 2020 2020 2020 2020 6764 6674 656d  ).        gdftem
-0000d9f0: 705f 7061 7468 203d 204e 6f6e 650a 2020  p_path = None.  
-0000da00: 2020 2020 2020 6764 6674 656d 705f 6c6f        gdftemp_lo
-0000da10: 636b 7061 7468 203d 204e 6f6e 650a 2020  ckpath = None.  
-0000da20: 2020 2020 2020 6966 2022 6122 206e 6f74        if "a" not
-0000da30: 2069 6e20 6669 6f6e 612e 7375 7070 6f72   in fiona.suppor
-0000da40: 7465 645f 6472 6976 6572 735b 6765 6f66  ted_drivers[geof
-0000da50: 696c 6574 7970 652e 6f67 7264 7269 7665  iletype.ogrdrive
-0000da60: 725d 3a0a 2020 2020 2020 2020 2020 2020  r]:.            
-0000da70: 2320 4765 7420 6120 756e 6971 7565 2074  # Get a unique t
-0000da80: 656d 7020 6669 6c65 2070 6174 682e 2054  emp file path. T
-0000da90: 6865 2066 696c 6520 6361 6e6e 6f74 2062  he file cannot b
-0000daa0: 6520 6372 6561 7465 6420 7965 742c 2073  e created yet, s
-0000dab0: 6f0a 2020 2020 2020 2020 2020 2020 2320  o.            # 
-0000dac0: 6f6e 6c79 2063 7265 6174 6520 6120 6c6f  only create a lo
-0000dad0: 636b 2066 696c 6520 746f 2065 7661 6465  ck file to evade
-0000dae0: 206f 7468 6572 2070 726f 6365 7373 6573   other processes
-0000daf0: 2075 7369 6e67 2074 6865 2073 616d 650a   using the same.
-0000db00: 2020 2020 2020 2020 2020 2020 2320 7465              # te
-0000db10: 6d70 2066 696c 6520 6e61 6d65 0a20 2020  mp file name.   
-0000db20: 2020 2020 2020 2020 2067 6466 7465 6d70           gdftemp
-0000db30: 5f70 6174 682c 2067 6466 7465 6d70 5f6c  _path, gdftemp_l
-0000db40: 6f63 6b70 6174 6820 3d20 5f69 6f5f 7574  ockpath = _io_ut
-0000db50: 696c 2e67 6574 5f74 656d 7066 696c 655f  il.get_tempfile_
-0000db60: 6c6f 636b 6564 280a 2020 2020 2020 2020  locked(.        
-0000db70: 2020 2020 2020 2020 6261 7365 5f66 696c          base_fil
-0000db80: 656e 616d 653d 2267 6466 7465 6d70 222c  ename="gdftemp",
-0000db90: 2073 7566 6669 783d 7061 7468 2e73 7566   suffix=path.suf
-0000dba0: 6669 782c 2064 6972 6e61 6d65 3d22 6765  fix, dirname="ge
-0000dbb0: 6f66 696c 655f 746f 5f66 696c 6522 0a20  ofile_to_file". 
-0000dbc0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000dbd0: 2020 2020 2020 2020 2077 7269 7465 5f74           write_t
-0000dbe0: 6f5f 6669 6c65 280a 2020 2020 2020 2020  o_file(.        
-0000dbf0: 2020 2020 2020 2020 6764 662c 0a20 2020          gdf,.   
-0000dc00: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-0000dc10: 683d 6764 6674 656d 705f 7061 7468 2c0a  h=gdftemp_path,.
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc30: 6c61 7965 723d 6c61 7965 722c 0a20 2020  layer=layer,.   
-0000dc40: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-0000dc50: 6578 3d69 6e64 6578 2c0a 2020 2020 2020  ex=index,.      
-0000dc60: 2020 2020 2020 2020 2020 666f 7263 655f            force_
-0000dc70: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
-0000dc80: 7970 653d 666f 7263 655f 6f75 7470 7574  ype=force_output
-0000dc90: 5f67 656f 6d65 7472 7974 7970 652c 0a20  _geometrytype,. 
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000dcb0: 6f72 6365 5f6d 756c 7469 7479 7065 3d66  orce_multitype=f
-0000dcc0: 6f72 6365 5f6d 756c 7469 7479 7065 2c0a  orce_multitype,.
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dce0: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
-0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000dd00: 7265 6174 655f 7370 6174 6961 6c5f 696e  reate_spatial_in
-0000dd10: 6465 783d 6372 6561 7465 5f73 7061 7469  dex=create_spati
-0000dd20: 616c 5f69 6e64 6578 2c0a 2020 2020 2020  al_index,.      
-0000dd30: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000dd40: 2023 2046 696c 6573 2064 6f6e 2774 2074   # Files don't t
-0000dd50: 7970 6963 616c 6c79 2073 7570 706f 7274  ypically support
-0000dd60: 2068 6176 696e 6720 6d75 6c74 6970 6c65   having multiple
-0000dd70: 2070 726f 6365 7373 6573 2077 7269 7469   processes writi
-0000dd80: 6e67 0a20 2020 2020 2020 2023 2073 696d  ng.        # sim
-0000dd90: 756c 7461 6e6f 7573 6c79 2074 6f20 7468  ultanously to th
-0000dda0: 656d 2c20 736f 2075 7365 206c 6f63 6b20  em, so use lock 
-0000ddb0: 6669 6c65 2074 6f20 7379 6e63 6872 6f6e  file to synchron
-0000ddc0: 697a 6520 6163 6365 7373 2e0a 2020 2020  ize access..    
-0000ddd0: 2020 2020 6c6f 636b 6669 6c65 203d 2050      lockfile = P
-0000dde0: 6174 6828 6622 7b73 7472 2870 6174 6829  ath(f"{str(path)
-0000ddf0: 7d2e 6c6f 636b 2229 0a20 2020 2020 2020  }.lock").       
-0000de00: 2073 7461 7274 5f74 696d 6520 3d20 6461   start_time = da
-0000de10: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-0000de20: 6e6f 7728 290a 2020 2020 2020 2020 7265  now().        re
-0000de30: 6164 7920 3d20 4661 6c73 650a 2020 2020  ady = False.    
-0000de40: 2020 2020 7768 696c 6520 6e6f 7420 7265      while not re
-0000de50: 6164 793a 0a20 2020 2020 2020 2020 2020  ady:.           
-0000de60: 2069 6620 5f69 6f5f 7574 696c 2e63 7265   if _io_util.cre
-0000de70: 6174 655f 6669 6c65 5f61 746f 6d69 6328  ate_file_atomic(
-0000de80: 6c6f 636b 6669 6c65 2920 6973 2054 7275  lockfile) is Tru
-0000de90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000dea0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000deb0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-0000dec0: 2067 6466 2077 6173 6e27 7420 7772 6974   gdf wasn't writ
-0000ded0: 7465 6e20 746f 2074 656d 7020 6669 6c65  ten to temp file
-0000dee0: 2c20 7573 6520 7374 616e 6461 7264 2077  , use standard w
-0000def0: 7269 7465 2d74 6f2d 6669 6c65 0a20 2020  rite-to-file.   
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df10: 2069 6620 6764 6674 656d 705f 7061 7468   if gdftemp_path
-0000df20: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df40: 2020 7772 6974 655f 746f 5f66 696c 6528    write_to_file(
-0000df50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df60: 2020 2020 2020 2020 2020 2020 2067 6466               gdf
-0000df70: 3d67 6466 2c0a 2020 2020 2020 2020 2020  =gdf,.          
-0000df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df90: 2020 7061 7468 3d70 6174 682c 0a20 2020    path=path,.   
-0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfb0: 2020 2020 2020 2020 206c 6179 6572 3d6c           layer=l
-0000dfc0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
-0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfe0: 2020 696e 6465 783d 696e 6465 782c 0a20    index=index,. 
-0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e000: 2020 2020 2020 2020 2020 2066 6f72 6365             force
-0000e010: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-0000e020: 7479 7065 3d66 6f72 6365 5f6f 7574 7075  type=force_outpu
-0000e030: 745f 6765 6f6d 6574 7279 7479 7065 2c0a  t_geometrytype,.
-0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e050: 2020 2020 2020 2020 2020 2020 666f 7263              forc
-0000e060: 655f 6d75 6c74 6974 7970 653d 666f 7263  e_multitype=forc
-0000e070: 655f 6d75 6c74 6974 7970 652c 0a20 2020  e_multitype,.   
-0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e090: 2020 2020 2020 2020 2061 7070 656e 643d           append=
-0000e0a0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0c0: 2020 7363 6865 6d61 3d73 6368 656d 612c    schema=schema,
-0000e0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e0e0: 2020 2020 2020 2020 2020 2020 2063 7265               cre
-0000e0f0: 6174 655f 7370 6174 6961 6c5f 696e 6465  ate_spatial_inde
-0000e100: 783d 6372 6561 7465 5f73 7061 7469 616c  x=create_spatial
-0000e110: 5f69 6e64 6578 2c0a 2020 2020 2020 2020  _index,.        
-0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e130: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e140: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e160: 2020 2020 2320 4966 2067 6466 2077 7269      # If gdf wri
-0000e170: 7474 656e 2074 6f20 7465 6d70 2066 696c  tten to temp fil
-0000e180: 652c 2075 7365 2061 7070 656e 645f 746f  e, use append_to
-0000e190: 5f6e 6f6c 6f63 6b20 2b20 636c 6561 6e75  _nolock + cleanu
-0000e1a0: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-0000e1b0: 2020 2020 2020 2020 2020 5f61 7070 656e            _appen
-0000e1c0: 645f 746f 5f6e 6f6c 6f63 6b28 0a20 2020  d_to_nolock(.   
-0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1e0: 2020 2020 2020 2020 2073 7263 3d67 6466           src=gdf
-0000e1f0: 7465 6d70 5f70 6174 682c 0a20 2020 2020  temp_path,.     
-0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e210: 2020 2020 2020 2064 7374 3d70 6174 682c         dst=path,
-0000e220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e230: 2020 2020 2020 2020 2020 2020 2064 7374               dst
-0000e240: 5f6c 6179 6572 3d6c 6179 6572 2c0a 2020  _layer=layer,.  
-0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e260: 2020 2020 2020 2020 2020 666f 7263 655f            force_
-0000e270: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
-0000e280: 7970 653d 666f 7263 655f 6f75 7470 7574  ype=force_output
-0000e290: 5f67 656f 6d65 7472 7974 7970 652c 0a20  _geometrytype,. 
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-0000e2c0: 655f 7370 6174 6961 6c5f 696e 6465 783d  e_spatial_index=
-0000e2d0: 6372 6561 7465 5f73 7061 7469 616c 5f69  create_spatial_i
-0000e2e0: 6e64 6578 2c0a 2020 2020 2020 2020 2020  ndex,.          
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e310: 2020 2020 2020 2020 7265 6d6f 7665 2867          remove(g
-0000e320: 6466 7465 6d70 5f70 6174 6829 0a20 2020  dftemp_path).   
-0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e340: 2020 2020 2069 6620 6764 6674 656d 705f       if gdftemp_
-0000e350: 6c6f 636b 7061 7468 2069 7320 6e6f 7420  lockpath is not 
-0000e360: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e380: 2020 6764 6674 656d 705f 6c6f 636b 7061    gdftemp_lockpa
-0000e390: 7468 2e75 6e6c 696e 6b28 290a 2020 2020  th.unlink().    
-0000e3a0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000e3b0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000e3c0: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-0000e3d0: 2020 2020 2020 2020 2320 4966 2073 716c          # If sql
-0000e3e0: 6974 6520 6f75 7470 7574 2066 696c 6520  ite output file 
-0000e3f0: 6c6f 636b 6564 2c20 616c 736f 2072 6574  locked, also ret
-0000e400: 7279 0a20 2020 2020 2020 2020 2020 2020  ry.             
-0000e410: 2020 2020 2020 2069 6620 6765 6f66 696c         if geofil
-0000e420: 6574 7970 652e 6973 5f73 7061 7469 616c  etype.is_spatial
-0000e430: 6974 655f 6261 7365 6420 616e 6420 7374  ite_based and st
-0000e440: 7228 6578 2920 6e6f 7420 696e 205b 0a20  r(ex) not in [. 
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2020 2020 2020 2022 6461 7461 6261 7365         "database
-0000e470: 2069 7320 6c6f 636b 6564 222c 0a20 2020   is locked",.   
-0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e490: 2020 2020 2022 6174 7465 6d70 7420 746f       "attempt to
-0000e4a0: 2077 7269 7465 2061 2072 6561 646f 6e6c   write a readonl
-0000e4b0: 7920 6461 7461 6261 7365 222c 0a20 2020  y database",.   
+00008850: 735f 696e 6465 782c 0a20 2020 2029 0a0a  s_index,.    )..
+00008860: 2020 2020 2320 4e6f 2061 7373 6572 7420      # No assert 
+00008870: 746f 206b 6565 7020 6261 636b 7761 7264  to keep backward
+00008880: 7320 636f 6d70 6174 6962 696c 6974 790a  s compatibility.
+00008890: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000088a0: 745f 6764 6620 2023 2074 7970 653a 2069  t_gdf  # type: i
+000088b0: 676e 6f72 650a 0a0a 6465 6620 7265 6164  gnore...def read
+000088c0: 5f66 696c 655f 6e6f 6765 6f6d 280a 2020  _file_nogeom(.  
+000088d0: 2020 7061 7468 3a20 556e 696f 6e5b 7374    path: Union[st
+000088e0: 722c 2022 6f73 2e50 6174 684c 696b 655b  r, "os.PathLike[
+000088f0: 416e 795d 225d 2c0a 2020 2020 6c61 7965  Any]"],.    laye
+00008900: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
+00008910: 203d 204e 6f6e 652c 0a20 2020 2063 6f6c   = None,.    col
+00008920: 756d 6e73 3a20 4f70 7469 6f6e 616c 5b49  umns: Optional[I
+00008930: 7465 7261 626c 655b 7374 725d 5d20 3d20  terable[str]] = 
+00008940: 4e6f 6e65 2c0a 2020 2020 6262 6f78 3d4e  None,.    bbox=N
+00008950: 6f6e 652c 0a20 2020 2072 6f77 733d 4e6f  one,.    rows=No
+00008960: 6e65 2c0a 2020 2020 7371 6c5f 7374 6d74  ne,.    sql_stmt
+00008970: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00008980: 3d20 4e6f 6e65 2c0a 2020 2020 7371 6c5f  = None,.    sql_
+00008990: 6469 616c 6563 743a 204f 7074 696f 6e61  dialect: Optiona
+000089a0: 6c5b 4c69 7465 7261 6c5b 2253 514c 4954  l[Literal["SQLIT
+000089b0: 4522 2c20 224f 4752 5351 4c22 5d5d 203d  E", "OGRSQL"]] =
+000089c0: 204e 6f6e 652c 0a20 2020 2066 6964 5f61   None,.    fid_a
+000089d0: 735f 696e 6465 783a 2062 6f6f 6c20 3d20  s_index: bool = 
+000089e0: 4661 6c73 652c 0a29 202d 3e20 7064 2e44  False,.) -> pd.D
+000089f0: 6174 6146 7261 6d65 3a0a 2020 2020 2222  ataFrame:.    ""
+00008a00: 220a 2020 2020 4445 5052 4543 4154 4544  ".    DEPRECATED
+00008a10: 3a20 706c 6561 7365 2075 7365 2072 6561  : please use rea
+00008a20: 645f 6669 6c65 2077 6974 6820 6f70 7469  d_file with opti
+00008a30: 6f6e 2069 676e 6f72 655f 6765 6f6d 6574  on ignore_geomet
+00008a40: 7279 3d54 7275 652e 0a20 2020 2022 2222  ry=True..    """
+00008a50: 0a20 2020 2077 6172 6e69 6e67 732e 7761  .    warnings.wa
+00008a60: 726e 280a 2020 2020 2020 2020 2272 6561  rn(.        "rea
+00008a70: 645f 6669 6c65 5f6e 6f67 656f 6d20 6973  d_file_nogeom is
+00008a80: 2064 6570 7265 6361 7465 643a 2075 7365   deprecated: use
+00008a90: 2072 6561 645f 6669 6c65 2077 6974 6820   read_file with 
+00008aa0: 6967 6e6f 7265 5f67 656f 6d65 7472 793d  ignore_geometry=
+00008ab0: 5472 7565 222c 0a20 2020 2020 2020 2046  True",.        F
+00008ac0: 7574 7572 6557 6172 6e69 6e67 2c0a 2020  utureWarning,.  
+00008ad0: 2020 290a 2020 2020 7265 7375 6c74 5f67    ).    result_g
+00008ae0: 6466 203d 205f 7265 6164 5f66 696c 655f  df = _read_file_
+00008af0: 6261 7365 280a 2020 2020 2020 2020 7061  base(.        pa
+00008b00: 7468 3d70 6174 682c 0a20 2020 2020 2020  th=path,.       
+00008b10: 206c 6179 6572 3d6c 6179 6572 2c0a 2020   layer=layer,.  
+00008b20: 2020 2020 2020 636f 6c75 6d6e 733d 636f        columns=co
+00008b30: 6c75 6d6e 732c 0a20 2020 2020 2020 2062  lumns,.        b
+00008b40: 626f 783d 6262 6f78 2c0a 2020 2020 2020  box=bbox,.      
+00008b50: 2020 726f 7773 3d72 6f77 732c 0a20 2020    rows=rows,.   
+00008b60: 2020 2020 2073 716c 5f73 746d 743d 7371       sql_stmt=sq
+00008b70: 6c5f 7374 6d74 2c0a 2020 2020 2020 2020  l_stmt,.        
+00008b80: 7371 6c5f 6469 616c 6563 743d 7371 6c5f  sql_dialect=sql_
+00008b90: 6469 616c 6563 742c 0a20 2020 2020 2020  dialect,.       
+00008ba0: 2069 676e 6f72 655f 6765 6f6d 6574 7279   ignore_geometry
+00008bb0: 3d54 7275 652c 0a20 2020 2020 2020 2066  =True,.        f
+00008bc0: 6964 5f61 735f 696e 6465 783d 6669 645f  id_as_index=fid_
+00008bd0: 6173 5f69 6e64 6578 2c0a 2020 2020 290a  as_index,.    ).
+00008be0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00008bf0: 7461 6e63 6528 7265 7375 6c74 5f67 6466  tance(result_gdf
+00008c00: 2c20 7064 2e44 6174 6146 7261 6d65 290a  , pd.DataFrame).
+00008c10: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00008c20: 745f 6764 660a 0a0a 6465 6620 5f72 6561  t_gdf...def _rea
+00008c30: 645f 6669 6c65 5f62 6173 6528 0a20 2020  d_file_base(.   
+00008c40: 2070 6174 683a 2055 6e69 6f6e 5b73 7472   path: Union[str
+00008c50: 2c20 226f 732e 5061 7468 4c69 6b65 5b41  , "os.PathLike[A
+00008c60: 6e79 5d22 5d2c 0a20 2020 206c 6179 6572  ny]"],.    layer
+00008c70: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00008c80: 3d20 4e6f 6e65 2c0a 2020 2020 636f 6c75  = None,.    colu
+00008c90: 6d6e 733a 204f 7074 696f 6e61 6c5b 4974  mns: Optional[It
+00008ca0: 6572 6162 6c65 5b73 7472 5d5d 203d 204e  erable[str]] = N
+00008cb0: 6f6e 652c 0a20 2020 2062 626f 783d 4e6f  one,.    bbox=No
+00008cc0: 6e65 2c0a 2020 2020 726f 7773 3d4e 6f6e  ne,.    rows=Non
+00008cd0: 652c 0a20 2020 2073 716c 5f73 746d 743a  e,.    sql_stmt:
+00008ce0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00008cf0: 204e 6f6e 652c 0a20 2020 2073 716c 5f64   None,.    sql_d
+00008d00: 6961 6c65 6374 3a20 4f70 7469 6f6e 616c  ialect: Optional
+00008d10: 5b4c 6974 6572 616c 5b22 5351 4c49 5445  [Literal["SQLITE
+00008d20: 222c 2022 4f47 5253 514c 225d 5d20 3d20  ", "OGRSQL"]] = 
+00008d30: 4e6f 6e65 2c0a 2020 2020 6967 6e6f 7265  None,.    ignore
+00008d40: 5f67 656f 6d65 7472 793a 2062 6f6f 6c20  _geometry: bool 
+00008d50: 3d20 4661 6c73 652c 0a20 2020 2066 6964  = False,.    fid
+00008d60: 5f61 735f 696e 6465 783a 2062 6f6f 6c20  _as_index: bool 
+00008d70: 3d20 4661 6c73 652c 0a29 202d 3e20 556e  = False,.) -> Un
+00008d80: 696f 6e5b 7064 2e44 6174 6146 7261 6d65  ion[pd.DataFrame
+00008d90: 2c20 6770 642e 4765 6f44 6174 6146 7261  , gpd.GeoDataFra
+00008da0: 6d65 5d3a 0a20 2020 2022 2222 0a20 2020  me]:.    """.   
+00008db0: 2052 6561 6473 2061 2066 696c 6520 746f   Reads a file to
+00008dc0: 2061 2070 616e 6461 7320 4461 7461 6672   a pandas Datafr
+00008dd0: 616d 652e 0a20 2020 2022 2222 0a20 2020  ame..    """.   
+00008de0: 2023 2043 6865 636b 2069 6620 7468 6520   # Check if the 
+00008df0: 6669 6420 636f 6c75 6d6e 206e 6565 6473  fid column needs
+00008e00: 2074 6f20 6265 2072 6561 6420 6173 2063   to be read as c
+00008e10: 6f6c 756d 6e20 7669 6120 7468 6520 636f  olumn via the co
+00008e20: 6c75 6d6e 7320 7061 7261 6d65 7465 720a  lumns parameter.
+00008e30: 2020 2020 6669 645f 6173 5f63 6f6c 756d      fid_as_colum
+00008e40: 6e20 3d20 4661 6c73 650a 2020 2020 6966  n = False.    if
+00008e50: 2063 6f6c 756d 6e73 2069 7320 6e6f 7420   columns is not 
+00008e60: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
+00008e70: 2022 6669 6422 2069 6e20 5b63 6f6c 756d   "fid" in [colum
+00008e80: 6e2e 6c6f 7765 7228 2920 666f 7220 636f  n.lower() for co
+00008e90: 6c75 6d6e 2069 6e20 636f 6c75 6d6e 735d  lumn in columns]
+00008ea0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+00008eb0: 645f 6173 5f63 6f6c 756d 6e20 3d20 5472  d_as_column = Tr
+00008ec0: 7565 0a0a 2020 2020 2320 5265 6164 2077  ue..    # Read w
+00008ed0: 6974 6820 7468 6520 656e 6769 6e65 2073  ith the engine s
+00008ee0: 7065 6369 6669 6564 0a20 2020 2065 6e67  pecified.    eng
+00008ef0: 696e 6520 3d20 5f67 6574 5f65 6e67 696e  ine = _get_engin
+00008f00: 6528 290a 2020 2020 6966 2065 6e67 696e  e().    if engin
+00008f10: 6520 3d3d 2022 7079 6f67 7269 6f22 3a0a  e == "pyogrio":.
+00008f20: 2020 2020 2020 2020 6764 6620 3d20 5f72          gdf = _r
+00008f30: 6561 645f 6669 6c65 5f62 6173 655f 7079  ead_file_base_py
+00008f40: 6f67 7269 6f28 0a20 2020 2020 2020 2020  ogrio(.         
+00008f50: 2020 2070 6174 683d 7061 7468 2c0a 2020     path=path,.  
+00008f60: 2020 2020 2020 2020 2020 6c61 7965 723d            layer=
+00008f70: 6c61 7965 722c 0a20 2020 2020 2020 2020  layer,.         
+00008f80: 2020 2063 6f6c 756d 6e73 3d63 6f6c 756d     columns=colum
+00008f90: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00008fa0: 6262 6f78 3d62 626f 782c 0a20 2020 2020  bbox=bbox,.     
+00008fb0: 2020 2020 2020 2072 6f77 733d 726f 7773         rows=rows
+00008fc0: 2c0a 2020 2020 2020 2020 2020 2020 7371  ,.            sq
+00008fd0: 6c5f 7374 6d74 3d73 716c 5f73 746d 742c  l_stmt=sql_stmt,
+00008fe0: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
+00008ff0: 5f64 6961 6c65 6374 3d73 716c 5f64 6961  _dialect=sql_dia
+00009000: 6c65 6374 2c0a 2020 2020 2020 2020 2020  lect,.          
+00009010: 2020 6967 6e6f 7265 5f67 656f 6d65 7472    ignore_geometr
+00009020: 793d 6967 6e6f 7265 5f67 656f 6d65 7472  y=ignore_geometr
+00009030: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
+00009040: 6964 5f61 735f 696e 6465 783d 6669 645f  id_as_index=fid_
+00009050: 6173 5f69 6e64 6578 206f 7220 6669 645f  as_index or fid_
+00009060: 6173 5f63 6f6c 756d 6e2c 0a20 2020 2020  as_column,.     
+00009070: 2020 2029 0a20 2020 2065 6c69 6620 656e     ).    elif en
+00009080: 6769 6e65 203d 3d20 2266 696f 6e61 223a  gine == "fiona":
+00009090: 0a20 2020 2020 2020 2067 6466 203d 205f  .        gdf = _
+000090a0: 7265 6164 5f66 696c 655f 6261 7365 5f66  read_file_base_f
+000090b0: 696f 6e61 280a 2020 2020 2020 2020 2020  iona(.          
+000090c0: 2020 7061 7468 3d70 6174 682c 0a20 2020    path=path,.   
+000090d0: 2020 2020 2020 2020 206c 6179 6572 3d6c           layer=l
+000090e0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+000090f0: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
+00009100: 732c 0a20 2020 2020 2020 2020 2020 2062  s,.            b
+00009110: 626f 783d 6262 6f78 2c0a 2020 2020 2020  box=bbox,.      
+00009120: 2020 2020 2020 726f 7773 3d72 6f77 732c        rows=rows,
+00009130: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
+00009140: 5f73 746d 743d 7371 6c5f 7374 6d74 2c0a  _stmt=sql_stmt,.
+00009150: 2020 2020 2020 2020 2020 2020 7371 6c5f              sql_
+00009160: 6469 616c 6563 743d 7371 6c5f 6469 616c  dialect=sql_dial
+00009170: 6563 742c 0a20 2020 2020 2020 2020 2020  ect,.           
+00009180: 2069 676e 6f72 655f 6765 6f6d 6574 7279   ignore_geometry
+00009190: 3d69 676e 6f72 655f 6765 6f6d 6574 7279  =ignore_geometry
+000091a0: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+000091b0: 645f 6173 5f69 6e64 6578 3d66 6964 5f61  d_as_index=fid_a
+000091c0: 735f 696e 6465 7820 6f72 2066 6964 5f61  s_index or fid_a
+000091d0: 735f 636f 6c75 6d6e 2c0a 2020 2020 2020  s_column,.      
+000091e0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+000091f0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00009200: 6545 7272 6f72 2866 2255 6e73 7570 706f  eError(f"Unsuppo
+00009210: 7274 6564 2065 6e67 696e 653a 207b 656e  rted engine: {en
+00009220: 6769 6e65 7d22 290a 0a20 2020 2023 2043  gine}")..    # C
+00009230: 6f70 7920 7468 6520 696e 6465 7820 746f  opy the index to
+00009240: 2061 2063 6f6c 756d 6e20 6966 206e 6565   a column if nee
+00009250: 6465 642e 2e2e 0a20 2020 2069 6620 6669  ded....    if fi
+00009260: 645f 6173 5f63 6f6c 756d 6e3a 0a20 2020  d_as_column:.   
+00009270: 2020 2020 2067 6466 5b22 6669 6422 5d20       gdf["fid"] 
+00009280: 3d20 6764 662e 696e 6465 780a 2020 2020  = gdf.index.    
+00009290: 2020 2020 6966 206e 6f74 2066 6964 5f61      if not fid_a
+000092a0: 735f 696e 6465 783a 0a20 2020 2020 2020  s_index:.       
+000092b0: 2020 2020 2067 6466 203d 2067 6466 2e72       gdf = gdf.r
+000092c0: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
+000092d0: 5472 7565 290a 0a20 2020 2072 6574 7572  True)..    retur
+000092e0: 6e20 6764 660a 0a0a 6465 6620 5f72 6561  n gdf...def _rea
+000092f0: 645f 6669 6c65 5f62 6173 655f 6669 6f6e  d_file_base_fion
+00009300: 6128 0a20 2020 2070 6174 683a 2055 6e69  a(.    path: Uni
+00009310: 6f6e 5b73 7472 2c20 226f 732e 5061 7468  on[str, "os.Path
+00009320: 4c69 6b65 5b41 6e79 5d22 5d2c 0a20 2020  Like[Any]"],.   
+00009330: 206c 6179 6572 3a20 4f70 7469 6f6e 616c   layer: Optional
+00009340: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00009350: 2020 636f 6c75 6d6e 733a 204f 7074 696f    columns: Optio
+00009360: 6e61 6c5b 4974 6572 6162 6c65 5b73 7472  nal[Iterable[str
+00009370: 5d5d 203d 204e 6f6e 652c 0a20 2020 2062  ]] = None,.    b
+00009380: 626f 783d 4e6f 6e65 2c0a 2020 2020 726f  box=None,.    ro
+00009390: 7773 3d4e 6f6e 652c 0a20 2020 2073 716c  ws=None,.    sql
+000093a0: 5f73 746d 743a 204f 7074 696f 6e61 6c5b  _stmt: Optional[
+000093b0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000093c0: 2073 716c 5f64 6961 6c65 6374 3a20 4f70   sql_dialect: Op
+000093d0: 7469 6f6e 616c 5b4c 6974 6572 616c 5b22  tional[Literal["
+000093e0: 5351 4c49 5445 222c 2022 4f47 5253 514c  SQLITE", "OGRSQL
+000093f0: 225d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  "]] = None,.    
+00009400: 6967 6e6f 7265 5f67 656f 6d65 7472 793a  ignore_geometry:
+00009410: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00009420: 2020 2066 6964 5f61 735f 696e 6465 783a     fid_as_index:
+00009430: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a29   bool = False,.)
+00009440: 202d 3e20 556e 696f 6e5b 7064 2e44 6174   -> Union[pd.Dat
+00009450: 6146 7261 6d65 2c20 6770 642e 4765 6f44  aFrame, gpd.GeoD
+00009460: 6174 6146 7261 6d65 5d3a 0a20 2020 2022  ataFrame]:.    "
+00009470: 2222 0a20 2020 2052 6561 6473 2061 2066  "".    Reads a f
+00009480: 696c 6520 746f 2061 2070 616e 6461 7320  ile to a pandas 
+00009490: 4461 7461 6672 616d 6520 7573 696e 6720  Dataframe using 
+000094a0: 6669 6f6e 612e 0a20 2020 2022 2222 0a20  fiona..    """. 
+000094b0: 2020 2069 6620 6967 6e6f 7265 5f67 656f     if ignore_geo
+000094c0: 6d65 7472 7920 616e 6420 636f 6c75 6d6e  metry and column
+000094d0: 7320 3d3d 205b 5d3a 0a20 2020 2020 2020  s == []:.       
+000094e0: 2072 6574 7572 6e20 7064 2e44 6174 6146   return pd.DataF
+000094f0: 7261 6d65 2829 0a20 2020 2069 6620 7371  rame().    if sq
+00009500: 6c5f 7374 6d74 2069 7320 6e6f 7420 4e6f  l_stmt is not No
+00009510: 6e65 3a0a 2020 2020 2020 2020 7261 6973  ne:.        rais
+00009520: 6520 5661 6c75 6545 7272 6f72 2822 7371  e ValueError("sq
+00009530: 6c5f 7374 6d74 2069 7320 6e6f 7420 7375  l_stmt is not su
+00009540: 7070 6f72 7465 6420 7769 7468 2066 696f  pported with fio
+00009550: 6e61 2065 6e67 696e 6522 290a 0a20 2020  na engine")..   
+00009560: 2023 2049 6e69 740a 2020 2020 7061 7468   # Init.    path
+00009570: 203d 2050 6174 6828 7061 7468 290a 2020   = Path(path).  
+00009580: 2020 6966 2070 6174 682e 6578 6973 7473    if path.exists
+00009590: 2829 2069 7320 4661 6c73 653a 0a20 2020  () is False:.   
+000095a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000095b0: 4572 726f 7228 6622 6669 6c65 2064 6f65  Error(f"file doe
+000095c0: 736e 2774 2065 7869 7374 3a20 7b70 6174  sn't exist: {pat
+000095d0: 687d 2229 0a0a 2020 2020 2320 4966 206e  h}")..    # If n
+000095e0: 6f20 6c61 7965 7220 6e61 6d65 2073 7065  o layer name spe
+000095f0: 6369 6669 6564 2c20 6368 6563 6b20 6966  cified, check if
+00009600: 2074 6865 7265 2069 7320 6f6e 6c79 206f   there is only o
+00009610: 6e65 206c 6179 6572 2069 6e20 7468 6520  ne layer in the 
+00009620: 6669 6c65 2e0a 2020 2020 6966 206c 6179  file..    if lay
+00009630: 6572 2069 7320 4e6f 6e65 3a0a 2020 2020  er is None:.    
+00009640: 2020 2020 6c61 7965 7220 3d20 6765 745f      layer = get_
+00009650: 6f6e 6c79 5f6c 6179 6572 2870 6174 6829  only_layer(path)
+00009660: 0a0a 2020 2020 2320 5645 5259 2044 4952  ..    # VERY DIR
+00009670: 5459 2068 6163 6b20 746f 2067 6574 2074  TY hack to get t
+00009680: 6865 2066 6964 0a20 2020 2069 6620 6669  he fid.    if fi
+00009690: 645f 6173 5f69 6e64 6578 3a0a 2020 2020  d_as_index:.    
+000096a0: 2020 2020 2320 4d61 6b65 2061 2063 6f70      # Make a cop
+000096b0: 792f 636f 7079 2069 6e70 7574 2066 696c  y/copy input fil
+000096c0: 6520 746f 2067 656f 7061 636b 6167 652c  e to geopackage,
+000096d0: 2061 7320 7765 2077 696c 6c20 6164 6420   as we will add 
+000096e0: 616e 2066 6964 2f72 6f77 6420 636f 6c75  an fid/rowd colu
+000096f0: 6d6e 0a20 2020 2020 2020 2074 6d70 5f66  mn.        tmp_f
+00009700: 6964 5f70 6174 6820 3d20 5061 7468 2874  id_path = Path(t
+00009710: 656d 7066 696c 652e 6d6b 6474 656d 7028  empfile.mkdtemp(
+00009720: 2929 202f 2066 227b 7061 7468 2e73 7465  )) / f"{path.ste
+00009730: 6d7d 2e67 706b 6722 0a20 2020 2020 2020  m}.gpkg".       
+00009740: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00009750: 2020 6966 2047 656f 6669 6c65 5479 7065    if GeofileType
+00009760: 2870 6174 6829 203d 3d20 4765 6f66 696c  (path) == Geofil
+00009770: 6554 7970 652e 4750 4b47 3a0a 2020 2020  eType.GPKG:.    
+00009780: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+00009790: 2870 6174 682c 2074 6d70 5f66 6964 5f70  (path, tmp_fid_p
+000097a0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+000097b0: 2020 2020 2061 6464 5f63 6f6c 756d 6e28       add_column(
+000097c0: 746d 705f 6669 645f 7061 7468 2c20 225f  tmp_fid_path, "_
+000097d0: 5f54 4d50 5f47 454f 4649 4c45 4f50 535f  _TMP_GEOFILEOPS_
+000097e0: 4649 4422 2c20 2249 4e54 4547 4552 222c  FID", "INTEGER",
+000097f0: 2022 6669 6422 290a 2020 2020 2020 2020   "fid").        
+00009800: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009810: 2020 2020 2020 2020 2020 636f 6e76 6572            conver
+00009820: 7428 7061 7468 2c20 746d 705f 6669 645f  t(path, tmp_fid_
+00009830: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+00009840: 2020 2020 2020 2320 6669 6420 696e 2073        # fid in s
+00009850: 6861 7065 6669 6c65 2069 7320 3020 6261  hapefile is 0 ba
+00009860: 7365 642c 2073 6f20 6669 642d 310a 2020  sed, so fid-1.  
+00009870: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00009880: 645f 636f 6c75 6d6e 2874 6d70 5f66 6964  d_column(tmp_fid
+00009890: 5f70 6174 682c 2022 5f5f 544d 505f 4745  _path, "__TMP_GE
+000098a0: 4f46 494c 454f 5053 5f46 4944 222c 2022  OFILEOPS_FID", "
+000098b0: 494e 5445 4745 5222 2c20 2266 6964 2d31  INTEGER", "fid-1
+000098c0: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+000098d0: 7061 7468 203d 2074 6d70 5f66 6964 5f70  path = tmp_fid_p
+000098e0: 6174 680a 2020 2020 2020 2020 6669 6e61  ath.        fina
+000098f0: 6c6c 793a 0a20 2020 2020 2020 2020 2020  lly:.           
+00009900: 2069 6620 746d 705f 6669 645f 7061 7468   if tmp_fid_path
+00009910: 2e70 6172 656e 742e 6578 6973 7473 2829  .parent.exists()
+00009920: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009930: 2020 7368 7574 696c 2e72 6d74 7265 6528    shutil.rmtree(
+00009940: 746d 705f 6669 645f 7061 7468 2c20 6967  tmp_fid_path, ig
+00009950: 6e6f 7265 5f65 7272 6f72 733d 5472 7565  nore_errors=True
+00009960: 290a 0a20 2020 2023 2043 6865 636b 696e  )..    # Checkin
+00009970: 6720 6966 2066 6965 6c64 2f63 6f6c 756d  g if field/colum
+00009980: 6e20 6e61 6d65 7320 7368 6f75 6c64 2062  n names should b
+00009990: 6520 7265 6164 2069 7320 6361 7365 2073  e read is case s
+000099a0: 656e 7369 7469 7665 2069 6e20 6669 6f6e  ensitive in fion
+000099b0: 612c 2073 6f0a 2020 2020 2320 6d61 6b65  a, so.    # make
+000099c0: 2073 7572 6520 7468 6520 636f 6c75 6d6e   sure the column
+000099d0: 206e 616d 6573 2073 7065 6369 6669 6564   names specified
+000099e0: 2068 6176 6520 7468 6520 7361 6d65 2063   have the same c
+000099f0: 6173 696e 672e 0a20 2020 2063 6f6c 756d  asing..    colum
+00009a00: 6e73 5f70 7265 7061 7265 6420 3d20 4e6f  ns_prepared = No
+00009a10: 6e65 0a20 2020 2069 6620 636f 6c75 6d6e  ne.    if column
+00009a20: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00009a30: 2020 2020 2020 206c 6179 6572 696e 666f         layerinfo
+00009a40: 203d 2067 6574 5f6c 6179 6572 696e 666f   = get_layerinfo
+00009a50: 2870 6174 682c 206c 6179 6572 3d6c 6179  (path, layer=lay
+00009a60: 6572 290a 2020 2020 2020 2020 636f 6c75  er).        colu
+00009a70: 6d6e 735f 7570 7065 725f 6c6f 6f6b 7570  mns_upper_lookup
+00009a80: 203d 207b 636f 6c75 6d6e 2e75 7070 6572   = {column.upper
+00009a90: 2829 3a20 636f 6c75 6d6e 2066 6f72 2063  (): column for c
+00009aa0: 6f6c 756d 6e20 696e 2063 6f6c 756d 6e73  olumn in columns
+00009ab0: 7d0a 2020 2020 2020 2020 636f 6c75 6d6e  }.        column
+00009ac0: 735f 7072 6570 6172 6564 203d 207b 0a20  s_prepared = {. 
+00009ad0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+00009ae0: 6e3a 2063 6f6c 756d 6e73 5f75 7070 6572  n: columns_upper
+00009af0: 5f6c 6f6f 6b75 705b 636f 6c75 6d6e 2e75  _lookup[column.u
+00009b00: 7070 6572 2829 5d0a 2020 2020 2020 2020  pper()].        
+00009b10: 2020 2020 666f 7220 636f 6c75 6d6e 2069      for column i
+00009b20: 6e20 6c61 7965 7269 6e66 6f2e 636f 6c75  n layerinfo.colu
+00009b30: 6d6e 730a 2020 2020 2020 2020 2020 2020  mns.            
+00009b40: 6966 2063 6f6c 756d 6e2e 7570 7065 7228  if column.upper(
+00009b50: 2920 696e 2063 6f6c 756d 6e73 5f75 7070  ) in columns_upp
+00009b60: 6572 5f6c 6f6f 6b75 700a 2020 2020 2020  er_lookup.      
+00009b70: 2020 7d0a 0a20 2020 2023 2052 6561 642e    }..    # Read.
+00009b80: 2e2e 0a20 2020 2063 6f6c 756d 6e73 5f6c  ...    columns_l
+00009b90: 6973 7420 3d20 4e6f 6e65 2069 6620 636f  ist = None if co
+00009ba0: 6c75 6d6e 735f 7072 6570 6172 6564 2069  lumns_prepared i
+00009bb0: 7320 4e6f 6e65 2065 6c73 6520 6c69 7374  s None else list
+00009bc0: 2863 6f6c 756d 6e73 5f70 7265 7061 7265  (columns_prepare
+00009bd0: 6429 0a20 2020 2072 6573 756c 745f 6764  d).    result_gd
+00009be0: 6620 3d20 6770 642e 7265 6164 5f66 696c  f = gpd.read_fil
+00009bf0: 6528 0a20 2020 2020 2020 2073 7472 2870  e(.        str(p
+00009c00: 6174 6829 2c0a 2020 2020 2020 2020 6c61  ath),.        la
+00009c10: 7965 723d 6c61 7965 722c 0a20 2020 2020  yer=layer,.     
+00009c20: 2020 2062 626f 783d 6262 6f78 2c0a 2020     bbox=bbox,.  
+00009c30: 2020 2020 2020 726f 7773 3d72 6f77 732c        rows=rows,
+00009c40: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
+00009c50: 5f66 6965 6c64 733d 636f 6c75 6d6e 735f  _fields=columns_
+00009c60: 6c69 7374 2c0a 2020 2020 2020 2020 7371  list,.        sq
+00009c70: 6c3d 7371 6c5f 7374 6d74 2c0a 2020 2020  l=sql_stmt,.    
+00009c80: 2020 2020 7371 6c5f 6469 616c 6563 743d      sql_dialect=
+00009c90: 7371 6c5f 6469 616c 6563 742c 0a20 2020  sql_dialect,.   
+00009ca0: 2020 2020 2069 676e 6f72 655f 6765 6f6d       ignore_geom
+00009cb0: 6574 7279 3d69 676e 6f72 655f 6765 6f6d  etry=ignore_geom
+00009cc0: 6574 7279 2c0a 2020 2020 290a 0a20 2020  etry,.    )..   
+00009cd0: 2023 2053 6574 2074 6865 2069 6e64 6578   # Set the index
+00009ce0: 2074 6f20 7468 6520 6261 636b 6564 2d75   to the backed-u
+00009cf0: 7020 6669 640a 2020 2020 6966 2066 6964  p fid.    if fid
+00009d00: 5f61 735f 696e 6465 783a 0a20 2020 2020  _as_index:.     
+00009d10: 2020 2072 6573 756c 745f 6764 6620 3d20     result_gdf = 
+00009d20: 7265 7375 6c74 5f67 6466 2e73 6574 5f69  result_gdf.set_i
+00009d30: 6e64 6578 2822 5f5f 544d 505f 4745 4f46  ndex("__TMP_GEOF
+00009d40: 494c 454f 5053 5f46 4944 2229 0a0a 2020  ILEOPS_FID")..  
+00009d50: 2020 2320 5265 6f72 6465 7220 636f 6c75    # Reorder colu
+00009d60: 6d6e 7320 2b20 6368 616e 6765 2063 6173  mns + change cas
+00009d70: 696e 6720 736f 2074 6865 7920 6172 6520  ing so they are 
+00009d80: 7468 6520 7361 6d65 2061 7320 636f 6c75  the same as colu
+00009d90: 6d6e 7320 7061 7261 6d65 7465 720a 2020  mns parameter.  
+00009da0: 2020 6966 2063 6f6c 756d 6e73 5f70 7265    if columns_pre
+00009db0: 7061 7265 6420 6973 206e 6f74 204e 6f6e  pared is not Non
+00009dc0: 6520 616e 6420 6c65 6e28 636f 6c75 6d6e  e and len(column
+00009dd0: 735f 7072 6570 6172 6564 2920 3e20 303a  s_prepared) > 0:
+00009de0: 0a20 2020 2020 2020 2072 6573 756c 745f  .        result_
+00009df0: 6764 6620 3d20 7265 7375 6c74 5f67 6466  gdf = result_gdf
+00009e00: 5b6c 6973 7428 636f 6c75 6d6e 735f 7072  [list(columns_pr
+00009e10: 6570 6172 6564 2920 2b20 5b22 6765 6f6d  epared) + ["geom
+00009e20: 6574 7279 225d 5d0a 2020 2020 2020 2020  etry"]].        
+00009e30: 7265 7375 6c74 5f67 6466 203d 2072 6573  result_gdf = res
+00009e40: 756c 745f 6764 662e 7265 6e61 6d65 2863  ult_gdf.rename(c
+00009e50: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 5f70  olumns=columns_p
+00009e60: 7265 7061 7265 6429 2020 2320 7479 7065  repared)  # type
+00009e70: 3a20 6967 6e6f 7265 0a0a 2020 2020 2320  : ignore..    # 
+00009e80: 5374 6172 7469 6e67 2066 726f 6d20 6669  Starting from fi
+00009e90: 6f6e 6120 312e 392c 2073 7472 696e 6720  ona 1.9, string 
+00009ea0: 636f 6c75 6d6e 7320 7769 7468 2061 6c6c  columns with all
+00009eb0: 204e 6f6e 6520 7661 6c75 6573 2061 7265   None values are
+00009ec0: 2072 6561 6420 6173 2062 6569 6e67 0a20   read as being. 
+00009ed0: 2020 2023 2066 6c6f 6174 2063 6f6c 756d     # float colum
+00009ee0: 6e73 2e20 436f 6e76 6572 7420 7468 656d  ns. Convert them
+00009ef0: 2074 6f20 6f62 6a65 6374 2074 7970 652e   to object type.
+00009f00: 0a20 2020 2066 6c6f 6174 5f63 6f6c 7320  .    float_cols 
+00009f10: 3d20 6c69 7374 2872 6573 756c 745f 6764  = list(result_gd
+00009f20: 662e 7365 6c65 6374 5f64 7479 7065 7328  f.select_dtypes(
+00009f30: 5b22 666c 6f61 7436 3422 5d29 2e63 6f6c  ["float64"]).col
+00009f40: 756d 6e73 290a 2020 2020 6966 206c 656e  umns).    if len
+00009f50: 2866 6c6f 6174 5f63 6f6c 7329 203e 2030  (float_cols) > 0
+00009f60: 3a0a 2020 2020 2020 2020 2320 4368 6563  :.        # Chec
+00009f70: 6b20 666f 7220 616c 6c20 666c 6f61 7420  k for all float 
+00009f80: 636f 6c75 6d6e 7320 666f 756e 6420 6966  columns found if
+00009f90: 2074 6865 7920 7368 6f75 6c64 2062 6520   they should be 
+00009fa0: 6f62 6a65 6374 2063 6f6c 756d 6e73 2069  object columns i
+00009fb0: 6e73 7465 6164 0a20 2020 2020 2020 2077  nstead.        w
+00009fc0: 6974 6820 6669 6f6e 612e 6f70 656e 2870  ith fiona.open(p
+00009fd0: 6174 682c 206c 6179 6572 3d6c 6179 6572  ath, layer=layer
+00009fe0: 2920 6173 2063 6f6c 6c65 6374 696f 6e3a  ) as collection:
+00009ff0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+0000a000: 6572 7420 636f 6c6c 6563 7469 6f6e 2e73  ert collection.s
+0000a010: 6368 656d 6120 6973 206e 6f74 204e 6f6e  chema is not Non
+0000a020: 650a 2020 2020 2020 2020 2020 2020 7072  e.            pr
+0000a030: 6f70 6572 7469 6573 203d 2063 6f6c 6c65  operties = colle
+0000a040: 6374 696f 6e2e 7363 6865 6d61 5b22 7072  ction.schema["pr
+0000a050: 6f70 6572 7469 6573 225d 0a20 2020 2020  operties"].     
+0000a060: 2020 2020 2020 2066 6f72 2063 6f6c 2069         for col i
+0000a070: 6e20 666c 6f61 745f 636f 6c73 3a0a 2020  n float_cols:.  
+0000a080: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000a090: 2063 6f6c 2069 6e20 7072 6f70 6572 7469   col in properti
+0000a0a0: 6573 2061 6e64 2070 726f 7065 7274 6965  es and propertie
+0000a0b0: 735b 636f 6c5d 2e73 7461 7274 7377 6974  s[col].startswit
+0000a0c0: 6828 2273 7472 2229 3a0a 2020 2020 2020  h("str"):.      
+0000a0d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000a0e0: 7375 6c74 5f67 6466 5b63 6f6c 5d20 3d20  sult_gdf[col] = 
+0000a0f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a100: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000a110: 5f67 6466 5b63 6f6c 5d20 2023 2074 7970  _gdf[col]  # typ
+0000a120: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
+0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a140: 2020 2e61 7374 7970 6528 6f62 6a65 6374    .astype(object
+0000a150: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
+0000a160: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000a170: 2020 2020 2020 2020 2020 2e72 6570 6c61            .repla
+0000a180: 6365 286e 702e 6e61 6e2c 204e 6f6e 6529  ce(np.nan, None)
+0000a190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a1a0: 2020 2020 2029 0a0a 2020 2020 2320 6173       )..    # as
+0000a1b0: 7365 7274 2074 6f20 6576 6164 6520 7079  sert to evade py
+0000a1c0: 4c61 6e63 6520 7761 726e 696e 670a 2020  Lance warning.  
+0000a1d0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+0000a1e0: 6e63 6528 7265 7375 6c74 5f67 6466 2c20  nce(result_gdf, 
+0000a1f0: 7064 2e44 6174 6146 7261 6d65 2920 6f72  pd.DataFrame) or
+0000a200: 2069 7369 6e73 7461 6e63 6528 0a20 2020   isinstance(.   
+0000a210: 2020 2020 2072 6573 756c 745f 6764 662c       result_gdf,
+0000a220: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
+0000a230: 650a 2020 2020 290a 2020 2020 7265 7475  e.    ).    retu
+0000a240: 726e 2072 6573 756c 745f 6764 660a 0a0a  rn result_gdf...
+0000a250: 6465 6620 5f72 6561 645f 6669 6c65 5f62  def _read_file_b
+0000a260: 6173 655f 7079 6f67 7269 6f28 0a20 2020  ase_pyogrio(.   
+0000a270: 2070 6174 683a 2055 6e69 6f6e 5b73 7472   path: Union[str
+0000a280: 2c20 226f 732e 5061 7468 4c69 6b65 5b41  , "os.PathLike[A
+0000a290: 6e79 5d22 5d2c 0a20 2020 206c 6179 6572  ny]"],.    layer
+0000a2a0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000a2b0: 3d20 4e6f 6e65 2c0a 2020 2020 636f 6c75  = None,.    colu
+0000a2c0: 6d6e 733a 204f 7074 696f 6e61 6c5b 4974  mns: Optional[It
+0000a2d0: 6572 6162 6c65 5b73 7472 5d5d 203d 204e  erable[str]] = N
+0000a2e0: 6f6e 652c 0a20 2020 2062 626f 783d 4e6f  one,.    bbox=No
+0000a2f0: 6e65 2c0a 2020 2020 726f 7773 3d4e 6f6e  ne,.    rows=Non
+0000a300: 652c 0a20 2020 2073 716c 5f73 746d 743a  e,.    sql_stmt:
+0000a310: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000a320: 204e 6f6e 652c 0a20 2020 2073 716c 5f64   None,.    sql_d
+0000a330: 6961 6c65 6374 3a20 4f70 7469 6f6e 616c  ialect: Optional
+0000a340: 5b4c 6974 6572 616c 5b22 5351 4c49 5445  [Literal["SQLITE
+0000a350: 222c 2022 4f47 5253 514c 225d 5d20 3d20  ", "OGRSQL"]] = 
+0000a360: 4e6f 6e65 2c0a 2020 2020 6967 6e6f 7265  None,.    ignore
+0000a370: 5f67 656f 6d65 7472 793a 2062 6f6f 6c20  _geometry: bool 
+0000a380: 3d20 4661 6c73 652c 0a20 2020 2066 6964  = False,.    fid
+0000a390: 5f61 735f 696e 6465 783a 2062 6f6f 6c20  _as_index: bool 
+0000a3a0: 3d20 4661 6c73 652c 0a29 202d 3e20 556e  = False,.) -> Un
+0000a3b0: 696f 6e5b 7064 2e44 6174 6146 7261 6d65  ion[pd.DataFrame
+0000a3c0: 2c20 6770 642e 4765 6f44 6174 6146 7261  , gpd.GeoDataFra
+0000a3d0: 6d65 5d3a 0a20 2020 2022 2222 0a20 2020  me]:.    """.   
+0000a3e0: 2052 6561 6473 2061 2066 696c 6520 746f   Reads a file to
+0000a3f0: 2061 2070 616e 6461 7320 4461 7461 6672   a pandas Datafr
+0000a400: 616d 6520 7573 696e 6720 7079 6f67 7269  ame using pyogri
+0000a410: 6f2e 0a20 2020 2022 2222 0a20 2020 2023  o..    """.    #
+0000a420: 2049 6e69 740a 2020 2020 7061 7468 203d   Init.    path =
+0000a430: 2050 6174 6828 7061 7468 290a 2020 2020   Path(path).    
+0000a440: 6966 2070 6174 682e 6578 6973 7473 2829  if path.exists()
+0000a450: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
+0000a460: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000a470: 726f 7228 6622 6669 6c65 2064 6f65 736e  ror(f"file doesn
+0000a480: 2774 2065 7869 7374 3a20 7b70 6174 687d  't exist: {path}
+0000a490: 2229 0a0a 2020 2020 2320 436f 6e76 6572  ")..    # Conver
+0000a4a0: 7420 736c 6963 6520 6f62 6a65 6374 2074  t slice object t
+0000a4b0: 6f20 7079 6f67 7269 6f20 7061 7261 6d65  o pyogrio parame
+0000a4c0: 7465 7273 0a20 2020 2069 6620 726f 7773  ters.    if rows
+0000a4d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000a4e0: 2020 2020 2020 736b 6970 5f66 6561 7475        skip_featu
+0000a4f0: 7265 7320 3d20 726f 7773 2e73 7461 7274  res = rows.start
+0000a500: 0a20 2020 2020 2020 206d 6178 5f66 6561  .        max_fea
+0000a510: 7475 7265 7320 3d20 726f 7773 2e73 746f  tures = rows.sto
+0000a520: 7020 2d20 726f 7773 2e73 7461 7274 0a20  p - rows.start. 
+0000a530: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a540: 2073 6b69 705f 6665 6174 7572 6573 203d   skip_features =
+0000a550: 2030 0a20 2020 2020 2020 206d 6178 5f66   0.        max_f
+0000a560: 6561 7475 7265 7320 3d20 4e6f 6e65 0a0a  eatures = None..
+0000a570: 2020 2020 2320 4966 206e 6f20 7371 6c5f      # If no sql_
+0000a580: 7374 6d74 2073 7065 6369 6669 6564 0a20  stmt specified. 
+0000a590: 2020 2063 6f6c 756d 6e73 5f70 7265 7061     columns_prepa
+0000a5a0: 7265 6420 3d20 4e6f 6e65 0a20 2020 2069  red = None.    i
+0000a5b0: 6620 7371 6c5f 7374 6d74 2069 7320 4e6f  f sql_stmt is No
+0000a5c0: 6e65 3a0a 2020 2020 2020 2020 2320 4966  ne:.        # If
+0000a5d0: 206e 6f20 6c61 7965 7220 7370 6563 6966   no layer specif
+0000a5e0: 6965 642c 2074 6865 7265 2073 686f 756c  ied, there shoul
+0000a5f0: 6420 6265 206f 6e6c 7920 6f6e 6520 6c61  d be only one la
+0000a600: 7965 7220 696e 2074 6865 2066 696c 652e  yer in the file.
+0000a610: 0a20 2020 2020 2020 2069 6620 6c61 7965  .        if laye
+0000a620: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+0000a630: 2020 2020 2020 206c 6179 6572 203d 2067         layer = g
+0000a640: 6574 5f6f 6e6c 795f 6c61 7965 7228 7061  et_only_layer(pa
+0000a650: 7468 290a 0a20 2020 2020 2020 2023 2043  th)..        # C
+0000a660: 6865 636b 696e 6720 6966 2063 6f6c 756d  hecking if colum
+0000a670: 6e20 6e61 6d65 7320 7368 6f75 6c64 2062  n names should b
+0000a680: 6520 7265 6164 2069 7320 6361 7365 2073  e read is case s
+0000a690: 656e 7369 7469 7665 2069 6e20 7079 6f67  ensitive in pyog
+0000a6a0: 7269 6f2c 2073 6f0a 2020 2020 2020 2020  rio, so.        
+0000a6b0: 2320 6d61 6b65 2073 7572 6520 7468 6520  # make sure the 
+0000a6c0: 636f 6c75 6d6e 206e 616d 6573 2073 7065  column names spe
+0000a6d0: 6369 6669 6564 2068 6176 6520 7468 6520  cified have the 
+0000a6e0: 7361 6d65 2063 6173 696e 672e 0a20 2020  same casing..   
+0000a6f0: 2020 2020 2069 6620 636f 6c75 6d6e 7320       if columns 
+0000a700: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000a710: 2020 2020 2020 2020 206c 6179 6572 696e           layerin
+0000a720: 666f 203d 2067 6574 5f6c 6179 6572 696e  fo = get_layerin
+0000a730: 666f 2870 6174 682c 206c 6179 6572 3d6c  fo(path, layer=l
+0000a740: 6179 6572 290a 2020 2020 2020 2020 2020  ayer).          
+0000a750: 2020 636f 6c75 6d6e 735f 7570 7065 725f    columns_upper_
+0000a760: 6c6f 6f6b 7570 203d 207b 636f 6c75 6d6e  lookup = {column
+0000a770: 2e75 7070 6572 2829 3a20 636f 6c75 6d6e  .upper(): column
+0000a780: 2066 6f72 2063 6f6c 756d 6e20 696e 2063   for column in c
+0000a790: 6f6c 756d 6e73 7d0a 2020 2020 2020 2020  olumns}.        
+0000a7a0: 2020 2020 636f 6c75 6d6e 735f 7072 6570      columns_prep
+0000a7b0: 6172 6564 203d 207b 0a20 2020 2020 2020  ared = {.       
+0000a7c0: 2020 2020 2020 2020 2063 6f6c 756d 6e3a           column:
+0000a7d0: 2063 6f6c 756d 6e73 5f75 7070 6572 5f6c   columns_upper_l
+0000a7e0: 6f6f 6b75 705b 636f 6c75 6d6e 2e75 7070  ookup[column.upp
+0000a7f0: 6572 2829 5d0a 2020 2020 2020 2020 2020  er()].          
+0000a800: 2020 2020 2020 666f 7220 636f 6c75 6d6e        for column
+0000a810: 2069 6e20 6c61 7965 7269 6e66 6f2e 636f   in layerinfo.co
+0000a820: 6c75 6d6e 730a 2020 2020 2020 2020 2020  lumns.          
+0000a830: 2020 2020 2020 6966 2063 6f6c 756d 6e2e        if column.
+0000a840: 7570 7065 7228 2920 696e 2063 6f6c 756d  upper() in colum
+0000a850: 6e73 5f75 7070 6572 5f6c 6f6f 6b75 700a  ns_upper_lookup.
+0000a860: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0000a870: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a880: 2320 4669 6c6c 206f 7574 2070 6c61 6365  # Fill out place
+0000a890: 686f 6c64 6572 732c 206b 6565 7020 636f  holders, keep co
+0000a8a0: 6c75 6d6e 735f 7072 6570 6172 6564 204e  lumns_prepared N
+0000a8b0: 6f6e 6520 6265 6361 7573 6520 636f 6c75  one because colu
+0000a8c0: 6d6e 2066 696c 7465 7269 6e67 0a20 2020  mn filtering.   
+0000a8d0: 2020 2020 2023 2073 686f 756c 6420 6861       # should ha
+0000a8e0: 7070 656e 2069 6e20 7371 6c5f 7374 6d74  ppen in sql_stmt
+0000a8f0: 2e0a 2020 2020 2020 2020 7371 6c5f 7374  ..        sql_st
+0000a900: 6d74 203d 205f 6669 6c6c 5f6f 7574 5f73  mt = _fill_out_s
+0000a910: 716c 5f70 6c61 6365 686f 6c64 6572 7328  ql_placeholders(
+0000a920: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+0000a930: 683d 7061 7468 2c20 6c61 7965 723d 6c61  h=path, layer=la
+0000a940: 7965 722c 2073 716c 5f73 746d 743d 7371  yer, sql_stmt=sq
+0000a950: 6c5f 7374 6d74 2c20 636f 6c75 6d6e 733d  l_stmt, columns=
+0000a960: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
+0000a970: 290a 0a20 2020 2023 2052 6561 6421 0a20  )..    # Read!. 
+0000a980: 2020 2063 6f6c 756d 6e73 5f6c 6973 7420     columns_list 
+0000a990: 3d20 4e6f 6e65 2069 6620 636f 6c75 6d6e  = None if column
+0000a9a0: 735f 7072 6570 6172 6564 2069 7320 4e6f  s_prepared is No
+0000a9b0: 6e65 2065 6c73 6520 6c69 7374 2863 6f6c  ne else list(col
+0000a9c0: 756d 6e73 5f70 7265 7061 7265 6429 0a20  umns_prepared). 
+0000a9d0: 2020 2072 6573 756c 745f 6764 6620 3d20     result_gdf = 
+0000a9e0: 7079 6f67 7269 6f2e 7265 6164 5f64 6174  pyogrio.read_dat
+0000a9f0: 6166 7261 6d65 280a 2020 2020 2020 2020  aframe(.        
+0000aa00: 7061 7468 2c0a 2020 2020 2020 2020 6c61  path,.        la
+0000aa10: 7965 723d 6c61 7965 722c 0a20 2020 2020  yer=layer,.     
+0000aa20: 2020 2063 6f6c 756d 6e73 3d63 6f6c 756d     columns=colum
+0000aa30: 6e73 5f6c 6973 742c 0a20 2020 2020 2020  ns_list,.       
+0000aa40: 2062 626f 783d 6262 6f78 2c0a 2020 2020   bbox=bbox,.    
+0000aa50: 2020 2020 736b 6970 5f66 6561 7475 7265      skip_feature
+0000aa60: 733d 736b 6970 5f66 6561 7475 7265 732c  s=skip_features,
+0000aa70: 0a20 2020 2020 2020 206d 6178 5f66 6561  .        max_fea
+0000aa80: 7475 7265 733d 6d61 785f 6665 6174 7572  tures=max_featur
+0000aa90: 6573 2c0a 2020 2020 2020 2020 7371 6c3d  es,.        sql=
+0000aaa0: 7371 6c5f 7374 6d74 2c0a 2020 2020 2020  sql_stmt,.      
+0000aab0: 2020 7371 6c5f 6469 616c 6563 743d 7371    sql_dialect=sq
+0000aac0: 6c5f 6469 616c 6563 742c 0a20 2020 2020  l_dialect,.     
+0000aad0: 2020 2072 6561 645f 6765 6f6d 6574 7279     read_geometry
+0000aae0: 3d6e 6f74 2069 676e 6f72 655f 6765 6f6d  =not ignore_geom
+0000aaf0: 6574 7279 2c0a 2020 2020 2020 2020 6669  etry,.        fi
+0000ab00: 645f 6173 5f69 6e64 6578 3d66 6964 5f61  d_as_index=fid_a
+0000ab10: 735f 696e 6465 782c 0a20 2020 2029 0a0a  s_index,.    )..
+0000ab20: 2020 2020 2320 5265 6f72 6465 7220 636f      # Reorder co
+0000ab30: 6c75 6d6e 7320 2b20 6368 616e 6765 2063  lumns + change c
+0000ab40: 6173 696e 6720 736f 2074 6865 7920 6172  asing so they ar
+0000ab50: 6520 7468 6520 7361 6d65 2061 7320 636f  e the same as co
+0000ab60: 6c75 6d6e 7320 7061 7261 6d65 7465 720a  lumns parameter.
+0000ab70: 2020 2020 6966 2063 6f6c 756d 6e73 5f70      if columns_p
+0000ab80: 7265 7061 7265 6420 6973 206e 6f74 204e  repared is not N
+0000ab90: 6f6e 6520 616e 6420 6c65 6e28 636f 6c75  one and len(colu
+0000aba0: 6d6e 735f 7072 6570 6172 6564 2920 3e20  mns_prepared) > 
+0000abb0: 303a 0a20 2020 2020 2020 2072 6573 756c  0:.        resul
+0000abc0: 745f 6764 6620 3d20 7265 7375 6c74 5f67  t_gdf = result_g
+0000abd0: 6466 5b6c 6973 7428 636f 6c75 6d6e 735f  df[list(columns_
+0000abe0: 7072 6570 6172 6564 2920 2b20 5b22 6765  prepared) + ["ge
+0000abf0: 6f6d 6574 7279 225d 5d0a 2020 2020 2020  ometry"]].      
+0000ac00: 2020 7265 7375 6c74 5f67 6466 203d 2072    result_gdf = r
+0000ac10: 6573 756c 745f 6764 662e 7265 6e61 6d65  esult_gdf.rename
+0000ac20: 2863 6f6c 756d 6e73 3d63 6f6c 756d 6e73  (columns=columns
+0000ac30: 5f70 7265 7061 7265 6429 2020 2320 7479  _prepared)  # ty
+0000ac40: 7065 3a20 6967 6e6f 7265 0a0a 2020 2020  pe: ignore..    
+0000ac50: 2320 6173 7365 7274 2074 6f20 6576 6164  # assert to evad
+0000ac60: 6520 7079 4c61 6e63 6520 7761 726e 696e  e pyLance warnin
+0000ac70: 670a 2020 2020 6173 7365 7274 2069 7369  g.    assert isi
+0000ac80: 6e73 7461 6e63 6528 7265 7375 6c74 5f67  nstance(result_g
+0000ac90: 6466 2c20 7064 2e44 6174 6146 7261 6d65  df, pd.DataFrame
+0000aca0: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+0000acb0: 0a20 2020 2020 2020 2072 6573 756c 745f  .        result_
+0000acc0: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
+0000acd0: 4672 616d 650a 2020 2020 290a 2020 2020  Frame.    ).    
+0000ace0: 7265 7475 726e 2072 6573 756c 745f 6764  return result_gd
+0000acf0: 660a 0a0a 6465 6620 5f66 696c 6c5f 6f75  f...def _fill_ou
+0000ad00: 745f 7371 6c5f 706c 6163 6568 6f6c 6465  t_sql_placeholde
+0000ad10: 7273 280a 2020 2020 7061 7468 3a20 5061  rs(.    path: Pa
+0000ad20: 7468 2c20 6c61 7965 723a 204f 7074 696f  th, layer: Optio
+0000ad30: 6e61 6c5b 7374 725d 2c20 7371 6c5f 7374  nal[str], sql_st
+0000ad40: 6d74 3a20 7374 722c 2063 6f6c 756d 6e73  mt: str, columns
+0000ad50: 3a20 4f70 7469 6f6e 616c 5b49 7465 7261  : Optional[Itera
+0000ad60: 626c 655b 7374 725d 5d0a 2920 2d3e 2073  ble[str]].) -> s
+0000ad70: 7472 3a0a 2020 2020 2320 4669 6c6c 206f  tr:.    # Fill o
+0000ad80: 7574 2070 6c61 6365 686f 6c64 6572 7320  ut placeholders 
+0000ad90: 696e 2074 6865 2073 716c 5f73 746d 7420  in the sql_stmt 
+0000ada0: 6966 206e 6565 6465 643a 0a20 2020 2070  if needed:.    p
+0000adb0: 6c61 6365 686f 6c64 6572 7320 3d20 5b0a  laceholders = [.
+0000adc0: 2020 2020 2020 2020 6e61 6d65 2066 6f72          name for
+0000add0: 205f 2c20 6e61 6d65 2c20 5f2c 205f 2069   _, name, _, _ i
+0000ade0: 6e20 7374 7269 6e67 2e46 6f72 6d61 7474  n string.Formatt
+0000adf0: 6572 2829 2e70 6172 7365 2873 716c 5f73  er().parse(sql_s
+0000ae00: 746d 7429 2069 6620 6e61 6d65 0a20 2020  tmt) if name.   
+0000ae10: 205d 0a20 2020 206c 6179 6572 5f74 6d70   ].    layer_tmp
+0000ae20: 203d 206c 6179 6572 0a20 2020 206c 6179   = layer.    lay
+0000ae30: 6572 696e 666f 203d 204e 6f6e 650a 2020  erinfo = None.  
+0000ae40: 2020 666f 726d 6174 5f6b 7761 7267 7320    format_kwargs 
+0000ae50: 3d20 7b7d 0a20 2020 2066 6f72 2070 6c61  = {}.    for pla
+0000ae60: 6365 686f 6c64 6572 2069 6e20 706c 6163  ceholder in plac
+0000ae70: 6568 6f6c 6465 7273 3a0a 2020 2020 2020  eholders:.      
+0000ae80: 2020 6966 206c 6179 6572 5f74 6d70 2069    if layer_tmp i
+0000ae90: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000aea0: 2020 2020 6c61 7965 725f 746d 7020 3d20      layer_tmp = 
+0000aeb0: 6765 745f 6f6e 6c79 5f6c 6179 6572 2870  get_only_layer(p
+0000aec0: 6174 6829 0a20 2020 2020 2020 2069 6620  ath).        if 
+0000aed0: 706c 6163 6568 6f6c 6465 7220 3d3d 2022  placeholder == "
+0000aee0: 696e 7075 745f 6c61 7965 7222 3a0a 2020  input_layer":.  
+0000aef0: 2020 2020 2020 2020 2020 666f 726d 6174            format
+0000af00: 5f6b 7761 7267 735b 706c 6163 6568 6f6c  _kwargs[placehol
+0000af10: 6465 725d 203d 206c 6179 6572 5f74 6d70  der] = layer_tmp
+0000af20: 0a20 2020 2020 2020 2065 6c69 6620 706c  .        elif pl
+0000af30: 6163 6568 6f6c 6465 7220 3d3d 2022 6765  aceholder == "ge
+0000af40: 6f6d 6574 7279 636f 6c75 6d6e 223a 0a20  ometrycolumn":. 
+0000af50: 2020 2020 2020 2020 2020 2069 6620 6c61             if la
+0000af60: 7965 7269 6e66 6f20 6973 204e 6f6e 653a  yerinfo is None:
+0000af70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000af80: 206c 6179 6572 696e 666f 203d 2067 6574   layerinfo = get
+0000af90: 5f6c 6179 6572 696e 666f 2870 6174 682c  _layerinfo(path,
+0000afa0: 206c 6179 6572 5f74 6d70 290a 2020 2020   layer_tmp).    
+0000afb0: 2020 2020 2020 2020 666f 726d 6174 5f6b          format_k
+0000afc0: 7761 7267 735b 706c 6163 6568 6f6c 6465  wargs[placeholde
+0000afd0: 725d 203d 206c 6179 6572 696e 666f 2e67  r] = layerinfo.g
+0000afe0: 656f 6d65 7472 7963 6f6c 756d 6e0a 2020  eometrycolumn.  
+0000aff0: 2020 2020 2020 656c 6966 2070 6c61 6365        elif place
+0000b000: 686f 6c64 6572 203d 3d20 2263 6f6c 756d  holder == "colum
+0000b010: 6e73 5f74 6f5f 7365 6c65 6374 5f73 7472  ns_to_select_str
+0000b020: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
+0000b030: 6620 6c61 7965 7269 6e66 6f20 6973 204e  f layerinfo is N
+0000b040: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000b050: 2020 2020 206c 6179 6572 696e 666f 203d       layerinfo =
+0000b060: 2067 6574 5f6c 6179 6572 696e 666f 2870   get_layerinfo(p
+0000b070: 6174 682c 206c 6179 6572 5f74 6d70 290a  ath, layer_tmp).
+0000b080: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+0000b090: 6d6e 735f 6173 6b65 6420 3d20 4e6f 6e65  mns_asked = None
+0000b0a0: 2069 6620 636f 6c75 6d6e 7320 6973 204e   if columns is N
+0000b0b0: 6f6e 6520 656c 7365 206c 6973 7428 636f  one else list(co
+0000b0c0: 6c75 6d6e 7329 0a20 2020 2020 2020 2020  lumns).         
+0000b0d0: 2020 2066 6f72 6d61 7474 6572 203d 205f     formatter = _
+0000b0e0: 6f67 725f 7371 6c5f 7574 696c 2e43 6f6c  ogr_sql_util.Col
+0000b0f0: 756d 6e46 6f72 6d61 7474 6572 280a 2020  umnFormatter(.  
+0000b100: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000b110: 6c75 6d6e 735f 6173 6b65 643d 636f 6c75  lumns_asked=colu
+0000b120: 6d6e 735f 6173 6b65 642c 0a20 2020 2020  mns_asked,.     
+0000b130: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0000b140: 6e73 5f69 6e5f 6c61 7965 723d 6c61 7965  ns_in_layer=laye
+0000b150: 7269 6e66 6f2e 636f 6c75 6d6e 732c 0a20  rinfo.columns,. 
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b170: 6964 5f63 6f6c 756d 6e3d 6c61 7965 7269  id_column=layeri
+0000b180: 6e66 6f2e 6669 645f 636f 6c75 6d6e 2c0a  nfo.fid_column,.
+0000b190: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000b1a0: 2020 2020 2020 2020 2020 666f 726d 6174            format
+0000b1b0: 5f6b 7761 7267 735b 706c 6163 6568 6f6c  _kwargs[placehol
+0000b1c0: 6465 725d 203d 2066 6f72 6d61 7474 6572  der] = formatter
+0000b1d0: 2e70 7265 6669 7865 645f 616c 6961 7365  .prefixed_aliase
+0000b1e0: 6428 290a 0a20 2020 2020 2020 2065 6c73  d()..        els
+0000b1f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000b200: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000b210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b220: 2066 2275 6e6b 6e6f 776e 2070 6c61 6365   f"unknown place
+0000b230: 686f 6c64 6572 207b 706c 6163 6568 6f6c  holder {placehol
+0000b240: 6465 727d 2069 6e20 7371 6c5f 7374 6d74  der} in sql_stmt
+0000b250: 3a20 7b73 716c 5f73 746d 747d 220a 2020  : {sql_stmt}".  
+0000b260: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000b270: 2069 6620 6c65 6e28 666f 726d 6174 5f6b   if len(format_k
+0000b280: 7761 7267 7329 203e 2030 3a0a 2020 2020  wargs) > 0:.    
+0000b290: 2020 2020 7371 6c5f 7374 6d74 203d 2073      sql_stmt = s
+0000b2a0: 716c 5f73 746d 742e 666f 726d 6174 282a  ql_stmt.format(*
+0000b2b0: 2a66 6f72 6d61 745f 6b77 6172 6773 290a  *format_kwargs).
+0000b2c0: 2020 2020 7265 7475 726e 2073 716c 5f73      return sql_s
+0000b2d0: 746d 740a 0a0a 6465 6620 7265 6164 5f66  tmt...def read_f
+0000b2e0: 696c 655f 7371 6c28 0a20 2020 2070 6174  ile_sql(.    pat
+0000b2f0: 683a 2055 6e69 6f6e 5b73 7472 2c20 226f  h: Union[str, "o
+0000b300: 732e 5061 7468 4c69 6b65 5b41 6e79 5d22  s.PathLike[Any]"
+0000b310: 5d2c 0a20 2020 2073 716c 5f73 746d 743a  ],.    sql_stmt:
+0000b320: 2073 7472 2c0a 2020 2020 7371 6c5f 6469   str,.    sql_di
+0000b330: 616c 6563 743a 204f 7074 696f 6e61 6c5b  alect: Optional[
+0000b340: 4c69 7465 7261 6c5b 2253 514c 4954 4522  Literal["SQLITE"
+0000b350: 2c20 224f 4752 5351 4c22 5d5d 203d 2022  , "OGRSQL"]] = "
+0000b360: 5351 4c49 5445 222c 0a20 2020 206c 6179  SQLITE",.    lay
+0000b370: 6572 3a20 4f70 7469 6f6e 616c 5b73 7472  er: Optional[str
+0000b380: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6967  ] = None,.    ig
+0000b390: 6e6f 7265 5f67 656f 6d65 7472 793a 2062  nore_geometry: b
+0000b3a0: 6f6f 6c20 3d20 4661 6c73 652c 0a29 202d  ool = False,.) -
+0000b3b0: 3e20 556e 696f 6e5b 7064 2e44 6174 6146  > Union[pd.DataF
+0000b3c0: 7261 6d65 2c20 6770 642e 4765 6f44 6174  rame, gpd.GeoDat
+0000b3d0: 6146 7261 6d65 5d3a 0a20 2020 2022 2222  aFrame]:.    """
+0000b3e0: 0a20 2020 2044 4550 5245 4341 5445 443a  .    DEPRECATED:
+0000b3f0: 2052 6561 6473 2061 2066 696c 6520 7573   Reads a file us
+0000b400: 696e 6720 616e 2073 716c 2073 7461 7465  ing an sql state
+0000b410: 6d65 6e74 2e0a 0a20 2020 2041 7267 733a  ment...    Args:
+0000b420: 0a20 2020 2020 2020 2070 6174 6820 2866  .        path (f
+0000b430: 696c 6520 7061 7468 293a 2070 6174 6820  ile path): path 
+0000b440: 746f 2074 6865 2066 696c 6520 746f 2072  to the file to r
+0000b450: 6561 6420 6672 6f6d 0a20 2020 2020 2020  ead from.       
+0000b460: 2073 716c 5f73 746d 7420 2873 7472 293a   sql_stmt (str):
+0000b470: 2073 716c 2073 7461 7465 6d65 6e74 2074   sql statement t
+0000b480: 6f20 7573 650a 2020 2020 2020 2020 7371  o use.        sq
+0000b490: 6c5f 6469 616c 6563 7420 2873 7472 2c20  l_dialect (str, 
+0000b4a0: 6f70 7469 6f6e 616c 293a 2053 716c 2064  optional): Sql d
+0000b4b0: 6961 6c65 6374 2075 7365 642e 2044 6566  ialect used. Def
+0000b4c0: 6175 6c74 7320 746f 2027 5351 4c49 5445  aults to 'SQLITE
+0000b4d0: 272e 0a20 2020 2020 2020 206c 6179 6572  '..        layer
+0000b4e0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+0000b4f0: 3a20 5468 6520 6c61 7965 7220 746f 2072  : The layer to r
+0000b500: 6561 642e 2049 6620 6e6f 206c 6179 6572  ead. If no layer
+0000b510: 2069 7320 7370 6563 6966 6965 642c 0a20   is specified,. 
+0000b520: 2020 2020 2020 2020 2020 2072 6561 6473             reads
+0000b530: 2074 6865 206f 6e6c 7920 6c61 7965 7220   the only layer 
+0000b540: 696e 2074 6865 2066 696c 6520 6f72 2074  in the file or t
+0000b550: 6872 6f77 7320 616e 2045 7863 6570 7469  hrows an Excepti
+0000b560: 6f6e 2e0a 2020 2020 2020 2020 6967 6e6f  on..        igno
+0000b570: 7265 5f67 656f 6d65 7472 7920 2862 6f6f  re_geometry (boo
+0000b580: 6c2c 206f 7074 696f 6e61 6c29 3a20 5472  l, optional): Tr
+0000b590: 7565 206e 6f74 2074 6f20 7265 6164 2f72  ue not to read/r
+0000b5a0: 6574 7572 6e20 7468 6520 6765 6f6d 6174  eturn the geomat
+0000b5b0: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
+0000b5c0: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
+0000b5d0: 652e 0a0a 2020 2020 5265 7475 726e 733a  e...    Returns:
+0000b5e0: 0a20 2020 2020 2020 2055 6e69 6f6e 5b70  .        Union[p
+0000b5f0: 642e 4461 7461 4672 616d 652c 2067 7064  d.DataFrame, gpd
+0000b600: 2e47 656f 4461 7461 4672 616d 655d 3a20  .GeoDataFrame]: 
+0000b610: 5468 6520 6461 7461 2072 6561 642e 0a20  The data read.. 
+0000b620: 2020 2022 2222 0a20 2020 2077 6172 6e69     """.    warni
+0000b630: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
+0000b640: 2020 2772 6561 645f 6669 6c65 5f73 716c    'read_file_sql
+0000b650: 2069 7320 6465 7072 6563 6174 6564 3a20   is deprecated: 
+0000b660: 7573 6520 7265 6164 5f66 696c 6521 204d  use read_file! M
+0000b670: 696e 643a 2073 716c 5f64 6961 6c65 6374  ind: sql_dialect
+0000b680: 2069 7320 6e6f 7420 2253 514c 4954 4522   is not "SQLITE"
+0000b690: 2027 0a20 2020 2020 2020 2022 6279 2064   '.        "by d
+0000b6a0: 6566 6175 6c74 2074 6865 7265 2122 2c0a  efault there!",.
+0000b6b0: 2020 2020 2020 2020 4675 7475 7265 5761          FutureWa
+0000b6c0: 726e 696e 672c 0a20 2020 2029 0a0a 2020  rning,.    )..  
+0000b6d0: 2020 2320 5275 6e0a 2020 2020 7265 7475    # Run.    retu
+0000b6e0: 726e 205f 7265 6164 5f66 696c 655f 6261  rn _read_file_ba
+0000b6f0: 7365 280a 2020 2020 2020 2020 7061 7468  se(.        path
+0000b700: 2c0a 2020 2020 2020 2020 7371 6c5f 7374  ,.        sql_st
+0000b710: 6d74 3d73 716c 5f73 746d 742c 0a20 2020  mt=sql_stmt,.   
+0000b720: 2020 2020 2073 716c 5f64 6961 6c65 6374       sql_dialect
+0000b730: 3d73 716c 5f64 6961 6c65 6374 2c0a 2020  =sql_dialect,.  
+0000b740: 2020 2020 2020 6c61 7965 723d 6c61 7965        layer=laye
+0000b750: 722c 0a20 2020 2020 2020 2069 676e 6f72  r,.        ignor
+0000b760: 655f 6765 6f6d 6574 7279 3d69 676e 6f72  e_geometry=ignor
+0000b770: 655f 6765 6f6d 6574 7279 2c0a 2020 2020  e_geometry,.    
+0000b780: 290a 0a0a 6465 6620 746f 5f66 696c 6528  )...def to_file(
+0000b790: 0a20 2020 2067 6466 3a20 556e 696f 6e5b  .    gdf: Union[
+0000b7a0: 7064 2e44 6174 6146 7261 6d65 2c20 6770  pd.DataFrame, gp
+0000b7b0: 642e 4765 6f44 6174 6146 7261 6d65 5d2c  d.GeoDataFrame],
+0000b7c0: 0a20 2020 2070 6174 683a 2055 6e69 6f6e  .    path: Union
+0000b7d0: 5b73 7472 2c20 226f 732e 5061 7468 4c69  [str, "os.PathLi
+0000b7e0: 6b65 5b41 6e79 5d22 5d2c 0a20 2020 206c  ke[Any]"],.    l
+0000b7f0: 6179 6572 3a20 4f70 7469 6f6e 616c 5b73  ayer: Optional[s
+0000b800: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000b810: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
+0000b820: 6d65 7472 7974 7970 653a 2055 6e69 6f6e  metrytype: Union
+0000b830: 5b47 656f 6d65 7472 7954 7970 652c 2073  [GeometryType, s
+0000b840: 7472 2c20 4e6f 6e65 5d20 3d20 4e6f 6e65  tr, None] = None
+0000b850: 2c0a 2020 2020 666f 7263 655f 6d75 6c74  ,.    force_mult
+0000b860: 6974 7970 653a 2062 6f6f 6c20 3d20 4661  itype: bool = Fa
+0000b870: 6c73 652c 0a20 2020 2061 7070 656e 643a  lse,.    append:
+0000b880: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+0000b890: 2020 2061 7070 656e 645f 7469 6d65 6f75     append_timeou
+0000b8a0: 745f 733a 2069 6e74 203d 2036 3030 2c0a  t_s: int = 600,.
+0000b8b0: 2020 2020 696e 6465 783a 204f 7074 696f      index: Optio
+0000b8c0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0000b8d0: 2c0a 2020 2020 6372 6561 7465 5f73 7061  ,.    create_spa
+0000b8e0: 7469 616c 5f69 6e64 6578 3a20 4f70 7469  tial_index: Opti
+0000b8f0: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
+0000b900: 652c 0a29 3a0a 2020 2020 2222 220a 2020  e,.):.    """.  
+0000b910: 2020 5772 6974 6573 2061 2070 616e 6461    Writes a panda
+0000b920: 7320 6461 7461 6672 616d 6520 746f 2066  s dataframe to f
+0000b930: 696c 652e 0a0a 2020 2020 5468 6520 6669  ile...    The fi
+0000b940: 6c65 666f 726d 6174 2069 7320 6465 7465  leformat is dete
+0000b950: 6374 6564 2062 6173 6564 206f 6e20 7468  cted based on th
+0000b960: 6520 6669 6c65 7061 7468 2065 7874 656e  e filepath exten
+0000b970: 7369 6f6e 2e0a 0a20 2020 2054 6865 2075  sion...    The u
+0000b980: 6e64 6572 6c79 696e 6720 6c69 6272 6172  nderlying librar
+0000b990: 7920 7573 6564 2074 6f20 7772 6974 6520  y used to write 
+0000b9a0: 7468 6520 6669 6c65 2063 616e 2062 6520  the file can be 
+0000b9b0: 6368 6f6f 7365 6e20 7573 696e 6720 7468  choosen using th
+0000b9c0: 650a 2020 2020 2247 464f 5f49 4f5f 454e  e.    "GFO_IO_EN
+0000b9d0: 4749 4e45 2220 656e 7669 726f 6e6d 656e  GINE" environmen
+0000b9e0: 7420 7661 7269 6162 6c65 2e20 506f 7373  t variable. Poss
+0000b9f0: 6962 6c65 2076 616c 7565 7320 6172 6520  ible values are 
+0000ba00: 2266 696f 6e61 2220 616e 6420 2270 796f  "fiona" and "pyo
+0000ba10: 6772 696f 222e 0a20 2020 2044 6566 6175  grio"..    Defau
+0000ba20: 6c74 2065 6e67 696e 6520 6973 2022 7079  lt engine is "py
+0000ba30: 6f67 7269 6f22 2e0a 0a20 2020 2041 7267  ogrio"...    Arg
+0000ba40: 733a 0a20 2020 2020 2020 2067 6466 2028  s:.        gdf (
+0000ba50: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
+0000ba60: 293a 2054 6865 2047 656f 4461 7461 4672  ): The GeoDataFr
+0000ba70: 616d 6520 746f 2065 7870 6f72 7420 746f  ame to export to
+0000ba80: 2066 696c 652e 0a20 2020 2020 2020 2070   file..        p
+0000ba90: 6174 6820 2855 6e69 6f6e 5b73 7472 2c29  ath (Union[str,)
+0000baa0: 3a20 5468 6520 6669 6c65 2070 6174 6820  : The file path 
+0000bab0: 746f 2077 7269 7465 2074 6f2e 0a20 2020  to write to..   
+0000bac0: 2020 2020 206c 6179 6572 2028 7374 722c       layer (str,
+0000bad0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+0000bae0: 6c61 7965 7220 746f 2072 6561 642e 2049  layer to read. I
+0000baf0: 6620 6e6f 206c 6179 6572 2069 7320 7370  f no layer is sp
+0000bb00: 6563 6966 6965 642c 0a20 2020 2020 2020  ecified,.       
+0000bb10: 2020 2020 2072 6561 6473 2074 6865 206f       reads the o
+0000bb20: 6e6c 7920 6c61 7965 7220 696e 2074 6865  nly layer in the
+0000bb30: 2066 696c 6520 6f72 2074 6872 6f77 7320   file or throws 
+0000bb40: 616e 2045 7863 6570 7469 6f6e 2e0a 2020  an Exception..  
+0000bb50: 2020 2020 2020 666f 7263 655f 6f75 7470        force_outp
+0000bb60: 7574 5f67 656f 6d65 7472 7974 7970 6520  ut_geometrytype 
+0000bb70: 2855 6e69 6f6e 5b47 656f 6d65 7472 7954  (Union[GeometryT
+0000bb80: 7970 652c 2073 7472 5d2c 206f 7074 696f  ype, str], optio
+0000bb90: 6e61 6c29 3a20 4765 6f6d 6574 7279 2074  nal): Geometry t
+0000bba0: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
+0000bbb0: 746f 2028 7472 7920 746f 2920 666f 7263  to (try to) forc
+0000bbc0: 6520 7468 6520 6f75 7470 7574 2074 6f2e  e the output to.
+0000bbd0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+0000bbe0: 652e 0a20 2020 2020 2020 2020 2020 204d  e..            M
+0000bbf0: 6172 6b3a 2063 6f6d 7061 7265 6420 746f  ark: compared to
+0000bc00: 206f 7468 6572 2066 756e 6374 696f 6e73   other functions
+0000bc10: 2069 6e20 6766 6f20 7769 7468 2074 6869   in gfo with thi
+0000bc20: 7320 7061 7261 6d65 7465 722c 2074 6865  s parameter, the
+0000bc30: 2062 6568 6176 696f 7572 0a20 2020 2020   behaviour.     
+0000bc40: 2020 2020 2020 2068 6572 6520 6973 206c         here is l
+0000bc50: 696d 6974 6564 2074 6f20 7468 6520 666f  imited to the fo
+0000bc60: 6c6c 6f77 696e 673a 0a20 2020 2020 2020  llowing:.       
+0000bc70: 2020 2020 2020 2020 202d 2066 6f72 2065           - for e
+0000bc80: 6d70 7479 2069 6e70 7574 2067 6466 2773  mpty input gdf's
+0000bc90: 2c20 6120 7374 616e 6461 7264 2067 656f  , a standard geo
+0000bca0: 6d65 7472 7920 7479 7065 2028 6567 2e20  metry type (eg. 
+0000bcb0: 506f 6c79 676f 6e2c 2e2e 2e29 2063 616e  Polygon,...) can
+0000bcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bcd0: 2020 2062 6520 7573 6564 2074 6f20 666f     be used to fo
+0000bce0: 7263 6520 7468 6520 6765 6f6d 6574 7279  rce the geometry
+0000bcf0: 2063 6f6c 756d 6e20 746f 2062 6520 6f66   column to be of
+0000bd00: 2074 6861 7420 7479 7065 2e0a 2020 2020   that type..    
+0000bd10: 2020 2020 2020 2020 2020 2020 2d20 6966              - if
+0000bd20: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
+0000bd30: 6f6d 6574 7279 7479 7065 2069 7320 6120  ometrytype is a 
+0000bd40: 4d55 4c54 4920 7479 7065 2c20 7061 7261  MULTI type, para
+0000bd50: 6d65 7465 720a 2020 2020 2020 2020 2020  meter.          
+0000bd60: 2020 2020 2020 2020 666f 7263 655f 6d75          force_mu
+0000bd70: 6c74 6974 7970 6520 6265 636f 6d65 7320  ltitype becomes 
+0000bd80: 5472 7565 2e0a 2020 2020 2020 2020 666f  True..        fo
+0000bd90: 7263 655f 6d75 6c74 6974 7970 6520 2862  rce_multitype (b
+0000bda0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+0000bdb0: 666f 7263 6520 7468 6520 6765 6f6d 6574  force the geomet
+0000bdc0: 7279 2074 7970 6520 746f 2061 206d 756c  ry type to a mul
+0000bdd0: 7469 7479 7065 0a20 2020 2020 2020 2020  titype.         
+0000bde0: 2020 2066 6f72 2066 696c 6520 7479 7065     for file type
+0000bdf0: 7320 7468 6174 2072 6571 7569 7265 206f  s that require o
+0000be00: 6e65 2067 656f 6d65 7472 7974 7970 6520  ne geometrytype 
+0000be10: 7065 7220 6c61 7965 722e 0a20 2020 2020  per layer..     
+0000be20: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+0000be30: 746f 2046 616c 7365 2e0a 2020 2020 2020  to False..      
+0000be40: 2020 6170 7065 6e64 2028 626f 6f6c 2c20    append (bool, 
+0000be50: 6f70 7469 6f6e 616c 293a 2054 7275 6520  optional): True 
+0000be60: 746f 2061 7070 656e 6420 746f 2074 6865  to append to the
+0000be70: 2066 696c 652f 6c61 7965 7220 6966 2069   file/layer if i
+0000be80: 7420 6578 6973 7473 2061 6c72 6561 6479  t exists already
+0000be90: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+0000bea0: 2069 7420 646f 6573 6e27 7420 6578 6973   it doesn't exis
+0000beb0: 7420 7965 742c 2069 7420 6973 2063 7265  t yet, it is cre
+0000bec0: 6174 6564 2e20 4465 6661 756c 7473 2074  ated. Defaults t
+0000bed0: 6f20 4661 6c73 652e 0a20 2020 2020 2020  o False..       
+0000bee0: 2061 7070 656e 645f 7469 6d65 6f75 745f   append_timeout_
+0000bef0: 7320 2869 6e74 2c20 6f70 7469 6f6e 616c  s (int, optional
+0000bf00: 293a 2054 6865 206d 6178 696d 756d 2074  ): The maximum t
+0000bf10: 696d 656f 7574 2074 6f20 7761 6974 2077  imeout to wait w
+0000bf20: 6865 6e20 7468 650a 2020 2020 2020 2020  hen the.        
+0000bf30: 2020 2020 6f75 7470 7574 2066 696c 6520      output file 
+0000bf40: 6973 2061 6c72 6561 6479 2062 6569 6e67  is already being
+0000bf50: 2077 7269 7474 656e 2074 6f20 6279 2061   written to by a
+0000bf60: 6e6f 7468 6572 2070 726f 6365 7373 2e0a  nother process..
+0000bf70: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+0000bf80: 756c 7473 2074 6f20 3630 302e 0a20 2020  ults to 600..   
+0000bf90: 2020 2020 2069 6e64 6578 2028 626f 6f6c       index (bool
+0000bfa0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+0000bfb0: 5472 7565 2c20 7772 6974 6520 696e 6465  True, write inde
+0000bfc0: 7820 696e 746f 206f 6e65 206f 7220 6d6f  x into one or mo
+0000bfd0: 7265 2063 6f6c 756d 6e73 2028 666f 720a  re columns (for.
+0000bfe0: 2020 2020 2020 2020 2020 2020 4d75 6c74              Mult
+0000bff0: 6949 6e64 6578 292e 204e 6f6e 6520 7772  iIndex). None wr
+0000c000: 6974 6573 2074 6865 2069 6e64 6578 2069  ites the index i
+0000c010: 6e74 6f20 6f6e 6520 6f72 206d 6f72 6520  nto one or more 
+0000c020: 636f 6c75 6d6e 7320 6f6e 6c79 2069 6620  columns only if 
+0000c030: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0000c040: 696e 6465 7820 6973 206e 616d 6564 2c20  index is named, 
+0000c050: 6973 2061 204d 756c 7469 496e 6465 782c  is a MultiIndex,
+0000c060: 206f 7220 6861 7320 6120 6e6f 6e2d 696e   or has a non-in
+0000c070: 7465 6765 7220 6461 7461 2074 7970 652e  teger data type.
+0000c080: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+0000c090: 4661 6c73 652c 206e 6f20 696e 6465 7820  False, no index 
+0000c0a0: 6973 2077 7269 7474 656e 2e20 4465 6661  is written. Defa
+0000c0b0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+0000c0c0: 2020 2020 2020 6372 6561 7465 5f73 7061        create_spa
+0000c0d0: 7469 616c 5f69 6e64 6578 2028 626f 6f6c  tial_index (bool
+0000c0e0: 2c20 6f70 7469 6f6e 616c 293a 2054 7275  , optional): Tru
+0000c0f0: 6520 746f 2066 6f72 6365 2063 7265 6174  e to force creat
+0000c100: 696f 6e20 6f66 2073 7061 7469 616c 2069  ion of spatial i
+0000c110: 6e64 6578 2c0a 2020 2020 2020 2020 2020  ndex,.          
+0000c120: 2020 4661 6c73 6520 746f 2061 766f 6964    False to avoid
+0000c130: 2063 7265 6174 696f 6e2e 204e 6f6e 6520   creation. None 
+0000c140: 6c65 6164 7320 746f 2074 6865 2064 6566  leads to the def
+0000c150: 6175 6c74 2062 6568 6176 696f 7572 206f  ault behaviour o
+0000c160: 6620 6764 616c 2e0a 2020 2020 2020 2020  f gdal..        
+0000c170: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+0000c180: 5472 7565 2e0a 0a20 2020 2052 6169 7365  True...    Raise
+0000c190: 733a 0a20 2020 2020 2020 2056 616c 7565  s:.        Value
+0000c1a0: 4572 726f 723a 2061 6e20 696e 7661 6c69  Error: an invali
+0000c1b0: 6420 7061 7261 6d65 7465 7220 7661 6c75  d parameter valu
+0000c1c0: 6520 7761 7320 7061 7373 6564 2e0a 2020  e was passed..  
+0000c1d0: 2020 2020 2020 5275 6e74 696d 6545 7272        RuntimeErr
+0000c1e0: 6f72 3a20 7469 6d65 6f75 7420 7761 7320  or: timeout was 
+0000c1f0: 7265 6163 6865 6420 7768 696c 6520 7472  reached while tr
+0000c200: 7969 6e67 2074 6f20 6170 7065 6e64 2064  ying to append d
+0000c210: 6174 6120 746f 2070 6174 682e 0a20 2020  ata to path..   
+0000c220: 2022 2222 0a20 2020 2023 2043 6865 636b   """.    # Check
+0000c230: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+0000c240: 730a 2020 2020 2320 2d2d 2d2d 2d2d 2d2d  s.    # --------
+0000c250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+0000c260: 2020 2070 6174 6820 3d20 5061 7468 2870     path = Path(p
+0000c270: 6174 6829 0a0a 2020 2020 2320 4966 206e  ath)..    # If n
+0000c280: 6f20 6c61 7965 7220 6e61 6d65 2073 7065  o layer name spe
+0000c290: 6369 6669 6564 2c20 6465 7465 726d 696e  cified, determin
+0000c2a0: 6520 6f6e 650a 2020 2020 6966 206c 6179  e one.    if lay
+0000c2b0: 6572 2069 7320 4e6f 6e65 3a0a 2020 2020  er is None:.    
+0000c2c0: 2020 2020 6966 2061 7070 656e 6420 616e      if append an
+0000c2d0: 6420 7061 7468 2e65 7869 7374 7328 293a  d path.exists():
+0000c2e0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+0000c2f0: 6572 203d 2067 6574 5f6f 6e6c 795f 6c61  er = get_only_la
+0000c300: 7965 7228 7061 7468 290a 2020 2020 2020  yer(path).      
+0000c310: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000c320: 2020 2020 6c61 7965 7220 3d20 5061 7468      layer = Path
+0000c330: 2870 6174 6829 2e73 7465 6d0a 0a20 2020  (path).stem..   
+0000c340: 2023 2049 6620 666f 7263 655f 6f75 7470   # If force_outp
+0000c350: 7574 5f67 656f 6d65 7472 7974 7970 6520  ut_geometrytype 
+0000c360: 6973 2061 2073 7472 696e 672c 2063 6865  is a string, che
+0000c370: 636b 2069 6620 6974 2069 7320 6120 2273  ck if it is a "s
+0000c380: 7461 6e64 6172 6422 2067 656f 6d65 7472  tandard" geometr
+0000c390: 790a 2020 2020 2320 7479 7065 2c20 6173  y.    # type, as
+0000c3a0: 2047 4441 4c20 616c 736f 2073 7570 706f   GDAL also suppo
+0000c3b0: 7274 7320 7370 6563 6961 6c20 6765 6f6d  rts special geom
+0000c3c0: 6574 7279 2074 7970 6573 206c 696b 6520  etry types like 
+0000c3d0: 2250 524f 4d4f 5445 5f54 4f5f 4d55 4c54  "PROMOTE_TO_MULT
+0000c3e0: 4922 0a20 2020 2069 6620 6973 696e 7374  I".    if isinst
+0000c3f0: 616e 6365 2866 6f72 6365 5f6f 7574 7075  ance(force_outpu
+0000c400: 745f 6765 6f6d 6574 7279 7479 7065 2c20  t_geometrytype, 
+0000c410: 7374 7229 3a0a 2020 2020 2020 2020 666f  str):.        fo
+0000c420: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
+0000c430: 7472 7974 7970 6520 3d20 666f 7263 655f  trytype = force_
+0000c440: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
+0000c450: 7970 652e 7570 7065 7228 290a 2020 2020  ype.upper().    
+0000c460: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000c470: 2020 2020 2023 2056 6572 6966 7920 6966       # Verify if
+0000c480: 2069 7420 6973 2061 2022 7374 616e 6461   it is a "standa
+0000c490: 7264 2220 6765 6f6d 6574 7279 2074 7970  rd" geometry typ
+0000c4a0: 652c 2061 7320 4744 414c 2061 6c73 6f20  e, as GDAL also 
+0000c4b0: 7375 7070 6f72 7473 0a20 2020 2020 2020  supports.       
+0000c4c0: 2020 2020 2023 2073 7065 6369 616c 2067       # special g
+0000c4d0: 656f 6d65 7472 7920 7479 7065 7320 6c69  eometry types li
+0000c4e0: 6b65 2022 5052 4f4d 4f54 455f 544f 5f4d  ke "PROMOTE_TO_M
+0000c4f0: 554c 5449 220a 2020 2020 2020 2020 2020  ULTI".          
+0000c500: 2020 666f 7263 655f 6f75 7470 7574 5f67    force_output_g
+0000c510: 656f 6d65 7472 7974 7970 6520 3d20 4765  eometrytype = Ge
+0000c520: 6f6d 6574 7279 5479 7065 5b66 6f72 6365  ometryType[force
+0000c530: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+0000c540: 7479 7065 5d0a 2020 2020 2020 2020 6578  type].        ex
+0000c550: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
+0000c560: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000c570: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+0000c580: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000c590: 556e 7375 7070 6f72 7465 6420 666f 7263  Unsupported forc
+0000c5a0: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
+0000c5b0: 7974 7970 653a 207b 666f 7263 655f 6f75  ytype: {force_ou
+0000c5c0: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
+0000c5d0: 657d 220a 2020 2020 2020 2020 2020 2020  e}".            
+0000c5e0: 290a 2020 2020 6966 2066 6f72 6365 5f6f  ).    if force_o
+0000c5f0: 7574 7075 745f 6765 6f6d 6574 7279 7479  utput_geometryty
+0000c600: 7065 2069 7320 6e6f 7420 4e6f 6e65 2061  pe is not None a
+0000c610: 6e64 2066 6f72 6365 5f6f 7574 7075 745f  nd force_output_
+0000c620: 6765 6f6d 6574 7279 7479 7065 2e69 735f  geometrytype.is_
+0000c630: 6d75 6c74 6974 7970 653a 0a20 2020 2020  multitype:.     
+0000c640: 2020 2066 6f72 6365 5f6d 756c 7469 7479     force_multity
+0000c650: 7065 203d 2054 7275 650a 0a20 2020 2023  pe = True..    #
+0000c660: 2049 6620 7468 6572 6520 6973 206e 6f20   If there is no 
+0000c670: 6765 6f6d 6574 7279 2063 6f6c 756d 6e20  geometry column 
+0000c680: 696e 2074 6865 2069 6e70 7574 2c20 616c  in the input, al
+0000c690: 7761 7973 2075 7365 2066 696f 6e61 2c20  ways use fiona, 
+0000c6a0: 6173 2070 796f 6772 696f 2064 6f65 736e  as pyogrio doesn
+0000c6b0: 2774 0a20 2020 2023 2073 7570 706f 7274  't.    # support
+0000c6c0: 2074 6861 7420 7965 7420 6174 2074 696d   that yet at tim
+0000c6d0: 6520 6f66 2077 7269 7469 6e67 2e0a 2020  e of writing..  
+0000c6e0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000c6f0: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
+0000c700: 4672 616d 6529 2069 7320 4661 6c73 6520  Frame) is False 
+0000c710: 6f72 2028 0a20 2020 2020 2020 2069 7369  or (.        isi
+0000c720: 6e73 7461 6e63 6528 6764 662c 2067 7064  nstance(gdf, gpd
+0000c730: 2e47 656f 4461 7461 4672 616d 6529 2061  .GeoDataFrame) a
+0000c740: 6e64 2022 6765 6f6d 6574 7279 2220 6e6f  nd "geometry" no
+0000c750: 7420 696e 2067 6466 2e63 6f6c 756d 6e73  t in gdf.columns
+0000c760: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000c770: 656e 6769 6e65 203d 2022 6669 6f6e 6122  engine = "fiona"
+0000c780: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0000c790: 2020 2065 6e67 696e 6520 3d20 5f67 6574     engine = _get
+0000c7a0: 5f65 6e67 696e 6528 290a 0a20 2020 2023  _engine()..    #
+0000c7b0: 204e 6f77 2077 7269 7465 2077 6974 6820   Now write with 
+0000c7c0: 7468 6520 636f 7272 6563 7420 656e 6769  the correct engi
+0000c7d0: 6e65 0a20 2020 2069 6620 656e 6769 6e65  ne.    if engine
+0000c7e0: 203d 3d20 2270 796f 6772 696f 223a 0a20   == "pyogrio":. 
+0000c7f0: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
+0000c800: 696e 7374 616e 6365 2867 6466 2c20 6770  instance(gdf, gp
+0000c810: 642e 4765 6f44 6174 6146 7261 6d65 290a  d.GeoDataFrame).
+0000c820: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000c830: 746f 5f66 696c 655f 7079 6f67 7269 6f28  to_file_pyogrio(
+0000c840: 0a20 2020 2020 2020 2020 2020 2067 6466  .            gdf
+0000c850: 3d67 6466 2c0a 2020 2020 2020 2020 2020  =gdf,.          
+0000c860: 2020 7061 7468 3d70 6174 682c 0a20 2020    path=path,.   
+0000c870: 2020 2020 2020 2020 206c 6179 6572 3d6c           layer=l
+0000c880: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+0000c890: 2020 666f 7263 655f 6f75 7470 7574 5f67    force_output_g
+0000c8a0: 656f 6d65 7472 7974 7970 653d 666f 7263  eometrytype=forc
+0000c8b0: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
+0000c8c0: 7974 7970 652c 0a20 2020 2020 2020 2020  ytype,.         
+0000c8d0: 2020 2066 6f72 6365 5f6d 756c 7469 7479     force_multity
+0000c8e0: 7065 3d66 6f72 6365 5f6d 756c 7469 7479  pe=force_multity
+0000c8f0: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+0000c900: 6170 7065 6e64 3d61 7070 656e 642c 0a20  append=append,. 
+0000c910: 2020 2020 2020 2020 2020 2061 7070 656e             appen
+0000c920: 645f 7469 6d65 6f75 745f 733d 6170 7065  d_timeout_s=appe
+0000c930: 6e64 5f74 696d 656f 7574 5f73 2c0a 2020  nd_timeout_s,.  
+0000c940: 2020 2020 2020 2020 2020 696e 6465 783d            index=
+0000c950: 696e 6465 782c 0a20 2020 2020 2020 2020  index,.         
+0000c960: 2020 2063 7265 6174 655f 7370 6174 6961     create_spatia
+0000c970: 6c5f 696e 6465 783d 6372 6561 7465 5f73  l_index=create_s
+0000c980: 7061 7469 616c 5f69 6e64 6578 2c0a 2020  patial_index,.  
+0000c990: 2020 2020 2020 290a 2020 2020 656c 6966        ).    elif
+0000c9a0: 2065 6e67 696e 6520 3d3d 2022 6669 6f6e   engine == "fion
+0000c9b0: 6122 3a0a 2020 2020 2020 2020 7265 7475  a":.        retu
+0000c9c0: 726e 205f 746f 5f66 696c 655f 6669 6f6e  rn _to_file_fion
+0000c9d0: 6128 0a20 2020 2020 2020 2020 2020 2067  a(.            g
+0000c9e0: 6466 3d67 6466 2c0a 2020 2020 2020 2020  df=gdf,.        
+0000c9f0: 2020 2020 7061 7468 3d70 6174 682c 0a20      path=path,. 
+0000ca00: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+0000ca10: 3d6c 6179 6572 2c0a 2020 2020 2020 2020  =layer,.        
+0000ca20: 2020 2020 666f 7263 655f 6f75 7470 7574      force_output
+0000ca30: 5f67 656f 6d65 7472 7974 7970 653d 666f  _geometrytype=fo
+0000ca40: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
+0000ca50: 7472 7974 7970 652c 0a20 2020 2020 2020  trytype,.       
+0000ca60: 2020 2020 2066 6f72 6365 5f6d 756c 7469       force_multi
+0000ca70: 7479 7065 3d66 6f72 6365 5f6d 756c 7469  type=force_multi
+0000ca80: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
+0000ca90: 2020 6170 7065 6e64 3d61 7070 656e 642c    append=append,
+0000caa0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+0000cab0: 656e 645f 7469 6d65 6f75 745f 733d 6170  end_timeout_s=ap
+0000cac0: 7065 6e64 5f74 696d 656f 7574 5f73 2c0a  pend_timeout_s,.
+0000cad0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0000cae0: 783d 696e 6465 782c 0a20 2020 2020 2020  x=index,.       
+0000caf0: 2020 2020 2063 7265 6174 655f 7370 6174       create_spat
+0000cb00: 6961 6c5f 696e 6465 783d 6372 6561 7465  ial_index=create
+0000cb10: 5f73 7061 7469 616c 5f69 6e64 6578 2c0a  _spatial_index,.
+0000cb20: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
+0000cb30: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
+0000cb40: 6520 5661 6c75 6545 7272 6f72 2866 2255  e ValueError(f"U
+0000cb50: 6e73 7570 706f 7274 6564 2065 6e67 696e  nsupported engin
+0000cb60: 653a 207b 656e 6769 6e65 7d22 290a 0a0a  e: {engine}")...
+0000cb70: 6465 6620 5f67 6574 5f65 6e67 696e 6528  def _get_engine(
+0000cb80: 293a 0a20 2020 2072 6574 7572 6e20 6f73  ):.    return os
+0000cb90: 2e65 6e76 6972 6f6e 2e67 6574 2822 4746  .environ.get("GF
+0000cba0: 4f5f 494f 5f45 4e47 494e 4522 2c20 2270  O_IO_ENGINE", "p
+0000cbb0: 796f 6772 696f 2229 0a0a 0a64 6566 205f  yogrio")...def _
+0000cbc0: 746f 5f66 696c 655f 6669 6f6e 6128 0a20  to_file_fiona(. 
+0000cbd0: 2020 2067 6466 3a20 556e 696f 6e5b 7064     gdf: Union[pd
+0000cbe0: 2e44 6174 6146 7261 6d65 2c20 6770 642e  .DataFrame, gpd.
+0000cbf0: 4765 6f44 6174 6146 7261 6d65 5d2c 0a20  GeoDataFrame],. 
+0000cc00: 2020 2070 6174 683a 2050 6174 682c 0a20     path: Path,. 
+0000cc10: 2020 206c 6179 6572 3a20 7374 722c 0a20     layer: str,. 
+0000cc20: 2020 2066 6f72 6365 5f6f 7574 7075 745f     force_output_
+0000cc30: 6765 6f6d 6574 7279 7479 7065 3a20 556e  geometrytype: Un
+0000cc40: 696f 6e5b 4765 6f6d 6574 7279 5479 7065  ion[GeometryType
+0000cc50: 2c20 7374 722c 204e 6f6e 655d 203d 204e  , str, None] = N
+0000cc60: 6f6e 652c 0a20 2020 2066 6f72 6365 5f6d  one,.    force_m
+0000cc70: 756c 7469 7479 7065 3a20 626f 6f6c 203d  ultitype: bool =
+0000cc80: 2046 616c 7365 2c0a 2020 2020 6170 7065   False,.    appe
+0000cc90: 6e64 3a20 626f 6f6c 203d 2046 616c 7365  nd: bool = False
+0000cca0: 2c0a 2020 2020 6170 7065 6e64 5f74 696d  ,.    append_tim
+0000ccb0: 656f 7574 5f73 3a20 696e 7420 3d20 3630  eout_s: int = 60
+0000ccc0: 302c 0a20 2020 2069 6e64 6578 3a20 4f70  0,.    index: Op
+0000ccd0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0000cce0: 6f6e 652c 0a20 2020 2063 7265 6174 655f  one,.    create_
+0000ccf0: 7370 6174 6961 6c5f 696e 6465 783a 204f  spatial_index: O
+0000cd00: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0000cd10: 5472 7565 2c0a 293a 0a20 2020 2022 2222  True,.):.    """
+0000cd20: 0a20 2020 2057 7269 7465 7320 6120 7061  .    Writes a pa
+0000cd30: 6e64 6173 2064 6174 6166 7261 6d65 2074  ndas dataframe t
+0000cd40: 6f20 6669 6c65 2075 7369 6e67 2066 696f  o file using fio
+0000cd50: 6e61 2e0a 2020 2020 2222 220a 2020 2020  na..    """.    
+0000cd60: 2320 4861 6e64 6c65 2073 6f6d 6520 7370  # Handle some sp
+0000cd70: 6563 6966 6963 2063 6173 6573 2077 6865  ecific cases whe
+0000cd80: 7265 2074 6865 2066 696c 6520 7363 6865  re the file sche
+0000cd90: 6d61 206e 6565 6473 2074 6f20 6265 206d  ma needs to be m
+0000cda0: 616e 6970 756c 6174 6564 2e0a 2020 2020  anipulated..    
+0000cdb0: 7363 6865 6d61 203d 204e 6f6e 650a 2020  schema = None.  
+0000cdc0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000cdd0: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
+0000cde0: 4672 616d 6529 2069 7320 4661 6c73 6520  Frame) is False 
+0000cdf0: 6f72 2028 0a20 2020 2020 2020 2069 7369  or (.        isi
+0000ce00: 6e73 7461 6e63 6528 6764 662c 2067 7064  nstance(gdf, gpd
+0000ce10: 2e47 656f 4461 7461 4672 616d 6529 2061  .GeoDataFrame) a
+0000ce20: 6e64 2022 6765 6f6d 6574 7279 2220 6e6f  nd "geometry" no
+0000ce30: 7420 696e 2067 6466 2e63 6f6c 756d 6e73  t in gdf.columns
+0000ce40: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000ce50: 2320 4e6f 2067 656f 6d65 7472 792c 2073  # No geometry, s
+0000ce60: 6f20 7072 6570 6172 6520 746f 2062 6520  o prepare to be 
+0000ce70: 7772 6974 7465 6e20 6173 2061 7474 7269  written as attri
+0000ce80: 6275 7465 2074 6162 6c65 3a20 6164 6420  bute table: add 
+0000ce90: 6765 6f6d 6574 7279 2063 6f6c 756d 6e0a  geometry column.
+0000cea0: 2020 2020 2020 2020 2320 7769 7468 204e          # with N
+0000ceb0: 6f6e 6520 6765 6f6d 6574 7279 2074 7970  one geometry typ
+0000cec0: 6520 696e 2073 6368 656d 610a 2020 2020  e in schema.    
+0000ced0: 2020 2020 6764 6620 3d20 6770 642e 4765      gdf = gpd.Ge
+0000cee0: 6f44 6174 6146 7261 6d65 2867 6466 2c20  oDataFrame(gdf, 
+0000cef0: 6765 6f6d 6574 7279 3d5b 4e6f 6e65 2066  geometry=[None f
+0000cf00: 6f72 2069 2069 6e20 6764 662e 696e 6465  or i in gdf.inde
+0000cf10: 785d 2920 2023 2074 7970 653a 2069 676e  x])  # type: ign
+0000cf20: 6f72 650a 2020 2020 2020 2020 7363 6865  ore.        sche
+0000cf30: 6d61 203d 2067 7064 5f69 6f5f 6669 6c65  ma = gpd_io_file
+0000cf40: 2e69 6e66 6572 5f73 6368 656d 6128 6764  .infer_schema(gd
+0000cf50: 6629 0a20 2020 2020 2020 2073 6368 656d  f).        schem
+0000cf60: 615b 2267 656f 6d65 7472 7922 5d20 3d20  a["geometry"] = 
+0000cf70: 224e 6f6e 6522 0a20 2020 2065 6c69 6620  "None".    elif 
+0000cf80: 280a 2020 2020 2020 2020 6c65 6e28 6764  (.        len(gd
+0000cf90: 6629 203d 3d20 300a 2020 2020 2020 2020  f) == 0.        
+0000cfa0: 616e 6420 666f 7263 655f 6f75 7470 7574  and force_output
+0000cfb0: 5f67 656f 6d65 7472 7974 7970 6520 6973  _geometrytype is
+0000cfc0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+0000cfd0: 2020 616e 6420 6973 696e 7374 616e 6365    and isinstance
+0000cfe0: 2866 6f72 6365 5f6f 7574 7075 745f 6765  (force_output_ge
+0000cff0: 6f6d 6574 7279 7479 7065 2c20 4765 6f6d  ometrytype, Geom
+0000d000: 6574 7279 5479 7065 290a 2020 2020 293a  etryType).    ):
+0000d010: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
+0000d020: 6520 6764 6620 6973 2065 6d70 7479 2062  e gdf is empty b
+0000d030: 7574 2061 2067 656f 6d65 7472 7920 7479  ut a geometry ty
+0000d040: 7065 2069 7320 7370 6563 6966 6965 642c  pe is specified,
+0000d050: 2075 7365 2074 6865 2073 7065 6369 6669   use the specifi
+0000d060: 6564 2074 7970 650a 2020 2020 2020 2020  ed type.        
+0000d070: 7363 6865 6d61 203d 2067 7064 5f69 6f5f  schema = gpd_io_
+0000d080: 6669 6c65 2e69 6e66 6572 5f73 6368 656d  file.infer_schem
+0000d090: 6128 6764 6629 0a20 2020 2020 2020 2023  a(gdf).        #
+0000d0a0: 2047 656f 6d65 7472 7920 7479 7065 206d   Geometry type m
+0000d0b0: 7573 7420 6265 2069 6e20 6361 6d65 6c63  ust be in camelc
+0000d0c0: 6173 6520 666f 7220 6669 6f6e 610a 2020  ase for fiona.  
+0000d0d0: 2020 2020 2020 7363 6865 6d61 5b22 6765        schema["ge
+0000d0e0: 6f6d 6574 7279 225d 203d 2066 6f72 6365  ometry"] = force
+0000d0f0: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+0000d100: 7479 7065 2e6e 616d 655f 6361 6d65 6c63  type.name_camelc
+0000d110: 6173 650a 2020 2020 6173 7365 7274 2069  ase.    assert i
+0000d120: 7369 6e73 7461 6e63 6528 6764 662c 2067  sinstance(gdf, g
+0000d130: 7064 2e47 656f 4461 7461 4672 616d 6529  pd.GeoDataFrame)
+0000d140: 0a0a 2020 2020 2320 436f 6e76 6572 7420  ..    # Convert 
+0000d150: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
+0000d160: 6d65 7472 7974 7970 6520 746f 2073 7472  metrytype to str
+0000d170: 696e 6720 746f 2073 696d 706c 6966 7920  ing to simplify 
+0000d180: 636f 6465 2061 6674 6572 7761 7264 730a  code afterwards.
+0000d190: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000d1a0: 6528 666f 7263 655f 6f75 7470 7574 5f67  e(force_output_g
+0000d1b0: 656f 6d65 7472 7974 7970 652c 2047 656f  eometrytype, Geo
+0000d1c0: 6d65 7472 7954 7970 6529 3a0a 2020 2020  metryType):.    
+0000d1d0: 2020 2020 666f 7263 655f 6f75 7470 7574      force_output
+0000d1e0: 5f67 656f 6d65 7472 7974 7970 6520 3d20  _geometrytype = 
+0000d1f0: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
+0000d200: 6d65 7472 7974 7970 652e 6e61 6d65 0a0a  metrytype.name..
+0000d210: 2020 2020 2320 4e6f 2074 6865 2066 696c      # No the fil
+0000d220: 6520 6361 6e20 6163 7475 616c 6c79 2062  e can actually b
+0000d230: 6520 7772 6974 7465 6e0a 2020 2020 2320  e written.    # 
+0000d240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d260: 2d2d 2d0a 2020 2020 2320 4669 6f6e 6120  ---.    # Fiona 
+0000d270: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+0000d280: 7468 6520 6f75 7470 7574 2067 656f 6d65  the output geome
+0000d290: 7472 7974 7970 6520 7061 7261 6d65 7465  trytype paramete
+0000d2a0: 7220 6173 2075 7365 6420 696e 2067 6461  r as used in gda
+0000d2b0: 6c2c 2073 6f20 6173 2061 0a20 2020 2023  l, so as a.    #
+0000d2c0: 206c 6967 6874 7765 6967 6874 2069 6d70   lightweight imp
+0000d2d0: 6c65 6d65 6e74 6174 696f 6e20 6a75 7374  lementation just
+0000d2e0: 2073 6574 2066 6f72 6365 0a20 2020 2064   set force.    d
+0000d2f0: 6566 2077 7269 7465 5f74 6f5f 6669 6c65  ef write_to_file
+0000d300: 280a 2020 2020 2020 2020 6764 663a 2067  (.        gdf: g
+0000d310: 7064 2e47 656f 4461 7461 4672 616d 652c  pd.GeoDataFrame,
+0000d320: 0a20 2020 2020 2020 2070 6174 683a 2050  .        path: P
+0000d330: 6174 682c 0a20 2020 2020 2020 206c 6179  ath,.        lay
+0000d340: 6572 3a20 7374 722c 0a20 2020 2020 2020  er: str,.       
+0000d350: 2069 6e64 6578 3a20 4f70 7469 6f6e 616c   index: Optional
+0000d360: 5b62 6f6f 6c5d 203d 204e 6f6e 652c 0a20  [bool] = None,. 
+0000d370: 2020 2020 2020 2066 6f72 6365 5f6f 7574         force_out
+0000d380: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
+0000d390: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000d3a0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000d3b0: 666f 7263 655f 6d75 6c74 6974 7970 653a  force_multitype:
+0000d3c0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+0000d3d0: 2020 2020 2020 2061 7070 656e 643a 2062         append: b
+0000d3e0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000d3f0: 2020 2020 2073 6368 656d 613a 204f 7074       schema: Opt
+0000d400: 696f 6e61 6c5b 6469 6374 5d20 3d20 4e6f  ional[dict] = No
+0000d410: 6e65 2c0a 2020 2020 2020 2020 6372 6561  ne,.        crea
+0000d420: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
+0000d430: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+0000d440: 203d 2054 7275 652c 0a20 2020 2029 3a0a   = True,.    ):.
+0000d450: 2020 2020 2020 2020 2320 5072 6570 6172          # Prepar
+0000d460: 6520 6172 6773 2066 6f72 2074 6f5f 6669  e args for to_fi
+0000d470: 6c65 0a20 2020 2020 2020 2069 6620 6170  le.        if ap
+0000d480: 7065 6e64 2069 7320 5472 7565 3a0a 2020  pend is True:.  
+0000d490: 2020 2020 2020 2020 2020 6966 2070 6174            if pat
+0000d4a0: 682e 6578 6973 7473 2829 3a0a 2020 2020  h.exists():.    
+0000d4b0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0000d4c0: 203d 2022 6122 0a20 2020 2020 2020 2020   = "a".         
+0000d4d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000d4e0: 2020 2020 2020 2020 206d 6f64 6520 3d20           mode = 
+0000d4f0: 2277 220a 2020 2020 2020 2020 656c 7365  "w".        else
+0000d500: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+0000d510: 6465 203d 2022 7722 0a0a 2020 2020 2020  de = "w"..      
+0000d520: 2020 6b77 6172 6773 203d 207b 7d0a 2020    kwargs = {}.  
+0000d530: 2020 2020 2020 6b77 6172 6773 5b22 656e        kwargs["en
+0000d540: 6769 6e65 225d 203d 2022 6669 6f6e 6122  gine"] = "fiona"
+0000d550: 0a20 2020 2020 2020 206b 7761 7267 735b  .        kwargs[
+0000d560: 226d 6f64 6522 5d20 3d20 6d6f 6465 0a20  "mode"] = mode. 
+0000d570: 2020 2020 2020 2067 656f 6669 6c65 7479         geofilety
+0000d580: 7065 203d 2047 656f 6669 6c65 5479 7065  pe = GeofileType
+0000d590: 2870 6174 6829 0a20 2020 2020 2020 206b  (path).        k
+0000d5a0: 7761 7267 735b 2264 7269 7665 7222 5d20  wargs["driver"] 
+0000d5b0: 3d20 6765 6f66 696c 6574 7970 652e 6f67  = geofiletype.og
+0000d5c0: 7264 7269 7665 720a 2020 2020 2020 2020  rdriver.        
+0000d5d0: 6b77 6172 6773 5b22 696e 6465 7822 5d20  kwargs["index"] 
+0000d5e0: 3d20 696e 6465 780a 2020 2020 2020 2020  = index.        
+0000d5f0: 6966 2063 7265 6174 655f 7370 6174 6961  if create_spatia
+0000d600: 6c5f 696e 6465 7820 6973 206e 6f74 204e  l_index is not N
+0000d610: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d620: 206b 7761 7267 735b 2253 5041 5449 414c   kwargs["SPATIAL
+0000d630: 5f49 4e44 4558 225d 203d 2063 7265 6174  _INDEX"] = creat
+0000d640: 655f 7370 6174 6961 6c5f 696e 6465 780a  e_spatial_index.
+0000d650: 2020 2020 2020 2020 6966 2066 6f72 6365          if force
+0000d660: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+0000d670: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+0000d680: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+0000d690: 6172 6773 5b22 6765 6f6d 6574 7279 7479  args["geometryty
+0000d6a0: 7065 225d 203d 2066 6f72 6365 5f6f 7574  pe"] = force_out
+0000d6b0: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
+0000d6c0: 0a20 2020 2020 2020 2069 6620 7363 6865  .        if sche
+0000d6d0: 6d61 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ma is not None:.
+0000d6e0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+0000d6f0: 6773 5b22 7363 6865 6d61 225d 203d 2073  gs["schema"] = s
+0000d700: 6368 656d 610a 0a20 2020 2020 2020 2023  chema..        #
+0000d710: 204e 6f77 2077 6520 6361 6e20 7772 6974   Now we can writ
+0000d720: 650a 2020 2020 2020 2020 6966 2067 656f  e.        if geo
+0000d730: 6669 6c65 7479 7065 203d 3d20 4765 6f66  filetype == Geof
+0000d740: 696c 6554 7970 652e 4553 5249 5368 6170  ileType.ESRIShap
+0000d750: 6566 696c 653a 0a20 2020 2020 2020 2020  efile:.         
+0000d760: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
+0000d770: 2020 2069 6620 696e 6465 7820 6973 2054     if index is T
+0000d780: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
+0000d790: 2020 2020 2067 6466 5f74 6f5f 7772 6974       gdf_to_writ
+0000d7a0: 6520 3d20 6764 662e 7265 7365 745f 696e  e = gdf.reset_in
+0000d7b0: 6465 7828 6472 6f70 3d54 7275 6529 0a20  dex(drop=True). 
+0000d7c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000d7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d7e0: 2067 6466 5f74 6f5f 7772 6974 6520 3d20   gdf_to_write = 
+0000d7f0: 6764 660a 2020 2020 2020 2020 2020 2020  gdf.            
+0000d800: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
+0000d810: 6764 665f 746f 5f77 7269 7465 203d 2067  gdf_to_write = g
+0000d820: 6466 0a20 2020 2020 2020 2020 2020 2067  df.            g
+0000d830: 6466 5f74 6f5f 7772 6974 652e 746f 5f66  df_to_write.to_f
+0000d840: 696c 6528 7374 7228 7061 7468 292c 202a  ile(str(path), *
+0000d850: 2a6b 7761 7267 7329 2020 2320 7479 7065  *kwargs)  # type
+0000d860: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+0000d870: 2065 6c69 6620 6765 6f66 696c 6574 7970   elif geofiletyp
+0000d880: 6520 3d3d 2047 656f 6669 6c65 5479 7065  e == GeofileType
+0000d890: 2e47 504b 473a 0a20 2020 2020 2020 2020  .GPKG:.         
+0000d8a0: 2020 2023 2054 7279 2074 6f20 6861 726d     # Try to harm
+0000d8b0: 6f6e 697a 6520 7468 6520 6765 6f6d 6574  onize the geomet
+0000d8c0: 7279 7479 7065 2074 6f20 6f6e 6520 286d  rytype to one (m
+0000d8d0: 756c 7469 2974 7970 652c 2061 7320 4750  ulti)type, as GP
+0000d8e0: 4b47 0a20 2020 2020 2020 2020 2020 2023  KG.            #
+0000d8f0: 2064 6f65 736e 2774 206c 696b 6520 3e20   doesn't like > 
+0000d900: 3120 7479 7065 2069 6e20 6120 6c61 7965  1 type in a laye
+0000d910: 720a 2020 2020 2020 2020 2020 2020 6966  r.            if
+0000d920: 2073 6368 656d 6120 6973 204e 6f6e 6520   schema is None 
+0000d930: 6f72 2028 6c65 6e28 6764 6629 203e 2030  or (len(gdf) > 0
+0000d940: 2061 6e64 2073 6368 656d 615b 2267 656f   and schema["geo
+0000d950: 6d65 7472 7922 5d20 213d 2022 4e6f 6e65  metry"] != "None
+0000d960: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0000d970: 2020 2020 6764 665f 746f 5f77 7269 7465      gdf_to_write
+0000d980: 203d 2067 6466 2e63 6f70 7928 290a 2020   = gdf.copy().  
+0000d990: 2020 2020 2020 2020 2020 2020 2020 6764                gd
+0000d9a0: 665f 746f 5f77 7269 7465 2e67 656f 6d65  f_to_write.geome
+0000d9b0: 7472 7920 3d20 6765 6f73 6572 6965 735f  try = geoseries_
+0000d9c0: 7574 696c 2e68 6172 6d6f 6e69 7a65 5f67  util.harmonize_g
+0000d9d0: 656f 6d65 7472 7974 7970 6573 280a 2020  eometrytypes(.  
+0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9f0: 2020 6764 662e 6765 6f6d 6574 7279 2c20    gdf.geometry, 
+0000da00: 666f 7263 655f 6d75 6c74 6974 7970 653d  force_multitype=
+0000da10: 666f 7263 655f 6d75 6c74 6974 7970 650a  force_multitype.
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000da40: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+0000da50: 6e63 6528 6764 665f 746f 5f77 7269 7465  nce(gdf_to_write
+0000da60: 2c20 6770 642e 4765 6f44 6174 6146 7261  , gpd.GeoDataFra
+0000da70: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+0000da80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000da90: 2020 2020 2020 6764 665f 746f 5f77 7269        gdf_to_wri
+0000daa0: 7465 203d 2067 6466 0a20 2020 2020 2020  te = gdf.       
+0000dab0: 2020 2020 2067 6466 5f74 6f5f 7772 6974       gdf_to_writ
+0000dac0: 652e 746f 5f66 696c 6528 7374 7228 7061  e.to_file(str(pa
+0000dad0: 7468 292c 206c 6179 6572 3d6c 6179 6572  th), layer=layer
+0000dae0: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+0000daf0: 2020 2020 656c 6966 2067 656f 6669 6c65      elif geofile
+0000db00: 7479 7065 203d 3d20 4765 6f66 696c 6554  type == GeofileT
+0000db10: 7970 652e 5351 4c69 7465 3a0a 2020 2020  ype.SQLite:.    
+0000db20: 2020 2020 2020 2020 6764 662e 746f 5f66          gdf.to_f
+0000db30: 696c 6528 7374 7228 7061 7468 292c 206c  ile(str(path), l
+0000db40: 6179 6572 3d6c 6179 6572 2c20 2a2a 6b77  ayer=layer, **kw
+0000db50: 6172 6773 290a 2020 2020 2020 2020 656c  args).        el
+0000db60: 6966 2067 656f 6669 6c65 7479 7065 203d  if geofiletype =
+0000db70: 3d20 4765 6f66 696c 6554 7970 652e 4765  = GeofileType.Ge
+0000db80: 6f4a 534f 4e3a 0a20 2020 2020 2020 2020  oJSON:.         
+0000db90: 2020 2067 6466 2e74 6f5f 6669 6c65 2873     gdf.to_file(s
+0000dba0: 7472 2870 6174 6829 2c20 2a2a 6b77 6172  tr(path), **kwar
+0000dbb0: 6773 290a 2020 2020 2020 2020 656c 7365  gs).        else
+0000dbc0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000dbd0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+0000dbe0: 224e 6f74 2069 6d70 6c65 6d65 6e74 6564  "Not implemented
+0000dbf0: 2066 6f72 2067 656f 6669 6c65 7479 7065   for geofiletype
+0000dc00: 207b 6765 6f66 696c 6574 7970 657d 2229   {geofiletype}")
+0000dc10: 0a0a 2020 2020 2320 4966 206e 6f20 6170  ..    # If no ap
+0000dc20: 7065 6e64 2c20 6a75 7374 2077 7269 7465  pend, just write
+0000dc30: 2074 6f20 6f75 7470 7574 2070 6174 680a   to output path.
+0000dc40: 2020 2020 6966 206e 6f74 2061 7070 656e      if not appen
+0000dc50: 643a 0a20 2020 2020 2020 2077 7269 7465  d:.        write
+0000dc60: 5f74 6f5f 6669 6c65 280a 2020 2020 2020  _to_file(.      
+0000dc70: 2020 2020 2020 6764 663d 6764 662c 0a20        gdf=gdf,. 
+0000dc80: 2020 2020 2020 2020 2020 2070 6174 683d             path=
+0000dc90: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000dca0: 2020 6c61 7965 723d 6c61 7965 722c 0a20    layer=layer,. 
+0000dcb0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+0000dcc0: 3d69 6e64 6578 2c0a 2020 2020 2020 2020  =index,.        
+0000dcd0: 2020 2020 666f 7263 655f 6f75 7470 7574      force_output
+0000dce0: 5f67 656f 6d65 7472 7974 7970 653d 666f  _geometrytype=fo
+0000dcf0: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
+0000dd00: 7472 7974 7970 652c 0a20 2020 2020 2020  trytype,.       
+0000dd10: 2020 2020 2066 6f72 6365 5f6d 756c 7469       force_multi
+0000dd20: 7479 7065 3d66 6f72 6365 5f6d 756c 7469  type=force_multi
+0000dd30: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
+0000dd40: 2020 6170 7065 6e64 3d61 7070 656e 642c    append=append,
+0000dd50: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
+0000dd60: 656d 613d 7363 6865 6d61 2c0a 2020 2020  ema=schema,.    
+0000dd70: 2020 2020 2020 2020 6372 6561 7465 5f73          create_s
+0000dd80: 7061 7469 616c 5f69 6e64 6578 3d63 7265  patial_index=cre
+0000dd90: 6174 655f 7370 6174 6961 6c5f 696e 6465  ate_spatial_inde
+0000dda0: 782c 0a20 2020 2020 2020 2029 0a20 2020  x,.        ).   
+0000ddb0: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
+0000ddc0: 2041 7070 656e 6420 6973 2061 736b 6564   Append is asked
+0000ddd0: 2c20 6368 6563 6b20 6966 2074 6865 2066  , check if the f
+0000dde0: 696f 6e61 2064 7269 7665 7220 7375 7070  iona driver supp
+0000ddf0: 6f72 7473 2061 7070 656e 6469 6e67 2e20  orts appending. 
+0000de00: 4966 0a20 2020 2020 2020 2023 206e 6f74  If.        # not
+0000de10: 2c20 7772 6974 6520 746f 2074 656d 706f  , write to tempo
+0000de20: 7261 7279 206f 7574 7075 7420 6669 6c65  rary output file
+0000de30: 0a0a 2020 2020 2020 2020 2320 5265 6d61  ..        # Rema
+0000de40: 726b 3a20 6669 6f6e 6120 7072 652d 312e  rk: fiona pre-1.
+0000de50: 382e 3134 2064 6964 6e27 7420 7375 7070  8.14 didn't supp
+0000de60: 6f72 7420 6170 7065 6e64 696e 6720 746f  ort appending to
+0000de70: 2067 656f 7061 636b 6167 652e 204f 6e63   geopackage. Onc
+0000de80: 650a 2020 2020 2020 2020 2320 6f6c 6465  e.        # olde
+0000de90: 7220 7665 7273 696f 6e73 2062 6563 6f6d  r versions becom
+0000dea0: 6573 2072 6172 652c 2064 6570 656e 6465  es rare, depende
+0000deb0: 6e63 7920 6361 6e20 6265 2070 7574 2074  ncy can be put t
+0000dec0: 6f20 7468 6973 2076 6572 7369 6f6e 2c20  o this version, 
+0000ded0: 616e 640a 2020 2020 2020 2020 2320 7468  and.        # th
+0000dee0: 6973 2063 6f64 6520 6361 6e20 6265 2063  is code can be c
+0000def0: 6c65 616e 6564 2075 702e 2e2e 0a20 2020  leaned up....   
+0000df00: 2020 2020 2067 656f 6669 6c65 7479 7065       geofiletype
+0000df10: 203d 2047 656f 6669 6c65 5479 7065 2870   = GeofileType(p
+0000df20: 6174 6829 0a20 2020 2020 2020 2067 6466  ath).        gdf
+0000df30: 7465 6d70 5f70 6174 6820 3d20 4e6f 6e65  temp_path = None
+0000df40: 0a20 2020 2020 2020 2067 6466 7465 6d70  .        gdftemp
+0000df50: 5f6c 6f63 6b70 6174 6820 3d20 4e6f 6e65  _lockpath = None
+0000df60: 0a20 2020 2020 2020 2069 6620 2261 2220  .        if "a" 
+0000df70: 6e6f 7420 696e 2066 696f 6e61 2e73 7570  not in fiona.sup
+0000df80: 706f 7274 6564 5f64 7269 7665 7273 5b67  ported_drivers[g
+0000df90: 656f 6669 6c65 7479 7065 2e6f 6772 6472  eofiletype.ogrdr
+0000dfa0: 6976 6572 5d3a 0a20 2020 2020 2020 2020  iver]:.         
+0000dfb0: 2020 2023 2047 6574 2061 2075 6e69 7175     # Get a uniqu
+0000dfc0: 6520 7465 6d70 2066 696c 6520 7061 7468  e temp file path
+0000dfd0: 2e20 5468 6520 6669 6c65 2063 616e 6e6f  . The file canno
+0000dfe0: 7420 6265 2063 7265 6174 6564 2079 6574  t be created yet
+0000dff0: 2c20 736f 0a20 2020 2020 2020 2020 2020  , so.           
+0000e000: 2023 206f 6e6c 7920 6372 6561 7465 2061   # only create a
+0000e010: 206c 6f63 6b20 6669 6c65 2074 6f20 6576   lock file to ev
+0000e020: 6164 6520 6f74 6865 7220 7072 6f63 6573  ade other proces
+0000e030: 7365 7320 7573 696e 6720 7468 6520 7361  ses using the sa
+0000e040: 6d65 0a20 2020 2020 2020 2020 2020 2023  me.            #
+0000e050: 2074 656d 7020 6669 6c65 206e 616d 650a   temp file name.
+0000e060: 2020 2020 2020 2020 2020 2020 6764 6674              gdft
+0000e070: 656d 705f 7061 7468 2c20 6764 6674 656d  emp_path, gdftem
+0000e080: 705f 6c6f 636b 7061 7468 203d 205f 696f  p_lockpath = _io
+0000e090: 5f75 7469 6c2e 6765 745f 7465 6d70 6669  _util.get_tempfi
+0000e0a0: 6c65 5f6c 6f63 6b65 6428 0a20 2020 2020  le_locked(.     
+0000e0b0: 2020 2020 2020 2020 2020 2062 6173 655f             base_
+0000e0c0: 6669 6c65 6e61 6d65 3d22 6764 6674 656d  filename="gdftem
+0000e0d0: 7022 2c20 7375 6666 6978 3d70 6174 682e  p", suffix=path.
+0000e0e0: 7375 6666 6978 2c20 6469 726e 616d 653d  suffix, dirname=
+0000e0f0: 2267 656f 6669 6c65 5f74 6f5f 6669 6c65  "geofile_to_file
+0000e100: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0000e110: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+0000e120: 655f 746f 5f66 696c 6528 0a20 2020 2020  e_to_file(.     
+0000e130: 2020 2020 2020 2020 2020 2067 6466 2c0a             gdf,.
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e150: 7061 7468 3d67 6466 7465 6d70 5f70 6174  path=gdftemp_pat
+0000e160: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+0000e170: 2020 206c 6179 6572 3d6c 6179 6572 2c0a     layer=layer,.
+0000e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e190: 696e 6465 783d 696e 6465 782c 0a20 2020  index=index,.   
+0000e1a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000e1b0: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
+0000e1c0: 7279 7479 7065 3d66 6f72 6365 5f6f 7574  rytype=force_out
+0000e1d0: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
+0000e1e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e1f0: 2020 666f 7263 655f 6d75 6c74 6974 7970    force_multityp
+0000e200: 653d 666f 7263 655f 6d75 6c74 6974 7970  e=force_multityp
+0000e210: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000e220: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
+0000e230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e240: 2020 6372 6561 7465 5f73 7061 7469 616c    create_spatial
+0000e250: 5f69 6e64 6578 3d63 7265 6174 655f 7370  _index=create_sp
+0000e260: 6174 6961 6c5f 696e 6465 782c 0a20 2020  atial_index,.   
+0000e270: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000e280: 2020 2020 2320 4669 6c65 7320 646f 6e27      # Files don'
+0000e290: 7420 7479 7069 6361 6c6c 7920 7375 7070  t typically supp
+0000e2a0: 6f72 7420 6861 7669 6e67 206d 756c 7469  ort having multi
+0000e2b0: 706c 6520 7072 6f63 6573 7365 7320 7772  ple processes wr
+0000e2c0: 6974 696e 670a 2020 2020 2020 2020 2320  iting.        # 
+0000e2d0: 7369 6d75 6c74 616e 6f75 736c 7920 746f  simultanously to
+0000e2e0: 2074 6865 6d2c 2073 6f20 7573 6520 6c6f   them, so use lo
+0000e2f0: 636b 2066 696c 6520 746f 2073 796e 6368  ck file to synch
+0000e300: 726f 6e69 7a65 2061 6363 6573 732e 0a20  ronize access.. 
+0000e310: 2020 2020 2020 206c 6f63 6b66 696c 6520         lockfile 
+0000e320: 3d20 5061 7468 2866 227b 7374 7228 7061  = Path(f"{str(pa
+0000e330: 7468 297d 2e6c 6f63 6b22 290a 2020 2020  th)}.lock").    
+0000e340: 2020 2020 7374 6172 745f 7469 6d65 203d      start_time =
+0000e350: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+0000e360: 6d65 2e6e 6f77 2829 0a20 2020 2020 2020  me.now().       
+0000e370: 2072 6561 6479 203d 2046 616c 7365 0a20   ready = False. 
+0000e380: 2020 2020 2020 2077 6869 6c65 206e 6f74         while not
+0000e390: 2072 6561 6479 3a0a 2020 2020 2020 2020   ready:.        
+0000e3a0: 2020 2020 6966 205f 696f 5f75 7469 6c2e      if _io_util.
+0000e3b0: 6372 6561 7465 5f66 696c 655f 6174 6f6d  create_file_atom
+0000e3c0: 6963 286c 6f63 6b66 696c 6529 2069 7320  ic(lockfile) is 
+0000e3d0: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
+0000e3e0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000e400: 2049 6620 6764 6620 7761 736e 2774 2077   If gdf wasn't w
+0000e410: 7269 7474 656e 2074 6f20 7465 6d70 2066  ritten to temp f
+0000e420: 696c 652c 2075 7365 2073 7461 6e64 6172  ile, use standar
+0000e430: 6420 7772 6974 652d 746f 2d66 696c 650a  d write-to-file.
+0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e450: 2020 2020 6966 2067 6466 7465 6d70 5f70      if gdftemp_p
+0000e460: 6174 6820 6973 204e 6f6e 653a 0a20 2020  ath is None:.   
+0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e480: 2020 2020 2077 7269 7465 5f74 6f5f 6669       write_to_fi
+0000e490: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4b0: 6764 663d 6764 662c 0a20 2020 2020 2020  gdf=gdf,.       
 0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 205d 3a0a 2020 2020 2020 2020 2020 2020   ]:.            
-0000e4e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000e4f0: 6520 6578 0a20 2020 2020 2020 2020 2020  e ex.           
-0000e500: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
+0000e4d0: 2020 2020 2070 6174 683d 7061 7468 2c0a       path=path,.
+0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4f0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+0000e500: 723d 6c61 7965 722c 0a20 2020 2020 2020  r=layer,.       
 0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2020 7265 6164 7920 3d20 5472 7565 0a20    ready = True. 
-0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e540: 2020 206c 6f63 6b66 696c 652e 756e 6c69     lockfile.unli
-0000e550: 6e6b 2829 0a20 2020 2020 2020 2020 2020  nk().           
-0000e560: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e570: 2020 2020 2020 2074 696d 655f 7761 6974         time_wait
-0000e580: 696e 6720 3d20 2864 6174 6574 696d 652e  ing = (datetime.
-0000e590: 6461 7465 7469 6d65 2e6e 6f77 2829 202d  datetime.now() -
-0000e5a0: 2073 7461 7274 5f74 696d 6529 2e74 6f74   start_time).tot
-0000e5b0: 616c 5f73 6563 6f6e 6473 2829 0a20 2020  al_seconds().   
-0000e5c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e5d0: 7469 6d65 5f77 6169 7469 6e67 203e 2061  time_waiting > a
-0000e5e0: 7070 656e 645f 7469 6d65 6f75 745f 733a  ppend_timeout_s:
-0000e5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e600: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
-0000e610: 6d65 4572 726f 7228 0a20 2020 2020 2020  meError(.       
+0000e520: 2020 2020 2069 6e64 6578 3d69 6e64 6578       index=index
+0000e530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e540: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000e550: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
+0000e560: 7472 7974 7970 653d 666f 7263 655f 6f75  trytype=force_ou
+0000e570: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
+0000e580: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e5a0: 6f72 6365 5f6d 756c 7469 7479 7065 3d66  orce_multitype=f
+0000e5b0: 6f72 6365 5f6d 756c 7469 7479 7065 2c0a  orce_multitype,.
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2020 2020 2020 2020 2020 2020 6170 7065              appe
+0000e5e0: 6e64 3d54 7275 652c 0a20 2020 2020 2020  nd=True,.       
+0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e600: 2020 2020 2073 6368 656d 613d 7363 6865       schema=sche
+0000e610: 6d61 2c0a 2020 2020 2020 2020 2020 2020  ma,.            
 0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2066 2274 6f5f 6669 6c65 2074 696d 656f   f"to_file timeo
-0000e640: 7574 206f 6620 7b61 7070 656e 645f 7469  ut of {append_ti
-0000e650: 6d65 6f75 745f 737d 2072 6561 6368 6564  meout_s} reached
-0000e660: 2c20 7374 6f70 2061 7070 656e 6420 220a  , stop append ".
-0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e680: 2020 2020 2020 2020 6622 746f 207b 7061          f"to {pa
-0000e690: 7468 7d21 220a 2020 2020 2020 2020 2020  th}!".          
-0000e6a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000e6b0: 2020 2020 2020 2020 2023 2053 6c65 6570           # Sleep
-0000e6c0: 2066 6f72 2061 2073 6563 6f6e 6420 6265   for a second be
-0000e6d0: 666f 7265 2074 7279 696e 6720 6167 6169  fore trying agai
-0000e6e0: 6e0a 2020 2020 2020 2020 2020 2020 7469  n.            ti
-0000e6f0: 6d65 2e73 6c65 6570 2831 290a 0a0a 6465  me.sleep(1)...de
-0000e700: 6620 5f74 6f5f 6669 6c65 5f70 796f 6772  f _to_file_pyogr
-0000e710: 696f 280a 2020 2020 6764 663a 2055 6e69  io(.    gdf: Uni
-0000e720: 6f6e 5b70 642e 4461 7461 4672 616d 652c  on[pd.DataFrame,
-0000e730: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-0000e740: 655d 2c0a 2020 2020 7061 7468 3a20 5061  e],.    path: Pa
-0000e750: 7468 2c0a 2020 2020 6c61 7965 723a 2073  th,.    layer: s
-0000e760: 7472 2c0a 2020 2020 666f 7263 655f 6f75  tr,.    force_ou
-0000e770: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-0000e780: 653a 2055 6e69 6f6e 5b47 656f 6d65 7472  e: Union[Geometr
-0000e790: 7954 7970 652c 2073 7472 2c20 4e6f 6e65  yType, str, None
-0000e7a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 666f  ] = None,.    fo
-0000e7b0: 7263 655f 6d75 6c74 6974 7970 653a 2062  rce_multitype: b
-0000e7c0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000e7d0: 2061 7070 656e 643a 2062 6f6f 6c20 3d20   append: bool = 
-0000e7e0: 4661 6c73 652c 0a20 2020 2061 7070 656e  False,.    appen
-0000e7f0: 645f 7469 6d65 6f75 745f 733a 2069 6e74  d_timeout_s: int
-0000e800: 203d 2036 3030 2c0a 2020 2020 696e 6465   = 600,.    inde
-0000e810: 783a 2062 6f6f 6c20 3d20 5472 7565 2c0a  x: bool = True,.
-0000e820: 2020 2020 6372 6561 7465 5f73 7061 7469      create_spati
-0000e830: 616c 5f69 6e64 6578 3a20 4f70 7469 6f6e  al_index: Option
-0000e840: 616c 5b62 6f6f 6c5d 203d 2054 7275 652c  al[bool] = True,
-0000e850: 0a29 3a0a 2020 2020 2222 220a 2020 2020  .):.    """.    
-0000e860: 5772 6974 6573 2061 2070 616e 6461 7320  Writes a pandas 
-0000e870: 6461 7461 6672 616d 6520 746f 2066 696c  dataframe to fil
-0000e880: 6520 7573 696e 6720 7079 6f67 7269 6f2e  e using pyogrio.
-0000e890: 0a20 2020 2022 2222 0a20 2020 2023 2050  .    """.    # P
-0000e8a0: 7265 7061 7265 2061 7267 7320 666f 7220  repare args for 
-0000e8b0: 7772 6974 655f 6461 7461 6672 616d 650a  write_dataframe.
-0000e8c0: 2020 2020 6b77 6172 6773 203d 207b 7d0a      kwargs = {}.
-0000e8d0: 0a20 2020 2069 6620 6170 7065 6e64 2069  .    if append i
-0000e8e0: 7320 5472 7565 2061 6e64 2070 6174 682e  s True and path.
-0000e8f0: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-0000e900: 2020 6b77 6172 6773 5b22 6170 7065 6e64    kwargs["append
-0000e910: 225d 203d 2054 7275 650a 2020 2020 2020  "] = True.      
-0000e920: 2020 6c61 7965 7269 6e66 6f20 3d20 6765    layerinfo = ge
-0000e930: 745f 6c61 7965 7269 6e66 6f28 7061 7468  t_layerinfo(path
-0000e940: 2c20 6c61 7965 7229 0a20 2020 2020 2020  , layer).       
-0000e950: 2066 696c 655f 636f 6c73 203d 205b 636f   file_cols = [co
-0000e960: 6c2e 7570 7065 7228 2920 666f 7220 636f  l.upper() for co
-0000e970: 6c20 696e 206c 6179 6572 696e 666f 2e63  l in layerinfo.c
-0000e980: 6f6c 756d 6e73 5d0a 2020 2020 2020 2020  olumns].        
-0000e990: 6764 665f 636f 6c73 203d 205b 636f 6c2e  gdf_cols = [col.
-0000e9a0: 7570 7065 7228 2920 666f 7220 636f 6c20  upper() for col 
-0000e9b0: 696e 2067 6466 2e63 6f6c 756d 6e73 2069  in gdf.columns i
-0000e9c0: 6620 636f 6c20 213d 2067 6466 2e67 656f  f col != gdf.geo
-0000e9d0: 6d65 7472 792e 6e61 6d65 5d0a 2020 2020  metry.name].    
-0000e9e0: 2020 2020 6966 2067 6466 5f63 6f6c 7320      if gdf_cols 
-0000e9f0: 213d 2066 696c 655f 636f 6c73 3a0a 2020  != file_cols:.  
-0000ea00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000ea10: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-0000ea20: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-0000ea30: 7469 6e61 7469 6f6e 206c 6179 6572 2064  tination layer d
-0000ea40: 6f65 736e 2774 2068 6176 6520 7468 6520  oesn't have the 
-0000ea50: 7361 6d65 2063 6f6c 756d 6e73 2061 7320  same columns as 
-0000ea60: 6764 663a 2022 0a20 2020 2020 2020 2020  gdf: ".         
-0000ea70: 2020 2020 2020 2066 227b 6669 6c65 5f63         f"{file_c
-0000ea80: 6f6c 737d 2076 7320 7b67 6466 5f63 6f6c  ols} vs {gdf_col
-0000ea90: 737d 220a 2020 2020 2020 2020 2020 2020  s}".            
-0000eaa0: 290a 0a20 2020 2069 6620 6372 6561 7465  )..    if create
-0000eab0: 5f73 7061 7469 616c 5f69 6e64 6578 2069  _spatial_index i
-0000eac0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000ead0: 2020 2020 6b77 6172 6773 5b22 5350 4154      kwargs["SPAT
-0000eae0: 4941 4c5f 494e 4445 5822 5d20 3d20 6372  IAL_INDEX"] = cr
-0000eaf0: 6561 7465 5f73 7061 7469 616c 5f69 6e64  eate_spatial_ind
-0000eb00: 6578 0a20 2020 2067 656f 6669 6c65 7479  ex.    geofilety
-0000eb10: 7065 203d 2047 656f 6669 6c65 5479 7065  pe = GeofileType
-0000eb20: 2870 6174 6829 0a20 2020 206b 7761 7267  (path).    kwarg
-0000eb30: 735b 2264 7269 7665 7222 5d20 3d20 6765  s["driver"] = ge
-0000eb40: 6f66 696c 6574 7970 652e 6f67 7264 7269  ofiletype.ogrdri
-0000eb50: 7665 720a 2020 2020 6966 2063 7265 6174  ver.    if creat
-0000eb60: 655f 7370 6174 6961 6c5f 696e 6465 7820  e_spatial_index 
-0000eb70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000eb80: 2020 2020 206b 7761 7267 735b 2253 5041       kwargs["SPA
-0000eb90: 5449 414c 5f49 4e44 4558 225d 203d 2063  TIAL_INDEX"] = c
-0000eba0: 7265 6174 655f 7370 6174 6961 6c5f 696e  reate_spatial_in
-0000ebb0: 6465 780a 2020 2020 6966 2066 6f72 6365  dex.    if force
-0000ebc0: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-0000ebd0: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-0000ebe0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-0000ebf0: 6e73 7461 6e63 6528 666f 7263 655f 6f75  nstance(force_ou
-0000ec00: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-0000ec10: 652c 2047 656f 6d65 7472 7954 7970 6529  e, GeometryType)
-0000ec20: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0000ec30: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
-0000ec40: 7472 7974 7970 6520 3d20 666f 7263 655f  trytype = force_
-0000ec50: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
-0000ec60: 7970 652e 6e61 6d65 5f63 616d 656c 6361  ype.name_camelca
-0000ec70: 7365 0a20 2020 2020 2020 206b 7761 7267  se.        kwarg
-0000ec80: 735b 2267 656f 6d65 7472 795f 7479 7065  s["geometry_type
-0000ec90: 225d 203d 2066 6f72 6365 5f6f 7574 7075  "] = force_outpu
-0000eca0: 745f 6765 6f6d 6574 7279 7479 7065 0a20  t_geometrytype. 
-0000ecb0: 2020 2069 6620 666f 7263 655f 6d75 6c74     if force_mult
-0000ecc0: 6974 7970 653a 0a20 2020 2020 2020 206b  itype:.        k
-0000ecd0: 7761 7267 735b 2270 726f 6d6f 7465 5f74  wargs["promote_t
-0000ece0: 6f5f 6d75 6c74 6922 5d20 3d20 5472 7565  o_multi"] = True
-0000ecf0: 0a0a 2020 2020 2320 4e6f 7720 7765 2063  ..    # Now we c
-0000ed00: 616e 2077 7269 7465 0a20 2020 2067 6466  an write.    gdf
-0000ed10: 5f74 6f5f 7772 6974 6520 3d20 6764 660a  _to_write = gdf.
-0000ed20: 2020 2020 6966 2067 656f 6669 6c65 7479      if geofilety
-0000ed30: 7065 203d 3d20 4765 6f66 696c 6554 7970  pe == GeofileTyp
-0000ed40: 652e 4553 5249 5368 6170 6566 696c 653a  e.ESRIShapefile:
-0000ed50: 0a20 2020 2020 2020 2069 6620 696e 6465  .        if inde
-0000ed60: 7820 6973 2054 7275 653a 0a20 2020 2020  x is True:.     
-0000ed70: 2020 2020 2020 2067 6466 5f74 6f5f 7772         gdf_to_wr
-0000ed80: 6974 6520 3d20 6764 662e 7265 7365 745f  ite = gdf.reset_
-0000ed90: 696e 6465 7828 6472 6f70 3d54 7275 6529  index(drop=True)
-0000eda0: 0a0a 2020 2020 6966 2067 656f 6669 6c65  ..    if geofile
-0000edb0: 7479 7065 2e69 735f 7369 6e67 6c65 6c61  type.is_singlela
-0000edc0: 7965 723a 0a20 2020 2020 2020 2070 796f  yer:.        pyo
-0000edd0: 6772 696f 2e77 7269 7465 5f64 6174 6166  grio.write_dataf
-0000ede0: 7261 6d65 2867 6466 5f74 6f5f 7772 6974  rame(gdf_to_writ
-0000edf0: 652c 2073 7472 2870 6174 6829 2c20 2a2a  e, str(path), **
-0000ee00: 6b77 6172 6773 290a 2020 2020 656c 7365  kwargs).    else
-0000ee10: 3a0a 2020 2020 2020 2020 7079 6f67 7269  :.        pyogri
-0000ee20: 6f2e 7772 6974 655f 6461 7461 6672 616d  o.write_datafram
-0000ee30: 6528 6764 665f 746f 5f77 7269 7465 2c20  e(gdf_to_write, 
-0000ee40: 7374 7228 7061 7468 292c 206c 6179 6572  str(path), layer
-0000ee50: 3d6c 6179 6572 2c20 2a2a 6b77 6172 6773  =layer, **kwargs
-0000ee60: 290a 0a20 2020 2072 6574 7572 6e0a 0a0a  )..    return...
-0000ee70: 6465 6620 6765 745f 6372 7328 7061 7468  def get_crs(path
-0000ee80: 3a20 556e 696f 6e5b 7374 722c 2022 6f73  : Union[str, "os
-0000ee90: 2e50 6174 684c 696b 655b 416e 795d 225d  .PathLike[Any]"]
-0000eea0: 2920 2d3e 2070 7970 726f 6a2e 4352 533a  ) -> pyproj.CRS:
-0000eeb0: 0a20 2020 2022 2222 0a20 2020 2047 6574  .    """.    Get
-0000eec0: 2074 6865 2043 5253 2028 7072 6f6a 6563   the CRS (projec
-0000eed0: 7469 6f6e 2920 6f66 2074 6865 2066 696c  tion) of the fil
-0000eee0: 650a 0a20 2020 2041 7267 733a 0a20 2020  e..    Args:.   
-0000eef0: 2020 2020 2070 6174 6820 2850 6174 684c       path (PathL
-0000ef00: 696b 6529 3a20 5061 7468 2074 6f20 7468  ike): Path to th
-0000ef10: 6520 6669 6c65 2e0a 0a20 2020 2052 6574  e file...    Ret
-0000ef20: 7572 6e73 3a0a 2020 2020 2020 2020 7079  urns:.        py
-0000ef30: 7072 6f6a 2e43 5253 3a20 5468 6520 7072  proj.CRS: The pr
-0000ef40: 6f6a 6563 7469 6f6e 206f 6620 7468 6520  ojection of the 
-0000ef50: 6669 6c65 0a20 2020 2022 2222 0a20 2020  file.    """.   
-0000ef60: 2023 2054 4f44 4f3a 2073 6565 6d73 206c   # TODO: seems l
-0000ef70: 696b 6520 7375 7070 6f72 7420 666f 7220  ike support for 
-0000ef80: 6d75 6c74 6970 6c65 206c 6179 6572 7320  multiple layers 
-0000ef90: 696e 2074 6865 2066 696c 6520 6973 6e27  in the file isn'
-0000efa0: 7420 6865 7265 2079 6574 3f3f 3f0a 2020  t here yet???.  
-0000efb0: 2020 7769 7468 2066 696f 6e61 2e6f 7065    with fiona.ope
-0000efc0: 6e28 7374 7228 7061 7468 292c 2022 7222  n(str(path), "r"
-0000efd0: 2920 6173 2067 656f 6669 6c65 3a0a 2020  ) as geofile:.  
-0000efe0: 2020 2020 2020 6173 7365 7274 2067 656f        assert geo
-0000eff0: 6669 6c65 2069 7320 6e6f 7420 4e6f 6e65  file is not None
-0000f000: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000f010: 7079 7072 6f6a 2e43 5253 2867 656f 6669  pyproj.CRS(geofi
-0000f020: 6c65 2e63 7273 290a 0a0a 6465 6620 6973  le.crs)...def is
-0000f030: 5f67 656f 6669 6c65 2870 6174 683a 2055  _geofile(path: U
-0000f040: 6e69 6f6e 5b73 7472 2c20 226f 732e 5061  nion[str, "os.Pa
-0000f050: 7468 4c69 6b65 5b41 6e79 5d22 5d29 202d  thLike[Any]"]) -
-0000f060: 3e20 626f 6f6c 3a0a 2020 2020 2222 220a  > bool:.    """.
-0000f070: 2020 2020 4465 7465 726d 696e 6573 2062      Determines b
-0000f080: 6173 6564 206f 6e20 7468 6520 6669 6c65  ased on the file
-0000f090: 7061 7468 2069 6620 7468 6973 2069 7320  path if this is 
-0000f0a0: 6120 6765 6f66 696c 652e 0a0a 2020 2020  a geofile...    
-0000f0b0: 4172 6773 3a0a 2020 2020 2020 2020 7061  Args:.        pa
-0000f0c0: 7468 2028 5061 7468 4c69 6b65 293a 2054  th (PathLike): T
-0000f0d0: 6865 2066 696c 6520 7061 7468 2e0a 0a20  he file path... 
-0000f0e0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000f0f0: 2020 2020 626f 6f6c 3a20 5472 7565 2069      bool: True i
-0000f100: 6620 6974 2069 7320 6120 6765 6f20 6669  f it is a geo fi
-0000f110: 6c65 2e0a 2020 2020 2222 220a 2020 2020  le..    """.    
-0000f120: 7265 7475 726e 2069 735f 6765 6f66 696c  return is_geofil
-0000f130: 655f 6578 7428 5061 7468 2870 6174 6829  e_ext(Path(path)
-0000f140: 2e73 7566 6669 7829 0a0a 0a64 6566 2069  .suffix)...def i
-0000f150: 735f 6765 6f66 696c 655f 6578 7428 6669  s_geofile_ext(fi
-0000f160: 6c65 5f65 7874 3a20 7374 7229 202d 3e20  le_ext: str) -> 
-0000f170: 626f 6f6c 3a0a 2020 2020 2222 220a 2020  bool:.    """.  
-0000f180: 2020 4465 7465 726d 696e 6573 2062 6173    Determines bas
-0000f190: 6564 206f 6e20 7468 6520 6669 6c65 2065  ed on the file e
-0000f1a0: 7874 656e 7369 6f6e 2069 6620 7468 6973  xtension if this
-0000f1b0: 2069 7320 6120 6765 6f66 696c 652e 0a0a   is a geofile...
-0000f1c0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000f1d0: 2020 6669 6c65 5f65 7874 2028 7374 7229    file_ext (str)
-0000f1e0: 3a20 7468 6520 6578 7465 6e73 696f 6e2e  : the extension.
-0000f1f0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000f200: 2020 2020 2020 2062 6f6f 6c3a 2054 7275         bool: Tru
-0000f210: 6520 6966 2069 7420 6973 2061 2067 656f  e if it is a geo
-0000f220: 6669 6c65 2e0a 2020 2020 2222 220a 2020  file..    """.  
-0000f230: 2020 7472 793a 0a20 2020 2020 2020 2023    try:.        #
-0000f240: 2049 6620 7468 6520 6472 6976 6572 2063   If the driver c
-0000f250: 616e 2062 6520 6465 7465 726d 696e 6564  an be determined
-0000f260: 2c20 6974 2069 7320 6120 2873 7570 706f  , it is a (suppo
-0000f270: 7274 6564 2920 6765 6f20 6669 6c65 2e0a  rted) geo file..
-0000f280: 2020 2020 2020 2020 5f20 3d20 4765 6f66          _ = Geof
-0000f290: 696c 6554 7970 6528 6669 6c65 5f65 7874  ileType(file_ext
-0000f2a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000f2b0: 2054 7275 650a 2020 2020 6578 6365 7074   True.    except
-0000f2c0: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
-0000f2d0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0000f2e0: 0a0a 0a64 6566 2063 6d70 280a 2020 2020  ...def cmp(.    
-0000f2f0: 7061 7468 313a 2055 6e69 6f6e 5b73 7472  path1: Union[str
-0000f300: 2c20 226f 732e 5061 7468 4c69 6b65 5b41  , "os.PathLike[A
-0000f310: 6e79 5d22 5d2c 2070 6174 6832 3a20 556e  ny]"], path2: Un
-0000f320: 696f 6e5b 7374 722c 2022 6f73 2e50 6174  ion[str, "os.Pat
-0000f330: 684c 696b 655b 416e 795d 225d 0a29 202d  hLike[Any]"].) -
-0000f340: 3e20 626f 6f6c 3a0a 2020 2020 2222 220a  > bool:.    """.
-0000f350: 2020 2020 436f 6d70 6172 6520 6966 2074      Compare if t
-0000f360: 776f 2067 656f 6669 6c65 7320 6172 6520  wo geofiles are 
-0000f370: 6964 656e 7469 6361 6c2e 0a0a 2020 2020  identical...    
-0000f380: 466f 7220 6765 6f66 696c 6573 2074 6861  For geofiles tha
-0000f390: 7420 7573 6520 6d75 6c74 6970 6c65 2066  t use multiple f
-0000f3a0: 696c 6573 2c20 616c 6c20 7265 6c65 7661  iles, all releva
-0000f3b0: 6e74 2066 696c 6573 206d 7573 7420 6265  nt files must be
-0000f3c0: 2069 6465 6e74 6963 616c 2e0a 2020 2020   identical..    
-0000f3d0: 4567 2e20 666f 7220 7368 6170 6566 696c  Eg. for shapefil
-0000f3e0: 6573 2c20 7468 6520 2e73 6870 2c20 2e73  es, the .shp, .s
-0000f3f0: 6878 2061 6e64 202e 6462 6620 6669 6c65  hx and .dbf file
-0000f400: 206d 7573 7420 6265 2069 6465 6e74 6963   must be identic
-0000f410: 616c 2e0a 0a20 2020 2041 7267 733a 0a20  al...    Args:. 
-0000f420: 2020 2020 2020 2070 6174 6831 2028 5061         path1 (Pa
-0000f430: 7468 4c69 6b65 293a 2070 6174 6820 746f  thLike): path to
-0000f440: 2074 6865 2066 6972 7374 2066 696c 652e   the first file.
-0000f450: 0a20 2020 2020 2020 2070 6174 6832 2028  .        path2 (
-0000f460: 5061 7468 4c69 6b65 293a 2070 6174 6820  PathLike): path 
-0000f470: 746f 2074 6865 2073 6563 6f6e 6420 6669  to the second fi
-0000f480: 6c65 2e0a 0a20 2020 2052 6574 7572 6e73  le...    Returns
-0000f490: 3a0a 2020 2020 2020 2020 626f 6f6c 3a20  :.        bool: 
-0000f4a0: 5472 7565 2069 6620 7468 6520 6669 6c65  True if the file
-0000f4b0: 7320 6172 6520 6964 656e 7469 6361 6c0a  s are identical.
-0000f4c0: 2020 2020 2222 220a 2020 2020 2320 4368      """.    # Ch
-0000f4d0: 6563 6b20 696e 7075 7420 7061 7261 6d65  eck input parame
-0000f4e0: 7465 7273 0a20 2020 2070 6174 6831 5f70  ters.    path1_p
-0000f4f0: 203d 2050 6174 6828 7061 7468 3129 0a20   = Path(path1). 
-0000f500: 2020 2070 6174 6832 5f70 203d 2050 6174     path2_p = Pat
-0000f510: 6828 7061 7468 3229 0a0a 2020 2020 2320  h(path2)..    # 
-0000f520: 466f 7220 6120 7368 6170 6566 696c 652c  For a shapefile,
-0000f530: 206d 756c 7469 706c 6520 6669 6c65 7320   multiple files 
-0000f540: 6e65 6564 2074 6f20 6265 2063 6f6d 7061  need to be compa
-0000f550: 7265 640a 2020 2020 6966 2070 6174 6831  red.    if path1
-0000f560: 5f70 2e73 7566 6669 782e 6c6f 7765 7228  _p.suffix.lower(
-0000f570: 2920 3d3d 2022 2e73 6870 223a 0a20 2020  ) == ".shp":.   
-0000f580: 2020 2020 2070 6174 6832 5f6e 6f65 7874       path2_noext
-0000f590: 2c20 5f20 3d20 6f73 2e70 6174 682e 7370  , _ = os.path.sp
-0000f5a0: 6c69 7465 7874 2870 6174 6832 5f70 290a  litext(path2_p).
-0000f5b0: 2020 2020 2020 2020 7368 6170 6566 696c          shapefil
-0000f5c0: 655f 6261 7365 5f73 7566 6669 7865 7320  e_base_suffixes 
-0000f5d0: 3d20 5b22 2e73 6870 222c 2022 2e64 6266  = [".shp", ".dbf
-0000f5e0: 222c 2022 2e73 6878 225d 0a20 2020 2020  ", ".shx"].     
-0000f5f0: 2020 2070 6174 6831 5f6e 6f65 7874 203d     path1_noext =
-0000f600: 2070 6174 6831 5f70 2e70 6172 656e 7420   path1_p.parent 
-0000f610: 2f20 7061 7468 315f 702e 7374 656d 0a20  / path1_p.stem. 
-0000f620: 2020 2020 2020 2070 6174 6832 5f6e 6f65         path2_noe
-0000f630: 7874 203d 2070 6174 6832 5f70 2e70 6172  xt = path2_p.par
-0000f640: 656e 7420 2f20 7061 7468 325f 702e 7374  ent / path2_p.st
-0000f650: 656d 0a20 2020 2020 2020 2066 6f72 2065  em.        for e
-0000f660: 7874 2069 6e20 7368 6170 6566 696c 655f  xt in shapefile_
-0000f670: 6261 7365 5f73 7566 6669 7865 733a 0a20  base_suffixes:. 
-0000f680: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000f690: 7420 6669 6c65 636d 702e 636d 7028 6622  t filecmp.cmp(f"
-0000f6a0: 7b73 7472 2870 6174 6831 5f6e 6f65 7874  {str(path1_noext
-0000f6b0: 297d 7b65 7874 7d22 2c20 6622 7b73 7472  )}{ext}", f"{str
-0000f6c0: 2870 6174 6832 5f6e 6f65 7874 297d 7b65  (path2_noext)}{e
-0000f6d0: 7874 7d22 293a 0a20 2020 2020 2020 2020  xt}"):.         
-0000f6e0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0000f6f0: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
-0000f700: 2020 2020 2020 2020 6622 4669 6c65 207b          f"File {
-0000f710: 7061 7468 315f 6e6f 6578 747d 7b65 7874  path1_noext}{ext
-0000f720: 7d20 6973 2064 6966 6665 7265 6e74 2066  } is different f
-0000f730: 726f 6d20 7b70 6174 6832 5f6e 6f65 7874  rom {path2_noext
-0000f740: 7d7b 6578 747d 220a 2020 2020 2020 2020  }{ext}".        
-0000f750: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000f760: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000f770: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
-0000f780: 6574 7572 6e20 5472 7565 0a20 2020 2065  eturn True.    e
-0000f790: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
-0000f7a0: 7572 6e20 6669 6c65 636d 702e 636d 7028  urn filecmp.cmp(
-0000f7b0: 7374 7228 7061 7468 315f 7029 2c20 7374  str(path1_p), st
-0000f7c0: 7228 7061 7468 325f 7029 290a 0a0a 6465  r(path2_p))...de
-0000f7d0: 6620 636f 7079 2873 7263 3a20 556e 696f  f copy(src: Unio
-0000f7e0: 6e5b 7374 722c 2022 6f73 2e50 6174 684c  n[str, "os.PathL
-0000f7f0: 696b 655b 416e 795d 225d 2c20 6473 743a  ike[Any]"], dst:
-0000f800: 2055 6e69 6f6e 5b73 7472 2c20 226f 732e   Union[str, "os.
-0000f810: 5061 7468 4c69 6b65 5b41 6e79 5d22 5d29  PathLike[Any]"])
-0000f820: 3a0a 2020 2020 2222 220a 2020 2020 436f  :.    """.    Co
-0000f830: 7069 6573 2074 6865 2067 656f 6669 6c65  pies the geofile
-0000f840: 2066 726f 6d20 7372 6320 746f 2064 7374   from src to dst
-0000f850: 2e20 4973 2074 6865 2073 6f75 7263 6520  . Is the source 
-0000f860: 6669 6c65 2069 7320 6120 6765 6f66 696c  file is a geofil
-0000f870: 6520 636f 6e74 6169 6e69 6e67 0a20 2020  e containing.   
-0000f880: 206f 6620 6d75 6c74 6970 6c65 2066 696c   of multiple fil
-0000f890: 6573 2028 6567 2e20 2e73 6870 2920 616c  es (eg. .shp) al
-0000f8a0: 6c20 6669 6c65 7320 6172 6520 636f 7069  l files are copi
-0000f8b0: 6564 2e0a 0a20 2020 2041 7267 733a 0a20  ed...    Args:. 
-0000f8c0: 2020 2020 2020 2073 7263 2028 5061 7468         src (Path
-0000f8d0: 4c69 6b65 293a 2074 6865 2066 696c 6520  Like): the file 
-0000f8e0: 746f 2063 6f70 792e 0a20 2020 2020 2020  to copy..       
-0000f8f0: 2064 7374 2028 5061 7468 4c69 6b65 293a   dst (PathLike):
-0000f900: 2074 6865 206c 6f63 6174 696f 6e20 746f   the location to
-0000f910: 2063 6f70 7920 7468 6520 6669 6c65 2873   copy the file(s
-0000f920: 2920 746f 2e0a 2020 2020 2222 220a 2020  ) to..    """.  
-0000f930: 2020 2320 4368 6563 6b20 696e 7075 7420    # Check input 
-0000f940: 7061 7261 6d65 7465 7273 0a20 2020 2073  parameters.    s
-0000f950: 7263 203d 2050 6174 6828 7372 6329 0a20  rc = Path(src). 
-0000f960: 2020 2064 7374 203d 2050 6174 6828 6473     dst = Path(ds
-0000f970: 7429 0a20 2020 2067 656f 6669 6c65 7479  t).    geofilety
-0000f980: 7065 203d 2047 656f 6669 6c65 5479 7065  pe = GeofileType
-0000f990: 2873 7263 290a 0a20 2020 2023 2043 6f70  (src)..    # Cop
-0000f9a0: 7920 7468 6520 6d61 696e 2066 696c 650a  y the main file.
-0000f9b0: 2020 2020 7368 7574 696c 2e63 6f70 7928      shutil.copy(
-0000f9c0: 7374 7228 7372 6329 2c20 6473 7429 0a0a  str(src), dst)..
-0000f9d0: 2020 2020 2320 466f 7220 736f 6d65 2066      # For some f
-0000f9e0: 696c 6520 7479 7065 732c 2065 7874 7261  ile types, extra
-0000f9f0: 2066 696c 6573 206e 6565 6420 746f 2062   files need to b
-0000fa00: 6520 636f 7069 6564 0a20 2020 2023 2049  e copied.    # I
-0000fa10: 6620 6465 7374 2069 7320 6120 6469 722c  f dest is a dir,
-0000fa20: 206a 7573 7420 7573 6520 6d6f 7665 2e20   just use move. 
-0000fa30: 4f74 6865 7277 6973 6520 636f 6e63 6174  Otherwise concat
-0000fa40: 2064 6573 7420 6669 6c65 7061 7468 730a   dest filepaths.
-0000fa50: 2020 2020 6966 2067 656f 6669 6c65 7479      if geofilety
-0000fa60: 7065 2e73 7566 6669 7865 735f 6578 7472  pe.suffixes_extr
-0000fa70: 6166 696c 6573 2069 7320 6e6f 7420 4e6f  afiles is not No
-0000fa80: 6e65 3a0a 2020 2020 2020 2020 6966 2064  ne:.        if d
-0000fa90: 7374 2e69 735f 6469 7228 293a 0a20 2020  st.is_dir():.   
-0000faa0: 2020 2020 2020 2020 2066 6f72 2073 7566           for suf
-0000fab0: 6669 7820 696e 2067 656f 6669 6c65 7479  fix in geofilety
-0000fac0: 7065 2e73 7566 6669 7865 735f 6578 7472  pe.suffixes_extr
-0000fad0: 6166 696c 6573 3a0a 2020 2020 2020 2020  afiles:.        
-0000fae0: 2020 2020 2020 2020 7372 6366 696c 6520          srcfile 
-0000faf0: 3d20 7372 632e 7061 7265 6e74 202f 2066  = src.parent / f
-0000fb00: 227b 7372 632e 7374 656d 7d7b 7375 6666  "{src.stem}{suff
-0000fb10: 6978 7d22 0a20 2020 2020 2020 2020 2020  ix}".           
-0000fb20: 2020 2020 2069 6620 7372 6366 696c 652e       if srcfile.
-0000fb30: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-0000fb40: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-0000fb50: 7574 696c 2e63 6f70 7928 7374 7228 7372  util.copy(str(sr
-0000fb60: 6366 696c 6529 2c20 6473 7429 0a20 2020  cfile), dst).   
-0000fb70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000fb80: 2020 2020 2020 2066 6f72 2073 7566 6669         for suffi
-0000fb90: 7820 696e 2067 656f 6669 6c65 7479 7065  x in geofiletype
-0000fba0: 2e73 7566 6669 7865 735f 6578 7472 6166  .suffixes_extraf
-0000fbb0: 696c 6573 3a0a 2020 2020 2020 2020 2020  iles:.          
-0000fbc0: 2020 2020 2020 7372 6366 696c 6520 3d20        srcfile = 
-0000fbd0: 7372 632e 7061 7265 6e74 202f 2066 227b  src.parent / f"{
-0000fbe0: 7372 632e 7374 656d 7d7b 7375 6666 6978  src.stem}{suffix
-0000fbf0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-0000fc00: 2020 2064 7374 6669 6c65 203d 2064 7374     dstfile = dst
-0000fc10: 2e70 6172 656e 7420 2f20 6622 7b64 7374  .parent / f"{dst
-0000fc20: 2e73 7465 6d7d 7b73 7566 6669 787d 220a  .stem}{suffix}".
-0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc40: 6966 2073 7263 6669 6c65 2e65 7869 7374  if srcfile.exist
-0000fc50: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-0000fc60: 2020 2020 2020 2020 2073 6875 7469 6c2e           shutil.
-0000fc70: 636f 7079 2873 7472 2873 7263 6669 6c65  copy(str(srcfile
-0000fc80: 292c 2064 7374 6669 6c65 290a 0a0a 6465  ), dstfile)...de
-0000fc90: 6620 6d6f 7665 2873 7263 3a20 556e 696f  f move(src: Unio
-0000fca0: 6e5b 7374 722c 2022 6f73 2e50 6174 684c  n[str, "os.PathL
-0000fcb0: 696b 655b 416e 795d 225d 2c20 6473 743a  ike[Any]"], dst:
-0000fcc0: 2055 6e69 6f6e 5b73 7472 2c20 226f 732e   Union[str, "os.
-0000fcd0: 5061 7468 4c69 6b65 5b41 6e79 5d22 5d29  PathLike[Any]"])
-0000fce0: 3a0a 2020 2020 2222 220a 2020 2020 4d6f  :.    """.    Mo
-0000fcf0: 7665 7320 7468 6520 6765 6f66 696c 6520  ves the geofile 
-0000fd00: 6672 6f6d 2073 7263 2074 6f20 6473 742e  from src to dst.
-0000fd10: 2049 6620 7468 6520 736f 7572 6365 2066   If the source f
-0000fd20: 696c 6520 6973 2061 2067 656f 6669 6c65  ile is a geofile
-0000fd30: 2063 6f6e 7461 696e 696e 670a 2020 2020   containing.    
-0000fd40: 6f66 206d 756c 7469 706c 6520 6669 6c65  of multiple file
-0000fd50: 7320 2865 672e 202e 7368 7029 2061 6c6c  s (eg. .shp) all
-0000fd60: 2066 696c 6573 2061 7265 206d 6f76 6564   files are moved
-0000fd70: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-0000fd80: 2020 2020 2073 7263 2028 5061 7468 4c69       src (PathLi
-0000fd90: 6b65 293a 2074 6865 2066 696c 6520 746f  ke): the file to
-0000fda0: 206d 6f76 650a 2020 2020 2020 2020 6473   move.        ds
-0000fdb0: 7420 2850 6174 684c 696b 6529 3a20 7468  t (PathLike): th
-0000fdc0: 6520 6c6f 6361 7469 6f6e 2074 6f20 6d6f  e location to mo
-0000fdd0: 7665 2074 6865 2066 696c 6528 7329 2074  ve the file(s) t
-0000fde0: 6f0a 2020 2020 2222 220a 2020 2020 2320  o.    """.    # 
-0000fdf0: 4368 6563 6b20 696e 7075 7420 7061 7261  Check input para
-0000fe00: 6d65 7465 7273 0a20 2020 2073 7263 203d  meters.    src =
-0000fe10: 2050 6174 6828 7372 6329 0a20 2020 2064   Path(src).    d
-0000fe20: 7374 203d 2050 6174 6828 6473 7429 0a20  st = Path(dst). 
-0000fe30: 2020 2067 656f 6669 6c65 7479 7065 203d     geofiletype =
-0000fe40: 2047 656f 6669 6c65 5479 7065 2873 7263   GeofileType(src
-0000fe50: 290a 0a20 2020 2023 204d 6f76 6520 7468  )..    # Move th
-0000fe60: 6520 6d61 696e 2066 696c 650a 2020 2020  e main file.    
-0000fe70: 7368 7574 696c 2e6d 6f76 6528 7374 7228  shutil.move(str(
-0000fe80: 7372 6329 2c20 6473 7429 0a0a 2020 2020  src), dst)..    
-0000fe90: 2320 466f 7220 736f 6d65 2066 696c 6520  # For some file 
-0000fea0: 7479 7065 732c 2065 7874 7261 2066 696c  types, extra fil
-0000feb0: 6573 206e 6565 6420 746f 2062 6520 6d6f  es need to be mo
-0000fec0: 7665 640a 2020 2020 2320 4966 2064 6573  ved.    # If des
-0000fed0: 7420 6973 2061 2064 6972 2c20 6a75 7374  t is a dir, just
-0000fee0: 2075 7365 206d 6f76 652e 204f 7468 6572   use move. Other
-0000fef0: 7769 7365 2063 6f6e 6361 7420 6465 7374  wise concat dest
-0000ff00: 2066 696c 6570 6174 6873 0a20 2020 2069   filepaths.    i
-0000ff10: 6620 6765 6f66 696c 6574 7970 652e 7375  f geofiletype.su
-0000ff20: 6666 6978 6573 5f65 7874 7261 6669 6c65  ffixes_extrafile
-0000ff30: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-0000ff40: 2020 2020 2020 2069 6620 6473 742e 6973         if dst.is
-0000ff50: 5f64 6972 2829 3a0a 2020 2020 2020 2020  _dir():.        
-0000ff60: 2020 2020 666f 7220 7375 6666 6978 2069      for suffix i
-0000ff70: 6e20 6765 6f66 696c 6574 7970 652e 7375  n geofiletype.su
-0000ff80: 6666 6978 6573 5f65 7874 7261 6669 6c65  ffixes_extrafile
-0000ff90: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000ffa0: 2020 2073 7263 6669 6c65 203d 2073 7263     srcfile = src
-0000ffb0: 2e70 6172 656e 7420 2f20 6622 7b73 7263  .parent / f"{src
-0000ffc0: 2e73 7465 6d7d 7b73 7566 6669 787d 220a  .stem}{suffix}".
-0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffe0: 6966 2073 7263 6669 6c65 2e65 7869 7374  if srcfile.exist
-0000fff0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00010000: 2020 2020 2020 2020 2073 6875 7469 6c2e           shutil.
-00010010: 6d6f 7665 2873 7472 2873 7263 6669 6c65  move(str(srcfile
-00010020: 292c 2064 7374 290a 2020 2020 2020 2020  ), dst).        
-00010030: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00010040: 2020 666f 7220 7375 6666 6978 2069 6e20    for suffix in 
-00010050: 6765 6f66 696c 6574 7970 652e 7375 6666  geofiletype.suff
-00010060: 6978 6573 5f65 7874 7261 6669 6c65 733a  ixes_extrafiles:
-00010070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010080: 2073 7263 6669 6c65 203d 2073 7263 2e70   srcfile = src.p
-00010090: 6172 656e 7420 2f20 6622 7b73 7263 2e73  arent / f"{src.s
-000100a0: 7465 6d7d 7b73 7566 6669 787d 220a 2020  tem}{suffix}".  
-000100b0: 2020 2020 2020 2020 2020 2020 2020 6473                ds
-000100c0: 7466 696c 6520 3d20 6473 742e 7061 7265  tfile = dst.pare
-000100d0: 6e74 202f 2066 227b 6473 742e 7374 656d  nt / f"{dst.stem
-000100e0: 7d7b 7375 6666 6978 7d22 0a20 2020 2020  }{suffix}".     
-000100f0: 2020 2020 2020 2020 2020 2069 6620 7372             if sr
-00010100: 6366 696c 652e 6578 6973 7473 2829 3a0a  cfile.exists():.
-00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010120: 2020 2020 7368 7574 696c 2e6d 6f76 6528      shutil.move(
-00010130: 7374 7228 7372 6366 696c 6529 2c20 6473  str(srcfile), ds
-00010140: 7466 696c 6529 0a0a 0a64 6566 2072 656d  tfile)...def rem
-00010150: 6f76 6528 7061 7468 3a20 556e 696f 6e5b  ove(path: Union[
-00010160: 7374 722c 2022 6f73 2e50 6174 684c 696b  str, "os.PathLik
-00010170: 655b 416e 795d 225d 2c20 6d69 7373 696e  e[Any]"], missin
-00010180: 675f 6f6b 3a20 626f 6f6c 203d 2046 616c  g_ok: bool = Fal
-00010190: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
-000101a0: 2052 656d 6f76 6573 2074 6865 2067 656f   Removes the geo
-000101b0: 6669 6c65 2e20 4973 2069 7420 6973 2061  file. Is it is a
-000101c0: 2067 656f 6669 6c65 2063 6f6d 706f 7365   geofile compose
-000101d0: 6420 6f66 206d 756c 7469 706c 6520 6669  d of multiple fi
-000101e0: 6c65 730a 2020 2020 2865 672e 202e 7368  les.    (eg. .sh
-000101f0: 7029 2061 6c6c 2066 696c 6573 2061 7265  p) all files are
-00010200: 2072 656d 6f76 6564 2e0a 2020 2020 4966   removed..    If
-00010210: 202e 6c6f 636b 2066 696c 6573 2061 7265   .lock files are
-00010220: 2070 7265 7365 6e74 2c20 7468 6579 2061   present, they a
-00010230: 7265 2072 656d 6f76 6564 2061 7320 7765  re removed as we
-00010240: 6c6c 2e0a 0a20 2020 2041 7267 733a 0a20  ll...    Args:. 
-00010250: 2020 2020 2020 2070 6174 6820 2850 6174         path (Pat
-00010260: 684c 696b 6529 3a20 7468 6520 6669 6c65  hLike): the file
-00010270: 2074 6f20 7265 6d6f 7665 0a20 2020 2022   to remove.    "
-00010280: 2222 0a20 2020 2023 2043 6865 636b 2069  "".    # Check i
-00010290: 6e70 7574 2070 6172 616d 6574 6572 730a  nput parameters.
-000102a0: 2020 2020 7061 7468 203d 2050 6174 6828      path = Path(
-000102b0: 7061 7468 290a 2020 2020 6765 6f66 696c  path).    geofil
-000102c0: 6574 7970 6520 3d20 4765 6f66 696c 6554  etype = GeofileT
-000102d0: 7970 6528 7061 7468 290a 0a20 2020 2023  ype(path)..    #
-000102e0: 2049 6620 7468 6572 6520 6973 2061 206c   If there is a l
-000102f0: 6f63 6b20 6669 6c65 2c20 7265 6d6f 7665  ock file, remove
-00010300: 2069 740a 2020 2020 6c6f 636b 6669 6c65   it.    lockfile
-00010310: 5f70 6174 6820 3d20 7061 7468 2e70 6172  _path = path.par
-00010320: 656e 7420 2f20 6622 7b70 6174 682e 6e61  ent / f"{path.na
-00010330: 6d65 7d2e 6c6f 636b 220a 2020 2020 6c6f  me}.lock".    lo
-00010340: 636b 6669 6c65 5f70 6174 682e 756e 6c69  ckfile_path.unli
-00010350: 6e6b 286d 6973 7369 6e67 5f6f 6b3d 5472  nk(missing_ok=Tr
-00010360: 7565 290a 0a20 2020 2023 2052 656d 6f76  ue)..    # Remov
-00010370: 6520 7468 6520 6d61 696e 2066 696c 650a  e the main file.
-00010380: 2020 2020 6966 2070 6174 682e 6578 6973      if path.exis
-00010390: 7473 2829 3a0a 2020 2020 2020 2020 7061  ts():.        pa
-000103a0: 7468 2e75 6e6c 696e 6b28 6d69 7373 696e  th.unlink(missin
-000103b0: 675f 6f6b 3d6d 6973 7369 6e67 5f6f 6b29  g_ok=missing_ok)
-000103c0: 0a0a 2020 2020 2320 466f 7220 736f 6d65  ..    # For some
-000103d0: 2066 696c 6520 7479 7065 732c 2065 7874   file types, ext
-000103e0: 7261 2066 696c 6573 206e 6565 6420 746f  ra files need to
-000103f0: 2062 6520 7265 6d6f 7665 640a 2020 2020   be removed.    
-00010400: 6966 2067 656f 6669 6c65 7479 7065 2e73  if geofiletype.s
-00010410: 7566 6669 7865 735f 6578 7472 6166 696c  uffixes_extrafil
-00010420: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-00010430: 2020 2020 2020 2020 666f 7220 7375 6666          for suff
-00010440: 6978 2069 6e20 6765 6f66 696c 6574 7970  ix in geofiletyp
-00010450: 652e 7375 6666 6978 6573 5f65 7874 7261  e.suffixes_extra
-00010460: 6669 6c65 733a 0a20 2020 2020 2020 2020  files:.         
-00010470: 2020 2063 7572 725f 7061 7468 203d 2070     curr_path = p
-00010480: 6174 682e 7061 7265 6e74 202f 2066 227b  ath.parent / f"{
-00010490: 7061 7468 2e73 7465 6d7d 7b73 7566 6669  path.stem}{suffi
-000104a0: 787d 220a 2020 2020 2020 2020 2020 2020  x}".            
-000104b0: 6375 7272 5f70 6174 682e 756e 6c69 6e6b  curr_path.unlink
-000104c0: 286d 6973 7369 6e67 5f6f 6b3d 5472 7565  (missing_ok=True
-000104d0: 290a 0a0a 6465 6620 6170 7065 6e64 5f74  )...def append_t
-000104e0: 6f28 0a20 2020 2073 7263 3a20 556e 696f  o(.    src: Unio
-000104f0: 6e5b 7374 722c 2022 6f73 2e50 6174 684c  n[str, "os.PathL
-00010500: 696b 655b 416e 795d 225d 2c0a 2020 2020  ike[Any]"],.    
-00010510: 6473 743a 2055 6e69 6f6e 5b73 7472 2c20  dst: Union[str, 
-00010520: 226f 732e 5061 7468 4c69 6b65 5b41 6e79  "os.PathLike[Any
-00010530: 5d22 5d2c 0a20 2020 2073 7263 5f6c 6179  ]"],.    src_lay
-00010540: 6572 3a20 4f70 7469 6f6e 616c 5b73 7472  er: Optional[str
-00010550: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6473  ] = None,.    ds
-00010560: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
-00010570: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00010580: 2020 2073 7263 5f63 7273 3a20 556e 696f     src_crs: Unio
-00010590: 6e5b 696e 742c 2073 7472 2c20 4e6f 6e65  n[int, str, None
-000105a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6473  ] = None,.    ds
-000105b0: 745f 6372 733a 2055 6e69 6f6e 5b69 6e74  t_crs: Union[int
-000105c0: 2c20 7374 722c 204e 6f6e 655d 203d 204e  , str, None] = N
-000105d0: 6f6e 652c 0a20 2020 2072 6570 726f 6a65  one,.    reproje
-000105e0: 6374 3a20 626f 6f6c 203d 2046 616c 7365  ct: bool = False
-000105f0: 2c0a 2020 2020 6578 706c 6f64 6563 6f6c  ,.    explodecol
-00010600: 6c65 6374 696f 6e73 3a20 626f 6f6c 203d  lections: bool =
-00010610: 2046 616c 7365 2c0a 2020 2020 666f 7263   False,.    forc
-00010620: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
-00010630: 7974 7970 653a 2055 6e69 6f6e 5b47 656f  ytype: Union[Geo
-00010640: 6d65 7472 7954 7970 652c 2073 7472 2c20  metryType, str, 
-00010650: 4e6f 6e65 5d20 3d20 4e6f 6e65 2c0a 2020  None] = None,.  
-00010660: 2020 6372 6561 7465 5f73 7061 7469 616c    create_spatial
-00010670: 5f69 6e64 6578 3a20 4f70 7469 6f6e 616c  _index: Optional
-00010680: 5b62 6f6f 6c5d 203d 2054 7275 652c 0a20  [bool] = True,. 
-00010690: 2020 2061 7070 656e 645f 7469 6d65 6f75     append_timeou
-000106a0: 745f 733a 2069 6e74 203d 2036 3030 2c0a  t_s: int = 600,.
-000106b0: 2020 2020 7472 616e 7361 6374 696f 6e5f      transaction_
-000106c0: 7369 7a65 3a20 696e 7420 3d20 3530 3030  size: int = 5000
-000106d0: 302c 0a20 2020 2070 7265 7365 7276 655f  0,.    preserve_
-000106e0: 6669 643a 204f 7074 696f 6e61 6c5b 626f  fid: Optional[bo
-000106f0: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-00010700: 6f70 7469 6f6e 733a 2064 6963 7420 3d20  options: dict = 
-00010710: 7b7d 2c0a 293a 0a20 2020 2022 2222 0a20  {},.):.    """. 
-00010720: 2020 2041 7070 656e 6420 7372 6320 6669     Append src fi
-00010730: 6c65 2074 6f20 7468 6520 6473 7420 6669  le to the dst fi
-00010740: 6c65 2e0a 0a20 2020 2052 656d 6172 6b3a  le...    Remark:
-00010750: 2061 7070 656e 6420 6973 206e 6f74 2073   append is not s
-00010760: 7570 706f 7274 6564 2066 6f72 2061 6c6c  upported for all
-00010770: 2066 696c 6574 7970 6573 2069 6e20 6669   filetypes in fi
-00010780: 6f6e 612f 6765 6f70 616e 6461 7320 2830  ona/geopandas (0
-00010790: 2e38 290a 2020 2020 736f 2077 6f72 6b61  .8).    so worka
-000107a0: 726f 756e 6420 7669 6120 6764 616c 206e  round via gdal n
-000107b0: 6565 6465 642e 0a0a 2020 2020 5468 6520  eeded...    The 
-000107c0: 6f70 7469 6f6e 7320 7061 7261 6d65 7465  options paramete
-000107d0: 7220 6361 6e20 6265 2075 7365 6420 746f  r can be used to
-000107e0: 2070 6173 7320 616e 7920 7479 7065 206f   pass any type o
-000107f0: 6620 6f70 7469 6f6e 7320 746f 2047 4441  f options to GDA
-00010800: 4c20 696e 0a20 2020 2074 6865 2066 6f6c  L in.    the fol
-00010810: 6c6f 7769 6e67 2066 6f72 6d3a 0a20 2020  lowing form:.   
-00010820: 2020 2020 207b 2022 3c6f 7074 696f 6e5f       { "<option_
-00010830: 7479 7065 3e2e 3c6f 7074 696f 6e5f 6e61  type>.<option_na
-00010840: 6d65 3e22 3a20 3c6f 7074 696f 6e5f 7661  me>": <option_va
-00010850: 6c75 653e 207d 0a0a 2020 2020 5468 6520  lue> }..    The 
-00010860: 6f70 7469 6f6e 2074 7970 6573 2063 616e  option types can
-00010870: 2062 6520 616e 7920 6f66 2074 6865 2066   be any of the f
-00010880: 6f6c 6c6f 7769 6e67 3a0a 2020 2020 2020  ollowing:.      
-00010890: 2020 2d20 4c41 5945 525f 4352 4541 5449    - LAYER_CREATI
-000108a0: 4f4e 3a20 6c61 7965 7220 6372 6561 7469  ON: layer creati
-000108b0: 6f6e 206f 7074 696f 6e20 286c 636f 290a  on option (lco).
-000108c0: 2020 2020 2020 2020 2d20 4441 5441 5345          - DATASE
-000108d0: 545f 4352 4541 5449 4f4e 3a20 6461 7461  T_CREATION: data
-000108e0: 7365 7420 6372 6561 7469 6f6e 206f 7074  set creation opt
-000108f0: 696f 6e20 2864 7363 6f29 0a20 2020 2020  ion (dsco).     
-00010900: 2020 202d 2049 4e50 5554 5f4f 5045 4e3a     - INPUT_OPEN:
-00010910: 2069 6e70 7574 2064 6174 6173 6574 206f   input dataset o
-00010920: 7065 6e20 6f70 7469 6f6e 2028 6f6f 290a  pen option (oo).
-00010930: 2020 2020 2020 2020 2d20 4445 5354 494e          - DESTIN
-00010940: 4154 494f 4e5f 4f50 454e 3a20 6465 7374  ATION_OPEN: dest
-00010950: 696e 6174 696f 6e20 6461 7461 7365 7420  ination dataset 
-00010960: 6f70 656e 206f 7074 696f 6e20 2864 6f6f  open option (doo
-00010970: 290a 2020 2020 2020 2020 2d20 434f 4e46  ).        - CONF
-00010980: 4947 3a20 636f 6e66 6967 206f 7074 696f  IG: config optio
-00010990: 6e20 2863 6f6e 6669 6729 0a0a 2020 2020  n (config)..    
-000109a0: 5468 6520 6f70 7469 6f6e 7320 6361 6e20  The options can 
-000109b0: 6265 2066 6f75 6e64 2069 6e20 7468 6520  be found in the 
-000109c0: 5b47 4441 4c20 7665 6374 6f72 2064 7269  [GDAL vector dri
-000109d0: 7665 7220 646f 6375 6d65 6e74 6174 696f  ver documentatio
-000109e0: 6e5d 0a20 2020 2028 6874 7470 733a 2f2f  n].    (https://
-000109f0: 6764 616c 2e6f 7267 2f64 7269 7665 7273  gdal.org/drivers
-00010a00: 2f76 6563 746f 722f 696e 6465 782e 6874  /vector/index.ht
-00010a10: 6d6c 292e 0a0a 2020 2020 4172 6773 3a0a  ml)...    Args:.
-00010a20: 2020 2020 2020 2020 7372 6320 2855 6e69          src (Uni
-00010a30: 6f6e 5b73 7472 2c29 3a20 736f 7572 6365  on[str,): source
-00010a40: 2066 696c 6520 7061 7468 2e0a 2020 2020   file path..    
-00010a50: 2020 2020 6473 7420 2855 6e69 6f6e 5b73      dst (Union[s
-00010a60: 7472 2c29 3a20 6465 7374 696e 6174 696f  tr,): destinatio
-00010a70: 6e20 6669 6c65 2070 6174 682e 0a20 2020  n file path..   
-00010a80: 2020 2020 2073 7263 5f6c 6179 6572 2028       src_layer (
-00010a90: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00010aa0: 736f 7572 6365 206c 6179 6572 2e20 4465  source layer. De
-00010ab0: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-00010ac0: 2020 2020 2020 2020 6473 745f 6c61 7965          dst_laye
-00010ad0: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
-00010ae0: 293a 2064 6573 7469 6e61 7469 6f6e 206c  ): destination l
-00010af0: 6179 6572 2e20 4465 6661 756c 7473 2074  ayer. Defaults t
-00010b00: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-00010b10: 7372 635f 6372 7320 2873 7472 2c20 6f70  src_crs (str, op
-00010b20: 7469 6f6e 616c 293a 2061 6e20 6570 7367  tional): an epsg
-00010b30: 2069 6e74 206f 7220 616e 7974 6869 6e67   int or anything
-00010b40: 2073 7570 706f 7274 6564 0a20 2020 2020   supported.     
-00010b50: 2020 2020 2020 2062 7920 7468 6520 4f47         by the OG
-00010b60: 5253 7061 7469 616c 5265 6665 7265 6e63  RSpatialReferenc
-00010b70: 652e 5365 7446 726f 6d55 7365 7249 6e70  e.SetFromUserInp
-00010b80: 7574 2829 2063 616c 6c2c 2077 6869 6368  ut() call, which
-00010b90: 2069 6e63 6c75 6465 730a 2020 2020 2020   includes.      
-00010ba0: 2020 2020 2020 616e 2045 5053 4720 7374        an EPSG st
-00010bb0: 7269 6e67 2028 6567 2e20 2245 5053 473a  ring (eg. "EPSG:
-00010bc0: 3433 3236 2229 2c20 6120 7765 6c6c 206b  4326"), a well k
-00010bd0: 6e6f 776e 2074 6578 7420 2857 4b54 2920  nown text (WKT) 
-00010be0: 4352 530a 2020 2020 2020 2020 2020 2020  CRS.            
-00010bf0: 6465 6669 6e69 7469 6f6e 2c2e 2e2e 2044  definition,... D
-00010c00: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-00010c10: 0a20 2020 2020 2020 2064 7374 5f63 7273  .        dst_crs
-00010c20: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-00010c30: 3a20 616e 2065 7073 6720 696e 7420 6f72  : an epsg int or
-00010c40: 2061 6e79 7468 696e 6720 7375 7070 6f72   anything suppor
-00010c50: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00010c60: 6279 2074 6865 204f 4752 5370 6174 6961  by the OGRSpatia
-00010c70: 6c52 6566 6572 656e 6365 2e53 6574 4672  lReference.SetFr
-00010c80: 6f6d 5573 6572 496e 7075 7428 2920 6361  omUserInput() ca
-00010c90: 6c6c 2c20 7768 6963 6820 696e 636c 7564  ll, which includ
-00010ca0: 6573 0a20 2020 2020 2020 2020 2020 2061  es.            a
-00010cb0: 6e20 4550 5347 2073 7472 696e 6720 2865  n EPSG string (e
-00010cc0: 672e 2022 4550 5347 3a34 3332 3622 292c  g. "EPSG:4326"),
-00010cd0: 2061 2077 656c 6c20 6b6e 6f77 6e20 7465   a well known te
-00010ce0: 7874 2028 574b 5429 2043 5253 0a20 2020  xt (WKT) CRS.   
-00010cf0: 2020 2020 2020 2020 2064 6566 696e 6974           definit
-00010d00: 696f 6e2c 2e2e 2e20 4465 6661 756c 7473  ion,... Defaults
-00010d10: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
-00010d20: 2020 7265 7072 6f6a 6563 7420 2862 6f6f    reproject (boo
-00010d30: 6c2c 206f 7074 696f 6e61 6c29 3a20 5472  l, optional): Tr
-00010d40: 7565 2074 6f20 7265 7072 6f6a 6563 7420  ue to reproject 
-00010d50: 7768 696c 6520 636f 6e76 6572 7469 6e67  while converting
-00010d60: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00010d70: 2066 696c 652e 2044 6566 6175 6c74 7320   file. Defaults 
-00010d80: 746f 2046 616c 7365 2e0a 2020 2020 2020  to False..      
-00010d90: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
-00010da0: 696f 6e73 2028 626f 6f6c 292c 206f 7074  ions (bool), opt
-00010db0: 696f 6e61 6c29 3a20 5472 7565 2074 6f20  ional): True to 
-00010dc0: 6f75 7470 7574 206f 6e6c 7920 7369 6d70  output only simp
-00010dd0: 6c65 2067 656f 6d65 7472 6965 732e 0a20  le geometries.. 
-00010de0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00010df0: 6c74 7320 746f 2046 616c 7365 2e0a 2020  lts to False..  
-00010e00: 2020 2020 2020 666f 7263 655f 6f75 7470        force_outp
-00010e10: 7574 5f67 656f 6d65 7472 7974 7970 6520  ut_geometrytype 
-00010e20: 2855 6e69 6f6e 5b47 656f 6d65 7472 7954  (Union[GeometryT
-00010e30: 7970 652c 2073 7472 5d2c 206f 7074 696f  ype, str], optio
-00010e40: 6e61 6c29 3a20 4765 6f6d 6574 7279 2074  nal): Geometry t
-00010e50: 7970 652e 0a20 2020 2020 2020 2020 2020  ype..           
-00010e60: 2074 6f20 2874 7279 2074 6f29 2066 6f72   to (try to) for
-00010e70: 6365 2074 6865 206f 7574 7075 7420 746f  ce the output to
-00010e80: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00010e90: 6e65 2e0a 2020 2020 2020 2020 6372 6561  ne..        crea
-00010ea0: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
-00010eb0: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-00010ec0: 293a 2054 7275 6520 746f 2063 7265 6174  ): True to creat
-00010ed0: 6520 6120 7370 6174 6961 6c20 696e 6465  e a spatial inde
-00010ee0: 780a 2020 2020 2020 2020 2020 2020 6f6e  x.            on
-00010ef0: 2074 6865 2064 6573 7469 6e61 7469 6f6e   the destination
-00010f00: 2066 696c 652f 6c61 7965 722e 2049 6620   file/layer. If 
-00010f10: 4e6f 6e65 2c20 7468 6520 6465 6661 756c  None, the defaul
-00010f20: 7420 6265 6861 7669 6f75 7220 6279 2067  t behaviour by g
-00010f30: 6461 6c20 666f 720a 2020 2020 2020 2020  dal for.        
-00010f40: 2020 2020 7468 6174 2066 696c 6520 7479      that file ty
-00010f50: 7065 2069 7320 7265 7370 6563 7465 642e  pe is respected.
-00010f60: 2049 6620 7468 6520 4c41 5945 525f 4352   If the LAYER_CR
-00010f70: 4541 5449 4f4e 2e53 5041 5449 414c 5f49  EATION.SPATIAL_I
-00010f80: 4e44 4558 0a20 2020 2020 2020 2020 2020  NDEX.           
-00010f90: 2070 6172 616d 6574 6572 2069 7320 7370   parameter is sp
-00010fa0: 6563 6966 6965 6420 696e 206f 7074 696f  ecified in optio
-00010fb0: 6e73 2c20 6372 6561 7465 5f73 7061 7469  ns, create_spati
-00010fc0: 616c 5f69 6e64 6578 2069 7320 6967 6e6f  al_index is igno
-00010fd0: 7265 642e 0a20 2020 2020 2020 2020 2020  red..           
-00010fe0: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-00010ff0: 652e 0a20 2020 2020 2020 2061 7070 656e  e..        appen
-00011000: 645f 7469 6d65 6f75 745f 7320 2869 6e74  d_timeout_s (int
-00011010: 2c20 6f70 7469 6f6e 616c 293a 2074 696d  , optional): tim
-00011020: 656f 7574 2074 6f20 7573 6520 6966 2074  eout to use if t
-00011030: 6865 206f 7574 7075 7420 6669 6c65 2069  he output file i
-00011040: 730a 2020 2020 2020 2020 2020 2020 6265  s.            be
-00011050: 696e 6720 7772 6974 7465 6e20 746f 2062  ing written to b
-00011060: 7920 616e 6f74 6865 7220 7072 6f63 6573  y another proces
-00011070: 7320 616c 7265 6164 792e 2044 6566 6175  s already. Defau
-00011080: 6c74 7320 746f 2036 3030 2e0a 2020 2020  lts to 600..    
-00011090: 2020 2020 7472 616e 7361 6374 696f 6e5f      transaction_
-000110a0: 7369 7a65 2028 696e 742c 206f 7074 696f  size (int, optio
-000110b0: 6e61 6c29 3a20 5472 616e 7361 6374 696f  nal): Transactio
-000110c0: 6e20 7369 7a65 2e0a 2020 2020 2020 2020  n size..        
-000110d0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-000110e0: 3530 3030 302e 0a20 2020 2020 2020 2070  50000..        p
-000110f0: 7265 7365 7276 655f 6669 6420 2862 6f6f  reserve_fid (boo
-00011100: 6c2c 206f 7074 696f 6e61 6c29 3a20 5472  l, optional): Tr
-00011110: 7565 2074 6f20 6d61 6b65 2061 6e20 6578  ue to make an ex
-00011120: 7472 6120 6566 666f 7274 2074 6f20 7072  tra effort to pr
-00011130: 6573 6572 7665 2066 6964 2773 206f 660a  eserve fid's of.
-00011140: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00011150: 736f 7572 6365 206c 6179 6572 2074 6f20  source layer to 
-00011160: 7468 6520 6465 7374 696e 6174 696f 6e20  the destination 
-00011170: 6c61 7965 722e 2046 616c 7365 206e 6f74  layer. False not
-00011180: 2074 6f20 646f 2061 6e79 2065 6666 6f72   to do any effor
-00011190: 742e 204e 6f6e 650a 2020 2020 2020 2020  t. None.        
-000111a0: 2020 2020 746f 2075 7365 2074 6865 2064      to use the d
-000111b0: 6566 6175 6c74 2062 6568 6176 696f 7572  efault behaviour
-000111c0: 206f 6620 6764 616c 2c20 7468 6174 2061   of gdal, that a
-000111d0: 6c72 6561 6479 2070 7265 7365 7276 6573  lready preserves
-000111e0: 2069 6e20 736f 6d65 2063 6173 6573 2e0a   in some cases..
-000111f0: 2020 2020 2020 2020 2020 2020 536f 6d65              Some
-00011200: 2066 696c 6520 666f 726d 6174 7320 646f   file formats do
-00011210: 6e27 7420 6578 706c 6963 6974 6c79 2073  n't explicitly s
-00011220: 746f 7265 2074 6865 2066 6964 2028 652e  tore the fid (e.
-00011230: 672e 2073 6861 7065 6669 6c65 292c 2073  g. shapefile), s
-00011240: 6f20 7468 6579 0a20 2020 2020 2020 2020  o they.         
-00011250: 2020 2077 696c 6c20 6e65 7665 7220 6265     will never be
-00011260: 2061 626c 6520 746f 2070 7265 7365 7276   able to preserv
-00011270: 6520 6669 6473 2e20 4465 6661 756c 7473  e fids. Defaults
-00011280: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
-00011290: 2020 6f70 7469 6f6e 7320 2864 6963 742c    options (dict,
-000112a0: 206f 7074 696f 6e61 6c29 3a20 6f70 7469   optional): opti
-000112b0: 6f6e 7320 746f 2070 6173 7320 746f 2067  ons to pass to g
-000112c0: 6461 6c2e 0a0a 2020 2020 5261 6973 6573  dal...    Raises
-000112d0: 3a0a 2020 2020 2020 2020 5661 6c75 6545  :.        ValueE
-000112e0: 7272 6f72 3a20 616e 2069 6e76 616c 6964  rror: an invalid
-000112f0: 2070 6172 616d 6574 6572 2076 616c 7565   parameter value
-00011300: 2077 6173 2070 6173 7365 642e 0a20 2020   was passed..   
-00011310: 2020 2020 2052 756e 7469 6d65 4572 726f       RuntimeErro
-00011320: 723a 2074 696d 656f 7574 2077 6173 2072  r: timeout was r
-00011330: 6561 6368 6564 2077 6869 6c65 2074 7279  eached while try
-00011340: 696e 6720 746f 2061 7070 656e 6420 6461  ing to append da
-00011350: 7461 2074 6f20 7061 7468 2e0a 2020 2020  ta to path..    
-00011360: 2222 220a 2020 2020 2320 4368 6563 6b2f  """.    # Check/
-00011370: 636c 6561 6e20 696e 7075 7420 7061 7261  clean input para
-00011380: 6d73 0a20 2020 2073 7263 203d 2050 6174  ms.    src = Pat
-00011390: 6828 7372 6329 0a20 2020 2064 7374 203d  h(src).    dst =
-000113a0: 2050 6174 6828 6473 7429 0a20 2020 2069   Path(dst).    i
-000113b0: 6620 666f 7263 655f 6f75 7470 7574 5f67  f force_output_g
-000113c0: 656f 6d65 7472 7974 7970 6520 6973 206e  eometrytype is n
-000113d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000113e0: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
-000113f0: 6f6d 6574 7279 7479 7065 203d 2047 656f  ometrytype = Geo
-00011400: 6d65 7472 7954 7970 6528 666f 7263 655f  metryType(force_
-00011410: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
-00011420: 7970 6529 0a0a 2020 2020 2320 4669 6c65  ype)..    # File
-00011430: 7320 646f 6e27 7420 7479 7069 6361 6c6c  s don't typicall
-00011440: 7920 7375 7070 6f72 7420 6861 7669 6e67  y support having
-00011450: 206d 756c 7469 706c 6520 7072 6f63 6573   multiple proces
-00011460: 7365 7320 7772 6974 696e 670a 2020 2020  ses writing.    
-00011470: 2320 7369 6d75 6c74 616e 6f75 736c 7920  # simultanously 
-00011480: 746f 2074 6865 6d2c 2073 6f20 7573 6520  to them, so use 
-00011490: 6c6f 636b 2066 696c 6520 746f 2073 796e  lock file to syn
-000114a0: 6368 726f 6e69 7a65 2061 6363 6573 732e  chronize access.
-000114b0: 0a20 2020 206c 6f63 6b66 696c 6520 3d20  .    lockfile = 
-000114c0: 5061 7468 2866 227b 7374 7228 6473 7429  Path(f"{str(dst)
-000114d0: 7d2e 6c6f 636b 2229 0a0a 2020 2020 2320  }.lock")..    # 
-000114e0: 4966 2074 6865 2064 6573 7469 6e61 7469  If the destinati
-000114f0: 6f6e 2066 696c 6520 646f 6573 6e27 7420  on file doesn't 
-00011500: 6578 6973 7420 7965 742c 2062 7574 2074  exist yet, but t
-00011510: 6865 206c 6f63 6b66 696c 6520 646f 6573  he lockfile does
-00011520: 2c0a 2020 2020 2320 7472 7920 7265 6d6f  ,.    # try remo
-00011530: 7669 6e67 2074 6865 206c 6f63 6b66 696c  ving the lockfil
-00011540: 6520 6173 2069 7420 6d69 6768 7420 6265  e as it might be
-00011550: 2061 2067 686f 7374 206c 6f63 6b66 696c   a ghost lockfil
-00011560: 652e 0a20 2020 2069 6620 6e6f 7420 6473  e..    if not ds
-00011570: 742e 6578 6973 7473 2829 2061 6e64 206c  t.exists() and l
-00011580: 6f63 6b66 696c 652e 6578 6973 7473 2829  ockfile.exists()
-00011590: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
-000115a0: 2020 2020 2020 2020 2020 206c 6f63 6b66             lockf
-000115b0: 696c 652e 756e 6c69 6e6b 2829 0a20 2020  ile.unlink().   
-000115c0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-000115d0: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
-000115e0: 2020 205f 203d 204e 6f6e 650a 0a20 2020     _ = None..   
-000115f0: 2023 2043 7265 6174 696e 6720 6c6f 636b   # Creating lock
-00011600: 6669 6c65 2061 6e64 2061 7070 656e 640a  file and append.
-00011610: 2020 2020 7374 6172 745f 7469 6d65 203d      start_time =
-00011620: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
-00011630: 6d65 2e6e 6f77 2829 0a20 2020 2072 6561  me.now().    rea
-00011640: 6479 203d 2046 616c 7365 0a20 2020 2077  dy = False.    w
-00011650: 6869 6c65 206e 6f74 2072 6561 6479 3a0a  hile not ready:.
-00011660: 2020 2020 2020 2020 6966 205f 696f 5f75          if _io_u
-00011670: 7469 6c2e 6372 6561 7465 5f66 696c 655f  til.create_file_
-00011680: 6174 6f6d 6963 286c 6f63 6b66 696c 6529  atomic(lockfile)
-00011690: 2069 7320 5472 7565 3a0a 2020 2020 2020   is True:.      
-000116a0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000116b0: 2020 2020 2020 2020 2020 2023 2061 7070             # app
-000116c0: 656e 640a 2020 2020 2020 2020 2020 2020  end.            
-000116d0: 2020 2020 5f61 7070 656e 645f 746f 5f6e      _append_to_n
-000116e0: 6f6c 6f63 6b28 0a20 2020 2020 2020 2020  olock(.         
-000116f0: 2020 2020 2020 2020 2020 2073 7263 3d73             src=s
-00011700: 7263 2c0a 2020 2020 2020 2020 2020 2020  rc,.            
-00011710: 2020 2020 2020 2020 6473 743d 6473 742c          dst=dst,
-00011720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011730: 2020 2020 2073 7263 5f6c 6179 6572 3d73       src_layer=s
-00011740: 7263 5f6c 6179 6572 2c0a 2020 2020 2020  rc_layer,.      
-00011750: 2020 2020 2020 2020 2020 2020 2020 6473                ds
-00011760: 745f 6c61 7965 723d 6473 745f 6c61 7965  t_layer=dst_laye
-00011770: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00011780: 2020 2020 2020 2073 7263 5f63 7273 3d73         src_crs=s
-00011790: 7263 5f63 7273 2c0a 2020 2020 2020 2020  rc_crs,.        
-000117a0: 2020 2020 2020 2020 2020 2020 6473 745f              dst_
-000117b0: 6372 733d 6473 745f 6372 732c 0a20 2020  crs=dst_crs,.   
-000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117d0: 2072 6570 726f 6a65 6374 3d72 6570 726f   reproject=repro
-000117e0: 6a65 6374 2c0a 2020 2020 2020 2020 2020  ject,.          
-000117f0: 2020 2020 2020 2020 2020 6578 706c 6f64            explod
-00011800: 6563 6f6c 6c65 6374 696f 6e73 3d65 7870  ecollections=exp
-00011810: 6c6f 6465 636f 6c6c 6563 7469 6f6e 732c  lodecollections,
-00011820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011830: 2020 2020 2066 6f72 6365 5f6f 7574 7075       force_outpu
-00011840: 745f 6765 6f6d 6574 7279 7479 7065 3d66  t_geometrytype=f
-00011850: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
-00011860: 6574 7279 7479 7065 2c0a 2020 2020 2020  etrytype,.      
-00011870: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-00011880: 6561 7465 5f73 7061 7469 616c 5f69 6e64  eate_spatial_ind
-00011890: 6578 3d63 7265 6174 655f 7370 6174 6961  ex=create_spatia
-000118a0: 6c5f 696e 6465 782c 0a20 2020 2020 2020  l_index,.       
-000118b0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-000118c0: 6e73 6163 7469 6f6e 5f73 697a 653d 7472  nsaction_size=tr
-000118d0: 616e 7361 6374 696f 6e5f 7369 7a65 2c0a  ansaction_size,.
-000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118f0: 2020 2020 7072 6573 6572 7665 5f66 6964      preserve_fid
-00011900: 3d70 7265 7365 7276 655f 6669 642c 0a20  =preserve_fid,. 
-00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 2020 206f 7074 696f 6e73 3d6f 7074 696f     options=optio
-00011930: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-00011940: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00011950: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
-00011960: 2020 2020 2020 2020 2020 2072 6561 6479             ready
-00011970: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00011980: 2020 2020 2020 2020 6c6f 636b 6669 6c65          lockfile
-00011990: 2e75 6e6c 696e 6b28 290a 2020 2020 2020  .unlink().      
-000119a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000119b0: 2020 2020 7469 6d65 5f77 6169 7469 6e67      time_waiting
-000119c0: 203d 2028 6461 7465 7469 6d65 2e64 6174   = (datetime.dat
-000119d0: 6574 696d 652e 6e6f 7728 2920 2d20 7374  etime.now() - st
-000119e0: 6172 745f 7469 6d65 292e 746f 7461 6c5f  art_time).total_
-000119f0: 7365 636f 6e64 7328 290a 2020 2020 2020  seconds().      
-00011a00: 2020 2020 2020 6966 2074 696d 655f 7761        if time_wa
-00011a10: 6974 696e 6720 3e20 6170 7065 6e64 5f74  iting > append_t
-00011a20: 696d 656f 7574 5f73 3a0a 2020 2020 2020  imeout_s:.      
-00011a30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00011a40: 5275 6e74 696d 6545 7272 6f72 280a 2020  RuntimeError(.  
-00011a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a60: 2020 6622 6170 7065 6e64 5f74 6f20 7469    f"append_to ti
-00011a70: 6d65 6f75 7420 6f66 207b 6170 7065 6e64  meout of {append
-00011a80: 5f74 696d 656f 7574 5f73 7d20 7265 6163  _timeout_s} reac
-00011a90: 6865 642c 2073 6f20 7374 6f70 2077 7269  hed, so stop wri
-00011aa0: 7465 2022 0a20 2020 2020 2020 2020 2020  te ".           
-00011ab0: 2020 2020 2020 2020 2066 2274 6f20 7b64           f"to {d
-00011ac0: 7374 7d21 220a 2020 2020 2020 2020 2020  st}!".          
-00011ad0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00011ae0: 2023 2053 6c65 6570 2066 6f72 2061 2073   # Sleep for a s
-00011af0: 6563 6f6e 6420 6265 666f 7265 2074 7279  econd before try
-00011b00: 696e 6720 6167 6169 6e0a 2020 2020 2020  ing again.      
-00011b10: 2020 7469 6d65 2e73 6c65 6570 2831 290a    time.sleep(1).
-00011b20: 0a0a 6465 6620 5f61 7070 656e 645f 746f  ..def _append_to
-00011b30: 5f6e 6f6c 6f63 6b28 0a20 2020 2073 7263  _nolock(.    src
-00011b40: 3a20 5061 7468 2c0a 2020 2020 6473 743a  : Path,.    dst:
-00011b50: 2050 6174 682c 0a20 2020 2073 7263 5f6c   Path,.    src_l
-00011b60: 6179 6572 3a20 4f70 7469 6f6e 616c 5b73  ayer: Optional[s
-00011b70: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00011b80: 6473 745f 6c61 7965 723a 204f 7074 696f  dst_layer: Optio
-00011b90: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00011ba0: 0a20 2020 2073 7263 5f63 7273 3a20 556e  .    src_crs: Un
-00011bb0: 696f 6e5b 696e 742c 2073 7472 2c20 4e6f  ion[int, str, No
-00011bc0: 6e65 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ne] = None,.    
-00011bd0: 6473 745f 6372 733a 2055 6e69 6f6e 5b69  dst_crs: Union[i
-00011be0: 6e74 2c20 7374 722c 204e 6f6e 655d 203d  nt, str, None] =
-00011bf0: 204e 6f6e 652c 0a20 2020 2072 6570 726f   None,.    repro
-00011c00: 6a65 6374 3a20 626f 6f6c 203d 2046 616c  ject: bool = Fal
-00011c10: 7365 2c0a 2020 2020 6578 706c 6f64 6563  se,.    explodec
-00011c20: 6f6c 6c65 6374 696f 6e73 3a20 626f 6f6c  ollections: bool
-00011c30: 203d 2046 616c 7365 2c0a 2020 2020 6372   = False,.    cr
-00011c40: 6561 7465 5f73 7061 7469 616c 5f69 6e64  eate_spatial_ind
-00011c50: 6578 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ex: Optional[boo
-00011c60: 6c5d 203d 2054 7275 652c 0a20 2020 2066  l] = True,.    f
-00011c70: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
-00011c80: 6574 7279 7479 7065 3a20 556e 696f 6e5b  etrytype: Union[
-00011c90: 4765 6f6d 6574 7279 5479 7065 2c20 7374  GeometryType, st
-00011ca0: 722c 204e 6f6e 655d 203d 204e 6f6e 652c  r, None] = None,
-00011cb0: 0a20 2020 2074 7261 6e73 6163 7469 6f6e  .    transaction
-00011cc0: 5f73 697a 653a 2069 6e74 203d 2035 3030  _size: int = 500
-00011cd0: 3030 2c0a 2020 2020 7072 6573 6572 7665  00,.    preserve
-00011ce0: 5f66 6964 3a20 4f70 7469 6f6e 616c 5b62  _fid: Optional[b
-00011cf0: 6f6f 6c5d 203d 204e 6f6e 652c 0a20 2020  ool] = None,.   
-00011d00: 206f 7074 696f 6e73 3a20 6469 6374 203d   options: dict =
-00011d10: 207b 7d2c 0a29 3a0a 2020 2020 2320 4368   {},.):.    # Ch
-00011d20: 6563 6b2f 636c 6561 6e20 696e 7075 7420  eck/clean input 
-00011d30: 7061 7261 6d73 0a20 2020 206f 7074 696f  params.    optio
-00011d40: 6e73 203d 205f 6f67 725f 7574 696c 2e5f  ns = _ogr_util._
-00011d50: 7072 6570 6172 655f 6764 616c 5f6f 7074  prepare_gdal_opt
-00011d60: 696f 6e73 286f 7074 696f 6e73 290a 2020  ions(options).  
-00011d70: 2020 6966 2028 0a20 2020 2020 2020 2063    if (.        c
-00011d80: 7265 6174 655f 7370 6174 6961 6c5f 696e  reate_spatial_in
-00011d90: 6465 7820 6973 206e 6f74 204e 6f6e 650a  dex is not None.
-00011da0: 2020 2020 2020 2020 616e 6420 224c 4159          and "LAY
-00011db0: 4552 5f43 5245 4154 494f 4e2e 5350 4154  ER_CREATION.SPAT
-00011dc0: 4941 4c5f 494e 4445 5822 206e 6f74 2069  IAL_INDEX" not i
-00011dd0: 6e20 6f70 7469 6f6e 730a 2020 2020 293a  n options.    ):
-00011de0: 0a20 2020 2020 2020 206f 7074 696f 6e73  .        options
-00011df0: 5b22 4c41 5945 525f 4352 4541 5449 4f4e  ["LAYER_CREATION
-00011e00: 2e53 5041 5449 414c 5f49 4e44 4558 225d  .SPATIAL_INDEX"]
-00011e10: 203d 2063 7265 6174 655f 7370 6174 6961   = create_spatia
-00011e20: 6c5f 696e 6465 780a 0a20 2020 2023 2057  l_index..    # W
-00011e30: 6865 6e20 6372 6561 7469 6e67 2f61 7070  hen creating/app
-00011e40: 656e 6469 6e67 2074 6f20 6120 7368 6170  ending to a shap
-00011e50: 6566 696c 652c 206c 6175 6e64 6572 2074  efile, launder t
-00011e60: 6865 2063 6f6c 756d 6e73 206e 616d 6573  he columns names
-00011e70: 2076 6961 0a20 2020 2023 2061 2073 716c   via.    # a sql
-00011e80: 2073 7461 7465 6d65 6e74 2c20 6f74 6865   statement, othe
-00011e90: 7277 6973 6520 7768 656e 2061 7070 656e  rwise when appen
-00011ea0: 6469 6e67 2074 6865 206c 6175 6e64 6572  ding the launder
-00011eb0: 6564 2063 6f6c 756d 6e73 2077 696c 6c0a  ed columns will.
-00011ec0: 2020 2020 2320 6765 7420 4e55 4c4c 2076      # get NULL v
-00011ed0: 616c 7565 7320 696e 7374 6561 6420 6f66  alues instead of
-00011ee0: 2074 6865 2064 6174 612e 0a20 2020 2073   the data..    s
-00011ef0: 716c 5f73 746d 7420 3d20 4e6f 6e65 0a20  ql_stmt = None. 
-00011f00: 2020 2073 7263 5f6c 6179 6572 696e 666f     src_layerinfo
-00011f10: 203d 204e 6f6e 650a 2020 2020 6966 2064   = None.    if d
-00011f20: 7374 2e73 7566 6669 782e 6c6f 7765 7228  st.suffix.lower(
-00011f30: 2920 3d3d 2022 2e73 6870 223a 0a20 2020  ) == ".shp":.   
-00011f40: 2020 2020 2073 7263 5f6c 6179 6572 696e       src_layerin
-00011f50: 666f 203d 2067 6574 5f6c 6179 6572 696e  fo = get_layerin
-00011f60: 666f 2873 7263 2c20 7372 635f 6c61 7965  fo(src, src_laye
-00011f70: 7229 0a20 2020 2020 2020 2073 7263 5f63  r).        src_c
-00011f80: 6f6c 756d 6e73 203d 2073 7263 5f6c 6179  olumns = src_lay
-00011f90: 6572 696e 666f 2e63 6f6c 756d 6e73 0a20  erinfo.columns. 
-00011fa0: 2020 2020 2020 2063 6f6c 756d 6e73 5f6c         columns_l
-00011fb0: 6175 6e64 6572 6564 203d 205f 6c61 756e  aundered = _laun
-00011fc0: 6465 725f 636f 6c75 6d6e 5f6e 616d 6573  der_column_names
-00011fd0: 2873 7263 5f63 6f6c 756d 6e73 290a 2020  (src_columns).  
-00011fe0: 2020 2020 2020 636f 6c75 6d6e 735f 616c        columns_al
-00011ff0: 6961 7365 6420 3d20 5b0a 2020 2020 2020  iased = [.      
-00012000: 2020 2020 2020 6627 227b 636f 6c75 6d6e        f'"{column
-00012010: 7d22 2041 5320 227b 6c61 756e 6465 7265  }" AS "{laundere
-00012020: 647d 2227 2066 6f72 2063 6f6c 756d 6e2c  d}"' for column,
-00012030: 206c 6175 6e64 6572 6564 2069 6e20 636f   laundered in co
-00012040: 6c75 6d6e 735f 6c61 756e 6465 7265 640a  lumns_laundered.
-00012050: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00012060: 2020 6c61 7965 7220 3d20 7372 635f 6c61    layer = src_la
-00012070: 7965 7220 6966 2073 7263 5f6c 6179 6572  yer if src_layer
-00012080: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-00012090: 6520 6765 745f 6f6e 6c79 5f6c 6179 6572  e get_only_layer
-000120a0: 2873 7263 290a 2020 2020 2020 2020 7371  (src).        sq
-000120b0: 6c5f 7374 6d74 203d 2066 2753 454c 4543  l_stmt = f'SELEC
-000120c0: 5420 7b22 2c20 222e 6a6f 696e 2863 6f6c  T {", ".join(col
-000120d0: 756d 6e73 5f61 6c69 6173 6564 297d 2046  umns_aliased)} F
-000120e0: 524f 4d20 227b 6c61 7965 727d 2227 0a0a  ROM "{layer}"'..
-000120f0: 2020 2020 2320 5768 656e 2064 7374 2066      # When dst f
-00012100: 696c 6520 646f 6573 6e27 7420 6578 6973  ile doesn't exis
-00012110: 7420 616e 6420 7372 6320 6973 2065 6d70  t and src is emp
-00012120: 7479 2066 6f72 6365 5f6f 7574 7075 745f  ty force_output_
-00012130: 6765 6f6d 6574 7279 7479 7065 2073 686f  geometrytype sho
-00012140: 756c 6420 6265 0a20 2020 2023 2073 7065  uld be.    # spe
-00012150: 6369 6669 6564 2c20 6f74 6865 7277 6973  cified, otherwis
-00012160: 6520 696e 7661 6c69 6420 6f75 7470 7574  e invalid output
-00012170: 2e0a 2020 2020 6966 2066 6f72 6365 5f6f  ..    if force_o
-00012180: 7574 7075 745f 6765 6f6d 6574 7279 7479  utput_geometryty
-00012190: 7065 2069 7320 4e6f 6e65 2061 6e64 206e  pe is None and n
-000121a0: 6f74 2064 7374 2e65 7869 7374 7328 293a  ot dst.exists():
-000121b0: 0a20 2020 2020 2020 2069 6620 7372 635f  .        if src_
-000121c0: 6c61 7965 7269 6e66 6f20 6973 204e 6f6e  layerinfo is Non
-000121d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000121e0: 7263 5f6c 6179 6572 696e 666f 203d 2067  rc_layerinfo = g
-000121f0: 6574 5f6c 6179 6572 696e 666f 2873 7263  et_layerinfo(src
-00012200: 2c20 7372 635f 6c61 7965 7229 0a20 2020  , src_layer).   
-00012210: 2020 2020 2066 6f72 6365 5f6f 7574 7075       force_outpu
-00012220: 745f 6765 6f6d 6574 7279 7479 7065 203d  t_geometrytype =
-00012230: 2073 7263 5f6c 6179 6572 696e 666f 2e67   src_layerinfo.g
-00012240: 656f 6d65 7472 7974 7970 650a 0a20 2020  eometrytype..   
-00012250: 2023 2047 6f21 0a20 2020 2074 7261 6e73   # Go!.    trans
-00012260: 6c61 7465 5f69 6e66 6f20 3d20 5f6f 6772  late_info = _ogr
-00012270: 5f75 7469 6c2e 5665 6374 6f72 5472 616e  _util.VectorTran
-00012280: 736c 6174 6549 6e66 6f28 0a20 2020 2020  slateInfo(.     
-00012290: 2020 2069 6e70 7574 5f70 6174 683d 7372     input_path=sr
-000122a0: 632c 0a20 2020 2020 2020 206f 7574 7075  c,.        outpu
-000122b0: 745f 7061 7468 3d64 7374 2c0a 2020 2020  t_path=dst,.    
-000122c0: 2020 2020 696e 7075 745f 6c61 7965 7273      input_layers
-000122d0: 3d73 7263 5f6c 6179 6572 2c0a 2020 2020  =src_layer,.    
-000122e0: 2020 2020 6f75 7470 7574 5f6c 6179 6572      output_layer
-000122f0: 3d64 7374 5f6c 6179 6572 2c0a 2020 2020  =dst_layer,.    
-00012300: 2020 2020 696e 7075 745f 7372 733d 7372      input_srs=sr
-00012310: 635f 6372 732c 0a20 2020 2020 2020 206f  c_crs,.        o
-00012320: 7574 7075 745f 7372 733d 6473 745f 6372  utput_srs=dst_cr
-00012330: 732c 0a20 2020 2020 2020 2073 716c 5f73  s,.        sql_s
-00012340: 746d 743d 7371 6c5f 7374 6d74 2c0a 2020  tmt=sql_stmt,.  
-00012350: 2020 2020 2020 7371 6c5f 6469 616c 6563        sql_dialec
-00012360: 743d 224f 4752 5351 4c22 2c0a 2020 2020  t="OGRSQL",.    
-00012370: 2020 2020 7265 7072 6f6a 6563 743d 7265      reproject=re
-00012380: 7072 6f6a 6563 742c 0a20 2020 2020 2020  project,.       
-00012390: 2074 7261 6e73 6163 7469 6f6e 5f73 697a   transaction_siz
-000123a0: 653d 7472 616e 7361 6374 696f 6e5f 7369  e=transaction_si
-000123b0: 7a65 2c0a 2020 2020 2020 2020 6170 7065  ze,.        appe
-000123c0: 6e64 3d54 7275 652c 0a20 2020 2020 2020  nd=True,.       
-000123d0: 2075 7064 6174 653d 5472 7565 2c0a 2020   update=True,.  
-000123e0: 2020 2020 2020 6578 706c 6f64 6563 6f6c        explodecol
-000123f0: 6c65 6374 696f 6e73 3d65 7870 6c6f 6465  lections=explode
-00012400: 636f 6c6c 6563 7469 6f6e 732c 0a20 2020  collections,.   
-00012410: 2020 2020 2066 6f72 6365 5f6f 7574 7075       force_outpu
-00012420: 745f 6765 6f6d 6574 7279 7479 7065 3d66  t_geometrytype=f
-00012430: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
-00012440: 6574 7279 7479 7065 2c0a 2020 2020 2020  etrytype,.      
-00012450: 2020 6f70 7469 6f6e 733d 6f70 7469 6f6e    options=option
-00012460: 732c 0a20 2020 2020 2020 2070 7265 7365  s,.        prese
-00012470: 7276 655f 6669 643d 7072 6573 6572 7665  rve_fid=preserve
-00012480: 5f66 6964 2c0a 2020 2020 290a 2020 2020  _fid,.    ).    
-00012490: 5f6f 6772 5f75 7469 6c2e 7665 6374 6f72  _ogr_util.vector
-000124a0: 5f74 7261 6e73 6c61 7465 5f62 795f 696e  _translate_by_in
-000124b0: 666f 2869 6e66 6f3d 7472 616e 736c 6174  fo(info=translat
-000124c0: 655f 696e 666f 290a 0a0a 6465 6620 636f  e_info)...def co
-000124d0: 6e76 6572 7428 0a20 2020 2073 7263 3a20  nvert(.    src: 
-000124e0: 556e 696f 6e5b 7374 722c 2022 6f73 2e50  Union[str, "os.P
-000124f0: 6174 684c 696b 655b 416e 795d 225d 2c0a  athLike[Any]"],.
-00012500: 2020 2020 6473 743a 2055 6e69 6f6e 5b73      dst: Union[s
-00012510: 7472 2c20 226f 732e 5061 7468 4c69 6b65  tr, "os.PathLike
-00012520: 5b41 6e79 5d22 5d2c 0a20 2020 2073 7263  [Any]"],.    src
-00012530: 5f6c 6179 6572 3a20 4f70 7469 6f6e 616c  _layer: Optional
-00012540: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-00012550: 2020 6473 745f 6c61 7965 723a 204f 7074    dst_layer: Opt
-00012560: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00012570: 652c 0a20 2020 2073 7263 5f63 7273 3a20  e,.    src_crs: 
-00012580: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
-00012590: 4e6f 6e65 5d20 3d20 4e6f 6e65 2c0a 2020  None] = None,.  
-000125a0: 2020 6473 745f 6372 733a 2055 6e69 6f6e    dst_crs: Union
-000125b0: 5b73 7472 2c20 696e 742c 204e 6f6e 655d  [str, int, None]
-000125c0: 203d 204e 6f6e 652c 0a20 2020 2072 6570   = None,.    rep
-000125d0: 726f 6a65 6374 3a20 626f 6f6c 203d 2046  roject: bool = F
-000125e0: 616c 7365 2c0a 2020 2020 6578 706c 6f64  alse,.    explod
-000125f0: 6563 6f6c 6c65 6374 696f 6e73 3a20 626f  ecollections: bo
-00012600: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00012610: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
-00012620: 6d65 7472 7974 7970 653a 2055 6e69 6f6e  metrytype: Union
-00012630: 5b47 656f 6d65 7472 7954 7970 652c 2073  [GeometryType, s
-00012640: 7472 2c20 4e6f 6e65 5d20 3d20 4e6f 6e65  tr, None] = None
-00012650: 2c0a 2020 2020 6372 6561 7465 5f73 7061  ,.    create_spa
-00012660: 7469 616c 5f69 6e64 6578 3a20 4f70 7469  tial_index: Opti
-00012670: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
-00012680: 652c 0a20 2020 2070 7265 7365 7276 655f  e,.    preserve_
-00012690: 6669 643a 204f 7074 696f 6e61 6c5b 626f  fid: Optional[bo
-000126a0: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-000126b0: 6f70 7469 6f6e 733a 2064 6963 7420 3d20  options: dict = 
-000126c0: 7b7d 2c0a 2020 2020 6170 7065 6e64 3a20  {},.    append: 
-000126d0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-000126e0: 2020 666f 7263 653a 2062 6f6f 6c20 3d20    force: bool = 
-000126f0: 4661 6c73 652c 0a29 3a0a 2020 2020 2222  False,.):.    ""
-00012700: 220a 2020 2020 5265 6164 2061 206c 6179  ".    Read a lay
-00012710: 6572 2066 726f 6d20 6120 736f 7572 6365  er from a source
-00012720: 2066 696c 6520 616e 6420 7772 6974 6520   file and write 
-00012730: 6974 2074 6f20 6120 6e65 7720 6465 7374  it to a new dest
-00012740: 696e 6174 696f 6e20 6669 6c65 2e0a 0a20  ination file... 
-00012750: 2020 2054 7970 6963 616c 6c79 2075 7365     Typically use
-00012760: 6420 746f 2063 6f6e 7665 7274 2066 726f  d to convert fro
-00012770: 6d20 6f6e 6520 6669 6c65 666f 726d 6174  m one fileformat
-00012780: 2074 6f20 616e 6f74 6865 7220 6f72 2074   to another or t
-00012790: 6f20 7265 7072 6f6a 6563 742e 0a0a 2020  o reproject...  
-000127a0: 2020 5468 6520 6f70 7469 6f6e 7320 7061    The options pa
-000127b0: 7261 6d65 7465 7220 6361 6e20 6265 2075  rameter can be u
-000127c0: 7365 6420 746f 2070 6173 7320 616e 7920  sed to pass any 
-000127d0: 7479 7065 206f 6620 6f70 7469 6f6e 7320  type of options 
-000127e0: 746f 2047 4441 4c20 696e 0a20 2020 2074  to GDAL in.    t
-000127f0: 6865 2066 6f6c 6c6f 7769 6e67 2066 6f72  he following for
-00012800: 6d3a 0a20 2020 2020 2020 207b 2022 3c6f  m:.        { "<o
-00012810: 7074 696f 6e5f 7479 7065 3e2e 3c6f 7074  ption_type>.<opt
-00012820: 696f 6e5f 6e61 6d65 3e22 3a20 3c6f 7074  ion_name>": <opt
-00012830: 696f 6e5f 7661 6c75 653e 207d 0a0a 2020  ion_value> }..  
-00012840: 2020 5468 6520 6f70 7469 6f6e 2074 7970    The option typ
-00012850: 6573 2063 616e 2062 6520 616e 7920 6f66  es can be any of
-00012860: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
-00012870: 2020 2020 2020 2020 2d20 4c41 5945 525f          - LAYER_
-00012880: 4352 4541 5449 4f4e 3a20 6c61 7965 7220  CREATION: layer 
-00012890: 6372 6561 7469 6f6e 206f 7074 696f 6e20  creation option 
-000128a0: 286c 636f 290a 2020 2020 2020 2020 2d20  (lco).        - 
-000128b0: 4441 5441 5345 545f 4352 4541 5449 4f4e  DATASET_CREATION
-000128c0: 3a20 6461 7461 7365 7420 6372 6561 7469  : dataset creati
-000128d0: 6f6e 206f 7074 696f 6e20 2864 7363 6f29  on option (dsco)
-000128e0: 0a20 2020 2020 2020 202d 2049 4e50 5554  .        - INPUT
-000128f0: 5f4f 5045 4e3a 2069 6e70 7574 2064 6174  _OPEN: input dat
-00012900: 6173 6574 206f 7065 6e20 6f70 7469 6f6e  aset open option
-00012910: 2028 6f6f 290a 2020 2020 2020 2020 2d20   (oo).        - 
-00012920: 4445 5354 494e 4154 494f 4e5f 4f50 454e  DESTINATION_OPEN
-00012930: 3a20 6465 7374 696e 6174 696f 6e20 6461  : destination da
-00012940: 7461 7365 7420 6f70 656e 206f 7074 696f  taset open optio
-00012950: 6e20 2864 6f6f 290a 2020 2020 2020 2020  n (doo).        
-00012960: 2d20 434f 4e46 4947 3a20 636f 6e66 6967  - CONFIG: config
-00012970: 206f 7074 696f 6e20 2863 6f6e 6669 6729   option (config)
-00012980: 0a0a 2020 2020 5468 6520 6f70 7469 6f6e  ..    The option
-00012990: 7320 6361 6e20 6265 2066 6f75 6e64 2069  s can be found i
-000129a0: 6e20 7468 6520 5b47 4441 4c20 7665 6374  n the [GDAL vect
-000129b0: 6f72 2064 7269 7665 7220 646f 6375 6d65  or driver docume
-000129c0: 6e74 6174 696f 6e5d 0a20 2020 2028 6874  ntation].    (ht
-000129d0: 7470 733a 2f2f 6764 616c 2e6f 7267 2f64  tps://gdal.org/d
-000129e0: 7269 7665 7273 2f76 6563 746f 722f 696e  rivers/vector/in
-000129f0: 6465 782e 6874 6d6c 292e 0a0a 2020 2020  dex.html)...    
-00012a00: 4172 6773 3a0a 2020 2020 2020 2020 7372  Args:.        sr
-00012a10: 6320 2850 6174 684c 696b 6529 3a20 5468  c (PathLike): Th
-00012a20: 6520 736f 7572 6365 2066 696c 6520 7061  e source file pa
-00012a30: 7468 2e0a 2020 2020 2020 2020 6473 7420  th..        dst 
-00012a40: 2850 6174 684c 696b 6529 3a20 5468 6520  (PathLike): The 
-00012a50: 6465 7374 696e 6174 696f 6e20 6669 6c65  destination file
-00012a60: 2070 6174 682e 0a20 2020 2020 2020 2073   path..        s
-00012a70: 7263 5f6c 6179 6572 2028 7374 722c 206f  rc_layer (str, o
-00012a80: 7074 696f 6e61 6c29 3a20 5468 6520 736f  ptional): The so
-00012a90: 7572 6365 206c 6179 6572 2e20 4966 204e  urce layer. If N
-00012aa0: 6f6e 6520 616e 6420 7468 6572 6520 6973  one and there is
-00012ab0: 206f 6e6c 790a 2020 2020 2020 2020 2020   only.          
-00012ac0: 2020 6f6e 6520 6c61 7965 7220 696e 2074    one layer in t
-00012ad0: 6865 2073 7263 2066 696c 652c 2074 6861  he src file, tha
-00012ae0: 7420 6c61 7965 7220 6973 2074 616b 656e  t layer is taken
-00012af0: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00012b00: 6e65 2e0a 2020 2020 2020 2020 6473 745f  ne..        dst_
-00012b10: 6c61 7965 7220 2873 7472 2c20 6f70 7469  layer (str, opti
-00012b20: 6f6e 616c 293a 2054 6865 2064 6573 7469  onal): The desti
-00012b30: 6e61 7469 6f6e 206c 6179 6572 2e20 4966  nation layer. If
-00012b40: 204e 6f6e 652c 2074 6865 2066 696c 650a   None, the file.
-00012b50: 2020 2020 2020 2020 2020 2020 7374 656d              stem
-00012b60: 2069 7320 7461 6b65 6e20 6173 206c 6179   is taken as lay
-00012b70: 6572 206e 616d 652e 2044 6566 6175 6c74  er name. Default
-00012b80: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-00012b90: 2020 2073 7263 5f63 7273 2028 556e 696f     src_crs (Unio
-00012ba0: 6e5b 7374 722c 2069 6e74 5d2c 206f 7074  n[str, int], opt
-00012bb0: 696f 6e61 6c29 3a20 616e 2065 7073 6720  ional): an epsg 
-00012bc0: 696e 7420 6f72 2061 6e79 7468 696e 6720  int or anything 
-00012bd0: 7375 7070 6f72 7465 640a 2020 2020 2020  supported.      
-00012be0: 2020 2020 2020 6279 2074 6865 204f 4752        by the OGR
-00012bf0: 5370 6174 6961 6c52 6566 6572 656e 6365  SpatialReference
-00012c00: 2e53 6574 4672 6f6d 5573 6572 496e 7075  .SetFromUserInpu
-00012c10: 7428 2920 6361 6c6c 2c20 7768 6963 6820  t() call, which 
-00012c20: 696e 636c 7564 6573 0a20 2020 2020 2020  includes.       
-00012c30: 2020 2020 2061 6e20 4550 5347 2073 7472       an EPSG str
-00012c40: 696e 6720 2865 672e 2022 4550 5347 3a34  ing (eg. "EPSG:4
-00012c50: 3332 3622 292c 2061 2077 656c 6c20 6b6e  326"), a well kn
-00012c60: 6f77 6e20 7465 7874 2028 574b 5429 2043  own text (WKT) C
-00012c70: 5253 0a20 2020 2020 2020 2020 2020 2064  RS.            d
-00012c80: 6566 696e 6974 696f 6e2c 2e2e 2e20 4465  efinition,... De
-00012c90: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-00012ca0: 2020 2020 2020 2020 6473 745f 6372 7320          dst_crs 
-00012cb0: 2855 6e69 6f6e 5b73 7472 2c20 696e 745d  (Union[str, int]
-00012cc0: 2c20 6f70 7469 6f6e 616c 293a 2061 6e20  , optional): an 
-00012cd0: 6570 7367 2069 6e74 206f 7220 616e 7974  epsg int or anyt
-00012ce0: 6869 6e67 2073 7570 706f 7274 6564 0a20  hing supported. 
-00012cf0: 2020 2020 2020 2020 2020 2062 7920 7468             by th
-00012d00: 6520 4f47 5253 7061 7469 616c 5265 6665  e OGRSpatialRefe
-00012d10: 7265 6e63 652e 5365 7446 726f 6d55 7365  rence.SetFromUse
-00012d20: 7249 6e70 7574 2829 2063 616c 6c2c 2077  rInput() call, w
-00012d30: 6869 6368 2069 6e63 6c75 6465 730a 2020  hich includes.  
-00012d40: 2020 2020 2020 2020 2020 616e 2045 5053            an EPS
-00012d50: 4720 7374 7269 6e67 2028 6567 2e20 2245  G string (eg. "E
-00012d60: 5053 473a 3433 3236 2229 2c20 6120 7765  PSG:4326"), a we
-00012d70: 6c6c 206b 6e6f 776e 2074 6578 7420 2857  ll known text (W
-00012d80: 4b54 2920 4352 530a 2020 2020 2020 2020  KT) CRS.        
-00012d90: 2020 2020 6465 6669 6e69 7469 6f6e 2c2e      definition,.
-00012da0: 2e2e 2044 6566 6175 6c74 7320 746f 204e  .. Defaults to N
-00012db0: 6f6e 652e 0a20 2020 2020 2020 2072 6570  one..        rep
-00012dc0: 726f 6a65 6374 2028 626f 6f6c 2c20 6f70  roject (bool, op
-00012dd0: 7469 6f6e 616c 293a 2054 7275 6520 746f  tional): True to
-00012de0: 2072 6570 726f 6a65 6374 2077 6869 6c65   reproject while
-00012df0: 2063 6f6e 7665 7274 696e 6720 7468 650a   converting the.
-00012e00: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00012e10: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
-00012e20: 6c73 652e 0a20 2020 2020 2020 2065 7870  lse..        exp
-00012e30: 6c6f 6465 636f 6c6c 6563 7469 6f6e 7320  lodecollections 
-00012e40: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
-00012e50: 3a20 5472 7565 2074 6f20 6f75 7470 7574  : True to output
-00012e60: 206f 6e6c 7920 7369 6d70 6c65 0a20 2020   only simple.   
-00012e70: 2020 2020 2020 2020 2067 656f 6d65 7472           geometr
-00012e80: 6965 732e 2044 6566 6175 6c74 7320 746f  ies. Defaults to
-00012e90: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00012ea0: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
-00012eb0: 6d65 7472 7974 7970 6520 2855 6e69 6f6e  metrytype (Union
-00012ec0: 5b47 656f 6d65 7472 7954 7970 652c 2073  [GeometryType, s
-00012ed0: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
-00012ee0: 4765 6f6d 6574 7279 2074 7970 652e 0a20  Geometry type.. 
-00012ef0: 2020 2020 2020 2020 2020 2074 6f20 2874             to (t
-00012f00: 7279 2074 6f29 2066 6f72 6365 2074 6865  ry to) force the
-00012f10: 206f 7574 7075 7420 746f 2e20 4465 6661   output to. Defa
-00012f20: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-00012f30: 2020 2020 2020 6372 6561 7465 5f73 7061        create_spa
-00012f40: 7469 616c 5f69 6e64 6578 2028 626f 6f6c  tial_index (bool
-00012f50: 2c20 6f70 7469 6f6e 616c 293a 2054 7275  , optional): Tru
-00012f60: 6520 746f 2063 7265 6174 6520 6120 7370  e to create a sp
-00012f70: 6174 6961 6c20 696e 6465 780a 2020 2020  atial index.    
-00012f80: 2020 2020 2020 2020 6f6e 2074 6865 2064          on the d
-00012f90: 6573 7469 6e61 7469 6f6e 2066 696c 652f  estination file/
-00012fa0: 6c61 7965 722e 2049 6620 4e6f 6e65 2c20  layer. If None, 
-00012fb0: 7468 6520 6465 6661 756c 7420 6265 6861  the default beha
-00012fc0: 7669 6f75 7220 6279 2067 6461 6c20 666f  viour by gdal fo
-00012fd0: 720a 2020 2020 2020 2020 2020 2020 7468  r.            th
-00012fe0: 6174 2066 696c 6520 7479 7065 2069 7320  at file type is 
-00012ff0: 7265 7370 6563 7465 642e 2049 6620 7468  respected. If th
-00013000: 6520 4c41 5945 525f 4352 4541 5449 4f4e  e LAYER_CREATION
-00013010: 2e53 5041 5449 414c 5f49 4e44 4558 0a20  .SPATIAL_INDEX. 
-00013020: 2020 2020 2020 2020 2020 2070 6172 616d             param
-00013030: 6574 6572 2069 7320 7370 6563 6966 6965  eter is specifie
-00013040: 6420 696e 206f 7074 696f 6e73 2c20 6372  d in options, cr
-00013050: 6561 7465 5f73 7061 7469 616c 5f69 6e64  eate_spatial_ind
-00013060: 6578 2069 7320 6967 6e6f 7265 642e 0a20  ex is ignored.. 
-00013070: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00013080: 6c74 7320 746f 2054 7275 652e 0a20 2020  lts to True..   
-00013090: 2020 2020 2070 7265 7365 7276 655f 6669       preserve_fi
-000130a0: 6420 2862 6f6f 6c2c 206f 7074 696f 6e61  d (bool, optiona
-000130b0: 6c29 3a20 5472 7565 2074 6f20 6d61 6b65  l): True to make
-000130c0: 2061 6e20 6578 7472 6120 6566 666f 7274   an extra effort
-000130d0: 2074 6f20 7072 6573 6572 7665 2066 6964   to preserve fid
-000130e0: 2773 206f 660a 2020 2020 2020 2020 2020  's of.          
-000130f0: 2020 7468 6520 736f 7572 6365 206c 6179    the source lay
-00013100: 6572 2074 6f20 7468 6520 6465 7374 696e  er to the destin
-00013110: 6174 696f 6e20 6c61 7965 722e 2046 616c  ation layer. Fal
-00013120: 7365 206e 6f74 2074 6f20 646f 2061 6e79  se not to do any
-00013130: 2065 6666 6f72 742e 204e 6f6e 650a 2020   effort. None.  
-00013140: 2020 2020 2020 2020 2020 746f 2075 7365            to use
-00013150: 2074 6865 2064 6566 6175 6c74 2062 6568   the default beh
-00013160: 6176 696f 7572 206f 6620 6764 616c 2c20  aviour of gdal, 
-00013170: 7468 6174 2061 6c72 6561 6479 2070 7265  that already pre
-00013180: 7365 7276 6573 2069 6e20 736f 6d65 2063  serves in some c
-00013190: 6173 6573 2e0a 2020 2020 2020 2020 2020  ases..          
-000131a0: 2020 536f 6d65 2066 696c 6520 666f 726d    Some file form
-000131b0: 6174 7320 646f 6e27 7420 6578 706c 6963  ats don't explic
-000131c0: 6974 6c79 2073 746f 7265 2074 6865 2066  itly store the f
-000131d0: 6964 2028 652e 672e 2073 6861 7065 6669  id (e.g. shapefi
-000131e0: 6c65 292c 2073 6f20 7468 6579 0a20 2020  le), so they.   
-000131f0: 2020 2020 2020 2020 2077 696c 6c20 6e65           will ne
-00013200: 7665 7220 6265 2061 626c 6520 746f 2070  ver be able to p
-00013210: 7265 7365 7276 6520 6669 6473 2e20 4465  reserve fids. De
-00013220: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-00013230: 2020 2020 2020 2020 6f70 7469 6f6e 7320          options 
-00013240: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
-00013250: 3a20 6f70 7469 6f6e 7320 746f 2070 6173  : options to pas
-00013260: 7320 746f 2067 6461 6c2e 0a20 2020 2020  s to gdal..     
-00013270: 2020 2061 7070 656e 6420 2862 6f6f 6c2c     append (bool,
-00013280: 206f 7074 696f 6e61 6c29 3a20 5472 7565   optional): True
-00013290: 2074 6f20 6170 7065 6e64 2074 6f20 7468   to append to th
-000132a0: 6520 6f75 7470 7574 2066 696c 6520 6966  e output file if
-000132b0: 2069 7420 6578 6973 7473 2e0a 2020 2020   it exists..    
-000132c0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-000132d0: 2074 6f20 4661 6c73 652e 0a20 2020 2020   to False..     
-000132e0: 2020 2066 6f72 6365 2028 626f 6f6c 2c20     force (bool, 
-000132f0: 6f70 7469 6f6e 616c 293a 206f 7665 7277  optional): overw
-00013300: 7269 7465 2065 7869 7374 696e 6720 6f75  rite existing ou
-00013310: 7470 7574 2066 696c 6528 7329 0a20 2020  tput file(s).   
-00013320: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00013330: 7320 746f 2046 616c 7365 2e0a 2020 2020  s to False..    
-00013340: 2222 220a 2020 2020 2320 496e 6974 0a20  """.    # Init. 
-00013350: 2020 2073 7263 203d 2050 6174 6828 7372     src = Path(sr
-00013360: 6329 0a20 2020 2064 7374 203d 2050 6174  c).    dst = Pat
-00013370: 6828 6473 7429 0a0a 2020 2020 2320 4966  h(dst)..    # If
-00013380: 2073 6f75 7263 6520 6669 6c65 2064 6f65   source file doe
-00013390: 736e 2774 2065 7869 7374 2c20 7261 6973  sn't exist, rais
-000133a0: 6520 6572 726f 720a 2020 2020 6966 206e  e error.    if n
-000133b0: 6f74 2073 7263 2e65 7869 7374 7328 293a  ot src.exists():
-000133c0: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-000133d0: 616c 7565 4572 726f 7228 6622 7372 6320  alueError(f"src 
-000133e0: 6669 6c65 2064 6f65 736e 2774 2065 7869  file doesn't exi
-000133f0: 7374 3a20 7b73 7263 7d22 290a 2020 2020  st: {src}").    
-00013400: 2320 4966 2064 6573 7420 6669 6c65 2065  # If dest file e
-00013410: 7869 7374 7320 616c 7265 6164 792c 2072  xists already, r
-00013420: 656d 6f76 6520 6974 0a20 2020 2069 6620  emove it.    if 
-00013430: 6e6f 7420 6170 7065 6e64 2061 6e64 2064  not append and d
-00013440: 7374 2e65 7869 7374 7328 293a 0a20 2020  st.exists():.   
-00013450: 2020 2020 2069 6620 666f 7263 6520 6973       if force is
-00013460: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
-00013470: 2020 2072 656d 6f76 6528 6473 7429 0a20     remove(dst). 
-00013480: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00013490: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000134a0: 696e 666f 2866 224f 7574 7075 7420 6669  info(f"Output fi
-000134b0: 6c65 2065 7869 7374 7320 616c 7265 6164  le exists alread
-000134c0: 792c 2073 6f20 7374 6f70 3a20 7b64 7374  y, so stop: {dst
-000134d0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-000134e0: 7265 7475 726e 0a0a 2020 2020 2320 436f  return..    # Co
-000134f0: 6e76 6572 740a 2020 2020 6c6f 6767 6572  nvert.    logger
-00013500: 2e69 6e66 6f28 6622 436f 6e76 6572 7420  .info(f"Convert 
-00013510: 7b73 7263 7d20 746f 207b 6473 747d 2229  {src} to {dst}")
-00013520: 0a20 2020 205f 6170 7065 6e64 5f74 6f5f  .    _append_to_
-00013530: 6e6f 6c6f 636b 280a 2020 2020 2020 2020  nolock(.        
-00013540: 7372 632c 0a20 2020 2020 2020 2064 7374  src,.        dst
-00013550: 2c0a 2020 2020 2020 2020 7372 635f 6c61  ,.        src_la
-00013560: 7965 722c 0a20 2020 2020 2020 2064 7374  yer,.        dst
-00013570: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
-00013580: 7372 635f 6372 733d 7372 635f 6372 732c  src_crs=src_crs,
-00013590: 0a20 2020 2020 2020 2064 7374 5f63 7273  .        dst_crs
-000135a0: 3d64 7374 5f63 7273 2c0a 2020 2020 2020  =dst_crs,.      
-000135b0: 2020 7265 7072 6f6a 6563 743d 7265 7072    reproject=repr
-000135c0: 6f6a 6563 742c 0a20 2020 2020 2020 2065  oject,.        e
-000135d0: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
-000135e0: 733d 6578 706c 6f64 6563 6f6c 6c65 6374  s=explodecollect
-000135f0: 696f 6e73 2c0a 2020 2020 2020 2020 666f  ions,.        fo
-00013600: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
-00013610: 7472 7974 7970 653d 666f 7263 655f 6f75  trytype=force_ou
-00013620: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-00013630: 652c 0a20 2020 2020 2020 2063 7265 6174  e,.        creat
-00013640: 655f 7370 6174 6961 6c5f 696e 6465 783d  e_spatial_index=
-00013650: 6372 6561 7465 5f73 7061 7469 616c 5f69  create_spatial_i
-00013660: 6e64 6578 2c0a 2020 2020 2020 2020 7072  ndex,.        pr
-00013670: 6573 6572 7665 5f66 6964 3d70 7265 7365  eserve_fid=prese
-00013680: 7276 655f 6669 642c 0a20 2020 2020 2020  rve_fid,.       
-00013690: 206f 7074 696f 6e73 3d6f 7074 696f 6e73   options=options
-000136a0: 2c0a 2020 2020 290a 0a0a 6465 6620 5f6c  ,.    )...def _l
-000136b0: 6175 6e64 6572 5f63 6f6c 756d 6e5f 6e61  aunder_column_na
-000136c0: 6d65 7328 636f 6c75 6d6e 733a 2049 7465  mes(columns: Ite
-000136d0: 7261 626c 6529 202d 3e20 4c69 7374 5b54  rable) -> List[T
-000136e0: 7570 6c65 5b73 7472 2c20 7374 725d 5d3a  uple[str, str]]:
-000136f0: 0a20 2020 2022 2222 0a20 2020 204c 6175  .    """.    Lau
-00013700: 6e64 6572 7320 7468 6520 636f 6c75 6d6e  nders the column
-00013710: 206e 616d 6573 2070 6173 7365 6420 746f   names passed to
-00013720: 2063 6f6d 706c 7920 7769 7468 2073 6861   comply with sha
-00013730: 7065 6669 6c65 2072 6573 7472 6963 7469  pefile restricti
-00013740: 6f6e 732e 0a0a 2020 2020 5261 7469 6f6e  ons...    Ration
-00013750: 616c 653a 206e 6f72 6d61 6c6c 7920 6764  ale: normally gd
-00013760: 616c 206c 6175 6e64 6572 7320 7468 656d  al launders them
-00013770: 2069 6620 6e65 6564 6564 2c20 6275 7420   if needed, but 
-00013780: 7768 656e 2079 6f75 2061 7070 656e 640a  when you append.
-00013790: 2020 2020 6d75 6c74 6970 6c65 2066 696c      multiple fil
-000137a0: 6573 2074 6f20 6120 7368 6170 6566 696c  es to a shapefil
-000137b0: 6520 7769 7468 2063 6f6c 756d 6e73 2074  e with columns t
-000137c0: 6861 7420 6e65 6564 2074 6f20 6265 206c  hat need to be l
-000137d0: 6175 6e64 6572 6564 0a20 2020 2074 6865  aundered.    the
-000137e0: 7920 6172 6520 6e6f 7420 6d61 7463 6865  y are not matche
-000137f0: 6420 616e 6420 736f 2061 7265 2061 7070  d and so are app
-00013800: 656e 6465 6420 7769 7468 204e 554c 4c20  ended with NULL 
-00013810: 7661 6c75 6573 2066 6f72 2074 6865 7365  values for these
-00013820: 0a20 2020 2063 6f6c 756d 6e73 2e20 4e6f  .    columns. No
-00013830: 726d 616c 6c79 2074 6865 202d 7265 6c61  rmally the -rela
-00013840: 7865 6446 6965 6c64 4e61 6d65 4d61 7463  xedFieldNameMatc
-00013850: 6820 7061 7261 6d65 7465 7220 696e 206f  h parameter in o
-00013860: 6772 326f 6772 0a20 2020 2073 686f 756c  gr2ogr.    shoul
-00013870: 6420 6669 7820 7468 6973 2c20 6275 7420  d fix this, but 
-00013880: 6974 2073 6565 6d73 2074 6861 7420 7468  it seems that th
-00013890: 6973 2069 736e 2774 2073 7570 706f 7274  is isn't support
-000138a0: 6564 2066 6f72 2073 6861 7065 6669 6c65  ed for shapefile
-000138b0: 732e 0a0a 2020 2020 4c61 756e 6465 7269  s...    Launderi
-000138c0: 6e67 2069 7320 6261 7365 6420 6f6e 2074  ng is based on t
-000138d0: 6869 7320 7465 7874 2066 726f 6d20 7468  his text from th
-000138e0: 6520 6764 616c 2073 6861 7065 6669 6c65  e gdal shapefile
-000138f0: 2064 7269 7665 720a 2020 2020 646f 6375   driver.    docu
-00013900: 6d65 6e74 6174 696f 6e3a 0a0a 2020 2020  mentation:..    
-00013910: 5368 6170 6566 696c 6520 6665 6174 7572  Shapefile featur
-00013920: 6520 6174 7472 6962 7574 6573 2061 7265  e attributes are
-00013930: 2073 746f 7265 6420 696e 2061 6e20 6173   stored in an as
-00013940: 736f 6369 6174 6564 202e 6462 6620 6669  sociated .dbf fi
-00013950: 6c65 2c20 616e 640a 2020 2020 736f 2061  le, and.    so a
-00013960: 7474 7269 6275 7465 7320 7375 6666 6572  ttributes suffer
-00013970: 2061 206e 756d 6265 7220 6f66 206c 696d   a number of lim
-00013980: 6974 6174 696f 6e73 3a0a 2020 2020 2d20  itations:.    - 
-00013990: 2020 4174 7472 6962 7574 6520 6e61 6d65    Attribute name
-000139a0: 7320 6361 6e20 6f6e 6c79 2062 6520 7570  s can only be up
-000139b0: 2074 6f20 3130 2063 6861 7261 6374 6572   to 10 character
-000139c0: 7320 6c6f 6e67 2e0a 2020 2020 2020 2020  s long..        
-000139d0: 5468 6520 4f47 5220 5368 6170 6566 696c  The OGR Shapefil
-000139e0: 6520 6472 6976 6572 2074 7269 6573 2074  e driver tries t
-000139f0: 6f20 6765 6e65 7261 7465 2075 6e69 7175  o generate uniqu
-00013a00: 6520 6669 656c 640a 2020 2020 2020 2020  e field.        
-00013a10: 6e61 6d65 732e 2053 7563 6365 7373 6976  names. Successiv
-00013a20: 6520 6475 706c 6963 6174 6520 6669 656c  e duplicate fiel
-00013a30: 6420 6e61 6d65 732c 2069 6e63 6c75 6469  d names, includi
-00013a40: 6e67 2074 686f 7365 2063 7265 6174 6564  ng those created
-00013a50: 2062 790a 2020 2020 2020 2020 7472 756e   by.        trun
-00013a60: 6361 7469 6f6e 2074 6f20 3130 2063 6861  cation to 10 cha
-00013a70: 7261 6374 6572 732c 2077 696c 6c20 6265  racters, will be
-00013a80: 2074 7275 6e63 6174 6564 2074 6f20 3820   truncated to 8 
-00013a90: 6368 6172 6163 7465 7273 2061 6e64 0a20  characters and. 
-00013aa0: 2020 2020 2020 2061 7070 656e 6465 6420         appended 
-00013ab0: 7769 7468 2061 2073 6572 6961 6c20 6e75  with a serial nu
-00013ac0: 6d62 6572 2066 726f 6d20 3120 746f 2039  mber from 1 to 9
-00013ad0: 392e 0a0a 2020 2020 2020 2020 466f 7220  9...        For 
-00013ae0: 6578 616d 706c 653a 0a0a 2020 2020 2020  example:..      
-00013af0: 2020 2d20 2061 20e2 8692 2061 2c20 6120    -  a ... a, a 
-00013b00: e286 9220 615f 312c 2041 20e2 8692 2041  ... a_1, A ... A
-00013b10: 5f32 3b0a 2020 2020 2020 2020 2d20 2061  _2;.        -  a
-00013b20: 6263 6465 6667 6869 6a6b 20e2 8692 2061  bcdefghijk ... a
-00013b30: 6263 6465 6667 6869 6a2c 2061 6263 6465  bcdefghij, abcde
-00013b40: 6667 6869 6a6b 6c20 e286 9220 6162 6364  fghijkl ... abcd
-00013b50: 6566 6768 5f31 0a0a 2020 2020 2d20 2020  efgh_1..    -   
-00013b60: 4f6e 6c79 2049 6e74 6567 6572 2c20 496e  Only Integer, In
-00013b70: 7465 6765 7236 342c 2052 6561 6c2c 2053  teger64, Real, S
-00013b80: 7472 696e 6720 616e 6420 4461 7465 2028  tring and Date (
-00013b90: 6e6f 7420 4461 7465 5469 6d65 2c20 6a75  not DateTime, ju
-00013ba0: 7374 0a20 2020 2020 2020 2079 6561 722f  st.        year/
-00013bb0: 6d6f 6e74 682f 6461 7929 2066 6965 6c64  month/day) field
-00013bc0: 2074 7970 6573 2061 7265 2073 7570 706f   types are suppo
-00013bd0: 7274 6564 2e20 5468 6520 7661 7269 6f75  rted. The variou
-00013be0: 7320 6c69 7374 2c20 616e 640a 2020 2020  s list, and.    
-00013bf0: 2020 2020 6269 6e61 7279 2066 6965 6c64      binary field
-00013c00: 2074 7970 6573 2063 616e 6e6f 7420 6265   types cannot be
-00013c10: 2063 7265 6174 6564 2e0a 2020 2020 2d20   created..    - 
-00013c20: 2020 5468 6520 6669 656c 6420 7769 6474    The field widt
-00013c30: 6820 616e 6420 7072 6563 6973 696f 6e20  h and precision 
-00013c40: 6172 6520 6469 7265 6374 6c79 2075 7365  are directly use
-00013c50: 6420 746f 2065 7374 6162 6c69 7368 2073  d to establish s
-00013c60: 746f 7261 6765 0a20 2020 2020 2020 2073  torage.        s
-00013c70: 697a 6520 696e 2074 6865 202e 6462 6620  ize in the .dbf 
-00013c80: 6669 6c65 2e20 5468 6973 206d 6561 6e73  file. This means
-00013c90: 2074 6861 7420 7374 7269 6e67 7320 6c6f   that strings lo
-00013ca0: 6e67 6572 2074 6861 6e20 7468 6520 6669  nger than the fi
-00013cb0: 656c 640a 2020 2020 2020 2020 7769 6474  eld.        widt
-00013cc0: 682c 206f 7220 6e75 6d62 6572 7320 7468  h, or numbers th
-00013cd0: 6174 2064 6f6e 2774 2066 6974 2069 6e74  at don't fit int
-00013ce0: 6f20 7468 6520 696e 6469 6361 7465 6420  o the indicated 
-00013cf0: 6669 656c 6420 666f 726d 6174 2077 696c  field format wil
-00013d00: 6c0a 2020 2020 2020 2020 7375 6666 6572  l.        suffer
-00013d10: 2074 7275 6e63 6174 696f 6e2e 0a20 2020   truncation..   
-00013d20: 202d 2020 2049 6e74 6567 6572 2066 6965   -   Integer fie
-00013d30: 6c64 7320 7769 7468 6f75 7420 616e 2065  lds without an e
-00013d40: 7870 6c69 6369 7420 7769 6474 6820 6172  xplicit width ar
-00013d50: 6520 7472 6561 7465 6420 6173 2077 6964  e treated as wid
-00013d60: 7468 2039 2c20 616e 640a 2020 2020 2020  th 9, and.      
-00013d70: 2020 6578 7465 6e64 6564 2074 6f20 3130    extended to 10
-00013d80: 206f 7220 3131 2069 6620 6e65 6564 6564   or 11 if needed
-00013d90: 2e0a 2020 2020 2d20 2020 496e 7465 6765  ..    -   Intege
-00013da0: 7236 3420 6669 656c 6473 2077 6974 686f  r64 fields witho
-00013db0: 7574 2061 6e20 6578 706c 6963 6974 2077  ut an explicit w
-00013dc0: 6964 7468 2061 7265 2074 7265 6174 6564  idth are treated
-00013dd0: 2061 7320 7769 6474 6820 3138 2c0a 2020   as width 18,.  
-00013de0: 2020 2020 2020 616e 6420 6578 7465 6e64        and extend
-00013df0: 6564 2074 6f20 3139 206f 7220 3230 2069  ed to 19 or 20 i
-00013e00: 6620 6e65 6564 6564 2e0a 2020 2020 2d20  f needed..    - 
-00013e10: 2020 5265 616c 2028 666c 6f61 7469 6e67    Real (floating
-00013e20: 2070 6f69 6e74 2920 6669 656c 6473 2077   point) fields w
-00013e30: 6974 686f 7574 2061 6e20 6578 706c 6963  ithout an explic
-00013e40: 6974 2077 6964 7468 2061 7265 2074 7265  it width are tre
-00013e50: 6174 6564 2061 730a 2020 2020 2020 2020  ated as.        
-00013e60: 7769 6474 6820 3234 2077 6974 6820 3135  width 24 with 15
-00013e70: 2064 6563 696d 616c 2070 6c61 6365 7320   decimal places 
-00013e80: 6f66 2070 7265 6369 7369 6f6e 2e0a 2020  of precision..  
-00013e90: 2020 2d20 2020 5374 7269 6e67 2066 6965    -   String fie
-00013ea0: 6c64 7320 7769 7468 6f75 7420 616e 2061  lds without an a
-00013eb0: 7373 6967 6e65 6420 7769 6474 6820 6172  ssigned width ar
-00013ec0: 6520 7472 6561 7465 6420 6173 2038 3020  e treated as 80 
-00013ed0: 6368 6172 6163 7465 7273 2e0a 0a20 2020  characters...   
-00013ee0: 2041 7267 733a 0a20 2020 2020 2020 2063   Args:.        c
-00013ef0: 6f6c 756d 6e73 2028 4974 6572 6162 6c65  olumns (Iterable
-00013f00: 293a 2074 6865 2063 6f6c 756d 6e73 2074  ): the columns t
-00013f10: 6f20 6c61 756e 6465 722e 0a0a 2020 2020  o launder...    
-00013f20: 5265 7475 726e 733a 2061 204c 6973 7420  Returns: a List 
-00013f30: 6f66 2074 7570 706c 6573 2077 6974 6820  of tupples with 
-00013f40: 7468 6520 6f72 6967 696e 616c 2061 6e64  the original and
-00013f50: 206c 6175 6e64 6572 6564 2063 6f6c 756d   laundered colum
-00013f60: 6e20 6e61 6d65 732e 0a20 2020 2022 2222  n names..    """
-00013f70: 0a20 2020 206c 6175 6e64 6572 6564 203d  .    laundered =
-00013f80: 205b 5d0a 2020 2020 6c61 756e 6465 7265   [].    laundere
-00013f90: 645f 7570 7065 7220 3d20 5b5d 0a20 2020  d_upper = [].   
-00013fa0: 2066 6f72 2063 6f6c 756d 6e20 696e 2063   for column in c
-00013fb0: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
-00013fc0: 2320 446f 7562 6c65 7320 696e 2063 6173  # Doubles in cas
-00013fd0: 696e 6720 6172 6565 206e 6f74 2061 6c6c  ing aree not all
-00013fe0: 6f77 6564 2065 6974 6865 720a 2020 2020  owed either.    
-00013ff0: 2020 2020 6966 206c 656e 2863 6f6c 756d      if len(colum
-00014000: 6e29 203c 3d20 3130 3a0a 2020 2020 2020  n) <= 10:.      
-00014010: 2020 2020 2020 6966 2063 6f6c 756d 6e2e        if column.
-00014020: 7570 7065 7228 2920 6e6f 7420 696e 206c  upper() not in l
-00014030: 6175 6e64 6572 6564 5f75 7070 6572 3a0a  aundered_upper:.
-00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014050: 6c61 756e 6465 7265 645f 7570 7065 722e  laundered_upper.
-00014060: 6170 7065 6e64 2863 6f6c 756d 6e2e 7570  append(column.up
-00014070: 7065 7228 2929 0a20 2020 2020 2020 2020  per()).         
-00014080: 2020 2020 2020 206c 6175 6e64 6572 6564         laundered
-00014090: 2e61 7070 656e 6428 2863 6f6c 756d 6e2c  .append((column,
-000140a0: 2063 6f6c 756d 6e29 290a 2020 2020 2020   column)).      
-000140b0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-000140c0: 7565 0a0a 2020 2020 2020 2020 2320 4c61  ue..        # La
-000140d0: 756e 6465 7269 6e67 2069 7320 6e65 6564  undering is need
-000140e0: 6564 0a20 2020 2020 2020 2063 6f6c 756d  ed.        colum
-000140f0: 6e5f 6c61 756e 6465 7265 6420 3d20 636f  n_laundered = co
-00014100: 6c75 6d6e 5b3a 3130 5d0a 2020 2020 2020  lumn[:10].      
-00014110: 2020 6966 2063 6f6c 756d 6e5f 6c61 756e    if column_laun
-00014120: 6465 7265 642e 7570 7065 7228 2920 6e6f  dered.upper() no
-00014130: 7420 696e 206c 6175 6e64 6572 6564 5f75  t in laundered_u
-00014140: 7070 6572 3a0a 2020 2020 2020 2020 2020  pper:.          
-00014150: 2020 6c61 756e 6465 7265 645f 7570 7065    laundered_uppe
-00014160: 722e 6170 7065 6e64 2863 6f6c 756d 6e5f  r.append(column_
-00014170: 6c61 756e 6465 7265 642e 7570 7065 7228  laundered.upper(
-00014180: 2929 0a20 2020 2020 2020 2020 2020 206c  )).            l
-00014190: 6175 6e64 6572 6564 2e61 7070 656e 6428  aundered.append(
-000141a0: 2863 6f6c 756d 6e2c 2063 6f6c 756d 6e5f  (column, column_
-000141b0: 6c61 756e 6465 7265 6429 290a 2020 2020  laundered)).    
-000141c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000141d0: 2020 2020 2020 2320 4a75 7374 2074 616b        # Just tak
-000141e0: 696e 6720 6669 7273 7420 3130 2063 6861  ing first 10 cha
-000141f0: 7261 6374 6572 7320 6469 646e 2774 2068  racters didn't h
-00014200: 656c 700a 2020 2020 2020 2020 2020 2020  elp.            
-00014210: 666f 7220 696e 6465 7820 696e 2072 616e  for index in ran
-00014220: 6765 2831 2c20 3130 3129 3a0a 2020 2020  ge(1, 101):.    
-00014230: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00014240: 6e64 6578 203e 3d20 3130 303a 0a20 2020  ndex >= 100:.   
-00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-00014270: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
-00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014290: 2020 2020 224e 6f74 2073 7570 706f 7274      "Not support
-000142a0: 6564 2074 6f20 6c61 756e 6465 7220 3e20  ed to launder > 
-000142b0: 3939 2063 6f6c 756d 6e73 2073 7461 7274  99 columns start
-000142c0: 696e 6720 220a 2020 2020 2020 2020 2020  ing ".          
-000142d0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000142e0: 7769 7468 207b 636f 6c75 6d6e 5f6c 6175  with {column_lau
-000142f0: 6e64 6572 6564 5b3a 385d 7d22 0a20 2020  ndered[:8]}".   
-00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014310: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00014320: 2020 2069 6620 696e 6465 7820 3c3d 2039     if index <= 9
-00014330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014340: 2020 2020 2020 636f 6c75 6d6e 5f6c 6175        column_lau
-00014350: 6e64 6572 6564 203d 2066 227b 636f 6c75  ndered = f"{colu
-00014360: 6d6e 5f6c 6175 6e64 6572 6564 5b3a 385d  mn_laundered[:8]
-00014370: 7d5f 7b69 6e64 6578 7d22 0a20 2020 2020  }_{index}".     
-00014380: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00014390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000143a0: 2020 2020 2063 6f6c 756d 6e5f 6c61 756e       column_laun
-000143b0: 6465 7265 6420 3d20 6622 7b63 6f6c 756d  dered = f"{colum
-000143c0: 6e5f 6c61 756e 6465 7265 645b 3a38 5d7d  n_laundered[:8]}
-000143d0: 7b69 6e64 6578 7d22 0a20 2020 2020 2020  {index}".       
-000143e0: 2020 2020 2020 2020 2069 6620 636f 6c75           if colu
-000143f0: 6d6e 5f6c 6175 6e64 6572 6564 2e75 7070  mn_laundered.upp
-00014400: 6572 2829 206e 6f74 2069 6e20 6c61 756e  er() not in laun
-00014410: 6465 7265 645f 7570 7065 723a 0a20 2020  dered_upper:.   
-00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014430: 206c 6175 6e64 6572 6564 5f75 7070 6572   laundered_upper
-00014440: 2e61 7070 656e 6428 636f 6c75 6d6e 5f6c  .append(column_l
-00014450: 6175 6e64 6572 6564 2e75 7070 6572 2829  aundered.upper()
-00014460: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014470: 2020 2020 2020 6c61 756e 6465 7265 642e        laundered.
-00014480: 6170 7065 6e64 2828 636f 6c75 6d6e 2c20  append((column, 
-00014490: 636f 6c75 6d6e 5f6c 6175 6e64 6572 6564  column_laundered
-000144a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-000144b0: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
-000144c0: 2020 7265 7475 726e 206c 6175 6e64 6572    return launder
-000144d0: 6564 0a                                  ed.
+0000e630: 6372 6561 7465 5f73 7061 7469 616c 5f69  create_spatial_i
+0000e640: 6e64 6578 3d63 7265 6174 655f 7370 6174  ndex=create_spat
+0000e650: 6961 6c5f 696e 6465 782c 0a20 2020 2020  ial_index,.     
+0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e670: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000e680: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6a0: 2020 2020 2020 2023 2049 6620 6764 6620         # If gdf 
+0000e6b0: 7772 6974 7465 6e20 746f 2074 656d 7020  written to temp 
+0000e6c0: 6669 6c65 2c20 7573 6520 6170 7065 6e64  file, use append
+0000e6d0: 5f74 6f5f 6e6f 6c6f 636b 202b 2063 6c65  _to_nolock + cle
+0000e6e0: 616e 7570 0a20 2020 2020 2020 2020 2020  anup.           
+0000e6f0: 2020 2020 2020 2020 2020 2020 205f 6170               _ap
+0000e700: 7065 6e64 5f74 6f5f 6e6f 6c6f 636b 280a  pend_to_nolock(.
+0000e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e720: 2020 2020 2020 2020 2020 2020 7372 633d              src=
+0000e730: 6764 6674 656d 705f 7061 7468 2c0a 2020  gdftemp_path,.  
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e750: 2020 2020 2020 2020 2020 6473 743d 7061            dst=pa
+0000e760: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e780: 6473 745f 6c61 7965 723d 6c61 7965 722c  dst_layer=layer,
+0000e790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e7a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000e7b0: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
+0000e7c0: 7279 7479 7065 3d66 6f72 6365 5f6f 7574  rytype=force_out
+0000e7d0: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
+0000e7e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+0000e800: 6561 7465 5f73 7061 7469 616c 5f69 6e64  eate_spatial_ind
+0000e810: 6578 3d63 7265 6174 655f 7370 6174 6961  ex=create_spatia
+0000e820: 6c5f 696e 6465 782c 0a20 2020 2020 2020  l_index,.       
+0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e840: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000e850: 2020 2020 2020 2020 2020 2072 656d 6f76             remov
+0000e860: 6528 6764 6674 656d 705f 7061 7468 290a  e(gdftemp_path).
+0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e880: 2020 2020 2020 2020 6966 2067 6466 7465          if gdfte
+0000e890: 6d70 5f6c 6f63 6b70 6174 6820 6973 206e  mp_lockpath is n
+0000e8a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8c0: 2020 2020 2067 6466 7465 6d70 5f6c 6f63       gdftemp_loc
+0000e8d0: 6b70 6174 682e 756e 6c69 6e6b 2829 0a20  kpath.unlink(). 
+0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000e8f0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0000e900: 6173 2065 783a 0a20 2020 2020 2020 2020  as ex:.         
+0000e910: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+0000e920: 7371 6c69 7465 206f 7574 7075 7420 6669  sqlite output fi
+0000e930: 6c65 206c 6f63 6b65 642c 2061 6c73 6f20  le locked, also 
+0000e940: 7265 7472 790a 2020 2020 2020 2020 2020  retry.          
+0000e950: 2020 2020 2020 2020 2020 6966 2067 656f            if geo
+0000e960: 6669 6c65 7479 7065 2e69 735f 7370 6174  filetype.is_spat
+0000e970: 6961 6c69 7465 5f62 6173 6564 2061 6e64  ialite_based and
+0000e980: 2073 7472 2865 7829 206e 6f74 2069 6e20   str(ex) not in 
+0000e990: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+0000e9a0: 2020 2020 2020 2020 2020 2264 6174 6162            "datab
+0000e9b0: 6173 6520 6973 206c 6f63 6b65 6422 2c0a  ase is locked",.
+0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9d0: 2020 2020 2020 2020 2261 7474 656d 7074          "attempt
+0000e9e0: 2074 6f20 7772 6974 6520 6120 7265 6164   to write a read
+0000e9f0: 6f6e 6c79 2064 6174 6162 6173 6522 2c0a  only database",.
+0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea10: 2020 2020 5d3a 0a20 2020 2020 2020 2020      ]:.         
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000ea30: 6169 7365 2065 780a 2020 2020 2020 2020  aise ex.        
+0000ea40: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
+0000ea50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea60: 2020 2020 2072 6561 6479 203d 2054 7275       ready = Tru
+0000ea70: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000ea80: 2020 2020 2020 6c6f 636b 6669 6c65 2e75        lockfile.u
+0000ea90: 6e6c 696e 6b28 290a 2020 2020 2020 2020  nlink().        
+0000eaa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000eab0: 2020 2020 2020 2020 2020 7469 6d65 5f77            time_w
+0000eac0: 6169 7469 6e67 203d 2028 6461 7465 7469  aiting = (dateti
+0000ead0: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
+0000eae0: 2920 2d20 7374 6172 745f 7469 6d65 292e  ) - start_time).
+0000eaf0: 746f 7461 6c5f 7365 636f 6e64 7328 290a  total_seconds().
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 6966 2074 696d 655f 7761 6974 696e 6720  if time_waiting 
+0000eb20: 3e20 6170 7065 6e64 5f74 696d 656f 7574  > append_timeout
+0000eb30: 5f73 3a0a 2020 2020 2020 2020 2020 2020  _s:.            
+0000eb40: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+0000eb50: 6e74 696d 6545 7272 6f72 280a 2020 2020  ntimeError(.    
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb70: 2020 2020 6622 746f 5f66 696c 6520 7469      f"to_file ti
+0000eb80: 6d65 6f75 7420 6f66 207b 6170 7065 6e64  meout of {append
+0000eb90: 5f74 696d 656f 7574 5f73 7d20 7265 6163  _timeout_s} reac
+0000eba0: 6865 642c 2073 746f 7020 6170 7065 6e64  hed, stop append
+0000ebb0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000ebc0: 2020 2020 2020 2020 2020 2066 2274 6f20             f"to 
+0000ebd0: 7b70 6174 687d 2122 0a20 2020 2020 2020  {path}!".       
+0000ebe0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+0000ebf0: 2020 2020 2020 2020 2020 2020 2320 536c              # Sl
+0000ec00: 6565 7020 666f 7220 6120 7365 636f 6e64  eep for a second
+0000ec10: 2062 6566 6f72 6520 7472 7969 6e67 2061   before trying a
+0000ec20: 6761 696e 0a20 2020 2020 2020 2020 2020  gain.           
+0000ec30: 2074 696d 652e 736c 6565 7028 3129 0a0a   time.sleep(1)..
+0000ec40: 0a64 6566 205f 746f 5f66 696c 655f 7079  .def _to_file_py
+0000ec50: 6f67 7269 6f28 0a20 2020 2067 6466 3a20  ogrio(.    gdf: 
+0000ec60: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
+0000ec70: 2c0a 2020 2020 7061 7468 3a20 5061 7468  ,.    path: Path
+0000ec80: 2c0a 2020 2020 6c61 7965 723a 2073 7472  ,.    layer: str
+0000ec90: 2c0a 2020 2020 666f 7263 655f 6f75 7470  ,.    force_outp
+0000eca0: 7574 5f67 656f 6d65 7472 7974 7970 653a  ut_geometrytype:
+0000ecb0: 2055 6e69 6f6e 5b47 656f 6d65 7472 7954   Union[GeometryT
+0000ecc0: 7970 652c 2073 7472 2c20 4e6f 6e65 5d20  ype, str, None] 
+0000ecd0: 3d20 4e6f 6e65 2c0a 2020 2020 666f 7263  = None,.    forc
+0000ece0: 655f 6d75 6c74 6974 7970 653a 2062 6f6f  e_multitype: boo
+0000ecf0: 6c20 3d20 4661 6c73 652c 0a20 2020 2061  l = False,.    a
+0000ed00: 7070 656e 643a 2062 6f6f 6c20 3d20 4661  ppend: bool = Fa
+0000ed10: 6c73 652c 0a20 2020 2061 7070 656e 645f  lse,.    append_
+0000ed20: 7469 6d65 6f75 745f 733a 2069 6e74 203d  timeout_s: int =
+0000ed30: 2036 3030 2c0a 2020 2020 696e 6465 783a   600,.    index:
+0000ed40: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+0000ed50: 3d20 4e6f 6e65 2c0a 2020 2020 6372 6561  = None,.    crea
+0000ed60: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
+0000ed70: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+0000ed80: 203d 2054 7275 652c 0a29 3a0a 2020 2020   = True,.):.    
+0000ed90: 2222 220a 2020 2020 5772 6974 6573 2061  """.    Writes a
+0000eda0: 2070 616e 6461 7320 6461 7461 6672 616d   pandas datafram
+0000edb0: 6520 746f 2066 696c 6520 7573 696e 6720  e to file using 
+0000edc0: 7079 6f67 7269 6f2e 0a0a 2020 2020 5265  pyogrio...    Re
+0000edd0: 6d61 726b 3a20 7468 6973 2066 756e 6374  mark: this funct
+0000ede0: 696f 6e20 6f6e 6c79 2073 7570 706f 7274  ion only support
+0000edf0: 7320 7772 6974 696e 6720 4765 6f44 6174  s writing GeoDat
+0000ee00: 6146 7261 6d65 7320 6174 2074 6865 206d  aFrames at the m
+0000ee10: 6f6d 656e 742e 0a20 2020 2022 2222 0a20  oment..    """. 
+0000ee20: 2020 2023 2050 7265 7061 7265 2061 7267     # Prepare arg
+0000ee30: 7320 666f 7220 7772 6974 655f 6461 7461  s for write_data
+0000ee40: 6672 616d 650a 2020 2020 6b77 6172 6773  frame.    kwargs
+0000ee50: 203d 207b 7d0a 2020 2020 6b77 6172 6773   = {}.    kwargs
+0000ee60: 5b22 656e 6769 6e65 225d 203d 2022 7079  ["engine"] = "py
+0000ee70: 6f67 7269 6f22 0a0a 2020 2020 2320 4368  ogrio"..    # Ch
+0000ee80: 6563 6b20 7570 6672 6f6e 7420 6966 2061  eck upfront if a
+0000ee90: 7070 656e 6420 6973 2067 6f69 6e67 2074  ppend is going t
+0000eea0: 6f20 776f 726b 2074 6f20 6769 7665 206e  o work to give n
+0000eeb0: 6963 6520 6572 726f 720a 2020 2020 6966  ice error.    if
+0000eec0: 2061 7070 656e 6420 6973 2054 7275 6520   append is True 
+0000eed0: 616e 6420 7061 7468 2e65 7869 7374 7328  and path.exists(
+0000eee0: 293a 0a20 2020 2020 2020 206b 7761 7267  ):.        kwarg
+0000eef0: 735b 2261 7070 656e 6422 5d20 3d20 5472  s["append"] = Tr
+0000ef00: 7565 0a20 2020 2020 2020 206c 6179 6572  ue.        layer
+0000ef10: 696e 666f 203d 2067 6574 5f6c 6179 6572  info = get_layer
+0000ef20: 696e 666f 2870 6174 682c 206c 6179 6572  info(path, layer
+0000ef30: 290a 2020 2020 2020 2020 6669 6c65 5f63  ).        file_c
+0000ef40: 6f6c 7320 3d20 5b63 6f6c 2e75 7070 6572  ols = [col.upper
+0000ef50: 2829 2066 6f72 2063 6f6c 2069 6e20 6c61  () for col in la
+0000ef60: 7965 7269 6e66 6f2e 636f 6c75 6d6e 735d  yerinfo.columns]
+0000ef70: 0a20 2020 2020 2020 2067 6466 5f63 6f6c  .        gdf_col
+0000ef80: 7320 3d20 5b63 6f6c 2e75 7070 6572 2829  s = [col.upper()
+0000ef90: 2066 6f72 2063 6f6c 2069 6e20 6764 662e   for col in gdf.
+0000efa0: 636f 6c75 6d6e 7320 6966 2063 6f6c 2021  columns if col !
+0000efb0: 3d20 6764 662e 6765 6f6d 6574 7279 2e6e  = gdf.geometry.n
+0000efc0: 616d 655d 0a20 2020 2020 2020 2069 6620  ame].        if 
+0000efd0: 6764 665f 636f 6c73 2021 3d20 6669 6c65  gdf_cols != file
+0000efe0: 5f63 6f6c 733a 0a20 2020 2020 2020 2020  _cols:.         
+0000eff0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000f000: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000f010: 2020 2020 2022 6465 7374 696e 6174 696f       "destinatio
+0000f020: 6e20 6c61 7965 7220 646f 6573 6e27 7420  n layer doesn't 
+0000f030: 6861 7665 2074 6865 2073 616d 6520 636f  have the same co
+0000f040: 6c75 6d6e 7320 6173 2067 6466 3a20 220a  lumns as gdf: ".
+0000f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f060: 6622 7b66 696c 655f 636f 6c73 7d20 7673  f"{file_cols} vs
+0000f070: 207b 6764 665f 636f 6c73 7d22 0a20 2020   {gdf_cols}".   
+0000f080: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000f090: 6966 2063 7265 6174 655f 7370 6174 6961  if create_spatia
+0000f0a0: 6c5f 696e 6465 7820 6973 206e 6f74 204e  l_index is not N
+0000f0b0: 6f6e 653a 0a20 2020 2020 2020 206b 7761  one:.        kwa
+0000f0c0: 7267 735b 2253 5041 5449 414c 5f49 4e44  rgs["SPATIAL_IND
+0000f0d0: 4558 225d 203d 2063 7265 6174 655f 7370  EX"] = create_sp
+0000f0e0: 6174 6961 6c5f 696e 6465 780a 2020 2020  atial_index.    
+0000f0f0: 6765 6f66 696c 6574 7970 6520 3d20 4765  geofiletype = Ge
+0000f100: 6f66 696c 6554 7970 6528 7061 7468 290a  ofileType(path).
+0000f110: 2020 2020 6b77 6172 6773 5b22 6472 6976      kwargs["driv
+0000f120: 6572 225d 203d 2067 656f 6669 6c65 7479  er"] = geofilety
+0000f130: 7065 2e6f 6772 6472 6976 6572 0a20 2020  pe.ogrdriver.   
+0000f140: 206b 7761 7267 735b 2269 6e64 6578 225d   kwargs["index"]
+0000f150: 203d 2069 6e64 6578 0a20 2020 2069 6620   = index.    if 
+0000f160: 6372 6561 7465 5f73 7061 7469 616c 5f69  create_spatial_i
+0000f170: 6e64 6578 2069 7320 6e6f 7420 4e6f 6e65  ndex is not None
+0000f180: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
+0000f190: 5b22 5350 4154 4941 4c5f 494e 4445 5822  ["SPATIAL_INDEX"
+0000f1a0: 5d20 3d20 6372 6561 7465 5f73 7061 7469  ] = create_spati
+0000f1b0: 616c 5f69 6e64 6578 0a20 2020 2069 6620  al_index.    if 
+0000f1c0: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
+0000f1d0: 6d65 7472 7974 7970 6520 6973 206e 6f74  metrytype is not
+0000f1e0: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+0000f1f0: 6620 6973 696e 7374 616e 6365 2866 6f72  f isinstance(for
+0000f200: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
+0000f210: 7279 7479 7065 2c20 4765 6f6d 6574 7279  rytype, Geometry
+0000f220: 5479 7065 293a 0a20 2020 2020 2020 2020  Type):.         
+0000f230: 2020 2066 6f72 6365 5f6f 7574 7075 745f     force_output_
+0000f240: 6765 6f6d 6574 7279 7479 7065 203d 2066  geometrytype = f
+0000f250: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
+0000f260: 6574 7279 7479 7065 2e6e 616d 655f 6361  etrytype.name_ca
+0000f270: 6d65 6c63 6173 650a 2020 2020 2020 2020  melcase.        
+0000f280: 6b77 6172 6773 5b22 6765 6f6d 6574 7279  kwargs["geometry
+0000f290: 5f74 7970 6522 5d20 3d20 666f 7263 655f  _type"] = force_
+0000f2a0: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
+0000f2b0: 7970 650a 2020 2020 6966 2066 6f72 6365  ype.    if force
+0000f2c0: 5f6d 756c 7469 7479 7065 3a0a 2020 2020  _multitype:.    
+0000f2d0: 2020 2020 6b77 6172 6773 5b22 7072 6f6d      kwargs["prom
+0000f2e0: 6f74 655f 746f 5f6d 756c 7469 225d 203d  ote_to_multi"] =
+0000f2f0: 2054 7275 650a 0a20 2020 2023 204e 6f77   True..    # Now
+0000f300: 2077 6520 6361 6e20 7772 6974 650a 2020   we can write.  
+0000f310: 2020 6966 2067 656f 6669 6c65 7479 7065    if geofiletype
+0000f320: 2e69 735f 7369 6e67 6c65 6c61 7965 723a  .is_singlelayer:
+0000f330: 0a20 2020 2020 2020 2067 6466 2e74 6f5f  .        gdf.to_
+0000f340: 6669 6c65 2873 7472 2870 6174 6829 2c20  file(str(path), 
+0000f350: 2a2a 6b77 6172 6773 290a 2020 2020 656c  **kwargs).    el
+0000f360: 7365 3a0a 2020 2020 2020 2020 6764 662e  se:.        gdf.
+0000f370: 746f 5f66 696c 6528 7374 7228 7061 7468  to_file(str(path
+0000f380: 292c 206c 6179 6572 3d6c 6179 6572 2c20  ), layer=layer, 
+0000f390: 2a2a 6b77 6172 6773 290a 0a0a 6465 6620  **kwargs)...def 
+0000f3a0: 6765 745f 6372 7328 7061 7468 3a20 556e  get_crs(path: Un
+0000f3b0: 696f 6e5b 7374 722c 2022 6f73 2e50 6174  ion[str, "os.Pat
+0000f3c0: 684c 696b 655b 416e 795d 225d 2920 2d3e  hLike[Any]"]) ->
+0000f3d0: 2070 7970 726f 6a2e 4352 533a 0a20 2020   pyproj.CRS:.   
+0000f3e0: 2022 2222 0a20 2020 2047 6574 2074 6865   """.    Get the
+0000f3f0: 2043 5253 2028 7072 6f6a 6563 7469 6f6e   CRS (projection
+0000f400: 2920 6f66 2074 6865 2066 696c 650a 0a20  ) of the file.. 
+0000f410: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000f420: 2070 6174 6820 2850 6174 684c 696b 6529   path (PathLike)
+0000f430: 3a20 5061 7468 2074 6f20 7468 6520 6669  : Path to the fi
+0000f440: 6c65 2e0a 0a20 2020 2052 6574 7572 6e73  le...    Returns
+0000f450: 3a0a 2020 2020 2020 2020 7079 7072 6f6a  :.        pyproj
+0000f460: 2e43 5253 3a20 5468 6520 7072 6f6a 6563  .CRS: The projec
+0000f470: 7469 6f6e 206f 6620 7468 6520 6669 6c65  tion of the file
+0000f480: 0a20 2020 2022 2222 0a20 2020 2023 2054  .    """.    # T
+0000f490: 4f44 4f3a 2073 6565 6d73 206c 696b 6520  ODO: seems like 
+0000f4a0: 7375 7070 6f72 7420 666f 7220 6d75 6c74  support for mult
+0000f4b0: 6970 6c65 206c 6179 6572 7320 696e 2074  iple layers in t
+0000f4c0: 6865 2066 696c 6520 6973 6e27 7420 6865  he file isn't he
+0000f4d0: 7265 2079 6574 3f3f 3f0a 2020 2020 7769  re yet???.    wi
+0000f4e0: 7468 2066 696f 6e61 2e6f 7065 6e28 7374  th fiona.open(st
+0000f4f0: 7228 7061 7468 292c 2022 7222 2920 6173  r(path), "r") as
+0000f500: 2067 656f 6669 6c65 3a0a 2020 2020 2020   geofile:.      
+0000f510: 2020 6173 7365 7274 2067 656f 6669 6c65    assert geofile
+0000f520: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+0000f530: 2020 2020 2072 6574 7572 6e20 7079 7072       return pypr
+0000f540: 6f6a 2e43 5253 2867 656f 6669 6c65 2e63  oj.CRS(geofile.c
+0000f550: 7273 290a 0a0a 6465 6620 6973 5f67 656f  rs)...def is_geo
+0000f560: 6669 6c65 2870 6174 683a 2055 6e69 6f6e  file(path: Union
+0000f570: 5b73 7472 2c20 226f 732e 5061 7468 4c69  [str, "os.PathLi
+0000f580: 6b65 5b41 6e79 5d22 5d29 202d 3e20 626f  ke[Any]"]) -> bo
+0000f590: 6f6c 3a0a 2020 2020 2222 220a 2020 2020  ol:.    """.    
+0000f5a0: 4465 7465 726d 696e 6573 2062 6173 6564  Determines based
+0000f5b0: 206f 6e20 7468 6520 6669 6c65 7061 7468   on the filepath
+0000f5c0: 2069 6620 7468 6973 2069 7320 6120 6765   if this is a ge
+0000f5d0: 6f66 696c 652e 0a0a 2020 2020 4172 6773  ofile...    Args
+0000f5e0: 3a0a 2020 2020 2020 2020 7061 7468 2028  :.        path (
+0000f5f0: 5061 7468 4c69 6b65 293a 2054 6865 2066  PathLike): The f
+0000f600: 696c 6520 7061 7468 2e0a 0a20 2020 2052  ile path...    R
+0000f610: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000f620: 626f 6f6c 3a20 5472 7565 2069 6620 6974  bool: True if it
+0000f630: 2069 7320 6120 6765 6f20 6669 6c65 2e0a   is a geo file..
+0000f640: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+0000f650: 726e 2069 735f 6765 6f66 696c 655f 6578  rn is_geofile_ex
+0000f660: 7428 5061 7468 2870 6174 6829 2e73 7566  t(Path(path).suf
+0000f670: 6669 7829 0a0a 0a64 6566 2069 735f 6765  fix)...def is_ge
+0000f680: 6f66 696c 655f 6578 7428 6669 6c65 5f65  ofile_ext(file_e
+0000f690: 7874 3a20 7374 7229 202d 3e20 626f 6f6c  xt: str) -> bool
+0000f6a0: 3a0a 2020 2020 2222 220a 2020 2020 4465  :.    """.    De
+0000f6b0: 7465 726d 696e 6573 2062 6173 6564 206f  termines based o
+0000f6c0: 6e20 7468 6520 6669 6c65 2065 7874 656e  n the file exten
+0000f6d0: 7369 6f6e 2069 6620 7468 6973 2069 7320  sion if this is 
+0000f6e0: 6120 6765 6f66 696c 652e 0a0a 2020 2020  a geofile...    
+0000f6f0: 4172 6773 3a0a 2020 2020 2020 2020 6669  Args:.        fi
+0000f700: 6c65 5f65 7874 2028 7374 7229 3a20 7468  le_ext (str): th
+0000f710: 6520 6578 7465 6e73 696f 6e2e 0a0a 2020  e extension...  
+0000f720: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000f730: 2020 2062 6f6f 6c3a 2054 7275 6520 6966     bool: True if
+0000f740: 2069 7420 6973 2061 2067 656f 6669 6c65   it is a geofile
+0000f750: 2e0a 2020 2020 2222 220a 2020 2020 7472  ..    """.    tr
+0000f760: 793a 0a20 2020 2020 2020 2023 2049 6620  y:.        # If 
+0000f770: 7468 6520 6472 6976 6572 2063 616e 2062  the driver can b
+0000f780: 6520 6465 7465 726d 696e 6564 2c20 6974  e determined, it
+0000f790: 2069 7320 6120 2873 7570 706f 7274 6564   is a (supported
+0000f7a0: 2920 6765 6f20 6669 6c65 2e0a 2020 2020  ) geo file..    
+0000f7b0: 2020 2020 5f20 3d20 4765 6f66 696c 6554      _ = GeofileT
+0000f7c0: 7970 6528 6669 6c65 5f65 7874 290a 2020  ype(file_ext).  
+0000f7d0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000f7e0: 650a 2020 2020 6578 6365 7074 2045 7863  e.    except Exc
+0000f7f0: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+0000f800: 7265 7475 726e 2046 616c 7365 0a0a 0a64  return False...d
+0000f810: 6566 2063 6d70 280a 2020 2020 7061 7468  ef cmp(.    path
+0000f820: 313a 2055 6e69 6f6e 5b73 7472 2c20 226f  1: Union[str, "o
+0000f830: 732e 5061 7468 4c69 6b65 5b41 6e79 5d22  s.PathLike[Any]"
+0000f840: 5d2c 2070 6174 6832 3a20 556e 696f 6e5b  ], path2: Union[
+0000f850: 7374 722c 2022 6f73 2e50 6174 684c 696b  str, "os.PathLik
+0000f860: 655b 416e 795d 225d 0a29 202d 3e20 626f  e[Any]"].) -> bo
+0000f870: 6f6c 3a0a 2020 2020 2222 220a 2020 2020  ol:.    """.    
+0000f880: 436f 6d70 6172 6520 6966 2074 776f 2067  Compare if two g
+0000f890: 656f 6669 6c65 7320 6172 6520 6964 656e  eofiles are iden
+0000f8a0: 7469 6361 6c2e 0a0a 2020 2020 466f 7220  tical...    For 
+0000f8b0: 6765 6f66 696c 6573 2074 6861 7420 7573  geofiles that us
+0000f8c0: 6520 6d75 6c74 6970 6c65 2066 696c 6573  e multiple files
+0000f8d0: 2c20 616c 6c20 7265 6c65 7661 6e74 2066  , all relevant f
+0000f8e0: 696c 6573 206d 7573 7420 6265 2069 6465  iles must be ide
+0000f8f0: 6e74 6963 616c 2e0a 2020 2020 4567 2e20  ntical..    Eg. 
+0000f900: 666f 7220 7368 6170 6566 696c 6573 2c20  for shapefiles, 
+0000f910: 7468 6520 2e73 6870 2c20 2e73 6878 2061  the .shp, .shx a
+0000f920: 6e64 202e 6462 6620 6669 6c65 206d 7573  nd .dbf file mus
+0000f930: 7420 6265 2069 6465 6e74 6963 616c 2e0a  t be identical..
+0000f940: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000f950: 2020 2070 6174 6831 2028 5061 7468 4c69     path1 (PathLi
+0000f960: 6b65 293a 2070 6174 6820 746f 2074 6865  ke): path to the
+0000f970: 2066 6972 7374 2066 696c 652e 0a20 2020   first file..   
+0000f980: 2020 2020 2070 6174 6832 2028 5061 7468       path2 (Path
+0000f990: 4c69 6b65 293a 2070 6174 6820 746f 2074  Like): path to t
+0000f9a0: 6865 2073 6563 6f6e 6420 6669 6c65 2e0a  he second file..
+0000f9b0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000f9c0: 2020 2020 2020 626f 6f6c 3a20 5472 7565        bool: True
+0000f9d0: 2069 6620 7468 6520 6669 6c65 7320 6172   if the files ar
+0000f9e0: 6520 6964 656e 7469 6361 6c0a 2020 2020  e identical.    
+0000f9f0: 2222 220a 2020 2020 2320 4368 6563 6b20  """.    # Check 
+0000fa00: 696e 7075 7420 7061 7261 6d65 7465 7273  input parameters
+0000fa10: 0a20 2020 2070 6174 6831 5f70 203d 2050  .    path1_p = P
+0000fa20: 6174 6828 7061 7468 3129 0a20 2020 2070  ath(path1).    p
+0000fa30: 6174 6832 5f70 203d 2050 6174 6828 7061  ath2_p = Path(pa
+0000fa40: 7468 3229 0a0a 2020 2020 2320 466f 7220  th2)..    # For 
+0000fa50: 6120 7368 6170 6566 696c 652c 206d 756c  a shapefile, mul
+0000fa60: 7469 706c 6520 6669 6c65 7320 6e65 6564  tiple files need
+0000fa70: 2074 6f20 6265 2063 6f6d 7061 7265 640a   to be compared.
+0000fa80: 2020 2020 6966 2070 6174 6831 5f70 2e73      if path1_p.s
+0000fa90: 7566 6669 782e 6c6f 7765 7228 2920 3d3d  uffix.lower() ==
+0000faa0: 2022 2e73 6870 223a 0a20 2020 2020 2020   ".shp":.       
+0000fab0: 2070 6174 6832 5f6e 6f65 7874 2c20 5f20   path2_noext, _ 
+0000fac0: 3d20 6f73 2e70 6174 682e 7370 6c69 7465  = os.path.splite
+0000fad0: 7874 2870 6174 6832 5f70 290a 2020 2020  xt(path2_p).    
+0000fae0: 2020 2020 7368 6170 6566 696c 655f 6261      shapefile_ba
+0000faf0: 7365 5f73 7566 6669 7865 7320 3d20 5b22  se_suffixes = ["
+0000fb00: 2e73 6870 222c 2022 2e64 6266 222c 2022  .shp", ".dbf", "
+0000fb10: 2e73 6878 225d 0a20 2020 2020 2020 2070  .shx"].        p
+0000fb20: 6174 6831 5f6e 6f65 7874 203d 2070 6174  ath1_noext = pat
+0000fb30: 6831 5f70 2e70 6172 656e 7420 2f20 7061  h1_p.parent / pa
+0000fb40: 7468 315f 702e 7374 656d 0a20 2020 2020  th1_p.stem.     
+0000fb50: 2020 2070 6174 6832 5f6e 6f65 7874 203d     path2_noext =
+0000fb60: 2070 6174 6832 5f70 2e70 6172 656e 7420   path2_p.parent 
+0000fb70: 2f20 7061 7468 325f 702e 7374 656d 0a20  / path2_p.stem. 
+0000fb80: 2020 2020 2020 2066 6f72 2065 7874 2069         for ext i
+0000fb90: 6e20 7368 6170 6566 696c 655f 6261 7365  n shapefile_base
+0000fba0: 5f73 7566 6669 7865 733a 0a20 2020 2020  _suffixes:.     
+0000fbb0: 2020 2020 2020 2069 6620 6e6f 7420 6669         if not fi
+0000fbc0: 6c65 636d 702e 636d 7028 6622 7b73 7472  lecmp.cmp(f"{str
+0000fbd0: 2870 6174 6831 5f6e 6f65 7874 297d 7b65  (path1_noext)}{e
+0000fbe0: 7874 7d22 2c20 6622 7b73 7472 2870 6174  xt}", f"{str(pat
+0000fbf0: 6832 5f6e 6f65 7874 297d 7b65 7874 7d22  h2_noext)}{ext}"
+0000fc00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000fc10: 2020 206c 6f67 6765 722e 696e 666f 280a     logger.info(.
+0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc30: 2020 2020 6622 4669 6c65 207b 7061 7468      f"File {path
+0000fc40: 315f 6e6f 6578 747d 7b65 7874 7d20 6973  1_noext}{ext} is
+0000fc50: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
+0000fc60: 7b70 6174 6832 5f6e 6f65 7874 7d7b 6578  {path2_noext}{ex
+0000fc70: 747d 220a 2020 2020 2020 2020 2020 2020  t}".            
+0000fc80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000fc90: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000fca0: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
+0000fcb0: 6e20 5472 7565 0a20 2020 2065 6c73 653a  n True.    else:
+0000fcc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000fcd0: 6669 6c65 636d 702e 636d 7028 7374 7228  filecmp.cmp(str(
+0000fce0: 7061 7468 315f 7029 2c20 7374 7228 7061  path1_p), str(pa
+0000fcf0: 7468 325f 7029 290a 0a0a 6465 6620 636f  th2_p))...def co
+0000fd00: 7079 2873 7263 3a20 556e 696f 6e5b 7374  py(src: Union[st
+0000fd10: 722c 2022 6f73 2e50 6174 684c 696b 655b  r, "os.PathLike[
+0000fd20: 416e 795d 225d 2c20 6473 743a 2055 6e69  Any]"], dst: Uni
+0000fd30: 6f6e 5b73 7472 2c20 226f 732e 5061 7468  on[str, "os.Path
+0000fd40: 4c69 6b65 5b41 6e79 5d22 5d29 3a0a 2020  Like[Any]"]):.  
+0000fd50: 2020 2222 220a 2020 2020 436f 7069 6573    """.    Copies
+0000fd60: 2074 6865 2067 656f 6669 6c65 2066 726f   the geofile fro
+0000fd70: 6d20 7372 6320 746f 2064 7374 2e20 4973  m src to dst. Is
+0000fd80: 2074 6865 2073 6f75 7263 6520 6669 6c65   the source file
+0000fd90: 2069 7320 6120 6765 6f66 696c 6520 636f   is a geofile co
+0000fda0: 6e74 6169 6e69 6e67 0a20 2020 206f 6620  ntaining.    of 
+0000fdb0: 6d75 6c74 6970 6c65 2066 696c 6573 2028  multiple files (
+0000fdc0: 6567 2e20 2e73 6870 2920 616c 6c20 6669  eg. .shp) all fi
+0000fdd0: 6c65 7320 6172 6520 636f 7069 6564 2e0a  les are copied..
+0000fde0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000fdf0: 2020 2073 7263 2028 5061 7468 4c69 6b65     src (PathLike
+0000fe00: 293a 2074 6865 2066 696c 6520 746f 2063  ): the file to c
+0000fe10: 6f70 792e 0a20 2020 2020 2020 2064 7374  opy..        dst
+0000fe20: 2028 5061 7468 4c69 6b65 293a 2074 6865   (PathLike): the
+0000fe30: 206c 6f63 6174 696f 6e20 746f 2063 6f70   location to cop
+0000fe40: 7920 7468 6520 6669 6c65 2873 2920 746f  y the file(s) to
+0000fe50: 2e0a 2020 2020 2222 220a 2020 2020 2320  ..    """.    # 
+0000fe60: 4368 6563 6b20 696e 7075 7420 7061 7261  Check input para
+0000fe70: 6d65 7465 7273 0a20 2020 2073 7263 203d  meters.    src =
+0000fe80: 2050 6174 6828 7372 6329 0a20 2020 2064   Path(src).    d
+0000fe90: 7374 203d 2050 6174 6828 6473 7429 0a20  st = Path(dst). 
+0000fea0: 2020 2067 656f 6669 6c65 7479 7065 203d     geofiletype =
+0000feb0: 2047 656f 6669 6c65 5479 7065 2873 7263   GeofileType(src
+0000fec0: 290a 0a20 2020 2023 2043 6f70 7920 7468  )..    # Copy th
+0000fed0: 6520 6d61 696e 2066 696c 650a 2020 2020  e main file.    
+0000fee0: 7368 7574 696c 2e63 6f70 7928 7374 7228  shutil.copy(str(
+0000fef0: 7372 6329 2c20 6473 7429 0a0a 2020 2020  src), dst)..    
+0000ff00: 2320 466f 7220 736f 6d65 2066 696c 6520  # For some file 
+0000ff10: 7479 7065 732c 2065 7874 7261 2066 696c  types, extra fil
+0000ff20: 6573 206e 6565 6420 746f 2062 6520 636f  es need to be co
+0000ff30: 7069 6564 0a20 2020 2023 2049 6620 6465  pied.    # If de
+0000ff40: 7374 2069 7320 6120 6469 722c 206a 7573  st is a dir, jus
+0000ff50: 7420 7573 6520 6d6f 7665 2e20 4f74 6865  t use move. Othe
+0000ff60: 7277 6973 6520 636f 6e63 6174 2064 6573  rwise concat des
+0000ff70: 7420 6669 6c65 7061 7468 730a 2020 2020  t filepaths.    
+0000ff80: 6966 2067 656f 6669 6c65 7479 7065 2e73  if geofiletype.s
+0000ff90: 7566 6669 7865 735f 6578 7472 6166 696c  uffixes_extrafil
+0000ffa0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0000ffb0: 2020 2020 2020 2020 6966 2064 7374 2e69          if dst.i
+0000ffc0: 735f 6469 7228 293a 0a20 2020 2020 2020  s_dir():.       
+0000ffd0: 2020 2020 2066 6f72 2073 7566 6669 7820       for suffix 
+0000ffe0: 696e 2067 656f 6669 6c65 7479 7065 2e73  in geofiletype.s
+0000fff0: 7566 6669 7865 735f 6578 7472 6166 696c  uffixes_extrafil
+00010000: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00010010: 2020 2020 7372 6366 696c 6520 3d20 7372      srcfile = sr
+00010020: 632e 7061 7265 6e74 202f 2066 227b 7372  c.parent / f"{sr
+00010030: 632e 7374 656d 7d7b 7375 6666 6978 7d22  c.stem}{suffix}"
+00010040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010050: 2069 6620 7372 6366 696c 652e 6578 6973   if srcfile.exis
+00010060: 7473 2829 3a0a 2020 2020 2020 2020 2020  ts():.          
+00010070: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
+00010080: 2e63 6f70 7928 7374 7228 7372 6366 696c  .copy(str(srcfil
+00010090: 6529 2c20 6473 7429 0a20 2020 2020 2020  e), dst).       
+000100a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000100b0: 2020 2066 6f72 2073 7566 6669 7820 696e     for suffix in
+000100c0: 2067 656f 6669 6c65 7479 7065 2e73 7566   geofiletype.suf
+000100d0: 6669 7865 735f 6578 7472 6166 696c 6573  fixes_extrafiles
+000100e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000100f0: 2020 7372 6366 696c 6520 3d20 7372 632e    srcfile = src.
+00010100: 7061 7265 6e74 202f 2066 227b 7372 632e  parent / f"{src.
+00010110: 7374 656d 7d7b 7375 6666 6978 7d22 0a20  stem}{suffix}". 
+00010120: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00010130: 7374 6669 6c65 203d 2064 7374 2e70 6172  stfile = dst.par
+00010140: 656e 7420 2f20 6622 7b64 7374 2e73 7465  ent / f"{dst.ste
+00010150: 6d7d 7b73 7566 6669 787d 220a 2020 2020  m}{suffix}".    
+00010160: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00010170: 7263 6669 6c65 2e65 7869 7374 7328 293a  rcfile.exists():
+00010180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010190: 2020 2020 2073 6875 7469 6c2e 636f 7079       shutil.copy
+000101a0: 2873 7472 2873 7263 6669 6c65 292c 2064  (str(srcfile), d
+000101b0: 7374 6669 6c65 290a 0a0a 6465 6620 6d6f  stfile)...def mo
+000101c0: 7665 2873 7263 3a20 556e 696f 6e5b 7374  ve(src: Union[st
+000101d0: 722c 2022 6f73 2e50 6174 684c 696b 655b  r, "os.PathLike[
+000101e0: 416e 795d 225d 2c20 6473 743a 2055 6e69  Any]"], dst: Uni
+000101f0: 6f6e 5b73 7472 2c20 226f 732e 5061 7468  on[str, "os.Path
+00010200: 4c69 6b65 5b41 6e79 5d22 5d29 3a0a 2020  Like[Any]"]):.  
+00010210: 2020 2222 220a 2020 2020 4d6f 7665 7320    """.    Moves 
+00010220: 7468 6520 6765 6f66 696c 6520 6672 6f6d  the geofile from
+00010230: 2073 7263 2074 6f20 6473 742e 2049 6620   src to dst. If 
+00010240: 7468 6520 736f 7572 6365 2066 696c 6520  the source file 
+00010250: 6973 2061 2067 656f 6669 6c65 2063 6f6e  is a geofile con
+00010260: 7461 696e 696e 670a 2020 2020 6f66 206d  taining.    of m
+00010270: 756c 7469 706c 6520 6669 6c65 7320 2865  ultiple files (e
+00010280: 672e 202e 7368 7029 2061 6c6c 2066 696c  g. .shp) all fil
+00010290: 6573 2061 7265 206d 6f76 6564 2e0a 0a20  es are moved... 
+000102a0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000102b0: 2073 7263 2028 5061 7468 4c69 6b65 293a   src (PathLike):
+000102c0: 2074 6865 2066 696c 6520 746f 206d 6f76   the file to mov
+000102d0: 650a 2020 2020 2020 2020 6473 7420 2850  e.        dst (P
+000102e0: 6174 684c 696b 6529 3a20 7468 6520 6c6f  athLike): the lo
+000102f0: 6361 7469 6f6e 2074 6f20 6d6f 7665 2074  cation to move t
+00010300: 6865 2066 696c 6528 7329 2074 6f0a 2020  he file(s) to.  
+00010310: 2020 2222 220a 2020 2020 2320 4368 6563    """.    # Chec
+00010320: 6b20 696e 7075 7420 7061 7261 6d65 7465  k input paramete
+00010330: 7273 0a20 2020 2073 7263 203d 2050 6174  rs.    src = Pat
+00010340: 6828 7372 6329 0a20 2020 2064 7374 203d  h(src).    dst =
+00010350: 2050 6174 6828 6473 7429 0a20 2020 2067   Path(dst).    g
+00010360: 656f 6669 6c65 7479 7065 203d 2047 656f  eofiletype = Geo
+00010370: 6669 6c65 5479 7065 2873 7263 290a 0a20  fileType(src).. 
+00010380: 2020 2023 204d 6f76 6520 7468 6520 6d61     # Move the ma
+00010390: 696e 2066 696c 650a 2020 2020 7368 7574  in file.    shut
+000103a0: 696c 2e6d 6f76 6528 7374 7228 7372 6329  il.move(str(src)
+000103b0: 2c20 6473 7429 0a0a 2020 2020 2320 466f  , dst)..    # Fo
+000103c0: 7220 736f 6d65 2066 696c 6520 7479 7065  r some file type
+000103d0: 732c 2065 7874 7261 2066 696c 6573 206e  s, extra files n
+000103e0: 6565 6420 746f 2062 6520 6d6f 7665 640a  eed to be moved.
+000103f0: 2020 2020 2320 4966 2064 6573 7420 6973      # If dest is
+00010400: 2061 2064 6972 2c20 6a75 7374 2075 7365   a dir, just use
+00010410: 206d 6f76 652e 204f 7468 6572 7769 7365   move. Otherwise
+00010420: 2063 6f6e 6361 7420 6465 7374 2066 696c   concat dest fil
+00010430: 6570 6174 6873 0a20 2020 2069 6620 6765  epaths.    if ge
+00010440: 6f66 696c 6574 7970 652e 7375 6666 6978  ofiletype.suffix
+00010450: 6573 5f65 7874 7261 6669 6c65 7320 6973  es_extrafiles is
+00010460: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00010470: 2020 2069 6620 6473 742e 6973 5f64 6972     if dst.is_dir
+00010480: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00010490: 666f 7220 7375 6666 6978 2069 6e20 6765  for suffix in ge
+000104a0: 6f66 696c 6574 7970 652e 7375 6666 6978  ofiletype.suffix
+000104b0: 6573 5f65 7874 7261 6669 6c65 733a 0a20  es_extrafiles:. 
+000104c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000104d0: 7263 6669 6c65 203d 2073 7263 2e70 6172  rcfile = src.par
+000104e0: 656e 7420 2f20 6622 7b73 7263 2e73 7465  ent / f"{src.ste
+000104f0: 6d7d 7b73 7566 6669 787d 220a 2020 2020  m}{suffix}".    
+00010500: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00010510: 7263 6669 6c65 2e65 7869 7374 7328 293a  rcfile.exists():
+00010520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010530: 2020 2020 2073 6875 7469 6c2e 6d6f 7665       shutil.move
+00010540: 2873 7472 2873 7263 6669 6c65 292c 2064  (str(srcfile), d
+00010550: 7374 290a 2020 2020 2020 2020 656c 7365  st).        else
+00010560: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00010570: 7220 7375 6666 6978 2069 6e20 6765 6f66  r suffix in geof
+00010580: 696c 6574 7970 652e 7375 6666 6978 6573  iletype.suffixes
+00010590: 5f65 7874 7261 6669 6c65 733a 0a20 2020  _extrafiles:.   
+000105a0: 2020 2020 2020 2020 2020 2020 2073 7263               src
+000105b0: 6669 6c65 203d 2073 7263 2e70 6172 656e  file = src.paren
+000105c0: 7420 2f20 6622 7b73 7263 2e73 7465 6d7d  t / f"{src.stem}
+000105d0: 7b73 7566 6669 787d 220a 2020 2020 2020  {suffix}".      
+000105e0: 2020 2020 2020 2020 2020 6473 7466 696c            dstfil
+000105f0: 6520 3d20 6473 742e 7061 7265 6e74 202f  e = dst.parent /
+00010600: 2066 227b 6473 742e 7374 656d 7d7b 7375   f"{dst.stem}{su
+00010610: 6666 6978 7d22 0a20 2020 2020 2020 2020  ffix}".         
+00010620: 2020 2020 2020 2069 6620 7372 6366 696c         if srcfil
+00010630: 652e 6578 6973 7473 2829 3a0a 2020 2020  e.exists():.    
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 7368 7574 696c 2e6d 6f76 6528 7374 7228  shutil.move(str(
+00010660: 7372 6366 696c 6529 2c20 6473 7466 696c  srcfile), dstfil
+00010670: 6529 0a0a 0a64 6566 2072 656d 6f76 6528  e)...def remove(
+00010680: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
+00010690: 2022 6f73 2e50 6174 684c 696b 655b 416e   "os.PathLike[An
+000106a0: 795d 225d 2c20 6d69 7373 696e 675f 6f6b  y]"], missing_ok
+000106b0: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
+000106c0: 0a20 2020 2022 2222 0a20 2020 2052 656d  .    """.    Rem
+000106d0: 6f76 6573 2074 6865 2067 656f 6669 6c65  oves the geofile
+000106e0: 2e20 4973 2069 7420 6973 2061 2067 656f  . Is it is a geo
+000106f0: 6669 6c65 2063 6f6d 706f 7365 6420 6f66  file composed of
+00010700: 206d 756c 7469 706c 6520 6669 6c65 730a   multiple files.
+00010710: 2020 2020 2865 672e 202e 7368 7029 2061      (eg. .shp) a
+00010720: 6c6c 2066 696c 6573 2061 7265 2072 656d  ll files are rem
+00010730: 6f76 6564 2e0a 2020 2020 4966 202e 6c6f  oved..    If .lo
+00010740: 636b 2066 696c 6573 2061 7265 2070 7265  ck files are pre
+00010750: 7365 6e74 2c20 7468 6579 2061 7265 2072  sent, they are r
+00010760: 656d 6f76 6564 2061 7320 7765 6c6c 2e0a  emoved as well..
+00010770: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+00010780: 2020 2070 6174 6820 2850 6174 684c 696b     path (PathLik
+00010790: 6529 3a20 7468 6520 6669 6c65 2074 6f20  e): the file to 
+000107a0: 7265 6d6f 7665 0a20 2020 2022 2222 0a20  remove.    """. 
+000107b0: 2020 2023 2043 6865 636b 2069 6e70 7574     # Check input
+000107c0: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
+000107d0: 7061 7468 203d 2050 6174 6828 7061 7468  path = Path(path
+000107e0: 290a 2020 2020 6765 6f66 696c 6574 7970  ).    geofiletyp
+000107f0: 6520 3d20 4765 6f66 696c 6554 7970 6528  e = GeofileType(
+00010800: 7061 7468 290a 0a20 2020 2023 2049 6620  path)..    # If 
+00010810: 7468 6572 6520 6973 2061 206c 6f63 6b20  there is a lock 
+00010820: 6669 6c65 2c20 7265 6d6f 7665 2069 740a  file, remove it.
+00010830: 2020 2020 6c6f 636b 6669 6c65 5f70 6174      lockfile_pat
+00010840: 6820 3d20 7061 7468 2e70 6172 656e 7420  h = path.parent 
+00010850: 2f20 6622 7b70 6174 682e 6e61 6d65 7d2e  / f"{path.name}.
+00010860: 6c6f 636b 220a 2020 2020 6c6f 636b 6669  lock".    lockfi
+00010870: 6c65 5f70 6174 682e 756e 6c69 6e6b 286d  le_path.unlink(m
+00010880: 6973 7369 6e67 5f6f 6b3d 5472 7565 290a  issing_ok=True).
+00010890: 0a20 2020 2023 2052 656d 6f76 6520 7468  .    # Remove th
+000108a0: 6520 6d61 696e 2066 696c 650a 2020 2020  e main file.    
+000108b0: 6966 2070 6174 682e 6578 6973 7473 2829  if path.exists()
+000108c0: 3a0a 2020 2020 2020 2020 7061 7468 2e75  :.        path.u
+000108d0: 6e6c 696e 6b28 6d69 7373 696e 675f 6f6b  nlink(missing_ok
+000108e0: 3d6d 6973 7369 6e67 5f6f 6b29 0a0a 2020  =missing_ok)..  
+000108f0: 2020 2320 466f 7220 736f 6d65 2066 696c    # For some fil
+00010900: 6520 7479 7065 732c 2065 7874 7261 2066  e types, extra f
+00010910: 696c 6573 206e 6565 6420 746f 2062 6520  iles need to be 
+00010920: 7265 6d6f 7665 640a 2020 2020 6966 2067  removed.    if g
+00010930: 656f 6669 6c65 7479 7065 2e73 7566 6669  eofiletype.suffi
+00010940: 7865 735f 6578 7472 6166 696c 6573 2069  xes_extrafiles i
+00010950: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00010960: 2020 2020 666f 7220 7375 6666 6978 2069      for suffix i
+00010970: 6e20 6765 6f66 696c 6574 7970 652e 7375  n geofiletype.su
+00010980: 6666 6978 6573 5f65 7874 7261 6669 6c65  ffixes_extrafile
+00010990: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+000109a0: 7572 725f 7061 7468 203d 2070 6174 682e  urr_path = path.
+000109b0: 7061 7265 6e74 202f 2066 227b 7061 7468  parent / f"{path
+000109c0: 2e73 7465 6d7d 7b73 7566 6669 787d 220a  .stem}{suffix}".
+000109d0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000109e0: 5f70 6174 682e 756e 6c69 6e6b 286d 6973  _path.unlink(mis
+000109f0: 7369 6e67 5f6f 6b3d 5472 7565 290a 0a0a  sing_ok=True)...
+00010a00: 6465 6620 6170 7065 6e64 5f74 6f28 0a20  def append_to(. 
+00010a10: 2020 2073 7263 3a20 556e 696f 6e5b 7374     src: Union[st
+00010a20: 722c 2022 6f73 2e50 6174 684c 696b 655b  r, "os.PathLike[
+00010a30: 416e 795d 225d 2c0a 2020 2020 6473 743a  Any]"],.    dst:
+00010a40: 2055 6e69 6f6e 5b73 7472 2c20 226f 732e   Union[str, "os.
+00010a50: 5061 7468 4c69 6b65 5b41 6e79 5d22 5d2c  PathLike[Any]"],
+00010a60: 0a20 2020 2073 7263 5f6c 6179 6572 3a20  .    src_layer: 
+00010a70: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00010a80: 4e6f 6e65 2c0a 2020 2020 6473 745f 6c61  None,.    dst_la
+00010a90: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
+00010aa0: 725d 203d 204e 6f6e 652c 0a20 2020 2073  r] = None,.    s
+00010ab0: 7263 5f63 7273 3a20 556e 696f 6e5b 696e  rc_crs: Union[in
+00010ac0: 742c 2073 7472 2c20 4e6f 6e65 5d20 3d20  t, str, None] = 
+00010ad0: 4e6f 6e65 2c0a 2020 2020 6473 745f 6372  None,.    dst_cr
+00010ae0: 733a 2055 6e69 6f6e 5b69 6e74 2c20 7374  s: Union[int, st
+00010af0: 722c 204e 6f6e 655d 203d 204e 6f6e 652c  r, None] = None,
+00010b00: 0a20 2020 2072 6570 726f 6a65 6374 3a20  .    reproject: 
+00010b10: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00010b20: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
+00010b30: 696f 6e73 3a20 626f 6f6c 203d 2046 616c  ions: bool = Fal
+00010b40: 7365 2c0a 2020 2020 666f 7263 655f 6f75  se,.    force_ou
+00010b50: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
+00010b60: 653a 2055 6e69 6f6e 5b47 656f 6d65 7472  e: Union[Geometr
+00010b70: 7954 7970 652c 2073 7472 2c20 4e6f 6e65  yType, str, None
+00010b80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6372  ] = None,.    cr
+00010b90: 6561 7465 5f73 7061 7469 616c 5f69 6e64  eate_spatial_ind
+00010ba0: 6578 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ex: Optional[boo
+00010bb0: 6c5d 203d 2054 7275 652c 0a20 2020 2061  l] = True,.    a
+00010bc0: 7070 656e 645f 7469 6d65 6f75 745f 733a  ppend_timeout_s:
+00010bd0: 2069 6e74 203d 2036 3030 2c0a 2020 2020   int = 600,.    
+00010be0: 7472 616e 7361 6374 696f 6e5f 7369 7a65  transaction_size
+00010bf0: 3a20 696e 7420 3d20 3530 3030 302c 0a20  : int = 50000,. 
+00010c00: 2020 2070 7265 7365 7276 655f 6669 643a     preserve_fid:
+00010c10: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00010c20: 3d20 4e6f 6e65 2c0a 2020 2020 6f70 7469  = None,.    opti
+00010c30: 6f6e 733a 2064 6963 7420 3d20 7b7d 2c0a  ons: dict = {},.
+00010c40: 293a 0a20 2020 2022 2222 0a20 2020 2041  ):.    """.    A
+00010c50: 7070 656e 6420 7372 6320 6669 6c65 2074  ppend src file t
+00010c60: 6f20 7468 6520 6473 7420 6669 6c65 2e0a  o the dst file..
+00010c70: 0a20 2020 2052 656d 6172 6b3a 2061 7070  .    Remark: app
+00010c80: 656e 6420 6973 206e 6f74 2073 7570 706f  end is not suppo
+00010c90: 7274 6564 2066 6f72 2061 6c6c 2066 696c  rted for all fil
+00010ca0: 6574 7970 6573 2069 6e20 6669 6f6e 612f  etypes in fiona/
+00010cb0: 6765 6f70 616e 6461 7320 2830 2e38 290a  geopandas (0.8).
+00010cc0: 2020 2020 736f 2077 6f72 6b61 726f 756e      so workaroun
+00010cd0: 6420 7669 6120 6764 616c 206e 6565 6465  d via gdal neede
+00010ce0: 642e 0a0a 2020 2020 5468 6520 6f70 7469  d...    The opti
+00010cf0: 6f6e 7320 7061 7261 6d65 7465 7220 6361  ons parameter ca
+00010d00: 6e20 6265 2075 7365 6420 746f 2070 6173  n be used to pas
+00010d10: 7320 616e 7920 7479 7065 206f 6620 6f70  s any type of op
+00010d20: 7469 6f6e 7320 746f 2047 4441 4c20 696e  tions to GDAL in
+00010d30: 0a20 2020 2074 6865 2066 6f6c 6c6f 7769  .    the followi
+00010d40: 6e67 2066 6f72 6d3a 0a20 2020 2020 2020  ng form:.       
+00010d50: 207b 2022 3c6f 7074 696f 6e5f 7479 7065   { "<option_type
+00010d60: 3e2e 3c6f 7074 696f 6e5f 6e61 6d65 3e22  >.<option_name>"
+00010d70: 3a20 3c6f 7074 696f 6e5f 7661 6c75 653e  : <option_value>
+00010d80: 207d 0a0a 2020 2020 5468 6520 6f70 7469   }..    The opti
+00010d90: 6f6e 2074 7970 6573 2063 616e 2062 6520  on types can be 
+00010da0: 616e 7920 6f66 2074 6865 2066 6f6c 6c6f  any of the follo
+00010db0: 7769 6e67 3a0a 2020 2020 2020 2020 2d20  wing:.        - 
+00010dc0: 4c41 5945 525f 4352 4541 5449 4f4e 3a20  LAYER_CREATION: 
+00010dd0: 6c61 7965 7220 6372 6561 7469 6f6e 206f  layer creation o
+00010de0: 7074 696f 6e20 286c 636f 290a 2020 2020  ption (lco).    
+00010df0: 2020 2020 2d20 4441 5441 5345 545f 4352      - DATASET_CR
+00010e00: 4541 5449 4f4e 3a20 6461 7461 7365 7420  EATION: dataset 
+00010e10: 6372 6561 7469 6f6e 206f 7074 696f 6e20  creation option 
+00010e20: 2864 7363 6f29 0a20 2020 2020 2020 202d  (dsco).        -
+00010e30: 2049 4e50 5554 5f4f 5045 4e3a 2069 6e70   INPUT_OPEN: inp
+00010e40: 7574 2064 6174 6173 6574 206f 7065 6e20  ut dataset open 
+00010e50: 6f70 7469 6f6e 2028 6f6f 290a 2020 2020  option (oo).    
+00010e60: 2020 2020 2d20 4445 5354 494e 4154 494f      - DESTINATIO
+00010e70: 4e5f 4f50 454e 3a20 6465 7374 696e 6174  N_OPEN: destinat
+00010e80: 696f 6e20 6461 7461 7365 7420 6f70 656e  ion dataset open
+00010e90: 206f 7074 696f 6e20 2864 6f6f 290a 2020   option (doo).  
+00010ea0: 2020 2020 2020 2d20 434f 4e46 4947 3a20        - CONFIG: 
+00010eb0: 636f 6e66 6967 206f 7074 696f 6e20 2863  config option (c
+00010ec0: 6f6e 6669 6729 0a0a 2020 2020 5468 6520  onfig)..    The 
+00010ed0: 6f70 7469 6f6e 7320 6361 6e20 6265 2066  options can be f
+00010ee0: 6f75 6e64 2069 6e20 7468 6520 5b47 4441  ound in the [GDA
+00010ef0: 4c20 7665 6374 6f72 2064 7269 7665 7220  L vector driver 
+00010f00: 646f 6375 6d65 6e74 6174 696f 6e5d 0a20  documentation]. 
+00010f10: 2020 2028 6874 7470 733a 2f2f 6764 616c     (https://gdal
+00010f20: 2e6f 7267 2f64 7269 7665 7273 2f76 6563  .org/drivers/vec
+00010f30: 746f 722f 696e 6465 782e 6874 6d6c 292e  tor/index.html).
+00010f40: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00010f50: 2020 2020 7372 6320 2855 6e69 6f6e 5b73      src (Union[s
+00010f60: 7472 2c29 3a20 736f 7572 6365 2066 696c  tr,): source fil
+00010f70: 6520 7061 7468 2e0a 2020 2020 2020 2020  e path..        
+00010f80: 6473 7420 2855 6e69 6f6e 5b73 7472 2c29  dst (Union[str,)
+00010f90: 3a20 6465 7374 696e 6174 696f 6e20 6669  : destination fi
+00010fa0: 6c65 2070 6174 682e 0a20 2020 2020 2020  le path..       
+00010fb0: 2073 7263 5f6c 6179 6572 2028 7374 722c   src_layer (str,
+00010fc0: 206f 7074 696f 6e61 6c29 3a20 736f 7572   optional): sour
+00010fd0: 6365 206c 6179 6572 2e20 4465 6661 756c  ce layer. Defaul
+00010fe0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00010ff0: 2020 2020 6473 745f 6c61 7965 7220 2873      dst_layer (s
+00011000: 7472 2c20 6f70 7469 6f6e 616c 293a 2064  tr, optional): d
+00011010: 6573 7469 6e61 7469 6f6e 206c 6179 6572  estination layer
+00011020: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00011030: 6e65 2e0a 2020 2020 2020 2020 7372 635f  ne..        src_
+00011040: 6372 7320 2873 7472 2c20 6f70 7469 6f6e  crs (str, option
+00011050: 616c 293a 2061 6e20 6570 7367 2069 6e74  al): an epsg int
+00011060: 206f 7220 616e 7974 6869 6e67 2073 7570   or anything sup
+00011070: 706f 7274 6564 0a20 2020 2020 2020 2020  ported.         
+00011080: 2020 2062 7920 7468 6520 4f47 5253 7061     by the OGRSpa
+00011090: 7469 616c 5265 6665 7265 6e63 652e 5365  tialReference.Se
+000110a0: 7446 726f 6d55 7365 7249 6e70 7574 2829  tFromUserInput()
+000110b0: 2063 616c 6c2c 2077 6869 6368 2069 6e63   call, which inc
+000110c0: 6c75 6465 730a 2020 2020 2020 2020 2020  ludes.          
+000110d0: 2020 616e 2045 5053 4720 7374 7269 6e67    an EPSG string
+000110e0: 2028 6567 2e20 2245 5053 473a 3433 3236   (eg. "EPSG:4326
+000110f0: 2229 2c20 6120 7765 6c6c 206b 6e6f 776e  "), a well known
+00011100: 2074 6578 7420 2857 4b54 2920 4352 530a   text (WKT) CRS.
+00011110: 2020 2020 2020 2020 2020 2020 6465 6669              defi
+00011120: 6e69 7469 6f6e 2c2e 2e2e 2044 6566 6175  nition,... Defau
+00011130: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
+00011140: 2020 2020 2064 7374 5f63 7273 2028 7374       dst_crs (st
+00011150: 722c 206f 7074 696f 6e61 6c29 3a20 616e  r, optional): an
+00011160: 2065 7073 6720 696e 7420 6f72 2061 6e79   epsg int or any
+00011170: 7468 696e 6720 7375 7070 6f72 7465 640a  thing supported.
+00011180: 2020 2020 2020 2020 2020 2020 6279 2074              by t
+00011190: 6865 204f 4752 5370 6174 6961 6c52 6566  he OGRSpatialRef
+000111a0: 6572 656e 6365 2e53 6574 4672 6f6d 5573  erence.SetFromUs
+000111b0: 6572 496e 7075 7428 2920 6361 6c6c 2c20  erInput() call, 
+000111c0: 7768 6963 6820 696e 636c 7564 6573 0a20  which includes. 
+000111d0: 2020 2020 2020 2020 2020 2061 6e20 4550             an EP
+000111e0: 5347 2073 7472 696e 6720 2865 672e 2022  SG string (eg. "
+000111f0: 4550 5347 3a34 3332 3622 292c 2061 2077  EPSG:4326"), a w
+00011200: 656c 6c20 6b6e 6f77 6e20 7465 7874 2028  ell known text (
+00011210: 574b 5429 2043 5253 0a20 2020 2020 2020  WKT) CRS.       
+00011220: 2020 2020 2064 6566 696e 6974 696f 6e2c       definition,
+00011230: 2e2e 2e20 4465 6661 756c 7473 2074 6f20  ... Defaults to 
+00011240: 4e6f 6e65 2e0a 2020 2020 2020 2020 7265  None..        re
+00011250: 7072 6f6a 6563 7420 2862 6f6f 6c2c 206f  project (bool, o
+00011260: 7074 696f 6e61 6c29 3a20 5472 7565 2074  ptional): True t
+00011270: 6f20 7265 7072 6f6a 6563 7420 7768 696c  o reproject whil
+00011280: 6520 636f 6e76 6572 7469 6e67 2074 6865  e converting the
+00011290: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+000112a0: 652e 2044 6566 6175 6c74 7320 746f 2046  e. Defaults to F
+000112b0: 616c 7365 2e0a 2020 2020 2020 2020 6578  alse..        ex
+000112c0: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
+000112d0: 2028 626f 6f6c 292c 206f 7074 696f 6e61   (bool), optiona
+000112e0: 6c29 3a20 5472 7565 2074 6f20 6f75 7470  l): True to outp
+000112f0: 7574 206f 6e6c 7920 7369 6d70 6c65 2067  ut only simple g
+00011300: 656f 6d65 7472 6965 732e 0a20 2020 2020  eometries..     
+00011310: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00011320: 746f 2046 616c 7365 2e0a 2020 2020 2020  to False..      
+00011330: 2020 666f 7263 655f 6f75 7470 7574 5f67    force_output_g
+00011340: 656f 6d65 7472 7974 7970 6520 2855 6e69  eometrytype (Uni
+00011350: 6f6e 5b47 656f 6d65 7472 7954 7970 652c  on[GeometryType,
+00011360: 2073 7472 5d2c 206f 7074 696f 6e61 6c29   str], optional)
+00011370: 3a20 4765 6f6d 6574 7279 2074 7970 652e  : Geometry type.
+00011380: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
+00011390: 2874 7279 2074 6f29 2066 6f72 6365 2074  (try to) force t
+000113a0: 6865 206f 7574 7075 7420 746f 2e20 4465  he output to. De
+000113b0: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
+000113c0: 2020 2020 2020 2020 6372 6561 7465 5f73          create_s
+000113d0: 7061 7469 616c 5f69 6e64 6578 2028 626f  patial_index (bo
+000113e0: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2054  ol, optional): T
+000113f0: 7275 6520 746f 2063 7265 6174 6520 6120  rue to create a 
+00011400: 7370 6174 6961 6c20 696e 6465 780a 2020  spatial index.  
+00011410: 2020 2020 2020 2020 2020 6f6e 2074 6865            on the
+00011420: 2064 6573 7469 6e61 7469 6f6e 2066 696c   destination fil
+00011430: 652f 6c61 7965 722e 2049 6620 4e6f 6e65  e/layer. If None
+00011440: 2c20 7468 6520 6465 6661 756c 7420 6265  , the default be
+00011450: 6861 7669 6f75 7220 6279 2067 6461 6c20  haviour by gdal 
+00011460: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+00011470: 7468 6174 2066 696c 6520 7479 7065 2069  that file type i
+00011480: 7320 7265 7370 6563 7465 642e 2049 6620  s respected. If 
+00011490: 7468 6520 4c41 5945 525f 4352 4541 5449  the LAYER_CREATI
+000114a0: 4f4e 2e53 5041 5449 414c 5f49 4e44 4558  ON.SPATIAL_INDEX
+000114b0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+000114c0: 616d 6574 6572 2069 7320 7370 6563 6966  ameter is specif
+000114d0: 6965 6420 696e 206f 7074 696f 6e73 2c20  ied in options, 
+000114e0: 6372 6561 7465 5f73 7061 7469 616c 5f69  create_spatial_i
+000114f0: 6e64 6578 2069 7320 6967 6e6f 7265 642e  ndex is ignored.
+00011500: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
+00011510: 6175 6c74 7320 746f 2054 7275 652e 0a20  aults to True.. 
+00011520: 2020 2020 2020 2061 7070 656e 645f 7469         append_ti
+00011530: 6d65 6f75 745f 7320 2869 6e74 2c20 6f70  meout_s (int, op
+00011540: 7469 6f6e 616c 293a 2074 696d 656f 7574  tional): timeout
+00011550: 2074 6f20 7573 6520 6966 2074 6865 206f   to use if the o
+00011560: 7574 7075 7420 6669 6c65 2069 730a 2020  utput file is.  
+00011570: 2020 2020 2020 2020 2020 6265 696e 6720            being 
+00011580: 7772 6974 7465 6e20 746f 2062 7920 616e  written to by an
+00011590: 6f74 6865 7220 7072 6f63 6573 7320 616c  other process al
+000115a0: 7265 6164 792e 2044 6566 6175 6c74 7320  ready. Defaults 
+000115b0: 746f 2036 3030 2e0a 2020 2020 2020 2020  to 600..        
+000115c0: 7472 616e 7361 6374 696f 6e5f 7369 7a65  transaction_size
+000115d0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
+000115e0: 3a20 5472 616e 7361 6374 696f 6e20 7369  : Transaction si
+000115f0: 7a65 2e0a 2020 2020 2020 2020 2020 2020  ze..            
+00011600: 4465 6661 756c 7473 2074 6f20 3530 3030  Defaults to 5000
+00011610: 302e 0a20 2020 2020 2020 2070 7265 7365  0..        prese
+00011620: 7276 655f 6669 6420 2862 6f6f 6c2c 206f  rve_fid (bool, o
+00011630: 7074 696f 6e61 6c29 3a20 5472 7565 2074  ptional): True t
+00011640: 6f20 6d61 6b65 2061 6e20 6578 7472 6120  o make an extra 
+00011650: 6566 666f 7274 2074 6f20 7072 6573 6572  effort to preser
+00011660: 7665 2066 6964 2773 206f 660a 2020 2020  ve fid's of.    
+00011670: 2020 2020 2020 2020 7468 6520 736f 7572          the sour
+00011680: 6365 206c 6179 6572 2074 6f20 7468 6520  ce layer to the 
+00011690: 6465 7374 696e 6174 696f 6e20 6c61 7965  destination laye
+000116a0: 722e 2046 616c 7365 206e 6f74 2074 6f20  r. False not to 
+000116b0: 646f 2061 6e79 2065 6666 6f72 742e 204e  do any effort. N
+000116c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000116d0: 746f 2075 7365 2074 6865 2064 6566 6175  to use the defau
+000116e0: 6c74 2062 6568 6176 696f 7572 206f 6620  lt behaviour of 
+000116f0: 6764 616c 2c20 7468 6174 2061 6c72 6561  gdal, that alrea
+00011700: 6479 2070 7265 7365 7276 6573 2069 6e20  dy preserves in 
+00011710: 736f 6d65 2063 6173 6573 2e0a 2020 2020  some cases..    
+00011720: 2020 2020 2020 2020 536f 6d65 2066 696c          Some fil
+00011730: 6520 666f 726d 6174 7320 646f 6e27 7420  e formats don't 
+00011740: 6578 706c 6963 6974 6c79 2073 746f 7265  explicitly store
+00011750: 2074 6865 2066 6964 2028 652e 672e 2073   the fid (e.g. s
+00011760: 6861 7065 6669 6c65 292c 2073 6f20 7468  hapefile), so th
+00011770: 6579 0a20 2020 2020 2020 2020 2020 2077  ey.            w
+00011780: 696c 6c20 6e65 7665 7220 6265 2061 626c  ill never be abl
+00011790: 6520 746f 2070 7265 7365 7276 6520 6669  e to preserve fi
+000117a0: 6473 2e20 4465 6661 756c 7473 2074 6f20  ds. Defaults to 
+000117b0: 4e6f 6e65 2e0a 2020 2020 2020 2020 6f70  None..        op
+000117c0: 7469 6f6e 7320 2864 6963 742c 206f 7074  tions (dict, opt
+000117d0: 696f 6e61 6c29 3a20 6f70 7469 6f6e 7320  ional): options 
+000117e0: 746f 2070 6173 7320 746f 2067 6461 6c2e  to pass to gdal.
+000117f0: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
+00011800: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+00011810: 3a20 616e 2069 6e76 616c 6964 2070 6172  : an invalid par
+00011820: 616d 6574 6572 2076 616c 7565 2077 6173  ameter value was
+00011830: 2070 6173 7365 642e 0a20 2020 2020 2020   passed..       
+00011840: 2052 756e 7469 6d65 4572 726f 723a 2074   RuntimeError: t
+00011850: 696d 656f 7574 2077 6173 2072 6561 6368  imeout was reach
+00011860: 6564 2077 6869 6c65 2074 7279 696e 6720  ed while trying 
+00011870: 746f 2061 7070 656e 6420 6461 7461 2074  to append data t
+00011880: 6f20 7061 7468 2e0a 2020 2020 2222 220a  o path..    """.
+00011890: 2020 2020 2320 4368 6563 6b2f 636c 6561      # Check/clea
+000118a0: 6e20 696e 7075 7420 7061 7261 6d73 0a20  n input params. 
+000118b0: 2020 2073 7263 203d 2050 6174 6828 7372     src = Path(sr
+000118c0: 6329 0a20 2020 2064 7374 203d 2050 6174  c).    dst = Pat
+000118d0: 6828 6473 7429 0a20 2020 2069 6620 666f  h(dst).    if fo
+000118e0: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
+000118f0: 7472 7974 7970 6520 6973 206e 6f74 204e  trytype is not N
+00011900: 6f6e 653a 0a20 2020 2020 2020 2066 6f72  one:.        for
+00011910: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
+00011920: 7279 7479 7065 203d 2047 656f 6d65 7472  rytype = Geometr
+00011930: 7954 7970 6528 666f 7263 655f 6f75 7470  yType(force_outp
+00011940: 7574 5f67 656f 6d65 7472 7974 7970 6529  ut_geometrytype)
+00011950: 0a0a 2020 2020 2320 4669 6c65 7320 646f  ..    # Files do
+00011960: 6e27 7420 7479 7069 6361 6c6c 7920 7375  n't typically su
+00011970: 7070 6f72 7420 6861 7669 6e67 206d 756c  pport having mul
+00011980: 7469 706c 6520 7072 6f63 6573 7365 7320  tiple processes 
+00011990: 7772 6974 696e 670a 2020 2020 2320 7369  writing.    # si
+000119a0: 6d75 6c74 616e 6f75 736c 7920 746f 2074  multanously to t
+000119b0: 6865 6d2c 2073 6f20 7573 6520 6c6f 636b  hem, so use lock
+000119c0: 2066 696c 6520 746f 2073 796e 6368 726f   file to synchro
+000119d0: 6e69 7a65 2061 6363 6573 732e 0a20 2020  nize access..   
+000119e0: 206c 6f63 6b66 696c 6520 3d20 5061 7468   lockfile = Path
+000119f0: 2866 227b 7374 7228 6473 7429 7d2e 6c6f  (f"{str(dst)}.lo
+00011a00: 636b 2229 0a0a 2020 2020 2320 4966 2074  ck")..    # If t
+00011a10: 6865 2064 6573 7469 6e61 7469 6f6e 2066  he destination f
+00011a20: 696c 6520 646f 6573 6e27 7420 6578 6973  ile doesn't exis
+00011a30: 7420 7965 742c 2062 7574 2074 6865 206c  t yet, but the l
+00011a40: 6f63 6b66 696c 6520 646f 6573 2c0a 2020  ockfile does,.  
+00011a50: 2020 2320 7472 7920 7265 6d6f 7669 6e67    # try removing
+00011a60: 2074 6865 206c 6f63 6b66 696c 6520 6173   the lockfile as
+00011a70: 2069 7420 6d69 6768 7420 6265 2061 2067   it might be a g
+00011a80: 686f 7374 206c 6f63 6b66 696c 652e 0a20  host lockfile.. 
+00011a90: 2020 2069 6620 6e6f 7420 6473 742e 6578     if not dst.ex
+00011aa0: 6973 7473 2829 2061 6e64 206c 6f63 6b66  ists() and lockf
+00011ab0: 696c 652e 6578 6973 7473 2829 3a0a 2020  ile.exists():.  
+00011ac0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00011ad0: 2020 2020 2020 206c 6f63 6b66 696c 652e         lockfile.
+00011ae0: 756e 6c69 6e6b 2829 0a20 2020 2020 2020  unlink().       
+00011af0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00011b00: 6e3a 0a20 2020 2020 2020 2020 2020 205f  n:.            _
+00011b10: 203d 204e 6f6e 650a 0a20 2020 2023 2043   = None..    # C
+00011b20: 7265 6174 696e 6720 6c6f 636b 6669 6c65  reating lockfile
+00011b30: 2061 6e64 2061 7070 656e 640a 2020 2020   and append.    
+00011b40: 7374 6172 745f 7469 6d65 203d 2064 6174  start_time = dat
+00011b50: 6574 696d 652e 6461 7465 7469 6d65 2e6e  etime.datetime.n
+00011b60: 6f77 2829 0a20 2020 2072 6561 6479 203d  ow().    ready =
+00011b70: 2046 616c 7365 0a20 2020 2077 6869 6c65   False.    while
+00011b80: 206e 6f74 2072 6561 6479 3a0a 2020 2020   not ready:.    
+00011b90: 2020 2020 6966 205f 696f 5f75 7469 6c2e      if _io_util.
+00011ba0: 6372 6561 7465 5f66 696c 655f 6174 6f6d  create_file_atom
+00011bb0: 6963 286c 6f63 6b66 696c 6529 2069 7320  ic(lockfile) is 
+00011bc0: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
+00011bd0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00011be0: 2020 2020 2020 2023 2061 7070 656e 640a         # append.
+00011bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c00: 5f61 7070 656e 645f 746f 5f6e 6f6c 6f63  _append_to_noloc
+00011c10: 6b28 0a20 2020 2020 2020 2020 2020 2020  k(.             
+00011c20: 2020 2020 2020 2073 7263 3d73 7263 2c0a         src=src,.
+00011c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c40: 2020 2020 6473 743d 6473 742c 0a20 2020      dst=dst,.   
+00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c60: 2073 7263 5f6c 6179 6572 3d73 7263 5f6c   src_layer=src_l
+00011c70: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+00011c80: 2020 2020 2020 2020 2020 6473 745f 6c61            dst_la
+00011c90: 7965 723d 6473 745f 6c61 7965 722c 0a20  yer=dst_layer,. 
+00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cb0: 2020 2073 7263 5f63 7273 3d73 7263 5f63     src_crs=src_c
+00011cc0: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+00011cd0: 2020 2020 2020 2020 6473 745f 6372 733d          dst_crs=
+00011ce0: 6473 745f 6372 732c 0a20 2020 2020 2020  dst_crs,.       
+00011cf0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+00011d00: 726f 6a65 6374 3d72 6570 726f 6a65 6374  roject=reproject
+00011d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011d20: 2020 2020 2020 6578 706c 6f64 6563 6f6c        explodecol
+00011d30: 6c65 6374 696f 6e73 3d65 7870 6c6f 6465  lections=explode
+00011d40: 636f 6c6c 6563 7469 6f6e 732c 0a20 2020  collections,.   
+00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d60: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
+00011d70: 6f6d 6574 7279 7479 7065 3d66 6f72 6365  ometrytype=force
+00011d80: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+00011d90: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
+00011da0: 2020 2020 2020 2020 2020 6372 6561 7465            create
+00011db0: 5f73 7061 7469 616c 5f69 6e64 6578 3d63  _spatial_index=c
+00011dc0: 7265 6174 655f 7370 6174 6961 6c5f 696e  reate_spatial_in
+00011dd0: 6465 782c 0a20 2020 2020 2020 2020 2020  dex,.           
+00011de0: 2020 2020 2020 2020 2074 7261 6e73 6163           transac
+00011df0: 7469 6f6e 5f73 697a 653d 7472 616e 7361  tion_size=transa
+00011e00: 6374 696f 6e5f 7369 7a65 2c0a 2020 2020  ction_size,.    
+00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e20: 7072 6573 6572 7665 5f66 6964 3d70 7265  preserve_fid=pre
+00011e30: 7365 7276 655f 6669 642c 0a20 2020 2020  serve_fid,.     
+00011e40: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00011e50: 7074 696f 6e73 3d6f 7074 696f 6e73 2c0a  ptions=options,.
+00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e70: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
+00011e80: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+00011e90: 2020 2020 2020 2072 6561 6479 203d 2054         ready = T
+00011ea0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+00011eb0: 2020 2020 6c6f 636b 6669 6c65 2e75 6e6c      lockfile.unl
+00011ec0: 696e 6b28 290a 2020 2020 2020 2020 656c  ink().        el
+00011ed0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00011ee0: 7469 6d65 5f77 6169 7469 6e67 203d 2028  time_waiting = (
+00011ef0: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
+00011f00: 652e 6e6f 7728 2920 2d20 7374 6172 745f  e.now() - start_
+00011f10: 7469 6d65 292e 746f 7461 6c5f 7365 636f  time).total_seco
+00011f20: 6e64 7328 290a 2020 2020 2020 2020 2020  nds().          
+00011f30: 2020 6966 2074 696d 655f 7761 6974 696e    if time_waitin
+00011f40: 6720 3e20 6170 7065 6e64 5f74 696d 656f  g > append_timeo
+00011f50: 7574 5f73 3a0a 2020 2020 2020 2020 2020  ut_s:.          
+00011f60: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
+00011f70: 696d 6545 7272 6f72 280a 2020 2020 2020  imeError(.      
+00011f80: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00011f90: 6170 7065 6e64 5f74 6f20 7469 6d65 6f75  append_to timeou
+00011fa0: 7420 6f66 207b 6170 7065 6e64 5f74 696d  t of {append_tim
+00011fb0: 656f 7574 5f73 7d20 7265 6163 6865 642c  eout_s} reached,
+00011fc0: 2073 6f20 7374 6f70 2077 7269 7465 2022   so stop write "
+00011fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011fe0: 2020 2020 2066 2274 6f20 7b64 7374 7d21       f"to {dst}!
+00011ff0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012000: 2020 290a 0a20 2020 2020 2020 2023 2053    )..        # S
+00012010: 6c65 6570 2066 6f72 2061 2073 6563 6f6e  leep for a secon
+00012020: 6420 6265 666f 7265 2074 7279 696e 6720  d before trying 
+00012030: 6167 6169 6e0a 2020 2020 2020 2020 7469  again.        ti
+00012040: 6d65 2e73 6c65 6570 2831 290a 0a0a 6465  me.sleep(1)...de
+00012050: 6620 5f61 7070 656e 645f 746f 5f6e 6f6c  f _append_to_nol
+00012060: 6f63 6b28 0a20 2020 2073 7263 3a20 5061  ock(.    src: Pa
+00012070: 7468 2c0a 2020 2020 6473 743a 2050 6174  th,.    dst: Pat
+00012080: 682c 0a20 2020 2073 7263 5f6c 6179 6572  h,.    src_layer
+00012090: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000120a0: 3d20 4e6f 6e65 2c0a 2020 2020 6473 745f  = None,.    dst_
+000120b0: 6c61 7965 723a 204f 7074 696f 6e61 6c5b  layer: Optional[
+000120c0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000120d0: 2073 7263 5f63 7273 3a20 556e 696f 6e5b   src_crs: Union[
+000120e0: 696e 742c 2073 7472 2c20 4e6f 6e65 5d20  int, str, None] 
+000120f0: 3d20 4e6f 6e65 2c0a 2020 2020 6473 745f  = None,.    dst_
+00012100: 6372 733a 2055 6e69 6f6e 5b69 6e74 2c20  crs: Union[int, 
+00012110: 7374 722c 204e 6f6e 655d 203d 204e 6f6e  str, None] = Non
+00012120: 652c 0a20 2020 2072 6570 726f 6a65 6374  e,.    reproject
+00012130: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00012140: 2020 2020 6578 706c 6f64 6563 6f6c 6c65      explodecolle
+00012150: 6374 696f 6e73 3a20 626f 6f6c 203d 2046  ctions: bool = F
+00012160: 616c 7365 2c0a 2020 2020 6372 6561 7465  alse,.    create
+00012170: 5f73 7061 7469 616c 5f69 6e64 6578 3a20  _spatial_index: 
+00012180: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00012190: 2054 7275 652c 0a20 2020 2066 6f72 6365   True,.    force
+000121a0: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+000121b0: 7479 7065 3a20 556e 696f 6e5b 4765 6f6d  type: Union[Geom
+000121c0: 6574 7279 5479 7065 2c20 7374 722c 204e  etryType, str, N
+000121d0: 6f6e 655d 203d 204e 6f6e 652c 0a20 2020  one] = None,.   
+000121e0: 2074 7261 6e73 6163 7469 6f6e 5f73 697a   transaction_siz
+000121f0: 653a 2069 6e74 203d 2035 3030 3030 2c0a  e: int = 50000,.
+00012200: 2020 2020 7072 6573 6572 7665 5f66 6964      preserve_fid
+00012210: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+00012220: 203d 204e 6f6e 652c 0a20 2020 206f 7074   = None,.    opt
+00012230: 696f 6e73 3a20 6469 6374 203d 207b 7d2c  ions: dict = {},
+00012240: 0a29 3a0a 2020 2020 2320 4368 6563 6b2f  .):.    # Check/
+00012250: 636c 6561 6e20 696e 7075 7420 7061 7261  clean input para
+00012260: 6d73 0a20 2020 206f 7074 696f 6e73 203d  ms.    options =
+00012270: 205f 6f67 725f 7574 696c 2e5f 7072 6570   _ogr_util._prep
+00012280: 6172 655f 6764 616c 5f6f 7074 696f 6e73  are_gdal_options
+00012290: 286f 7074 696f 6e73 290a 2020 2020 6966  (options).    if
+000122a0: 2028 0a20 2020 2020 2020 2063 7265 6174   (.        creat
+000122b0: 655f 7370 6174 6961 6c5f 696e 6465 7820  e_spatial_index 
+000122c0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+000122d0: 2020 2020 616e 6420 224c 4159 4552 5f43      and "LAYER_C
+000122e0: 5245 4154 494f 4e2e 5350 4154 4941 4c5f  REATION.SPATIAL_
+000122f0: 494e 4445 5822 206e 6f74 2069 6e20 6f70  INDEX" not in op
+00012300: 7469 6f6e 730a 2020 2020 293a 0a20 2020  tions.    ):.   
+00012310: 2020 2020 206f 7074 696f 6e73 5b22 4c41       options["LA
+00012320: 5945 525f 4352 4541 5449 4f4e 2e53 5041  YER_CREATION.SPA
+00012330: 5449 414c 5f49 4e44 4558 225d 203d 2063  TIAL_INDEX"] = c
+00012340: 7265 6174 655f 7370 6174 6961 6c5f 696e  reate_spatial_in
+00012350: 6465 780a 0a20 2020 2023 2057 6865 6e20  dex..    # When 
+00012360: 6372 6561 7469 6e67 2f61 7070 656e 6469  creating/appendi
+00012370: 6e67 2074 6f20 6120 7368 6170 6566 696c  ng to a shapefil
+00012380: 652c 206c 6175 6e64 6572 2074 6865 2063  e, launder the c
+00012390: 6f6c 756d 6e73 206e 616d 6573 2076 6961  olumns names via
+000123a0: 0a20 2020 2023 2061 2073 716c 2073 7461  .    # a sql sta
+000123b0: 7465 6d65 6e74 2c20 6f74 6865 7277 6973  tement, otherwis
+000123c0: 6520 7768 656e 2061 7070 656e 6469 6e67  e when appending
+000123d0: 2074 6865 206c 6175 6e64 6572 6564 2063   the laundered c
+000123e0: 6f6c 756d 6e73 2077 696c 6c0a 2020 2020  olumns will.    
+000123f0: 2320 6765 7420 4e55 4c4c 2076 616c 7565  # get NULL value
+00012400: 7320 696e 7374 6561 6420 6f66 2074 6865  s instead of the
+00012410: 2064 6174 612e 0a20 2020 2073 716c 5f73   data..    sql_s
+00012420: 746d 7420 3d20 4e6f 6e65 0a20 2020 2073  tmt = None.    s
+00012430: 7263 5f6c 6179 6572 696e 666f 203d 204e  rc_layerinfo = N
+00012440: 6f6e 650a 2020 2020 6966 2064 7374 2e73  one.    if dst.s
+00012450: 7566 6669 782e 6c6f 7765 7228 2920 3d3d  uffix.lower() ==
+00012460: 2022 2e73 6870 223a 0a20 2020 2020 2020   ".shp":.       
+00012470: 2073 7263 5f6c 6179 6572 696e 666f 203d   src_layerinfo =
+00012480: 2067 6574 5f6c 6179 6572 696e 666f 2873   get_layerinfo(s
+00012490: 7263 2c20 7372 635f 6c61 7965 7229 0a20  rc, src_layer). 
+000124a0: 2020 2020 2020 2073 7263 5f63 6f6c 756d         src_colum
+000124b0: 6e73 203d 2073 7263 5f6c 6179 6572 696e  ns = src_layerin
+000124c0: 666f 2e63 6f6c 756d 6e73 0a20 2020 2020  fo.columns.     
+000124d0: 2020 2063 6f6c 756d 6e73 5f6c 6175 6e64     columns_laund
+000124e0: 6572 6564 203d 205f 6c61 756e 6465 725f  ered = _launder_
+000124f0: 636f 6c75 6d6e 5f6e 616d 6573 2873 7263  column_names(src
+00012500: 5f63 6f6c 756d 6e73 290a 2020 2020 2020  _columns).      
+00012510: 2020 636f 6c75 6d6e 735f 616c 6961 7365    columns_aliase
+00012520: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
+00012530: 2020 6627 227b 636f 6c75 6d6e 7d22 2041    f'"{column}" A
+00012540: 5320 227b 6c61 756e 6465 7265 647d 2227  S "{laundered}"'
+00012550: 2066 6f72 2063 6f6c 756d 6e2c 206c 6175   for column, lau
+00012560: 6e64 6572 6564 2069 6e20 636f 6c75 6d6e  ndered in column
+00012570: 735f 6c61 756e 6465 7265 640a 2020 2020  s_laundered.    
+00012580: 2020 2020 5d0a 2020 2020 2020 2020 6c61      ].        la
+00012590: 7965 7220 3d20 7372 635f 6c61 7965 7220  yer = src_layer 
+000125a0: 6966 2073 7263 5f6c 6179 6572 2069 7320  if src_layer is 
+000125b0: 6e6f 7420 4e6f 6e65 2065 6c73 6520 6765  not None else ge
+000125c0: 745f 6f6e 6c79 5f6c 6179 6572 2873 7263  t_only_layer(src
+000125d0: 290a 2020 2020 2020 2020 7371 6c5f 7374  ).        sql_st
+000125e0: 6d74 203d 2066 2753 454c 4543 5420 7b22  mt = f'SELECT {"
+000125f0: 2c20 222e 6a6f 696e 2863 6f6c 756d 6e73  , ".join(columns
+00012600: 5f61 6c69 6173 6564 297d 2046 524f 4d20  _aliased)} FROM 
+00012610: 227b 6c61 7965 727d 2227 0a0a 2020 2020  "{layer}"'..    
+00012620: 2320 5768 656e 2064 7374 2066 696c 6520  # When dst file 
+00012630: 646f 6573 6e27 7420 6578 6973 7420 616e  doesn't exist an
+00012640: 6420 7372 6320 6973 2065 6d70 7479 2066  d src is empty f
+00012650: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
+00012660: 6574 7279 7479 7065 2073 686f 756c 6420  etrytype should 
+00012670: 6265 0a20 2020 2023 2073 7065 6369 6669  be.    # specifi
+00012680: 6564 2c20 6f74 6865 7277 6973 6520 696e  ed, otherwise in
+00012690: 7661 6c69 6420 6f75 7470 7574 2e0a 2020  valid output..  
+000126a0: 2020 6966 2066 6f72 6365 5f6f 7574 7075    if force_outpu
+000126b0: 745f 6765 6f6d 6574 7279 7479 7065 2069  t_geometrytype i
+000126c0: 7320 4e6f 6e65 2061 6e64 206e 6f74 2064  s None and not d
+000126d0: 7374 2e65 7869 7374 7328 293a 0a20 2020  st.exists():.   
+000126e0: 2020 2020 2069 6620 7372 635f 6c61 7965       if src_laye
+000126f0: 7269 6e66 6f20 6973 204e 6f6e 653a 0a20  rinfo is None:. 
+00012700: 2020 2020 2020 2020 2020 2073 7263 5f6c             src_l
+00012710: 6179 6572 696e 666f 203d 2067 6574 5f6c  ayerinfo = get_l
+00012720: 6179 6572 696e 666f 2873 7263 2c20 7372  ayerinfo(src, sr
+00012730: 635f 6c61 7965 7229 0a20 2020 2020 2020  c_layer).       
+00012740: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
+00012750: 6f6d 6574 7279 7479 7065 203d 2073 7263  ometrytype = src
+00012760: 5f6c 6179 6572 696e 666f 2e67 656f 6d65  _layerinfo.geome
+00012770: 7472 7974 7970 650a 0a20 2020 2023 2047  trytype..    # G
+00012780: 6f21 0a20 2020 2074 7261 6e73 6c61 7465  o!.    translate
+00012790: 5f69 6e66 6f20 3d20 5f6f 6772 5f75 7469  _info = _ogr_uti
+000127a0: 6c2e 5665 6374 6f72 5472 616e 736c 6174  l.VectorTranslat
+000127b0: 6549 6e66 6f28 0a20 2020 2020 2020 2069  eInfo(.        i
+000127c0: 6e70 7574 5f70 6174 683d 7372 632c 0a20  nput_path=src,. 
+000127d0: 2020 2020 2020 206f 7574 7075 745f 7061         output_pa
+000127e0: 7468 3d64 7374 2c0a 2020 2020 2020 2020  th=dst,.        
+000127f0: 696e 7075 745f 6c61 7965 7273 3d73 7263  input_layers=src
+00012800: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+00012810: 6f75 7470 7574 5f6c 6179 6572 3d64 7374  output_layer=dst
+00012820: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+00012830: 696e 7075 745f 7372 733d 7372 635f 6372  input_srs=src_cr
+00012840: 732c 0a20 2020 2020 2020 206f 7574 7075  s,.        outpu
+00012850: 745f 7372 733d 6473 745f 6372 732c 0a20  t_srs=dst_crs,. 
+00012860: 2020 2020 2020 2073 716c 5f73 746d 743d         sql_stmt=
+00012870: 7371 6c5f 7374 6d74 2c0a 2020 2020 2020  sql_stmt,.      
+00012880: 2020 7371 6c5f 6469 616c 6563 743d 224f    sql_dialect="O
+00012890: 4752 5351 4c22 2c0a 2020 2020 2020 2020  GRSQL",.        
+000128a0: 7265 7072 6f6a 6563 743d 7265 7072 6f6a  reproject=reproj
+000128b0: 6563 742c 0a20 2020 2020 2020 2074 7261  ect,.        tra
+000128c0: 6e73 6163 7469 6f6e 5f73 697a 653d 7472  nsaction_size=tr
+000128d0: 616e 7361 6374 696f 6e5f 7369 7a65 2c0a  ansaction_size,.
+000128e0: 2020 2020 2020 2020 6170 7065 6e64 3d54          append=T
+000128f0: 7275 652c 0a20 2020 2020 2020 2075 7064  rue,.        upd
+00012900: 6174 653d 5472 7565 2c0a 2020 2020 2020  ate=True,.      
+00012910: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
+00012920: 696f 6e73 3d65 7870 6c6f 6465 636f 6c6c  ions=explodecoll
+00012930: 6563 7469 6f6e 732c 0a20 2020 2020 2020  ections,.       
+00012940: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
+00012950: 6f6d 6574 7279 7479 7065 3d66 6f72 6365  ometrytype=force
+00012960: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+00012970: 7479 7065 2c0a 2020 2020 2020 2020 6f70  type,.        op
+00012980: 7469 6f6e 733d 6f70 7469 6f6e 732c 0a20  tions=options,. 
+00012990: 2020 2020 2020 2070 7265 7365 7276 655f         preserve_
+000129a0: 6669 643d 7072 6573 6572 7665 5f66 6964  fid=preserve_fid
+000129b0: 2c0a 2020 2020 290a 2020 2020 5f6f 6772  ,.    ).    _ogr
+000129c0: 5f75 7469 6c2e 7665 6374 6f72 5f74 7261  _util.vector_tra
+000129d0: 6e73 6c61 7465 5f62 795f 696e 666f 2869  nslate_by_info(i
+000129e0: 6e66 6f3d 7472 616e 736c 6174 655f 696e  nfo=translate_in
+000129f0: 666f 290a 0a0a 6465 6620 636f 6e76 6572  fo)...def conver
+00012a00: 7428 0a20 2020 2073 7263 3a20 556e 696f  t(.    src: Unio
+00012a10: 6e5b 7374 722c 2022 6f73 2e50 6174 684c  n[str, "os.PathL
+00012a20: 696b 655b 416e 795d 225d 2c0a 2020 2020  ike[Any]"],.    
+00012a30: 6473 743a 2055 6e69 6f6e 5b73 7472 2c20  dst: Union[str, 
+00012a40: 226f 732e 5061 7468 4c69 6b65 5b41 6e79  "os.PathLike[Any
+00012a50: 5d22 5d2c 0a20 2020 2073 7263 5f6c 6179  ]"],.    src_lay
+00012a60: 6572 3a20 4f70 7469 6f6e 616c 5b73 7472  er: Optional[str
+00012a70: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6473  ] = None,.    ds
+00012a80: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
+00012a90: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00012aa0: 2020 2073 7263 5f63 7273 3a20 556e 696f     src_crs: Unio
+00012ab0: 6e5b 7374 722c 2069 6e74 2c20 4e6f 6e65  n[str, int, None
+00012ac0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6473  ] = None,.    ds
+00012ad0: 745f 6372 733a 2055 6e69 6f6e 5b73 7472  t_crs: Union[str
+00012ae0: 2c20 696e 742c 204e 6f6e 655d 203d 204e  , int, None] = N
+00012af0: 6f6e 652c 0a20 2020 2072 6570 726f 6a65  one,.    reproje
+00012b00: 6374 3a20 626f 6f6c 203d 2046 616c 7365  ct: bool = False
+00012b10: 2c0a 2020 2020 6578 706c 6f64 6563 6f6c  ,.    explodecol
+00012b20: 6c65 6374 696f 6e73 3a20 626f 6f6c 203d  lections: bool =
+00012b30: 2046 616c 7365 2c0a 2020 2020 666f 7263   False,.    forc
+00012b40: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
+00012b50: 7974 7970 653a 2055 6e69 6f6e 5b47 656f  ytype: Union[Geo
+00012b60: 6d65 7472 7954 7970 652c 2073 7472 2c20  metryType, str, 
+00012b70: 4e6f 6e65 5d20 3d20 4e6f 6e65 2c0a 2020  None] = None,.  
+00012b80: 2020 6372 6561 7465 5f73 7061 7469 616c    create_spatial
+00012b90: 5f69 6e64 6578 3a20 4f70 7469 6f6e 616c  _index: Optional
+00012ba0: 5b62 6f6f 6c5d 203d 2054 7275 652c 0a20  [bool] = True,. 
+00012bb0: 2020 2070 7265 7365 7276 655f 6669 643a     preserve_fid:
+00012bc0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00012bd0: 3d20 4e6f 6e65 2c0a 2020 2020 6f70 7469  = None,.    opti
+00012be0: 6f6e 733a 2064 6963 7420 3d20 7b7d 2c0a  ons: dict = {},.
+00012bf0: 2020 2020 6170 7065 6e64 3a20 626f 6f6c      append: bool
+00012c00: 203d 2046 616c 7365 2c0a 2020 2020 666f   = False,.    fo
+00012c10: 7263 653a 2062 6f6f 6c20 3d20 4661 6c73  rce: bool = Fals
+00012c20: 652c 0a29 3a0a 2020 2020 2222 220a 2020  e,.):.    """.  
+00012c30: 2020 5265 6164 2061 206c 6179 6572 2066    Read a layer f
+00012c40: 726f 6d20 6120 736f 7572 6365 2066 696c  rom a source fil
+00012c50: 6520 616e 6420 7772 6974 6520 6974 2074  e and write it t
+00012c60: 6f20 6120 6e65 7720 6465 7374 696e 6174  o a new destinat
+00012c70: 696f 6e20 6669 6c65 2e0a 0a20 2020 2054  ion file...    T
+00012c80: 7970 6963 616c 6c79 2075 7365 6420 746f  ypically used to
+00012c90: 2063 6f6e 7665 7274 2066 726f 6d20 6f6e   convert from on
+00012ca0: 6520 6669 6c65 666f 726d 6174 2074 6f20  e fileformat to 
+00012cb0: 616e 6f74 6865 7220 6f72 2074 6f20 7265  another or to re
+00012cc0: 7072 6f6a 6563 742e 0a0a 2020 2020 5468  project...    Th
+00012cd0: 6520 6f70 7469 6f6e 7320 7061 7261 6d65  e options parame
+00012ce0: 7465 7220 6361 6e20 6265 2075 7365 6420  ter can be used 
+00012cf0: 746f 2070 6173 7320 616e 7920 7479 7065  to pass any type
+00012d00: 206f 6620 6f70 7469 6f6e 7320 746f 2047   of options to G
+00012d10: 4441 4c20 696e 0a20 2020 2074 6865 2066  DAL in.    the f
+00012d20: 6f6c 6c6f 7769 6e67 2066 6f72 6d3a 0a20  ollowing form:. 
+00012d30: 2020 2020 2020 207b 2022 3c6f 7074 696f         { "<optio
+00012d40: 6e5f 7479 7065 3e2e 3c6f 7074 696f 6e5f  n_type>.<option_
+00012d50: 6e61 6d65 3e22 3a20 3c6f 7074 696f 6e5f  name>": <option_
+00012d60: 7661 6c75 653e 207d 0a0a 2020 2020 5468  value> }..    Th
+00012d70: 6520 6f70 7469 6f6e 2074 7970 6573 2063  e option types c
+00012d80: 616e 2062 6520 616e 7920 6f66 2074 6865  an be any of the
+00012d90: 2066 6f6c 6c6f 7769 6e67 3a0a 2020 2020   following:.    
+00012da0: 2020 2020 2d20 4c41 5945 525f 4352 4541      - LAYER_CREA
+00012db0: 5449 4f4e 3a20 6c61 7965 7220 6372 6561  TION: layer crea
+00012dc0: 7469 6f6e 206f 7074 696f 6e20 286c 636f  tion option (lco
+00012dd0: 290a 2020 2020 2020 2020 2d20 4441 5441  ).        - DATA
+00012de0: 5345 545f 4352 4541 5449 4f4e 3a20 6461  SET_CREATION: da
+00012df0: 7461 7365 7420 6372 6561 7469 6f6e 206f  taset creation o
+00012e00: 7074 696f 6e20 2864 7363 6f29 0a20 2020  ption (dsco).   
+00012e10: 2020 2020 202d 2049 4e50 5554 5f4f 5045       - INPUT_OPE
+00012e20: 4e3a 2069 6e70 7574 2064 6174 6173 6574  N: input dataset
+00012e30: 206f 7065 6e20 6f70 7469 6f6e 2028 6f6f   open option (oo
+00012e40: 290a 2020 2020 2020 2020 2d20 4445 5354  ).        - DEST
+00012e50: 494e 4154 494f 4e5f 4f50 454e 3a20 6465  INATION_OPEN: de
+00012e60: 7374 696e 6174 696f 6e20 6461 7461 7365  stination datase
+00012e70: 7420 6f70 656e 206f 7074 696f 6e20 2864  t open option (d
+00012e80: 6f6f 290a 2020 2020 2020 2020 2d20 434f  oo).        - CO
+00012e90: 4e46 4947 3a20 636f 6e66 6967 206f 7074  NFIG: config opt
+00012ea0: 696f 6e20 2863 6f6e 6669 6729 0a0a 2020  ion (config)..  
+00012eb0: 2020 5468 6520 6f70 7469 6f6e 7320 6361    The options ca
+00012ec0: 6e20 6265 2066 6f75 6e64 2069 6e20 7468  n be found in th
+00012ed0: 6520 5b47 4441 4c20 7665 6374 6f72 2064  e [GDAL vector d
+00012ee0: 7269 7665 7220 646f 6375 6d65 6e74 6174  river documentat
+00012ef0: 696f 6e5d 0a20 2020 2028 6874 7470 733a  ion].    (https:
+00012f00: 2f2f 6764 616c 2e6f 7267 2f64 7269 7665  //gdal.org/drive
+00012f10: 7273 2f76 6563 746f 722f 696e 6465 782e  rs/vector/index.
+00012f20: 6874 6d6c 292e 0a0a 2020 2020 4172 6773  html)...    Args
+00012f30: 3a0a 2020 2020 2020 2020 7372 6320 2850  :.        src (P
+00012f40: 6174 684c 696b 6529 3a20 5468 6520 736f  athLike): The so
+00012f50: 7572 6365 2066 696c 6520 7061 7468 2e0a  urce file path..
+00012f60: 2020 2020 2020 2020 6473 7420 2850 6174          dst (Pat
+00012f70: 684c 696b 6529 3a20 5468 6520 6465 7374  hLike): The dest
+00012f80: 696e 6174 696f 6e20 6669 6c65 2070 6174  ination file pat
+00012f90: 682e 0a20 2020 2020 2020 2073 7263 5f6c  h..        src_l
+00012fa0: 6179 6572 2028 7374 722c 206f 7074 696f  ayer (str, optio
+00012fb0: 6e61 6c29 3a20 5468 6520 736f 7572 6365  nal): The source
+00012fc0: 206c 6179 6572 2e20 4966 204e 6f6e 6520   layer. If None 
+00012fd0: 616e 6420 7468 6572 6520 6973 206f 6e6c  and there is onl
+00012fe0: 790a 2020 2020 2020 2020 2020 2020 6f6e  y.            on
+00012ff0: 6520 6c61 7965 7220 696e 2074 6865 2073  e layer in the s
+00013000: 7263 2066 696c 652c 2074 6861 7420 6c61  rc file, that la
+00013010: 7965 7220 6973 2074 616b 656e 2e20 4465  yer is taken. De
+00013020: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
+00013030: 2020 2020 2020 2020 6473 745f 6c61 7965          dst_laye
+00013040: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
+00013050: 293a 2054 6865 2064 6573 7469 6e61 7469  ): The destinati
+00013060: 6f6e 206c 6179 6572 2e20 4966 204e 6f6e  on layer. If Non
+00013070: 652c 2074 6865 2066 696c 650a 2020 2020  e, the file.    
+00013080: 2020 2020 2020 2020 7374 656d 2069 7320          stem is 
+00013090: 7461 6b65 6e20 6173 206c 6179 6572 206e  taken as layer n
+000130a0: 616d 652e 2044 6566 6175 6c74 7320 746f  ame. Defaults to
+000130b0: 204e 6f6e 652e 0a20 2020 2020 2020 2073   None..        s
+000130c0: 7263 5f63 7273 2028 556e 696f 6e5b 7374  rc_crs (Union[st
+000130d0: 722c 2069 6e74 5d2c 206f 7074 696f 6e61  r, int], optiona
+000130e0: 6c29 3a20 616e 2065 7073 6720 696e 7420  l): an epsg int 
+000130f0: 6f72 2061 6e79 7468 696e 6720 7375 7070  or anything supp
+00013100: 6f72 7465 640a 2020 2020 2020 2020 2020  orted.          
+00013110: 2020 6279 2074 6865 204f 4752 5370 6174    by the OGRSpat
+00013120: 6961 6c52 6566 6572 656e 6365 2e53 6574  ialReference.Set
+00013130: 4672 6f6d 5573 6572 496e 7075 7428 2920  FromUserInput() 
+00013140: 6361 6c6c 2c20 7768 6963 6820 696e 636c  call, which incl
+00013150: 7564 6573 0a20 2020 2020 2020 2020 2020  udes.           
+00013160: 2061 6e20 4550 5347 2073 7472 696e 6720   an EPSG string 
+00013170: 2865 672e 2022 4550 5347 3a34 3332 3622  (eg. "EPSG:4326"
+00013180: 292c 2061 2077 656c 6c20 6b6e 6f77 6e20  ), a well known 
+00013190: 7465 7874 2028 574b 5429 2043 5253 0a20  text (WKT) CRS. 
+000131a0: 2020 2020 2020 2020 2020 2064 6566 696e             defin
+000131b0: 6974 696f 6e2c 2e2e 2e20 4465 6661 756c  ition,... Defaul
+000131c0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+000131d0: 2020 2020 6473 745f 6372 7320 2855 6e69      dst_crs (Uni
+000131e0: 6f6e 5b73 7472 2c20 696e 745d 2c20 6f70  on[str, int], op
+000131f0: 7469 6f6e 616c 293a 2061 6e20 6570 7367  tional): an epsg
+00013200: 2069 6e74 206f 7220 616e 7974 6869 6e67   int or anything
+00013210: 2073 7570 706f 7274 6564 0a20 2020 2020   supported.     
+00013220: 2020 2020 2020 2062 7920 7468 6520 4f47         by the OG
+00013230: 5253 7061 7469 616c 5265 6665 7265 6e63  RSpatialReferenc
+00013240: 652e 5365 7446 726f 6d55 7365 7249 6e70  e.SetFromUserInp
+00013250: 7574 2829 2063 616c 6c2c 2077 6869 6368  ut() call, which
+00013260: 2069 6e63 6c75 6465 730a 2020 2020 2020   includes.      
+00013270: 2020 2020 2020 616e 2045 5053 4720 7374        an EPSG st
+00013280: 7269 6e67 2028 6567 2e20 2245 5053 473a  ring (eg. "EPSG:
+00013290: 3433 3236 2229 2c20 6120 7765 6c6c 206b  4326"), a well k
+000132a0: 6e6f 776e 2074 6578 7420 2857 4b54 2920  nown text (WKT) 
+000132b0: 4352 530a 2020 2020 2020 2020 2020 2020  CRS.            
+000132c0: 6465 6669 6e69 7469 6f6e 2c2e 2e2e 2044  definition,... D
+000132d0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+000132e0: 0a20 2020 2020 2020 2072 6570 726f 6a65  .        reproje
+000132f0: 6374 2028 626f 6f6c 2c20 6f70 7469 6f6e  ct (bool, option
+00013300: 616c 293a 2054 7275 6520 746f 2072 6570  al): True to rep
+00013310: 726f 6a65 6374 2077 6869 6c65 2063 6f6e  roject while con
+00013320: 7665 7274 696e 6720 7468 650a 2020 2020  verting the.    
+00013330: 2020 2020 2020 2020 6669 6c65 2e20 4465          file. De
+00013340: 6661 756c 7473 2074 6f20 4661 6c73 652e  faults to False.
+00013350: 0a20 2020 2020 2020 2065 7870 6c6f 6465  .        explode
+00013360: 636f 6c6c 6563 7469 6f6e 7320 2862 6f6f  collections (boo
+00013370: 6c2c 206f 7074 696f 6e61 6c29 3a20 5472  l, optional): Tr
+00013380: 7565 2074 6f20 6f75 7470 7574 206f 6e6c  ue to output onl
+00013390: 7920 7369 6d70 6c65 0a20 2020 2020 2020  y simple.       
+000133a0: 2020 2020 2067 656f 6d65 7472 6965 732e       geometries.
+000133b0: 2044 6566 6175 6c74 7320 746f 2046 616c   Defaults to Fal
+000133c0: 7365 2e0a 2020 2020 2020 2020 666f 7263  se..        forc
+000133d0: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
+000133e0: 7974 7970 6520 2855 6e69 6f6e 5b47 656f  ytype (Union[Geo
+000133f0: 6d65 7472 7954 7970 652c 2073 7472 5d2c  metryType, str],
+00013400: 206f 7074 696f 6e61 6c29 3a20 4765 6f6d   optional): Geom
+00013410: 6574 7279 2074 7970 652e 0a20 2020 2020  etry type..     
+00013420: 2020 2020 2020 2074 6f20 2874 7279 2074         to (try t
+00013430: 6f29 2066 6f72 6365 2074 6865 206f 7574  o) force the out
+00013440: 7075 7420 746f 2e20 4465 6661 756c 7473  put to. Defaults
+00013450: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
+00013460: 2020 6372 6561 7465 5f73 7061 7469 616c    create_spatial
+00013470: 5f69 6e64 6578 2028 626f 6f6c 2c20 6f70  _index (bool, op
+00013480: 7469 6f6e 616c 293a 2054 7275 6520 746f  tional): True to
+00013490: 2063 7265 6174 6520 6120 7370 6174 6961   create a spatia
+000134a0: 6c20 696e 6465 780a 2020 2020 2020 2020  l index.        
+000134b0: 2020 2020 6f6e 2074 6865 2064 6573 7469      on the desti
+000134c0: 6e61 7469 6f6e 2066 696c 652f 6c61 7965  nation file/laye
+000134d0: 722e 2049 6620 4e6f 6e65 2c20 7468 6520  r. If None, the 
+000134e0: 6465 6661 756c 7420 6265 6861 7669 6f75  default behaviou
+000134f0: 7220 6279 2067 6461 6c20 666f 720a 2020  r by gdal for.  
+00013500: 2020 2020 2020 2020 2020 7468 6174 2066            that f
+00013510: 696c 6520 7479 7065 2069 7320 7265 7370  ile type is resp
+00013520: 6563 7465 642e 2049 6620 7468 6520 4c41  ected. If the LA
+00013530: 5945 525f 4352 4541 5449 4f4e 2e53 5041  YER_CREATION.SPA
+00013540: 5449 414c 5f49 4e44 4558 0a20 2020 2020  TIAL_INDEX.     
+00013550: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+00013560: 2069 7320 7370 6563 6966 6965 6420 696e   is specified in
+00013570: 206f 7074 696f 6e73 2c20 6372 6561 7465   options, create
+00013580: 5f73 7061 7469 616c 5f69 6e64 6578 2069  _spatial_index i
+00013590: 7320 6967 6e6f 7265 642e 0a20 2020 2020  s ignored..     
+000135a0: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+000135b0: 746f 2054 7275 652e 0a20 2020 2020 2020  to True..       
+000135c0: 2070 7265 7365 7276 655f 6669 6420 2862   preserve_fid (b
+000135d0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+000135e0: 5472 7565 2074 6f20 6d61 6b65 2061 6e20  True to make an 
+000135f0: 6578 7472 6120 6566 666f 7274 2074 6f20  extra effort to 
+00013600: 7072 6573 6572 7665 2066 6964 2773 206f  preserve fid's o
+00013610: 660a 2020 2020 2020 2020 2020 2020 7468  f.            th
+00013620: 6520 736f 7572 6365 206c 6179 6572 2074  e source layer t
+00013630: 6f20 7468 6520 6465 7374 696e 6174 696f  o the destinatio
+00013640: 6e20 6c61 7965 722e 2046 616c 7365 206e  n layer. False n
+00013650: 6f74 2074 6f20 646f 2061 6e79 2065 6666  ot to do any eff
+00013660: 6f72 742e 204e 6f6e 650a 2020 2020 2020  ort. None.      
+00013670: 2020 2020 2020 746f 2075 7365 2074 6865        to use the
+00013680: 2064 6566 6175 6c74 2062 6568 6176 696f   default behavio
+00013690: 7572 206f 6620 6764 616c 2c20 7468 6174  ur of gdal, that
+000136a0: 2061 6c72 6561 6479 2070 7265 7365 7276   already preserv
+000136b0: 6573 2069 6e20 736f 6d65 2063 6173 6573  es in some cases
+000136c0: 2e0a 2020 2020 2020 2020 2020 2020 536f  ..            So
+000136d0: 6d65 2066 696c 6520 666f 726d 6174 7320  me file formats 
+000136e0: 646f 6e27 7420 6578 706c 6963 6974 6c79  don't explicitly
+000136f0: 2073 746f 7265 2074 6865 2066 6964 2028   store the fid (
+00013700: 652e 672e 2073 6861 7065 6669 6c65 292c  e.g. shapefile),
+00013710: 2073 6f20 7468 6579 0a20 2020 2020 2020   so they.       
+00013720: 2020 2020 2077 696c 6c20 6e65 7665 7220       will never 
+00013730: 6265 2061 626c 6520 746f 2070 7265 7365  be able to prese
+00013740: 7276 6520 6669 6473 2e20 4465 6661 756c  rve fids. Defaul
+00013750: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00013760: 2020 2020 6f70 7469 6f6e 7320 2864 6963      options (dic
+00013770: 742c 206f 7074 696f 6e61 6c29 3a20 6f70  t, optional): op
+00013780: 7469 6f6e 7320 746f 2070 6173 7320 746f  tions to pass to
+00013790: 2067 6461 6c2e 0a20 2020 2020 2020 2061   gdal..        a
+000137a0: 7070 656e 6420 2862 6f6f 6c2c 206f 7074  ppend (bool, opt
+000137b0: 696f 6e61 6c29 3a20 5472 7565 2074 6f20  ional): True to 
+000137c0: 6170 7065 6e64 2074 6f20 7468 6520 6f75  append to the ou
+000137d0: 7470 7574 2066 696c 6520 6966 2069 7420  tput file if it 
+000137e0: 6578 6973 7473 2e0a 2020 2020 2020 2020  exists..        
+000137f0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00013800: 4661 6c73 652e 0a20 2020 2020 2020 2066  False..        f
+00013810: 6f72 6365 2028 626f 6f6c 2c20 6f70 7469  orce (bool, opti
+00013820: 6f6e 616c 293a 206f 7665 7277 7269 7465  onal): overwrite
+00013830: 2065 7869 7374 696e 6720 6f75 7470 7574   existing output
+00013840: 2066 696c 6528 7329 0a20 2020 2020 2020   file(s).       
+00013850: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00013860: 2046 616c 7365 2e0a 2020 2020 2222 220a   False..    """.
+00013870: 2020 2020 2320 496e 6974 0a20 2020 2073      # Init.    s
+00013880: 7263 203d 2050 6174 6828 7372 6329 0a20  rc = Path(src). 
+00013890: 2020 2064 7374 203d 2050 6174 6828 6473     dst = Path(ds
+000138a0: 7429 0a0a 2020 2020 2320 4966 2073 6f75  t)..    # If sou
+000138b0: 7263 6520 6669 6c65 2064 6f65 736e 2774  rce file doesn't
+000138c0: 2065 7869 7374 2c20 7261 6973 6520 6572   exist, raise er
+000138d0: 726f 720a 2020 2020 6966 206e 6f74 2073  ror.    if not s
+000138e0: 7263 2e65 7869 7374 7328 293a 0a20 2020  rc.exists():.   
+000138f0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00013900: 4572 726f 7228 6622 7372 6320 6669 6c65  Error(f"src file
+00013910: 2064 6f65 736e 2774 2065 7869 7374 3a20   doesn't exist: 
+00013920: 7b73 7263 7d22 290a 2020 2020 2320 4966  {src}").    # If
+00013930: 2064 6573 7420 6669 6c65 2065 7869 7374   dest file exist
+00013940: 7320 616c 7265 6164 792c 2072 656d 6f76  s already, remov
+00013950: 6520 6974 0a20 2020 2069 6620 6e6f 7420  e it.    if not 
+00013960: 6170 7065 6e64 2061 6e64 2064 7374 2e65  append and dst.e
+00013970: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
+00013980: 2069 6620 666f 7263 6520 6973 2054 7275   if force is Tru
+00013990: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000139a0: 656d 6f76 6528 6473 7429 0a20 2020 2020  emove(dst).     
+000139b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000139c0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+000139d0: 2866 224f 7574 7075 7420 6669 6c65 2065  (f"Output file e
+000139e0: 7869 7374 7320 616c 7265 6164 792c 2073  xists already, s
+000139f0: 6f20 7374 6f70 3a20 7b64 7374 7d22 290a  o stop: {dst}").
+00013a00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013a10: 726e 0a0a 2020 2020 2320 436f 6e76 6572  rn..    # Conver
+00013a20: 740a 2020 2020 6c6f 6767 6572 2e69 6e66  t.    logger.inf
+00013a30: 6f28 6622 436f 6e76 6572 7420 7b73 7263  o(f"Convert {src
+00013a40: 7d20 746f 207b 6473 747d 2229 0a20 2020  } to {dst}").   
+00013a50: 205f 6170 7065 6e64 5f74 6f5f 6e6f 6c6f   _append_to_nolo
+00013a60: 636b 280a 2020 2020 2020 2020 7372 632c  ck(.        src,
+00013a70: 0a20 2020 2020 2020 2064 7374 2c0a 2020  .        dst,.  
+00013a80: 2020 2020 2020 7372 635f 6c61 7965 722c        src_layer,
+00013a90: 0a20 2020 2020 2020 2064 7374 5f6c 6179  .        dst_lay
+00013aa0: 6572 2c0a 2020 2020 2020 2020 7372 635f  er,.        src_
+00013ab0: 6372 733d 7372 635f 6372 732c 0a20 2020  crs=src_crs,.   
+00013ac0: 2020 2020 2064 7374 5f63 7273 3d64 7374       dst_crs=dst
+00013ad0: 5f63 7273 2c0a 2020 2020 2020 2020 7265  _crs,.        re
+00013ae0: 7072 6f6a 6563 743d 7265 7072 6f6a 6563  project=reprojec
+00013af0: 742c 0a20 2020 2020 2020 2065 7870 6c6f  t,.        explo
+00013b00: 6465 636f 6c6c 6563 7469 6f6e 733d 6578  decollections=ex
+00013b10: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
+00013b20: 2c0a 2020 2020 2020 2020 666f 7263 655f  ,.        force_
+00013b30: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
+00013b40: 7970 653d 666f 7263 655f 6f75 7470 7574  ype=force_output
+00013b50: 5f67 656f 6d65 7472 7974 7970 652c 0a20  _geometrytype,. 
+00013b60: 2020 2020 2020 2063 7265 6174 655f 7370         create_sp
+00013b70: 6174 6961 6c5f 696e 6465 783d 6372 6561  atial_index=crea
+00013b80: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
+00013b90: 2c0a 2020 2020 2020 2020 7072 6573 6572  ,.        preser
+00013ba0: 7665 5f66 6964 3d70 7265 7365 7276 655f  ve_fid=preserve_
+00013bb0: 6669 642c 0a20 2020 2020 2020 206f 7074  fid,.        opt
+00013bc0: 696f 6e73 3d6f 7074 696f 6e73 2c0a 2020  ions=options,.  
+00013bd0: 2020 290a 0a0a 6465 6620 5f6c 6175 6e64    )...def _laund
+00013be0: 6572 5f63 6f6c 756d 6e5f 6e61 6d65 7328  er_column_names(
+00013bf0: 636f 6c75 6d6e 733a 2049 7465 7261 626c  columns: Iterabl
+00013c00: 6529 202d 3e20 4c69 7374 5b54 7570 6c65  e) -> List[Tuple
+00013c10: 5b73 7472 2c20 7374 725d 5d3a 0a20 2020  [str, str]]:.   
+00013c20: 2022 2222 0a20 2020 204c 6175 6e64 6572   """.    Launder
+00013c30: 7320 7468 6520 636f 6c75 6d6e 206e 616d  s the column nam
+00013c40: 6573 2070 6173 7365 6420 746f 2063 6f6d  es passed to com
+00013c50: 706c 7920 7769 7468 2073 6861 7065 6669  ply with shapefi
+00013c60: 6c65 2072 6573 7472 6963 7469 6f6e 732e  le restrictions.
+00013c70: 0a0a 2020 2020 5261 7469 6f6e 616c 653a  ..    Rationale:
+00013c80: 206e 6f72 6d61 6c6c 7920 6764 616c 206c   normally gdal l
+00013c90: 6175 6e64 6572 7320 7468 656d 2069 6620  aunders them if 
+00013ca0: 6e65 6564 6564 2c20 6275 7420 7768 656e  needed, but when
+00013cb0: 2079 6f75 2061 7070 656e 640a 2020 2020   you append.    
+00013cc0: 6d75 6c74 6970 6c65 2066 696c 6573 2074  multiple files t
+00013cd0: 6f20 6120 7368 6170 6566 696c 6520 7769  o a shapefile wi
+00013ce0: 7468 2063 6f6c 756d 6e73 2074 6861 7420  th columns that 
+00013cf0: 6e65 6564 2074 6f20 6265 206c 6175 6e64  need to be laund
+00013d00: 6572 6564 0a20 2020 2074 6865 7920 6172  ered.    they ar
+00013d10: 6520 6e6f 7420 6d61 7463 6865 6420 616e  e not matched an
+00013d20: 6420 736f 2061 7265 2061 7070 656e 6465  d so are appende
+00013d30: 6420 7769 7468 204e 554c 4c20 7661 6c75  d with NULL valu
+00013d40: 6573 2066 6f72 2074 6865 7365 0a20 2020  es for these.   
+00013d50: 2063 6f6c 756d 6e73 2e20 4e6f 726d 616c   columns. Normal
+00013d60: 6c79 2074 6865 202d 7265 6c61 7865 6446  ly the -relaxedF
+00013d70: 6965 6c64 4e61 6d65 4d61 7463 6820 7061  ieldNameMatch pa
+00013d80: 7261 6d65 7465 7220 696e 206f 6772 326f  rameter in ogr2o
+00013d90: 6772 0a20 2020 2073 686f 756c 6420 6669  gr.    should fi
+00013da0: 7820 7468 6973 2c20 6275 7420 6974 2073  x this, but it s
+00013db0: 6565 6d73 2074 6861 7420 7468 6973 2069  eems that this i
+00013dc0: 736e 2774 2073 7570 706f 7274 6564 2066  sn't supported f
+00013dd0: 6f72 2073 6861 7065 6669 6c65 732e 0a0a  or shapefiles...
+00013de0: 2020 2020 4c61 756e 6465 7269 6e67 2069      Laundering i
+00013df0: 7320 6261 7365 6420 6f6e 2074 6869 7320  s based on this 
+00013e00: 7465 7874 2066 726f 6d20 7468 6520 6764  text from the gd
+00013e10: 616c 2073 6861 7065 6669 6c65 2064 7269  al shapefile dri
+00013e20: 7665 720a 2020 2020 646f 6375 6d65 6e74  ver.    document
+00013e30: 6174 696f 6e3a 0a0a 2020 2020 5368 6170  ation:..    Shap
+00013e40: 6566 696c 6520 6665 6174 7572 6520 6174  efile feature at
+00013e50: 7472 6962 7574 6573 2061 7265 2073 746f  tributes are sto
+00013e60: 7265 6420 696e 2061 6e20 6173 736f 6369  red in an associ
+00013e70: 6174 6564 202e 6462 6620 6669 6c65 2c20  ated .dbf file, 
+00013e80: 616e 640a 2020 2020 736f 2061 7474 7269  and.    so attri
+00013e90: 6275 7465 7320 7375 6666 6572 2061 206e  butes suffer a n
+00013ea0: 756d 6265 7220 6f66 206c 696d 6974 6174  umber of limitat
+00013eb0: 696f 6e73 3a0a 2020 2020 2d20 2020 4174  ions:.    -   At
+00013ec0: 7472 6962 7574 6520 6e61 6d65 7320 6361  tribute names ca
+00013ed0: 6e20 6f6e 6c79 2062 6520 7570 2074 6f20  n only be up to 
+00013ee0: 3130 2063 6861 7261 6374 6572 7320 6c6f  10 characters lo
+00013ef0: 6e67 2e0a 2020 2020 2020 2020 5468 6520  ng..        The 
+00013f00: 4f47 5220 5368 6170 6566 696c 6520 6472  OGR Shapefile dr
+00013f10: 6976 6572 2074 7269 6573 2074 6f20 6765  iver tries to ge
+00013f20: 6e65 7261 7465 2075 6e69 7175 6520 6669  nerate unique fi
+00013f30: 656c 640a 2020 2020 2020 2020 6e61 6d65  eld.        name
+00013f40: 732e 2053 7563 6365 7373 6976 6520 6475  s. Successive du
+00013f50: 706c 6963 6174 6520 6669 656c 6420 6e61  plicate field na
+00013f60: 6d65 732c 2069 6e63 6c75 6469 6e67 2074  mes, including t
+00013f70: 686f 7365 2063 7265 6174 6564 2062 790a  hose created by.
+00013f80: 2020 2020 2020 2020 7472 756e 6361 7469          truncati
+00013f90: 6f6e 2074 6f20 3130 2063 6861 7261 6374  on to 10 charact
+00013fa0: 6572 732c 2077 696c 6c20 6265 2074 7275  ers, will be tru
+00013fb0: 6e63 6174 6564 2074 6f20 3820 6368 6172  ncated to 8 char
+00013fc0: 6163 7465 7273 2061 6e64 0a20 2020 2020  acters and.     
+00013fd0: 2020 2061 7070 656e 6465 6420 7769 7468     appended with
+00013fe0: 2061 2073 6572 6961 6c20 6e75 6d62 6572   a serial number
+00013ff0: 2066 726f 6d20 3120 746f 2039 392e 0a0a   from 1 to 99...
+00014000: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
+00014010: 706c 653a 0a0a 2020 2020 2020 2020 2d20  ple:..        - 
+00014020: 2061 20e2 8692 2061 2c20 6120 e286 9220   a ... a, a ... 
+00014030: 615f 312c 2041 20e2 8692 2041 5f32 3b0a  a_1, A ... A_2;.
+00014040: 2020 2020 2020 2020 2d20 2061 6263 6465          -  abcde
+00014050: 6667 6869 6a6b 20e2 8692 2061 6263 6465  fghijk ... abcde
+00014060: 6667 6869 6a2c 2061 6263 6465 6667 6869  fghij, abcdefghi
+00014070: 6a6b 6c20 e286 9220 6162 6364 6566 6768  jkl ... abcdefgh
+00014080: 5f31 0a0a 2020 2020 2d20 2020 4f6e 6c79  _1..    -   Only
+00014090: 2049 6e74 6567 6572 2c20 496e 7465 6765   Integer, Intege
+000140a0: 7236 342c 2052 6561 6c2c 2053 7472 696e  r64, Real, Strin
+000140b0: 6720 616e 6420 4461 7465 2028 6e6f 7420  g and Date (not 
+000140c0: 4461 7465 5469 6d65 2c20 6a75 7374 0a20  DateTime, just. 
+000140d0: 2020 2020 2020 2079 6561 722f 6d6f 6e74         year/mont
+000140e0: 682f 6461 7929 2066 6965 6c64 2074 7970  h/day) field typ
+000140f0: 6573 2061 7265 2073 7570 706f 7274 6564  es are supported
+00014100: 2e20 5468 6520 7661 7269 6f75 7320 6c69  . The various li
+00014110: 7374 2c20 616e 640a 2020 2020 2020 2020  st, and.        
+00014120: 6269 6e61 7279 2066 6965 6c64 2074 7970  binary field typ
+00014130: 6573 2063 616e 6e6f 7420 6265 2063 7265  es cannot be cre
+00014140: 6174 6564 2e0a 2020 2020 2d20 2020 5468  ated..    -   Th
+00014150: 6520 6669 656c 6420 7769 6474 6820 616e  e field width an
+00014160: 6420 7072 6563 6973 696f 6e20 6172 6520  d precision are 
+00014170: 6469 7265 6374 6c79 2075 7365 6420 746f  directly used to
+00014180: 2065 7374 6162 6c69 7368 2073 746f 7261   establish stora
+00014190: 6765 0a20 2020 2020 2020 2073 697a 6520  ge.        size 
+000141a0: 696e 2074 6865 202e 6462 6620 6669 6c65  in the .dbf file
+000141b0: 2e20 5468 6973 206d 6561 6e73 2074 6861  . This means tha
+000141c0: 7420 7374 7269 6e67 7320 6c6f 6e67 6572  t strings longer
+000141d0: 2074 6861 6e20 7468 6520 6669 656c 640a   than the field.
+000141e0: 2020 2020 2020 2020 7769 6474 682c 206f          width, o
+000141f0: 7220 6e75 6d62 6572 7320 7468 6174 2064  r numbers that d
+00014200: 6f6e 2774 2066 6974 2069 6e74 6f20 7468  on't fit into th
+00014210: 6520 696e 6469 6361 7465 6420 6669 656c  e indicated fiel
+00014220: 6420 666f 726d 6174 2077 696c 6c0a 2020  d format will.  
+00014230: 2020 2020 2020 7375 6666 6572 2074 7275        suffer tru
+00014240: 6e63 6174 696f 6e2e 0a20 2020 202d 2020  ncation..    -  
+00014250: 2049 6e74 6567 6572 2066 6965 6c64 7320   Integer fields 
+00014260: 7769 7468 6f75 7420 616e 2065 7870 6c69  without an expli
+00014270: 6369 7420 7769 6474 6820 6172 6520 7472  cit width are tr
+00014280: 6561 7465 6420 6173 2077 6964 7468 2039  eated as width 9
+00014290: 2c20 616e 640a 2020 2020 2020 2020 6578  , and.        ex
+000142a0: 7465 6e64 6564 2074 6f20 3130 206f 7220  tended to 10 or 
+000142b0: 3131 2069 6620 6e65 6564 6564 2e0a 2020  11 if needed..  
+000142c0: 2020 2d20 2020 496e 7465 6765 7236 3420    -   Integer64 
+000142d0: 6669 656c 6473 2077 6974 686f 7574 2061  fields without a
+000142e0: 6e20 6578 706c 6963 6974 2077 6964 7468  n explicit width
+000142f0: 2061 7265 2074 7265 6174 6564 2061 7320   are treated as 
+00014300: 7769 6474 6820 3138 2c0a 2020 2020 2020  width 18,.      
+00014310: 2020 616e 6420 6578 7465 6e64 6564 2074    and extended t
+00014320: 6f20 3139 206f 7220 3230 2069 6620 6e65  o 19 or 20 if ne
+00014330: 6564 6564 2e0a 2020 2020 2d20 2020 5265  eded..    -   Re
+00014340: 616c 2028 666c 6f61 7469 6e67 2070 6f69  al (floating poi
+00014350: 6e74 2920 6669 656c 6473 2077 6974 686f  nt) fields witho
+00014360: 7574 2061 6e20 6578 706c 6963 6974 2077  ut an explicit w
+00014370: 6964 7468 2061 7265 2074 7265 6174 6564  idth are treated
+00014380: 2061 730a 2020 2020 2020 2020 7769 6474   as.        widt
+00014390: 6820 3234 2077 6974 6820 3135 2064 6563  h 24 with 15 dec
+000143a0: 696d 616c 2070 6c61 6365 7320 6f66 2070  imal places of p
+000143b0: 7265 6369 7369 6f6e 2e0a 2020 2020 2d20  recision..    - 
+000143c0: 2020 5374 7269 6e67 2066 6965 6c64 7320    String fields 
+000143d0: 7769 7468 6f75 7420 616e 2061 7373 6967  without an assig
+000143e0: 6e65 6420 7769 6474 6820 6172 6520 7472  ned width are tr
+000143f0: 6561 7465 6420 6173 2038 3020 6368 6172  eated as 80 char
+00014400: 6163 7465 7273 2e0a 0a20 2020 2041 7267  acters...    Arg
+00014410: 733a 0a20 2020 2020 2020 2063 6f6c 756d  s:.        colum
+00014420: 6e73 2028 4974 6572 6162 6c65 293a 2074  ns (Iterable): t
+00014430: 6865 2063 6f6c 756d 6e73 2074 6f20 6c61  he columns to la
+00014440: 756e 6465 722e 0a0a 2020 2020 5265 7475  under...    Retu
+00014450: 726e 733a 2061 204c 6973 7420 6f66 2074  rns: a List of t
+00014460: 7570 706c 6573 2077 6974 6820 7468 6520  upples with the 
+00014470: 6f72 6967 696e 616c 2061 6e64 206c 6175  original and lau
+00014480: 6e64 6572 6564 2063 6f6c 756d 6e20 6e61  ndered column na
+00014490: 6d65 732e 0a20 2020 2022 2222 0a20 2020  mes..    """.   
+000144a0: 206c 6175 6e64 6572 6564 203d 205b 5d0a   laundered = [].
+000144b0: 2020 2020 6c61 756e 6465 7265 645f 7570      laundered_up
+000144c0: 7065 7220 3d20 5b5d 0a20 2020 2066 6f72  per = [].    for
+000144d0: 2063 6f6c 756d 6e20 696e 2063 6f6c 756d   column in colum
+000144e0: 6e73 3a0a 2020 2020 2020 2020 2320 446f  ns:.        # Do
+000144f0: 7562 6c65 7320 696e 2063 6173 696e 6720  ubles in casing 
+00014500: 6172 6565 206e 6f74 2061 6c6c 6f77 6564  aree not allowed
+00014510: 2065 6974 6865 720a 2020 2020 2020 2020   either.        
+00014520: 6966 206c 656e 2863 6f6c 756d 6e29 203c  if len(column) <
+00014530: 3d20 3130 3a0a 2020 2020 2020 2020 2020  = 10:.          
+00014540: 2020 6966 2063 6f6c 756d 6e2e 7570 7065    if column.uppe
+00014550: 7228 2920 6e6f 7420 696e 206c 6175 6e64  r() not in laund
+00014560: 6572 6564 5f75 7070 6572 3a0a 2020 2020  ered_upper:.    
+00014570: 2020 2020 2020 2020 2020 2020 6c61 756e              laun
+00014580: 6465 7265 645f 7570 7065 722e 6170 7065  dered_upper.appe
+00014590: 6e64 2863 6f6c 756d 6e2e 7570 7065 7228  nd(column.upper(
+000145a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000145b0: 2020 206c 6175 6e64 6572 6564 2e61 7070     laundered.app
+000145c0: 656e 6428 2863 6f6c 756d 6e2c 2063 6f6c  end((column, col
+000145d0: 756d 6e29 290a 2020 2020 2020 2020 2020  umn)).          
+000145e0: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
+000145f0: 2020 2020 2020 2020 2320 4c61 756e 6465          # Launde
+00014600: 7269 6e67 2069 7320 6e65 6564 6564 0a20  ring is needed. 
+00014610: 2020 2020 2020 2063 6f6c 756d 6e5f 6c61         column_la
+00014620: 756e 6465 7265 6420 3d20 636f 6c75 6d6e  undered = column
+00014630: 5b3a 3130 5d0a 2020 2020 2020 2020 6966  [:10].        if
+00014640: 2063 6f6c 756d 6e5f 6c61 756e 6465 7265   column_laundere
+00014650: 642e 7570 7065 7228 2920 6e6f 7420 696e  d.upper() not in
+00014660: 206c 6175 6e64 6572 6564 5f75 7070 6572   laundered_upper
+00014670: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+00014680: 756e 6465 7265 645f 7570 7065 722e 6170  undered_upper.ap
+00014690: 7065 6e64 2863 6f6c 756d 6e5f 6c61 756e  pend(column_laun
+000146a0: 6465 7265 642e 7570 7065 7228 2929 0a20  dered.upper()). 
+000146b0: 2020 2020 2020 2020 2020 206c 6175 6e64             laund
+000146c0: 6572 6564 2e61 7070 656e 6428 2863 6f6c  ered.append((col
+000146d0: 756d 6e2c 2063 6f6c 756d 6e5f 6c61 756e  umn, column_laun
+000146e0: 6465 7265 6429 290a 2020 2020 2020 2020  dered)).        
+000146f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014700: 2020 2320 4a75 7374 2074 616b 696e 6720    # Just taking 
+00014710: 6669 7273 7420 3130 2063 6861 7261 6374  first 10 charact
+00014720: 6572 7320 6469 646e 2774 2068 656c 700a  ers didn't help.
+00014730: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00014740: 696e 6465 7820 696e 2072 616e 6765 2831  index in range(1
+00014750: 2c20 3130 3129 3a0a 2020 2020 2020 2020  , 101):.        
+00014760: 2020 2020 2020 2020 6966 2069 6e64 6578          if index
+00014770: 203e 3d20 3130 303a 0a20 2020 2020 2020   >= 100:.       
+00014780: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00014790: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+000147a0: 6445 7272 6f72 280a 2020 2020 2020 2020  dError(.        
+000147b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147c0: 224e 6f74 2073 7570 706f 7274 6564 2074  "Not supported t
+000147d0: 6f20 6c61 756e 6465 7220 3e20 3939 2063  o launder > 99 c
+000147e0: 6f6c 756d 6e73 2073 7461 7274 696e 6720  olumns starting 
+000147f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00014800: 2020 2020 2020 2020 2020 6622 7769 7468            f"with
+00014810: 207b 636f 6c75 6d6e 5f6c 6175 6e64 6572   {column_launder
+00014820: 6564 5b3a 385d 7d22 0a20 2020 2020 2020  ed[:8]}".       
+00014830: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00014840: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014850: 6620 696e 6465 7820 3c3d 2039 3a0a 2020  f index <= 9:.  
+00014860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014870: 2020 636f 6c75 6d6e 5f6c 6175 6e64 6572    column_launder
+00014880: 6564 203d 2066 227b 636f 6c75 6d6e 5f6c  ed = f"{column_l
+00014890: 6175 6e64 6572 6564 5b3a 385d 7d5f 7b69  aundered[:8]}_{i
+000148a0: 6e64 6578 7d22 0a20 2020 2020 2020 2020  ndex}".         
+000148b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148d0: 2063 6f6c 756d 6e5f 6c61 756e 6465 7265   column_laundere
+000148e0: 6420 3d20 6622 7b63 6f6c 756d 6e5f 6c61  d = f"{column_la
+000148f0: 756e 6465 7265 645b 3a38 5d7d 7b69 6e64  undered[:8]}{ind
+00014900: 6578 7d22 0a20 2020 2020 2020 2020 2020  ex}".           
+00014910: 2020 2020 2069 6620 636f 6c75 6d6e 5f6c       if column_l
+00014920: 6175 6e64 6572 6564 2e75 7070 6572 2829  aundered.upper()
+00014930: 206e 6f74 2069 6e20 6c61 756e 6465 7265   not in laundere
+00014940: 645f 7570 7065 723a 0a20 2020 2020 2020  d_upper:.       
+00014950: 2020 2020 2020 2020 2020 2020 206c 6175               lau
+00014960: 6e64 6572 6564 5f75 7070 6572 2e61 7070  ndered_upper.app
+00014970: 656e 6428 636f 6c75 6d6e 5f6c 6175 6e64  end(column_laund
+00014980: 6572 6564 2e75 7070 6572 2829 290a 2020  ered.upper()).  
+00014990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149a0: 2020 6c61 756e 6465 7265 642e 6170 7065    laundered.appe
+000149b0: 6e64 2828 636f 6c75 6d6e 2c20 636f 6c75  nd((column, colu
+000149c0: 6d6e 5f6c 6175 6e64 6572 6564 2929 0a20  mn_laundered)). 
+000149d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149e0: 2020 2062 7265 616b 0a0a 2020 2020 7265     break..    re
+000149f0: 7475 726e 206c 6175 6e64 6572 6564 0a    turn laundered.
```

### Comparing `geofileops-0.8.0a2/geofileops/geoops.py` & `geofileops-0.8.0a3/geofileops/geoops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/helpers/_parameter_helper.py` & `geofileops-0.8.0a3/geofileops/helpers/_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/helpers/layerstyles.py` & `geofileops-0.8.0a3/geofileops/helpers/layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_general_util.py` & `geofileops-0.8.0a3/geofileops/util/_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_geoops_gpd.py` & `geofileops-0.8.0a3/geofileops/util/_geoops_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_geoops_ogr.py` & `geofileops-0.8.0a3/geofileops/util/_geoops_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_geoops_sql.py` & `geofileops-0.8.0a3/geofileops/util/_geoops_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_io_util.py` & `geofileops-0.8.0a3/geofileops/util/_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_ogr_sql_util.py` & `geofileops-0.8.0a3/geofileops/util/_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_ogr_util.py` & `geofileops-0.8.0a3/geofileops/util/_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_processing_util.py` & `geofileops-0.8.0a3/geofileops/util/_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/_sqlite_util.py` & `geofileops-0.8.0a3/geofileops/util/_sqlite_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/geodataframe_util.py` & `geofileops-0.8.0a3/geofileops/util/geodataframe_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/geofiletype.py` & `geofileops-0.8.0a3/geofileops/util/geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/geofiletypes.csv` & `geofileops-0.8.0a3/geofileops/util/geofiletypes.csv`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/geometry_util.py` & `geofileops-0.8.0a3/geofileops/util/geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/geoseries_util.py` & `geofileops-0.8.0a3/geofileops/util/geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/grid_util.py` & `geofileops-0.8.0a3/geofileops/util/grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops/util/test.gpkg` & `geofileops-0.8.0a3/geofileops/util/test.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/geofileops.egg-info/PKG-INFO` & `geofileops-0.8.0a3/geofileops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a2
+Version: 0.8.0a3
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a2/geofileops.egg-info/SOURCES.txt` & `geofileops-0.8.0a3/geofileops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/setup.py` & `geofileops-0.8.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/BEFL-kbl.gpkg` & `geofileops-0.8.0a3/tests/data/BEFL-kbl.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/geofileops_testdata.qgz` & `geofileops-0.8.0a3/tests/data/geofileops_testdata.qgz`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/linestring-row-trees.gpkg` & `geofileops-0.8.0a3/tests/data/linestring-row-trees.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/linestring-watercourse.gpkg` & `geofileops-0.8.0a3/tests/data/linestring-watercourse.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/linestrings_hedges.gpkg` & `geofileops-0.8.0a3/tests/data/linestrings_hedges.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/point.gpkg` & `geofileops-0.8.0a3/tests/data/point.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-invalid.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-invalid.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-no-rows.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-no-rows.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-overlappingcircles-all.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-all.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-overlappingcircles-one.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-one.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-overlappingcircles-two+three.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-two+three.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-parcel.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-parcel.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-simplify-onborder-testcase.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-simplify-onborder-testcase.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-twolayers.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-twolayers.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygon-zone.gpkg` & `geofileops-0.8.0a3/tests/data/polygon-zone.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygonstyle.qml` & `geofileops-0.8.0a3/tests/data/polygonstyle.qml`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/data/polygonstyle.sld` & `geofileops-0.8.0a3/tests/data/polygonstyle.sld`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_general_util.py` & `geofileops-0.8.0a3/tests/test_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geofile.py` & `geofileops-0.8.0a3/tests/test_geofile.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,27 @@
     yield engine
     if engine_backup is None:
         del os.environ["GFO_IO_ENGINE"]
     else:
         os.environ["GFO_IO_ENGINE"] = engine_backup
 
 
+@pytest.fixture
+def points_gdf():
+    nb_points = 10
+    gdf = gpd.GeoDataFrame(
+        [
+            {"geometry": sh_geom.Point(x, y), "value1": x + y, "value2": x * y}
+            for x, y in zip(range(nb_points), range(nb_points))
+        ],
+        crs="epsg:4326",
+    )  # type: ignore
+    return gdf
+
+
 def test_add_column(tmp_path):
     test_path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path)
 
     # The area column shouldn't be in the test file yet
     layerinfo = gfo.get_layerinfo(path=test_path, layer="parcels")
     assert "AREA" not in layerinfo.columns
 
@@ -468,27 +481,33 @@
     assert gfo.is_geofile(
         test_helper.get_testfile("polygon-parcel").with_suffix(".shp")
     )
 
     assert gfo.is_geofile("/test/testje.txt") is False
 
 
+def test_listlayers_errors():
+    path = "not_existing_file.gpkg"
+    with pytest.raises(RuntimeError, match=f"listlayers error for {path}"):
+        _ = gfo.listlayers(path)
+
+
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
 def test_listlayers_one_layer(suffix):
-    # Test Geopackage with 1 layer
+    # Test with 1 layer
     src = test_helper.get_testfile("polygon-parcel", suffix=suffix)
     layers = gfo.listlayers(src)
     if suffix == ".gpkg":
         assert layers[0] == "parcels"
     else:
         assert layers[0] == src.stem
 
 
 def test_listlayers_two_layers():
-    # Test geopackage 2 layers
+    # Test geopackage with 2 layers
     src = test_helper.get_testfile("polygon-twolayers")
     layers = gfo.listlayers(src)
     assert "parcels" in layers
     assert "zones" in layers
 
 
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
@@ -546,21 +565,31 @@
 
     # Update column for rows where area > 5
     gfo.update_column(test_path, name="AreA", expression="-1", where="area > 4000")
     gdf = gfo.read_file(test_path)
     gdf_filtered = gdf[gdf["AREA"] == -1]
     assert len(gdf_filtered) == 20
 
+
+def test_update_column_error(tmp_path):
+    test_path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path)
+    layerinfo = gfo.get_layerinfo(path=test_path, layer="parcels")
+
     # Trying to update column that doesn't exist should raise ValueError
     assert "not_existing column" not in layerinfo.columns
     with pytest.raises(ValueError, match="Column .* doesn't exist in"):
         gfo.update_column(
             test_path, name="not_existing column", expression="ST_area(geom)"
         )
 
+    # Try to update column with invalid expression
+    assert "not_existing column" not in layerinfo.columns
+    with pytest.raises(RuntimeError, match="update_column error for"):
+        gfo.update_column(test_path, name="OPPERVL", expression="invalid_expression")
+
 
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
 def test_read_file(suffix, engine_setter):
     # Prepare test data
     src = test_helper.get_testfile("polygon-parcel", suffix=suffix)
 
     # Test with defaults
@@ -740,51 +769,113 @@
         # Rename non-existing column to existing columns doesn't give an error
         gfo.rename_column(test_path, "OPPERVL", "area")
         result_layerinfo = gfo.get_layerinfo(test_path)
         assert "OPPERVL" not in result_layerinfo.columns
         assert "area" in result_layerinfo.columns
 
 
-@pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
-def test_rename_layer(tmp_path, suffix):
-    test_path = test_helper.get_testfile(
-        "polygon-parcel", dst_dir=tmp_path, suffix=suffix
-    )
+def test_rename_column_unsupported(tmp_path):
+    path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path, suffix=".shp")
+    with pytest.raises(ValueError, match="rename_column is not possible for"):
+        _ = gfo.rename_column(path, column_name="abc", new_column_name="def")
 
-    if suffix == ".gpkg":
-        gfo.add_layerstyle(test_path, layer="parcels", name="stylename", qml="")
-        gfo.rename_layer(test_path, layer="parcels", new_layer="parcels_renamed")
-        layernames_renamed = gfo.listlayers(path=test_path)
-        assert layernames_renamed[0] == "parcels_renamed"
-        assert len(gfo.get_layerstyles(test_path, layer="parcels_renamed")) == 1
-    elif suffix == ".shp":
-        # Now test rename layer
-        with pytest.raises(ValueError, match="rename_layer is not possible"):
-            gfo.rename_layer(
-                test_path,
-                layer="polygons_parcels",
-                new_layer="polygons_parcels_renamed",
-            )
-            layernames_renamed = gfo.listlayers(path=test_path)
-            assert layernames_renamed[0] == "polygons_parcels_renamed"
-    else:
-        raise Exception(f"test not implemented for suffix {suffix}")
+    path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path, suffix=".fgb")
+    with pytest.raises(ValueError, match="rename_column is not implemented for"):
+        _ = gfo.rename_column(path, column_name="abc", new_column_name="def")
+
+
+def test_rename_layer(tmp_path):
+    test_path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path)
+    gfo.add_layerstyle(test_path, layer="parcels", name="stylename", qml="")
+
+    gfo.rename_layer(test_path, new_layer="parcels_renamed")
+    layernames_renamed = gfo.listlayers(path=test_path)
+    assert layernames_renamed[0] == "parcels_renamed"
+    assert len(gfo.get_layerstyles(test_path, layer="parcels_renamed")) == 1
+
+
+def test_rename_layer_unsupported(tmp_path):
+    path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path, suffix=".shp")
+    with pytest.raises(ValueError, match="rename_layer not possible for"):
+        _ = gfo.rename_layer(path, layer="layer", new_layer="new_layer")
+
+    path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path, suffix=".fgb")
+    with pytest.raises(ValueError, match="rename_layer not implemented for"):
+        _ = gfo.rename_layer(path, layer="layer", new_layer="new_layer")
 
 
 def test_execute_sql(tmp_path):
     # Prepare testfile
     test_path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path)
 
     # Test using execute_sql for creating/dropping indexes
     gfo.execute_sql(
         path=test_path, sql_stmt='CREATE INDEX idx_parcels_oidn ON "parcels"("oidn")'
     )
     gfo.execute_sql(path=test_path, sql_stmt="DROP INDEX idx_parcels_oidn")
 
 
+def test_execute_sql_invalid(tmp_path):
+    # Prepare testfile
+    test_path = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path)
+
+    # Test using execute_sql with invalid sql statement
+    with pytest.raises(RuntimeError, match="execute_sql error"):
+        gfo.execute_sql(path=test_path, sql_stmt="SELECT abc FROM cde")
+
+
+def test_fill_out_sql_placeholders():
+    path = test_helper.get_testfile("polygon-parcel")
+    layer = gfo.get_only_layer(path)
+    columns = ["UIDN", "OIDN"]
+
+    # Test the different existing placeholders
+    sql_stmt = 'SELECT {columns_to_select_str} FROM "parcels"'
+    result = fileops._fill_out_sql_placeholders(
+        path, layer=layer, sql_stmt=sql_stmt, columns=columns
+    )
+    assert result == 'SELECT ,"UIDN" "UIDN", "OIDN" "OIDN" FROM "parcels"'
+
+    sql_stmt = 'SELECT {geometrycolumn} FROM "parcels"'
+    result = fileops._fill_out_sql_placeholders(
+        path, layer=layer, sql_stmt=sql_stmt, columns=columns
+    )
+    assert result == 'SELECT geom FROM "parcels"'
+
+    sql_stmt = 'SELECT geom FROM "{input_layer}"'
+    result = fileops._fill_out_sql_placeholders(
+        path, layer=layer, sql_stmt=sql_stmt, columns=columns
+    )
+    assert result == 'SELECT geom FROM "parcels"'
+
+
+def test_fill_out_sql_placeholders_errors():
+    path = test_helper.get_testfile("polygon-parcel")
+
+    # Test invalid placeholder
+    sql_stmt = 'SELECT {invalid_placeholder} FROM "parcel"'
+    with pytest.raises(ValueError, match="unknown placeholder invalid_placeholder "):
+        fileops._fill_out_sql_placeholders(
+            path, layer="parcel", sql_stmt=sql_stmt, columns=None
+        )
+
+
+def test_spatial_index_unsupported(tmp_path):
+    path = tmp_path / "unsupported_type.unsupported"
+    path.touch()
+    with pytest.raises(ValueError, match="Unknown extension .unsupported"):
+        _ = gfo.create_spatial_index(path, "layer")
+
+    with pytest.raises(ValueError, match="Unknown extension .unsupported"):
+        _ = gfo.has_spatial_index(path, "layer")
+
+    with pytest.raises(ValueError, match="Unknown extension .unsupported"):
+        _ = gfo.remove_spatial_index(path, "layer")
+
+
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
 def test_spatial_index(tmp_path, suffix):
     test_path = test_helper.get_testfile(
         "polygon-parcel", dst_dir=tmp_path, suffix=suffix
     )
     layer = gfo.get_only_layer(test_path)
 
@@ -1029,14 +1120,181 @@
     # The result type in the geodataframe is also the same as originaly
     test_read_geometrytypes = geoseries_util.get_geometrytypes(test_read_gdf.geometry)
     assert len(test_gdf) == len(test_read_gdf)
     assert test_read_geometrytypes == test_geometrytypes
 
 
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
+def test_to_file_index(tmp_path, points_gdf, suffix, engine_setter):
+    """Strongly based on similar test in geopandas."""
+
+    class FileNumber(object):
+        def __init__(self, tmpdir, base, ext):
+            self.tmpdir = str(tmpdir)
+            self.base = base
+            self.ext = ext
+            self.fileno = 0
+
+        def __repr__(self):
+            filename = "{0}{1:02d}.{2}".format(self.base, self.fileno, self.ext)
+            return os.path.join(self.tmpdir, filename)
+
+        def __next__(self):
+            self.fileno += 1
+            return repr(self)
+
+    fngen = FileNumber(tmp_path, "check", suffix)
+
+    def do_checks(df, index_is_used):
+        # check combinations of index=None|True|False on GeoDataFrame
+        other_cols = list(df.columns)
+        other_cols.remove("geometry")
+
+        if suffix == ".shp":
+            # ESRI Shapefile will add FID if no other columns exist
+            driver_col = ["FID"]
+        else:
+            driver_col = []
+
+        if index_is_used:
+            index_cols = list(df.index.names)
+        else:
+            index_cols = [None] * len(df.index.names)
+
+        # replicate pandas' default index names for regular and MultiIndex
+        if index_cols == [None]:
+            index_cols = ["index"]
+        elif len(index_cols) > 1 and not all(index_cols):
+            for level, index_col in enumerate(index_cols):
+                if index_col is None:
+                    index_cols[level] = "level_" + str(level)  # type: ignore
+
+        # check GeoDataFrame with default index=None to autodetect
+        tempfilename = next(fngen)
+        gfo.to_file(df, tempfilename, index=None)
+        df_check = gfo.read_file(tempfilename)
+        if len(other_cols) == 0:
+            expected_cols = driver_col[:]
+        else:
+            expected_cols = []
+        if index_is_used:
+            expected_cols += index_cols
+        expected_cols += other_cols + ["geometry"]
+        assert list(df_check.columns) == expected_cols
+
+        # check GeoDataFrame with index=True
+        tempfilename = next(fngen)
+        gfo.to_file(df, tempfilename, index=True)
+        df_check = gfo.read_file(tempfilename)
+        assert list(df_check.columns) == index_cols + other_cols + ["geometry"]
+
+        # check GeoDataFrame with index=False
+        tempfilename = next(fngen)
+        gfo.to_file(df, tempfilename, index=False)
+        df_check = gfo.read_file(tempfilename)
+        if len(other_cols) == 0:
+            expected_cols = driver_col + ["geometry"]
+        else:
+            expected_cols = other_cols + ["geometry"]
+        assert list(df_check.columns) == expected_cols
+
+        return
+
+    # Checks where index is not used/saved
+    # ------------------------------------
+
+    # index is a default RangeIndex
+    p_gdf = points_gdf.copy()
+    gdf = gpd.GeoDataFrame(p_gdf["value1"], geometry=p_gdf.geometry)  # type: ignore
+    do_checks(gdf, index_is_used=False)
+
+    # index is a RangeIndex, starting from 1
+    gdf.index += 1
+    do_checks(gdf, index_is_used=False)
+
+    # index is a Int64Index regular sequence from 1
+    p_gdf.index = list(range(1, len(gdf) + 1))
+    gdf = gpd.GeoDataFrame(p_gdf["value1"], geometry=p_gdf.geometry)  # type: ignore
+    do_checks(gdf, index_is_used=False)
+
+    # index was a default RangeIndex, but delete one row to make an Int64Index
+    p_gdf = points_gdf.copy()
+    gdf = gpd.GeoDataFrame(p_gdf["value1"], geometry=p_gdf.geometry)  # type: ignore
+    gdf = gdf.drop(5, axis=0)
+    do_checks(gdf, index_is_used=False)
+
+    # no other columns (except geometry)
+    gdf = gpd.GeoDataFrame(geometry=p_gdf.geometry)  # type: ignore
+    do_checks(gdf, index_is_used=False)
+
+    # Checks where index is used/saved
+    # --------------------------------
+
+    # named index
+    p_gdf = points_gdf.copy()
+    gdf = gpd.GeoDataFrame(p_gdf["value1"], geometry=p_gdf.geometry)  # type: ignore
+    gdf.index.name = "foo_index"
+    do_checks(gdf, index_is_used=True)
+
+    # named index, same as pandas' default name after .reset_index(drop=False)
+    gdf.index.name = "index"
+    do_checks(gdf, index_is_used=True)
+
+    # named MultiIndex
+    p_gdf = points_gdf.copy()
+    p_gdf["value3"] = p_gdf["value2"] - p_gdf["value1"]
+    p_gdf.set_index(["value1", "value2"], inplace=True)
+    gdf = gpd.GeoDataFrame(p_gdf, geometry=p_gdf.geometry)  # type: ignore
+    do_checks(gdf, index_is_used=True)
+
+    # partially unnamed MultiIndex
+    gdf.index.names = ["first", None]  # type: ignore
+    do_checks(gdf, index_is_used=True)
+
+    # unnamed MultiIndex
+    gdf.index.names = [None, None]  # type: ignore
+    do_checks(gdf, index_is_used=True)
+
+    # unnamed Float64Index
+    p_gdf = points_gdf.copy()
+    gdf = gpd.GeoDataFrame(p_gdf["value1"], geometry=p_gdf.geometry)  # type: ignore
+    gdf.index = p_gdf.index.astype(float) / 10
+    do_checks(gdf, index_is_used=True)
+
+    # named Float64Index
+    gdf.index.name = "centile"
+    do_checks(gdf, index_is_used=True)
+
+    # index as string
+    p_gdf = points_gdf.copy()
+    gdf = gpd.GeoDataFrame(p_gdf["value1"], geometry=p_gdf.geometry)  # type: ignore
+    gdf.index = pd.TimedeltaIndex(range(len(gdf)), "days")  # type: ignore
+    # TODO: TimedeltaIndex is an invalid field type
+    gdf.index = gdf.index.astype(str)
+    do_checks(gdf, index_is_used=True)
+
+    # unnamed DatetimeIndex
+    p_gdf = points_gdf.copy()
+    gdf = gpd.GeoDataFrame(p_gdf["value1"], geometry=p_gdf.geometry)  # type: ignore
+    gdf.index = pd.TimedeltaIndex(
+        range(len(gdf)), "days"
+    ) + pd.DatetimeIndex(  # type: ignore
+        ["1999-12-27"] * len(gdf)
+    )
+    if suffix == ".shp":
+        # Shapefile driver does not support datetime fields
+        gdf.index = gdf.index.astype(str)
+    do_checks(gdf, index_is_used=True)
+
+    # named DatetimeIndex
+    gdf.index.name = "datetime"
+    do_checks(gdf, index_is_used=True)
+
+
+@pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
 def test_remove(tmp_path, suffix):
     # Prepare test data
     src = test_helper.get_testfile("polygon-parcel", dst_dir=tmp_path, suffix=suffix)
     assert src.exists()
 
     # Remove and check result
     gfo.remove(src)
```

### Comparing `geofileops-0.8.0a2/tests/test_geofileops_singlelayer.py` & `geofileops-0.8.0a3/tests/test_geofileops_singlelayer.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geofileops_singlelayer_gpd.py` & `geofileops-0.8.0a3/tests/test_geofileops_singlelayer_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geofileops_singlelayer_ogr.py` & `geofileops-0.8.0a3/tests/test_geofileops_singlelayer_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geofileops_singlelayer_sql.py` & `geofileops-0.8.0a3/tests/test_geofileops_singlelayer_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geofileops_twolayers.py` & `geofileops-0.8.0a3/tests/test_geofileops_twolayers.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geofiletype.py` & `geofileops-0.8.0a3/tests/test_geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geometry_util.py` & `geofileops-0.8.0a3/tests/test_geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_geoseries_util.py` & `geofileops-0.8.0a3/tests/test_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_grid_util.py` & `geofileops-0.8.0a3/tests/test_grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_helper.py` & `geofileops-0.8.0a3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_io_util.py` & `geofileops-0.8.0a3/tests/test_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_layerstyles.py` & `geofileops-0.8.0a3/tests/test_layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_ogr_sql_util.py` & `geofileops-0.8.0a3/tests/test_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_ogr_util.py` & `geofileops-0.8.0a3/tests/test_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_parameter_helper.py` & `geofileops-0.8.0a3/tests/test_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_processing_util.py` & `geofileops-0.8.0a3/tests/test_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_spatialite.py` & `geofileops-0.8.0a3/tests/test_spatialite.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a2/tests/test_sqlite_util.py` & `geofileops-0.8.0a3/tests/test_sqlite_util.py`

 * *Files identical despite different names*


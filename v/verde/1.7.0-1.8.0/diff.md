# Comparing `tmp/verde-1.7.0.tar.gz` & `tmp/verde-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verde-1.7.0.tar", last modified: Fri Mar 25 15:24:42 2022, max compression
+gzip compressed data, was "verde-1.8.0.tar", last modified: Mon May  8 20:13:36 2023, max compression
```

## Comparing `verde-1.7.0.tar` & `verde-1.8.0.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 15:24:42.206263 verde-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-03-25 15:24:30.000000 verde-1.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-03-25 15:24:30.000000 verde-1.7.0/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-03-25 15:24:30.000000 verde-1.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-03-25 15:24:30.000000 verde-1.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-03-25 15:24:30.000000 verde-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-03-25 15:24:30.000000 verde-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6305 2022-03-25 15:24:42.206263 verde-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-03-25 15:24:30.000000 verde-1.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-03-25 15:24:30.000000 verde-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-03-25 15:24:42.206263 verde-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-03-25 15:24:30.000000 verde-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 15:24:42.198263 verde-1.7.0/verde/
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-03-25 15:24:30.000000 verde-1.7.0/verde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-03-25 15:24:30.000000 verde-1.7.0/verde/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-03-25 15:24:41.000000 verde-1.7.0/verde/_version_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 15:24:42.202263 verde-1.7.0/verde/base/
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-03-25 15:24:30.000000 verde-1.7.0/verde/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33567 2022-03-25 15:24:30.000000 verde-1.7.0/verde/base/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-03-25 15:24:30.000000 verde-1.7.0/verde/base/least_squares.py
--rw-r--r--   0 runner    (1001) docker     (121)     9653 2022-03-25 15:24:30.000000 verde-1.7.0/verde/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    21918 2022-03-25 15:24:30.000000 verde-1.7.0/verde/blockreduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     4725 2022-03-25 15:24:30.000000 verde-1.7.0/verde/chain.py
--rw-r--r--   0 runner    (1001) docker     (121)    49713 2022-03-25 15:24:30.000000 verde-1.7.0/verde/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 15:24:42.202263 verde-1.7.0/verde/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-03-25 15:24:30.000000 verde-1.7.0/verde/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-03-25 15:24:30.000000 verde-1.7.0/verde/datasets/registry.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13266 2022-03-25 15:24:30.000000 verde-1.7.0/verde/datasets/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-03-25 15:24:30.000000 verde-1.7.0/verde/datasets/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-03-25 15:24:30.000000 verde-1.7.0/verde/distances.py
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-03-25 15:24:30.000000 verde-1.7.0/verde/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     9470 2022-03-25 15:24:30.000000 verde-1.7.0/verde/mask.py
--rw-r--r--   0 runner    (1001) docker     (121)    34191 2022-03-25 15:24:30.000000 verde-1.7.0/verde/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-03-25 15:24:30.000000 verde-1.7.0/verde/projections.py
--rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-03-25 15:24:30.000000 verde-1.7.0/verde/scipygridder.py
--rw-r--r--   0 runner    (1001) docker     (121)    21304 2022-03-25 15:24:30.000000 verde-1.7.0/verde/spline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-03-25 15:24:30.000000 verde-1.7.0/verde/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 15:24:42.202263 verde-1.7.0/verde/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 15:24:42.206263 verde-1.7.0/verde/tests/baseline/
--rw-r--r--   0 runner    (1001) docker     (121)    26105 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/baseline/test_setup_baja_bathymetry.png
--rw-r--r--   0 runner    (1001) docker     (121)    16819 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/baseline/test_setup_california_gps.png
--rw-r--r--   0 runner    (1001) docker     (121)    15184 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/baseline/test_setup_rio_magnetic.png
--rw-r--r--   0 runner    (1001) docker     (121)    23948 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/baseline/test_setup_texas_wind.png
--rw-r--r--   0 runner    (1001) docker     (121)    18114 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    11653 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_blockreduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (121)    10974 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     4654 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_minimal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_projections.py
--rw-r--r--   0 runner    (1001) docker     (121)     3665 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7053 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_spline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_trend.py
--rw-r--r--   0 runner    (1001) docker     (121)    12178 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5713 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-03-25 15:24:30.000000 verde-1.7.0/verde/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8732 2022-03-25 15:24:30.000000 verde-1.7.0/verde/trend.py
--rw-r--r--   0 runner    (1001) docker     (121)    26705 2022-03-25 15:24:30.000000 verde-1.7.0/verde/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    18860 2022-03-25 15:24:30.000000 verde-1.7.0/verde/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 15:24:42.198263 verde-1.7.0/verde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6305 2022-03-25 15:24:41.000000 verde-1.7.0/verde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-03-25 15:24:42.000000 verde-1.7.0/verde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-25 15:24:41.000000 verde-1.7.0/verde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-25 15:24:41.000000 verde-1.7.0/verde.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-25 15:24:41.000000 verde-1.7.0/verde.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-25 15:24:41.000000 verde-1.7.0/verde.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:13:36.892670 verde-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 20:13:18.000000 verde-1.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-08 20:13:18.000000 verde-1.8.0/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-08 20:13:18.000000 verde-1.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-08 20:13:18.000000 verde-1.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-08 20:13:18.000000 verde-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 20:13:18.000000 verde-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-08 20:13:36.892670 verde-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-08 20:13:18.000000 verde-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-08 20:13:18.000000 verde-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-08 20:13:36.892670 verde-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:13:36.884669 verde-1.8.0/verde/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-08 20:13:18.000000 verde-1.8.0/verde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-08 20:13:18.000000 verde-1.8.0/verde/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 20:13:36.000000 verde-1.8.0/verde/_version_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:13:36.888669 verde-1.8.0/verde/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 20:13:18.000000 verde-1.8.0/verde/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33549 2023-05-08 20:13:18.000000 verde-1.8.0/verde/base/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-08 20:13:18.000000 verde-1.8.0/verde/base/least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-08 20:13:18.000000 verde-1.8.0/verde/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21918 2023-05-08 20:13:18.000000 verde-1.8.0/verde/blockreduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-05-08 20:13:18.000000 verde-1.8.0/verde/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54818 2023-05-08 20:13:18.000000 verde-1.8.0/verde/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:13:36.888669 verde-1.8.0/verde/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-08 20:13:18.000000 verde-1.8.0/verde/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 20:13:18.000000 verde-1.8.0/verde/datasets/registry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-05-08 20:13:18.000000 verde-1.8.0/verde/datasets/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-08 20:13:18.000000 verde-1.8.0/verde/datasets/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-08 20:13:18.000000 verde-1.8.0/verde/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-08 20:13:18.000000 verde-1.8.0/verde/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-05-08 20:13:18.000000 verde-1.8.0/verde/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-05-08 20:13:18.000000 verde-1.8.0/verde/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-08 20:13:18.000000 verde-1.8.0/verde/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-08 20:13:18.000000 verde-1.8.0/verde/projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-05-08 20:13:18.000000 verde-1.8.0/verde/scipygridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-05-08 20:13:18.000000 verde-1.8.0/verde/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-08 20:13:18.000000 verde-1.8.0/verde/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:13:36.892670 verde-1.8.0/verde/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:13:36.892670 verde-1.8.0/verde/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    26105 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/baseline/test_setup_baja_bathymetry.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16819 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/baseline/test_setup_california_gps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/baseline/test_setup_rio_magnetic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/baseline/test_setup_texas_wind.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_blockreduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 20:13:18.000000 verde-1.8.0/verde/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-08 20:13:18.000000 verde-1.8.0/verde/trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27075 2023-05-08 20:13:18.000000 verde-1.8.0/verde/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18774 2023-05-08 20:13:18.000000 verde-1.8.0/verde/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:13:36.884669 verde-1.8.0/verde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-08 20:13:36.000000 verde-1.8.0/verde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-08 20:13:36.000000 verde-1.8.0/verde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:13:36.000000 verde-1.8.0/verde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 20:13:36.000000 verde-1.8.0/verde.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 20:13:36.000000 verde-1.8.0/verde.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:13:36.000000 verde-1.8.0/verde.egg-info/zip-safe
```

### Comparing `verde-1.7.0/CITATION.rst` & `verde-1.8.0/CITATION.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
     Uieda, L. (2018). Verde: Processing and gridding spatial data using Green's
     functions. Journal of Open Source Software, 3(29), 957. doi:10.21105/joss.00957
 
 This is an open-access publication and can be freely downloaded from
 https://doi.org/10.21105/joss.00957
 
-Here is a Bibtex entry to make things easier if you're using Latex::
+Here is a Bibtex entry to make things easier if you're using Latex:
+
+.. code:: bibtex
 
     @article{uieda2018,
       title = {{Verde}: {Processing} and gridding spatial data using {Green's} functions},
       author = {Uieda, Leonardo},
       year = {2018},
       journal = {Journal of Open Source Software},
       volume = {3},
```

### Comparing `verde-1.7.0/CONTRIBUTING.md` & `verde-1.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/LICENSE.txt` & `verde-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/PKG-INFO` & `verde-1.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,395 +1,366 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7665 7264  : 2.1.Name: verd
-00000020: 650a 5665 7273 696f 6e3a 2031 2e37 2e30  e.Version: 1.7.0
-00000030: 0a53 756d 6d61 7279 3a20 2250 726f 6365  .Summary: "Proce
-00000040: 7373 696e 6720 616e 6420 6772 6964 6469  ssing and griddi
-00000050: 6e67 2073 7061 7469 616c 2064 6174 612c  ng spatial data,
-00000060: 206d 6163 6869 6e65 2d6c 6561 726e 696e   machine-learnin
-00000070: 6720 7374 796c 6522 0a48 6f6d 652d 7061  g style".Home-pa
-00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000090: 7562 2e63 6f6d 2f66 6174 6961 6e64 6f2f  ub.com/fatiando/
-000000a0: 7665 7264 650a 4175 7468 6f72 3a20 5468  verde.Author: Th
-000000b0: 6520 5665 7264 6520 4465 7665 6c6f 7065  e Verde Develope
-000000c0: 7273 0a41 7574 686f 722d 656d 6169 6c3a  rs.Author-email:
-000000d0: 2066 6174 6961 6e64 6f61 7465 7272 6140   fatiandoaterra@
-000000e0: 7072 6f74 6f6e 6d61 696c 2e63 6f6d 0a4d  protonmail.com.M
-000000f0: 6169 6e74 6169 6e65 723a 2022 4c65 6f6e  aintainer: "Leon
-00000100: 6172 646f 2055 6965 6461 220a 4d61 696e  ardo Uieda".Main
-00000110: 7461 696e 6572 2d65 6d61 696c 3a20 6c65  tainer-email: le
-00000120: 6f75 6965 6461 4067 6d61 696c 2e63 6f6d  ouieda@gmail.com
-00000130: 0a4c 6963 656e 7365 3a20 4253 4420 332d  .License: BSD 3-
-00000140: 436c 6175 7365 204c 6963 656e 7365 0a50  Clause License.P
-00000150: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
-00000160: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
-00000170: 3a2f 2f77 7777 2e66 6174 6961 6e64 6f2e  ://www.fatiando.
-00000180: 6f72 672f 7665 7264 650a 5072 6f6a 6563  org/verde.Projec
-00000190: 742d 5552 4c3a 2052 656c 6561 7365 204e  t-URL: Release N
-000001a0: 6f74 6573 2c20 6874 7470 733a 2f2f 6769  otes, https://gi
-000001b0: 7468 7562 2e63 6f6d 2f66 6174 6961 6e64  thub.com/fatiand
-000001c0: 6f2f 7665 7264 652f 7265 6c65 6173 6573  o/verde/releases
-000001d0: 0a50 726f 6a65 6374 2d55 524c 3a20 4275  .Project-URL: Bu
-000001e0: 6720 5472 6163 6b65 722c 2068 7474 7073  g Tracker, https
-000001f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
-00000200: 7469 616e 646f 2f76 6572 6465 2f69 7373  tiando/verde/iss
-00000210: 7565 730a 5072 6f6a 6563 742d 5552 4c3a  ues.Project-URL:
-00000220: 2053 6f75 7263 6520 436f 6465 2c20 6874   Source Code, ht
-00000230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000240: 2f66 6174 6961 6e64 6f2f 7665 7264 650a  /fatiando/verde.
-00000250: 4b65 7977 6f72 6473 3a20 7370 6174 6961  Keywords: spatia
-00000260: 6c2c 6765 6f73 6369 656e 6365 2c67 656f  l,geoscience,geo
-00000270: 7068 7973 6963 732c 6772 6964 6469 6e67  physics,gridding
-00000280: 2c69 6e74 6572 706f 6c61 7469 6f6e 0a50  ,interpolation.P
-00000290: 6c61 7466 6f72 6d3a 2061 6e79 0a43 6c61  latform: any.Cla
-000002a0: 7373 6966 6965 723a 2044 6576 656c 6f70  ssifier: Develop
-000002b0: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
-000002c0: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
-000002d0: 6162 6c65 0a43 6c61 7373 6966 6965 723a  able.Classifier:
-000002e0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000002f0: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
-00000300: 7365 6172 6368 0a43 6c61 7373 6966 6965  search.Classifie
-00000310: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000320: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000330: 7273 0a43 6c61 7373 6966 6965 723a 2049  rs.Classifier: I
-00000340: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-00000350: 203a 3a20 4564 7563 6174 696f 6e0a 436c   :: Education.Cl
-00000360: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-00000370: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000380: 6420 3a3a 2042 5344 204c 6963 656e 7365  d :: BSD License
-00000390: 0a43 6c61 7373 6966 6965 723a 204e 6174  .Classifier: Nat
-000003a0: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
-000003b0: 2045 6e67 6c69 7368 0a43 6c61 7373 6966   English.Classif
-000003c0: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-000003d0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000003e0: 7065 6e64 656e 740a 436c 6173 7369 6669  pendent.Classifi
-000003f0: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
-00000400: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-00000410: 696e 670a 436c 6173 7369 6669 6572 3a20  ing.Classifier: 
-00000420: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
-00000430: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
-00000440: 204c 6962 7261 7269 6573 0a43 6c61 7373   Libraries.Class
-00000450: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000460: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000470: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-00000480: 6c79 0a43 6c61 7373 6966 6965 723a 2050  ly.Classifier: P
-00000490: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000004a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000004b0: 2033 2e36 0a43 6c61 7373 6966 6965 723a   3.6.Classifier:
-000004c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000004d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000004e0: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
-000004f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000500: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000510: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-00000520: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000530: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000540: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-00000550: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000560: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000570: 7974 686f 6e20 3a3a 2033 2e31 300a 5265  ython :: 3.10.Re
-00000580: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
-00000590: 3d33 2e36 0a44 6573 6372 6970 7469 6f6e  =3.6.Description
-000005a0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-000005b0: 6578 742f 782d 7273 740a 4c69 6365 6e73  ext/x-rst.Licens
-000005c0: 652d 4669 6c65 3a20 4c49 4345 4e53 452e  e-File: LICENSE.
-000005d0: 7478 740a 0a2e 2e20 696d 6167 653a 3a20  txt.... image:: 
-000005e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000005f0: 6f6d 2f66 6174 6961 6e64 6f2f 7665 7264  om/fatiando/verd
-00000600: 652f 7261 772f 6d61 696e 2f64 6f63 2f5f  e/raw/main/doc/_
-00000610: 7374 6174 6963 2f72 6561 646d 652d 6261  static/readme-ba
-00000620: 6e6e 6572 2e70 6e67 0a20 2020 203a 616c  nner.png.    :al
-00000630: 743a 2056 6572 6465 0a0a 6044 6f63 756d  t: Verde..`Docum
-00000640: 656e 7461 7469 6f6e 203c 6874 7470 3a2f  entation <http:/
-00000650: 2f77 7777 2e66 6174 6961 6e64 6f2e 6f72  /www.fatiando.or
-00000660: 672f 7665 7264 653e 605f 5f20 7c0a 6044  g/verde>`__ |.`D
-00000670: 6f63 756d 656e 7461 7469 6f6e 2028 6465  ocumentation (de
-00000680: 7620 7665 7273 696f 6e29 203c 6874 7470  v version) <http
-00000690: 3a2f 2f77 7777 2e66 6174 6961 6e64 6f2e  ://www.fatiando.
-000006a0: 6f72 672f 7665 7264 652f 6465 763e 605f  org/verde/dev>`_
-000006b0: 5f20 7c0a 5061 7274 206f 6620 7468 6520  _ |.Part of the 
-000006c0: 6046 6174 6961 6e64 6f20 6120 5465 7272  `Fatiando a Terr
-000006d0: 6120 3c68 7474 7073 3a2f 2f77 7777 2e66  a <https://www.f
-000006e0: 6174 6961 6e64 6f2e 6f72 673e 605f 5f20  atiando.org>`__ 
-000006f0: 7072 6f6a 6563 740a 0a0a 2e2e 2069 6d61  project..... ima
-00000700: 6765 3a3a 2068 7474 703a 2f2f 696d 672e  ge:: http://img.
-00000710: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000720: 762f 7665 7264 652e 7376 673f 7374 796c  v/verde.svg?styl
-00000730: 653d 666c 6174 2d73 7175 6172 6526 6c61  e=flat-square&la
-00000740: 6265 6c3d 7665 7273 696f 6e0a 2020 2020  bel=version.    
-00000750: 3a61 6c74 3a20 4c61 7465 7374 2076 6572  :alt: Latest ver
-00000760: 7369 6f6e 206f 6e20 5079 5049 0a20 2020  sion on PyPI.   
-00000770: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000780: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000790: 672f 7079 7069 2f76 6572 6465 0a2e 2e20  g/pypi/verde... 
-000007a0: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-000007b0: 696d 672e 7368 6965 6c64 732e 696f 2f63  img.shields.io/c
-000007c0: 6f6e 6461 2f76 6e2f 636f 6e64 612d 666f  onda/vn/conda-fo
-000007d0: 7267 652f 7665 7264 652e 7376 673f 7374  rge/verde.svg?st
-000007e0: 796c 653d 666c 6174 2d73 7175 6172 650a  yle=flat-square.
-000007f0: 2020 2020 3a61 6c74 3a20 4c61 7465 7374      :alt: Latest
-00000800: 2076 6572 7369 6f6e 206f 6e20 636f 6e64   version on cond
-00000810: 612d 666f 7267 650a 2020 2020 3a74 6172  a-forge.    :tar
-00000820: 6765 743a 2068 7474 7073 3a2f 2f67 6974  get: https://git
-00000830: 6875 622e 636f 6d2f 636f 6e64 612d 666f  hub.com/conda-fo
-00000840: 7267 652f 7665 7264 652d 6665 6564 7374  rge/verde-feedst
-00000850: 6f63 6b0a 2e2e 2069 6d61 6765 3a3a 2068  ock... image:: h
-00000860: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000870: 6473 2e69 6f2f 636f 6465 636f 762f 632f  ds.io/codecov/c/
-00000880: 6769 7468 7562 2f66 6174 6961 6e64 6f2f  github/fatiando/
-00000890: 7665 7264 652f 6d61 696e 2e73 7667 3f73  verde/main.svg?s
-000008a0: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-000008b0: 0a20 2020 203a 616c 743a 2054 6573 7420  .    :alt: Test 
-000008c0: 636f 7665 7261 6765 2073 7461 7475 730a  coverage status.
-000008d0: 2020 2020 3a74 6172 6765 743a 2068 7474      :target: htt
-000008e0: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-000008f0: 6768 2f66 6174 6961 6e64 6f2f 7665 7264  gh/fatiando/verd
-00000900: 650a 2e2e 2069 6d61 6765 3a3a 2068 7474  e... image:: htt
-00000910: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000920: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00000930: 6f6e 732f 7665 7264 652e 7376 673f 7374  ons/verde.svg?st
-00000940: 796c 653d 666c 6174 2d73 7175 6172 650a  yle=flat-square.
-00000950: 2020 2020 3a61 6c74 3a20 436f 6d70 6174      :alt: Compat
-00000960: 6962 6c65 2050 7974 686f 6e20 7665 7273  ible Python vers
-00000970: 696f 6e73 2e0a 2020 2020 3a74 6172 6765  ions..    :targe
-00000980: 743a 2068 7474 7073 3a2f 2f70 7970 692e  t: https://pypi.
-00000990: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
-000009a0: 7665 7264 650a 2e2e 2069 6d61 6765 3a3a  verde... image::
-000009b0: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
-000009c0: 656c 6473 2e69 6f2f 6261 6467 652f 646f  elds.io/badge/do
-000009d0: 692d 3130 2e32 3131 3035 2532 466a 6f73  i-10.21105%2Fjos
-000009e0: 732e 3030 3935 372d 626c 7565 2e73 7667  s.00957-blue.svg
-000009f0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
-00000a00: 7265 0a20 2020 203a 616c 743a 2044 6967  re.    :alt: Dig
-00000a10: 6974 616c 204f 626a 6563 7420 4964 656e  ital Object Iden
-00000a20: 7469 6669 6572 2066 6f72 2074 6865 204a  tifier for the J
-00000a30: 4f53 5320 7061 7065 720a 2020 2020 3a74  OSS paper.    :t
-00000a40: 6172 6765 743a 2068 7474 7073 3a2f 2f64  arget: https://d
-00000a50: 6f69 2e6f 7267 2f31 302e 3231 3130 352f  oi.org/10.21105/
-00000a60: 6a6f 7373 2e30 3039 3537 0a0a 0a2e 2e20  joss.00957..... 
-00000a70: 706c 6163 6568 6f6c 6465 722d 666f 722d  placeholder-for-
-00000a80: 646f 632d 696e 6465 780a 0a0a 4162 6f75  doc-index...Abou
-00000a90: 740a 2d2d 2d2d 2d0a 0a2a 2a56 6572 6465  t.-----..**Verde
-00000aa0: 2a2a 2069 7320 6120 5079 7468 6f6e 206c  ** is a Python l
-00000ab0: 6962 7261 7279 2066 6f72 2070 726f 6365  ibrary for proce
-00000ac0: 7373 696e 6720 7370 6174 6961 6c20 6461  ssing spatial da
-00000ad0: 7461 2028 6261 7468 796d 6574 7279 2c0a  ta (bathymetry,.
-00000ae0: 6765 6f70 6879 7369 6373 2073 7572 7665  geophysics surve
-00000af0: 7973 2c20 6574 6329 2061 6e64 2069 6e74  ys, etc) and int
-00000b00: 6572 706f 6c61 7469 6e67 2069 7420 6f6e  erpolating it on
-00000b10: 2072 6567 756c 6172 2067 7269 6473 2028   regular grids (
-00000b20: 692e 652e 2c0a 2a67 7269 6464 696e 672a  i.e.,.*gridding*
-00000b30: 292e 0a0a 4f75 7220 636f 7265 2069 6e74  )...Our core int
-00000b40: 6572 706f 6c61 7469 6f6e 206d 6574 686f  erpolation metho
-00000b50: 6473 2061 7265 2069 6e73 7069 7265 6420  ds are inspired 
-00000b60: 6279 206d 6163 6869 6e65 2d6c 6561 726e  by machine-learn
-00000b70: 696e 672e 0a41 7320 7375 6368 2c20 5665  ing..As such, Ve
-00000b80: 7264 6520 696d 706c 656d 656e 7473 2061  rde implements a
-00000b90: 6e20 696e 7465 7266 6163 6520 7468 6174  n interface that
-00000ba0: 2069 7320 7369 6d69 6c61 7220 746f 2074   is similar to t
-00000bb0: 6865 2070 6f70 756c 6172 0a60 7363 696b  he popular.`scik
-00000bc0: 6974 2d6c 6561 726e 203c 6874 7470 733a  it-learn <https:
-00000bd0: 2f2f 7363 696b 6974 2d6c 6561 726e 2e6f  //scikit-learn.o
-00000be0: 7267 2f3e 605f 5f20 6c69 6272 6172 792e  rg/>`__ library.
-00000bf0: 0a57 6520 616c 736f 2070 726f 7669 6465  .We also provide
-00000c00: 206f 7468 6572 2061 6e61 6c79 7369 7320   other analysis 
-00000c10: 6d65 7468 6f64 7320 7468 6174 2061 7265  methods that are
-00000c20: 206f 6674 656e 2075 7365 6420 696e 2063   often used in c
-00000c30: 6f6d 6269 6e61 7469 6f6e 2077 6974 680a  ombination with.
-00000c40: 6772 6964 6469 6e67 2c20 6c69 6b65 2074  gridding, like t
-00000c50: 7265 6e64 2072 656d 6f76 616c 2c20 626c  rend removal, bl
-00000c60: 6f63 6b65 642f 7769 6e64 6f77 6564 206f  ocked/windowed o
-00000c70: 7065 7261 7469 6f6e 732c 2063 726f 7373  perations, cross
-00000c80: 2d76 616c 6964 6174 696f 6e2c 0a61 6e64  -validation,.and
-00000c90: 206d 6f72 6521 0a0a 0a50 726f 6a65 6374   more!...Project
-00000ca0: 2067 6f61 6c73 0a2d 2d2d 2d2d 2d2d 2d2d   goals.---------
-00000cb0: 2d2d 2d2d 0a0a 2a20 5072 6f76 6964 6520  ----..* Provide 
-00000cc0: 6120 6d61 6368 696e 652d 6c65 6172 6e69  a machine-learni
-00000cd0: 6e67 2069 6e73 7069 7265 6420 696e 7465  ng inspired inte
-00000ce0: 7266 6163 6520 666f 7220 6772 6964 6469  rface for griddi
-00000cf0: 6e67 2073 7061 7469 616c 2064 6174 610a  ng spatial data.
-00000d00: 2a20 496e 7465 6772 6174 696f 6e20 7769  * Integration wi
-00000d10: 7468 2074 6865 2053 6369 7079 2073 7461  th the Scipy sta
-00000d20: 636b 3a20 6e75 6d70 792c 2070 616e 6461  ck: numpy, panda
-00000d30: 732c 2073 6369 6b69 742d 6c65 6172 6e2c  s, scikit-learn,
-00000d40: 2061 6e64 2078 6172 7261 790a 2a20 496e   and xarray.* In
-00000d50: 636c 7564 6520 636f 6d6d 6f6e 2070 726f  clude common pro
-00000d60: 6365 7373 696e 6720 616e 6420 6461 7461  cessing and data
-00000d70: 2070 7265 7061 7261 7469 6f6e 2074 6173   preparation tas
-00000d80: 6b73 2c20 6c69 6b65 2062 6c6f 636b 6564  ks, like blocked
-00000d90: 206d 6561 6e73 2061 6e64 2032 4420 7472   means and 2D tr
-00000da0: 656e 6473 0a2a 2053 7570 706f 7274 2066  ends.* Support f
-00000db0: 6f72 2067 7269 6464 696e 6720 7363 616c  or gridding scal
-00000dc0: 6172 2061 6e64 2076 6563 746f 7220 6461  ar and vector da
-00000dd0: 7461 2028 6c69 6b65 2077 696e 6420 7370  ta (like wind sp
-00000de0: 6565 6420 6f72 2047 5053 2076 656c 6f63  eed or GPS veloc
-00000df0: 6974 6965 7329 0a2a 2053 7570 706f 7274  ities).* Support
-00000e00: 2066 6f72 2062 6f74 6820 4361 7274 6573   for both Cartes
-00000e10: 6961 6e20 616e 6420 6765 6f67 7261 7068  ian and geograph
-00000e20: 6963 2063 6f6f 7264 696e 6174 6573 0a0a  ic coordinates..
-00000e30: 5468 6520 6669 7273 7420 7265 6c65 6173  The first releas
-00000e40: 6520 6f66 2056 6572 6465 2077 6173 2066  e of Verde was f
-00000e50: 6f63 7573 6564 206f 6e20 6d65 6574 696e  ocused on meetin
-00000e60: 6720 6d6f 7374 206f 6620 7468 6573 6520  g most of these 
-00000e70: 696e 6974 6961 6c20 676f 616c 730a 616e  initial goals.an
-00000e80: 6420 6573 7461 626c 6973 6869 6e67 2074  d establishing t
-00000e90: 6865 206c 6f6f 6b20 616e 6420 6665 656c  he look and feel
-00000ea0: 206f 6620 7468 6520 6c69 6272 6172 792e   of the library.
-00000eb0: 0a4c 6174 6572 2072 656c 6561 7365 7320  .Later releases 
-00000ec0: 7769 6c6c 2066 6f63 7573 206f 6e20 6578  will focus on ex
-00000ed0: 7061 6e64 696e 6720 7468 6520 7261 6e67  panding the rang
-00000ee0: 6520 6f66 2067 7269 6464 6572 7320 6176  e of gridders av
-00000ef0: 6169 6c61 626c 652c 0a6f 7074 696d 697a  ailable,.optimiz
-00000f00: 696e 6720 7468 6520 636f 6465 2c20 616e  ing the code, an
-00000f10: 6420 696d 7072 6f76 696e 6720 616c 676f  d improving algo
-00000f20: 7269 7468 6d73 2073 6f20 7468 6174 206c  rithms so that l
-00000f30: 6172 6765 722d 7468 616e 2d6d 656d 6f72  arger-than-memor
-00000f40: 790a 6461 7461 7365 7473 2063 616e 2061  y.datasets can a
-00000f50: 6c73 6f20 6265 2073 7570 706f 7274 6564  lso be supported
-00000f60: 2e0a 0a0a 436f 6e74 6163 7469 6e67 2075  ....Contacting u
-00000f70: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  s.-------------.
-00000f80: 0a46 696e 6420 6f75 7420 6d6f 7265 2061  .Find out more a
-00000f90: 626f 7574 2068 6f77 2074 6f20 7265 6163  bout how to reac
-00000fa0: 6820 7573 2061 740a 6066 6174 6961 6e64  h us at.`fatiand
-00000fb0: 6f2e 6f72 672f 636f 6e74 6163 7420 3c68  o.org/contact <h
-00000fc0: 7474 7073 3a2f 2f77 7777 2e66 6174 6961  ttps://www.fatia
-00000fd0: 6e64 6f2e 6f72 672f 636f 6e74 6163 742f  ndo.org/contact/
-00000fe0: 3e60 5f5f 0a0a 4369 7469 6e67 2056 6572  >`__..Citing Ver
-00000ff0: 6465 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  de.------------.
-00001000: 0a54 6869 7320 6973 2072 6573 6561 7263  .This is researc
-00001010: 6820 736f 6674 7761 7265 202a 2a6d 6164  h software **mad
-00001020: 6520 6279 2073 6369 656e 7469 7374 732a  e by scientists*
-00001030: 2a20 2873 6565 0a60 4155 5448 4f52 532e  * (see.`AUTHORS.
-00001040: 6d64 203c 6874 7470 733a 2f2f 6769 7468  md <https://gith
-00001050: 7562 2e63 6f6d 2f66 6174 6961 6e64 6f2f  ub.com/fatiando/
-00001060: 7665 7264 652f 626c 6f62 2f6d 6169 6e2f  verde/blob/main/
-00001070: 4155 5448 4f52 532e 6d64 3e60 5f5f 292e  AUTHORS.md>`__).
-00001080: 2043 6974 6174 696f 6e73 0a68 656c 7020   Citations.help 
-00001090: 7573 206a 7573 7469 6679 2074 6865 2065  us justify the e
-000010a0: 6666 6f72 7420 7468 6174 2067 6f65 7320  ffort that goes 
-000010b0: 696e 746f 2062 7569 6c64 696e 6720 616e  into building an
-000010c0: 6420 6d61 696e 7461 696e 696e 6720 7468  d maintaining th
-000010d0: 6973 2070 726f 6a65 6374 2e20 4966 2079  is project. If y
-000010e0: 6f75 0a75 7365 6420 5665 7264 6520 666f  ou.used Verde fo
-000010f0: 7220 796f 7572 2072 6573 6561 7263 682c  r your research,
-00001100: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
-00001110: 2063 6974 696e 6720 7573 2e0a 0a53 6565   citing us...See
-00001120: 206f 7572 2060 4349 5441 5449 4f4e 2e72   our `CITATION.r
-00001130: 7374 2066 696c 6520 3c68 7474 7073 3a2f  st file <https:/
-00001140: 2f67 6974 6875 622e 636f 6d2f 6661 7469  /github.com/fati
-00001150: 616e 646f 2f76 6572 6465 2f62 6c6f 622f  ando/verde/blob/
-00001160: 6d61 696e 2f43 4954 4154 494f 4e2e 7273  main/CITATION.rs
-00001170: 743e 605f 5f0a 746f 2066 696e 6420 6f75  t>`__.to find ou
-00001180: 7420 6d6f 7265 2e0a 0a0a 436f 6e74 7269  t more....Contri
-00001190: 6275 7469 6e67 0a2d 2d2d 2d2d 2d2d 2d2d  buting.---------
-000011a0: 2d2d 2d0a 0a43 6f64 6520 6f66 2063 6f6e  ---..Code of con
-000011b0: 6475 6374 0a2b 2b2b 2b2b 2b2b 2b2b 2b2b  duct.+++++++++++
-000011c0: 2b2b 2b2b 0a0a 506c 6561 7365 206e 6f74  ++++..Please not
-000011d0: 6520 7468 6174 2074 6869 7320 7072 6f6a  e that this proj
-000011e0: 6563 7420 6973 2072 656c 6561 7365 6420  ect is released 
-000011f0: 7769 7468 2061 0a60 436f 6e74 7269 6275  with a.`Contribu
-00001200: 746f 7220 436f 6465 206f 6620 436f 6e64  tor Code of Cond
-00001210: 7563 7420 3c68 7474 7073 3a2f 2f67 6974  uct <https://git
-00001220: 6875 622e 636f 6d2f 6661 7469 616e 646f  hub.com/fatiando
-00001230: 2f76 6572 6465 2f62 6c6f 622f 6d61 696e  /verde/blob/main
-00001240: 2f43 4f44 455f 4f46 5f43 4f4e 4455 4354  /CODE_OF_CONDUCT
-00001250: 2e6d 643e 605f 5f2e 0a42 7920 7061 7274  .md>`__..By part
-00001260: 6963 6970 6174 696e 6720 696e 2074 6869  icipating in thi
-00001270: 7320 7072 6f6a 6563 7420 796f 7520 6167  s project you ag
-00001280: 7265 6520 746f 2061 6269 6465 2062 7920  ree to abide by 
-00001290: 6974 7320 7465 726d 732e 0a0a 436f 6e74  its terms...Cont
-000012a0: 7269 6275 7469 6e67 2047 7569 6465 6c69  ributing Guideli
-000012b0: 6e65 730a 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  nes.++++++++++++
-000012c0: 2b2b 2b2b 2b2b 2b2b 2b2b 2b0a 0a50 6c65  +++++++++++..Ple
-000012d0: 6173 6520 7265 6164 206f 7572 0a60 436f  ase read our.`Co
-000012e0: 6e74 7269 6275 7469 6e67 2047 7569 6465  ntributing Guide
-000012f0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001300: 2e63 6f6d 2f66 6174 6961 6e64 6f2f 7665  .com/fatiando/ve
-00001310: 7264 652f 626c 6f62 2f6d 6169 6e2f 434f  rde/blob/main/CO
-00001320: 4e54 5249 4255 5449 4e47 2e6d 643e 605f  NTRIBUTING.md>`_
-00001330: 5f0a 746f 2073 6565 2068 6f77 2079 6f75  _.to see how you
-00001340: 2063 616e 2068 656c 7020 616e 6420 6769   can help and gi
-00001350: 7665 2066 6565 6462 6163 6b2e 0a0a 496d  ve feedback...Im
-00001360: 706f 7374 6572 2073 796e 6472 6f6d 6520  poster syndrome 
-00001370: 6469 7363 6c61 696d 6572 0a2b 2b2b 2b2b  disclaimer.+++++
-00001380: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
-00001390: 2b2b 2b2b 2b2b 2b0a 0a2a 2a57 6520 7761  +++++++..**We wa
-000013a0: 6e74 2079 6f75 7220 6865 6c70 2e2a 2a20  nt your help.** 
-000013b0: 4e6f 2c20 7265 616c 6c79 2e0a 0a54 6865  No, really...The
-000013c0: 7265 206d 6179 2062 6520 6120 6c69 7474  re may be a litt
-000013d0: 6c65 2076 6f69 6365 2069 6e73 6964 6520  le voice inside 
-000013e0: 796f 7572 2068 6561 6420 7468 6174 2069  your head that i
-000013f0: 7320 7465 6c6c 696e 6720 796f 7520 7468  s telling you th
-00001400: 6174 2079 6f75 2772 650a 6e6f 7420 7265  at you're.not re
-00001410: 6164 7920 746f 2062 6520 616e 206f 7065  ady to be an ope
-00001420: 6e20 736f 7572 6365 2063 6f6e 7472 6962  n source contrib
-00001430: 7574 6f72 3b20 7468 6174 2079 6f75 7220  utor; that your 
-00001440: 736b 696c 6c73 2061 7265 6e27 7420 6e65  skills aren't ne
-00001450: 6172 6c79 2067 6f6f 640a 656e 6f75 6768  arly good.enough
-00001460: 2074 6f20 636f 6e74 7269 6275 7465 2e0a   to contribute..
-00001470: 5768 6174 2063 6f75 6c64 2079 6f75 2070  What could you p
-00001480: 6f73 7369 626c 7920 6f66 6665 723f 0a0a  ossibly offer?..
-00001490: 5765 2061 7373 7572 6520 796f 7520 7468  We assure you th
-000014a0: 6174 2074 6865 206c 6974 746c 6520 766f  at the little vo
-000014b0: 6963 6520 696e 2079 6f75 7220 6865 6164  ice in your head
-000014c0: 2069 7320 7772 6f6e 672e 0a0a 2a2a 4265   is wrong...**Be
-000014d0: 696e 6720 6120 636f 6e74 7269 6275 746f  ing a contributo
-000014e0: 7220 646f 6573 6e27 7420 6a75 7374 206d  r doesn't just m
-000014f0: 6561 6e20 7772 6974 696e 6720 636f 6465  ean writing code
-00001500: 2a2a 2e0a 4571 7561 6c6c 7920 696d 706f  **..Equally impo
-00001510: 7274 616e 7420 636f 6e74 7269 6275 7469  rtant contributi
-00001520: 6f6e 7320 696e 636c 7564 653a 0a77 7269  ons include:.wri
-00001530: 7469 6e67 206f 7220 7072 6f6f 662d 7265  ting or proof-re
-00001540: 6164 696e 6720 646f 6375 6d65 6e74 6174  ading documentat
-00001550: 696f 6e2c 2073 7567 6765 7374 696e 6720  ion, suggesting 
-00001560: 6f72 2069 6d70 6c65 6d65 6e74 696e 6720  or implementing 
-00001570: 7465 7374 732c 206f 720a 6576 656e 2067  tests, or.even g
-00001580: 6976 696e 6720 6665 6564 6261 636b 2061  iving feedback a
-00001590: 626f 7574 2074 6865 2070 726f 6a65 6374  bout the project
-000015a0: 2028 696e 636c 7564 696e 6720 6769 7669   (including givi
-000015b0: 6e67 2066 6565 6462 6163 6b20 6162 6f75  ng feedback abou
-000015c0: 7420 7468 650a 636f 6e74 7269 6275 7469  t the.contributi
-000015d0: 6f6e 2070 726f 6365 7373 292e 0a49 6620  on process)..If 
-000015e0: 796f 7527 7265 2063 6f6d 696e 6720 746f  you're coming to
-000015f0: 2074 6865 2070 726f 6a65 6374 2077 6974   the project wit
-00001600: 6820 6672 6573 6820 6579 6573 2c20 796f  h fresh eyes, yo
-00001610: 7520 6d69 6768 7420 7365 6520 7468 6520  u might see the 
-00001620: 6572 726f 7273 2061 6e64 0a61 7373 756d  errors and.assum
-00001630: 7074 696f 6e73 2074 6861 7420 7365 6173  ptions that seas
-00001640: 6f6e 6564 2063 6f6e 7472 6962 7574 6f72  oned contributor
-00001650: 7320 6861 7665 2067 6c6f 7373 6564 206f  s have glossed o
-00001660: 7665 722e 0a49 6620 796f 7520 6361 6e20  ver..If you can 
-00001670: 7772 6974 6520 616e 7920 636f 6465 2061  write any code a
-00001680: 7420 616c 6c2c 2079 6f75 2063 616e 2063  t all, you can c
-00001690: 6f6e 7472 6962 7574 6520 636f 6465 2074  ontribute code t
-000016a0: 6f20 6f70 656e 2073 6f75 7263 652e 0a57  o open source..W
-000016b0: 6520 6172 6520 636f 6e73 7461 6e74 6c79  e are constantly
-000016c0: 2074 7279 696e 6720 6f75 7420 6e65 7720   trying out new 
-000016d0: 736b 696c 6c73 2c20 6d61 6b69 6e67 206d  skills, making m
-000016e0: 6973 7461 6b65 732c 2061 6e64 206c 6561  istakes, and lea
-000016f0: 726e 696e 6720 6672 6f6d 0a74 686f 7365  rning from.those
-00001700: 206d 6973 7461 6b65 732e 0a54 6861 7427   mistakes..That'
-00001710: 7320 686f 7720 7765 2061 6c6c 2069 6d70  s how we all imp
-00001720: 726f 7665 2061 6e64 2077 6520 6172 6520  rove and we are 
-00001730: 6861 7070 7920 746f 2068 656c 7020 6f74  happy to help ot
-00001740: 6865 7273 206c 6561 726e 2e0a 0a2a 5468  hers learn...*Th
-00001750: 6973 2064 6973 636c 6169 6d65 7220 7761  is disclaimer wa
-00001760: 7320 6164 6170 7465 6420 6672 6f6d 2074  s adapted from t
-00001770: 6865 2a0a 604d 6574 5079 2070 726f 6a65  he*.`MetPy proje
-00001780: 6374 203c 6874 7470 733a 2f2f 6769 7468  ct <https://gith
-00001790: 7562 2e63 6f6d 2f55 6e69 6461 7461 2f4d  ub.com/Unidata/M
-000017a0: 6574 5079 3e60 5f5f 2e0a 0a0a 4c69 6365  etPy>`__....Lice
-000017b0: 6e73 650a 2d2d 2d2d 2d2d 2d0a 0a54 6869  nse.-------..Thi
-000017c0: 7320 6973 2066 7265 6520 736f 6674 7761  s is free softwa
-000017d0: 7265 3a20 796f 7520 6361 6e20 7265 6469  re: you can redi
-000017e0: 7374 7269 6275 7465 2069 7420 616e 642f  stribute it and/
-000017f0: 6f72 206d 6f64 6966 7920 6974 2075 6e64  or modify it und
-00001800: 6572 2074 6865 2074 6572 6d73 0a6f 6620  er the terms.of 
-00001810: 7468 6520 2a2a 4253 4420 332d 636c 6175  the **BSD 3-clau
-00001820: 7365 204c 6963 656e 7365 2a2a 2e20 4120  se License**. A 
-00001830: 636f 7079 206f 6620 7468 6973 206c 6963  copy of this lic
-00001840: 656e 7365 2069 7320 7072 6f76 6964 6564  ense is provided
-00001850: 2069 6e0a 604c 4943 454e 5345 2e74 7874   in.`LICENSE.txt
-00001860: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001870: 2e63 6f6d 2f66 6174 6961 6e64 6f2f 7665  .com/fatiando/ve
-00001880: 7264 652f 626c 6f62 2f6d 6169 6e2f 4c49  rde/blob/main/LI
-00001890: 4345 4e53 452e 7478 743e 605f 5f2e 0a0a  CENSE.txt>`__...
-000018a0: 0a                                       .
+00000020: 650a 5665 7273 696f 6e3a 2031 2e38 2e30  e.Version: 1.8.0
+00000030: 0a53 756d 6d61 7279 3a20 5072 6f63 6573  .Summary: Proces
+00000040: 7369 6e67 2061 6e64 2067 7269 6464 696e  sing and griddin
+00000050: 6720 7370 6174 6961 6c20 6461 7461 2c20  g spatial data, 
+00000060: 6d61 6368 696e 652d 6c65 6172 6e69 6e67  machine-learning
+00000070: 2073 7479 6c65 0a48 6f6d 652d 7061 6765   style.Home-page
+00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000090: 2e63 6f6d 2f66 6174 6961 6e64 6f2f 7665  .com/fatiando/ve
+000000a0: 7264 650a 4175 7468 6f72 3a20 5468 6520  rde.Author: The 
+000000b0: 5665 7264 6520 4465 7665 6c6f 7065 7273  Verde Developers
+000000c0: 0a41 7574 686f 722d 656d 6169 6c3a 2066  .Author-email: f
+000000d0: 6174 6961 6e64 6f61 7465 7272 6140 7072  atiandoaterra@pr
+000000e0: 6f74 6f6e 6d61 696c 2e63 6f6d 0a4d 6169  otonmail.com.Mai
+000000f0: 6e74 6169 6e65 723a 2022 4c65 6f6e 6172  ntainer: "Leonar
+00000100: 646f 2055 6965 6461 220a 4d61 696e 7461  do Uieda".Mainta
+00000110: 696e 6572 2d65 6d61 696c 3a20 6c65 6f75  iner-email: leou
+00000120: 6965 6461 4067 6d61 696c 2e63 6f6d 0a4c  ieda@gmail.com.L
+00000130: 6963 656e 7365 3a20 4253 4420 332d 436c  icense: BSD 3-Cl
+00000140: 6175 7365 204c 6963 656e 7365 0a50 726f  ause License.Pro
+00000150: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
+00000160: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
+00000170: 2f77 7777 2e66 6174 6961 6e64 6f2e 6f72  /www.fatiando.or
+00000180: 672f 7665 7264 650a 5072 6f6a 6563 742d  g/verde.Project-
+00000190: 5552 4c3a 2052 656c 6561 7365 204e 6f74  URL: Release Not
+000001a0: 6573 2c20 6874 7470 733a 2f2f 6769 7468  es, https://gith
+000001b0: 7562 2e63 6f6d 2f66 6174 6961 6e64 6f2f  ub.com/fatiando/
+000001c0: 7665 7264 652f 7265 6c65 6173 6573 0a50  verde/releases.P
+000001d0: 726f 6a65 6374 2d55 524c 3a20 4275 6720  roject-URL: Bug 
+000001e0: 5472 6163 6b65 722c 2068 7474 7073 3a2f  Tracker, https:/
+000001f0: 2f67 6974 6875 622e 636f 6d2f 6661 7469  /github.com/fati
+00000200: 616e 646f 2f76 6572 6465 2f69 7373 7565  ando/verde/issue
+00000210: 730a 5072 6f6a 6563 742d 5552 4c3a 2053  s.Project-URL: S
+00000220: 6f75 7263 6520 436f 6465 2c20 6874 7470  ource Code, http
+00000230: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+00000240: 6174 6961 6e64 6f2f 7665 7264 650a 4b65  atiando/verde.Ke
+00000250: 7977 6f72 6473 3a20 7370 6174 6961 6c2c  ywords: spatial,
+00000260: 6765 6f73 6369 656e 6365 2c67 656f 7068  geoscience,geoph
+00000270: 7973 6963 732c 6772 6964 6469 6e67 2c69  ysics,gridding,i
+00000280: 6e74 6572 706f 6c61 7469 6f6e 0a50 6c61  nterpolation.Pla
+00000290: 7466 6f72 6d3a 2061 6e79 0a43 6c61 7373  tform: any.Class
+000002a0: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+000002b0: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+000002c0: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+000002d0: 6c65 0a43 6c61 7373 6966 6965 723a 2049  le.Classifier: I
+000002e0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+000002f0: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+00000300: 6172 6368 0a43 6c61 7373 6966 6965 723a  arch.Classifier:
+00000310: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+00000320: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000330: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+00000340: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000350: 3a20 4564 7563 6174 696f 6e0a 436c 6173  : Education.Clas
+00000360: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+00000370: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000380: 3a3a 2042 5344 204c 6963 656e 7365 0a43  :: BSD License.C
+00000390: 6c61 7373 6966 6965 723a 204e 6174 7572  lassifier: Natur
+000003a0: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
+000003b0: 6e67 6c69 7368 0a43 6c61 7373 6966 6965  nglish.Classifie
+000003c0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000003d0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000003e0: 6e64 656e 740a 436c 6173 7369 6669 6572  ndent.Classifier
+000003f0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
+00000400: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000410: 670a 436c 6173 7369 6669 6572 3a20 546f  g.Classifier: To
+00000420: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000430: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
+00000440: 6962 7261 7269 6573 0a43 6c61 7373 6966  ibraries.Classif
+00000450: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000460: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000470: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
+00000480: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000490: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000004a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000004b0: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
+000004c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000004d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000004e0: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+000004f0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000500: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000510: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+00000520: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000530: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000540: 6e20 3a3a 2033 2e31 300a 5265 7175 6972  n :: 3.10.Requir
+00000550: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
+00000560: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000570: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000580: 6d61 726b 646f 776e 0a50 726f 7669 6465  markdown.Provide
+00000590: 732d 4578 7472 613a 2066 6173 740a 4c69  s-Extra: fast.Li
+000005a0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+000005b0: 4e53 452e 7478 740a 0a3c 696d 6720 7372  NSE.txt..<img sr
+000005c0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+000005d0: 622e 636f 6d2f 6661 7469 616e 646f 2f76  b.com/fatiando/v
+000005e0: 6572 6465 2f72 6177 2f6d 6169 6e2f 646f  erde/raw/main/do
+000005f0: 632f 5f73 7461 7469 632f 7265 6164 6d65  c/_static/readme
+00000600: 2d62 616e 6e65 722e 706e 6722 2061 6c74  -banner.png" alt
+00000610: 3d22 5665 7264 6522 3e0a 0a3c 6832 2061  ="Verde">..<h2 a
+00000620: 6c69 676e 3d22 6365 6e74 6572 223e 5072  lign="center">Pr
+00000630: 6f63 6573 7369 6e67 2061 6e64 2067 7269  ocessing and gri
+00000640: 6464 696e 6720 7370 6174 6961 6c20 6461  dding spatial da
+00000650: 7461 2c20 6d61 6368 696e 652d 6c65 6172  ta, machine-lear
+00000660: 6e69 6e67 2073 7479 6c65 3c2f 6832 3e0a  ning style</h2>.
+00000670: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000680: 7222 3e0a 3c61 2068 7265 663d 2268 7474  r">.<a href="htt
+00000690: 7073 3a2f 2f77 7777 2e66 6174 6961 6e64  ps://www.fatiand
+000006a0: 6f2e 6f72 672f 7665 7264 6522 3e3c 7374  o.org/verde"><st
+000006b0: 726f 6e67 3e44 6f63 756d 656e 7461 7469  rong>Documentati
+000006c0: 6f6e 3c2f 7374 726f 6e67 3e20 286c 6174  on</strong> (lat
+000006d0: 6573 7429 3c2f 613e 20e2 80a2 0a3c 6120  est)</a> ....<a 
+000006e0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+000006f0: 772e 6661 7469 616e 646f 2e6f 7267 2f76  w.fatiando.org/v
+00000700: 6572 6465 2f64 6576 223e 3c73 7472 6f6e  erde/dev"><stron
+00000710: 673e 446f 6375 6d65 6e74 6174 696f 6e3c  g>Documentation<
+00000720: 2f73 7472 6f6e 673e 2028 6d61 696e 2062  /strong> (main b
+00000730: 7261 6e63 6829 3c2f 613e 20e2 80a2 0a3c  ranch)</a> ....<
+00000740: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000750: 6769 7468 7562 2e63 6f6d 2f66 6174 6961  github.com/fatia
+00000760: 6e64 6f2f 7665 7264 652f 626c 6f62 2f6d  ndo/verde/blob/m
+00000770: 6169 6e2f 434f 4e54 5249 4255 5449 4e47  ain/CONTRIBUTING
+00000780: 2e6d 6422 3e3c 7374 726f 6e67 3e43 6f6e  .md"><strong>Con
+00000790: 7472 6962 7574 696e 673c 2f73 7472 6f6e  tributing</stron
+000007a0: 673e 3c2f 613e 20e2 80a2 0a3c 6120 6872  g></a> ....<a hr
+000007b0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+000007c0: 6661 7469 616e 646f 2e6f 7267 2f63 6f6e  fatiando.org/con
+000007d0: 7461 6374 2f22 3e3c 7374 726f 6e67 3e43  tact/"><strong>C
+000007e0: 6f6e 7461 6374 3c2f 7374 726f 6e67 3e3c  ontact</strong><
+000007f0: 2f61 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  /a>.</p>..<p ali
+00000800: 676e 3d22 6365 6e74 6572 223e 0a50 6172  gn="center">.Par
+00000810: 7420 6f66 2074 6865 203c 6120 6872 6566  t of the <a href
+00000820: 3d22 6874 7470 733a 2f2f 7777 772e 6661  ="https://www.fa
+00000830: 7469 616e 646f 2e6f 7267 223e 3c73 7472  tiando.org"><str
+00000840: 6f6e 673e 4661 7469 616e 646f 2061 2054  ong>Fatiando a T
+00000850: 6572 7261 3c2f 7374 726f 6e67 3e3c 2f61  erra</strong></a
+00000860: 3e20 7072 6f6a 6563 740a 3c2f 703e 0a0a  > project.</p>..
+00000870: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000880: 223e 0a3c 6120 6872 6566 3d22 6874 7470  ">.<a href="http
+00000890: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+000008a0: 6f72 672f 7079 7069 2f76 6572 6465 223e  org/pypi/verde">
+000008b0: 3c69 6d67 2073 7263 3d22 6874 7470 3a2f  <img src="http:/
+000008c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000008d0: 7079 7069 2f76 2f76 6572 6465 2e73 7667  pypi/v/verde.svg
+000008e0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+000008f0: 7265 2220 616c 743d 224c 6174 6573 7420  re" alt="Latest 
+00000900: 7665 7273 696f 6e20 6f6e 2050 7950 4922  version on PyPI"
+00000910: 3e3c 2f61 3e0a 3c61 2068 7265 663d 2268  ></a>.<a href="h
+00000920: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000930: 6d2f 636f 6e64 612d 666f 7267 652f 7665  m/conda-forge/ve
+00000940: 7264 652d 6665 6564 7374 6f63 6b22 3e3c  rde-feedstock"><
+00000950: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000960: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000970: 636f 6e64 612f 766e 2f63 6f6e 6461 2d66  conda/vn/conda-f
+00000980: 6f72 6765 2f76 6572 6465 2e73 7667 3f73  orge/verde.svg?s
+00000990: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+000009a0: 2220 616c 743d 224c 6174 6573 7420 7665  " alt="Latest ve
+000009b0: 7273 696f 6e20 6f6e 2063 6f6e 6461 2d66  rsion on conda-f
+000009c0: 6f72 6765 223e 3c2f 613e 0a3c 6120 6872  orge"></a>.<a hr
+000009d0: 6566 3d22 6874 7470 733a 2f2f 636f 6465  ef="https://code
+000009e0: 636f 762e 696f 2f67 682f 6661 7469 616e  cov.io/gh/fatian
+000009f0: 646f 2f76 6572 6465 223e 3c69 6d67 2073  do/verde"><img s
+00000a00: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000a10: 7368 6965 6c64 732e 696f 2f63 6f64 6563  shields.io/codec
+00000a20: 6f76 2f63 2f67 6974 6875 622f 6661 7469  ov/c/github/fati
+00000a30: 616e 646f 2f76 6572 6465 2f6d 6169 6e2e  ando/verde/main.
+00000a40: 7376 673f 7374 796c 653d 666c 6174 2d73  svg?style=flat-s
+00000a50: 7175 6172 6522 2061 6c74 3d22 5465 7374  quare" alt="Test
+00000a60: 2063 6f76 6572 6167 6520 7374 6174 7573   coverage status
+00000a70: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
+00000a80: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+00000a90: 686f 6e2e 6f72 672f 7079 7069 2f76 6572  hon.org/pypi/ver
+00000aa0: 6465 223e 3c69 6d67 2073 7263 3d22 6874  de"><img src="ht
+00000ab0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000ac0: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000ad0: 696f 6e73 2f76 6572 6465 2e73 7667 3f73  ions/verde.svg?s
+00000ae0: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00000af0: 2220 616c 743d 2243 6f6d 7061 7469 626c  " alt="Compatibl
+00000b00: 6520 5079 7468 6f6e 2076 6572 7369 6f6e  e Python version
+00000b10: 732e 223e 3c2f 613e 0a3c 6120 6872 6566  s."></a>.<a href
+00000b20: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+00000b30: 672f 3130 2e32 3131 3035 2f6a 6f73 732e  g/10.21105/joss.
+00000b40: 3030 3935 3722 3e3c 696d 6720 7372 633d  00957"><img src=
+00000b50: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000b60: 656c 6473 2e69 6f2f 6261 6467 652f 646f  elds.io/badge/do
+00000b70: 692d 3130 2e32 3131 3035 2532 466a 6f73  i-10.21105%2Fjos
+00000b80: 732e 3030 3935 372d 626c 7565 3f73 7479  s.00957-blue?sty
+00000b90: 6c65 3d66 6c61 742d 7371 7561 7265 2220  le=flat-square" 
+00000ba0: 616c 743d 2244 4f49 2075 7365 6420 746f  alt="DOI used to
+00000bb0: 2063 6974 6520 7468 6973 2073 6f66 7477   cite this softw
+00000bc0: 6172 6522 3e3c 2f61 3e0a 3c2f 703e 0a0a  are"></a>.</p>..
+00000bd0: 2323 2041 626f 7574 0a0a 2a2a 5665 7264  ## About..**Verd
+00000be0: 652a 2a20 6973 2061 2050 7974 686f 6e20  e** is a Python 
+00000bf0: 6c69 6272 6172 7920 666f 7220 7072 6f63  library for proc
+00000c00: 6573 7369 6e67 2073 7061 7469 616c 2064  essing spatial d
+00000c10: 6174 6120 2874 6f70 6f67 7261 7068 792c  ata (topography,
+00000c20: 2070 6f69 6e74 0a63 6c6f 7564 732c 2062   point.clouds, b
+00000c30: 6174 6879 6d65 7472 792c 2067 656f 7068  athymetry, geoph
+00000c40: 7973 6963 7320 7375 7276 6579 732c 2065  ysics surveys, e
+00000c50: 7463 2920 616e 6420 696e 7465 7270 6f6c  tc) and interpol
+00000c60: 6174 696e 6720 7468 656d 206f 6e20 6120  ating them on a 
+00000c70: 3244 0a73 7572 6661 6365 2028 692e 652e  2D.surface (i.e.
+00000c80: 2c20 6772 6964 6469 6e67 2920 7769 7468  , gridding) with
+00000c90: 2061 2068 696e 7420 6f66 206d 6163 6869   a hint of machi
+00000ca0: 6e65 206c 6561 726e 696e 672e 0a0a 4f75  ne learning...Ou
+00000cb0: 7220 636f 7265 2069 6e74 6572 706f 6c61  r core interpola
+00000cc0: 7469 6f6e 206d 6574 686f 6473 2061 7265  tion methods are
+00000cd0: 2069 6e73 7069 7265 6420 6279 206d 6163   inspired by mac
+00000ce0: 6869 6e65 2d6c 6561 726e 696e 672e 0a41  hine-learning..A
+00000cf0: 7320 7375 6368 2c20 5665 7264 6520 696d  s such, Verde im
+00000d00: 706c 656d 656e 7473 2061 6e20 696e 7465  plements an inte
+00000d10: 7266 6163 6520 7468 6174 2069 7320 7369  rface that is si
+00000d20: 6d69 6c61 7220 746f 2074 6865 2070 6f70  milar to the pop
+00000d30: 756c 6172 0a5b 7363 696b 6974 2d6c 6561  ular.[scikit-lea
+00000d40: 726e 5d28 6874 7470 733a 2f2f 7363 696b  rn](https://scik
+00000d50: 6974 2d6c 6561 726e 2e6f 7267 2f29 206c  it-learn.org/) l
+00000d60: 6962 7261 7279 2e0a 5765 2061 6c73 6f20  ibrary..We also 
+00000d70: 7072 6f76 6964 6520 6f74 6865 7220 616e  provide other an
+00000d80: 616c 7973 6973 206d 6574 686f 6473 2074  alysis methods t
+00000d90: 6861 7420 6172 6520 6f66 7465 6e20 7573  hat are often us
+00000da0: 6564 2069 6e20 636f 6d62 696e 6174 696f  ed in combinatio
+00000db0: 6e20 7769 7468 0a67 7269 6464 696e 672c  n with.gridding,
+00000dc0: 206c 696b 6520 7472 656e 6420 7265 6d6f   like trend remo
+00000dd0: 7661 6c2c 2062 6c6f 636b 6564 2f77 696e  val, blocked/win
+00000de0: 646f 7765 6420 6f70 6572 6174 696f 6e73  dowed operations
+00000df0: 2c20 6372 6f73 732d 7661 6c69 6461 7469  , cross-validati
+00000e00: 6f6e 2c0a 616e 6420 6d6f 7265 210a 0a23  on,.and more!..#
+00000e10: 2320 5072 6f6a 6563 7420 676f 616c 730a  # Project goals.
+00000e20: 0a2a 2050 726f 7669 6465 2061 206d 6163  .* Provide a mac
+00000e30: 6869 6e65 2d6c 6561 726e 696e 6720 696e  hine-learning in
+00000e40: 7370 6972 6564 2069 6e74 6572 6661 6365  spired interface
+00000e50: 2066 6f72 2067 7269 6464 696e 6720 7370   for gridding sp
+00000e60: 6174 6961 6c20 6461 7461 0a2a 2049 6e74  atial data.* Int
+00000e70: 6567 7261 7469 6f6e 2077 6974 6820 7468  egration with th
+00000e80: 6520 5363 6970 7920 7374 6163 6b3a 206e  e Scipy stack: n
+00000e90: 756d 7079 2c20 7061 6e64 6173 2c20 7363  umpy, pandas, sc
+00000ea0: 696b 6974 2d6c 6561 726e 2c20 616e 6420  ikit-learn, and 
+00000eb0: 7861 7272 6179 0a2a 2049 6e63 6c75 6465  xarray.* Include
+00000ec0: 2063 6f6d 6d6f 6e20 7072 6f63 6573 7369   common processi
+00000ed0: 6e67 2061 6e64 2064 6174 6120 7072 6570  ng and data prep
+00000ee0: 6172 6174 696f 6e20 7461 736b 732c 206c  aration tasks, l
+00000ef0: 696b 6520 626c 6f63 6b65 6420 6d65 616e  ike blocked mean
+00000f00: 7320 616e 6420 3244 2074 7265 6e64 730a  s and 2D trends.
+00000f10: 2a20 5375 7070 6f72 7420 666f 7220 6772  * Support for gr
+00000f20: 6964 6469 6e67 2073 6361 6c61 7220 616e  idding scalar an
+00000f30: 6420 7665 6374 6f72 2064 6174 6120 286c  d vector data (l
+00000f40: 696b 6520 7769 6e64 2073 7065 6564 206f  ike wind speed o
+00000f50: 7220 4750 5320 7665 6c6f 6369 7469 6573  r GPS velocities
+00000f60: 290a 2a20 5375 7070 6f72 7420 666f 7220  ).* Support for 
+00000f70: 626f 7468 2043 6172 7465 7369 616e 2061  both Cartesian a
+00000f80: 6e64 2067 656f 6772 6170 6869 6320 636f  nd geographic co
+00000f90: 6f72 6469 6e61 7465 730a 0a23 2320 5072  ordinates..## Pr
+00000fa0: 6f6a 6563 7420 7374 6174 7573 0a0a 2a2a  oject status..**
+00000fb0: 5665 7264 6520 6973 2073 7461 626c 6520  Verde is stable 
+00000fc0: 616e 6420 7265 6164 7920 666f 7220 7573  and ready for us
+00000fd0: 6521 2a2a 0a54 6869 7320 6d65 616e 7320  e!**.This means 
+00000fe0: 7468 6174 2077 6520 6172 6520 6361 7265  that we are care
+00000ff0: 6675 6c20 6162 6f75 7420 696e 7472 6f64  ful about introd
+00001000: 7563 696e 6720 6261 636b 7761 7264 7320  ucing backwards 
+00001010: 696e 636f 6d70 6174 6962 6c65 2063 6861  incompatible cha
+00001020: 6e67 6573 0a61 6e64 2077 696c 6c20 7072  nges.and will pr
+00001030: 6f76 6964 6520 616d 706c 6520 7761 726e  ovide ample warn
+00001040: 696e 6720 7768 656e 2064 6f69 6e67 2073  ing when doing s
+00001050: 6f2e 2055 7067 7261 6469 6e67 206d 696e  o. Upgrading min
+00001060: 6f72 2076 6572 7369 6f6e 7320 6f66 2056  or versions of V
+00001070: 6572 6465 0a73 686f 756c 6420 6e6f 7420  erde.should not 
+00001080: 7265 7175 6972 6520 6d61 6b69 6e67 2063  require making c
+00001090: 6861 6e67 6573 2074 6f20 796f 7572 2063  hanges to your c
+000010a0: 6f64 652e 0a0a 5468 6520 6669 7273 7420  ode...The first 
+000010b0: 6d61 6a6f 7220 7265 6c65 6173 6520 6f66  major release of
+000010c0: 2056 6572 6465 2077 6173 2066 6f63 7573   Verde was focus
+000010d0: 6564 206f 6e20 6d65 6574 696e 6720 6d6f  ed on meeting mo
+000010e0: 7374 206f 6620 7468 6573 6520 696e 6974  st of these init
+000010f0: 6961 6c0a 676f 616c 7320 616e 6420 6573  ial.goals and es
+00001100: 7461 626c 6973 6869 6e67 2074 6865 206c  tablishing the l
+00001110: 6f6f 6b20 616e 6420 6665 656c 206f 6620  ook and feel of 
+00001120: 7468 6520 6c69 6272 6172 792e 0a4c 6174  the library..Lat
+00001130: 6572 2072 656c 6561 7365 7320 7769 6c6c  er releases will
+00001140: 2066 6f63 7573 206f 6e20 6578 7061 6e64   focus on expand
+00001150: 696e 6720 7468 6520 7261 6e67 6520 6f66  ing the range of
+00001160: 2067 7269 6464 6572 7320 6176 6169 6c61   gridders availa
+00001170: 626c 652c 0a6f 7074 696d 697a 696e 6720  ble,.optimizing 
+00001180: 7468 6520 636f 6465 2c20 616e 6420 696d  the code, and im
+00001190: 7072 6f76 696e 6720 616c 676f 7269 7468  proving algorith
+000011a0: 6d73 2073 6f20 7468 6174 206c 6172 6765  ms so that large
+000011b0: 722d 7468 616e 2d6d 656d 6f72 790a 6461  r-than-memory.da
+000011c0: 7461 7365 7473 2063 616e 2061 6c73 6f20  tasets can also 
+000011d0: 6265 2073 7570 706f 7274 6564 2e0a 0a23  be supported...#
+000011e0: 2320 4765 7474 696e 6720 696e 766f 6c76  # Getting involv
+000011f0: 6564 0a0a f09f 97a8 efb8 8f20 2a2a 436f  ed......... **Co
+00001200: 6e74 6163 7420 7573 3a2a 2a0a 4669 6e64  ntact us:**.Find
+00001210: 206f 7574 206d 6f72 6520 6162 6f75 7420   out more about 
+00001220: 686f 7720 746f 2072 6561 6368 2075 7320  how to reach us 
+00001230: 6174 0a5b 6661 7469 616e 646f 2e6f 7267  at.[fatiando.org
+00001240: 2f63 6f6e 7461 6374 5d28 6874 7470 733a  /contact](https:
+00001250: 2f2f 7777 772e 6661 7469 616e 646f 2e6f  //www.fatiando.o
+00001260: 7267 2f63 6f6e 7461 6374 2f29 2e0a 0af0  rg/contact/)....
+00001270: 9f91 a9f0 9f8f bee2 808d f09f 92bb 202a  .............. *
+00001280: 2a43 6f6e 7472 6962 7574 696e 6720 746f  *Contributing to
+00001290: 2070 726f 6a65 6374 2064 6576 656c 6f70   project develop
+000012a0: 6d65 6e74 3a2a 2a0a 506c 6561 7365 2072  ment:**.Please r
+000012b0: 6561 6420 6f75 720a 5b43 6f6e 7472 6962  ead our.[Contrib
+000012c0: 7574 696e 6720 4775 6964 655d 2868 7474  uting Guide](htt
+000012d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000012e0: 6661 7469 616e 646f 2f76 6572 6465 2f62  fatiando/verde/b
+000012f0: 6c6f 622f 6d61 696e 2f43 4f4e 5452 4942  lob/main/CONTRIB
+00001300: 5554 494e 472e 6d64 290a 746f 2073 6565  UTING.md).to see
+00001310: 2068 6f77 2079 6f75 2063 616e 2068 656c   how you can hel
+00001320: 7020 616e 6420 6769 7665 2066 6565 6462  p and give feedb
+00001330: 6163 6b2e 0a0a f09f a791 f09f 8fbe e280  ack.............
+00001340: 8df0 9fa4 9de2 808d f09f a791 f09f 8fbc  ................
+00001350: 202a 2a43 6f64 6520 6f66 2063 6f6e 6475   **Code of condu
+00001360: 6374 3a2a 2a0a 5468 6973 2070 726f 6a65  ct:**.This proje
+00001370: 6374 2069 7320 7265 6c65 6173 6564 2077  ct is released w
+00001380: 6974 6820 610a 5b43 6f64 6520 6f66 2043  ith a.[Code of C
+00001390: 6f6e 6475 6374 5d28 6874 7470 733a 2f2f  onduct](https://
+000013a0: 6769 7468 7562 2e63 6f6d 2f66 6174 6961  github.com/fatia
+000013b0: 6e64 6f2f 636f 6d6d 756e 6974 792f 626c  ndo/community/bl
+000013c0: 6f62 2f6d 6169 6e2f 434f 4445 5f4f 465f  ob/main/CODE_OF_
+000013d0: 434f 4e44 5543 542e 6d64 292e 0a42 7920  CONDUCT.md)..By 
+000013e0: 7061 7274 6963 6970 6174 696e 6720 696e  participating in
+000013f0: 2074 6869 7320 7072 6f6a 6563 7420 796f   this project yo
+00001400: 7520 6167 7265 6520 746f 2061 6269 6465  u agree to abide
+00001410: 2062 7920 6974 7320 7465 726d 732e 0a0a   by its terms...
+00001420: 3e20 2a2a 496d 706f 7374 6572 2073 796e  > **Imposter syn
+00001430: 6472 6f6d 6520 6469 7363 6c61 696d 6572  drome disclaimer
+00001440: 3a2a 2a0a 3e20 5765 2077 616e 7420 796f  :**.> We want yo
+00001450: 7572 2068 656c 702e 202a 2a4e 6f2c 2072  ur help. **No, r
+00001460: 6561 6c6c 792e 2a2a 2054 6865 7265 206d  eally.** There m
+00001470: 6179 2062 6520 6120 6c69 7474 6c65 2076  ay be a little v
+00001480: 6f69 6365 2069 6e73 6964 6520 796f 7572  oice inside your
+00001490: 0a3e 2068 6561 6420 7468 6174 2069 7320  .> head that is 
+000014a0: 7465 6c6c 696e 6720 796f 7520 7468 6174  telling you that
+000014b0: 2079 6f75 2772 6520 6e6f 7420 7265 6164   you're not read
+000014c0: 792c 2074 6861 7420 796f 7520 6172 656e  y, that you aren
+000014d0: 2774 2073 6b69 6c6c 6564 0a3e 2065 6e6f  't skilled.> eno
+000014e0: 7567 6820 746f 2063 6f6e 7472 6962 7574  ugh to contribut
+000014f0: 652e 2057 6520 6173 7375 7265 2079 6f75  e. We assure you
+00001500: 2074 6861 7420 7468 6520 6c69 7474 6c65   that the little
+00001510: 2076 6f69 6365 2069 6e20 796f 7572 2068   voice in your h
+00001520: 6561 6420 6973 0a3e 2077 726f 6e67 2e20  ead is.> wrong. 
+00001530: 4d6f 7374 2069 6d70 6f72 7461 6e74 6c79  Most importantly
+00001540: 2c20 2a2a 7468 6572 6520 6172 6520 6d61  , **there are ma
+00001550: 6e79 2076 616c 7561 626c 6520 7761 7973  ny valuable ways
+00001560: 2074 6f20 636f 6e74 7269 6275 7465 2062   to contribute b
+00001570: 6573 6964 6573 0a3e 2077 7269 7469 6e67  esides.> writing
+00001580: 2063 6f64 652a 2a2e 0a3e 0a3e 202a 5468   code**..>.> *Th
+00001590: 6973 2064 6973 636c 6169 6d65 7220 7761  is disclaimer wa
+000015a0: 7320 6164 6170 7465 6420 6672 6f6d 2074  s adapted from t
+000015b0: 6865 2a0a 3e20 5b4d 6574 5079 2070 726f  he*.> [MetPy pro
+000015c0: 6a65 6374 5d28 6874 7470 733a 2f2f 6769  ject](https://gi
+000015d0: 7468 7562 2e63 6f6d 2f55 6e69 6461 7461  thub.com/Unidata
+000015e0: 2f4d 6574 5079 292e 0a0a 2323 204c 6963  /MetPy)...## Lic
+000015f0: 656e 7365 0a0a 5468 6973 2069 7320 6672  ense..This is fr
+00001600: 6565 2073 6f66 7477 6172 653a 2079 6f75  ee software: you
+00001610: 2063 616e 2072 6564 6973 7472 6962 7574   can redistribut
+00001620: 6520 6974 2061 6e64 2f6f 7220 6d6f 6469  e it and/or modi
+00001630: 6679 2069 7420 756e 6465 7220 7468 6520  fy it under the 
+00001640: 7465 726d 730a 6f66 2074 6865 202a 2a42  terms.of the **B
+00001650: 5344 2033 2d63 6c61 7573 6520 4c69 6365  SD 3-clause Lice
+00001660: 6e73 652a 2a2e 2041 2063 6f70 7920 6f66  nse**. A copy of
+00001670: 2074 6869 7320 6c69 6365 6e73 6520 6973   this license is
+00001680: 2070 726f 7669 6465 6420 696e 0a5b 604c   provided in.[`L
+00001690: 4943 454e 5345 2e74 7874 605d 2868 7474  ICENSE.txt`](htt
+000016a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000016b0: 6661 7469 616e 646f 2f76 6572 6465 2f62  fatiando/verde/b
+000016c0: 6c6f 622f 6d61 696e 2f4c 4943 454e 5345  lob/main/LICENSE
+000016d0: 2e74 7874 292e 0a                        .txt)..
```

### Comparing `verde-1.7.0/setup.cfg` & `verde-1.8.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = verde
 fullname = Verde
-description = "Processing and gridding spatial data, machine-learning style"
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+description = Processing and gridding spatial data, machine-learning style
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = The Verde Developers
 author_email = fatiandoaterra@protonmail.com
 maintainer = "Leonardo Uieda"
 maintainer_email = leouieda@gmail.com
 license = BSD 3-Clause License
 license_file = LICENSE.txt
 platform = any
@@ -19,15 +19,14 @@
 	Intended Audience :: Education
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering
 	Topic :: Software Development :: Libraries
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 url = https://github.com/fatiando/verde
 project_urls = 
 	Documentation = https://www.fatiando.org/verde
@@ -35,23 +34,28 @@
 	Bug Tracker = https://github.com/fatiando/verde/issues
 	Source Code = https://github.com/fatiando/verde
 
 [options]
 zip_safe = True
 include_package_data = True
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
-	numpy
-	scipy
-	pandas
-	xarray
-	scikit-learn
-	pooch>=0.7.0
-	dask!=2021.03.0
+	numpy>=1.19
+	scipy>=1.5
+	pandas>=1.1
+	xarray>=0.16
+	scikit-learn>=0.24
+	pooch>=1.2
+	dask>=2021.05.0
+
+[options.extras_require]
+fast = 
+	numba>=0.52
+	pykdtree>=1.3
 
 [options.package_data]
 verde.tests = data/*, baseline/*
 verde.datasets = registry.txt
 
 [flake8]
 max-line-length = 88
```

### Comparing `verde-1.7.0/verde/__init__.py` & `verde-1.8.0/verde/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .chain import Chain
 from .coordinates import (
     block_split,
     expanding_window,
     get_region,
     grid_coordinates,
     inside,
+    line_coordinates,
     longitude_continuity,
     pad_region,
     profile_coordinates,
     rolling_window,
     scatter_points,
 )
 from .distances import median_distance
@@ -26,16 +27,17 @@
 from .mask import convexhull_mask, distance_mask
 from .model_selection import (
     BlockKFold,
     BlockShuffleSplit,
     cross_val_score,
     train_test_split,
 )
+from .neighbors import KNeighbors
 from .projections import project_grid, project_region
-from .scipygridder import ScipyGridder
+from .scipygridder import Cubic, Linear, ScipyGridder
 from .spline import Spline, SplineCV
 from .trend import Trend
 from .utils import grid_to_table, make_xarray_grid, maxabs, variance_to_weights
 from .vector import Vector, VectorSpline2D
 
 
 def test(doctest=True, verbose=True, coverage=False, figures=True):
@@ -87,10 +89,11 @@
     status = pytest.main(args)
 
     warnings.warn(
         f"The '{package}.test' function is deprecated since v1.7.0 and "
         "will be removed in v2.0.0. "
         f"Use 'pytest --pyargs {package}' to run the tests.",
         FutureWarning,
+        stacklevel=2,
     )
 
     assert status == 0, "Some tests have failed."
```

### Comparing `verde-1.7.0/verde/_version.py` & `verde-1.8.0/verde/_version.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/base/base_classes.py` & `verde-1.8.0/verde/base/base_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     def filter(self, coordinates, data, weights=None):  # noqa: A003
         """
         Filter the data through the gridder and produce residuals.
 
         Calls ``fit`` on the data, evaluates the residuals (data - predicted
         data), and returns the coordinates, residuals, and weights.
 
-        No very useful by itself but this interface makes gridders compatible
+        Not very useful by itself but this interface makes gridders compatible
         with other processing operations and is used by :class:`verde.Chain` to
         join them together (for example, so you can fit a spline on the
         residuals of a trend).
 
         Parameters
         ----------
         coordinates : tuple of arrays
@@ -357,14 +357,15 @@
 
         """
         warnings.warn(
             "The default scoring will change from R² to negative root mean "
             "squared error (RMSE) in Verde 2.0.0. "
             "This may change model selection results slightly.",
             FutureWarning,
+            stacklevel=2,
         )
         return score_estimator("r2", self, coordinates, data, weights=weights)
 
     def grid(
         self,
         region=None,
         shape=None,
@@ -454,23 +455,14 @@
                 + "Please pass only coordinates or either the spacing or the shape."
             )
         if coordinates is not None and region is not None:
             raise ValueError(
                 "Both coordinates and region were provided. "
                 + "Please pass region only if spacing or shape is specified."
             )
-        # Raise deprecation warning for the region, shape and spacing arguments
-        if spacing is not None or shape is not None or region is not None:
-            warnings.warn(
-                "The 'spacing', 'shape' and 'region' arguments will be removed "
-                + "in Verde v2.0.0. "
-                + "Please use the 'verde.grid_coordinates' function to define "
-                + "grid coordinates and pass them as the 'coordinates' argument.",
-                FutureWarning,
-            )
         # Get grid coordinates from coordinates parameter
         if coordinates is not None:
             ndim = get_ndim_horizontal_coords(*coordinates[:2])
             if ndim == 1:
                 # Build a meshgrid if easting and northing are 1d
                 coordinates = meshgrid_from_1d(coordinates)
             else:
@@ -527,14 +519,20 @@
         If the interpolator collected the input data region, then it will be
         used if ``region=None``. Otherwise, you must specify the grid region.
 
         Use the *dims* and *data_names* arguments to set custom names for the
         dimensions and the data field(s) in the output
         :class:`pandas.DataFrame`. Default names are provided.
 
+        .. warning::
+
+            The ``scatter`` method is deprecated and will be removed in Verde
+            2.0.0. Use :func:`verde.scatter_points` and the ``predict`` method
+            instead.
+
         Parameters
         ----------
         region : list = [W, E, S, N]
             The west, east, south, and north boundaries of a given region.
         size : int
             The number of points to generate.
         random_state : numpy.random.RandomState or an int seed
@@ -566,14 +564,21 @@
 
         Returns
         -------
         table : pandas.DataFrame
             The interpolated values on a random set of points.
 
         """
+        warnings.warn(
+            "The 'scatter' method is deprecated and will be removed in Verde "
+            "2.0.0. Use 'verde.scatter_points' and the 'predict' method "
+            "instead.",
+            FutureWarning,
+            stacklevel=2,
+        )
         dims = self._get_dims(dims)
         region = get_instance_region(self, region)
         coordinates = scatter_points(region, size, random_state=random_state, **kwargs)
         if projection is None:
             data = check_data(self.predict(coordinates))
         else:
             data = check_data(
```

### Comparing `verde-1.7.0/verde/base/least_squares.py` & `verde-1.8.0/verde/base/least_squares.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/base/utils.py` & `verde-1.8.0/verde/base/utils.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/blockreduce.py` & `verde-1.8.0/verde/blockreduce.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/chain.py` & `verde-1.8.0/verde/chain.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/coordinates.py` & `verde-1.8.0/verde/coordinates.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,21 +184,125 @@
         coordinates.append(random.uniform(lower, upper, size))
     if extra_coords is not None:
         for value in np.atleast_1d(extra_coords):
             coordinates.append(np.ones_like(coordinates[0]) * value)
     return tuple(coordinates)
 
 
+def line_coordinates(
+    start, stop, size=None, spacing=None, adjust="spacing", pixel_register=False
+):
+    """
+    Generate evenly spaced points between two values.
+
+    Able to handle either specifying the number of points required (*size*) or
+    the size of the interval between points (*spacing*). If using *size*, the
+    output will be similar to using :func:`numpy.linspace`. When using
+    *spacing*, if the interval is not divisible by the desired spacing, either
+    the interval or the spacing will have to be adjusted. By default, the
+    spacing will be rounded to the nearest multiple. Optionally, the *stop*
+    value can be adjusted to fit the exact spacing given.
+
+    Parameters
+    ----------
+    start : float
+        The starting value of the sequence.
+    stop : float
+        The end value of the sequence.
+    num : int or None
+        The number of points in the sequence. If None, *spacing* must be
+        provided.
+    spacing : float or None
+        The step size (interval) between points in the sequence. If None,
+        *size* must be provided.
+    adjust : {'spacing', 'region'}
+        Whether to adjust the spacing or the interval/region if required.
+        Ignored if *size* is given instead of *spacing*. Defaults to adjusting
+        the spacing.
+    pixel_register : bool
+        If True, the points will refer to the center of each interval (pixel)
+        instead of the boundaries. In practice, this means that there will be
+        one less element in the sequence if *spacing* is provided. If *size* is
+        provided, the requested number of elements is respected. Default is
+        False.
+
+    Returns
+    -------
+    sequence : array
+        The generated sequence of values.
+
+    Examples
+    --------
+
+    >>> # Lower printing precision to shorten this example
+    >>> import numpy as np; np.set_printoptions(precision=2, suppress=True)
+
+    >>> values = line_coordinates(0, 5, spacing=2.5)
+    >>> print(values.shape)
+    (3,)
+    >>> print(values)
+    [0.  2.5 5. ]
+    >>> print(line_coordinates(0, 10, size=5))
+    [ 0.   2.5  5.   7.5 10. ]
+    >>> print(line_coordinates(0, 10, spacing=2.5))
+    [ 0.   2.5  5.   7.5 10. ]
+
+    The spacing is adjusted to fit the interval by default but this can be
+    changed to adjusting the interval/region instead:
+
+    >>> print(line_coordinates(0, 10, spacing=2.4))
+    [ 0.   2.5  5.   7.5 10. ]
+    >>> print(line_coordinates(0, 10, spacing=2.4, adjust="region"))
+    [0.  2.4 4.8 7.2 9.6]
+    >>> print(line_coordinates(0, 10, spacing=2.6))
+    [ 0.   2.5  5.   7.5 10. ]
+    >>> print(line_coordinates(0, 10, spacing=2.6, adjust="region"))
+    [ 0.   2.6  5.2  7.8 10.4]
+
+    Optionally, return values at the center of the intervals instead of their
+    boundaries:
+
+    >>> print(line_coordinates(0, 10, spacing=2.5, pixel_register=True))
+    [1.25 3.75 6.25 8.75]
+
+    Notice that this produces one value less than the non-pixel registered
+    version. If using *size* instead of *spacing*, the number of values will be
+    *size* regardless and the spacing will therefore be different from the
+    non-pixel registered version:
+
+    >>> print(line_coordinates(0, 10, size=5, pixel_register=True))
+    [1. 3. 5. 7. 9.]
+
+    """
+    if size is not None and spacing is not None:
+        raise ValueError("Both size and spacing provided. Only one is allowed.")
+    if size is None and spacing is None:
+        raise ValueError("Either a size or a spacing must be provided.")
+    if spacing is not None:
+        size, stop = spacing_to_size(start, stop, spacing, adjust)
+    elif pixel_register:
+        # Starts by generating grid-line registered coordinates and shifting
+        # them to the center of the pixel. Need 1 more point if given a size
+        # instead of spacing so that we can do that because we discard the last
+        # point when shifting the coordinates.
+        size = size + 1
+    values = np.linspace(start, stop, size)
+    if pixel_register:
+        values = values[:-1] + (values[1] - values[0]) / 2
+    return values
+
+
 def grid_coordinates(
     region,
     shape=None,
     spacing=None,
     adjust="spacing",
     pixel_register=False,
     extra_coords=None,
+    meshgrid=True,
 ):
     """
     Generate the coordinates for each point on a regular grid.
 
     The grid can be specified by either the number of points in each dimension
     (the *shape*) or by the grid node spacing.
 
@@ -231,14 +335,22 @@
         registered (only if given *spacing* and not *shape*). Default is False.
     extra_coords : None, scalar, or list
         If not None, then value(s) of extra coordinate arrays to be generated.
         These extra arrays will have the same *shape* as the others but will
         contain a constant value. Will generate an extra array per value given
         in *extra_coords*. Use this to generate arrays of constant heights or
         times, for example, that might be needed to evaluate a gridder.
+    meshgrid : bool
+        If True, will call :func:`numpy.meshgrid` on the generated coordinates
+        and return 2D arrays (useful if you need the coordinate values for
+        every single point on a grid). Otherwise, will return 1D coordinate
+        arrays (useful if you're making a :class:`xarray.DataArray` or looping
+        over grid coordinates with two ``for`` loops). Passing False to
+        *meshgrid* is **incompatible with *extra_coords* and an exception will
+        be raised** if used together (:class:`ValueError`).
 
     Returns
     -------
     coordinates : tuple of arrays
         Arrays with coordinates of each point in the grid. Each array contains
         values for a dimension in the order: easting, northing, vertical, and
         any extra dimensions given in *extra_coords*. All arrays will have the
@@ -280,14 +392,26 @@
     >>> print(north)
     [[ 0.   0.   0. ]
      [ 2.5  2.5  2.5]
      [ 5.   5.   5. ]
      [ 7.5  7.5  7.5]
      [10.  10.  10. ]]
 
+    If you don't need the 2D arrays, then use ``meshgrid=False``:
+
+    >>> east, north = grid_coordinates(
+    ...     region=(0, 5, 0, 10), spacing=2.5, meshgrid=False,
+    ... )
+    >>> print(east.shape, north.shape)
+    (3,) (5,)
+    >>> print(east)
+    [0.  2.5 5. ]
+    >>> print(north)
+    [ 0.   2.5  5.   7.5 10. ]
+
     The spacing can be different for northing and easting, respectively:
 
     >>> east, north = grid_coordinates(region=(-5, 1, 0, 10), spacing=(2.5, 1))
     >>> print(east.shape, north.shape)
     (5, 7) (5, 7)
     >>> print(east)
     [[-5. -4. -3. -2. -1.  0.  1.]
@@ -420,96 +544,109 @@
      [0.1 0.1 0.1]
      [0.1 0.1 0.1]]
 
     See also
     --------
     scatter_points : Generate the coordinates for a random scatter of points
     profile_coordinates : Coordinates for a profile between two points
+    line_coordinates: Generate evenly spaced points between two values
 
     """
     check_region(region)
     if shape is not None and spacing is not None:
         raise ValueError("Both grid shape and spacing provided. Only one is allowed.")
     if shape is None and spacing is None:
         raise ValueError("Either a grid shape or a spacing must be provided.")
-    if spacing is not None:
-        shape, region = spacing_to_shape(region, spacing, adjust)
-    elif pixel_register:
-        # Starts by generating grid-line registered coordinates and shifting
-        # them to the center of the pixel. Need 1 more point if given a shape
-        # so that we can do that because we discard the last point when
-        # shifting the coordinates.
-        shape = tuple(i + 1 for i in shape)
-    east_lines = np.linspace(region[0], region[1], shape[1])
-    north_lines = np.linspace(region[2], region[3], shape[0])
-    if pixel_register:
-        east_lines = east_lines[:-1] + (east_lines[1] - east_lines[0]) / 2
-        north_lines = north_lines[:-1] + (north_lines[1] - north_lines[0]) / 2
-    coordinates = list(np.meshgrid(east_lines, north_lines))
+    if shape is None:
+        shape = (None, None)
+        # Make sure the spacing is a tuple of 2 numbers
+        spacing = np.atleast_1d(spacing)
+        if len(spacing) == 1:
+            spacing = (spacing[0], spacing[0])
+        elif len(spacing) > 2:
+            raise ValueError(f"Only two values allowed for grid spacing: {spacing}")
+    else:
+        spacing = (None, None)
+
+    east = line_coordinates(
+        region[0],
+        region[1],
+        size=shape[1],
+        spacing=spacing[1],
+        adjust=adjust,
+        pixel_register=pixel_register,
+    )
+    north = line_coordinates(
+        region[2],
+        region[3],
+        size=shape[0],
+        spacing=spacing[0],
+        adjust=adjust,
+        pixel_register=pixel_register,
+    )
+    coordinates = [east, north]
+    if meshgrid:
+        coordinates = list(np.meshgrid(east, north))
     if extra_coords is not None:
+        if not meshgrid:
+            raise ValueError(
+                "Using 'meshgrid=False' and 'extra_coords' is 'verde.grid_coordinates' is not allowed."
+            )
         for value in np.atleast_1d(extra_coords):
             coordinates.append(np.ones_like(coordinates[0]) * value)
     return tuple(coordinates)
 
 
-def spacing_to_shape(region, spacing, adjust):
+def spacing_to_size(start, stop, spacing, adjust):
     """
-    Convert the grid spacing to a grid shape.
+    Convert a spacing to the number of points between start and stop.
 
-    Adjusts the spacing or the region if the desired spacing is not a multiple
-    of the grid dimensions.
+    Takes into account if the spacing or the interval needs to be adjusted.
 
     Parameters
     ----------
-    region : list = [W, E, S, N]
-        The boundaries of a given region in Cartesian or geographic
-        coordinates.
-    spacing : float, tuple = (s_north, s_east), or None
-        The grid spacing in the South-North and West-East directions,
-        respectively. A single value means that the spacing is equal in both
-        directions.
+    start : float
+        The starting value of the sequence.
+    stop : float
+        The end value of the sequence.
+    spacing : float
+        The step size (interval) between points in the sequence.
     adjust : {'spacing', 'region'}
-        Whether to adjust the spacing or the region if required. Ignored if
-        *shape* is given instead of *spacing*. Defaults to adjusting the
-        spacing.
+        Whether to adjust the spacing or the interval/region if required.
+        Defaults to adjusting the spacing.
 
     Returns
     -------
-    shape, region : tuples
-        The calculated shape and region that best fits the desired spacing.
-        Spacing or region may be adjusted.
+    size : int
+        The number of points between start and stop.
+    stop : float
+        The end of the interval, which may or may not have been adjusted.
 
     """
     if adjust not in ["spacing", "region"]:
         raise ValueError(
             "Invalid value for *adjust* '{}'. Should be 'spacing' or 'region'".format(
                 adjust
             )
         )
-
-    spacing = np.atleast_1d(spacing)
-    if len(spacing) > 2:
-        raise ValueError(
-            "Only two values allowed for grid spacing: {}".format(str(spacing))
-        )
-    elif len(spacing) == 1:
-        deast = dnorth = spacing[0]
-    elif len(spacing) == 2:
-        dnorth, deast = spacing
-
-    w, e, s, n = region
     # Add 1 to get the number of nodes, not segments
-    nnorth = int(round((n - s) / dnorth)) + 1
-    neast = int(round((e - w) / deast)) + 1
+    size = int(round((stop - start) / spacing)) + 1
+    # If the spacing >= 2 * (stop - start), it rounds to zero so we'd be
+    # generating a single point, which isn't equivalent to adjusting the
+    # spacing or the region. To get the appropriate behaviour of decreasing the
+    # spacing until it fits the region or increasing the region until it fits
+    # at least 1 spacing, we need to always round to at least 1 in the code
+    # above.
+    if size == 1:
+        size += 1
     if adjust == "region":
-        # The shape is the same but we adjust the region so that the spacing
+        # The size is the same but we adjust the interval so that the spacing
         # isn't altered when we do the linspace.
-        n = s + (nnorth - 1) * dnorth
-        e = w + (neast - 1) * deast
-    return (nnorth, neast), (w, e, s, n)
+        stop = start + (size - 1) * spacing
+    return size, stop
 
 
 def shape_to_spacing(region, shape, pixel_register=False):
     """
     Calculate the spacing of a grid given region and shape.
 
     Parameters
@@ -692,16 +829,16 @@
     [-10. -10. -10.   0.   0.   0.  10.  10.  10.]
 
     """
     check_region(region)
     w, e, s, n = region
     easting, northing = coordinates[:2]
     # Allocate temporary arrays to minimize memory allocation overhead
-    out = np.empty_like(easting, dtype=np.bool)
-    tmp = tuple(np.empty_like(easting, dtype=np.bool) for i in range(4))
+    out = np.empty_like(easting, dtype=bool)
+    tmp = tuple(np.empty_like(easting, dtype=bool) for i in range(4))
     # Using the logical functions is a lot faster than & > < for some reason
     # Plus, this way avoids repeated allocation of intermediate arrays
     in_we = np.logical_and(
         np.greater_equal(easting, w, out=tmp[0]),
         np.less_equal(easting, e, out=tmp[1]),
         out=tmp[2],
     )
@@ -1082,15 +1219,16 @@
         # the number of nodes.
         spacing = tuple(dim / (n - 1) for dim, n in zip(dimensions, shape))
     spacing = np.atleast_1d(spacing)
     if np.any(spacing > size):
         warnings.warn(
             f"Rolling windows do not overlap (size '{size}' and spacing '{spacing}'). "
             "Some data points may not be included in any window. "
-            "Increase size or decrease spacing to avoid this."
+            "Increase size or decrease spacing to avoid this.",
+            stacklevel=2,
         )
 
 
 def expanding_window(coordinates, center, sizes):
     """
     Select points on windows of changing size around a center point.
```

### Comparing `verde-1.7.0/verde/datasets/__init__.py` & `verde-1.8.0/verde/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/datasets/sample_data.py` & `verde-1.8.0/verde/datasets/sample_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,29 @@
 
 def _datasets_deprecation_warning():
     warnings.warn(
         "All sample datasets in Verde are deprecated and will be "
         "removed in Verde v2.0.0. The tutorials/examples will transition "
         "to using Ensaio (https://www.fatiando.org/ensaio/) instead.",
         DeprecationWarning,
+        stacklevel=2,
     )
 
 
 def locate():
     r"""
     The absolute path to the sample data storage location on disk.
 
+    .. warning::
+
+        All sample datasets in Verde are deprecated and will be
+        **removed in Verde v2.0.0**.
+        The tutorials/examples will transition to using
+        `Ensaio <https://www.fatiando.org/ensaio/>`__ instead.
+
     This is where the data are saved on your computer. The location is
     dependent on the operating system. The folder locations are defined by the
     ``appdirs``  package (see the `appdirs documentation
     <https://github.com/ActiveState/appdirs>`__).
 
     The location can be overwritten by the ``VERDE_DATA_DIR`` environment
     variable to the desired destination.
@@ -147,15 +155,16 @@
     --------
     fetch_baja_bathymetry: Sample bathymetry data from Baja California.
 
     """
     if kwargs:
         warnings.warn(
             "All kwargs are being ignored. They are accepted to "
-            + "guarantee backward compatibility."
+            + "guarantee backward compatibility.",
+            stacklevel=2,
         )
     _setup_map(
         ax,
         xticks=np.arange(-114, -105, 2),
         yticks=np.arange(21, 30, 2),
         coastlines=coastlines,
         region=region,
@@ -206,14 +215,15 @@
     setup_rio_magnetic_map: Utility function to help setup a Cartopy map.
 
     """
     warnings.warn(
         "The Rio magnetic anomaly dataset is deprecated and will be removed "
         "in Verde v2.0.0. Use a different dataset instead.",
         FutureWarning,
+        stacklevel=2,
     )
     data_file = REGISTRY.fetch("rio-magnetic.csv.xz")
     data = pd.read_csv(data_file, compression="xz")
     return data
 
 
 def setup_rio_magnetic_map(ax, region=(-42.6, -42, -22.5, -22)):
@@ -239,14 +249,15 @@
     fetch_rio_magnetic: Magnetic anomaly data from Rio de Janeiro, Brazil.
 
     """
     warnings.warn(
         "The Rio magnetic anomaly dataset is deprecated and will be removed "
         "in Verde v2.0.0. Use a different dataset instead.",
         FutureWarning,
+        stacklevel=2,
     )
     _setup_map(
         ax,
         xticks=np.arange(-42.5, -42, 0.1),
         yticks=np.arange(-22.5, -21.99, 0.1),
         region=region,
         crs=ccrs.PlateCarree(),
@@ -326,15 +337,16 @@
     --------
     fetch_california_gps: Sample GPS velocity data from California.
 
     """
     if kwargs:
         warnings.warn(
             "All kwargs are being ignored. They are accepted to "
-            + "guarantee backward compatibility."
+            + "guarantee backward compatibility.",
+            stacklevel=2,
         )
     _setup_map(
         ax,
         xticks=np.arange(-124, -115, 4),
         yticks=np.arange(33, 42, 2),
         coastlines=coastlines,
         region=region,
@@ -405,15 +417,16 @@
     --------
     fetch_texas_wind: Sample wind speed and air temperature data for Texas.
 
     """
     if kwargs:
         warnings.warn(
             "All kwargs are being ignored. They are accepted to "
-            + "guarantee backward compatibility."
+            + "guarantee backward compatibility.",
+            stacklevel=2,
         )
     _setup_map(
         ax,
         xticks=np.arange(-106, -92, 3),
         yticks=np.arange(27, 38, 3),
         coastlines=coastlines,
         region=region,
```

### Comparing `verde-1.7.0/verde/datasets/synthetic.py` & `verde-1.8.0/verde/datasets/synthetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,8 +25,9 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         warnings.warn(
             "Using CheckerBoard from verde.datasets is deprecated and will be "
             "removed in Verde 2.0.0. "
             "Use verde.synthetic.CheckerBoard instead.",
             FutureWarning,
+            stacklevel=2,
         )
```

### Comparing `verde-1.7.0/verde/distances.py` & `verde-1.8.0/verde/distances.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/io.py` & `verde-1.8.0/verde/io.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/mask.py` & `verde-1.8.0/verde/mask.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/model_selection.py` & `verde-1.8.0/verde/model_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,15 @@
             except ValueError:
                 warnings.warn(
                     "Could not balance folds to have approximately the same "
                     "number of data points. Dividing into folds with equal "
                     "number of blocks instead. Decreasing n_splits or increasing "
                     "the number of blocks may help.",
                     UserWarning,
+                    stacklevel=2,
                 )
                 folds = [i for _, i in KFold(n_splits=self.n_splits).split(block_ids)]
         else:
             folds = [i for _, i in KFold(n_splits=self.n_splits).split(block_ids)]
         for test_blocks in folds:
             test_points = np.where(np.isin(labels, block_ids[test_blocks]))[0]
             yield test_points
@@ -745,14 +746,15 @@
     """
     if client is not None:
         warnings.warn(
             "The 'client' parameter of 'verde.cross_val_score' is deprecated "
             "and will be removed in Verde 2.0.0. "
             "Use the 'delayed' parameter instead.",
             FutureWarning,
+            stacklevel=2,
         )
     coordinates, data, weights = check_fit_input(
         coordinates, data, weights, unpack=False
     )
     if cv is None:
         cv = KFold(shuffle=True, random_state=0, n_splits=5)
     feature_matrix = np.transpose(n_1d_arrays(coordinates, 2))
```

### Comparing `verde-1.7.0/verde/projections.py` & `verde-1.8.0/verde/projections.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 """
 import numpy as np
 
 from .blockreduce import BlockReduce
 from .chain import Chain
 from .coordinates import check_region, get_region, grid_coordinates, shape_to_spacing
 from .mask import convexhull_mask
-from .scipygridder import ScipyGridder
+from .neighbors import KNeighbors
+from .scipygridder import Cubic, Linear
 from .utils import grid_to_table
 
 
 def project_region(region, projection):
     """
     Calculate the bounding box of a region in projected coordinates.
 
@@ -95,18 +96,18 @@
         easting/longitude dimension.
     projection : callable
         Should be a callable object (like a function) ``projection(easting,
         northing) -> (proj_easting, proj_northing)`` that takes in easting and
         northing coordinate arrays and returns projected northing and easting
         coordinate arrays.
     method : string or Verde gridder
-        If a string, will use it to create a :class:`~verde.ScipyGridder` with
-        the corresponding method (nearest, linear, or cubic). Otherwise, should
-        be a gridder/estimator object, like :class:`~verde.Spline`. Default is
-        ``"linear"``.
+        If a string, will use it to create :class:`~verde.KNeighbors`,
+        :class:`~verde.Linear`, or :class:`~verde.Cubic` (``"nearest"``,
+        ``"linear"``, or ``"cubic"``). Otherwise, should be a gridder/estimator
+        object, like :class:`~verde.Spline`. Default is ``"linear"``.
     antialias : bool
         If True, will run a :class:`~verde.BlockReduce` with a mean function to
         avoid aliasing when the projection results in oversampling of the data
         in some areas (for example, in polar projections). If False, will not
         run the blocked mean.
 
     Returns
@@ -123,14 +124,25 @@
     if len(grid.dims) != 2:
         raise ValueError(
             "Projecting grids with number of dimensions other than 2 is not "
             "currently supported (dimensions of the given DataArray: {}).".format(
                 len(grid.dims)
             )
         )
+    if isinstance(method, str):
+        classes = dict(
+            linear=Linear,
+            nearest=KNeighbors,
+            cubic=Cubic,
+        )
+        if method not in classes:
+            raise ValueError(
+                f"Invalid interpolation method '{method}'. Must be one of {classes.keys()}."
+            )
+        method = classes[method]()
 
     # Can be set to None for some data arrays depending on how they are created
     # so we can't just rely on the default value for getattr.
     name = getattr(grid, "name", None)
     if name is None:
         name = "scalars"
 
@@ -145,23 +157,19 @@
     check_region(region)
 
     steps = []
     if antialias:
         steps.append(
             ("mean", BlockReduce(np.mean, spacing=spacing, region=data_region))
         )
-    if isinstance(method, str):
-        steps.append(("spline", ScipyGridder(method)))
-    else:
-        steps.append(("spline", method))
+    steps.append(("interpolator", method))
     interpolator = Chain(steps)
     interpolator.fit(coordinates, data[name])
 
     projected = interpolator.grid(
         region=region,
         spacing=spacing,
         data_names=kwargs.pop("data_names", [name]),
-        **kwargs
+        **kwargs,
     )
-    if method not in ["linear", "cubic"]:
-        projected = convexhull_mask(coordinates, grid=projected)
+    projected = convexhull_mask(coordinates, grid=projected)
     return projected[name]
```

### Comparing `verde-1.7.0/verde/scipygridder.py` & `verde-1.8.0/verde/neighbors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,131 +1,122 @@
 # Copyright (c) 2017 The Verde Developers.
 # Distributed under the terms of the BSD 3-Clause License.
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # This code is part of the Fatiando a Terra project (https://www.fatiando.org)
 #
 """
-A gridder that uses scipy.interpolate as the backend.
+Nearest neighbor interpolation
 """
-from warnings import warn
+import warnings
 
 import numpy as np
-from scipy.interpolate import (
-    CloughTocher2DInterpolator,
-    LinearNDInterpolator,
-    NearestNDInterpolator,
-)
 from sklearn.utils.validation import check_is_fitted
 
-from .base import BaseGridder, check_fit_input
+from .base import BaseGridder, check_fit_input, n_1d_arrays
 from .coordinates import get_region
+from .utils import kdtree
 
 
-class ScipyGridder(BaseGridder):
+class KNeighbors(BaseGridder):
     """
-    A scipy.interpolate based gridder for scalar Cartesian data.
+    Nearest neighbor interpolation.
 
-    Provides a verde gridder interface to the scipy interpolators
-    :class:`scipy.interpolate.LinearNDInterpolator`,
-    :class:`scipy.interpolate.NearestNDInterpolator`, and
-    :class:`scipy.interpolate.CloughTocher2DInterpolator` (cubic).
+    This gridder assumes Cartesian coordinates.
+
+    Interpolation based on the values of the *k* nearest neighbors of each
+    interpolated point. The number of neighbors *k* can be controlled and
+    mostly influences the spatial smoothness of the interpolated values.
+
+    The data values of the *k* nearest neighbors are combined into a single
+    value by a reduction function, which defaults to the mean. This can also be
+    configured.
+
+    .. note::
+
+        If installed, package ``pykdtree`` will be used for the nearest
+        neighbors look-up instead of :class:`scipy.spatial.cKDTree` for better
+        performance.
 
     Parameters
     ----------
-    method : str
-        The interpolation method. Either ``'linear'``, ``'nearest'``, or
-        ``'cubic'``.
-    extra_args : None or dict
-        Extra keyword arguments to pass to the scipy interpolator class. See
-        the documentation for each interpolator for a list of possible
-        arguments.
+    k : int
+        The number of neighbors to use for each interpolated point. Default is
+        1.
+    reduction : function
+        Function used to combine the values of the *k* neighbors into a single
+        value. Can be any function that takes a 1D numpy array as input and
+        outputs a single value. Default is :func:`numpy.mean`.
 
     Attributes
     ----------
-    interpolator_ : scipy interpolator class
-        An instance of the corresponding scipy interpolator class.
+    tree_ : K-D tree
+        An instance of the K-D tree data structure for the data points that is
+        used to query for nearest neighbors.
+    data_ : 1D array
+        A copy of the input data as a 1D array. Used to look up values for
+        interpolation/prediction.
     region_ : tuple
         The boundaries (``[W, E, S, N]``) of the data used to fit the
         interpolator. Used as the default region for the
-        :meth:`~verde.ScipyGridder.grid` and
-        :meth:`~verde.ScipyGridder.scatter` methods.
+        :meth:`~verde.KNeighbors.grid`` method.
 
     """
 
-    def __init__(self, method="cubic", extra_args=None):
+    def __init__(self, k=1, reduction=np.mean):
         super().__init__()
-        self.method = method
-        self.extra_args = extra_args
+        self.k = k
+        self.reduction = reduction
 
     def fit(self, coordinates, data, weights=None):
         """
         Fit the interpolator to the given data.
 
-        Any keyword arguments passed as the ``extra_args`` attribute will be
-        used when instantiating the scipy interpolator.
-
         The data region is captured and used as default for the
-        :meth:`~verde.ScipyGridder.grid` and
-        :meth:`~verde.ScipyGridder.scatter` methods.
+        :meth:`~verde.KNeighbors.grid` method.
 
         Parameters
         ----------
         coordinates : tuple of arrays
             Arrays with the coordinates of each data point. Should be in the
             following order: (easting, northing, vertical, ...). Only easting
             and northing will be used, all subsequent coordinates will be
             ignored.
         data : array
             The data values that will be interpolated.
         weights : None or array
-            If not None, then the weights assigned to each data point.
-            Typically, this should be 1 over the data uncertainty squared.
-            Ignored for this interpolator. Only present for compatibility with
-            other gridder.
+            Data weights are **not supported** by this interpolator and will be
+            ignored. Only present for compatibility with other gridders.
 
         Returns
         -------
-        self : verde.ScipyGridder
+        self
             Returns this gridder instance for chaining operations.
 
         """
-        classes = dict(
-            linear=LinearNDInterpolator,
-            nearest=NearestNDInterpolator,
-            cubic=CloughTocher2DInterpolator,
-        )
-        if self.method not in classes:
-            raise ValueError(
-                "Invalid interpolation method '{}'. Must be one of {}.".format(
-                    self.method, str(classes.keys())
-                )
-            )
-        if self.extra_args is None:
-            kwargs = {}
-        else:
-            kwargs = self.extra_args
         if weights is not None:
-            warn(
+            warnings.warn(
                 "{} does not support weights and they will be ignored.".format(
                     self.__class__.__name__
-                )
+                ),
+                stacklevel=2,
             )
         coordinates, data, weights = check_fit_input(coordinates, data, weights)
-        easting, northing = coordinates[:2]
-        self.region_ = get_region((easting, northing))
-        points = np.column_stack((np.ravel(easting), np.ravel(northing)))
-        self.interpolator_ = classes[self.method](points, np.ravel(data), **kwargs)
+        self.region_ = get_region(coordinates[:2])
+        self.tree_ = kdtree(coordinates[:2])
+        # Make sure this is an array and not a subclass of array (pandas,
+        # xarray, etc) so that we can index it later during predict.
+        self.data_ = np.asarray(data).ravel().copy()
         return self
 
     def predict(self, coordinates):
         """
         Interpolate data on the given set of points.
 
-        Requires a fitted gridder (see :meth:`~verde.ScipyGridder.fit`).
+        Requires a fitted gridder (see :meth:`~verde.KNeighbors.fit`).
 
         Parameters
         ----------
         coordinates : tuple of arrays
             Arrays with the coordinates of each data point. Should be in the
             following order: (easting, northing, vertical, ...). Only easting
             and northing will be used, all subsequent coordinates will be
@@ -133,10 +124,17 @@
 
         Returns
         -------
         data : array
             The data values interpolated on the given points.
 
         """
-        check_is_fitted(self, ["interpolator_"])
-        easting, northing = coordinates[:2]
-        return self.interpolator_((easting, northing))
+        check_is_fitted(self, ["tree_"])
+        distances, indices = self.tree_.query(
+            np.transpose(n_1d_arrays(coordinates, 2)), k=self.k
+        )
+        if indices.ndim == 1:
+            indices = np.atleast_2d(indices).T
+        neighbor_values = np.reshape(self.data_[indices.ravel()], indices.shape)
+        data = self.reduction(neighbor_values, axis=1)
+        shape = np.broadcast(*coordinates[:2]).shape
+        return data.reshape(shape)
```

### Comparing `verde-1.7.0/verde/spline.py` & `verde-1.8.0/verde/spline.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,45 +56,53 @@
         v2.0.0. Use ``delayed`` instead.
 
     Other cross-validation generators from :mod:`sklearn.model_selection` can
     be used by passing them through the *cv* argument.
 
     Parameters
     ----------
-    mindists : iterable or 1d array
+    mindists : iterable or 1d array or None
+        **DEPRECATED:** This argument is no longer needed and will be removed
+        in Verde 2.0.0. This fudge factor is no longer required since a new
+        formulation eliminates the singularity at zero distance. Use the
+        default value of ``mindists=None`` to get the future behaviour.
         List (or other iterable) of *mindist* parameter values to try. Can be
         considered a minimum distance between the point forces and data points.
-        Needed because the Green's functions are singular when forces and data
-        points coincide. Acts as a fudge factor.
     dampings : iterable or 1d array
         List (or other iterable) of *damping* parameter values to try. Is the
         positive damping regularization parameter. Controls how much smoothness
         is imposed on the estimated forces. If None, no regularization is used.
     force_coords : None or tuple of arrays
         The easting and northing coordinates of the point forces. If None
         (default), then will be set to the data coordinates the first time
         :meth:`~verde.SplineCV.fit` is called.
     engine : str
-        Computation engine for the Jacobian matrix and prediction. Can be
-        ``'auto'``, ``'numba'``, or ``'numpy'``. If ``'auto'``, will use numba
-        if it is installed or numpy otherwise. The numba version is
-        multi-threaded and usually faster, which makes fitting and predicting
-        faster.
+        **DEPRECATED:** This option is deprecated and will be removed in Verde
+        v2.0.0. The numba engine will be the only option. Computation engine
+        for the Jacobian matrix and prediction. Can be ``'auto'``, ``'numba'``,
+        or ``'numpy'``. If ``'auto'``, will use numba if it is installed or
+        numpy otherwise. The numba version is multi-threaded and usually
+        faster, which makes fitting and predicting faster.
     cv : None or cross-validation generator
         Any scikit-learn cross-validation generator. If not given, will use the
         default set by :func:`verde.cross_val_score`.
     client : None or dask.distributed.Client
         **DEPRECATED:** This option is deprecated and will be removed in Verde
         v2.0.0. If None, then computations are run serially. Otherwise, should
         be a dask ``Client`` object. It will be used to dispatch computations
         to the dask cluster.
     delayed : bool
         If True, will use :func:`dask.delayed` to dispatch computations and
         allow mod:`dask` to execute the grid search in parallel (see note
         above).
+    scoring : None, str, or callable
+        The scoring function (or name of a function) used for cross-validation.
+        Must be known to scikit-learn. See the description of *scoring* in
+        :func:`sklearn.model_selection.cross_val_score` for details. If None,
+        will fall back to the :meth:`verde.Spline.score` method.
 
     Attributes
     ----------
     force_ : array
         The estimated forces that fit the observed data.
     force_coords_ : tuple of arrays
         The easting and northing coordinates of the point forces. Same as
@@ -122,36 +130,58 @@
     Spline : The bi-harmonic spline
     cross_val_score : Score an estimator/gridder using cross-validation
 
     """
 
     def __init__(
         self,
-        mindists=(1e3, 10e3, 100e3),
+        mindists=None,
         dampings=(1e-10, 1e-5, 1e-1),
         force_coords=None,
         engine="auto",
         cv=None,
         client=None,
         delayed=False,
+        scoring=None,
     ):
         super().__init__()
         self.dampings = dampings
-        self.mindists = mindists
+        if mindists is None:
+            self.mindists = [0]
+        else:
+            self.mindists = mindists
+            warnings.warn(
+                "The mindists parameter of verde.SplineCV is no longer "
+                "required and will be removed in Verde 2.0.0. Use the default "
+                "value to obtain the future behavior.",
+                FutureWarning,
+                stacklevel=2,
+            )
         self.force_coords = force_coords
         self.engine = engine
         self.cv = cv
         self.client = client
         self.delayed = delayed
+        self.scoring = scoring
+        if engine != "auto":
+            warnings.warn(
+                "The 'engine' parameter of 'verde.SplineCV' is "
+                "deprecated and will be removed in Verde 2.0.0. "
+                "The faster and memory efficient numba engine will be "
+                "the only option.",
+                FutureWarning,
+                stacklevel=2,
+            )
         if client is not None:
             warnings.warn(
                 "The 'client' parameter of 'verde.SplineCV' is "
                 "deprecated and will be removed in Verde 2.0.0. "
                 "Use the 'delayed' parameter instead.",
                 FutureWarning,
+                stacklevel=2,
             )
 
     def fit(self, coordinates, data, weights=None):
         """
         Fit the spline to the given data and automatically tune parameters.
 
         For each combination of the parameters given, computes the mean cross
@@ -216,14 +246,15 @@
                 score = cross_val_score(
                     spline,
                     coordinates=coordinates,
                     data=data,
                     weights=weights,
                     cv=self.cv,
                     delayed=self.delayed,
+                    scoring=self.scoring,
                 )
                 scores.append(dispatch(np.mean, delayed=self.delayed)(score))
         best = dispatch(np.argmax, delayed=self.delayed)(scores)
         if self.delayed:
             best = best.compute()
         else:
             scores = np.asarray(scores)
@@ -321,32 +352,35 @@
     Before fitting, the Jacobian (design, sensitivity, feature, etc) matrix for
     the spline is normalized using
     :class:`sklearn.preprocessing.StandardScaler` without centering the mean so
     that the transformation can be undone in the estimated forces.
 
     Parameters
     ----------
-    mindist : float
-        A minimum distance between the point forces and data points. Needed
-        because the Green's functions are singular when forces and data points
-        coincide. Acts as a fudge factor.
+    mindist : float or None
+        **DEPRECATED:** This argument is no longer needed and will be removed
+        in Verde 2.0.0. This fudge factor is no longer required since a new
+        formulation eliminates the singularity at zero distance. Use the
+        default value of ``mindist=None`` to get the future behaviour. A
+        minimum distance between the point forces and data points.
     damping : None or float
         The positive damping regularization parameter. Controls how much
         smoothness is imposed on the estimated forces. If None, no
         regularization is used.
     force_coords : None or tuple of arrays
         The easting and northing coordinates of the point forces. If None
         (default), then will be set to the data coordinates used to fit the
         spline.
     engine : str
-        Computation engine for the Jacobian matrix and prediction. Can be
-        ``'auto'``, ``'numba'``, or ``'numpy'``. If ``'auto'``, will use numba
-        if it is installed or numpy otherwise. The numba version is
-        multi-threaded and usually faster, which makes fitting and predicting
-        faster.
+        **DEPRECATED:** This option is deprecated and will be removed in Verde
+        v2.0.0. The numba engine will be the only option. Computation engine
+        for the Jacobian matrix and prediction. Can be ``'auto'``, ``'numba'``,
+        or ``'numpy'``. If ``'auto'``, will use numba if it is installed or
+        numpy otherwise. The numba version is multi-threaded and usually
+        faster, which makes fitting and predicting faster.
 
     Attributes
     ----------
     force_ : array
         The estimated forces that fit the observed data.
     force_coords_ : tuple of arrays
         The easting and northing coordinates of the point forces. Same as
@@ -359,20 +393,39 @@
 
     See also
     --------
     SplineCV : Cross-validated version of the bi-harmonic spline
 
     """
 
-    def __init__(self, mindist=1e-5, damping=None, force_coords=None, engine="auto"):
+    def __init__(self, mindist=None, damping=None, force_coords=None, engine="auto"):
         super().__init__()
-        self.mindist = mindist
         self.damping = damping
         self.force_coords = force_coords
         self.engine = engine
+        if engine != "auto":
+            warnings.warn(
+                "The 'engine' parameter of 'verde.Spline' is "
+                "deprecated and will be removed in Verde 2.0.0. "
+                "The faster and memory efficient numba engine will be "
+                "the only option.",
+                FutureWarning,
+                stacklevel=2,
+            )
+        if mindist is None:
+            self.mindist = 0
+        else:
+            self.mindist = mindist
+            warnings.warn(
+                "The mindist parameter of verde.Spline is no longer required "
+                "and will be removed in Verde 2.0.0. Use the default value "
+                "to obtain the future behavior.",
+                FutureWarning,
+                stacklevel=2,
+            )
 
     def fit(self, coordinates, data, weights=None):
         """
         Fit the biharmonic spline to the given data.
 
         The data region is captured and used as default for the
         :meth:`~verde.Spline.grid` and :meth:`~verde.Spline.scatter` methods.
@@ -499,67 +552,99 @@
 
     """
     # Check if we're using weights without damping and warn the user that it
     # might not have any effect.
     if weights is not None and spline.damping is None:
         warnings.warn(
             "Weights might have no effect if no regularization is used. "
-            "Use damping or specify force positions that are different from the data."
+            "Use damping or specify force positions that are different from the data.",
+            stacklevel=2,
         )
 
 
-def greens_func(east, north, mindist):
+def greens_func_numpy(east, north, mindist):
+    "Calculate the Green's function for the Bi-Harmonic Spline"
+    distance = np.sqrt(east**2 + north**2)
+    # The mindist factor was used to avoid NaNs when the distance approaches
+    # zero and the log tents to -infinity. This is no longer needed with
+    # current implementation below. Keep it for compatibility only but remove
+    # in Verde 2.0.0.
+    distance += mindist
+    # Calculate this way instead of x²(log(x) - 1) to avoid calculating log of
+    # 0. The limit for this as x->0 is 0 anyway. This is good for small values
+    # of distance but for larger distances it fails because of an overflow in
+    # the power operator. Saw this on Wikipedia but there was no citation in
+    # December 2022: https://en.wikipedia.org/wiki/Radial_basis_function
+    result = np.empty_like(distance)
+    small = distance < 1
+    big = ~small
+    result[small] = distance[small] * (
+        np.log(distance[small] ** distance[small]) - distance[small]
+    )
+    result[big] = distance[big] ** 2 * (np.log(distance[big]) - 1)
+    return result
+
+
+@jit(nopython=True)
+def greens_func_jit(east, north, mindist):
     "Calculate the Green's function for the Bi-Harmonic Spline"
     distance = np.sqrt(east**2 + north**2)
-    # The mindist factor helps avoid singular matrices when the force and
-    # computation point are too close
+    # The mindist factor was used to avoid NaNs when the distance approaches
+    # zero and the log tents to -infinity. This is no longer needed with
+    # current implementation below. Keep it for compatibility only but remove
+    # in Verde 2.0.0.
     distance += mindist
-    return (distance**2) * (np.log(distance) - 1)
+    # Calculate this way instead of x²(log(x) - 1) to avoid calculating log of
+    # 0. The limit for this as x->0 is 0 anyway. This is good for small values
+    # of distance but for larger distances it fails because of an overflow in
+    # the power operator. Saw this on Wikipedia but there was no citation in
+    # December 2022: https://en.wikipedia.org/wiki/Radial_basis_function
+    if distance < 1:
+        result = distance * (np.log(distance**distance) - distance)
+    else:
+        result = distance**2 * (np.log(distance) - 1)
+    return result
 
 
 def predict_numpy(east, north, force_east, force_north, mindist, forces, result):
     "Calculate the predicted data using numpy."
     result[:] = 0
     for j in range(forces.size):
-        green = greens_func(east - force_east[j], north - force_north[j], mindist)
+        green = greens_func_numpy(east - force_east[j], north - force_north[j], mindist)
         result += green * forces[j]
     return result
 
 
 def jacobian_numpy(east, north, force_east, force_north, mindist, jac):
     "Calculate the Jacobian using numpy broadcasting."
     # Reshaping the data to a column vector will automatically build a distance
     # matrix between each data point and force.
-    jac[:] = greens_func(
+    jac[:] = greens_func_numpy(
         east.reshape((east.size, 1)) - force_east,
         north.reshape((north.size, 1)) - force_north,
         mindist,
     )
     return jac
 
 
-@jit(nopython=True, fastmath=True, parallel=True)
+@jit(nopython=True, parallel=True)
 def predict_numba(east, north, force_east, force_north, mindist, forces, result):
     "Calculate the predicted data using numba to speed things up."
     for i in numba.prange(east.size):
         result[i] = 0
         for j in range(forces.size):
-            green = GREENS_FUNC_JIT(
+            green = greens_func_jit(
                 east[i] - force_east[j], north[i] - force_north[j], mindist
             )
             result[i] += green * forces[j]
     return result
 
 
-@jit(nopython=True, fastmath=True, parallel=True)
+@jit(nopython=True, parallel=True)
 def jacobian_numba(east, north, force_east, force_north, mindist, jac):
     "Calculate the Jacobian matrix using numba to speed things up."
     for i in numba.prange(east.size):
         for j in range(force_east.size):
-            jac[i, j] = GREENS_FUNC_JIT(
+            jac[i, j] = greens_func_jit(
                 east[i] - force_east[j], north[i] - force_north[j], mindist
             )
     return jac
-
-
-# Jit compile the Green's functions for use in the numba functions
-GREENS_FUNC_JIT = jit(nopython=True, fastmath=True)(greens_func)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `verde-1.7.0/verde/tests/baseline/test_setup_baja_bathymetry.png` & `verde-1.8.0/verde/tests/baseline/test_setup_baja_bathymetry.png`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/baseline/test_setup_california_gps.png` & `verde-1.8.0/verde/tests/baseline/test_setup_california_gps.png`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/baseline/test_setup_rio_magnetic.png` & `verde-1.8.0/verde/tests/baseline/test_setup_rio_magnetic.png`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/baseline/test_setup_texas_wind.png` & `verde-1.8.0/verde/tests/baseline/test_setup_texas_wind.png`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_base.py` & `verde-1.8.0/verde/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # This code is part of the Fatiando a Terra project (https://www.fatiando.org)
 #
 """
 Test the base classes and their utility functions.
 """
-import warnings
-
 import numpy as np
 import numpy.testing as npt
 import pytest
 
 from ..base.base_classes import (
     BaseBlockCrossValidator,
     BaseGridder,
@@ -146,15 +144,16 @@
     # Grid passing grid coordinates
     grids.append(grd.grid(coordinates=coordinates_true))
     # Grid passing grid coordinates as 1d arrays
     grids.append(grd.grid(coordinates=tuple(np.unique(c) for c in coordinates_true)))
     # Grid on profile
     prof = grd.profile((0, -10), (10, -10), 30)
     # Grid on scatter
-    scat = grd.scatter(region=region, size=1000, random_state=0)
+    with pytest.warns(FutureWarning):
+        scat = grd.scatter(region=region, size=1000, random_state=0)
 
     for grid in grids:
         npt.assert_allclose(grid.scalars.values, data_true)
         npt.assert_allclose(grid.easting.values, coordinates_true[0][0, :])
         npt.assert_allclose(grid.northing.values, coordinates_true[1][:, 0])
     npt.assert_allclose(scat.scalars, data)
     npt.assert_allclose(
@@ -384,23 +383,14 @@
         grd.grid(coordinates=grid_coords, shape=(30, 30))
     # Check error is raised if coordinates and spacing are passed
     with pytest.raises(ValueError):
         grd.grid(coordinates=grid_coords, spacing=10)
     # Check error is raised if both coordinates and region are passed
     with pytest.raises(ValueError):
         grd.grid(coordinates=grid_coords, region=region)
-    # Check if FutureWarning is raised after passing region, spacing or shape
-    with warnings.catch_warnings(record=True) as warns:
-        grd.grid(region=region, shape=(4, 4))
-        assert len(warns) == 1
-        assert issubclass(warns[0].category, FutureWarning)
-    with warnings.catch_warnings(record=True) as warns:
-        grd.grid(region=region, spacing=1)
-        assert len(warns) == 1
-        assert issubclass(warns[0].category, FutureWarning)
 
 
 def test_check_fit_input():
     "Make sure no exceptions are raised for standard cases"
     size = 20
     data = np.arange(size)
     coords = (np.arange(size), np.arange(size))
```

### Comparing `verde-1.7.0/verde/tests/test_blockreduce.py` & `verde-1.8.0/verde/tests/test_blockreduce.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_chain.py` & `verde-1.8.0/verde/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_coordinates.py` & `verde-1.8.0/verde/tests/test_coordinates.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 import numpy as np
 import numpy.testing as npt
 import pytest
 
 from ..coordinates import (
     check_region,
     grid_coordinates,
+    line_coordinates,
     longitude_continuity,
     profile_coordinates,
     rolling_window,
-    spacing_to_shape,
+    spacing_to_size,
 )
 
 
 def test_rolling_window_invalid_coordinate_shapes():
     "Shapes of input coordinates must all be the same"
     coordinates = [np.arange(10), np.arange(10).reshape((5, 2))]
     with pytest.raises(ValueError):
@@ -94,51 +95,71 @@
             + r"than dimensions of the region "
             + r"'\({0}, {0}, {0}, {0}\)'.".format(float_regex)
         )
         with pytest.raises(ValueError, match=err_msg):
             rolling_window(coords, size=oversize, spacing=2)
 
 
-def test_spacing_to_shape():
-    "Check that correct spacing and region are returned"
-    region = (-10, 0, 0, 5)
+def test_spacing_to_size():
+    "Check that correct size and stop are returned"
+    start, stop = -10, 0
 
-    shape, new_region = spacing_to_shape(region, spacing=2.5, adjust="spacing")
-    npt.assert_allclose(shape, (3, 5))
-    npt.assert_allclose(new_region, region)
+    size, new_stop = spacing_to_size(start, stop, spacing=2.5, adjust="spacing")
+    npt.assert_allclose(size, 5)
+    npt.assert_allclose(new_stop, stop)
 
-    shape, new_region = spacing_to_shape(region, spacing=(2.5, 2), adjust="spacing")
-    npt.assert_allclose(shape, (3, 6))
-    npt.assert_allclose(new_region, region)
+    size, new_stop = spacing_to_size(start, stop, spacing=2, adjust="spacing")
+    npt.assert_allclose(size, 6)
+    npt.assert_allclose(new_stop, stop)
 
-    shape, new_region = spacing_to_shape(region, spacing=2.6, adjust="spacing")
-    npt.assert_allclose(shape, (3, 5))
-    npt.assert_allclose(new_region, region)
+    size, new_stop = spacing_to_size(start, stop, spacing=2.6, adjust="spacing")
+    npt.assert_allclose(size, 5)
+    npt.assert_allclose(new_stop, stop)
 
-    shape, new_region = spacing_to_shape(region, spacing=2.4, adjust="spacing")
-    npt.assert_allclose(shape, (3, 5))
-    npt.assert_allclose(new_region, region)
+    size, new_stop = spacing_to_size(start, stop, spacing=2.4, adjust="spacing")
+    npt.assert_allclose(size, 5)
+    npt.assert_allclose(new_stop, stop)
 
-    shape, new_region = spacing_to_shape(region, spacing=(2.4, 1.9), adjust="spacing")
-    npt.assert_allclose(shape, (3, 6))
-    npt.assert_allclose(new_region, region)
+    size, new_stop = spacing_to_size(start, stop, spacing=2.6, adjust="region")
+    npt.assert_allclose(size, 5)
+    npt.assert_allclose(new_stop, 0.4)
 
-    shape, new_region = spacing_to_shape(region, spacing=2.6, adjust="region")
-    npt.assert_allclose(shape, (3, 5))
-    npt.assert_allclose(new_region, (-10, 0.4, 0, 5.2))
+    size, new_stop = spacing_to_size(start, stop, spacing=2.4, adjust="region")
+    npt.assert_allclose(size, 5)
+    npt.assert_allclose(new_stop, -0.4)
 
-    shape, new_region = spacing_to_shape(region, spacing=(2.6, 2.4), adjust="region")
-    npt.assert_allclose(shape, (3, 5))
-    npt.assert_allclose(new_region, (-10, -0.4, 0, 5.2))
 
-
-def test_spacing_to_shape_fails():
-    "Should fail if more than 2 spacings are given"
+def test_line_coordinates_fails():
+    "Check failures for invalid arguments"
+    start, stop = 0, 1
+    size = 10
+    spacing = 0.1
+    # Make sure it doesn't fail for these parameters
+    line_coordinates(start, stop, size=size)
+    line_coordinates(start, stop, spacing=spacing)
     with pytest.raises(ValueError):
-        spacing_to_shape((0, 1, 0, 1), (1, 2, 3), adjust="region")
+        line_coordinates(start, stop)
+    with pytest.raises(ValueError):
+        line_coordinates(start, stop, size=size, spacing=spacing)
+
+
+def test_line_coordinates_spacing_larger_than_twice_interval():
+    "Check if pixel_register works when the spacing is greater than the limits"
+    start, stop = 0, 1
+    spacing = 3
+    coordinates = line_coordinates(start, stop, spacing=spacing)
+    npt.assert_allclose(coordinates, [0, 1])
+    coordinates = line_coordinates(start, stop, spacing=spacing, pixel_register=True)
+    npt.assert_allclose(coordinates, [0.5])
+    coordinates = line_coordinates(start, stop, spacing=spacing, adjust="region")
+    npt.assert_allclose(coordinates, [0, 3])
+    coordinates = line_coordinates(
+        start, stop, spacing=spacing, pixel_register=True, adjust="region"
+    )
+    npt.assert_allclose(coordinates, [1.5])
 
 
 def test_grid_coordinates_fails():
     "Check failures for invalid arguments"
     region = (0, 1, 0, 10)
     shape = (10, 20)
     spacing = 0.5
@@ -148,14 +169,16 @@
 
     with pytest.raises(ValueError):
         grid_coordinates(region, shape=shape, spacing=spacing)
     with pytest.raises(ValueError):
         grid_coordinates(region, shape=None, spacing=None)
     with pytest.raises(ValueError):
         grid_coordinates(region, spacing=spacing, adjust="invalid adjust")
+    with pytest.raises(ValueError):
+        grid_coordinates(region, spacing=(1, 2, 3))
 
 
 def test_check_region():
     "Make sure an exception is raised for bad regions"
     with pytest.raises(ValueError):
         check_region([])
     with pytest.raises(ValueError):
@@ -279,7 +302,15 @@
     longitude, latitude = grid_coordinates(boundaries, spacing=spacing)
     latitude[0] = -100
     with pytest.raises(ValueError):
         longitude_continuity([longitude, latitude], region)
     latitude[0] = 100
     with pytest.raises(ValueError):
         longitude_continuity([longitude, latitude], region)
+
+
+def test_meshgrid_extra_coords_error():
+    "Should raise an exception if meshgrid=False and extra_coords are used"
+    with pytest.raises(ValueError):
+        grid_coordinates(
+            region=(0, 1, 0, 3), spacing=0.1, meshgrid=False, extra_coords=10
+        )
```

### Comparing `verde-1.7.0/verde/tests/test_datasets.py` & `verde-1.8.0/verde/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_distances.py` & `verde-1.8.0/verde/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_io.py` & `verde-1.8.0/verde/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_mask.py` & `verde-1.8.0/verde/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_minimal.py` & `verde-1.8.0/verde/tests/test_minimal.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_model_selection.py` & `verde-1.8.0/verde/tests/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_projections.py` & `verde-1.8.0/verde/tests/test_projections.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 Test the projection functions.
 """
 import numpy as np
 import numpy.testing as npt
 import pytest
 import xarray as xr
 
+from ..neighbors import KNeighbors
 from ..projections import project_grid
-from ..scipygridder import ScipyGridder
 
 
 def projection(longitude, latitude):
     "Dummy projection"
     return longitude**2, latitude**2
 
 
 @pytest.mark.parametrize(
     "method",
-    ["nearest", "linear", "cubic", ScipyGridder("nearest")],
+    ["nearest", "linear", "cubic", KNeighbors()],
     ids=["nearest", "linear", "cubic", "gridder"],
 )
 def test_project_grid(method):
     "Use a simple projection to test that the output is as expected"
     shape = (50, 40)
     lats = np.linspace(2, 10, shape[1])
     lons = np.linspace(-10, 2, shape[0])
@@ -115,7 +115,18 @@
         np.linspace(0, 100, shape[2]),
     ]
     dims = ("height", "latitude", "longitude")
     data = np.ones(shape[:ndims], dtype="float")
     grid = xr.DataArray(data, coords=coords[:ndims], dims=dims[:ndims])
     with pytest.raises(ValueError):
         project_grid(grid, projection)
+
+
+def test_project_grid_fails_method():
+    "Should fail for invalid method name"
+    shape = (50, 40)
+    lats = np.linspace(2, 10, shape[1])
+    lons = np.linspace(-10, 2, shape[0])
+    data = np.ones(shape, dtype="float")
+    grid = xr.DataArray(data, coords=[lons, lats], dims=("latitude", "longitude"))
+    with pytest.raises(ValueError):
+        project_grid(grid, projection, method="some invalid method")
```

### Comparing `verde-1.7.0/verde/tests/test_scipy.py` & `verde-1.8.0/verde/tests/test_scipy.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,66 +11,124 @@
 
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import pytest
 
 from ..coordinates import grid_coordinates
-from ..scipygridder import ScipyGridder
+from ..scipygridder import Cubic, Linear, ScipyGridder
 from ..synthetic import CheckerBoard
 
 
-def test_scipy_gridder_same_points():
+@pytest.mark.parametrize(
+    "gridder",
+    [
+        ScipyGridder(method="nearest"),
+        ScipyGridder(method="linear"),
+        ScipyGridder(method="cubic"),
+        Linear(),
+        Linear(rescale=False),
+        Cubic(),
+        Cubic(rescale=False),
+    ],
+    ids=[
+        "nearest(scipy)",
+        "linear(scipy)",
+        "cubic(scipy)",
+        "linear",
+        "linear_norescale",
+        "cubic",
+        "cubic_norescale",
+    ],
+)
+def test_scipy_gridder_same_points(gridder):
     "See if the gridder recovers known points."
     region = (1000, 5000, -8000, -7000)
     synth = CheckerBoard(region=region)
     data = synth.scatter(size=1000, random_state=0)
     coords = (data.easting, data.northing)
     # The interpolation should be perfect on top of the data points
-    for method in ["nearest", "linear", "cubic"]:
-        grd = ScipyGridder(method=method)
-        grd.fit(coords, data.scalars)
-        predicted = grd.predict(coords)
-        npt.assert_allclose(predicted, data.scalars)
-        npt.assert_allclose(grd.score(coords, data.scalars), 1)
-
-
-def test_scipy_gridder():
+    gridder.fit(coords, data.scalars)
+    predicted = gridder.predict(coords)
+    npt.assert_allclose(predicted, data.scalars)
+    npt.assert_allclose(gridder.score(coords, data.scalars), 1)
+
+
+@pytest.mark.parametrize(
+    "gridder",
+    [
+        ScipyGridder(method="linear"),
+        ScipyGridder(method="cubic"),
+        Linear(),
+        Linear(rescale=False),
+        Cubic(),
+        Cubic(rescale=False),
+    ],
+    ids=[
+        "cubic(scipy)",
+        "cubic(scipy)",
+        "linear",
+        "linear_norescale",
+        "cubic",
+        "cubic_norescale",
+    ],
+)
+def test_scipy_gridder(gridder):
     "See if the gridder recovers known points."
     synth = CheckerBoard(region=(1000, 5000, -8000, -6000))
     data = synth.scatter(size=20000, random_state=0)
     coords = (data.easting, data.northing)
     pt_coords = (3000, -7000)
     true_data = synth.predict(pt_coords)
     # nearest will never be too close to the truth
-    grd = ScipyGridder("cubic").fit(coords, data.scalars)
-    npt.assert_almost_equal(grd.predict(pt_coords), true_data, decimal=2)
-    grd = ScipyGridder("linear").fit(coords, data.scalars)
-    npt.assert_almost_equal(grd.predict(pt_coords), true_data, decimal=1)
+    gridder.fit(coords, data.scalars)
+    npt.assert_almost_equal(gridder.predict(pt_coords), true_data, decimal=1)
+
+
+@pytest.mark.parametrize(
+    "gridder",
+    [
+        ScipyGridder(method="cubic"),
+        Linear(),
+    ],
+    ids=["cubic(scipy)", "linear"],
+)
+def test_scipy_gridder_region_xarray(gridder):
+    "See if the region is gotten from the data is correct."
+    region = (1000, 5000, -8000, -6000)
+    synth = CheckerBoard(region=region)
+    grid = synth.grid(shape=(101, 101))
+    coords = grid_coordinates(region, grid.scalars.shape)
+    gridder.fit(coords, grid.scalars)
+    npt.assert_allclose(gridder.region_, region)
 
 
-def test_scipy_gridder_region():
+@pytest.mark.parametrize(
+    "gridder",
+    [
+        ScipyGridder(method="cubic"),
+        Linear(),
+    ],
+    ids=["cubic(scipy)", "linear"],
+)
+def test_scipy_gridder_region_pandas(gridder):
     "See if the region is gotten from the data is correct."
     region = (1000, 5000, -8000, -6000)
     synth = CheckerBoard(region=region)
-    # Test using xarray objects
     grid = synth.grid(shape=(101, 101))
     coords = grid_coordinates(region, grid.scalars.shape)
-    grd = ScipyGridder().fit(coords, grid.scalars)
-    npt.assert_allclose(grd.region_, region)
-    # Test using pandas objects
     data = pd.DataFrame(
         {
             "easting": coords[0].ravel(),
             "northing": coords[1].ravel(),
             "scalars": grid.scalars.values.ravel(),
         }
     )
-    grd = ScipyGridder().fit((data.easting, data.northing), data.scalars)
-    npt.assert_allclose(grd.region_, region)
+    gridder.fit((data.easting, data.northing), data.scalars)
+    npt.assert_allclose(gridder.region_, region)
 
 
 def test_scipy_gridder_extra_args():
     "Passing in extra arguments to scipy"
     data = CheckerBoard().scatter(random_state=100)
     coords = (data.easting, data.northing)
     grd = ScipyGridder(method="linear", extra_args=dict(rescale=True))
```

### Comparing `verde-1.7.0/verde/tests/test_spline.py` & `verde-1.8.0/verde/tests/test_spline.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import numpy as np
 import numpy.testing as npt
 import pytest
 from dask.distributed import Client
 from sklearn.model_selection import ShuffleSplit
 
+from ..model_selection import cross_val_score
 from ..spline import Spline, SplineCV
 from ..synthetic import CheckerBoard
 from .utils import requires_numba
 
 
 @pytest.mark.parametrize(
     "delayed,client,engine",
@@ -35,23 +36,21 @@
     synth = CheckerBoard(region=region)
     data = synth.scatter(size=1500, random_state=0)
     coords = (data.easting, data.northing)
     # Can't test on many configurations because it takes too long for regular
     # testing
     spline = SplineCV(
         dampings=[None, 1e3],
-        mindists=[1e-7, 1e6],
         cv=ShuffleSplit(n_splits=1, random_state=0),
         delayed=delayed,
         client=client,
         engine=engine,
     ).fit(coords, data.scalars)
     if client is not None:
         client.close()
-    assert spline.mindist_ == 1e-7
     assert spline.damping_ is None
     # The interpolation should be perfect on top of the data points
     npt.assert_allclose(spline.predict(coords), data.scalars, rtol=1e-5)
     npt.assert_allclose(spline.score(coords, data.scalars), 1)
     npt.assert_allclose(spline.force_coords_, coords)
     # There should be 1 force per data point
     assert data.scalars.size == spline.force_.size
@@ -95,14 +94,33 @@
     npt.assert_allclose(
         spline.grid(region=region, shape=shape).scalars,
         synth.grid(region=region, shape=shape).scalars,
         rtol=5e-2,
     )
 
 
+def test_spline_cv_scoring():
+    "Check scoring parameter works with SplineCV"
+    region = (100, 500, -800, -700)
+    synth = CheckerBoard(region=region)
+    data = synth.scatter(size=1500, random_state=1)
+    coords = (data.easting, data.northing)
+    # Compare SplineCV to results from Spline with cross_val_score
+    for score in ["r2", "neg_root_mean_squared_error"]:
+        spline = Spline(damping=None)
+        score_spline = np.mean(
+            cross_val_score(spline, coords, data.scalars, scoring=score)
+        )
+        # Limit SplineCV to a single parameter set equal to Spline's defaults
+        spline_cv = SplineCV(dampings=[None], scoring=score)
+        spline_cv.fit(coords, data.scalars)
+        score_spline_cv = spline_cv.scores_[0]
+        npt.assert_allclose(score_spline, score_spline_cv, rtol=1e-5)
+
+
 def test_spline_weights():
     "Use weights to ignore an outlier"
     data = CheckerBoard().scatter(size=2000, random_state=1)
     data_outlier = data.scalars.copy()
     outlier = 500
     outlier_value = 100e3
     data_outlier[outlier] += outlier_value
@@ -130,16 +148,16 @@
 def test_spline_damping():
     "Test the spline solution with a bit of damping"
     region = (1000, 5000, -8000, -6000)
     synth = CheckerBoard(region=region)
     data = synth.scatter(size=3000, random_state=1)
     coords = (data.easting, data.northing)
     # The interpolation should be close on top of the data points
-    spline = Spline(damping=1e-8, mindist=1000).fit(coords, data.scalars)
-    npt.assert_allclose(spline.predict(coords), data.scalars, rtol=1e-2, atol=1)
+    spline = Spline(damping=1e-8).fit(coords, data.scalars)
+    npt.assert_allclose(spline.predict(coords), data.scalars, rtol=1e-2, atol=10)
     shape = (5, 5)
     region = (2000, 4000, -7500, -6500)
     # Tolerance needs to be kind of high to allow for error due to small
     # dataset
     npt.assert_allclose(
         spline.grid(region=region, shape=shape).scalars,
         synth.grid(region=region, shape=shape).scalars,
```

### Comparing `verde-1.7.0/verde/tests/test_trend.py` & `verde-1.8.0/verde/tests/test_trend.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_utils.py` & `verde-1.8.0/verde/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/test_vector.py` & `verde-1.8.0/verde/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/tests/utils.py` & `verde-1.8.0/verde/tests/utils.py`

 * *Files identical despite different names*

### Comparing `verde-1.7.0/verde/trend.py` & `verde-1.8.0/verde/trend.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,21 +188,21 @@
 
         Examples
         --------
 
         >>> import numpy as np
         >>> east = np.linspace(0, 4, 5)
         >>> north = np.linspace(-5, -1, 5)
-        >>> print(Trend(degree=1).jacobian((east, north), dtype=np.int))
+        >>> print(Trend(degree=1).jacobian((east, north), dtype=int))
         [[ 1  0 -5]
          [ 1  1 -4]
          [ 1  2 -3]
          [ 1  3 -2]
          [ 1  4 -1]]
-        >>> print(Trend(degree=2).jacobian((east, north), dtype=np.int))
+        >>> print(Trend(degree=2).jacobian((east, north), dtype=int))
         [[ 1  0 -5  0  0 25]
          [ 1  1 -4  1 -4 16]
          [ 1  2 -3  4 -6  9]
          [ 1  3 -2  9 -6  4]
          [ 1  4 -1 16 -4  1]]
 
         """
```

### Comparing `verde-1.7.0/verde/utils.py` & `verde-1.8.0/verde/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,23 +224,31 @@
     coordinates,
     data,
     data_names,
     dims=("northing", "easting"),
     extra_coords_names=None,
 ):
     """
-    Create an :class:`xarray.Dataset` grid from numpy arrays
+    Create an :class:`xarray.Dataset` grid from 2D numpy arrays
 
-    This functions creates an :class:`xarray.Dataset` out of 2d gridded data
+    This function creates an :class:`xarray.Dataset` out of 2d gridded data
     including easting and northing coordinates, any extra coordinates (like
     upward elevation, time, etc) and data arrays.
 
     Use this to transform the outputs of :func:`verde.grid_coordinates` and
     the ``predict`` method of a gridder into an :class:`xarray.Dataset`.
 
+    .. important::
+
+        This function does not perform any interpolation or gridding. If you
+        are dealing with 1d arrays and need to interpolate them on a regular
+        grid (a.k.a _grid_ them) you might want to use one of the available
+        interpolators in Verde, like :class:`verde.Spline`,
+        :class:`verde.KNeighbors`, :class:`Linear`, etc.
+
     .. note::
 
         This is a utility function to help create 2D grids (i.e., grids with
         two ``dims`` coordinates). For arbitrary N-dimensional arrays, use
         :mod:`xarray` directly.
 
     Parameters
```

### Comparing `verde-1.7.0/verde/vector.py` & `verde-1.8.0/verde/vector.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,21 +141,14 @@
         return tuple(comp.predict(coordinates) for comp in self.components)
 
 
 class VectorSpline2D(BaseGridder):
     r"""
     Elastically coupled interpolation of 2-component vector data.
 
-    .. warning::
-
-        The :class:`~verde.VectorSpline2D` class is deprecated and will be
-        removed in Verde v2.0.0. Its usage is restricted to GPS/GNSS data and
-        not in the general scope of Verde. Please use the implementation in the
-        `Erizo <https://github.com/fatiando/erizo>`__ package instead.
-
     This gridder assumes Cartesian coordinates.
 
     Uses the Green's functions based on elastic deformation from
     [SandwellWessel2016]_. The interpolation is done by estimating point forces
     that generate an elastic deformation that fits the observed vector data.
     The deformation equations are based on a 2D elastic sheet with a constant
     Poisson's ratio. The data can then be predicted at any desired location.
@@ -201,19 +194,20 @@
         smoothness is imposed on the estimated forces. If None, no
         regularization is used.
     force_coords : None or tuple of arrays
         The easting and northing coordinates of the point forces. If None
         (default), then will be set to the data coordinates the first time
         :meth:`~verde.VectorSpline2D.fit` is called.
     engine : str
-        Computation engine for the Jacobian matrix and predictions. Can be
-        ``'auto'``, ``'numba'``, or ``'numpy'``. If ``'auto'``, will use numba
-        if it is installed or numpy otherwise. The numba version is
-        multi-threaded and usually faster, which makes fitting and predicting
-        faster.
+        **DEPRECATED:** This option is deprecated and will be removed in Verde
+        v2.0.0. The numba engine will be the only option. Computation engine
+        for the Jacobian matrix and prediction. Can be ``'auto'``, ``'numba'``,
+        or ``'numpy'``. If ``'auto'``, will use numba if it is installed or
+        numpy otherwise. The numba version is multi-threaded and usually
+        faster, which makes fitting and predicting faster.
 
     Attributes
     ----------
     force_ : array
         The estimated forces that fit the observed data.
     region_ : tuple
         The boundaries (``[W, E, S, N]``) of the data used to fit the
@@ -228,20 +222,23 @@
     ):
         super().__init__()
         self.poisson = poisson
         self.mindist = mindist
         self.damping = damping
         self.force_coords = force_coords
         self.engine = engine
-        warnings.warn(
-            "VectorSpline2D is deprecated and will be removed in Verde v2.0.0."
-            " Please use the implementation in the Erizo package instead "
-            "(https://github.com/fatiando/erizo).",
-            FutureWarning,
-        )
+        if engine != "auto":
+            warnings.warn(
+                "The 'engine' parameter of 'verde.VectorSpline2D' is "
+                "deprecated and will be removed in Verde 2.0.0. "
+                "The faster and memory efficient numba engine will be "
+                "the only option.",
+                FutureWarning,
+                stacklevel=2,
+            )
 
     def fit(self, coordinates, data, weights=None):
         """
         Fit the gridder to the given 2-component vector data.
 
         The data region is captured and used as default for the
         :meth:`~verde.VectorSpline2D.grid` and
```

### Comparing `verde-1.7.0/verde.egg-info/PKG-INFO` & `verde-1.8.0/verde.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,395 +1,366 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7665 7264  : 2.1.Name: verd
-00000020: 650a 5665 7273 696f 6e3a 2031 2e37 2e30  e.Version: 1.7.0
-00000030: 0a53 756d 6d61 7279 3a20 2250 726f 6365  .Summary: "Proce
-00000040: 7373 696e 6720 616e 6420 6772 6964 6469  ssing and griddi
-00000050: 6e67 2073 7061 7469 616c 2064 6174 612c  ng spatial data,
-00000060: 206d 6163 6869 6e65 2d6c 6561 726e 696e   machine-learnin
-00000070: 6720 7374 796c 6522 0a48 6f6d 652d 7061  g style".Home-pa
-00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000090: 7562 2e63 6f6d 2f66 6174 6961 6e64 6f2f  ub.com/fatiando/
-000000a0: 7665 7264 650a 4175 7468 6f72 3a20 5468  verde.Author: Th
-000000b0: 6520 5665 7264 6520 4465 7665 6c6f 7065  e Verde Develope
-000000c0: 7273 0a41 7574 686f 722d 656d 6169 6c3a  rs.Author-email:
-000000d0: 2066 6174 6961 6e64 6f61 7465 7272 6140   fatiandoaterra@
-000000e0: 7072 6f74 6f6e 6d61 696c 2e63 6f6d 0a4d  protonmail.com.M
-000000f0: 6169 6e74 6169 6e65 723a 2022 4c65 6f6e  aintainer: "Leon
-00000100: 6172 646f 2055 6965 6461 220a 4d61 696e  ardo Uieda".Main
-00000110: 7461 696e 6572 2d65 6d61 696c 3a20 6c65  tainer-email: le
-00000120: 6f75 6965 6461 4067 6d61 696c 2e63 6f6d  ouieda@gmail.com
-00000130: 0a4c 6963 656e 7365 3a20 4253 4420 332d  .License: BSD 3-
-00000140: 436c 6175 7365 204c 6963 656e 7365 0a50  Clause License.P
-00000150: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
-00000160: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
-00000170: 3a2f 2f77 7777 2e66 6174 6961 6e64 6f2e  ://www.fatiando.
-00000180: 6f72 672f 7665 7264 650a 5072 6f6a 6563  org/verde.Projec
-00000190: 742d 5552 4c3a 2052 656c 6561 7365 204e  t-URL: Release N
-000001a0: 6f74 6573 2c20 6874 7470 733a 2f2f 6769  otes, https://gi
-000001b0: 7468 7562 2e63 6f6d 2f66 6174 6961 6e64  thub.com/fatiand
-000001c0: 6f2f 7665 7264 652f 7265 6c65 6173 6573  o/verde/releases
-000001d0: 0a50 726f 6a65 6374 2d55 524c 3a20 4275  .Project-URL: Bu
-000001e0: 6720 5472 6163 6b65 722c 2068 7474 7073  g Tracker, https
-000001f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
-00000200: 7469 616e 646f 2f76 6572 6465 2f69 7373  tiando/verde/iss
-00000210: 7565 730a 5072 6f6a 6563 742d 5552 4c3a  ues.Project-URL:
-00000220: 2053 6f75 7263 6520 436f 6465 2c20 6874   Source Code, ht
-00000230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000240: 2f66 6174 6961 6e64 6f2f 7665 7264 650a  /fatiando/verde.
-00000250: 4b65 7977 6f72 6473 3a20 7370 6174 6961  Keywords: spatia
-00000260: 6c2c 6765 6f73 6369 656e 6365 2c67 656f  l,geoscience,geo
-00000270: 7068 7973 6963 732c 6772 6964 6469 6e67  physics,gridding
-00000280: 2c69 6e74 6572 706f 6c61 7469 6f6e 0a50  ,interpolation.P
-00000290: 6c61 7466 6f72 6d3a 2061 6e79 0a43 6c61  latform: any.Cla
-000002a0: 7373 6966 6965 723a 2044 6576 656c 6f70  ssifier: Develop
-000002b0: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
-000002c0: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
-000002d0: 6162 6c65 0a43 6c61 7373 6966 6965 723a  able.Classifier:
-000002e0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000002f0: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
-00000300: 7365 6172 6368 0a43 6c61 7373 6966 6965  search.Classifie
-00000310: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000320: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000330: 7273 0a43 6c61 7373 6966 6965 723a 2049  rs.Classifier: I
-00000340: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-00000350: 203a 3a20 4564 7563 6174 696f 6e0a 436c   :: Education.Cl
-00000360: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-00000370: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000380: 6420 3a3a 2042 5344 204c 6963 656e 7365  d :: BSD License
-00000390: 0a43 6c61 7373 6966 6965 723a 204e 6174  .Classifier: Nat
-000003a0: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
-000003b0: 2045 6e67 6c69 7368 0a43 6c61 7373 6966   English.Classif
-000003c0: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-000003d0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000003e0: 7065 6e64 656e 740a 436c 6173 7369 6669  pendent.Classifi
-000003f0: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
-00000400: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-00000410: 696e 670a 436c 6173 7369 6669 6572 3a20  ing.Classifier: 
-00000420: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
-00000430: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
-00000440: 204c 6962 7261 7269 6573 0a43 6c61 7373   Libraries.Class
-00000450: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000460: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000470: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-00000480: 6c79 0a43 6c61 7373 6966 6965 723a 2050  ly.Classifier: P
-00000490: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000004a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000004b0: 2033 2e36 0a43 6c61 7373 6966 6965 723a   3.6.Classifier:
-000004c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000004d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000004e0: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
-000004f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000500: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000510: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-00000520: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000530: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000540: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-00000550: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000560: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000570: 7974 686f 6e20 3a3a 2033 2e31 300a 5265  ython :: 3.10.Re
-00000580: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
-00000590: 3d33 2e36 0a44 6573 6372 6970 7469 6f6e  =3.6.Description
-000005a0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-000005b0: 6578 742f 782d 7273 740a 4c69 6365 6e73  ext/x-rst.Licens
-000005c0: 652d 4669 6c65 3a20 4c49 4345 4e53 452e  e-File: LICENSE.
-000005d0: 7478 740a 0a2e 2e20 696d 6167 653a 3a20  txt.... image:: 
-000005e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000005f0: 6f6d 2f66 6174 6961 6e64 6f2f 7665 7264  om/fatiando/verd
-00000600: 652f 7261 772f 6d61 696e 2f64 6f63 2f5f  e/raw/main/doc/_
-00000610: 7374 6174 6963 2f72 6561 646d 652d 6261  static/readme-ba
-00000620: 6e6e 6572 2e70 6e67 0a20 2020 203a 616c  nner.png.    :al
-00000630: 743a 2056 6572 6465 0a0a 6044 6f63 756d  t: Verde..`Docum
-00000640: 656e 7461 7469 6f6e 203c 6874 7470 3a2f  entation <http:/
-00000650: 2f77 7777 2e66 6174 6961 6e64 6f2e 6f72  /www.fatiando.or
-00000660: 672f 7665 7264 653e 605f 5f20 7c0a 6044  g/verde>`__ |.`D
-00000670: 6f63 756d 656e 7461 7469 6f6e 2028 6465  ocumentation (de
-00000680: 7620 7665 7273 696f 6e29 203c 6874 7470  v version) <http
-00000690: 3a2f 2f77 7777 2e66 6174 6961 6e64 6f2e  ://www.fatiando.
-000006a0: 6f72 672f 7665 7264 652f 6465 763e 605f  org/verde/dev>`_
-000006b0: 5f20 7c0a 5061 7274 206f 6620 7468 6520  _ |.Part of the 
-000006c0: 6046 6174 6961 6e64 6f20 6120 5465 7272  `Fatiando a Terr
-000006d0: 6120 3c68 7474 7073 3a2f 2f77 7777 2e66  a <https://www.f
-000006e0: 6174 6961 6e64 6f2e 6f72 673e 605f 5f20  atiando.org>`__ 
-000006f0: 7072 6f6a 6563 740a 0a0a 2e2e 2069 6d61  project..... ima
-00000700: 6765 3a3a 2068 7474 703a 2f2f 696d 672e  ge:: http://img.
-00000710: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000720: 762f 7665 7264 652e 7376 673f 7374 796c  v/verde.svg?styl
-00000730: 653d 666c 6174 2d73 7175 6172 6526 6c61  e=flat-square&la
-00000740: 6265 6c3d 7665 7273 696f 6e0a 2020 2020  bel=version.    
-00000750: 3a61 6c74 3a20 4c61 7465 7374 2076 6572  :alt: Latest ver
-00000760: 7369 6f6e 206f 6e20 5079 5049 0a20 2020  sion on PyPI.   
-00000770: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000780: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000790: 672f 7079 7069 2f76 6572 6465 0a2e 2e20  g/pypi/verde... 
-000007a0: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-000007b0: 696d 672e 7368 6965 6c64 732e 696f 2f63  img.shields.io/c
-000007c0: 6f6e 6461 2f76 6e2f 636f 6e64 612d 666f  onda/vn/conda-fo
-000007d0: 7267 652f 7665 7264 652e 7376 673f 7374  rge/verde.svg?st
-000007e0: 796c 653d 666c 6174 2d73 7175 6172 650a  yle=flat-square.
-000007f0: 2020 2020 3a61 6c74 3a20 4c61 7465 7374      :alt: Latest
-00000800: 2076 6572 7369 6f6e 206f 6e20 636f 6e64   version on cond
-00000810: 612d 666f 7267 650a 2020 2020 3a74 6172  a-forge.    :tar
-00000820: 6765 743a 2068 7474 7073 3a2f 2f67 6974  get: https://git
-00000830: 6875 622e 636f 6d2f 636f 6e64 612d 666f  hub.com/conda-fo
-00000840: 7267 652f 7665 7264 652d 6665 6564 7374  rge/verde-feedst
-00000850: 6f63 6b0a 2e2e 2069 6d61 6765 3a3a 2068  ock... image:: h
-00000860: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000870: 6473 2e69 6f2f 636f 6465 636f 762f 632f  ds.io/codecov/c/
-00000880: 6769 7468 7562 2f66 6174 6961 6e64 6f2f  github/fatiando/
-00000890: 7665 7264 652f 6d61 696e 2e73 7667 3f73  verde/main.svg?s
-000008a0: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-000008b0: 0a20 2020 203a 616c 743a 2054 6573 7420  .    :alt: Test 
-000008c0: 636f 7665 7261 6765 2073 7461 7475 730a  coverage status.
-000008d0: 2020 2020 3a74 6172 6765 743a 2068 7474      :target: htt
-000008e0: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-000008f0: 6768 2f66 6174 6961 6e64 6f2f 7665 7264  gh/fatiando/verd
-00000900: 650a 2e2e 2069 6d61 6765 3a3a 2068 7474  e... image:: htt
-00000910: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000920: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00000930: 6f6e 732f 7665 7264 652e 7376 673f 7374  ons/verde.svg?st
-00000940: 796c 653d 666c 6174 2d73 7175 6172 650a  yle=flat-square.
-00000950: 2020 2020 3a61 6c74 3a20 436f 6d70 6174      :alt: Compat
-00000960: 6962 6c65 2050 7974 686f 6e20 7665 7273  ible Python vers
-00000970: 696f 6e73 2e0a 2020 2020 3a74 6172 6765  ions..    :targe
-00000980: 743a 2068 7474 7073 3a2f 2f70 7970 692e  t: https://pypi.
-00000990: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
-000009a0: 7665 7264 650a 2e2e 2069 6d61 6765 3a3a  verde... image::
-000009b0: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
-000009c0: 656c 6473 2e69 6f2f 6261 6467 652f 646f  elds.io/badge/do
-000009d0: 692d 3130 2e32 3131 3035 2532 466a 6f73  i-10.21105%2Fjos
-000009e0: 732e 3030 3935 372d 626c 7565 2e73 7667  s.00957-blue.svg
-000009f0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
-00000a00: 7265 0a20 2020 203a 616c 743a 2044 6967  re.    :alt: Dig
-00000a10: 6974 616c 204f 626a 6563 7420 4964 656e  ital Object Iden
-00000a20: 7469 6669 6572 2066 6f72 2074 6865 204a  tifier for the J
-00000a30: 4f53 5320 7061 7065 720a 2020 2020 3a74  OSS paper.    :t
-00000a40: 6172 6765 743a 2068 7474 7073 3a2f 2f64  arget: https://d
-00000a50: 6f69 2e6f 7267 2f31 302e 3231 3130 352f  oi.org/10.21105/
-00000a60: 6a6f 7373 2e30 3039 3537 0a0a 0a2e 2e20  joss.00957..... 
-00000a70: 706c 6163 6568 6f6c 6465 722d 666f 722d  placeholder-for-
-00000a80: 646f 632d 696e 6465 780a 0a0a 4162 6f75  doc-index...Abou
-00000a90: 740a 2d2d 2d2d 2d0a 0a2a 2a56 6572 6465  t.-----..**Verde
-00000aa0: 2a2a 2069 7320 6120 5079 7468 6f6e 206c  ** is a Python l
-00000ab0: 6962 7261 7279 2066 6f72 2070 726f 6365  ibrary for proce
-00000ac0: 7373 696e 6720 7370 6174 6961 6c20 6461  ssing spatial da
-00000ad0: 7461 2028 6261 7468 796d 6574 7279 2c0a  ta (bathymetry,.
-00000ae0: 6765 6f70 6879 7369 6373 2073 7572 7665  geophysics surve
-00000af0: 7973 2c20 6574 6329 2061 6e64 2069 6e74  ys, etc) and int
-00000b00: 6572 706f 6c61 7469 6e67 2069 7420 6f6e  erpolating it on
-00000b10: 2072 6567 756c 6172 2067 7269 6473 2028   regular grids (
-00000b20: 692e 652e 2c0a 2a67 7269 6464 696e 672a  i.e.,.*gridding*
-00000b30: 292e 0a0a 4f75 7220 636f 7265 2069 6e74  )...Our core int
-00000b40: 6572 706f 6c61 7469 6f6e 206d 6574 686f  erpolation metho
-00000b50: 6473 2061 7265 2069 6e73 7069 7265 6420  ds are inspired 
-00000b60: 6279 206d 6163 6869 6e65 2d6c 6561 726e  by machine-learn
-00000b70: 696e 672e 0a41 7320 7375 6368 2c20 5665  ing..As such, Ve
-00000b80: 7264 6520 696d 706c 656d 656e 7473 2061  rde implements a
-00000b90: 6e20 696e 7465 7266 6163 6520 7468 6174  n interface that
-00000ba0: 2069 7320 7369 6d69 6c61 7220 746f 2074   is similar to t
-00000bb0: 6865 2070 6f70 756c 6172 0a60 7363 696b  he popular.`scik
-00000bc0: 6974 2d6c 6561 726e 203c 6874 7470 733a  it-learn <https:
-00000bd0: 2f2f 7363 696b 6974 2d6c 6561 726e 2e6f  //scikit-learn.o
-00000be0: 7267 2f3e 605f 5f20 6c69 6272 6172 792e  rg/>`__ library.
-00000bf0: 0a57 6520 616c 736f 2070 726f 7669 6465  .We also provide
-00000c00: 206f 7468 6572 2061 6e61 6c79 7369 7320   other analysis 
-00000c10: 6d65 7468 6f64 7320 7468 6174 2061 7265  methods that are
-00000c20: 206f 6674 656e 2075 7365 6420 696e 2063   often used in c
-00000c30: 6f6d 6269 6e61 7469 6f6e 2077 6974 680a  ombination with.
-00000c40: 6772 6964 6469 6e67 2c20 6c69 6b65 2074  gridding, like t
-00000c50: 7265 6e64 2072 656d 6f76 616c 2c20 626c  rend removal, bl
-00000c60: 6f63 6b65 642f 7769 6e64 6f77 6564 206f  ocked/windowed o
-00000c70: 7065 7261 7469 6f6e 732c 2063 726f 7373  perations, cross
-00000c80: 2d76 616c 6964 6174 696f 6e2c 0a61 6e64  -validation,.and
-00000c90: 206d 6f72 6521 0a0a 0a50 726f 6a65 6374   more!...Project
-00000ca0: 2067 6f61 6c73 0a2d 2d2d 2d2d 2d2d 2d2d   goals.---------
-00000cb0: 2d2d 2d2d 0a0a 2a20 5072 6f76 6964 6520  ----..* Provide 
-00000cc0: 6120 6d61 6368 696e 652d 6c65 6172 6e69  a machine-learni
-00000cd0: 6e67 2069 6e73 7069 7265 6420 696e 7465  ng inspired inte
-00000ce0: 7266 6163 6520 666f 7220 6772 6964 6469  rface for griddi
-00000cf0: 6e67 2073 7061 7469 616c 2064 6174 610a  ng spatial data.
-00000d00: 2a20 496e 7465 6772 6174 696f 6e20 7769  * Integration wi
-00000d10: 7468 2074 6865 2053 6369 7079 2073 7461  th the Scipy sta
-00000d20: 636b 3a20 6e75 6d70 792c 2070 616e 6461  ck: numpy, panda
-00000d30: 732c 2073 6369 6b69 742d 6c65 6172 6e2c  s, scikit-learn,
-00000d40: 2061 6e64 2078 6172 7261 790a 2a20 496e   and xarray.* In
-00000d50: 636c 7564 6520 636f 6d6d 6f6e 2070 726f  clude common pro
-00000d60: 6365 7373 696e 6720 616e 6420 6461 7461  cessing and data
-00000d70: 2070 7265 7061 7261 7469 6f6e 2074 6173   preparation tas
-00000d80: 6b73 2c20 6c69 6b65 2062 6c6f 636b 6564  ks, like blocked
-00000d90: 206d 6561 6e73 2061 6e64 2032 4420 7472   means and 2D tr
-00000da0: 656e 6473 0a2a 2053 7570 706f 7274 2066  ends.* Support f
-00000db0: 6f72 2067 7269 6464 696e 6720 7363 616c  or gridding scal
-00000dc0: 6172 2061 6e64 2076 6563 746f 7220 6461  ar and vector da
-00000dd0: 7461 2028 6c69 6b65 2077 696e 6420 7370  ta (like wind sp
-00000de0: 6565 6420 6f72 2047 5053 2076 656c 6f63  eed or GPS veloc
-00000df0: 6974 6965 7329 0a2a 2053 7570 706f 7274  ities).* Support
-00000e00: 2066 6f72 2062 6f74 6820 4361 7274 6573   for both Cartes
-00000e10: 6961 6e20 616e 6420 6765 6f67 7261 7068  ian and geograph
-00000e20: 6963 2063 6f6f 7264 696e 6174 6573 0a0a  ic coordinates..
-00000e30: 5468 6520 6669 7273 7420 7265 6c65 6173  The first releas
-00000e40: 6520 6f66 2056 6572 6465 2077 6173 2066  e of Verde was f
-00000e50: 6f63 7573 6564 206f 6e20 6d65 6574 696e  ocused on meetin
-00000e60: 6720 6d6f 7374 206f 6620 7468 6573 6520  g most of these 
-00000e70: 696e 6974 6961 6c20 676f 616c 730a 616e  initial goals.an
-00000e80: 6420 6573 7461 626c 6973 6869 6e67 2074  d establishing t
-00000e90: 6865 206c 6f6f 6b20 616e 6420 6665 656c  he look and feel
-00000ea0: 206f 6620 7468 6520 6c69 6272 6172 792e   of the library.
-00000eb0: 0a4c 6174 6572 2072 656c 6561 7365 7320  .Later releases 
-00000ec0: 7769 6c6c 2066 6f63 7573 206f 6e20 6578  will focus on ex
-00000ed0: 7061 6e64 696e 6720 7468 6520 7261 6e67  panding the rang
-00000ee0: 6520 6f66 2067 7269 6464 6572 7320 6176  e of gridders av
-00000ef0: 6169 6c61 626c 652c 0a6f 7074 696d 697a  ailable,.optimiz
-00000f00: 696e 6720 7468 6520 636f 6465 2c20 616e  ing the code, an
-00000f10: 6420 696d 7072 6f76 696e 6720 616c 676f  d improving algo
-00000f20: 7269 7468 6d73 2073 6f20 7468 6174 206c  rithms so that l
-00000f30: 6172 6765 722d 7468 616e 2d6d 656d 6f72  arger-than-memor
-00000f40: 790a 6461 7461 7365 7473 2063 616e 2061  y.datasets can a
-00000f50: 6c73 6f20 6265 2073 7570 706f 7274 6564  lso be supported
-00000f60: 2e0a 0a0a 436f 6e74 6163 7469 6e67 2075  ....Contacting u
-00000f70: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  s.-------------.
-00000f80: 0a46 696e 6420 6f75 7420 6d6f 7265 2061  .Find out more a
-00000f90: 626f 7574 2068 6f77 2074 6f20 7265 6163  bout how to reac
-00000fa0: 6820 7573 2061 740a 6066 6174 6961 6e64  h us at.`fatiand
-00000fb0: 6f2e 6f72 672f 636f 6e74 6163 7420 3c68  o.org/contact <h
-00000fc0: 7474 7073 3a2f 2f77 7777 2e66 6174 6961  ttps://www.fatia
-00000fd0: 6e64 6f2e 6f72 672f 636f 6e74 6163 742f  ndo.org/contact/
-00000fe0: 3e60 5f5f 0a0a 4369 7469 6e67 2056 6572  >`__..Citing Ver
-00000ff0: 6465 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  de.------------.
-00001000: 0a54 6869 7320 6973 2072 6573 6561 7263  .This is researc
-00001010: 6820 736f 6674 7761 7265 202a 2a6d 6164  h software **mad
-00001020: 6520 6279 2073 6369 656e 7469 7374 732a  e by scientists*
-00001030: 2a20 2873 6565 0a60 4155 5448 4f52 532e  * (see.`AUTHORS.
-00001040: 6d64 203c 6874 7470 733a 2f2f 6769 7468  md <https://gith
-00001050: 7562 2e63 6f6d 2f66 6174 6961 6e64 6f2f  ub.com/fatiando/
-00001060: 7665 7264 652f 626c 6f62 2f6d 6169 6e2f  verde/blob/main/
-00001070: 4155 5448 4f52 532e 6d64 3e60 5f5f 292e  AUTHORS.md>`__).
-00001080: 2043 6974 6174 696f 6e73 0a68 656c 7020   Citations.help 
-00001090: 7573 206a 7573 7469 6679 2074 6865 2065  us justify the e
-000010a0: 6666 6f72 7420 7468 6174 2067 6f65 7320  ffort that goes 
-000010b0: 696e 746f 2062 7569 6c64 696e 6720 616e  into building an
-000010c0: 6420 6d61 696e 7461 696e 696e 6720 7468  d maintaining th
-000010d0: 6973 2070 726f 6a65 6374 2e20 4966 2079  is project. If y
-000010e0: 6f75 0a75 7365 6420 5665 7264 6520 666f  ou.used Verde fo
-000010f0: 7220 796f 7572 2072 6573 6561 7263 682c  r your research,
-00001100: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
-00001110: 2063 6974 696e 6720 7573 2e0a 0a53 6565   citing us...See
-00001120: 206f 7572 2060 4349 5441 5449 4f4e 2e72   our `CITATION.r
-00001130: 7374 2066 696c 6520 3c68 7474 7073 3a2f  st file <https:/
-00001140: 2f67 6974 6875 622e 636f 6d2f 6661 7469  /github.com/fati
-00001150: 616e 646f 2f76 6572 6465 2f62 6c6f 622f  ando/verde/blob/
-00001160: 6d61 696e 2f43 4954 4154 494f 4e2e 7273  main/CITATION.rs
-00001170: 743e 605f 5f0a 746f 2066 696e 6420 6f75  t>`__.to find ou
-00001180: 7420 6d6f 7265 2e0a 0a0a 436f 6e74 7269  t more....Contri
-00001190: 6275 7469 6e67 0a2d 2d2d 2d2d 2d2d 2d2d  buting.---------
-000011a0: 2d2d 2d0a 0a43 6f64 6520 6f66 2063 6f6e  ---..Code of con
-000011b0: 6475 6374 0a2b 2b2b 2b2b 2b2b 2b2b 2b2b  duct.+++++++++++
-000011c0: 2b2b 2b2b 0a0a 506c 6561 7365 206e 6f74  ++++..Please not
-000011d0: 6520 7468 6174 2074 6869 7320 7072 6f6a  e that this proj
-000011e0: 6563 7420 6973 2072 656c 6561 7365 6420  ect is released 
-000011f0: 7769 7468 2061 0a60 436f 6e74 7269 6275  with a.`Contribu
-00001200: 746f 7220 436f 6465 206f 6620 436f 6e64  tor Code of Cond
-00001210: 7563 7420 3c68 7474 7073 3a2f 2f67 6974  uct <https://git
-00001220: 6875 622e 636f 6d2f 6661 7469 616e 646f  hub.com/fatiando
-00001230: 2f76 6572 6465 2f62 6c6f 622f 6d61 696e  /verde/blob/main
-00001240: 2f43 4f44 455f 4f46 5f43 4f4e 4455 4354  /CODE_OF_CONDUCT
-00001250: 2e6d 643e 605f 5f2e 0a42 7920 7061 7274  .md>`__..By part
-00001260: 6963 6970 6174 696e 6720 696e 2074 6869  icipating in thi
-00001270: 7320 7072 6f6a 6563 7420 796f 7520 6167  s project you ag
-00001280: 7265 6520 746f 2061 6269 6465 2062 7920  ree to abide by 
-00001290: 6974 7320 7465 726d 732e 0a0a 436f 6e74  its terms...Cont
-000012a0: 7269 6275 7469 6e67 2047 7569 6465 6c69  ributing Guideli
-000012b0: 6e65 730a 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  nes.++++++++++++
-000012c0: 2b2b 2b2b 2b2b 2b2b 2b2b 2b0a 0a50 6c65  +++++++++++..Ple
-000012d0: 6173 6520 7265 6164 206f 7572 0a60 436f  ase read our.`Co
-000012e0: 6e74 7269 6275 7469 6e67 2047 7569 6465  ntributing Guide
-000012f0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001300: 2e63 6f6d 2f66 6174 6961 6e64 6f2f 7665  .com/fatiando/ve
-00001310: 7264 652f 626c 6f62 2f6d 6169 6e2f 434f  rde/blob/main/CO
-00001320: 4e54 5249 4255 5449 4e47 2e6d 643e 605f  NTRIBUTING.md>`_
-00001330: 5f0a 746f 2073 6565 2068 6f77 2079 6f75  _.to see how you
-00001340: 2063 616e 2068 656c 7020 616e 6420 6769   can help and gi
-00001350: 7665 2066 6565 6462 6163 6b2e 0a0a 496d  ve feedback...Im
-00001360: 706f 7374 6572 2073 796e 6472 6f6d 6520  poster syndrome 
-00001370: 6469 7363 6c61 696d 6572 0a2b 2b2b 2b2b  disclaimer.+++++
-00001380: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
-00001390: 2b2b 2b2b 2b2b 2b0a 0a2a 2a57 6520 7761  +++++++..**We wa
-000013a0: 6e74 2079 6f75 7220 6865 6c70 2e2a 2a20  nt your help.** 
-000013b0: 4e6f 2c20 7265 616c 6c79 2e0a 0a54 6865  No, really...The
-000013c0: 7265 206d 6179 2062 6520 6120 6c69 7474  re may be a litt
-000013d0: 6c65 2076 6f69 6365 2069 6e73 6964 6520  le voice inside 
-000013e0: 796f 7572 2068 6561 6420 7468 6174 2069  your head that i
-000013f0: 7320 7465 6c6c 696e 6720 796f 7520 7468  s telling you th
-00001400: 6174 2079 6f75 2772 650a 6e6f 7420 7265  at you're.not re
-00001410: 6164 7920 746f 2062 6520 616e 206f 7065  ady to be an ope
-00001420: 6e20 736f 7572 6365 2063 6f6e 7472 6962  n source contrib
-00001430: 7574 6f72 3b20 7468 6174 2079 6f75 7220  utor; that your 
-00001440: 736b 696c 6c73 2061 7265 6e27 7420 6e65  skills aren't ne
-00001450: 6172 6c79 2067 6f6f 640a 656e 6f75 6768  arly good.enough
-00001460: 2074 6f20 636f 6e74 7269 6275 7465 2e0a   to contribute..
-00001470: 5768 6174 2063 6f75 6c64 2079 6f75 2070  What could you p
-00001480: 6f73 7369 626c 7920 6f66 6665 723f 0a0a  ossibly offer?..
-00001490: 5765 2061 7373 7572 6520 796f 7520 7468  We assure you th
-000014a0: 6174 2074 6865 206c 6974 746c 6520 766f  at the little vo
-000014b0: 6963 6520 696e 2079 6f75 7220 6865 6164  ice in your head
-000014c0: 2069 7320 7772 6f6e 672e 0a0a 2a2a 4265   is wrong...**Be
-000014d0: 696e 6720 6120 636f 6e74 7269 6275 746f  ing a contributo
-000014e0: 7220 646f 6573 6e27 7420 6a75 7374 206d  r doesn't just m
-000014f0: 6561 6e20 7772 6974 696e 6720 636f 6465  ean writing code
-00001500: 2a2a 2e0a 4571 7561 6c6c 7920 696d 706f  **..Equally impo
-00001510: 7274 616e 7420 636f 6e74 7269 6275 7469  rtant contributi
-00001520: 6f6e 7320 696e 636c 7564 653a 0a77 7269  ons include:.wri
-00001530: 7469 6e67 206f 7220 7072 6f6f 662d 7265  ting or proof-re
-00001540: 6164 696e 6720 646f 6375 6d65 6e74 6174  ading documentat
-00001550: 696f 6e2c 2073 7567 6765 7374 696e 6720  ion, suggesting 
-00001560: 6f72 2069 6d70 6c65 6d65 6e74 696e 6720  or implementing 
-00001570: 7465 7374 732c 206f 720a 6576 656e 2067  tests, or.even g
-00001580: 6976 696e 6720 6665 6564 6261 636b 2061  iving feedback a
-00001590: 626f 7574 2074 6865 2070 726f 6a65 6374  bout the project
-000015a0: 2028 696e 636c 7564 696e 6720 6769 7669   (including givi
-000015b0: 6e67 2066 6565 6462 6163 6b20 6162 6f75  ng feedback abou
-000015c0: 7420 7468 650a 636f 6e74 7269 6275 7469  t the.contributi
-000015d0: 6f6e 2070 726f 6365 7373 292e 0a49 6620  on process)..If 
-000015e0: 796f 7527 7265 2063 6f6d 696e 6720 746f  you're coming to
-000015f0: 2074 6865 2070 726f 6a65 6374 2077 6974   the project wit
-00001600: 6820 6672 6573 6820 6579 6573 2c20 796f  h fresh eyes, yo
-00001610: 7520 6d69 6768 7420 7365 6520 7468 6520  u might see the 
-00001620: 6572 726f 7273 2061 6e64 0a61 7373 756d  errors and.assum
-00001630: 7074 696f 6e73 2074 6861 7420 7365 6173  ptions that seas
-00001640: 6f6e 6564 2063 6f6e 7472 6962 7574 6f72  oned contributor
-00001650: 7320 6861 7665 2067 6c6f 7373 6564 206f  s have glossed o
-00001660: 7665 722e 0a49 6620 796f 7520 6361 6e20  ver..If you can 
-00001670: 7772 6974 6520 616e 7920 636f 6465 2061  write any code a
-00001680: 7420 616c 6c2c 2079 6f75 2063 616e 2063  t all, you can c
-00001690: 6f6e 7472 6962 7574 6520 636f 6465 2074  ontribute code t
-000016a0: 6f20 6f70 656e 2073 6f75 7263 652e 0a57  o open source..W
-000016b0: 6520 6172 6520 636f 6e73 7461 6e74 6c79  e are constantly
-000016c0: 2074 7279 696e 6720 6f75 7420 6e65 7720   trying out new 
-000016d0: 736b 696c 6c73 2c20 6d61 6b69 6e67 206d  skills, making m
-000016e0: 6973 7461 6b65 732c 2061 6e64 206c 6561  istakes, and lea
-000016f0: 726e 696e 6720 6672 6f6d 0a74 686f 7365  rning from.those
-00001700: 206d 6973 7461 6b65 732e 0a54 6861 7427   mistakes..That'
-00001710: 7320 686f 7720 7765 2061 6c6c 2069 6d70  s how we all imp
-00001720: 726f 7665 2061 6e64 2077 6520 6172 6520  rove and we are 
-00001730: 6861 7070 7920 746f 2068 656c 7020 6f74  happy to help ot
-00001740: 6865 7273 206c 6561 726e 2e0a 0a2a 5468  hers learn...*Th
-00001750: 6973 2064 6973 636c 6169 6d65 7220 7761  is disclaimer wa
-00001760: 7320 6164 6170 7465 6420 6672 6f6d 2074  s adapted from t
-00001770: 6865 2a0a 604d 6574 5079 2070 726f 6a65  he*.`MetPy proje
-00001780: 6374 203c 6874 7470 733a 2f2f 6769 7468  ct <https://gith
-00001790: 7562 2e63 6f6d 2f55 6e69 6461 7461 2f4d  ub.com/Unidata/M
-000017a0: 6574 5079 3e60 5f5f 2e0a 0a0a 4c69 6365  etPy>`__....Lice
-000017b0: 6e73 650a 2d2d 2d2d 2d2d 2d0a 0a54 6869  nse.-------..Thi
-000017c0: 7320 6973 2066 7265 6520 736f 6674 7761  s is free softwa
-000017d0: 7265 3a20 796f 7520 6361 6e20 7265 6469  re: you can redi
-000017e0: 7374 7269 6275 7465 2069 7420 616e 642f  stribute it and/
-000017f0: 6f72 206d 6f64 6966 7920 6974 2075 6e64  or modify it und
-00001800: 6572 2074 6865 2074 6572 6d73 0a6f 6620  er the terms.of 
-00001810: 7468 6520 2a2a 4253 4420 332d 636c 6175  the **BSD 3-clau
-00001820: 7365 204c 6963 656e 7365 2a2a 2e20 4120  se License**. A 
-00001830: 636f 7079 206f 6620 7468 6973 206c 6963  copy of this lic
-00001840: 656e 7365 2069 7320 7072 6f76 6964 6564  ense is provided
-00001850: 2069 6e0a 604c 4943 454e 5345 2e74 7874   in.`LICENSE.txt
-00001860: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001870: 2e63 6f6d 2f66 6174 6961 6e64 6f2f 7665  .com/fatiando/ve
-00001880: 7264 652f 626c 6f62 2f6d 6169 6e2f 4c49  rde/blob/main/LI
-00001890: 4345 4e53 452e 7478 743e 605f 5f2e 0a0a  CENSE.txt>`__...
-000018a0: 0a                                       .
+00000020: 650a 5665 7273 696f 6e3a 2031 2e38 2e30  e.Version: 1.8.0
+00000030: 0a53 756d 6d61 7279 3a20 5072 6f63 6573  .Summary: Proces
+00000040: 7369 6e67 2061 6e64 2067 7269 6464 696e  sing and griddin
+00000050: 6720 7370 6174 6961 6c20 6461 7461 2c20  g spatial data, 
+00000060: 6d61 6368 696e 652d 6c65 6172 6e69 6e67  machine-learning
+00000070: 2073 7479 6c65 0a48 6f6d 652d 7061 6765   style.Home-page
+00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000090: 2e63 6f6d 2f66 6174 6961 6e64 6f2f 7665  .com/fatiando/ve
+000000a0: 7264 650a 4175 7468 6f72 3a20 5468 6520  rde.Author: The 
+000000b0: 5665 7264 6520 4465 7665 6c6f 7065 7273  Verde Developers
+000000c0: 0a41 7574 686f 722d 656d 6169 6c3a 2066  .Author-email: f
+000000d0: 6174 6961 6e64 6f61 7465 7272 6140 7072  atiandoaterra@pr
+000000e0: 6f74 6f6e 6d61 696c 2e63 6f6d 0a4d 6169  otonmail.com.Mai
+000000f0: 6e74 6169 6e65 723a 2022 4c65 6f6e 6172  ntainer: "Leonar
+00000100: 646f 2055 6965 6461 220a 4d61 696e 7461  do Uieda".Mainta
+00000110: 696e 6572 2d65 6d61 696c 3a20 6c65 6f75  iner-email: leou
+00000120: 6965 6461 4067 6d61 696c 2e63 6f6d 0a4c  ieda@gmail.com.L
+00000130: 6963 656e 7365 3a20 4253 4420 332d 436c  icense: BSD 3-Cl
+00000140: 6175 7365 204c 6963 656e 7365 0a50 726f  ause License.Pro
+00000150: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
+00000160: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
+00000170: 2f77 7777 2e66 6174 6961 6e64 6f2e 6f72  /www.fatiando.or
+00000180: 672f 7665 7264 650a 5072 6f6a 6563 742d  g/verde.Project-
+00000190: 5552 4c3a 2052 656c 6561 7365 204e 6f74  URL: Release Not
+000001a0: 6573 2c20 6874 7470 733a 2f2f 6769 7468  es, https://gith
+000001b0: 7562 2e63 6f6d 2f66 6174 6961 6e64 6f2f  ub.com/fatiando/
+000001c0: 7665 7264 652f 7265 6c65 6173 6573 0a50  verde/releases.P
+000001d0: 726f 6a65 6374 2d55 524c 3a20 4275 6720  roject-URL: Bug 
+000001e0: 5472 6163 6b65 722c 2068 7474 7073 3a2f  Tracker, https:/
+000001f0: 2f67 6974 6875 622e 636f 6d2f 6661 7469  /github.com/fati
+00000200: 616e 646f 2f76 6572 6465 2f69 7373 7565  ando/verde/issue
+00000210: 730a 5072 6f6a 6563 742d 5552 4c3a 2053  s.Project-URL: S
+00000220: 6f75 7263 6520 436f 6465 2c20 6874 7470  ource Code, http
+00000230: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+00000240: 6174 6961 6e64 6f2f 7665 7264 650a 4b65  atiando/verde.Ke
+00000250: 7977 6f72 6473 3a20 7370 6174 6961 6c2c  ywords: spatial,
+00000260: 6765 6f73 6369 656e 6365 2c67 656f 7068  geoscience,geoph
+00000270: 7973 6963 732c 6772 6964 6469 6e67 2c69  ysics,gridding,i
+00000280: 6e74 6572 706f 6c61 7469 6f6e 0a50 6c61  nterpolation.Pla
+00000290: 7466 6f72 6d3a 2061 6e79 0a43 6c61 7373  tform: any.Class
+000002a0: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+000002b0: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+000002c0: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+000002d0: 6c65 0a43 6c61 7373 6966 6965 723a 2049  le.Classifier: I
+000002e0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+000002f0: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+00000300: 6172 6368 0a43 6c61 7373 6966 6965 723a  arch.Classifier:
+00000310: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+00000320: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000330: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+00000340: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000350: 3a20 4564 7563 6174 696f 6e0a 436c 6173  : Education.Clas
+00000360: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+00000370: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000380: 3a3a 2042 5344 204c 6963 656e 7365 0a43  :: BSD License.C
+00000390: 6c61 7373 6966 6965 723a 204e 6174 7572  lassifier: Natur
+000003a0: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
+000003b0: 6e67 6c69 7368 0a43 6c61 7373 6966 6965  nglish.Classifie
+000003c0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000003d0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000003e0: 6e64 656e 740a 436c 6173 7369 6669 6572  ndent.Classifier
+000003f0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
+00000400: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000410: 670a 436c 6173 7369 6669 6572 3a20 546f  g.Classifier: To
+00000420: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000430: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
+00000440: 6962 7261 7269 6573 0a43 6c61 7373 6966  ibraries.Classif
+00000450: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000460: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000470: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
+00000480: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000490: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000004a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000004b0: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
+000004c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000004d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000004e0: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+000004f0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000500: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000510: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+00000520: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000530: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000540: 6e20 3a3a 2033 2e31 300a 5265 7175 6972  n :: 3.10.Requir
+00000550: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
+00000560: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000570: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000580: 6d61 726b 646f 776e 0a50 726f 7669 6465  markdown.Provide
+00000590: 732d 4578 7472 613a 2066 6173 740a 4c69  s-Extra: fast.Li
+000005a0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+000005b0: 4e53 452e 7478 740a 0a3c 696d 6720 7372  NSE.txt..<img sr
+000005c0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+000005d0: 622e 636f 6d2f 6661 7469 616e 646f 2f76  b.com/fatiando/v
+000005e0: 6572 6465 2f72 6177 2f6d 6169 6e2f 646f  erde/raw/main/do
+000005f0: 632f 5f73 7461 7469 632f 7265 6164 6d65  c/_static/readme
+00000600: 2d62 616e 6e65 722e 706e 6722 2061 6c74  -banner.png" alt
+00000610: 3d22 5665 7264 6522 3e0a 0a3c 6832 2061  ="Verde">..<h2 a
+00000620: 6c69 676e 3d22 6365 6e74 6572 223e 5072  lign="center">Pr
+00000630: 6f63 6573 7369 6e67 2061 6e64 2067 7269  ocessing and gri
+00000640: 6464 696e 6720 7370 6174 6961 6c20 6461  dding spatial da
+00000650: 7461 2c20 6d61 6368 696e 652d 6c65 6172  ta, machine-lear
+00000660: 6e69 6e67 2073 7479 6c65 3c2f 6832 3e0a  ning style</h2>.
+00000670: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000680: 7222 3e0a 3c61 2068 7265 663d 2268 7474  r">.<a href="htt
+00000690: 7073 3a2f 2f77 7777 2e66 6174 6961 6e64  ps://www.fatiand
+000006a0: 6f2e 6f72 672f 7665 7264 6522 3e3c 7374  o.org/verde"><st
+000006b0: 726f 6e67 3e44 6f63 756d 656e 7461 7469  rong>Documentati
+000006c0: 6f6e 3c2f 7374 726f 6e67 3e20 286c 6174  on</strong> (lat
+000006d0: 6573 7429 3c2f 613e 20e2 80a2 0a3c 6120  est)</a> ....<a 
+000006e0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+000006f0: 772e 6661 7469 616e 646f 2e6f 7267 2f76  w.fatiando.org/v
+00000700: 6572 6465 2f64 6576 223e 3c73 7472 6f6e  erde/dev"><stron
+00000710: 673e 446f 6375 6d65 6e74 6174 696f 6e3c  g>Documentation<
+00000720: 2f73 7472 6f6e 673e 2028 6d61 696e 2062  /strong> (main b
+00000730: 7261 6e63 6829 3c2f 613e 20e2 80a2 0a3c  ranch)</a> ....<
+00000740: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000750: 6769 7468 7562 2e63 6f6d 2f66 6174 6961  github.com/fatia
+00000760: 6e64 6f2f 7665 7264 652f 626c 6f62 2f6d  ndo/verde/blob/m
+00000770: 6169 6e2f 434f 4e54 5249 4255 5449 4e47  ain/CONTRIBUTING
+00000780: 2e6d 6422 3e3c 7374 726f 6e67 3e43 6f6e  .md"><strong>Con
+00000790: 7472 6962 7574 696e 673c 2f73 7472 6f6e  tributing</stron
+000007a0: 673e 3c2f 613e 20e2 80a2 0a3c 6120 6872  g></a> ....<a hr
+000007b0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+000007c0: 6661 7469 616e 646f 2e6f 7267 2f63 6f6e  fatiando.org/con
+000007d0: 7461 6374 2f22 3e3c 7374 726f 6e67 3e43  tact/"><strong>C
+000007e0: 6f6e 7461 6374 3c2f 7374 726f 6e67 3e3c  ontact</strong><
+000007f0: 2f61 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  /a>.</p>..<p ali
+00000800: 676e 3d22 6365 6e74 6572 223e 0a50 6172  gn="center">.Par
+00000810: 7420 6f66 2074 6865 203c 6120 6872 6566  t of the <a href
+00000820: 3d22 6874 7470 733a 2f2f 7777 772e 6661  ="https://www.fa
+00000830: 7469 616e 646f 2e6f 7267 223e 3c73 7472  tiando.org"><str
+00000840: 6f6e 673e 4661 7469 616e 646f 2061 2054  ong>Fatiando a T
+00000850: 6572 7261 3c2f 7374 726f 6e67 3e3c 2f61  erra</strong></a
+00000860: 3e20 7072 6f6a 6563 740a 3c2f 703e 0a0a  > project.</p>..
+00000870: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000880: 223e 0a3c 6120 6872 6566 3d22 6874 7470  ">.<a href="http
+00000890: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+000008a0: 6f72 672f 7079 7069 2f76 6572 6465 223e  org/pypi/verde">
+000008b0: 3c69 6d67 2073 7263 3d22 6874 7470 3a2f  <img src="http:/
+000008c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000008d0: 7079 7069 2f76 2f76 6572 6465 2e73 7667  pypi/v/verde.svg
+000008e0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+000008f0: 7265 2220 616c 743d 224c 6174 6573 7420  re" alt="Latest 
+00000900: 7665 7273 696f 6e20 6f6e 2050 7950 4922  version on PyPI"
+00000910: 3e3c 2f61 3e0a 3c61 2068 7265 663d 2268  ></a>.<a href="h
+00000920: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000930: 6d2f 636f 6e64 612d 666f 7267 652f 7665  m/conda-forge/ve
+00000940: 7264 652d 6665 6564 7374 6f63 6b22 3e3c  rde-feedstock"><
+00000950: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000960: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000970: 636f 6e64 612f 766e 2f63 6f6e 6461 2d66  conda/vn/conda-f
+00000980: 6f72 6765 2f76 6572 6465 2e73 7667 3f73  orge/verde.svg?s
+00000990: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+000009a0: 2220 616c 743d 224c 6174 6573 7420 7665  " alt="Latest ve
+000009b0: 7273 696f 6e20 6f6e 2063 6f6e 6461 2d66  rsion on conda-f
+000009c0: 6f72 6765 223e 3c2f 613e 0a3c 6120 6872  orge"></a>.<a hr
+000009d0: 6566 3d22 6874 7470 733a 2f2f 636f 6465  ef="https://code
+000009e0: 636f 762e 696f 2f67 682f 6661 7469 616e  cov.io/gh/fatian
+000009f0: 646f 2f76 6572 6465 223e 3c69 6d67 2073  do/verde"><img s
+00000a00: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000a10: 7368 6965 6c64 732e 696f 2f63 6f64 6563  shields.io/codec
+00000a20: 6f76 2f63 2f67 6974 6875 622f 6661 7469  ov/c/github/fati
+00000a30: 616e 646f 2f76 6572 6465 2f6d 6169 6e2e  ando/verde/main.
+00000a40: 7376 673f 7374 796c 653d 666c 6174 2d73  svg?style=flat-s
+00000a50: 7175 6172 6522 2061 6c74 3d22 5465 7374  quare" alt="Test
+00000a60: 2063 6f76 6572 6167 6520 7374 6174 7573   coverage status
+00000a70: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
+00000a80: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+00000a90: 686f 6e2e 6f72 672f 7079 7069 2f76 6572  hon.org/pypi/ver
+00000aa0: 6465 223e 3c69 6d67 2073 7263 3d22 6874  de"><img src="ht
+00000ab0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000ac0: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000ad0: 696f 6e73 2f76 6572 6465 2e73 7667 3f73  ions/verde.svg?s
+00000ae0: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00000af0: 2220 616c 743d 2243 6f6d 7061 7469 626c  " alt="Compatibl
+00000b00: 6520 5079 7468 6f6e 2076 6572 7369 6f6e  e Python version
+00000b10: 732e 223e 3c2f 613e 0a3c 6120 6872 6566  s."></a>.<a href
+00000b20: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+00000b30: 672f 3130 2e32 3131 3035 2f6a 6f73 732e  g/10.21105/joss.
+00000b40: 3030 3935 3722 3e3c 696d 6720 7372 633d  00957"><img src=
+00000b50: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000b60: 656c 6473 2e69 6f2f 6261 6467 652f 646f  elds.io/badge/do
+00000b70: 692d 3130 2e32 3131 3035 2532 466a 6f73  i-10.21105%2Fjos
+00000b80: 732e 3030 3935 372d 626c 7565 3f73 7479  s.00957-blue?sty
+00000b90: 6c65 3d66 6c61 742d 7371 7561 7265 2220  le=flat-square" 
+00000ba0: 616c 743d 2244 4f49 2075 7365 6420 746f  alt="DOI used to
+00000bb0: 2063 6974 6520 7468 6973 2073 6f66 7477   cite this softw
+00000bc0: 6172 6522 3e3c 2f61 3e0a 3c2f 703e 0a0a  are"></a>.</p>..
+00000bd0: 2323 2041 626f 7574 0a0a 2a2a 5665 7264  ## About..**Verd
+00000be0: 652a 2a20 6973 2061 2050 7974 686f 6e20  e** is a Python 
+00000bf0: 6c69 6272 6172 7920 666f 7220 7072 6f63  library for proc
+00000c00: 6573 7369 6e67 2073 7061 7469 616c 2064  essing spatial d
+00000c10: 6174 6120 2874 6f70 6f67 7261 7068 792c  ata (topography,
+00000c20: 2070 6f69 6e74 0a63 6c6f 7564 732c 2062   point.clouds, b
+00000c30: 6174 6879 6d65 7472 792c 2067 656f 7068  athymetry, geoph
+00000c40: 7973 6963 7320 7375 7276 6579 732c 2065  ysics surveys, e
+00000c50: 7463 2920 616e 6420 696e 7465 7270 6f6c  tc) and interpol
+00000c60: 6174 696e 6720 7468 656d 206f 6e20 6120  ating them on a 
+00000c70: 3244 0a73 7572 6661 6365 2028 692e 652e  2D.surface (i.e.
+00000c80: 2c20 6772 6964 6469 6e67 2920 7769 7468  , gridding) with
+00000c90: 2061 2068 696e 7420 6f66 206d 6163 6869   a hint of machi
+00000ca0: 6e65 206c 6561 726e 696e 672e 0a0a 4f75  ne learning...Ou
+00000cb0: 7220 636f 7265 2069 6e74 6572 706f 6c61  r core interpola
+00000cc0: 7469 6f6e 206d 6574 686f 6473 2061 7265  tion methods are
+00000cd0: 2069 6e73 7069 7265 6420 6279 206d 6163   inspired by mac
+00000ce0: 6869 6e65 2d6c 6561 726e 696e 672e 0a41  hine-learning..A
+00000cf0: 7320 7375 6368 2c20 5665 7264 6520 696d  s such, Verde im
+00000d00: 706c 656d 656e 7473 2061 6e20 696e 7465  plements an inte
+00000d10: 7266 6163 6520 7468 6174 2069 7320 7369  rface that is si
+00000d20: 6d69 6c61 7220 746f 2074 6865 2070 6f70  milar to the pop
+00000d30: 756c 6172 0a5b 7363 696b 6974 2d6c 6561  ular.[scikit-lea
+00000d40: 726e 5d28 6874 7470 733a 2f2f 7363 696b  rn](https://scik
+00000d50: 6974 2d6c 6561 726e 2e6f 7267 2f29 206c  it-learn.org/) l
+00000d60: 6962 7261 7279 2e0a 5765 2061 6c73 6f20  ibrary..We also 
+00000d70: 7072 6f76 6964 6520 6f74 6865 7220 616e  provide other an
+00000d80: 616c 7973 6973 206d 6574 686f 6473 2074  alysis methods t
+00000d90: 6861 7420 6172 6520 6f66 7465 6e20 7573  hat are often us
+00000da0: 6564 2069 6e20 636f 6d62 696e 6174 696f  ed in combinatio
+00000db0: 6e20 7769 7468 0a67 7269 6464 696e 672c  n with.gridding,
+00000dc0: 206c 696b 6520 7472 656e 6420 7265 6d6f   like trend remo
+00000dd0: 7661 6c2c 2062 6c6f 636b 6564 2f77 696e  val, blocked/win
+00000de0: 646f 7765 6420 6f70 6572 6174 696f 6e73  dowed operations
+00000df0: 2c20 6372 6f73 732d 7661 6c69 6461 7469  , cross-validati
+00000e00: 6f6e 2c0a 616e 6420 6d6f 7265 210a 0a23  on,.and more!..#
+00000e10: 2320 5072 6f6a 6563 7420 676f 616c 730a  # Project goals.
+00000e20: 0a2a 2050 726f 7669 6465 2061 206d 6163  .* Provide a mac
+00000e30: 6869 6e65 2d6c 6561 726e 696e 6720 696e  hine-learning in
+00000e40: 7370 6972 6564 2069 6e74 6572 6661 6365  spired interface
+00000e50: 2066 6f72 2067 7269 6464 696e 6720 7370   for gridding sp
+00000e60: 6174 6961 6c20 6461 7461 0a2a 2049 6e74  atial data.* Int
+00000e70: 6567 7261 7469 6f6e 2077 6974 6820 7468  egration with th
+00000e80: 6520 5363 6970 7920 7374 6163 6b3a 206e  e Scipy stack: n
+00000e90: 756d 7079 2c20 7061 6e64 6173 2c20 7363  umpy, pandas, sc
+00000ea0: 696b 6974 2d6c 6561 726e 2c20 616e 6420  ikit-learn, and 
+00000eb0: 7861 7272 6179 0a2a 2049 6e63 6c75 6465  xarray.* Include
+00000ec0: 2063 6f6d 6d6f 6e20 7072 6f63 6573 7369   common processi
+00000ed0: 6e67 2061 6e64 2064 6174 6120 7072 6570  ng and data prep
+00000ee0: 6172 6174 696f 6e20 7461 736b 732c 206c  aration tasks, l
+00000ef0: 696b 6520 626c 6f63 6b65 6420 6d65 616e  ike blocked mean
+00000f00: 7320 616e 6420 3244 2074 7265 6e64 730a  s and 2D trends.
+00000f10: 2a20 5375 7070 6f72 7420 666f 7220 6772  * Support for gr
+00000f20: 6964 6469 6e67 2073 6361 6c61 7220 616e  idding scalar an
+00000f30: 6420 7665 6374 6f72 2064 6174 6120 286c  d vector data (l
+00000f40: 696b 6520 7769 6e64 2073 7065 6564 206f  ike wind speed o
+00000f50: 7220 4750 5320 7665 6c6f 6369 7469 6573  r GPS velocities
+00000f60: 290a 2a20 5375 7070 6f72 7420 666f 7220  ).* Support for 
+00000f70: 626f 7468 2043 6172 7465 7369 616e 2061  both Cartesian a
+00000f80: 6e64 2067 656f 6772 6170 6869 6320 636f  nd geographic co
+00000f90: 6f72 6469 6e61 7465 730a 0a23 2320 5072  ordinates..## Pr
+00000fa0: 6f6a 6563 7420 7374 6174 7573 0a0a 2a2a  oject status..**
+00000fb0: 5665 7264 6520 6973 2073 7461 626c 6520  Verde is stable 
+00000fc0: 616e 6420 7265 6164 7920 666f 7220 7573  and ready for us
+00000fd0: 6521 2a2a 0a54 6869 7320 6d65 616e 7320  e!**.This means 
+00000fe0: 7468 6174 2077 6520 6172 6520 6361 7265  that we are care
+00000ff0: 6675 6c20 6162 6f75 7420 696e 7472 6f64  ful about introd
+00001000: 7563 696e 6720 6261 636b 7761 7264 7320  ucing backwards 
+00001010: 696e 636f 6d70 6174 6962 6c65 2063 6861  incompatible cha
+00001020: 6e67 6573 0a61 6e64 2077 696c 6c20 7072  nges.and will pr
+00001030: 6f76 6964 6520 616d 706c 6520 7761 726e  ovide ample warn
+00001040: 696e 6720 7768 656e 2064 6f69 6e67 2073  ing when doing s
+00001050: 6f2e 2055 7067 7261 6469 6e67 206d 696e  o. Upgrading min
+00001060: 6f72 2076 6572 7369 6f6e 7320 6f66 2056  or versions of V
+00001070: 6572 6465 0a73 686f 756c 6420 6e6f 7420  erde.should not 
+00001080: 7265 7175 6972 6520 6d61 6b69 6e67 2063  require making c
+00001090: 6861 6e67 6573 2074 6f20 796f 7572 2063  hanges to your c
+000010a0: 6f64 652e 0a0a 5468 6520 6669 7273 7420  ode...The first 
+000010b0: 6d61 6a6f 7220 7265 6c65 6173 6520 6f66  major release of
+000010c0: 2056 6572 6465 2077 6173 2066 6f63 7573   Verde was focus
+000010d0: 6564 206f 6e20 6d65 6574 696e 6720 6d6f  ed on meeting mo
+000010e0: 7374 206f 6620 7468 6573 6520 696e 6974  st of these init
+000010f0: 6961 6c0a 676f 616c 7320 616e 6420 6573  ial.goals and es
+00001100: 7461 626c 6973 6869 6e67 2074 6865 206c  tablishing the l
+00001110: 6f6f 6b20 616e 6420 6665 656c 206f 6620  ook and feel of 
+00001120: 7468 6520 6c69 6272 6172 792e 0a4c 6174  the library..Lat
+00001130: 6572 2072 656c 6561 7365 7320 7769 6c6c  er releases will
+00001140: 2066 6f63 7573 206f 6e20 6578 7061 6e64   focus on expand
+00001150: 696e 6720 7468 6520 7261 6e67 6520 6f66  ing the range of
+00001160: 2067 7269 6464 6572 7320 6176 6169 6c61   gridders availa
+00001170: 626c 652c 0a6f 7074 696d 697a 696e 6720  ble,.optimizing 
+00001180: 7468 6520 636f 6465 2c20 616e 6420 696d  the code, and im
+00001190: 7072 6f76 696e 6720 616c 676f 7269 7468  proving algorith
+000011a0: 6d73 2073 6f20 7468 6174 206c 6172 6765  ms so that large
+000011b0: 722d 7468 616e 2d6d 656d 6f72 790a 6461  r-than-memory.da
+000011c0: 7461 7365 7473 2063 616e 2061 6c73 6f20  tasets can also 
+000011d0: 6265 2073 7570 706f 7274 6564 2e0a 0a23  be supported...#
+000011e0: 2320 4765 7474 696e 6720 696e 766f 6c76  # Getting involv
+000011f0: 6564 0a0a f09f 97a8 efb8 8f20 2a2a 436f  ed......... **Co
+00001200: 6e74 6163 7420 7573 3a2a 2a0a 4669 6e64  ntact us:**.Find
+00001210: 206f 7574 206d 6f72 6520 6162 6f75 7420   out more about 
+00001220: 686f 7720 746f 2072 6561 6368 2075 7320  how to reach us 
+00001230: 6174 0a5b 6661 7469 616e 646f 2e6f 7267  at.[fatiando.org
+00001240: 2f63 6f6e 7461 6374 5d28 6874 7470 733a  /contact](https:
+00001250: 2f2f 7777 772e 6661 7469 616e 646f 2e6f  //www.fatiando.o
+00001260: 7267 2f63 6f6e 7461 6374 2f29 2e0a 0af0  rg/contact/)....
+00001270: 9f91 a9f0 9f8f bee2 808d f09f 92bb 202a  .............. *
+00001280: 2a43 6f6e 7472 6962 7574 696e 6720 746f  *Contributing to
+00001290: 2070 726f 6a65 6374 2064 6576 656c 6f70   project develop
+000012a0: 6d65 6e74 3a2a 2a0a 506c 6561 7365 2072  ment:**.Please r
+000012b0: 6561 6420 6f75 720a 5b43 6f6e 7472 6962  ead our.[Contrib
+000012c0: 7574 696e 6720 4775 6964 655d 2868 7474  uting Guide](htt
+000012d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000012e0: 6661 7469 616e 646f 2f76 6572 6465 2f62  fatiando/verde/b
+000012f0: 6c6f 622f 6d61 696e 2f43 4f4e 5452 4942  lob/main/CONTRIB
+00001300: 5554 494e 472e 6d64 290a 746f 2073 6565  UTING.md).to see
+00001310: 2068 6f77 2079 6f75 2063 616e 2068 656c   how you can hel
+00001320: 7020 616e 6420 6769 7665 2066 6565 6462  p and give feedb
+00001330: 6163 6b2e 0a0a f09f a791 f09f 8fbe e280  ack.............
+00001340: 8df0 9fa4 9de2 808d f09f a791 f09f 8fbc  ................
+00001350: 202a 2a43 6f64 6520 6f66 2063 6f6e 6475   **Code of condu
+00001360: 6374 3a2a 2a0a 5468 6973 2070 726f 6a65  ct:**.This proje
+00001370: 6374 2069 7320 7265 6c65 6173 6564 2077  ct is released w
+00001380: 6974 6820 610a 5b43 6f64 6520 6f66 2043  ith a.[Code of C
+00001390: 6f6e 6475 6374 5d28 6874 7470 733a 2f2f  onduct](https://
+000013a0: 6769 7468 7562 2e63 6f6d 2f66 6174 6961  github.com/fatia
+000013b0: 6e64 6f2f 636f 6d6d 756e 6974 792f 626c  ndo/community/bl
+000013c0: 6f62 2f6d 6169 6e2f 434f 4445 5f4f 465f  ob/main/CODE_OF_
+000013d0: 434f 4e44 5543 542e 6d64 292e 0a42 7920  CONDUCT.md)..By 
+000013e0: 7061 7274 6963 6970 6174 696e 6720 696e  participating in
+000013f0: 2074 6869 7320 7072 6f6a 6563 7420 796f   this project yo
+00001400: 7520 6167 7265 6520 746f 2061 6269 6465  u agree to abide
+00001410: 2062 7920 6974 7320 7465 726d 732e 0a0a   by its terms...
+00001420: 3e20 2a2a 496d 706f 7374 6572 2073 796e  > **Imposter syn
+00001430: 6472 6f6d 6520 6469 7363 6c61 696d 6572  drome disclaimer
+00001440: 3a2a 2a0a 3e20 5765 2077 616e 7420 796f  :**.> We want yo
+00001450: 7572 2068 656c 702e 202a 2a4e 6f2c 2072  ur help. **No, r
+00001460: 6561 6c6c 792e 2a2a 2054 6865 7265 206d  eally.** There m
+00001470: 6179 2062 6520 6120 6c69 7474 6c65 2076  ay be a little v
+00001480: 6f69 6365 2069 6e73 6964 6520 796f 7572  oice inside your
+00001490: 0a3e 2068 6561 6420 7468 6174 2069 7320  .> head that is 
+000014a0: 7465 6c6c 696e 6720 796f 7520 7468 6174  telling you that
+000014b0: 2079 6f75 2772 6520 6e6f 7420 7265 6164   you're not read
+000014c0: 792c 2074 6861 7420 796f 7520 6172 656e  y, that you aren
+000014d0: 2774 2073 6b69 6c6c 6564 0a3e 2065 6e6f  't skilled.> eno
+000014e0: 7567 6820 746f 2063 6f6e 7472 6962 7574  ugh to contribut
+000014f0: 652e 2057 6520 6173 7375 7265 2079 6f75  e. We assure you
+00001500: 2074 6861 7420 7468 6520 6c69 7474 6c65   that the little
+00001510: 2076 6f69 6365 2069 6e20 796f 7572 2068   voice in your h
+00001520: 6561 6420 6973 0a3e 2077 726f 6e67 2e20  ead is.> wrong. 
+00001530: 4d6f 7374 2069 6d70 6f72 7461 6e74 6c79  Most importantly
+00001540: 2c20 2a2a 7468 6572 6520 6172 6520 6d61  , **there are ma
+00001550: 6e79 2076 616c 7561 626c 6520 7761 7973  ny valuable ways
+00001560: 2074 6f20 636f 6e74 7269 6275 7465 2062   to contribute b
+00001570: 6573 6964 6573 0a3e 2077 7269 7469 6e67  esides.> writing
+00001580: 2063 6f64 652a 2a2e 0a3e 0a3e 202a 5468   code**..>.> *Th
+00001590: 6973 2064 6973 636c 6169 6d65 7220 7761  is disclaimer wa
+000015a0: 7320 6164 6170 7465 6420 6672 6f6d 2074  s adapted from t
+000015b0: 6865 2a0a 3e20 5b4d 6574 5079 2070 726f  he*.> [MetPy pro
+000015c0: 6a65 6374 5d28 6874 7470 733a 2f2f 6769  ject](https://gi
+000015d0: 7468 7562 2e63 6f6d 2f55 6e69 6461 7461  thub.com/Unidata
+000015e0: 2f4d 6574 5079 292e 0a0a 2323 204c 6963  /MetPy)...## Lic
+000015f0: 656e 7365 0a0a 5468 6973 2069 7320 6672  ense..This is fr
+00001600: 6565 2073 6f66 7477 6172 653a 2079 6f75  ee software: you
+00001610: 2063 616e 2072 6564 6973 7472 6962 7574   can redistribut
+00001620: 6520 6974 2061 6e64 2f6f 7220 6d6f 6469  e it and/or modi
+00001630: 6679 2069 7420 756e 6465 7220 7468 6520  fy it under the 
+00001640: 7465 726d 730a 6f66 2074 6865 202a 2a42  terms.of the **B
+00001650: 5344 2033 2d63 6c61 7573 6520 4c69 6365  SD 3-clause Lice
+00001660: 6e73 652a 2a2e 2041 2063 6f70 7920 6f66  nse**. A copy of
+00001670: 2074 6869 7320 6c69 6365 6e73 6520 6973   this license is
+00001680: 2070 726f 7669 6465 6420 696e 0a5b 604c   provided in.[`L
+00001690: 4943 454e 5345 2e74 7874 605d 2868 7474  ICENSE.txt`](htt
+000016a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000016b0: 6661 7469 616e 646f 2f76 6572 6465 2f62  fatiando/verde/b
+000016c0: 6c6f 622f 6d61 696e 2f4c 4943 454e 5345  lob/main/LICENSE
+000016d0: 2e74 7874 292e 0a                        .txt)..
```

### Comparing `verde-1.7.0/verde.egg-info/SOURCES.txt` & `verde-1.8.0/verde.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 AUTHORS.md
 CITATION.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 setup.cfg
-setup.py
 verde/__init__.py
 verde/_version.py
 verde/_version_generated.py
 verde/blockreduce.py
 verde/chain.py
 verde/coordinates.py
 verde/distances.py
 verde/io.py
 verde/mask.py
 verde/model_selection.py
+verde/neighbors.py
 verde/projections.py
 verde/scipygridder.py
 verde/spline.py
 verde/synthetic.py
 verde/trend.py
 verde/utils.py
 verde/vector.py
@@ -46,17 +46,19 @@
 verde/tests/test_coordinates.py
 verde/tests/test_datasets.py
 verde/tests/test_distances.py
 verde/tests/test_io.py
 verde/tests/test_mask.py
 verde/tests/test_minimal.py
 verde/tests/test_model_selection.py
+verde/tests/test_neighbors.py
 verde/tests/test_projections.py
 verde/tests/test_scipy.py
 verde/tests/test_spline.py
+verde/tests/test_synthetic.py
 verde/tests/test_trend.py
 verde/tests/test_utils.py
 verde/tests/test_vector.py
 verde/tests/utils.py
 verde/tests/baseline/test_setup_baja_bathymetry.png
 verde/tests/baseline/test_setup_california_gps.png
 verde/tests/baseline/test_setup_rio_magnetic.png
```


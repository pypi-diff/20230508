# Comparing `tmp/ecmwf_models-0.9.1.tar.gz` & `tmp/ecmwf_models-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".artifacts/dist/ecmwf_models-0.9.1.tar", last modified: Tue May  3 19:48:24 2022, max compression
+gzip compressed data, was "ecmwf_models-0.9.2.tar", last modified: Mon May  8 12:33:44 2023, max compression
```

## Comparing `ecmwf_models-0.9.1.tar` & `ecmwf_models-0.9.2.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10445 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)   822249 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/5x5_cell_partitioning.png
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9763 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/download.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/img2ts.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/img_read.rst
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/docs/ts_read.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/environment/
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/environment/latest.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3040 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/environment/pinned_linux.yml
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14827 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/era5-land_lut.csv
--rw-r--r--   0 runner    (1001) docker     (121)    19764 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/era5_lut.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6793 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/land_definition_files/
--rw-r--r--   0 runner    (1001) docker     (121)   163155 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/land_definition_files/landmask_0.1_0.1.nc
--rw-r--r--   0 runner    (1001) docker     (121)    52477 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/land_definition_files/landmask_0.25_0.25.nc
--rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/era5/reshuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models/erainterim/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/erainterim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10838 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/erainterim/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/erainterim/eraint_lut.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6858 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/erainterim/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/erainterim/reshuffle.py
--rw-r--r--   0 runner    (1001) docker     (121)     4941 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    21535 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/src/ecmwf_models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 19:47:04.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/src/ecmwf_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/tests/tests_era5/
--rw-r--r--   0 runner    (1001) docker     (121)     6591 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/tests_era5/test_era5_download.py
--rw-r--r--   0 runner    (1001) docker     (121)    12701 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/tests_era5/test_era5_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4902 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/tests_era5/test_era5_reshuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 19:48:24.000000 ecmwf_models-0.9.1/tests/tests_eraint/
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/tests_eraint/test_eraint_download.py
--rw-r--r--   0 runner    (1001) docker     (121)    11336 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/tests_eraint/test_eraint_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-05-03 19:41:27.000000 ecmwf_models-0.9.1/tests/tests_eraint/test_eraint_reshuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.848514 ecmwf_models-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.832514 ecmwf_models-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.840514 ecmwf_models-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-08 12:33:44.848514 ecmwf_models-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.840514 ecmwf_models-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   822249 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/5x5_cell_partitioning.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.840514 ecmwf_models-0.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/img2ts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/img_read.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/docs/ts_read.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.840514 ecmwf_models-0.9.2/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/environment/latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/environment/pinned_linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-08 12:33:44.848514 ecmwf_models-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.836514 ecmwf_models-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.844514 ecmwf_models-0.9.2/src/ecmwf_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.844514 ecmwf_models-0.9.2/src/ecmwf_models/era5/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/era5-land_lut.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19764 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/era5_lut.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.844514 ecmwf_models-0.9.2/src/ecmwf_models/era5/land_definition_files/
+-rw-r--r--   0 runner    (1001) docker     (123)   163155 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/land_definition_files/landmask_0.1_0.1.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    52477 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/land_definition_files/landmask_0.25_0.25.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/era5/reshuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.848514 ecmwf_models-0.9.2/src/ecmwf_models/erainterim/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/erainterim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/erainterim/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/erainterim/eraint_lut.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/erainterim/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/erainterim/reshuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21559 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/src/ecmwf_models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.844514 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-08 12:33:44.000000 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-08 12:33:44.000000 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:33:44.000000 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-08 12:33:44.000000 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:32:22.000000 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 12:33:44.000000 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 12:33:44.000000 ecmwf_models-0.9.2/src/ecmwf_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.848514 ecmwf_models-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.848514 ecmwf_models-0.9.2/tests/tests_era5/
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/tests_era5/test_era5_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/tests_era5/test_era5_download_cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/tests_era5/test_era5_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/tests_era5/test_era5_reshuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:44.848514 ecmwf_models-0.9.2/tests/tests_eraint/
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/tests_eraint/test_eraint_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/tests_eraint/test_eraint_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-08 12:28:46.000000 ecmwf_models-0.9.2/tests/tests_eraint/test_eraint_reshuffle.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ecmwf_models-0.9.1/.coveragerc` & `ecmwf_models-0.9.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/.github/workflows/ci.yml` & `ecmwf_models-0.9.2/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,40 +5,47 @@
 # https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Automated Tests
 
 on:
   push:
   pull_request:
+  workflow_dispatch:
   schedule: # only upstream, won't trigger on forks!
     - cron: '0 0 * * *' # daily
 jobs:
   build:
     strategy:
       matrix:
-        os: ["ubuntu-latest", "windows-latest"]
-        python-version: ['3.7', '3.8', '3.9']
-        ymlfile: ['latest.yml']
+        python-version: [ '3.8', '3.9', '3.10' ]
+        os: [ "ubuntu-latest" ]
+        ymlfile: [ "latest.yml" ]
+        include:
+          - os: "windows-latest"
+            python-version: "3.10"
+            ymlfile: "latest.yml"
     name: Py${{ matrix.python-version }}@${{ matrix.os }}|${{ matrix.ymlfile }}
     runs-on: ${{ matrix.os }}
 
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: true
           fetch-depth: 0
           lfs: true
       - name: Checkout LFS objects
         run: git lfs checkout
-      - uses: conda-incubator/setup-miniconda@v2.0.1
+      - uses: conda-incubator/setup-miniconda@v2
         with:
           miniconda-version: "latest"
           auto-update-conda: true
+          channel-priority: flexible
           python-version: ${{ matrix.python-version }}
           environment-file: environment/${{ matrix.ymlfile }}
+          mamba-version: "*"
           activate-environment: ecmwf_models # todo: must match with name in latest.yml
           auto-activate-base: false
       - name: Print Infos
         shell: bash -l {0}
         run: |
           conda info -a
           conda list
```

### Comparing `ecmwf_models-0.9.1/CHANGELOG.rst` & `ecmwf_models-0.9.2/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 =========
 Changelog
 =========
 
-Unreleased
-==========
+Unreleased changes in master branch
+===================================
+
+-
+
+Version 0.9.2
+=============
+
+- Fix issue with too large data requests to download, added command line arg to specify max request size.
+- Pin pynetcf>=0.5.0
+- Add test for downloading ERA5 data directly from CDS (requires CDS API key)
 
 Version 0.9.1
 =============
 
 - Fix returned status code in case of partial data availability.
 
 Version 0.9
```

### Comparing `ecmwf_models-0.9.1/CONTRIBUTING.rst` & `ecmwf_models-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/LICENSE.txt` & `ecmwf_models-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/PKG-INFO` & `ecmwf_models-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmwf_models
-Version: 0.9.1
+Version: 0.9.2
 Summary: Downloading, reading and TS conversion of ECMWF reanalysis data
 Home-page: https://github.com/TUW-GEO/ecmwf_models/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, https://ecmwf-models.readthedocs.io/en/latest/
 Platform: any
@@ -103,9 +103,7 @@
 
 Contribute
 ==========
 
 We are happy if you want to contribute. Please raise an issue explaining what
 is missing or if you find a bug.
 Please take a look at the `developers guide <https://github.com/TUW-GEO/ecmwf_models/blob/master/CONTRIBUTING.rst>`_.
-
-
```

### Comparing `ecmwf_models-0.9.1/README.rst` & `ecmwf_models-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/docs/5x5_cell_partitioning.png` & `ecmwf_models-0.9.2/docs/5x5_cell_partitioning.png`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/docs/Makefile` & `ecmwf_models-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/docs/conf.py` & `ecmwf_models-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/docs/download.rst` & `ecmwf_models-0.9.2/docs/download.rst`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/docs/img2ts.rst` & `ecmwf_models-0.9.2/docs/img2ts.rst`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/docs/img_read.rst` & `ecmwf_models-0.9.2/docs/img_read.rst`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/docs/ts_read.rst` & `ecmwf_models-0.9.2/docs/ts_read.rst`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/setup.cfg` & `ecmwf_models-0.9.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	numpy
 	pandas
 	netcdf4
 	pyresample
 	xarray
-	cdsapi
+	cdsapi>=0.6.1
 	ecmwf-api-client
 	datedown>=0.3
 	pygeobase
 	pygeogrids
 	repurpose
-	pynetcf
+	pynetcf>=0.5.0
 	pygrib
 	configobj
 	requests
 	more_itertools
 python_requires = >=3.6
 
 [options.packages.find]
```

### Comparing `ecmwf_models-0.9.1/setup.py` & `ecmwf_models-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/__init__.py` & `ecmwf_models-0.9.2/src/ecmwf_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/era5/download.py` & `ecmwf_models-0.9.2/src/ecmwf_models/era5/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
-
 """
 Module to download ERA5 from terminal in netcdf and grib format.
 """
+import pandas as pd
 
 from ecmwf_models.utils import (
     load_var_table,
     lookup,
     save_gribs_from_grib,
     save_ncs_from_nc,
     mkdate,
@@ -14,19 +14,19 @@
 )
 import warnings
 import errno
 import argparse
 import sys
 import os
 import logging
-from datetime import datetime, timedelta, time
+from datetime import datetime, time
 import shutil
 import cdsapi
-import calendar
 import multiprocessing
+import numpy as np
 
 
 def default_variables(product="era5"):
     """
     These variables are being downloaded, when None are passed by the user
 
     Parameters
@@ -36,14 +36,97 @@
         Either 'era5' or 'era5-land'.
     """
     lut = load_var_table(name=product)
     defaults = lut.loc[lut["default"] == 1]["dl_name"].values
     return defaults.tolist()
 
 
+def split_array(array, chunk_size):
+    """
+    Split an array into chunks of a given size.
+
+    Parameters
+    ----------
+    array : array-like
+        Array to split into chunks
+    chunk_size : int
+        Size of each chunk
+
+    Returns
+    -------
+    chunks : list
+        List of chunks
+    """
+    chunks = []
+    for i in range(0, len(array), chunk_size):
+        chunks.append(array[i:i + chunk_size])
+    return chunks
+
+
+def split_chunk(timestamps,
+                n_vars,
+                n_hsteps,
+                max_req_size=1000,
+                reduce=False,
+                daily_request=False):
+    """
+    Split the passed time stamps into chunks for a valid request. One chunk
+    can at most hold data for one month or one day, but cannot be larger than
+    the maximum request size.
+
+    Parameters
+    ----------
+    timestamps: pd.DatetimeIndex
+        List of daily timestamps to split into chunks
+    n_vars: int
+        Number of variables in each request.
+    max_req_size: int, optional (default: 1000)
+        Maximum size of a request that the CDS API can handle
+    reduce: bool, optional (default: False)
+        Return only the start and end of each subperiod instead of all
+        time stamps.
+    daily_request: bool, optional (default: False)
+        Only submit daily requests, otherwise monthly requests are allowed
+        (if the max_req_size is not reached).
+
+    Returns
+    -------
+    chunks: list
+        List of start and end dates that contain a chunk that the API can
+        handle.
+    """
+    n = int(max_req_size / n_vars / n_hsteps)
+
+    def yield_chunk():
+        for _, chunk_year in timestamps.groupby(timestamps.year).items():
+            for _, chunk_month in chunk_year.groupby(chunk_year.month).items():
+                if daily_request:
+                    for _, chunk_day in chunk_month.groupby(
+                            chunk_month.day).items():
+                        yield chunk_day
+                else:
+                    yield chunk_month
+
+    # each chunk contains either time stamps for one month, or for less,
+    # if the request of one month would be too large.
+    all_chunks = []
+    for chunk in yield_chunk():
+        if len(chunk) > n:
+            chunks = split_array(chunk, n)
+        else:
+            chunks = np.array([chunk])
+        for chunk in chunks:
+            if reduce:
+                all_chunks.append(np.array([chunk[0], chunk[-1]]))
+            else:
+                all_chunks.append(chunk)
+
+    return all_chunks
+
+
 def download_era5(
     c,
     years,
     months,
     days,
     h_steps,
     variables,
@@ -141,21 +224,22 @@
 def download_and_move(
     target_path,
     startdate,
     enddate,
     product="era5",
     variables=None,
     keep_original=False,
-    h_steps=[0, 6, 12, 18],
+    h_steps=(0, 6, 12, 18),
     grb=False,
     dry_run=False,
     grid=None,
     remap_method="bil",
     cds_kwds={},
     stepsize="month",
+    n_max_request=1000,
 ) -> int:
     """
     Downloads the data from the ECMWF servers and moves them to the target
     path.
     This is done in 30 day increments between start and end date.
 
     The files are then extracted into separate grib files per parameter and
@@ -169,99 +253,105 @@
         first date to download
     enddate: datetime
         last date to download
     product : str, optional (default: ERA5)
         Either ERA5 or ERA5Land
     variables : list, optional (default: None)
         Name of variables to download
-    keep_original: bool
+    keep_original: bool (default: False)
         keep the original downloaded data
-    h_steps: list
+    h_steps: list or tuple
         List of full hours to download data at the selected dates e.g [0, 12]
     grb: bool, optional (default: False)
         Download data as grib files
     dry_run: bool
         Do not download anything, this is just used for testing the functions
-    grid : dict, optional
+    grid : dict, optional (default: None)
         A grid on which to remap the data using CDO. This must be a dictionary
         using CDO's grid description format, e.g.::
 
             grid = {
                 "gridtype": "lonlat",
                 "xsize": 720,
                 "ysize": 360,
                 "xfirst": -179.75,
                 "yfirst": 89.75,
                 "xinc": 0.5,
                 "yinc": -0.5,
             }
 
         Default is to use no regridding.
-    remap_method : str, optional
+    remap_method : str, optional (dafault: 'bil')
         Method to be used for regridding. Available methods are:
         - "bil": bilinear (default)
         - "bic": bicubic
         - "nn": nearest neighbour
         - "dis": distance weighted
         - "con": 1st order conservative remapping
         - "con2": 2nd order conservative remapping
         - "laf": largest area fraction remapping
-    cds_kwds: dict, optional
+    cds_kwds: dict, optional (default: {})
         Additional arguments to be passed to the CDS API retrieve request.
-    stepsize : str, optional
-        Size of steps for requests, can be "month" or "day".
+    n_max_request : int, optional (default: 1000)
+        Maximum size that a request can have to be processed by CDS. At the
+        moment of writing this is 1000 (N_timstamps * N_variables in a request)
+        but as this is a server side settings, it can change.
 
     Returns
     -------
     status_code: int
         0 : Downloaded data ok
         -1 : Error
         -10 : No data available for requested time period
     """
+    h_steps = list(h_steps)
     product = product.lower()
 
     if variables is None:
         variables = default_variables(product=product)
     else:
         # find the dl_names
         variables = lookup(name=product, variables=variables)
         variables = variables["dl_name"].values.tolist()
 
-    curr_start = startdate
-
     if dry_run:
         warnings.warn("Dry run does not create connection to CDS")
         c = None
         cds_status_tracker = None
     else:
         cds_status_tracker = CDSStatusTracker()
         c = cdsapi.Client(
             error_callback=cds_status_tracker.handle_error_function)
 
-    all_status_codes = [] # Since we download month/month or day/day we need to
-                          # collect all the status codes to return a valid
-                          # status code for the whole time period
+    timestamps = pd.DatetimeIndex(
+        np.array([
+            datetime(t.year, t.month, t.day)
+            for t in pd.date_range(startdate, enddate, freq='D')
+        ]))
+
+    daily_request = True if stepsize == "day" else False
+    req_periods = split_chunk(
+        timestamps,
+        n_vars=len(variables),
+        n_hsteps=len(h_steps),
+        max_req_size=n_max_request,
+        reduce=True,
+        daily_request=daily_request)
+
+    # Since we download month/month or day/day we need to
+    # collect all the status codes to return a valid
+    # status code for the whole time period
+    all_status_codes = []
+
     pool = multiprocessing.Pool(1)
-    while curr_start <= enddate:
-        status_code = -1
-        sy, sm, sd = curr_start.year, curr_start.month, curr_start.day
-        y, m = sy, sm
-        if stepsize == "month":
-            sm_days = calendar.monthrange(sy,
-                                          sm)[1]  # days in the current month
-            if (enddate.year == y) and (enddate.month == m):
-                d = enddate.day
-            else:
-                d = sm_days
-        elif stepsize == "day":
-            d = sd
-        else:
-            raise ValueError(f"Invalid stepsize: {stepsize}")
+    for curr_start, curr_end in req_periods:
+        curr_start = pd.to_datetime(curr_start).to_pydatetime()
+        curr_end = pd.to_datetime(curr_end).to_pydatetime()
 
-        curr_end = datetime(y, m, d)
+        status_code = -1
 
         fname = "{start}_{end}.{ext}".format(
             start=curr_start.strftime("%Y%m%d"),
             end=curr_end.strftime("%Y%m%d"),
             ext="grb" if grb else "nc",
         )
 
@@ -272,17 +362,17 @@
 
         finished, i = False, 0
 
         while (not finished) and (i < 5):  # try max 5 times
             try:
                 finished = download_era5(
                     c,
-                    years=[sy],
-                    months=[sm],
-                    days=range(sd, d + 1),
+                    years=[curr_start.year],
+                    months=[curr_start.month],
+                    days=range(curr_start.day, curr_end.day + 1),
                     h_steps=h_steps,
                     variables=variables,
                     grb=grb,
                     product=product,
                     target=dl_file,
                     dry_run=dry_run,
                     cds_kwds=cds_kwds,
@@ -327,15 +417,14 @@
                         remap_method=remap_method,
                         keep_original=keep_original,
                     ),
                 )
 
         all_status_codes.append(status_code)
 
-        curr_start = curr_end + timedelta(days=1)
     pool.close()
     pool.join()
 
     # remove temporary files
     if not keep_original:
         shutil.rmtree(downloaded_data_path)
     if grid is not None:
@@ -419,37 +508,48 @@
               "ERA5-Land+data+documentation"),
     )
     parser.add_argument(
         "-keep",
         "--keep_original",
         type=str2bool,
         default="False",
-        help=("Also keep the originally, temporarily downloaded image stack "
-              "instead of deleting it after extracting single images. "
-              "Default is False."),
+        help=("Also keep the downloaded image stack as retrieved from CDS - "
+              "before slicing it into single images - instead of deleting it "
+              "after extracting all images. "
+              "Pass either True or False. Default is False."),
     )
     parser.add_argument(
         "-grb",
         "--as_grib",
         type=str2bool,
         default="False",
         help=("Download data in grib format instead of netcdf. "
-              "Default is False."),
+              "Pass either True or False. Default is False."),
     )
     parser.add_argument(
         "--h_steps",
         type=int,
         default=[0, 6, 12, 18],
         nargs="+",
         help=("Temporal resolution of downloaded images. "
               "Pass a set of full hours here, like '--h_steps 0 12'. "
               "By default 6H images (starting at 0:00 UTC, i.e. 0 6 12 18) "
               "will be downloaded"),
     )
 
+    parser.add_argument(
+        "--max_request_size",
+        type=int,
+        default=1000,
+        help=("Maximum number of requests that the CDS API allows. "
+              "The default is 1000, but depends on server side settings. "
+              "Server settings may change at some point. Change "
+              "accordingly here in case that 'the request is too large'. "
+              "A smaller number will results in smaller download chunks."))
+
     args = parser.parse_args(args)
 
     print("Downloading {p} {f} files between {s} and {e} into folder {root}"
           .format(
               p=args.product,
               f="grib" if args.as_grib is True else "netcdf",
               s=args.start.isoformat(),
@@ -466,14 +566,16 @@
         startdate=args.start,
         enddate=args.end,
         product=args.product,
         variables=args.variables,
         h_steps=args.h_steps,
         grb=args.as_grib,
         keep_original=args.keep_original,
+        stepsize='month',
+        n_max_request=args.max_request_size,
     )
     return status_code
 
 
 def run():
     status_code = main(sys.argv[1:])
     if status_code == -10:
```

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/era5/era5-land_lut.csv` & `ecmwf_models-0.9.2/src/ecmwf_models/era5/era5-land_lut.csv`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/era5/era5_lut.csv` & `ecmwf_models-0.9.2/src/ecmwf_models/era5/era5_lut.csv`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/era5/interface.py` & `ecmwf_models-0.9.2/src/ecmwf_models/era5/interface.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/era5/land_definition_files/landmask_0.1_0.1.nc` & `ecmwf_models-0.9.2/src/ecmwf_models/era5/land_definition_files/landmask_0.1_0.1.nc`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/era5/land_definition_files/landmask_0.25_0.25.nc` & `ecmwf_models-0.9.2/src/ecmwf_models/era5/land_definition_files/landmask_0.25_0.25.nc`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/era5/reshuffle.py` & `ecmwf_models-0.9.2/src/ecmwf_models/era5/reshuffle.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/erainterim/download.py` & `ecmwf_models-0.9.2/src/ecmwf_models/erainterim/download.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/erainterim/eraint_lut.csv` & `ecmwf_models-0.9.2/src/ecmwf_models/erainterim/eraint_lut.csv`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/erainterim/interface.py` & `ecmwf_models-0.9.2/src/ecmwf_models/erainterim/interface.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/erainterim/reshuffle.py` & `ecmwf_models-0.9.2/src/ecmwf_models/erainterim/reshuffle.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/grid.py` & `ecmwf_models-0.9.2/src/ecmwf_models/grid.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/interface.py` & `ecmwf_models-0.9.2/src/ecmwf_models/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 import warnings
 import os
 from pygeobase.io_base import ImageBase, MultiTemporalImageBase
 from pygeobase.object_base import Image
 import numpy as np
-from datetime import timedelta
+from datetime import timedelta, datetime  # noqa: F401
 
 from pygeogrids.netcdf import load_grid
 from pynetcf.time_series import GriddedNcOrthoMultiTs
 from ecmwf_models.grid import (
     ERA_RegularImgGrid,
     get_grid_resolution,
     ERA_IrregularImgGrid,
```

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models/utils.py` & `ecmwf_models-0.9.2/src/ecmwf_models/utils.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models.egg-info/PKG-INFO` & `ecmwf_models-0.9.2/src/ecmwf_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmwf-models
-Version: 0.9.1
+Version: 0.9.2
 Summary: Downloading, reading and TS conversion of ECMWF reanalysis data
 Home-page: https://github.com/TUW-GEO/ecmwf_models/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, https://ecmwf-models.readthedocs.io/en/latest/
 Platform: any
@@ -103,9 +103,7 @@
 
 Contribute
 ==========
 
 We are happy if you want to contribute. Please raise an issue explaining what
 is missing or if you find a bug.
 Please take a look at the `developers guide <https://github.com/TUW-GEO/ecmwf_models/blob/master/CONTRIBUTING.rst>`_.
-
-
```

### Comparing `ecmwf_models-0.9.1/src/ecmwf_models.egg-info/SOURCES.txt` & `ecmwf_models-0.9.2/src/ecmwf_models.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -53,12 +53,13 @@
 src/ecmwf_models/erainterim/interface.py
 src/ecmwf_models/erainterim/reshuffle.py
 tests/__init__.py
 tests/conftest.py
 tests/test_grid.py
 tests/test_utils.py
 tests/tests_era5/test_era5_download.py
+tests/tests_era5/test_era5_download_cds.py
 tests/tests_era5/test_era5_interface.py
 tests/tests_era5/test_era5_reshuffle.py
 tests/tests_eraint/test_eraint_download.py
 tests/tests_eraint/test_eraint_interface.py
 tests/tests_eraint/test_eraint_reshuffle.py
```

### Comparing `ecmwf_models-0.9.1/tests/test_grid.py` & `ecmwf_models-0.9.2/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/tests/test_utils.py` & `ecmwf_models-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/tests/tests_era5/test_era5_download.py` & `ecmwf_models-0.9.2/tests/tests_era5/test_era5_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import os
 import shutil
 from datetime import datetime
 import numpy as np
 import xarray as xr
 import pytest
 import tempfile
+import time
 
 grid = {
     "gridtype": "lonlat",
     "xsize": 720,
     "ysize": 360,
     "xfirst": -179.75,
     "yfirst": 89.75,
@@ -64,17 +65,18 @@
         os.mkdir(dl_path)
         os.mkdir(os.path.join(dl_path, 'temp_downloaded'))
 
         thefile = os.path.join(
             os.path.dirname(os.path.abspath(__file__)), '..',
             "ecmwf_models-test-data", "download",
             "era5_example_downloaded_raw.nc")
-        shutil.copyfile(
-            thefile,
-            os.path.join(dl_path, 'temp_downloaded', '20100101_20100101.nc'))
+        trgt = os.path.join(dl_path, 'temp_downloaded', '20100101_20100101.nc')
+        shutil.copyfile(thefile, trgt)
+
+        assert os.path.isfile(trgt)
 
         startdate = enddate = datetime(2010, 1, 1)
 
         download_and_move(
             dl_path,
             startdate,
             enddate,
@@ -179,8 +181,8 @@
         for f in os.listdir(os.path.join(dl_path, "2010", "001")):
             ds = xr.open_dataset(os.path.join(dl_path, "2010", "001", f))
             assert dict(ds.dims) == {"lon": 720, "lat": 360}
             assert np.all(np.arange(89.75, -90, -0.5) == ds.lat)
             assert np.all(np.arange(-179.75, 180, 0.5) == ds.lon)
 
 if __name__ == '__main__':
-    test_dry_download_nc_era5()
+    test_dry_download_nc_era5()
```

### Comparing `ecmwf_models-0.9.1/tests/tests_era5/test_era5_interface.py` & `ecmwf_models-0.9.2/tests/tests_era5/test_era5_interface.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/tests/tests_era5/test_era5_reshuffle.py` & `ecmwf_models-0.9.2/tests/tests_era5/test_era5_reshuffle.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/tests/tests_eraint/test_eraint_download.py` & `ecmwf_models-0.9.2/tests/tests_eraint/test_eraint_download.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/tests/tests_eraint/test_eraint_interface.py` & `ecmwf_models-0.9.2/tests/tests_eraint/test_eraint_interface.py`

 * *Files identical despite different names*

### Comparing `ecmwf_models-0.9.1/tests/tests_eraint/test_eraint_reshuffle.py` & `ecmwf_models-0.9.2/tests/tests_eraint/test_eraint_reshuffle.py`

 * *Files identical despite different names*


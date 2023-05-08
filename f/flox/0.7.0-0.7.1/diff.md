# Comparing `tmp/flox-0.7.0.tar.gz` & `tmp/flox-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flox-0.7.0.tar", last modified: Fri May  5 12:51:53 2023, max compression
+gzip compressed data, was "flox-0.7.1.tar", last modified: Mon May  8 17:58:16 2023, max compression
```

## Comparing `flox-0.7.0.tar` & `flox-0.7.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.769970 flox-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 12:51:21.000000 flox-0.7.0/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.757970 flox-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 12:51:21.000000 flox-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.757970 flox-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/ci-additional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-05 12:51:21.000000 flox-0.7.0/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-05 12:51:21.000000 flox-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-05 12:51:21.000000 flox-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-05 12:51:21.000000 flox-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-05 12:51:53.769970 flox-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-05 12:51:21.000000 flox-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.757970 flox-0.7.0/asv_bench/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/asv_bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/README_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/cohorts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-05 12:51:21.000000 flox-0.7.0/asv_bench/benchmarks/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 12:51:21.000000 flox-0.7.0/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-05 12:51:21.000000 flox-0.7.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 12:51:21.000000 flox-0.7.0/ci/minimal-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 12:51:21.000000 flox-0.7.0/ci/no-dask.yml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-05 12:51:21.000000 flox-0.7.0/ci/no-xarray.yml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 12:51:21.000000 flox-0.7.0/ci/upstream-dev-env.yml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 12:51:21.000000 flox-0.7.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-05 12:51:21.000000 flox-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.761970 flox-0.7.0/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)    43022 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/blockwise.png
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/cohorts-month-chunk4.png
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/cohorts-month-chunk5.png
--rw-r--r--   0 runner    (1001) docker     (123)    46006 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/map-reduce.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-blockwise-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-blockwise.svg
--rw-r--r--   0 runner    (1001) docker     (123)   102136 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-cohorts-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60369 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-cohorts.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105406 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62434 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False.svg
--rw-r--r--   0 runner    (1001) docker     (123)   101278 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62159 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True.svg
--rw-r--r--   0 runner    (1001) docker     (123)   177642 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/new-split-apply-combine-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61350 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/split-apply-combine.svg
--rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-05-05 12:51:21.000000 flox-0.7.0/docs/diagrams/split-reduce.png
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-05 12:51:21.000000 flox-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 12:51:21.000000 flox-0.7.0/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/aggregations.md
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/arrays.md
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/engines.md
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/implementation.md
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/docs/source/user-stories/
--rw-r--r--   0 runner    (1001) docker     (123)    74658 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/climatology-hourly.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/climatology.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/custom-aggregations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   395737 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/hourly-climatology.html
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories/overlaps.md
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/user-stories.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-05 12:51:21.000000 flox-0.7.0/docs/source/xarray.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.765970 flox-0.7.0/flox/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 12:51:21.000000 flox-0.7.0/flox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 12:51:53.000000 flox-0.7.0/flox/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-05 12:51:21.000000 flox-0.7.0/flox/aggregate_flox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-05 12:51:21.000000 flox-0.7.0/flox/aggregate_npg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-05-05 12:51:21.000000 flox-0.7.0/flox/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 12:51:21.000000 flox-0.7.0/flox/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    72841 2023-05-05 12:51:21.000000 flox-0.7.0/flox/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:21.000000 flox-0.7.0/flox/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-05 12:51:21.000000 flox-0.7.0/flox/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-05-05 12:51:21.000000 flox-0.7.0/flox/xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-05 12:51:21.000000 flox-0.7.0/flox/xrdtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-05 12:51:21.000000 flox-0.7.0/flox/xrutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.769970 flox-0.7.0/flox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 12:51:53.000000 flox-0.7.0/flox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-05 12:51:21.000000 flox-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 12:51:21.000000 flox-0.7.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:51:53.769970 flox-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 12:51:21.000000 flox-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:51:53.769970 flox-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-05 12:51:21.000000 flox-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 12:51:21.000000 flox-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    46313 2023-05-05 12:51:21.000000 flox-0.7.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-05-05 12:51:21.000000 flox-0.7.0/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 17:57:50.000000 flox-0.7.1/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 17:57:50.000000 flox-0.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/ci-additional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-08 17:57:50.000000 flox-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-08 17:57:50.000000 flox-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-08 17:57:50.000000 flox-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-08 17:58:16.539113 flox-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-08 17:57:50.000000 flox-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/asv_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/asv_bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/README_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-08 17:57:50.000000 flox-0.7.1/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 17:57:50.000000 flox-0.7.1/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 17:57:50.000000 flox-0.7.1/ci/minimal-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 17:57:50.000000 flox-0.7.1/ci/no-dask.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 17:57:50.000000 flox-0.7.1/ci/no-xarray.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-08 17:57:50.000000 flox-0.7.1/ci/upstream-dev-env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-08 17:57:50.000000 flox-0.7.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-08 17:57:50.000000 flox-0.7.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)    43022 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/blockwise.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/cohorts-month-chunk4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/cohorts-month-chunk5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46006 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/map-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-blockwise-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-blockwise.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   102136 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-cohorts-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60369 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-cohorts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105406 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62434 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   101278 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62159 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   177642 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-split-apply-combine-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61350 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/split-apply-combine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/split-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-08 17:57:50.000000 flox-0.7.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 17:57:50.000000 flox-0.7.1/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/aggregations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/arrays.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/engines.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/implementation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/source/user-stories/
+-rw-r--r--   0 runner    (1001) docker     (123)    74658 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/climatology-hourly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/climatology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/custom-aggregations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   395737 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/hourly-climatology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/overlaps.md
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/xarray.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/flox/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 17:57:50.000000 flox-0.7.1/flox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 17:58:16.000000 flox-0.7.1/flox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-08 17:57:50.000000 flox-0.7.1/flox/aggregate_flox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-08 17:57:50.000000 flox-0.7.1/flox/aggregate_npg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-05-08 17:57:50.000000 flox-0.7.1/flox/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 17:57:50.000000 flox-0.7.1/flox/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72861 2023-05-08 17:57:50.000000 flox-0.7.1/flox/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:50.000000 flox-0.7.1/flox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-08 17:57:50.000000 flox-0.7.1/flox/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-05-08 17:57:50.000000 flox-0.7.1/flox/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-08 17:57:50.000000 flox-0.7.1/flox/xrdtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-08 17:57:50.000000 flox-0.7.1/flox/xrutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/flox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-08 17:57:50.000000 flox-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 17:57:50.000000 flox-0.7.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:58:16.539113 flox-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 17:57:50.000000 flox-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-08 17:57:50.000000 flox-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-08 17:57:50.000000 flox-0.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47162 2023-05-08 17:57:50.000000 flox-0.7.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-05-08 17:57:50.000000 flox-0.7.1/tests/test_xarray.py
```

### Comparing `flox-0.7.0/.github/workflows/benchmarks.yml` & `flox-0.7.1/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/.github/workflows/ci-additional.yaml` & `flox-0.7.1/.github/workflows/ci-additional.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/.github/workflows/ci.yaml` & `flox-0.7.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/.github/workflows/pypi.yaml` & `flox-0.7.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/.github/workflows/testpypi-release.yaml` & `flox-0.7.1/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/.github/workflows/upstream-dev-ci.yaml` & `flox-0.7.1/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/.gitignore` & `flox-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/.pre-commit-config.yaml` & `flox-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/LICENSE` & `flox-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/PKG-INFO` & `flox-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.7.0
+Version: 0.7.1
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.7.0/README.md` & `flox-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/asv_bench/asv.conf.json` & `flox-0.7.1/asv_bench/asv.conf.json`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/asv_bench/benchmarks/README_CI.md` & `flox-0.7.1/asv_bench/benchmarks/README_CI.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/asv_bench/benchmarks/__init__.py` & `flox-0.7.1/asv_bench/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/asv_bench/benchmarks/cohorts.py` & `flox-0.7.1/asv_bench/benchmarks/cohorts.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/asv_bench/benchmarks/combine.py` & `flox-0.7.1/asv_bench/benchmarks/combine.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/asv_bench/benchmarks/reduce.py` & `flox-0.7.1/asv_bench/benchmarks/reduce.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/Makefile` & `flox-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/blockwise.png` & `flox-0.7.1/docs/diagrams/blockwise.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/cohorts-month-chunk4.png` & `flox-0.7.1/docs/diagrams/cohorts-month-chunk4.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/cohorts-month-chunk5.png` & `flox-0.7.1/docs/diagrams/cohorts-month-chunk5.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/map-reduce.png` & `flox-0.7.1/docs/diagrams/map-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-blockwise-annotated.svg` & `flox-0.7.1/docs/diagrams/new-blockwise-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-blockwise.svg` & `flox-0.7.1/docs/diagrams/new-blockwise.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-cohorts-annotated.svg` & `flox-0.7.1/docs/diagrams/new-cohorts-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-cohorts.svg` & `flox-0.7.1/docs/diagrams/new-cohorts.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False-annotated.svg` & `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-False.svg` & `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True-annotated.svg` & `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-map-reduce-reindex-True.svg` & `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/new-split-apply-combine-annotated.svg` & `flox-0.7.1/docs/diagrams/new-split-apply-combine-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/split-apply-combine.svg` & `flox-0.7.1/docs/diagrams/split-apply-combine.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/diagrams/split-reduce.png` & `flox-0.7.1/docs/diagrams/split-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/make.bat` & `flox-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/aggregations.md` & `flox-0.7.1/docs/source/aggregations.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/api.rst` & `flox-0.7.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/arrays.md` & `flox-0.7.1/docs/source/arrays.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/conf.py` & `flox-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/engines.md` & `flox-0.7.1/docs/source/engines.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/implementation.md` & `flox-0.7.1/docs/source/implementation.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/index.md` & `flox-0.7.1/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/intro.md` & `flox-0.7.1/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/user-stories/climatology-hourly.ipynb` & `flox-0.7.1/docs/source/user-stories/climatology-hourly.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/user-stories/climatology.ipynb` & `flox-0.7.1/docs/source/user-stories/climatology.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/user-stories/custom-aggregations.ipynb` & `flox-0.7.1/docs/source/user-stories/custom-aggregations.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/user-stories/hourly-climatology.html` & `flox-0.7.1/docs/source/user-stories/hourly-climatology.html`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/user-stories/overlaps.md` & `flox-0.7.1/docs/source/user-stories/overlaps.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/docs/source/xarray.md` & `flox-0.7.1/docs/source/xarray.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox/aggregate_flox.py` & `flox-0.7.1/flox/aggregate_flox.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox/aggregate_npg.py` & `flox-0.7.1/flox/aggregate_npg.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox/aggregations.py` & `flox-0.7.1/flox/aggregations.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox/core.py` & `flox-0.7.1/flox/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1871,20 +1871,14 @@
     if axis is None:
         axis_ = tuple(array.ndim + np.arange(-by_.ndim, 0))
     else:
         # TODO: How come this function doesn't exist according to mypy?
         axis_ = np.core.numeric.normalize_axis_tuple(axis, array.ndim)  # type: ignore
     nax = len(axis_)
 
-    if method in ["blockwise", "cohorts"] and nax != by_.ndim:
-        raise NotImplementedError(
-            "Must reduce along all dimensions of `by` when method != 'map-reduce'."
-            f"Received method={method!r}"
-        )
-
     # TODO: make sure expected_groups is unique
     if nax == 1 and by_.ndim > 1 and expected_groups is None:
         if not any_by_dask:
             expected_groups = _get_expected_groups(by_, sort)
         else:
             # When we reduce along all axes, we are guaranteed to see all
             # groups in the final combine stage, so everything works.
@@ -1945,14 +1939,20 @@
 
         if agg.chunk[0] is None and method != "blockwise":
             raise NotImplementedError(
                 f"Aggregation {agg.name!r} is only implemented for dask arrays when method='blockwise'."
                 f"\n\n Received: {func}"
             )
 
+        if method in ["blockwise", "cohorts"] and nax != by_.ndim:
+            raise NotImplementedError(
+                "Must reduce along all dimensions of `by` when method != 'map-reduce'."
+                f"Received method={method!r}"
+            )
+
         # TODO: just do this in dask_groupby_agg
         # we always need some fill_value (see above) so choose the default if needed
         if kwargs["fill_value"] is None:
             kwargs["fill_value"] = agg.fill_value[agg.name]
 
         partial_agg = partial(dask_groupby_agg, **kwargs)
```

### Comparing `flox-0.7.0/flox/visualize.py` & `flox-0.7.1/flox/visualize.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox/xarray.py` & `flox-0.7.1/flox/xarray.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox/xrdtypes.py` & `flox-0.7.1/flox/xrdtypes.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox/xrutils.py` & `flox-0.7.1/flox/xrutils.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/flox.egg-info/PKG-INFO` & `flox-0.7.1/flox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.7.0
+Version: 0.7.1
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.7.0/flox.egg-info/SOURCES.txt` & `flox-0.7.1/flox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/pyproject.toml` & `flox-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/tests/__init__.py` & `flox-0.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.0/tests/test_core.py` & `flox-0.7.1/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1343,7 +1343,41 @@
 @pytest.mark.parametrize("sort", [True, False])
 def test_expected_index_conversion_passthrough_range_index(sort):
     index = pd.RangeIndex(100)
     actual = _convert_expected_groups_to_index(
         expected_groups=(index,), isbin=(False,), sort=(sort,)
     )
     assert actual[0] is index
+
+
+def test_method_check_numpy():
+    bins = [-2, -1, 0, 1, 2]
+    field = np.ones((5, 3))
+    by = np.array([[-1.5, -1.5, 0.5, 1.5, 1.5] * 3]).reshape(5, 3)
+    actual, _ = groupby_reduce(
+        field,
+        by,
+        expected_groups=pd.IntervalIndex.from_breaks(bins),
+        func="count",
+        method="cohorts",
+        fill_value=np.nan,
+    )
+    expected = np.array([6, np.nan, 3, 6])
+    assert_equal(actual, expected)
+
+    actual, _ = groupby_reduce(
+        field,
+        by,
+        expected_groups=pd.IntervalIndex.from_breaks(bins),
+        func="count",
+        fill_value=np.nan,
+        method="cohorts",
+        axis=0,
+    )
+    expected = np.array(
+        [
+            [2.0, np.nan, 1.0, 2.0],
+            [2.0, np.nan, 1.0, 2.0],
+            [2.0, np.nan, 1.0, 2.0],
+        ]
+    )
+    assert_equal(actual, expected)
```

### Comparing `flox-0.7.0/tests/test_xarray.py` & `flox-0.7.1/tests/test_xarray.py`

 * *Files identical despite different names*


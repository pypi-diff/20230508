# Comparing `tmp/dvc-data-0.8.0.tar.gz` & `tmp/dvc-data-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-data-0.8.0.tar", last modified: Wed Sep 14 08:47:24 2022, max compression
+gzip compressed data, was "dvc-data-0.9.0.tar", last modified: Fri Sep 16 14:24:09 2022, max compression
```

## Comparing `dvc-data-0.8.0.tar` & `dvc-data-0.9.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.409344 dvc-data-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.405344 dvc-data-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.405344 dvc-data-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-14 08:47:00.000000 dvc-data-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-09-14 08:47:00.000000 dvc-data-0.8.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-09-14 08:47:00.000000 dvc-data-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-09-14 08:47:00.000000 dvc-data-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-09-14 08:47:24.409344 dvc-data-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-09-14 08:47:00.000000 dvc-data-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-09-14 08:47:00.000000 dvc-data-0.8.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-09-14 08:47:00.000000 dvc-data-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-09-14 08:47:24.409344 dvc-data-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.401344 dvc-data-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.405344 dvc-data-0.8.0/src/dvc_data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18192 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.405344 dvc-data-0.8.0/src/dvc_data/hashfile/
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/_ignore.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.405344 dvc-data-0.8.0/src/dvc_data/hashfile/db/
--rw-r--r--   0 runner    (1001) docker     (121)     5439 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3405 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/db/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/db/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/db/reference.py
--rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/gc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4736 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/hash_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/istextfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/obj.py
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/state.py
--rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/transfer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9223 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/hashfile/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10301 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/index.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-09-14 08:47:00.000000 dvc-data-0.8.0/src/dvc_data/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.405344 dvc-data-0.8.0/src/dvc_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-09-14 08:47:24.000000 dvc-data-0.8.0/src/dvc_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-09-14 08:47:24.000000 dvc-data-0.8.0/src/dvc_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 08:47:24.000000 dvc-data-0.8.0/src/dvc_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-14 08:47:24.000000 dvc-data-0.8.0/src/dvc_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 08:47:24.000000 dvc-data-0.8.0/src/dvc_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-14 08:47:24.000000 dvc-data-0.8.0/src/dvc_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-14 08:47:24.000000 dvc-data-0.8.0/src/dvc_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.409344 dvc-data-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.409344 dvc-data-0.8.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/benchmarks/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:24.409344 dvc-data-0.8.0/tests/hashfile/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_hash_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_istextfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/hashfile/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/test_dvc_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-09-14 08:47:00.000000 dvc-data-0.8.0/tests/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.971712 dvc-data-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.963712 dvc-data-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.967712 dvc-data-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-16 14:23:50.000000 dvc-data-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-09-16 14:23:50.000000 dvc-data-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-09-16 14:23:50.000000 dvc-data-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-09-16 14:23:50.000000 dvc-data-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-09-16 14:24:09.971712 dvc-data-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-09-16 14:23:50.000000 dvc-data-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-09-16 14:23:50.000000 dvc-data-0.9.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-09-16 14:23:50.000000 dvc-data-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-09-16 14:24:09.971712 dvc-data-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.963712 dvc-data-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.967712 dvc-data-0.9.0/src/dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18192 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.967712 dvc-data-0.9.0/src/dvc_data/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.967712 dvc-data-0.9.0/src/dvc_data/hashfile/db/
+-rw-r--r--   0 runner    (1001) docker     (121)     5439 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3405 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/db/index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/db/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/db/reference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/gc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4736 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/hash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/hash_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/obj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9223 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/hashfile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10301 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/index.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-09-16 14:23:50.000000 dvc-data-0.9.0/src/dvc_data/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.967712 dvc-data-0.9.0/src/dvc_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-09-16 14:24:09.000000 dvc-data-0.9.0/src/dvc_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-09-16 14:24:09.000000 dvc-data-0.9.0/src/dvc_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 14:24:09.000000 dvc-data-0.9.0/src/dvc_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-16 14:24:09.000000 dvc-data-0.9.0/src/dvc_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 14:24:09.000000 dvc-data-0.9.0/src/dvc_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-16 14:24:09.000000 dvc-data-0.9.0/src/dvc_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-16 14:24:09.000000 dvc-data-0.9.0/src/dvc_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.967712 dvc-data-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.967712 dvc-data-0.9.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/benchmarks/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 14:24:09.971712 dvc-data-0.9.0/tests/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_hash_stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/hashfile/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/test_dvc_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-09-16 14:23:50.000000 dvc-data-0.9.0/tests/test_index.py
```

### Comparing `dvc-data-0.8.0/.cruft.json` & `dvc-data-0.9.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/.github/dependabot.yml` & `dvc-data-0.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/.github/workflows/benchmark.yml` & `dvc-data-0.9.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/.github/workflows/release.yml` & `dvc-data-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/.github/workflows/tests.yml` & `dvc-data-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/.gitignore` & `dvc-data-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/.pre-commit-config.yaml` & `dvc-data-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/CODE_OF_CONDUCT.rst` & `dvc-data-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/CONTRIBUTING.rst` & `dvc-data-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/LICENSE` & `dvc-data-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/PKG-INFO` & `dvc-data-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 0.8.0
+Version: 0.9.0
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-0.8.0/README.rst` & `dvc-data-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/noxfile.py` & `dvc-data-0.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/pyproject.toml` & `dvc-data-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/setup.cfg` & `dvc-data-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	=src
 packages = find:
 install_requires = 
 	funcy>=1.14
 	dictdiffer>=0.8.1
 	pygtrie>=2.3.2
 	shortuuid>=0.5.0
-	dvc-objects==0.2.2
+	dvc-objects==0.3.2
 	diskcache>=5.2.1
 	nanotime>=0.5.2
 	attrs>=21.3.0
 
 [options.extras_require]
 cli = 
 	typer[all]>=0.6
```

### Comparing `dvc-data-0.8.0/src/dvc_data/cli.py` & `dvc-data-0.9.0/src/dvc_data/cli.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/fs.py` & `dvc-data-0.9.0/src/dvc_data/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/__init__.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/_progress.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/build.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/cache.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/checkout.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/db/__init__.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/db/index.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/db/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/db/local.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/db/local.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/db/reference.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/db/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/diff.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/gc.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/hash.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/hash_info.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/hash_info.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/istextfile.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/meta.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/meta.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/state.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/state.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/status.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/status.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/transfer.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/transfer.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/tree.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/hashfile/utils.py` & `dvc-data-0.9.0/src/dvc_data/hashfile/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/index.py` & `dvc-data-0.9.0/src/dvc_data/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data/repo.py` & `dvc-data-0.9.0/src/dvc_data/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data.egg-info/PKG-INFO` & `dvc-data-0.9.0/src/dvc_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 0.8.0
+Version: 0.9.0
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-0.8.0/src/dvc_data.egg-info/SOURCES.txt` & `dvc-data-0.9.0/src/dvc_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/src/dvc_data.egg-info/requires.txt` & `dvc-data-0.9.0/src/dvc_data.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 funcy>=1.14
 dictdiffer>=0.8.1
 pygtrie>=2.3.2
 shortuuid>=0.5.0
-dvc-objects==0.2.2
+dvc-objects==0.3.2
 diskcache>=5.2.1
 nanotime>=0.5.2
 attrs>=21.3.0
 
 [all]
 typer[all]>=0.6
 rich<13.0.0,>=10.11.0
```

### Comparing `dvc-data-0.8.0/tests/benchmarks/test_checkout.py` & `dvc-data-0.9.0/tests/benchmarks/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/hashfile/test_cache.py` & `dvc-data-0.9.0/tests/hashfile/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/hashfile/test_diff.py` & `dvc-data-0.9.0/tests/hashfile/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/hashfile/test_hash.py` & `dvc-data-0.9.0/tests/hashfile/test_hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/hashfile/test_hash_stream.py` & `dvc-data-0.9.0/tests/hashfile/test_hash_stream.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/hashfile/test_istextfile.py` & `dvc-data-0.9.0/tests/hashfile/test_istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/hashfile/test_tree.py` & `dvc-data-0.9.0/tests/hashfile/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/hashfile/test_utils.py` & `dvc-data-0.9.0/tests/hashfile/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-0.8.0/tests/test_index.py` & `dvc-data-0.9.0/tests/test_index.py`

 * *Files identical despite different names*


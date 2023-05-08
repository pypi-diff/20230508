# Comparing `tmp/pycollimator-1.3.884.post59.tar.gz` & `tmp/pycollimator-1.3.884.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/collimator/collimator/src/lib/pycollimator/dist/.tmp-aiet4dk4/pycollimator-1.3.884.post59.tar", last modified: Mon Dec 19 03:50:19 2022, max compression
+gzip compressed data, was "/home/runner/work/collimator/collimator/src/lib/pycollimator/dist/.tmp-9ig9swxr/pycollimator-1.3.884.post7.tar", last modified: Mon Dec 12 03:50:11 2022, max compression
```

## Comparing `pycollimator-1.3.884.post59.tar` & `pycollimator-1.3.884.post7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/BUILD.bazel
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      477 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/bootstrap.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      524 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/ci_checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/env.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/examples/BUILD.bazel
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/examples/run_simulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      986 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/examples/run_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/examples/upload_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      674 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/fetch-test-token.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/pycollimator/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10322 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/diagrams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/simulation_hashed_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pycollimator/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/pycollimator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-19 03:50:18.000000 pycollimator-1.3.884.post59/pycollimator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/pycollimator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 03:50:18.000000 pycollimator-1.3.884.post59/pycollimator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-19 03:50:18.000000 pycollimator-1.3.884.post59/pycollimator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-19 03:50:18.000000 pycollimator-1.3.884.post59/pycollimator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    93798 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/config-dev.json
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/config-local.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 03:50:19.000000 pycollimator-1.3.884.post59/tests/fixtures/backups/
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/fixtures/backups/db-backup.json
--rw-r--r--   0 runner    (1001) docker     (123)   356793 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/fixtures/stop.png
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/fixtures/test_001.json
--rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/fixtures/test_002.json
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/fixtures/test_003.json
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/fixtures/test_004.json
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/fixtures/test_005.json
--rw-r--r--   0 runner    (1001) docker     (123)      760 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/test_simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-19 03:49:57.000000 pycollimator-1.3.884.post59/tests/test_upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/BUILD.bazel
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      477 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/bootstrap.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      524 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/ci_checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/env.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/examples/BUILD.bazel
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/examples/run_simulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/examples/run_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/examples/upload_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      674 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/fetch-test-token.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/pycollimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17344 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/simulation_hashed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pycollimator/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/pycollimator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/pycollimator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/pycollimator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/pycollimator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/pycollimator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/pycollimator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    93798 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/config-dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/config-local.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 03:50:11.000000 pycollimator-1.3.884.post7/tests/fixtures/backups/
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/fixtures/backups/db-backup.json
+-rw-r--r--   0 runner    (1001) docker     (123)   356793 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/fixtures/stop.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/fixtures/test_001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/fixtures/test_002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/fixtures/test_003.json
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/fixtures/test_004.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/fixtures/test_005.json
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/test_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-12 03:49:50.000000 pycollimator-1.3.884.post7/tests/test_upload_file.py
```

### Comparing `pycollimator-1.3.884.post59/BUILD.bazel` & `pycollimator-1.3.884.post7/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/ci_checks.sh` & `pycollimator-1.3.884.post7/ci_checks.sh`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/examples/run_simulation.ipynb` & `pycollimator-1.3.884.post7/examples/run_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/examples/run_simulation.py` & `pycollimator-1.3.884.post7/examples/run_simulation.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/examples/upload_file.py` & `pycollimator-1.3.884.post7/examples/upload_file.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/fetch-test-token.sh` & `pycollimator-1.3.884.post7/fetch-test-token.sh`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/__init__.py` & `pycollimator-1.3.884.post7/pycollimator/__init__.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/api.py` & `pycollimator-1.3.884.post7/pycollimator/api.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/diagrams.py` & `pycollimator-1.3.884.post7/pycollimator/diagrams.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/error.py` & `pycollimator-1.3.884.post7/pycollimator/error.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/global_variables.py` & `pycollimator-1.3.884.post7/pycollimator/global_variables.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/log.py` & `pycollimator-1.3.884.post7/pycollimator/log.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/models.py` & `pycollimator-1.3.884.post7/pycollimator/models.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/projects.py` & `pycollimator-1.3.884.post7/pycollimator/projects.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/results.py` & `pycollimator-1.3.884.post7/pycollimator/results.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/simulation_hashed_file.py` & `pycollimator-1.3.884.post7/pycollimator/simulation_hashed_file.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/simulations.py` & `pycollimator-1.3.884.post7/pycollimator/simulations.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator/widgets.py` & `pycollimator-1.3.884.post7/pycollimator/widgets.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/pycollimator.egg-info/SOURCES.txt` & `pycollimator-1.3.884.post7/pycollimator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/requirements-lock.txt` & `pycollimator-1.3.884.post7/requirements-lock.txt`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/setup.py` & `pycollimator-1.3.884.post7/setup.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/__init__.py` & `pycollimator-1.3.884.post7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/fixtures/backups/db-backup.json` & `pycollimator-1.3.884.post7/tests/fixtures/backups/db-backup.json`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/fixtures/stop.png` & `pycollimator-1.3.884.post7/tests/fixtures/stop.png`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/fixtures/test_001.json` & `pycollimator-1.3.884.post7/tests/fixtures/test_001.json`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/fixtures/test_002.json` & `pycollimator-1.3.884.post7/tests/fixtures/test_002.json`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/fixtures/test_003.json` & `pycollimator-1.3.884.post7/tests/fixtures/test_003.json`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/test_auth.py` & `pycollimator-1.3.884.post7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/test_datasource.py` & `pycollimator-1.3.884.post7/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/test_projects.py` & `pycollimator-1.3.884.post7/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/test_results.py` & `pycollimator-1.3.884.post7/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/test_simulations.py` & `pycollimator-1.3.884.post7/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `pycollimator-1.3.884.post59/tests/test_upload_file.py` & `pycollimator-1.3.884.post7/tests/test_upload_file.py`

 * *Files identical despite different names*


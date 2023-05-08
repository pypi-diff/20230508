# Comparing `tmp/TPOT2-0.1.1a0.tar.gz` & `tmp/TPOT2-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPOT2-0.1.1a0.tar", last modified: Thu Apr 27 23:14:51 2023, max compression
+gzip compressed data, was "TPOT2-0.1.2a0.tar", last modified: Mon May  8 19:55:46 2023, max compression
```

## Comparing `TPOT2-0.1.1a0.tar` & `TPOT2-0.1.2a0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.729613 TPOT2-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 23:14:51.729613 TPOT2-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.713613 TPOT2-0.1.1a0/TPOT2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 23:14:51.000000 TPOT2-0.1.1a0/TPOT2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-27 23:14:51.000000 TPOT2-0.1.1a0/TPOT2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:14:51.000000 TPOT2-0.1.1a0/TPOT2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 23:14:51.000000 TPOT2-0.1.1a0/TPOT2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 23:14:51.000000 TPOT2-0.1.1a0/TPOT2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 23:14:51.000000 TPOT2-0.1.1a0/TPOT2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:14:51.000000 TPOT2-0.1.1a0/TPOT2.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-27 23:14:51.729613 TPOT2-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.713613 TPOT2-0.1.1a0/tpot2/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    42425 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/base_evolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.717613 TPOT2-0.1.1a0/tpot2/builtin_modules/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/arithmetictransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/cat_impute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/cat_one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/feature_encoding_frequency_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/feature_set_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/feature_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/genetic_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/numeric_impute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18836 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/passthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/builtin_modules/zero_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.721613 TPOT2-0.1.1a0/tpot2/config/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/all_single_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/autoqtl_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/hyperparametersuggestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/mdr_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/regressors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/special_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/config/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/estimator_objective_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.721613 TPOT2-0.1.1a0/tpot2/evolutionary_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/evolutionary_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/graphsklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/individual.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/logbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/parent_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/population.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.721613 TPOT2-0.1.1a0/tpot2/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.725613 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.725613 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/graph_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/graph_utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49289 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/individual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.725613 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.725613 TPOT2-0.1.1a0/tpot2/representations/subset_selector/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/subset_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/representations/subset_selector/subsetselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.725613 TPOT2-0.1.1a0/tpot2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/test_built_in_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/test_ea.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/test_full_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tests/test_population.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.729613 TPOT2-0.1.1a0/tpot2/tpot_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tpot_estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55260 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tpot_estimator/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:51.729613 TPOT2-0.1.1a0/tpot2/tpot_estimator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tpot_estimator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-27 23:14:40.000000 TPOT2-0.1.1a0/tpot2/tpot_estimator/templates/tpottemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.335537 TPOT2-0.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-08 19:55:46.335537 TPOT2-0.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.319537 TPOT2-0.1.2a0/TPOT2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-08 19:55:46.000000 TPOT2-0.1.2a0/TPOT2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-08 19:55:46.000000 TPOT2-0.1.2a0/TPOT2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:55:46.000000 TPOT2-0.1.2a0/TPOT2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 19:55:46.000000 TPOT2-0.1.2a0/TPOT2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-08 19:55:46.000000 TPOT2-0.1.2a0/TPOT2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 19:55:46.000000 TPOT2-0.1.2a0/TPOT2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:55:46.000000 TPOT2-0.1.2a0/TPOT2.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-08 19:55:46.335537 TPOT2-0.1.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.323537 TPOT2-0.1.2a0/tpot2/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42274 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/base_evolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.327537 TPOT2-0.1.2a0/tpot2/builtin_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/arithmetictransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/column_one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/feature_encoding_frequency_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/feature_set_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/feature_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/genetic_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18836 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/builtin_modules/zero_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.327537 TPOT2-0.1.2a0/tpot2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/all_single_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/autoqtl_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/hyperparametersuggestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/mdr_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/regressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/special_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/config/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/estimator_objective_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.327537 TPOT2-0.1.2a0/tpot2/evolutionary_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/evolutionary_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/graphsklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/logbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/parent_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.327537 TPOT2-0.1.2a0/tpot2/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.327537 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.331537 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/graph_utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46004 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.331537 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.331537 TPOT2-0.1.2a0/tpot2/representations/subset_selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/subset_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/representations/subset_selector/subsetselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.331537 TPOT2-0.1.2a0/tpot2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/test_built_in_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/test_ea.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/test_full_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tests/test_population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.335537 TPOT2-0.1.2a0/tpot2/tpot_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tpot_estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62848 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tpot_estimator/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:46.335537 TPOT2-0.1.2a0/tpot2/tpot_estimator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tpot_estimator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/tpot_estimator/templates/tpottemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-08 19:55:33.000000 TPOT2-0.1.2a0/tpot2/utils.py
```

### Comparing `TPOT2-0.1.1a0/PKG-INFO` & `TPOT2-0.1.2a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TPOT2
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: Tree-based Pipeline Optimization Tool
 Home-page: https://github.com/EpistasisLab/tpot2
 Author: Pedro Ribeiro
 License: GNU/LGPLv3
 Keywords: pipeline optimization,hyperparameter optimization,data science,machine learning,genetic programming,evolutionary computation
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: skrebate
 Provides-Extra: mdr
+License-File: LICENSE
 
 
 A Python tool that automatically creates and optimizes machine learning pipelines using genetic programming.
```

### Comparing `TPOT2-0.1.1a0/README.md` & `TPOT2-0.1.2a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # TPOT2 ALPHA
 
 ![Tests](https://github.com/EpistasisLab/tpot2/actions/workflows/tests.yml/badge.svg)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/tpot2?label=pypi%20downloads)](https://pypi.org/project/TPOT2)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/tpot2?label=conda%20downloads)](https://anaconda.org/conda-forge/tpot2)
 
 TPOT2 is a rewrite of TPOT with some additional functionality. Notably, we added support for graph-based pipelines and additional parameters to better specify the desired search space. 
 TPOT2 is currently in Alpha. This means that there will likely be some backwards incompatible changes to the API as we develop. Some implemented features may be buggy. There is a list of known issues written at the bottom of this README. Some features have placeholder names or are listed as "Experimental" in the doc string. These are features that may not be fully implemented and may or may work with all other features.
 
 If you are interested in using the current stable release of TPOT, you can do that here: [https://github.com/EpistasisLab/tpot/](https://github.com/EpistasisLab/tpot/). 
 
 
 ## License
 
-Please see the [repository license](https://github.com/EpistasisLab/tpot/blob/master/LICENSE) for the licensing and usage information for TPOT2.
+Please see the [repository license](https://github.com/EpistasisLab/tpot2/blob/main/LICENSE) for the licensing and usage information for TPOT2.
 Generally, we have licensed TPOT2 to make it as widely usable as possible.
 
 
 ## Installation
 
 TPOT2 requires a working installation of Python.
 
@@ -74,29 +76,33 @@
 
 #### 2
 
 When designing custom objective functions, avoid the use of global variables.
 
 Don't Do:
 ```
-global_a = 10
-def foo_objective(est, X, y):
-    return my_scorer(est, X, y, a=global_a)
+global_X = [[1,2],[4,5]]
+global_y = [0,1]
+def foo(est):
+    return my_scorer(est, X=global_X, y=global_y)
+
 ```
 
 Instead use a partial
 
-
 ```
 from functools import partial
 
-def foo_scorer(est, X, y, a):
-    return my_scorer(est, X, y, a=a)
+def foo_scorer(est, X, y):
+    return my_scorer(est, X, y)
 
-final_scorer = partial(foo_scorer, a=10)
+if __name__=='__main__':
+    X = [[1,2],[4,5]]
+    y = [0,1]
+    final_scorer = partial(foo_scorer, X=X, y=y)
 ```
 
 Similarly when using lambda functions.
 
 Dont Do:
 
 ```
```

### Comparing `TPOT2-0.1.1a0/TPOT2.egg-info/PKG-INFO` & `TPOT2-0.1.2a0/TPOT2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TPOT2
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: Tree-based Pipeline Optimization Tool
 Home-page: https://github.com/EpistasisLab/tpot2
 Author: Pedro Ribeiro
 License: GNU/LGPLv3
 Keywords: pipeline optimization,hyperparameter optimization,data science,machine learning,genetic programming,evolutionary computation
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: skrebate
 Provides-Extra: mdr
+License-File: LICENSE
 
 
 A Python tool that automatically creates and optimizes machine learning pipelines using genetic programming.
```

### Comparing `TPOT2-0.1.1a0/TPOT2.egg-info/SOURCES.txt` & `TPOT2-0.1.2a0/TPOT2.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 TPOT2.egg-info/PKG-INFO
 TPOT2.egg-info/SOURCES.txt
 TPOT2.egg-info/dependency_links.txt
@@ -15,23 +16,23 @@
 tpot2/estimator_objective_functions.py
 tpot2/graphsklearn.py
 tpot2/individual.py
 tpot2/logbook.py
 tpot2/objectives.py
 tpot2/parent_selectors.py
 tpot2/population.py
+tpot2/utils.py
 tpot2/builtin_modules/__init__.py
 tpot2/builtin_modules/arithmetictransformer.py
-tpot2/builtin_modules/cat_impute.py
-tpot2/builtin_modules/cat_one_hot_encoder.py
+tpot2/builtin_modules/column_one_hot_encoder.py
 tpot2/builtin_modules/feature_encoding_frequency_selector.py
 tpot2/builtin_modules/feature_set_selector.py
 tpot2/builtin_modules/feature_transformers.py
 tpot2/builtin_modules/genetic_encoders.py
-tpot2/builtin_modules/numeric_impute.py
+tpot2/builtin_modules/imputer.py
 tpot2/builtin_modules/one_hot_encoder.py
 tpot2/builtin_modules/passthrough.py
 tpot2/builtin_modules/zero_count.py
 tpot2/config/__init__.py
 tpot2/config/all_single_modules.py
 tpot2/config/autoqtl_builtins.py
 tpot2/config/classifiers.py
```

### Comparing `TPOT2-0.1.1a0/setup.py` & `TPOT2-0.1.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/base_evolver.py` & `TPOT2-0.1.2a0/tpot2/base_evolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import statistics
 from tqdm.dask import TqdmCallback
 import distributed
 from dask.distributed import Client
 from dask.distributed import LocalCluster
 from tpot2.parent_selectors import survival_select_NSGA2, TournamentSelection_Dominated
 import math
+from tpot2.utils import get_thresholds, beta_interpolation, remove_items, equalize_list, update_pareto_frontier
 
 class BaseEvolver():
     def __init__(   self, 
                     individual_generator ,
                     
                     objective_functions,
                     objective_function_weights,
@@ -265,24 +266,24 @@
         self.verbose  = verbose  
         self.callback = callback 
         self.generations = generations 
         self.n_jobs = n_jobs
 
 
         
-        if max_time_seconds  is None:
+        if max_time_seconds is None:
             self.max_time_seconds = float("inf")
         else:
             self.max_time_seconds = max_time_seconds  
         
         #functools requires none for infinite time, doesn't support inf
         if max_eval_time_seconds is not None and math.isinf(max_eval_time_seconds ):
-            self.max_eval_time_seconds = max_eval_time_seconds 
-        else:
             self.max_eval_time_seconds = None
+        else:
+            self.max_eval_time_seconds = max_eval_time_seconds
 
         
         self.n_initial_optimizations  = n_initial_optimizations  
         self.optimization_objective  = optimization_objective  
         self.max_optimize_time_seconds = max_optimize_time_seconds 
         self.optimization_steps = optimization_steps 
         
@@ -410,19 +411,21 @@
         if self.n_initial_optimizations > 0:
             self.optimize_population()
         if generations is None:
             generations = self.generations
 
         start_time = time.time() 
         
-        last_save_time = time.time()
-        
         generations_without_improvement = np.array([0 for _ in range(len(self.objective_function_weights))])
         best_scores = [-np.inf for _ in range(len(self.objective_function_weights))]
 
+
+        self.scheduled_timeout_time = time.time() + self.max_time_seconds
+
+
         try: 
             for gen in tnrange(generations,desc="Generation", disable=self.verbose<1):
                 
                 # Generation 0 is the initial population
                 if self.generation == 0:
                     if self.population_file is not None:
                         pickle.dump(self.population, open(self.population_file, "wb"))
@@ -442,14 +445,17 @@
 
                     self.generation += 1
                 # Generation 1 is the first generation after the initial population
                 else:
                     if time.time() - start_time > self.max_time_seconds:
                         break
                     self.step()
+                    
+                #update the pareto frontier
+                self.population.evaluated_individuals = update_pareto_frontier(self.population.evaluated_individuals, self.objective_names, self.objective_function_weights,self.generation-1)
 
                 if self.verbose >= 3:  
                     sign = np.sign(self.objective_function_weights)
                     valid_df = self.population.evaluated_individuals[~self.population.evaluated_individuals[self.objective_names].isin(["TIMEOUT","INVALID"]).any(axis=1)][self.objective_names]*sign
                     cur_best_scores = valid_df.max(axis=0)*sign
                     cur_best_scores = cur_best_scores.to_numpy()
                     print("Generation: ", self.generation)
@@ -639,15 +645,24 @@
         #print("evaluating this many individuals: ", len(individuals_to_evaluate))
 
         if len(individuals_to_evaluate) == 0:
             if self.verbose > 3:
                 print("No new individuals to evaluate")
             return
 
-        scores = tpot2.objectives.parallel_eval_objective_list(individuals_to_evaluate, self.objective_functions, self.n_jobs, verbose=self.verbose, timeout=self.max_eval_time_seconds, budget=budget, n_expected_columns=len(self.objective_names), client=self._client, **self.objective_kwargs)
+        if self.max_eval_time_seconds is not None:
+            theoretical_timeout = self.max_eval_time_seconds * math.ceil(len(individuals_to_evaluate) / self.n_jobs)
+            theoretical_timeout = theoretical_timeout*2
+        else:
+            theoretical_timeout = np.inf
+        scheduled_timeout_time_left = self.scheduled_timeout_time - time.time()
+        parallel_timeout = min(theoretical_timeout, scheduled_timeout_time_left)
+        if parallel_timeout < 0:
+            parallel_timeout = 10
+        scores = tpot2.objectives.parallel_eval_objective_list(individuals_to_evaluate, self.objective_functions, self.n_jobs, verbose=self.verbose, timeout=self.max_eval_time_seconds, budget=budget, n_expected_columns=len(self.objective_names), client=self._client, parallel_timeout=parallel_timeout, **self.objective_kwargs)
 
 
         self.population.update_column(individuals_to_evaluate, column_names=self.objective_names, data=scores)
         if budget is not None:
             self.population.update_column(individuals_to_evaluate, column_names="Budget", data=budget)
 
         self.population.remove_invalid_from_population(column_names=self.objective_names)
@@ -699,24 +714,35 @@
             unevaluated_individuals_this_step = self.get_unevaluated_individuals(this_step_names, budget=None, individual_list=cur_individuals)
 
             if len(unevaluated_individuals_this_step) == 0:
                 if self.verbose > 3:
                     print("No new individuals to evaluate")
                 continue
             
+            if self.max_eval_time_seconds is not None:
+                theoretical_timeout = self.max_eval_time_seconds * math.ceil(len(individuals_to_evaluate) / self.n_jobs)
+                theoretical_timeout = theoretical_timeout*2
+            else:
+                theoretical_timeout = np.inf
+            scheduled_timeout_time_left = self.scheduled_timeout_time - time.time()
+            parallel_timeout = min(theoretical_timeout, scheduled_timeout_time_left)
+            if parallel_timeout < 0:
+                parallel_timeout = 10
+
             scores = tpot2.objectives.parallel_eval_objective_list(individual_list=unevaluated_individuals_this_step,
                                     objective_list=self.objective_functions,
                                     n_jobs = self.n_jobs,
                                     verbose=self.verbose,
                                     timeout=self.max_eval_time_seconds,
                                     step=step,
                                     budget = self.budget,
                                     generation = self.generation,
                                     n_expected_columns=len(self.objective_names),
                                     client=self._client,
+                                    parallel_timeout=parallel_timeout,
                                     **self.objective_kwargs,
                                     )
 
             self.population.update_column(unevaluated_individuals_this_step, column_names=this_step_names, data=scores)
 
             self.population.remove_invalid_from_population(column_names=this_step_names)
             self.population.remove_invalid_from_population(column_names=this_step_names, invalid_value="TIMEOUT")
@@ -786,75 +812,7 @@
                     if step < self.evaluation_early_stop_steps - 1 and survival_counts[step]>1: #don't do selection for the last loop since they are completed
                         k = survival_counts[step] + len(invalids) #TODO can remove the min if the selections method can ignore k>population size
                         if len(cur_individuals)> 1 and k > self.n_jobs and k < len(cur_individuals):
                             weighted_scores = np.array([s * self.objective_function_weights for s in offspring_scores ])
 
                             new_population_index = survival_selector(weighted_scores, k=k)
                             cur_individuals = np.array(cur_individuals)[new_population_index]
-
-                    
-
-        
-
-
-
-
-
-
-
-
-
-def get_thresholds(scores, start=0, end=1, scale=.5, n=10,):
-       thresh = beta_interpolation(start=start, end=end, scale=scale, n=n)
-       return [np.percentile(scores, t) for t in thresh]
-
-
-
-
-
-def equalize_list(lst, n_steps):
-    step_size = len(lst) / n_steps
-    new_lst = []
-    for i in range(n_steps):
-        start_index = int(i * step_size)
-        end_index = int((i+1) * step_size)
-        if i == 0: # First segment
-            step_lst = [lst[start_index]] * (end_index - start_index)
-        elif i == n_steps-1: # Last segment
-            step_lst = [lst[-1]] * (end_index - start_index)
-        else: # Middle segment
-            segment = lst[start_index:end_index]
-            median_value = statistics.median(segment)
-            step_lst = [median_value] * (end_index - start_index)
-        new_lst.extend(step_lst)
-    return new_lst
-
-
-def beta_interpolation(start=0, end=1, scale=1, n=10, n_steps=None):
-    if n_steps is None:
-        n_steps = n
-    if n_steps > n:
-        n_steps = n
-    if scale <= 0:
-        scale = 0.0001
-    if scale >= 1:
-        scale = 0.9999
-
-    alpha = 2 * scale
-    beta = 2 - alpha
-    x = np.linspace(0,1,n)
-    values = scipy.special.betainc(alpha,beta,x)*(end-start)+start
-
-    if n_steps is not None:
-        return equalize_list(values, n_steps)
-    else:
-        return values
-
-#thanks chat gtp
-def remove_items(items, indexes_to_remove):
-    items = items.copy()
-    #if items is a numpy array, we need to convert to a list
-    if type(items) == np.ndarray:
-        items = items.tolist()
-    for index in sorted(indexes_to_remove, reverse=True):
-        del items[index]
-    return np.array(items)
```

### Comparing `TPOT2-0.1.1a0/tpot2/builtin_modules/arithmetictransformer.py` & `TPOT2-0.1.2a0/tpot2/builtin_modules/arithmetictransformer.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/builtin_modules/feature_encoding_frequency_selector.py` & `TPOT2-0.1.2a0/tpot2/builtin_modules/feature_encoding_frequency_selector.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/builtin_modules/feature_set_selector.py` & `TPOT2-0.1.2a0/tpot2/builtin_modules/feature_set_selector.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/builtin_modules/feature_transformers.py` & `TPOT2-0.1.2a0/tpot2/builtin_modules/feature_transformers.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/builtin_modules/genetic_encoders.py` & `TPOT2-0.1.2a0/tpot2/builtin_modules/genetic_encoders.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/builtin_modules/one_hot_encoder.py` & `TPOT2-0.1.2a0/tpot2/builtin_modules/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/builtin_modules/zero_count.py` & `TPOT2-0.1.2a0/tpot2/builtin_modules/zero_count.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/__init__.py` & `TPOT2-0.1.2a0/tpot2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/autoqtl_builtins.py` & `TPOT2-0.1.2a0/tpot2/config/autoqtl_builtins.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/classifiers.py` & `TPOT2-0.1.2a0/tpot2/config/classifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,23 @@
         'min_samples_split': trial.suggest_int(f'min_samples_split_{name}', 2, 20),
         'min_samples_leaf': trial.suggest_int(f'min_samples_leaf_{name}', 1, 20),
         'n_jobs': 1,
     }
     return params
 
 
-def params_GradientBoostingClassifier(trial, name=None):
+def params_GradientBoostingClassifier(trial,n_classes=None, name=None):
+    if n_classes is not None and n_classes > 2:
+        loss = 'log_loss'
+    else:
+        loss = trial.suggest_categorical(name=f'loss_{name}', choices=['log_loss', 'exponential'])
+    
     params = {
         'n_estimators': 100,
-        'loss': trial.suggest_categorical(name=f'loss_{name}', choices=['log_loss', 'exponential']),
+        'loss': loss,
         'learning_rate': trial.suggest_float(f'learning_rate_{name}', 1e-3, 1, log=True),
         'min_samples_leaf': trial.suggest_int(f'min_samples_leaf_{name}', 1, 20),
         'min_samples_split': trial.suggest_int(f'min_samples_split_{name}', 2, 20),
         'subsample': trial.suggest_float(f'subsample_{name}', 0.1, 1.0),
         'max_features': trial.suggest_float(f'max_features_{name}', 0.1, 1.0),
         'max_depth': trial.suggest_int(f'max_depth_{name}', 1, 10),
         'tol': 1e-4,
@@ -223,23 +228,23 @@
     params = {
         'alpha': trial.suggest_float(f'alpha_{name}', 1e-3, 100, log=True),
         'fit_prior': trial.suggest_categorical(f'fit_prior_{name}', [True, False]),
     }
     return params
 
 
-def make_classifier_config_dictionary(n_samples=10):
+def make_classifier_config_dictionary(n_samples=10, n_classes=None):
     n_samples = min(n_samples,100) #TODO optimize this
 
 
     return {
             LogisticRegression: params_LogisticRegression,
             DecisionTreeClassifier: params_DecisionTreeClassifier,
             KNeighborsClassifier:  partial(params_KNeighborsClassifier,n_samples=n_samples),
-            GradientBoostingClassifier: params_GradientBoostingClassifier,
+            GradientBoostingClassifier: partial(params_GradientBoostingClassifier, n_classes=n_classes),
             ExtraTreesClassifier:params_ExtraTreesClassifier,
             RandomForestClassifier: params_RandomForestClassifier,
             SGDClassifier:params_SGDClassifier,
             GaussianNB: {},
             BernoulliNB: params_BernoulliNB,
             MultinomialNB: params_MultinomialNB,
             XGBClassifier: params_XGBClassifier,
```

### Comparing `TPOT2-0.1.1a0/tpot2/config/hyperparametersuggestor.py` & `TPOT2-0.1.2a0/tpot2/config/hyperparametersuggestor.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/mdr_configs.py` & `TPOT2-0.1.2a0/tpot2/config/mdr_configs.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/regressors.py` & `TPOT2-0.1.2a0/tpot2/config/regressors.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/selectors.py` & `TPOT2-0.1.2a0/tpot2/config/selectors.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/special_configs.py` & `TPOT2-0.1.2a0/tpot2/config/special_configs.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/config/transformers.py` & `TPOT2-0.1.2a0/tpot2/config/transformers.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/estimator_objective_functions.py` & `TPOT2-0.1.2a0/tpot2/estimator_objective_functions.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/graphsklearn.py` & `TPOT2-0.1.2a0/tpot2/graphsklearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,19 @@
         #TODO clean this up
         try:
             nx.find_cycle(self.G)
             raise BaseException 
         except: 
             pass
         
+    def __str__(self):
+        if len(self.graph.edges) > 0:
+            return str(self.graph.edges)
+        else:
+            return str(self.graph.nodes)
 
     def fit(self, X, y, subset_col = None):
         # if self.subset_column is not None and self.subset_values is not None:
             
         #     if isinstance(X, pd.DataFrame):
         #         indeces_to_keep = X[self.subset_column].isin(self._subset_values)
         #         X = X[indeces_to_keep]
@@ -305,14 +310,16 @@
                                 y=y,
                                 method=self.method,
                                 cross_val_predict_cv = self.cross_val_predict_cv,
                                 memory = self.memory,
                                 topo_sort = self.topo_sorted_nodes,
                                 subset_col = subset_col,
                                 )
+        
+        return self
 
     def plot(self, ):
         plot(graph = self.graph)
 
     def __sklearn_is_fitted__(self):
         '''Indicate whether pipeline has been fit.'''
         try:
```

### Comparing `TPOT2-0.1.1a0/tpot2/individual.py` & `TPOT2-0.1.2a0/tpot2/individual.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/objectives.py` & `TPOT2-0.1.2a0/tpot2/objectives.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,22 +57,22 @@
 
             if len(w) and verbose>=4:
                 
                 warnings.warn(w[0].message)
             return value
         except func_timeout.exceptions.FunctionTimedOut:
             if verbose >= 4:
-                print(f'WARNING AN INDIVIDUAL TIMED OUT')
+                print(f'WARNING AN INDIVIDUAL TIMED OUT: \n {individual} \n')
             return ["TIMEOUT"]
         except Exception as e:
             if verbose == 4:
-                print(f'WARNING THIS INDIVIDUAL CAUSED AND EXCEPTION \n {e}')
+                print(f'WARNING THIS INDIVIDUAL CAUSED AND EXCEPTION \n {individual} \n {e} \n')
             if verbose >= 5:
                 trace = traceback.format_exc()
-                print(f'WARNING THIS INDIVIDUAL CAUSED AND EXCEPTION \n {e} \n {trace}')
+                print(f'WARNING THIS INDIVIDUAL CAUSED AND EXCEPTION \n {individual} \n {e} \n {trace}')
             return ["INVALID"]
         
 
 def eval_objective_list(ind, objective_list, verbose=0,**objective_kwargs):
 
     scores = np.concatenate([objective_nan_wrapper(ind, obj, verbose,**objective_kwargs) for obj in objective_list ])
     return scores
@@ -80,39 +80,57 @@
 def parallel_eval_objective_list(individual_list,
                                 objective_list,
                                 n_jobs = 1,
                                 verbose=0,
                                 timeout=None,
                                 n_expected_columns=None,
                                 client=None,
+                                parallel_timeout=None,
                                 **objective_kwargs):
 
     #offspring_scores = Parallel(n_jobs=n_jobs)(delayed(eval_objective_list)(ind,  objective_list, verbose, timeout=timeout)  for ind in individual_list )
     
     # delayed_values = [dask.delayed(eval_objective_list)(ind,  objective_list, verbose, timeout=timeout,**objective_kwargs)  for ind in individual_list]
     # with TqdmCallback(desc="Evaluating Individuals", disable=verbose<2, leave=False):
     #     offspring_scores = list(dask.compute( *delayed_values,
     #                             num_workers=n_jobs))
     # del delayed_values
     if client is None:
         client = dask.distributed.get_client()
     futures = [client.submit(eval_objective_list, ind,  objective_list, verbose, timeout=timeout,**objective_kwargs)  for ind in individual_list]
     
-    if verbose >= 2:
+    if verbose >= 6:
         dask.distributed.progress(futures, notebook=False)
     
-    dask.distributed.wait(futures)
+    try: 
+        if parallel_timeout is not None and np.isinf(parallel_timeout):
+            parallel_timeout = None
+        dask.distributed.wait(futures, timeout=parallel_timeout)
+    except dask.distributed.TimeoutError:
+        print("terminating parallel evaluation due to timeout")
+        pass
     
     offspring_scores = []
     # todo optimize this
-    for future in futures:
-        if not future.exception():
-            offspring_scores.append(future.result())
-        else:
+    for individual, future in zip(individual_list, futures):
+        if not future.done():
+            future.cancel()
+            offspring_scores.append(["TIMEOUT"])
+            if verbose >= 4:
+                print(f'WARNING AN INDIVIDUAL TIMED OUT: \n {individual} \n')
+        elif future.exception():
             offspring_scores.append(["INVALID"])
+            if verbose == 4:
+                print(f'WARNING THIS INDIVIDUAL CAUSED AND EXCEPTION \n {individual} \n {future.exception()} \n')
+            if verbose >= 5:
+                trace = traceback.format_exc()
+                print(f'WARNING THIS INDIVIDUAL CAUSED AND EXCEPTION \n {individual} \n {future.exception()} \n {future.traceback()}')
+        else:
+            offspring_scores.append(future.result())
+            
 
     if n_expected_columns is not None:
         offspring_scores = process_scores(offspring_scores, n_expected_columns)
     return offspring_scores
 
 
 ###################
```

### Comparing `TPOT2-0.1.1a0/tpot2/parent_selectors.py` & `TPOT2-0.1.2a0/tpot2/parent_selectors.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/population.py` & `TPOT2-0.1.2a0/tpot2/population.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/graph_utils/graph_utils.py` & `TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/graph_utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/representations/graph_pipeline_individual/individual.py` & `TPOT2-0.1.2a0/tpot2/representations/graph_pipeline_individual/individual.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sklearn.pipeline
 from typing import Generator
 import optuna
 from itertools import combinations
 from .graph_utils import graph_utils
 import itertools
 import baikal
+import copy
 
 class NodeLabel():
     def __init__(self, *,
 
         #intialized, but may change later
             method_class = None, #transformer or baseestimator
             hyperparameters=None,
@@ -100,39 +101,35 @@
     '''
     def __init__(
                 self,
                 root_config_dict,
                 inner_config_dict=None, 
                 leaf_config_dict=None,
                 initial_graph = None,
-                max_depth = np.inf,
                 max_size = np.inf, 
-                max_children = np.inf,
+                linear_pipeline = False,
                 name=None,
                 crossover_same_depth = False,
                 crossover_same_recursive_depth = True,
                 
 
                 unique_subset_values = None,
                 initial_subset_values = None,
                 ):
 
         self.__debug = False
 
         self.root_config_dict = root_config_dict
-        if inner_config_dict is None:
-            self.inner_config_dict = self.root_config_dict
-        else:
-            self.inner_config_dict = inner_config_dict
+        self.inner_config_dict = inner_config_dict
         self.leaf_config_dict = leaf_config_dict
 
-        self.max_depth = max_depth
+
         self.max_size = max_size
         self.name = name
-        self.max_children = max_children
+
         self.crossover_same_depth = crossover_same_depth
         self.crossover_same_recursive_depth = crossover_same_recursive_depth
 
         self.unique_subset_values = unique_subset_values
         self.initial_subset_values = initial_subset_values
 
         if self.unique_subset_values is not None:
@@ -184,33 +181,38 @@
 
  
         self.initialize_all_nodes()
 
         #self.root =list(nx.topological_sort(self.graph))[0]
 
 
-        self.mutate_methods_list = [    self._mutate_get_new_hyperparameter,
-                                        self._mutate_replace_method, 
-                                        self._mutate_insert_leaf,
+        self.mutate_methods_list =     [self._mutate_hyperparameters,
+                                        self._mutate_replace_node, 
                                         self._mutate_remove_node,
-                                        self._mutate_add_connection_from,
-                                        self._mutate_remove_extra_edge,
-                                        self._mutate_insert_inner_node,
+                                        ]
+        
+        self.crossover_methods_list = [
+                                        #self._crossover_swap_node,
+                                        #self._crossover_hyperparameters,
+                                        self._crossover_swap_branch,
+                                        #self._crossover_take_branch,
+                                        #self._crossover_swap_leaf_at_node,
                                         ]
 
+        if self.inner_config_dict is not None:
+            self.mutate_methods_list.append(self._mutate_insert_inner_node)
+            self.crossover_methods_list.append(self._crossover_take_branch) #this is the only crossover method that can create inner nodes
+            if not linear_pipeline:
+                self.mutate_methods_list.append(self._mutate_insert_bypass_node)
+
+        if not linear_pipeline:
+            self.mutate_methods_list.append(self._mutate_insert_leaf)
+
 
 
-        self.crossover_methods_list = [
-                                    #self._crossover_swap_node,
-                                    #self._crossover_hyperparameters,
-                                    self._crossover_swap_branch_with_all_children,
-                                    self._crossover_combine_and_prune,
-                                    self._crossover_take_branch_with_all_children,
-                                    #self._crossover_swap_leaf_at_node,
-                                            ]
 
         if self.unique_subset_values is not None:
             self.crossover_methods_list.append(self._crossover_row_subsets)
             self.mutate_methods_list.append(self._mutate_row_subsets )
 
         self.optimize_methods_list = [ #self._optimize_optuna_single_method_full_pipeline,
                                         self._optimize_optuna_all_methods_full_pipeline]
@@ -254,66 +256,15 @@
             compliant_leafs.append(first_leaf)
 
         #connect bad leaves to good leaves (making them internal nodes)
         if len(noncompliant_leafs) > 0:
             for node in noncompliant_leafs:
                 self.graph.add_edge(node, random.choice(compliant_leafs))
 
-    # max_depth = np.inf,
-    # max_size = np.inf, 
-    # max_children = np.inf,
-    def prune_to_limits(self,):
-        
-
-
-        #Find all leaves that are too deep,
-        # Get the sequence for the longest path
-        # remove nodes from path, starting from the leaves 
-
-
-        # nodelist = graph_utils.get_leaves(self.graph)
-        # if not np.isinf(self.max_depth):
-        #     for node in nodelist:
-        #         done = False
-        #         while not done: #TODO make more efficient
-        #             done = True
-        #             max_path = graph_utils.get_max_path_size(self.graph, self.root, node, return_path=True)
-        #             if len(max_path) > self.max_depth:
-        #                 max_path.reverse()
-        #                 if self.leaf_config_dict is not None:
-        #                     max_path.remove(node)
-        #                 number_to_remove = len(max_path) - self.max_depth
-        #                 #max_path.remove(node)
-        #                 for i in range(number_to_remove):
-        #                     graph_utils.remove_and_stitch(self.graph, max_path[i])
-        #                     done = False
-                        
-
-            
-        #max_size
-        nodelist = list(self.graph.nodes)
-        nodelist.remove(self.root)
-        if len(nodelist) > self.max_size:
-            random.shuffle(nodelist)
-            for n in nodelist[0:len(nodelist) - self.max_size]:
-                graph_utils.remove_and_stitch(self.graph, n)
-
-        #max children
-        nodelist= list(self.graph.nodes)
-        for node in nodelist:
-            #if a node has more children than allowed
-            successors = list(self.graph.successors(node))
-            num_successors = len(successors)
-            if num_successors > self.max_children:
-                #move the extra children
-                random.shuffle(successors)
-                for c in successors[0:num_successors-self.max_children]:
-                    self.graph.remove_edge(node,c)
 
-        graph_utils.remove_nodes_disconnected_from_node(self.graph, self.root)
 
 
     def _merge_duplicated_nodes(self): 
 
         graph_changed = False
         merged = False
         while(not merged):
@@ -552,17 +503,14 @@
     #TODO currently does not correctly return false when adding a leaf causes a duplicate node that is later merged
     def mutate(self,):
         self.key = None
         graph = self.select_graphindividual()
         return graph._mutate()
 
     def _mutate(self,):
-        
-
-        
         random.shuffle(self.mutate_methods_list)
         for mutate_method in self.mutate_methods_list:
             if mutate_method():
                 self._merge_duplicated_nodes()
 
                 if self.__debug:
                     print(mutate_method)
@@ -578,40 +526,45 @@
 
                     if self.__debug:
                         try:
                             nx.find_cycle(self.graph)
                             print('something went wrong with ', mutate_method)
                         except: 
                             pass
-
                 
                 return True
             
         return False
 
     def _mutate_row_subsets(self,):
         if self.unique_subset_values is not None:
             self.row_subset_selector.mutate()
 
 
-    def _mutate_get_new_hyperparameter(self):
+    def _mutate_hyperparameters(self):
+        '''
+        Mutates the hyperparameters for a randomly chosen node in the graph.
+        '''
         sorted_nodes_list = list(self.graph.nodes)
-        random.shuffle(sorted_nodes_list) #TODO: sort by number of children and/or parents? bias model one way or another
+        random.shuffle(sorted_nodes_list) 
         for node in sorted_nodes_list:
             if isinstance(node,GraphIndividual):
                 continue
             if isinstance(self.select_config_dict(node)[node.method_class], dict):
                 continue
             node.hyperparameters = self.select_config_dict(node)[node.method_class](config.hyperparametersuggestor) 
             
             return True
         return False
 
-    #cannot replace method with the same method
-    def _mutate_replace_method(self):
+    def _mutate_replace_node(self):
+        '''
+        Replaces the method in a randomly chosen node by a method from the available methods for that node.
+
+        '''
         sorted_nodes_list = list(self.graph.nodes)
         random.shuffle(sorted_nodes_list) 
         for node in sorted_nodes_list:
             if isinstance(node,GraphIndividual):
                 continue
             node.method_class = random.choice(list(self.select_config_dict(node).keys())) 
             if isinstance(self.select_config_dict(node)[node.method_class], dict):
@@ -620,151 +573,161 @@
                 hyperparameters = self.select_config_dict(node)[node.method_class](config.hyperparametersuggestor)
             node.hyperparameters = hyperparameters
             return True
             
         return False
 
 
-    #removes a random node and connects its parents to its children
-    # if the node is a leaf, and leafs are protected, randomly assign existing leaf
     def _mutate_remove_node(self):
+        '''
+        Removes a randomly chosen node and connects its parents to its children.
+        If the node is the only leaf for an inner node and 'leaf_config_dict' is not none, we do not remove it.
+        '''
         nodes_list = list(self.graph.nodes)
         nodes_list.remove(self.root)
         leaves = graph_utils.get_leaves(self.graph)
-        #random.shuffle(sorted_nodes_list) #TODO: sort by number of children and/or parents? bias model one way or another
+
         while len(nodes_list) > 0:
-            node = random.choices(nodes_list, weights=[1/((len(list(nx.neighbors(self.graph, n)))+1)**100) for n in nodes_list])[0]
+            node = random.choices(nodes_list,)[0]
             nodes_list.remove(node)
 
-            if self.leaf_config_dict is not None and len(list(nx.descendants(self.graph,node))) == 0 : #if we are protecting leafs and node is a leaf
+            if self.leaf_config_dict is not None and len(list(nx.descendants(self.graph,node))) == 0 : #if the node is a leaf
                 if len(leaves) <= 1:
                     continue #dont remove the last leaf
                 leaf_parents = self.graph.predecessors(node)
-                graph_utils.remove_and_stitch(self.graph, node)
-                leaves.remove(node)
-                for p in leaf_parents:
-                    # if p has no children, randomly assign a child from leaves
-                    if len(list(nx.descendants(self.graph,p))) < 1:
-                        new_child = random.choice(leaves)
-                        self.graph.add_edge(p, new_child)
 
-                
-                #TODO make more efficient
-                if any([len(list(nx.descendants(self.graph,lp))) < 2 for lp in leaf_parents]): #dont remove a leaf if it is the only input into another node.
+                # if any of the parents of the node has one one child, continue
+                if any([len(list(self.graph.successors(lp))) < 2 for lp in leaf_parents]): #dont remove a leaf if it is the only input into another node.
                     continue
 
+                graph_utils.remove_and_stitch(self.graph, node)
+                graph_utils.remove_nodes_disconnected_from_node(self.graph, self.root)
+                return True
+
             else:
                 graph_utils.remove_and_stitch(self.graph, node)
+                graph_utils.remove_nodes_disconnected_from_node(self.graph, self.root)
+                return True
             
-            return True
         return False
 
-        #loop through nodes and delete an edge to one of it's extra parents
-    def _mutate_remove_extra_edge(self):
+    def _mutate_remove_edge(self):
+        '''
+        Deletes an edge as long as deleting that edge does not make the graph disconnected.
+        '''
         sorted_nodes_list = list(self.graph.nodes)
-        random.shuffle(sorted_nodes_list) #TODO: sort by number of children and/or parents? bias model one way or another
+        random.shuffle(sorted_nodes_list) 
         for child_node in sorted_nodes_list:
             parents = list(self.graph.predecessors(child_node))
             if len(parents) > 1: # if it has more than one parent, you can remove an edge (if this is the only child of a node, it will become a leaf)
 
                 for parent_node in parents:
-                    #if we are protecting leafs and parent node is a leaf, skip
+                    # if removing the egde will make the parent_node a leaf node, skip
                     if self.leaf_config_dict is not None and len(list(self.graph.successors(parent_node))) < 2: 
                         continue
 
-                    
                     self.graph.remove_edge(parent_node, child_node)
                     return True
         return False
 
-    def _mutate_add_connection_from(self):
+    def _mutate_add_edge(self):
         '''
-        Randomly add an edge from a node to another node that is not an ancestor of the first node
+        Randomly add an edge from a node to another node that is not an ancestor of the first node.
         '''
         sorted_nodes_list = list(self.graph.nodes)
-        sorted_nodes_list2 = list(self.graph.nodes)
-        random.shuffle(sorted_nodes_list) #TODO: sort by number of children and/or parents? bias model one way or another
-        random.shuffle(sorted_nodes_list2)
+        random.shuffle(sorted_nodes_list)
         for child_node in sorted_nodes_list:
             for parent_node in sorted_nodes_list:
                 if self.leaf_config_dict is not None:
                     if len(list(self.graph.successors(parent_node))) == 0:
                         continue
                 
                 # skip if
-                # parent and child are the same node
-                # edge already exists
-                # child is an ancestor of parent
-                if  (child_node is not parent_node) and not self.graph.has_edge(parent_node,child_node) and (child_node not in nx.ancestors(self.graph, parent_node)): 
-                    
+                # - parent and child are the same node
+                # - edge already exists
+                # - child is an ancestor of parent
+                if  (child_node is not parent_node) and not self.graph.has_edge(parent_node,child_node) and (child_node not in nx.ancestors(self.graph, parent_node)):         
                     self.graph.add_edge(parent_node,child_node)
                     return True
 
         return False
 
 
-
-
-
     def _mutate_insert_leaf(self):
         if self.max_size > self.graph.number_of_nodes():
             sorted_nodes_list = list(self.graph.nodes)
             random.shuffle(sorted_nodes_list) #TODO: sort by number of children and/or parents? bias model one way or another
             for node in sorted_nodes_list:
                 #if leafs are protected, check if node is a leaf
                 #if node is a leaf, skip because we don't want to add node on top of node
                 if (self.leaf_config_dict is not None #if leafs are protected
                     and   len(list(self.graph.successors(node))) == 0 #if node is leaf
                     and  len(list(self.graph.predecessors(node))) > 0 #except if node is root, in which case we want to add a leaf even if it happens to be a leaf too
                     ):
                     
                     
                     continue
+      
+                #If node *is* the root or is not a leaf, add leaf node. (dont want to add leaf on top of leaf)
+                if self.leaf_config_dict is not None:
+                    new_node = create_node(self.leaf_config_dict)
+                else:
+                    new_node = create_node(self.inner_config_dict)
 
-                if self.max_children > len(list(self.graph.successors(node))):
-                    if np.isinf(self.max_depth) or  self.max_depth >= 1+  graph_utils.get_max_path_size(self.graph, self.root, node): #stackoverflow, check, can it be more efficient?:
-                        
-
-                        
-                            #If node *is* the root or is not a leaf, add leaf node. (dont want to add leaf on top of leaf)
-                        if self.leaf_config_dict is not None:
-                            new_node = create_node(self.leaf_config_dict)
-                        else:
-                            new_node = create_node(self.inner_config_dict)
+                self.graph.add_node(new_node)
+                self.graph.add_edge(node, new_node)
+                return True
 
+        return False
 
-                        self.graph.add_node(new_node)
-                        self.graph.add_edge(node, new_node)
-                        return True
+    def _mutate_insert_bypass_node(self):
+        if self.max_size > self.graph.number_of_nodes():
+            sorted_nodes_list = list(self.graph.nodes)
+            sorted_nodes_list2 = list(self.graph.nodes)
+            random.shuffle(sorted_nodes_list) #TODO: sort by number of children and/or parents? bias model one way or another
+            random.shuffle(sorted_nodes_list2)
+            for node in sorted_nodes_list:  
+                for child_node in sorted_nodes_list2:
+                    if child_node is not node and child_node not in nx.ancestors(self.graph, node):
+                        if self.leaf_config_dict is not None:
+                            #If if we are protecting leafs, dont add connection into a leaf
+                            if len(list(nx.descendants(self.graph,node))) ==0 :
+                                continue
+
+                            new_node = create_node(config_dict = self.inner_config_dict)
+
+                            self.graph.add_node(new_node)
+                            self.graph.add_edges_from([(node, new_node), (new_node, child_node)])
+                            return True
 
         return False
 
+
     def _mutate_insert_inner_node(self):
         if self.max_size > self.graph.number_of_nodes():
             sorted_nodes_list = list(self.graph.nodes)
             sorted_nodes_list2 = list(self.graph.nodes)
             random.shuffle(sorted_nodes_list) #TODO: sort by number of children and/or parents? bias model one way or another
             random.shuffle(sorted_nodes_list2)
             for node in sorted_nodes_list:
-                if self.max_children > len(self.graph):
-                    for child_node in sorted_nodes_list2:
-                        if child_node is not node and child_node not in nx.ancestors(self.graph, node):
-                            if self.leaf_config_dict is not None:
-                                #If if we are protecting leafs, dont add connection into a leaf
-                                if len(list(nx.descendants(self.graph,node))) ==0 :
-                                    continue
-                            
-                            #If adding this node will not make the graph too deep
-                            if np.isinf(self.max_depth) or  self.max_depth > graph_utils.get_max_path_through_node(self.graph, self.root, child_node): #this is pretty inneficient.
-
-                                    new_node = create_node(config_dict = self.inner_config_dict)
-
-                                    self.graph.add_node(new_node)
-                                    self.graph.add_edges_from([(node, new_node), (new_node, child_node)])
-                                    return True
+                #loop through children of node
+                for child_node in list(self.graph.successors(node)):
+                    
+                    if child_node is not node and child_node not in nx.ancestors(self.graph, node):
+                        if self.leaf_config_dict is not None:
+                            #If if we are protecting leafs, dont add connection into a leaf
+                            if len(list(nx.descendants(self.graph,node))) ==0 :
+                                continue
+                        
+                            new_node = create_node(config_dict = self.inner_config_dict)
+
+                            self.graph.add_node(new_node)
+                            self.graph.add_edges_from([(node, new_node), (new_node, child_node)])
+                            self.graph.remove_edge(node, child_node)
+                            return True
 
         return False
 
     ######################################################
     # Crossover
 
     def get_graphs(self):
@@ -806,15 +769,14 @@
 
         for g1, g2 in zip(g1_sorted_graphs, g2_sorted_graphs):
             if g1.graph.graph['depth'] == g2.graph.graph['depth'] and g1.graph.graph['recursive depth'] == g2.graph.graph['recursive depth']:
                 return g1, g2
 
         return ind1,ind2
 
-    #TODO make more efficient
     def crossover(self, ind2):
         '''
         self is the first individual, ind2 is the second individual
         If crossover_same_depth, it will select graphindividuals at the same recursive depth.
         Otherwise, it will select graphindividuals randomly from the entire graph and its subgraphs.
 
         This does not impact graphs without subgraphs. And it does not impacts nodes that are not graphindividuals. Cros
@@ -834,48 +796,36 @@
         return g1._crossover(g2)
     
     def _crossover(self, Graph):
     
         random.shuffle(self.crossover_methods_list)
         for crossover_method in self.crossover_methods_list:
             if crossover_method(Graph):
-                self.prune_to_limits()
                 self._merge_duplicated_nodes()
-                #Graph.prune_to_limits()
-                #Graph._merge_duplicated_nodes()
-
-            # if self.leaf_config_dict is not None:
-            #     self.fix_noncompliant_leafs()
-
-            self._merge_duplicated_nodes()
-
-            return True
+                return True
 
         if self.__debug:
             try:
                 nx.find_cycle(self.graph)
-                #nx.find_cycle(Graph.graph)
                 print('something went wrong with ', crossover_method)
             except: 
                 pass
 
         return False
 
 
-
-    #Mutators for the whole graph
-    #TODO
-
     def _crossover_row_subsets(self, G2):
         if self.unique_subset_values is not None and G2.unique_subset_values is not None:
             self.row_subset_selector.crossover(G2.row_subset_selector)
     
 
     def _crossover_swap_node(self, G2):
-
+        '''
+        Swaps randomly chosen node from Parent1 with a randomly chosen node from Parent2.
+        '''
         if self.crossover_same_depth:
             pair_gen = graph_utils.select_nodes_same_depth(self.graph, self.root, G2.graph, G2.root)
         else:
             pair_gen = graph_utils.select_nodes_randomly(self.graph, G2.graph)
 
         for node1, node2 in pair_gen:
             if not (node1 is self.root or node2 is G2.root): #TODO: allow root
@@ -898,72 +848,67 @@
                 G2.graph.add_edges_from([ (n, node1) for n in n2_p])
                 
                 return True
         return False
 
 
 
-    def _crossover_swap_branch_with_all_children(self, G2):
-
+    def _crossover_swap_branch(self, G2):
+        '''
+        swaps a branch from parent1 with a branch from parent2. does not modify parent2
+        '''
         if self.crossover_same_depth:
             pair_gen = graph_utils.select_nodes_same_depth(self.graph, self.root, G2.graph, G2.root)
         else:
             pair_gen = graph_utils.select_nodes_randomly(self.graph, G2.graph)
 
         for node1, node2 in pair_gen:
-
-            if node1 is self.root or node2 is G2.root:
+            #TODO: if root is in inner_config_dict, then do use it?
+            if node1 is self.root or node2 is G2.root: #dont want to add root as inner node
                 continue
             
-            #if node1 has fewer children than max_children, skip
-            if len(list(self.graph.successors(node1))) < self.max_children:
-                continue
-
-            #check if node2 type is in the list of allowed types
-            #is node2 is graph individual
-            if isinstance(node2,GraphIndividual):
-                if not ((isinstance(node2,GraphIndividual) and ("Recursive" in self.inner_config_dict or "Recursive" in self.leaf_config_dict))):
-                    continue
-            else:
-                if node2.method_class not in self.inner_config_dict: #in case node2 is a root with method that is not supposed to be an inner node #TODO if we should check for leaf config dict?
+            #check if node1 is a leaf and leafs are protected, don't add an input to the leave 
+            if self.leaf_config_dict is not None: #if we are protecting leaves, 
+                node1_is_leaf = len(list(self.graph.successors(node1))) == 0
+                node2_is_leaf = len(list(G2.graph.successors(node2))) == 0
+                #if not ((node1_is_leaf and node1_is_leaf) or (not node1_is_leaf and not node2_is_leaf)): #if node1 is a leaf
+                if (node1_is_leaf and (not node2_is_leaf)) or ( (not node1_is_leaf) and node2_is_leaf):
+                    #only continue if node1 and node2 are both leaves or both not leaves
                     continue
-            
+
             temp_graph_1 = self.graph.copy()
             temp_graph_1.remove_node(node1)
             graph_utils.remove_nodes_disconnected_from_node(temp_graph_1, self.root)
 
             #isolating the branch
             branch2 = G2.graph.copy()
             n2_descendants = nx.descendants(branch2,node2)
             for n in list(branch2.nodes):
                 if n not in n2_descendants and n is not node2: #removes all nodes not in the branch
                     branch2.remove_node(n)
 
-            leaves = graph_utils.get_leaves(branch2)
-            #if node1 plus node2 branch has more than max_children, skip
-            if branch2.number_of_nodes() + temp_graph_1.number_of_nodes() > self.max_size:
-                continue
-            
-            self.graph = temp_graph_1
-            #TODO check depth
-            #if max_depth of node1 plus node2 branch is greater than max_depth, skip 
-            # if np.isinf(self.max_depth) or  self.max_depth >= 1+  graph_utils.get_max_path_size(self.graph, self.root, node1) + graph_utils.get_max_path_size(branch2, node2, leaves[0]):
-            #     continue
+            branch2 = copy.deepcopy(branch2)
+            branch2_root = graph_utils.get_roots(branch2)[0]
+            temp_graph_1.add_edges_from(branch2.edges)
+            for p in list(self.graph.predecessors(node1)):
+                temp_graph_1.add_edge(p,branch2_root)
 
-            self.graph.add_edges_from(branch2.edges)
-            for p in nx.descendants(self.graph,node1):
-                self.graph.add_edge(p,node2)
+            if temp_graph_1.number_of_nodes() > self.max_size:
+                continue
 
+            self.graph = temp_graph_1
 
             return True
         return False
 
-    #picks two twos with same type and swaps hyperparameters
     #TODO: Currently returns true even if hyperparameters are blank
     def _crossover_hyperparameters(self, G2):
+        '''
+        Swaps the hyperparamters of one randomly chosen node in Parent1 with the hyperparameters of randnomly chosen node in Parent2.
+        '''
         if self.crossover_same_depth:
             pair_gen = graph_utils.select_nodes_same_depth(self.graph, self.root, G2.graph, G2.root)
         else:
             pair_gen = graph_utils.select_nodes_randomly(self.graph, G2.graph)
 
         for node1, node2 in pair_gen:
             if isinstance(node1,GraphIndividual) or isinstance(node2,GraphIndividual):
@@ -1003,88 +948,64 @@
             if len(node_leafs) >0:
                 for c in node_leafs:
                     if random.choice([True,False]):
                         G2.graph.remove_node(c)
                         self.graph.add_edge(node1, c)
                         success = True
 
-
         return success
 
 
-
-    def _crossover_take_branch_with_all_children(self, G2):
-
+    def _crossover_take_branch(self, G2):
+        '''
+        Takes a subgraph from Parent2 and add it to a randomly chosen node in Parent1.
+        '''
         if self.crossover_same_depth:
             pair_gen = graph_utils.select_nodes_same_depth(self.graph, self.root, G2.graph, G2.root)
         else:
             pair_gen = graph_utils.select_nodes_randomly(self.graph, G2.graph)
 
         for node1, node2 in pair_gen:
-            #if node1 has fewer children than max_children, skip
-            if len(list(self.graph.successors(node1))) < self.max_children:
+            #TODO: if root is in inner_config_dict, then do use it?
+            if node2 is G2.root: #dont want to add root as inner node
                 continue
-
-            #check if node2 type is in the list of allowed types
-            #is node2 is graph individual
-            if isinstance(node2,GraphIndividual):
-                if not ((isinstance(node2,GraphIndividual) and ("Recursive" in self.inner_config_dict or "Recursive" in self.leaf_config_dict))):
-                    continue
-            else:
-                if node2.method_class not in self.inner_config_dict: #in case node2 is a root with method that is not supposed to be an inner node 
-                    continue
             
 
+            #check if node1 is a leaf and leafs are protected, don't add an input to the leave 
+            if self.leaf_config_dict is not None and len(list(self.graph.successors(node1))) == 0:
+                continue
+
+            #icheck if node2 is graph individual
+            # if isinstance(node2,GraphIndividual):
+            #     if not ((isinstance(node2,GraphIndividual) and ("Recursive" in self.inner_config_dict or "Recursive" in self.leaf_config_dict))):
+            #         continue
+
             #isolating the branch
             branch2 = G2.graph.copy()
             n2_descendants = nx.descendants(branch2,node2)
             for n in list(branch2.nodes):
                 if n not in n2_descendants and n is not node2: #removes all nodes not in the branch
                     branch2.remove_node(n)
 
-            leaves = graph_utils.get_leaves(branch2)
             #if node1 plus node2 branch has more than max_children, skip
             if branch2.number_of_nodes() + self.graph.number_of_nodes() > self.max_size:
                 continue
 
-            #TODO check depth
-            #if max_depth of node1 plus node2 branch is greater than max_depth, skip 
-            # if np.isinf(self.max_depth) or  self.max_depth >= 1+  graph_utils.get_max_path_size(self.graph, self.root, node1) + graph_utils.get_max_path_size(branch2, node2, leaves[0]):
-            #     continue
-
+            branch2 = copy.deepcopy(branch2)
+            branch2_root = graph_utils.get_roots(branch2)[0]
             self.graph.add_edges_from(branch2.edges)
-            self.graph.add_edge(node1,node2)
-
+            self.graph.add_edge(node1,branch2_root)
 
             return True
         return False
 
     #TODO: swap all leaf nodes
     def _crossover_swap_all_leafs(self, G2):
         pass
 
-    #TODO
-    def _crossover_combine_and_prune(self, G2):
-        taget_size = (self.graph.number_of_nodes() + G2.graph.number_of_nodes())/2
-
-        branch2 = G2.graph.copy()
-        root_children = list(branch2.successors(G2.root))
-        branch2.remove_node(G2.root)
-        self.graph.add_edges_from(branch2.edges)
-        for c in root_children:
-            self.graph.add_edge(self.root, c)
-        
-        self._merge_duplicated_nodes()
-
-        #prune
-        while self.graph.number_of_nodes() > taget_size:
-            if not self._mutate_remove_node():
-                break
-
-        return True
 
     #TODO: currently ignores ensembles, make it include nodes inside of ensembles
     def optimize(self, objective_function, steps=5):
         random.shuffle(self.optimize_methods_list) #select an optimization method
         for optimize_method in self.optimize_methods_list:
             if optimize_method(objective_function, steps=steps):
                 return True
@@ -1149,14 +1070,16 @@
    
     def _cached_transform(cache_nunber=0):
         #use a cache for models at each CV fold?
         #cache just transformations at each fold?
         #TODO how to separate full model?
         pass
 
+    def __str__(self):
+        return self.export_pipeline().__str__()
 
     def unique_id(self) -> GraphKey:
         if self.key is None:
             g = self.flatten_pipeline()
             for n in g.nodes:
                 if "subset_values" in g.nodes[n]:
                     g.nodes[n]['label'] = {n.method_class: n.hyperparameters, "subset_values":g.nodes[n]["subset_values"]}
```

### Comparing `TPOT2-0.1.1a0/tpot2/representations/subset_selector/subsetselector.py` & `TPOT2-0.1.2a0/tpot2/representations/subset_selector/subsetselector.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/tests/test_hello_world.py` & `TPOT2-0.1.2a0/tpot2/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/tests/test_nodes.py` & `TPOT2-0.1.2a0/tpot2/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.1a0/tpot2/tpot_estimator/estimator.py` & `TPOT2-0.1.2a0/tpot2/tpot_estimator/estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,21 @@
                         scorers_weights,
                         classification,
                         cv = 5,
                         other_objective_functions=[tpot2.estimator_objective_functions.average_path_length_objective], #tpot2.estimator_objective_functions.number_of_nodes_objective],
                         other_objective_functions_weights = [-1],
                         objective_function_names = None,
                         bigger_is_better = True,
-                        max_depth = np.inf,
                         max_size = np.inf, 
-                        max_children = np.inf,
+                        linear_pipeline = False,
                         root_config_dict= 'Auto',
                         inner_config_dict=["selectors", "transformers"],
                         leaf_config_dict= None,                        
                         cross_val_predict_cv = 0,
+                        categorical_features = None,
                         subsets = None,
                         memory = None,
                         preprocessing = False,  
                         validation_strategy = "none",
                         validation_fraction = .2,
                         population_size = 50,
                         initial_population_size = None,
@@ -116,22 +116,20 @@
         
         objective_function_names : list, default=None
             A list of names to be applied to the objective functions. If None, will use the names of the objective functions.
         
         bigger_is_better : bool, default=True
             If True, the objective function is maximized. If False, the objective function is minimized. Use negative weights to reverse the direction.
 
-        max_depth : int, default=np.inf
-            The maximum depth from any node to the root of the pipelines to be generated.
         
         max_size : int, default=np.inf
             The maximum number of nodes of the pipelines to be generated.
         
-        max_children : ind, default=np.inf 
-            The maximum number of children nodes in the pipelines can have. If set to 1, the pipelines will be linear.
+        linear_pipeline : bool, default=False
+            If True, the pipelines generated will be linear. If False, the pipelines generated will be directed acyclic graphs.
         
         root_config_dict : dict, default='auto'
             The configuration dictionary to use for the root node of the model.
             If 'auto', will use "classifiers" if classification=True, else "regressors".
             - 'selectors' : A selection of sklearn Selector methods.
             - 'classifiers' : A selection of sklearn Classifier methods.
             - 'regressors' : A selection of sklearn Regressor methods.
@@ -189,14 +187,19 @@
         cross_val_predict_cv : int, default=0
             Number of folds to use for the cross_val_predict function for inner classifiers and regressors. Estimators will still be fit on the full dataset, but the following node will get the outputs from cross_val_predict.
             
             - 0-1 : When set to 0 or 1, the cross_val_predict function will not be used. The next layer will get the outputs from fitting and transforming the full dataset.
             - >=2 : When fitting pipelines with inner classifiers or regressors, they will still be fit on the full dataset. 
                     However, the output to the next node will come from cross_val_predict with the specified number of folds.
          
+        categorical_features: list or None
+            Categorical columns to inpute and/or one hot encode during the preprocessing step. Used only if preprocessing is not False.
+            - None : If None, TPOT2 will automatically use object columns in pandas dataframes as objects for one hot encoding in preprocessing.
+            - List of categorical features. If X is a dataframe, this should be a list of column names. If X is a numpy array, this should be a list of column indices
+
         subsets : str or list, default=None
             Sets the subsets that the FeatureSetSeletor will select from if set as an option in one of the configuration dictionaries.
             - str : If a string, it is assumed to be a path to a csv file with the subsets. 
                 The first column is assumed to be the name of the subset and the remaining columns are the features in the subset.
             - list or np.ndarray : If a list or np.ndarray, it is assumed to be a list of subsets.
             - None : If None, each column will be treated as a subset. One column will be selected per subset.
             If subsets is None, each column will be treated as a subset. One column will be selected per subset.
@@ -361,97 +364,117 @@
             - type : an type or subclass of a BaseEvolver
             - "nsga2" : tpot2.evolutionary_algorithms.eaNSGA2.eaNSGA2_Evolver
         
         verbose : int, default=1 
             How much information to print during the optimization process. Higher values include the information from lower values.
             0. nothing
             1. progress bar
-            2. evaluations progress bar
+            
             3. best individual
             4. warnings
             >=5. full warnings trace
+            6. evaluations progress bar. (Temporary: This used to be 2. Currently, using evaluation progress bar may prevent some instances were we terminate a generation early due to it reaching max_time_seconds in the middle of a generation OR a pipeline failed to be terminated normally and we need to manually terminate it.)
         
         periodic_checkpoint_folder : str, default=None
             Folder to save the population to periodically. If None, no periodic saving will be done.
             If provided, training will resume from this checkpoint.
         
         callback : tpot2.CallBackInterface, default=None
             Callback object. Not implemented
 
         processes : bool, default=True
             If True, will use multiprocessing to parallelize the optimization process. If False, will use threading.
             True seems to perform better. However, False is required for interactive debugging.
             
+        Attributes
+        ----------
+
+        fitted_pipeline_ : GraphPipeline
+            A fitted instance of the GraphPipeline that inherits from sklearn BaseEstimator. This is fitted on the full X, y passed to fit.
+
+        evaluated_individuals : A pandas data frame containing data for all evaluated individuals in the run. 
+            Columns: 
+            - *objective functions : The first few columns correspond to the passed in scorers and objective functions
+            - Parents : A tuple containing the indexes of the pipelines used to generate the pipeline of that row. If NaN, this pipeline was generated randomly in the initial population.
+            - Variation_Function : Which variation function was used to mutate or crossover the parents. If NaN, this pipeline was generated randomly in the initial population.
+            - Individual : The internal representation of the individual that is used during the evolutionary algorithm. This is not an sklearn BaseEstimator.
+            - Generation : The generation the pipeline first appeared. 
+            - Pareto_Front	: The nondominated front that this pipeline belongs to. 0 means that its scores is not strictly dominated by any other individual. 
+                            To save on computational time, the best frontier is updated iteratively each generation. 
+                            The pipelines with the 0th pareto front do represent the exact best frontier. However, the pipelines with pareto front >= 1 are only in reference to the other pipelines in the final population.
+                            All other pipelines are set to NaN. 
+            - Instance	: The unfitted GraphPipeline BaseEstimator. 
+            - *validation objective functions : Objective function scores evaluated on the validation set.
+            - Validation_Pareto_Front : The full pareto front calculated on the validation set. This is calculated for all pipelines with Pareto_Front equal to 0. Unlike the Pareto_Front which only calculates the frontier and the final population, the Validation Pareto Front is calculated for all pipelines tested on the validation set.
+            
+        pareto_front : The same pandas dataframe as evaluated individuals, but containing only the frontier pareto front pipelines.
         '''
 
         # sklearn BaseEstimator must have a corresponding attribute for each parameter.
         # These should not be modified once set.
+
         self.scorers = scorers
         self.scorers_weights = scorers_weights
         self.classification = classification
-        self.population_size = population_size
-        self.generations = generations
-        self.initial_population_size = initial_population_size
-        self.population_scaling = population_scaling
-        self.generations_until_end_population = generations_until_end_population
-        self.callback = callback
-        self.n_jobs= n_jobs
         self.cv = cv
-        self.verbose = verbose
         self.other_objective_functions = other_objective_functions
         self.other_objective_functions_weights = other_objective_functions_weights
+        self.objective_function_names = objective_function_names
         self.bigger_is_better = bigger_is_better
-        self.evolver = evolver
-
-        self.max_depth = max_depth
         self.max_size = max_size
-        self.max_children = max_children
+        self.linear_pipeline = linear_pipeline
         self.root_config_dict= root_config_dict
         self.inner_config_dict= inner_config_dict
         self.leaf_config_dict= leaf_config_dict
+        self.cross_val_predict_cv = cross_val_predict_cv
+        self.categorical_features = categorical_features
         self.subsets = subsets
-        self.max_time_seconds = max_time_seconds 
-        self.max_eval_time_seconds = max_eval_time_seconds
-        self.memory_limit = memory_limit
-        self.n_initial_optimizations  = n_initial_optimizations  
-        self.optimization_cv  = optimization_cv
-        self.max_optimize_time_seconds = max_optimize_time_seconds 
-        self.optimization_steps = optimization_steps 
-        self.periodic_checkpoint_folder = periodic_checkpoint_folder
-        self.threshold_evaluation_early_stop =threshold_evaluation_early_stop
-        self.threshold_evaluation_scaling =  threshold_evaluation_scaling
-        self.min_history_threshold = min_history_threshold
-        self.selection_evaluation_early_stop = selection_evaluation_early_stop
-        self.selection_evaluation_scaling =  selection_evaluation_scaling
-        self.scorers_early_stop_tol = scorers_early_stop_tol
-        self.other_objectives_early_stop_tol = other_objectives_early_stop_tol
-        self.early_stop = early_stop
-        self.warm_start = warm_start
         self.memory = memory
-        self.cross_val_predict_cv = cross_val_predict_cv
-        self.budget_range = budget_range
-        self.budget_scaling = budget_scaling
-        self.generations_until_end_budget = generations_until_end_budget
         self.preprocessing = preprocessing
         self.validation_strategy = validation_strategy
         self.validation_fraction = validation_fraction
-        self.subset_column = subset_column
-        self.stepwise_steps = stepwise_steps
+        self.population_size = population_size
+        self.initial_population_size = initial_population_size
+        self.population_scaling = population_scaling
+        self.generations_until_end_population = generations_until_end_population
+        self.generations = generations
+        self.early_stop = early_stop
+        self.scorers_early_stop_tol = scorers_early_stop_tol
+        self.other_objectives_early_stop_tol = other_objectives_early_stop_tol
+        self.max_time_seconds = max_time_seconds 
+        self.max_eval_time_seconds = max_eval_time_seconds
+        self.n_jobs= n_jobs
+        self.memory_limit = memory_limit
         self.client = client
-
-        self.survival_selector=survival_selector
-        self.parent_selector=parent_selector
         self.survival_percentage = survival_percentage
         self.crossover_probability = crossover_probability
         self.mutate_probability = mutate_probability
         self.mutate_then_crossover_probability= mutate_then_crossover_probability
         self.crossover_then_mutate_probability= crossover_then_mutate_probability
-
-        self.objective_function_names = objective_function_names
-
+        self.survival_selector=survival_selector
+        self.parent_selector=parent_selector
+        self.budget_range = budget_range
+        self.budget_scaling = budget_scaling
+        self.generations_until_end_budget = generations_until_end_budget
+        self.stepwise_steps = stepwise_steps
+        self.threshold_evaluation_early_stop =threshold_evaluation_early_stop
+        self.threshold_evaluation_scaling =  threshold_evaluation_scaling
+        self.min_history_threshold = min_history_threshold
+        self.selection_evaluation_early_stop = selection_evaluation_early_stop
+        self.selection_evaluation_scaling =  selection_evaluation_scaling
+        self.n_initial_optimizations  = n_initial_optimizations  
+        self.optimization_cv  = optimization_cv
+        self.max_optimize_time_seconds = max_optimize_time_seconds 
+        self.optimization_steps = optimization_steps 
+        self.warm_start = warm_start
+        self.subset_column = subset_column
+        self.evolver = evolver
+        self.verbose = verbose
+        self.periodic_checkpoint_folder = periodic_checkpoint_folder
+        self.callback = callback
         self.processes = processes
 
         #Initialize other used params
 
 
         if self.initial_population_size is None:
             self._initial_population_size = self.population_size
@@ -541,17 +564,33 @@
                 X, X_val, y, y_val = train_test_split(X, y, test_size=self.validation_fraction, stratify=y, random_state=42)
             else:
                 X, X_val, y, y_val = train_test_split(X, y, test_size=self.validation_fraction, random_state=42)
 
 
         X_original = X
         if self.preprocessing:
-            X = pd.DataFrame(X)
-            self._preprocessing_pipeline = sklearn.pipeline.make_pipeline(tpot2.CatImpute(), tpot2.NumericImpute(), tpot2.CatOneHotEncoder(),sklearn.preprocessing.StandardScaler())
-            X = self._preprocessing_pipeline.fit_transform(X)
+            #X = pd.DataFrame(X)
+
+            #TODO: check if there are missing values in X before imputation. If not, don't include imputation in pipeline. Check if there are categorical columns. If not, don't include one hot encoding in pipeline
+            if isinstance(X, pd.DataFrame): #pandas dataframe
+                if self.categorical_features is not None:
+                    X[self.categorical_features] = X[self.categorical_features].astype(object)
+                self._preprocessing_pipeline = sklearn.pipeline.make_pipeline(tpot2.builtin_modules.ColumnSimpleImputer("categorical", strategy='most_frequent'), #impute categorical columns
+                                                                            tpot2.builtin_modules.ColumnSimpleImputer("numeric", strategy='mean'),              #impute numeric columns
+                                                                            tpot2.builtin_modules.ColumnOneHotEncoder("categorical", min_frequency=0.0001))     #one hot encode categorical columns
+                X = self._preprocessing_pipeline.fit_transform(X)
+            else:
+                if self.categorical_features is not None: #numpy array and categorical columns specified
+                    self._preprocessing_pipeline = sklearn.pipeline.make_pipeline(tpot2.builtin_modules.ColumnSimpleImputer(self.categorical_features, strategy='most_frequent'),   #impute categorical columns
+                                                                            tpot2.builtin_modules.ColumnSimpleImputer("all", strategy='mean'),                                      #impute remaining numeric columns
+                                                                            tpot2.builtin_modules.ColumnOneHotEncoder(self.categorical_features, min_frequency=0.0001))             #one hot encode categorical columns
+                else: #numpy array and no categorical columns specified, just do imputation
+                    self._preprocessing_pipeline = sklearn.pipeline.make_pipeline(tpot2.builtin_modules.ColumnSimpleImputer("all", strategy='mean'))   
+
+
         else:
             self._preprocessing_pipeline = None
 
         #_, y = sklearn.utils.check_X_y(X, y, y_numeric=True)
 
         #Set up the configuation dictionaries and the search spaces
 
@@ -566,15 +605,16 @@
         if isinstance(X, pd.DataFrame):
             self.feature_names = X.columns
         else:
             self.feature_names = None
 
         if self.root_config_dict == 'Auto':
             if self.classification:
-                root_config_dict = get_configuration_dictionary("classifiers", n_samples, n_features, self.classification, subsets=self.subsets, feature_names=self.feature_names)
+                n_classes = len(np.unique(y))
+                root_config_dict = get_configuration_dictionary("classifiers", n_samples, n_features, self.classification, subsets=self.subsets, feature_names=self.feature_names, n_classes=n_classes)
             else:
                 root_config_dict = get_configuration_dictionary("regressors", n_samples, n_features, self.classification,subsets=self.subsets, feature_names=self.feature_names)
         else:
             root_config_dict = get_configuration_dictionary(self.root_config_dict, n_samples, n_features, self.classification, subsets=self.subsets,feature_names=self.feature_names)
 
         inner_config_dict = get_configuration_dictionary(self.inner_config_dict, n_samples, n_features, self.classification,subsets=self.subsets, feature_names=self.feature_names)
         leaf_config_dict = get_configuration_dictionary(self.leaf_config_dict, n_samples, n_features, self.classification, subsets=self.subsets, feature_names=self.feature_names)
@@ -601,40 +641,52 @@
             self.cv_gen = sklearn.model_selection.check_cv(self.cv, y, classifier=self.classification)
 
 
         self.individual_generator_instance = tpot2.estimator_graph_individual_generator(   
                                                             inner_config_dict=inner_config_dict,
                                                             root_config_dict=root_config_dict,
                                                             leaf_config_dict=leaf_config_dict,
-                                                            max_depth = self.max_depth,
                                                             max_size = self.max_size,
-                                                            max_children = self.max_children,
+                                                            linear_pipeline=self.linear_pipeline,
                                                                 )
 
         if self.threshold_evaluation_early_stop is not None or self.selection_evaluation_early_stop is not None:
             evaluation_early_stop_steps = self.cv
         else:
             evaluation_early_stop_steps = None
 
 
         X_future = _client.scatter(X)
         y_future = _client.scatter(y)
 
         #.export_pipeline(memory=self.memory, cross_val_predict_cv=self.cross_val_predict_cv, subset_column=self.subset_column),
         #tmp = partial(objective_function_generator, scorers= self._scorers, cv=self.cv_gen, other_objective_functions=self.other_objective_functions )
-        self.final_object_function_list =[ lambda pipeline_individual, X, y,is_classification=self.classification,
-                scorers= self._scorers, cv=self.cv_gen, other_objective_functions=self.other_objective_functions,
-                 memory=self.memory, cross_val_predict_cv=self.cross_val_predict_cv, subset_column=self.subset_column, **kwargs: objective_function_generator(
-                                pipeline_individual,
-                                #ind,
-                                X, y, 
-                                is_classification=is_classification,
-                                scorers= scorers, cv=cv, other_objective_functions=other_objective_functions,
-                                memory=memory, cross_val_predict_cv=cross_val_predict_cv, subset_column=subset_column,
-                                **kwargs,
+        self.final_object_function_list =[ lambda pipeline_individual, 
+                                            X, 
+                                            y,
+                                            is_classification=self.classification,
+                                            scorers= self._scorers, 
+                                            cv=self.cv_gen, 
+                                            other_objective_functions=self.other_objective_functions,
+                                            memory=self.memory, 
+                                            cross_val_predict_cv=self.cross_val_predict_cv, 
+                                            subset_column=self.subset_column, 
+                                            **kwargs: 
+                                            objective_function_generator(
+                                                pipeline_individual,
+                                                X, 
+                                                y, 
+                                                is_classification=is_classification,
+                                                scorers= scorers, 
+                                                cv=cv, 
+                                                other_objective_functions=other_objective_functions,
+                                                memory=memory, 
+                                                cross_val_predict_cv=cross_val_predict_cv, 
+                                                subset_column=subset_column,
+                                                **kwargs,
                                 )]
 
 
         #If warm start and we have an evolver instance, use the existing one
         if not(self.warm_start and self._evolver_instance is not None):
             self._evolver_instance = self._evolver(   individual_generator=self.individual_generator_instance, 
                                             objective_functions=self.final_object_function_list,
@@ -679,71 +731,104 @@
                                             crossover_then_mutate_probability= self.crossover_then_mutate_probability,
                                             
                                             )
 
         
         self._evolver_instance.optimize()
         #self._evolver_instance.population.update_pareto_fronts(self.objective_names, self.objective_function_weights)
-        #self.make_evaluated_individuals()
-
-
-        self.evaluated_individuals = self._evolver_instance.population.evaluated_individuals.copy()
-        self.evaluated_individuals = get_pareto_front(self.evaluated_individuals, self.objective_names, self.objective_function_weights)
+        self.make_evaluated_individuals()
 
         if validation_strategy == 'reshuffled':
             best_pareto_front_idx = list(self.pareto_front.index)
-            best_pareto_front = self.pareto_front.loc[best_pareto_front_idx]['Instance']
+            best_pareto_front = list(self.pareto_front.loc[best_pareto_front_idx]['Individual'])
             
             #reshuffle rows
             X, y = sklearn.utils.shuffle(X, y, random_state=1)
             X_future = _client.scatter(X)
             y_future = _client.scatter(y)
 
-            val_objective_function_list = [lambda ind, X, y, is_classification=self.classification,scorers= self._scorers, cv=self.cv_gen, other_objective_functions=self.other_objective_functions, **kwargs: objective_function_generator(
+            val_objective_function_list = [lambda   ind, 
+                                                    X, 
+                                                    y, 
+                                                    is_classification=self.classification,
+                                                    scorers= self._scorers, 
+                                                    cv=self.cv_gen, 
+                                                    other_objective_functions=self.other_objective_functions, 
+                                                    memory=self.memory, 
+                                                    cross_val_predict_cv=self.cross_val_predict_cv, 
+                                                    subset_column=self.subset_column, 
+                                                    **kwargs: objective_function_generator(
                                                                                                 ind,
-                                                                                                X,y, 
+                                                                                                X,
+                                                                                                y, 
                                                                                                 is_classification=is_classification,
-                                                                                                scorers= scorers, cv=cv, other_objective_functions=other_objective_functions,
+                                                                                                scorers= scorers, 
+                                                                                                cv=cv, 
+                                                                                                other_objective_functions=other_objective_functions,
+                                                                                                memory=memory, 
+                                                                                                cross_val_predict_cv=cross_val_predict_cv, 
+                                                                                                subset_column=subset_column,
                                                                                                 **kwargs,
                                                                                                 )]
             
+            objective_kwargs = {"X": X_future, "y": y_future}
             val_scores = tpot2.objectives.parallel_eval_objective_list(
                 best_pareto_front,
-                val_objective_function_list, n_jobs=self.n_jobs, verbose=self.verbose, timeout=self.max_eval_time_seconds,n_expected_columns=len(self.objective_names), client=_client, X= X_future, y= y_future)
+                val_objective_function_list, n_jobs=self.n_jobs, verbose=self.verbose, timeout=self.max_eval_time_seconds,n_expected_columns=len(self.objective_names), client=_client, **objective_kwargs)
 
             val_objective_names = ['validation_'+name for name in self.objective_names]
             self.objective_names_for_selection = val_objective_names
             self.evaluated_individuals.loc[best_pareto_front_idx,val_objective_names] = val_scores
 
+            self.evaluated_individuals["Validation_Pareto_Front"] = tpot2.get_pareto_front(self.evaluated_individuals, val_objective_names, self.objective_function_weights, invalid_values=["TIMEOUT","INVALID"])
+
         elif validation_strategy == 'split':
 
             
             X_future = _client.scatter(X)
             y_future = _client.scatter(y)
             X_val_future = _client.scatter(X_val)
             y_val_future = _client.scatter(y_val)
 
-
+            objective_kwargs = {"X": X_future, "y": y_future, "X_val" : X_val_future, "y_val":y_val_future }
+            
             best_pareto_front_idx = list(self.pareto_front.index)
-            best_pareto_front = self.pareto_front.loc[best_pareto_front_idx]['Instance']
-            val_objective_function_list = [lambda ind, X, y, X_val, y_val, scorers= self._scorers, other_objective_functions=self.other_objective_functions, **kwargs: val_objective_function_generator(
-                ind,
-                X,y,
-                X_val, y_val, 
-                scorers= scorers, other_objective_functions=other_objective_functions,
-                **kwargs,
-                )]
+            best_pareto_front = list(self.pareto_front.loc[best_pareto_front_idx]['Individual'])
+            val_objective_function_list = [lambda   ind, 
+                                                    X, 
+                                                    y, 
+                                                    X_val, 
+                                                    y_val, 
+                                                    scorers= self._scorers, 
+                                                    other_objective_functions=self.other_objective_functions, 
+                                                    memory=self.memory, 
+                                                    cross_val_predict_cv=self.cross_val_predict_cv, 
+                                                    subset_column=self.subset_column, 
+                                                    **kwargs: val_objective_function_generator(
+                                                        ind,
+                                                        X,
+                                                        y,
+                                                        X_val, 
+                                                        y_val, 
+                                                        scorers= scorers, 
+                                                        other_objective_functions=other_objective_functions,
+                                                        memory=memory, 
+                                                        cross_val_predict_cv=cross_val_predict_cv, 
+                                                        subset_column=subset_column,
+                                                        **kwargs,
+                                                        )]
             
             val_scores = tpot2.objectives.parallel_eval_objective_list(
                 best_pareto_front,
-                val_objective_function_list, n_jobs=self.n_jobs, verbose=self.verbose, timeout=self.max_eval_time_seconds,n_expected_columns=len(self.objective_names),client=_client, X=X_future, y=y_future, X_val=X_val_future, y_val=y_val_future)
+                val_objective_function_list, n_jobs=self.n_jobs, verbose=self.verbose, timeout=self.max_eval_time_seconds,n_expected_columns=len(self.objective_names),client=_client, **objective_kwargs)
 
             val_objective_names = ['validation_'+name for name in self.objective_names]
             self.objective_names_for_selection = val_objective_names
             self.evaluated_individuals.loc[best_pareto_front_idx,val_objective_names] = val_scores
+            self.evaluated_individuals["Validation_Pareto_Front"] = tpot2.get_pareto_front(self.evaluated_individuals, val_objective_names, self.objective_function_weights, invalid_values=["TIMEOUT","INVALID"])
         else:
             self.objective_names_for_selection = self.objective_names
 
         val_scores = self.evaluated_individuals[~self.evaluated_individuals[self.objective_names_for_selection].isin(["TIMEOUT","INVALID"]).any(axis=1)][self.objective_names_for_selection].astype(float)                                     
         weighted_scores = val_scores*self.objective_function_weights
         
         if self.bigger_is_better:
@@ -759,16 +844,15 @@
 
         if self.preprocessing:
             self.fitted_pipeline_ = sklearn.pipeline.make_pipeline(sklearn.base.clone(self._preprocessing_pipeline), best_individual_pipeline )
         else:
             self.fitted_pipeline_ = best_individual_pipeline 
         
         self.fitted_pipeline_.fit(X_original,y) #TODO use y_original as well?
-        if self.verbose >= 3:
-            best_individual.plot()
+
 
         if self.client is None: #no client was passed in
             #close cluster and client
             _client.close()
             cluster.close()
 
         return self
@@ -838,39 +922,14 @@
         else:
             if "Pareto_Front" not in self.evaluated_individuals:
                 return self.evaluated_individuals
             else:
                 return self.evaluated_individuals[self.evaluated_individuals["Pareto_Front"]==0]
 
 
-def get_pareto_front(df, column_names, weights, invalid_values=["TIMEOUT","INVALID"], inplace=True, top=None):
-    dftmp = df[~df[column_names].isin(invalid_values).any(axis=1)]
-
-    if "Budget" in dftmp.columns:
-        #get rows with the max budget
-        dftmp = dftmp[dftmp["Budget"]==dftmp["Budget"].max()]
-
-
-    indeces = dftmp[~dftmp[column_names].isna().any(axis=1)].index.values
-    weighted_scores = df.loc[indeces][column_names].to_numpy()  * weights
-
-    pareto_fronts = tpot2.parent_selectors.nondominated_sorting(weighted_scores)
-
-    if not inplace:
-        df = pd.DataFrame(index=df.index,columns=["Pareto_Front"], data=[])
-    
-    df["Pareto_Front"] = np.nan
-
-    for i, front in enumerate(pareto_fronts):
-        for index in front:
-            df.loc[indeces[index], "Pareto_Front"] = i
-
-    return df
-
-
 def _convert_parents_tuples_to_integers(row, object_to_int):
     if type(row) == list or type(row) == np.ndarray or type(row) == tuple:
         return tuple(object_to_int[obj] for obj in row)
     else:
         return np.nan
 
 def _apply_make_pipeline(graphindividual, preprocessing_pipeline=None):
@@ -878,15 +937,15 @@
         if preprocessing_pipeline is None:
             return graphindividual.export_pipeline()
         else:
             return sklearn.pipeline.make_pipeline(sklearn.base.clone(preprocessing_pipeline), graphindividual.export_pipeline())
     except:
         return None
 
-def get_configuration_dictionary(options, n_samples, n_features, classification, subsets=None, feature_names=None):
+def get_configuration_dictionary(options, n_samples, n_features, classification, subsets=None, feature_names=None, n_classes=None):
     if options is None:
         return options
 
     if isinstance(options, dict):
         return recursive_with_defaults(options, n_samples, n_features, classification, subsets=subsets, feature_names=feature_names)
     
     if not isinstance(options, list):
@@ -896,15 +955,15 @@
 
     for option in options:
 
         if option == "selectors":
             config_dict.update(tpot2.config.make_selector_config_dictionary(classification))
 
         elif option == "classifiers":
-            config_dict.update(tpot2.config.make_classifier_config_dictionary(n_samples=n_samples))
+            config_dict.update(tpot2.config.make_classifier_config_dictionary(n_samples=n_samples, n_classes=n_classes))
 
         elif option == "regressors":
             config_dict.update(tpot2.config.make_regressor_config_dictionary(n_samples=n_samples))
 
         elif option == "transformers":
             config_dict.update(tpot2.config.make_transformer_config_dictionary(n_features=n_features))
         
@@ -973,22 +1032,21 @@
         #flatten
         other_scores = np.array(other_scores).flatten().tolist()
     else:
         other_scores = []
         
     return np.concatenate([cv_obj_scores,other_scores])
 
-
-def val_objective_function_generator(pipeline, X_train, y_train, X_test, y_test, scorers, other_objective_functions, memory=None, cross_val_predict_cv=None, subset_column=None, ):
+def val_objective_function_generator(pipeline, X_train, y_train, X_test, y_test, scorers, other_objective_functions, memory, cross_val_predict_cv, subset_column):
     #subsample the data
     pipeline = pipeline.export_pipeline(memory=memory, cross_val_predict_cv=cross_val_predict_cv, subset_column=subset_column)
     fitted_pipeline = sklearn.base.clone(pipeline)
     fitted_pipeline.fit(X_train, y_train)
 
-    this_fold_scores = [sklearn.metrics.get_scorer(scorer)(fitted_pipeline, X_test, y_test) for scorer in scorers] 
-    
+    if len(scorers) > 0:
+        scores =[sklearn.metrics.get_scorer(scorer)(fitted_pipeline, X_test, y_test) for scorer in scorers] 
+
     other_scores = []
-    #TODO use same exported pipeline as for each objective
     if other_objective_functions is not None and len(other_objective_functions) >0:
         other_scores = [obj(sklearn.base.clone(pipeline)) for obj in other_objective_functions]
     
-    return np.concatenate([this_fold_scores,other_scores])
+    return np.concatenate([scores,other_scores])
```

### Comparing `TPOT2-0.1.1a0/tpot2/tpot_estimator/templates/tpottemplates.py` & `TPOT2-0.1.2a0/tpot2/tpot_estimator/templates/tpottemplates.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,21 +11,21 @@
                         scorers_weights=[1],
                         classification=False,
                         cv=5,
                         other_objective_functions=[tpot2.estimator_objective_functions.average_path_length_objective], #tpot2.estimator_objective_functions.number_of_nodes_objective],
                         other_objective_functions_weights=[-1],
                         objective_function_names=None,
                         bigger_is_better=True,
-                        max_depth=np.inf,
                         max_size=np.inf, 
-                        max_children=np.inf,
+                        linear_pipeline=False,
                         root_config_dict='Auto',
                         inner_config_dict=["selectors", "transformers"],
                         leaf_config_dict=None,                        
                         cross_val_predict_cv=0,
+                        categorical_features = None,
                         subsets=None,
                         memory=None,
                         preprocessing=False,  
                         validation_strategy="none",
                         validation_fraction=.2,
                         population_size=50,
                         initial_population_size=None,
@@ -73,21 +73,21 @@
             scorers_weights=scorers_weights,
             classification=classification,
             cv=cv,
             other_objective_functions=other_objective_functions, #tpot2.estimator_objective_functions.number_of_nodes_objective],
             other_objective_functions_weights=other_objective_functions_weights,
             objective_function_names=objective_function_names,
             bigger_is_better=bigger_is_better,
-            max_depth=max_depth,
             max_size=max_size, 
-            max_children=max_children,
+            linear_pipeline=linear_pipeline,
             root_config_dict=root_config_dict,
             inner_config_dict=inner_config_dict,
             leaf_config_dict=leaf_config_dict,                        
             cross_val_predict_cv=cross_val_predict_cv,
+            categorical_features = categorical_features,
             subsets=subsets,
             memory=memory,
             preprocessing=preprocessing,  
             validation_strategy=validation_strategy,
             validation_fraction=validation_fraction,
             population_size=population_size,
             initial_population_size=initial_population_size,
@@ -138,21 +138,22 @@
                         scorers_weights=[1],
                         classification=True,
                         cv=5,
                         other_objective_functions=[tpot2.estimator_objective_functions.average_path_length_objective], #tpot2.estimator_objective_functions.number_of_nodes_objective],
                         other_objective_functions_weights=[-1],
                         objective_function_names=None,
                         bigger_is_better=True,
-                        max_depth=np.inf,
+                        
                         max_size=np.inf, 
-                        max_children=np.inf,
+                        linear_pipeline=False,
                         root_config_dict='Auto',
                         inner_config_dict=["selectors", "transformers"],
                         leaf_config_dict=None,                        
                         cross_val_predict_cv=0,
+                        categorical_features = None,
                         subsets=None,
                         memory=None,
                         preprocessing=False,  
                         validation_strategy="none",
                         validation_fraction=.2,
                         population_size=50,
                         initial_population_size=None,
@@ -200,21 +201,22 @@
             scorers_weights=scorers_weights,
             classification=classification,
             cv=cv,
             other_objective_functions=other_objective_functions, #tpot2.estimator_objective_functions.number_of_nodes_objective],
             other_objective_functions_weights=other_objective_functions_weights,
             objective_function_names=objective_function_names,
             bigger_is_better=bigger_is_better,
-            max_depth=max_depth,
+           
             max_size=max_size, 
-            max_children=max_children,
+            linear_pipeline=linear_pipeline,
             root_config_dict=root_config_dict,
             inner_config_dict=inner_config_dict,
             leaf_config_dict=leaf_config_dict,                        
             cross_val_predict_cv=cross_val_predict_cv,
+            categorical_features = categorical_features,
             subsets=subsets,
             memory=memory,
             preprocessing=preprocessing,  
             validation_strategy=validation_strategy,
             validation_fraction=validation_fraction,
             population_size=population_size,
             initial_population_size=initial_population_size,
```


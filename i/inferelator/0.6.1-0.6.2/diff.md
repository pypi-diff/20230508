# Comparing `tmp/inferelator-0.6.1.tar.gz` & `tmp/inferelator-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/chris/PycharmProjects/inferelator/dist/.tmp-z1r7x3rx/inferelator-0.6.1.tar", last modified: Tue Jan  3 17:26:39 2023, max compression
+gzip compressed data, was "/home/chris/PycharmProjects/inferelator/dist/.tmp-b4xsterv/inferelator-0.6.2.tar", last modified: Mon May  8 19:24:20 2023, max compression
```

## Comparing `inferelator-0.6.1.tar` & `inferelator-0.6.2.tar`

### file list

```diff
@@ -1,88 +1,94 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.488986 inferelator-0.6.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1368 2021-09-29 15:35:11.000000 inferelator-0.6.1/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     3234 2023-01-03 17:26:39.484986 inferelator-0.6.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     2633 2023-01-03 17:25:48.000000 inferelator-0.6.1/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.476986 inferelator-0.6.1/inferelator/
--rw-rw-r--   0 chris     (1000) chris     (1000)      723 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.476986 inferelator-0.6.1/inferelator/benchmarking/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2021-08-13 20:14:01.000000 inferelator-0.6.1/inferelator/benchmarking/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4907 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/benchmarking/celloracle.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7292 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/benchmarking/scenic.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    21630 2021-09-29 15:35:11.000000 inferelator-0.6.1/inferelator/crossvalidation_workflow.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.476986 inferelator-0.6.1/inferelator/distributed/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2313 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8444 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/dask.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    18110 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/dask_cluster_controller.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      251 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/dask_k8_controller.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2105 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/dask_local_controller.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5500 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/inferelator_mp.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1480 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/joblib_controller.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1307 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/distributed/local_controller.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.480986 inferelator-0.6.1/inferelator/postprocessing/
--rw-rw-r--   0 chris     (1000) chris     (1000)      395 2020-12-07 20:06:39.000000 inferelator-0.6.1/inferelator/postprocessing/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      731 2020-12-07 20:06:39.000000 inferelator-0.6.1/inferelator/postprocessing/column_names.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3850 2021-09-29 15:35:11.000000 inferelator-0.6.1/inferelator/postprocessing/f1_score.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7342 2021-09-29 15:35:11.000000 inferelator-0.6.1/inferelator/postprocessing/inferelator_results.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4460 2021-09-29 15:35:11.000000 inferelator-0.6.1/inferelator/postprocessing/matthews_correlation.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5423 2021-09-29 15:35:11.000000 inferelator-0.6.1/inferelator/postprocessing/model_metrics.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10761 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/postprocessing/model_performance.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6720 2021-09-29 15:35:11.000000 inferelator-0.6.1/inferelator/postprocessing/precision_recall.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10896 2021-02-05 16:50:26.000000 inferelator-0.6.1/inferelator/postprocessing/results_processor.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8726 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/postprocessing/results_processor_mtl.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.480986 inferelator-0.6.1/inferelator/preprocessing/
--rw-rw-r--   0 chris     (1000) chris     (1000)      126 2022-09-14 18:35:03.000000 inferelator-0.6.1/inferelator/preprocessing/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9321 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/preprocessing/design_response_translation.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14408 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/preprocessing/metadata_parser.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    15286 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/preprocessing/priors.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3689 2021-02-05 16:50:26.000000 inferelator-0.6.1/inferelator/preprocessing/simulate_data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6354 2020-12-07 20:06:39.000000 inferelator-0.6.1/inferelator/preprocessing/single_cell.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       84 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/preprocessing/tfa.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6341 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/preprocessing/velocity.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.484986 inferelator-0.6.1/inferelator/regression/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-06-04 16:11:42.000000 inferelator-0.6.1/inferelator/regression/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    20677 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/regression/amusr_math.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    16644 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/regression/amusr_regression.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9875 2022-12-09 19:08:13.000000 inferelator-0.6.1/inferelator/regression/base_regression.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10271 2021-09-27 14:15:05.000000 inferelator-0.6.1/inferelator/regression/bayes_stats.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1924 2022-03-03 16:16:38.000000 inferelator-0.6.1/inferelator/regression/bbsr_multitask.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9671 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/regression/bbsr_python.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1530 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/regression/elasticnet_python.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8912 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/regression/mi.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6687 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/regression/sklearn_regression.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12460 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/regression/stability_selection.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.472986 inferelator-0.6.1/inferelator/tests/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.484986 inferelator-0.6.1/inferelator/tests/artifacts/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-06-04 16:11:42.000000 inferelator-0.6.1/inferelator/tests/artifacts/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2277 2022-03-03 16:16:38.000000 inferelator-0.6.1/inferelator/tests/artifacts/test_data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3334 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/tests/artifacts/test_stubs.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.484986 inferelator-0.6.1/inferelator/tfa/
--rw-rw-r--   0 chris     (1000) chris     (1000)       79 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/tfa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2176 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/tfa/pinv_tfa.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/tfa/ridge_tfa.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6684 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/tfa/tfa_base.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4204 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/tfa/velocity_tfa.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.484986 inferelator-0.6.1/inferelator/utils/
--rw-rw-r--   0 chris     (1000) chris     (1000)      453 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/utils/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    38628 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/utils/data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2271 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/utils/debug.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17587 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/utils/loader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1284 2021-05-03 23:10:24.000000 inferelator-0.6.1/inferelator/utils/profiler.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12946 2020-06-04 16:11:42.000000 inferelator-0.6.1/inferelator/utils/validator.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7801 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/workflow.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.484986 inferelator-0.6.1/inferelator/workflows/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/workflows/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    28161 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/workflows/amusr_workflow.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4166 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/workflows/homology_workflow.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3794 2022-09-14 16:51:32.000000 inferelator-0.6.1/inferelator/workflows/single_cell_workflow.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10572 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/workflows/tfa_workflow.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12483 2023-01-03 17:25:51.000000 inferelator-0.6.1/inferelator/workflows/velocity_workflow.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    46309 2023-01-03 17:26:06.000000 inferelator-0.6.1/inferelator/workflows/workflow_base.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-01-03 17:26:39.476986 inferelator-0.6.1/inferelator.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     3234 2023-01-03 17:26:39.000000 inferelator-0.6.1/inferelator.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     2731 2023-01-03 17:26:39.000000 inferelator-0.6.1/inferelator.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-01-03 17:26:39.000000 inferelator-0.6.1/inferelator.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2019-09-06 16:51:36.000000 inferelator-0.6.1/inferelator.egg-info/not-zip-safe
--rw-r--r--   0 chris     (1000) chris     (1000)       86 2023-01-03 17:26:39.000000 inferelator-0.6.1/inferelator.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       12 2023-01-03 17:26:39.000000 inferelator-0.6.1/inferelator.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-01-03 17:26:39.488986 inferelator-0.6.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     1388 2023-01-03 17:25:51.000000 inferelator-0.6.1/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.246469 inferelator-0.6.2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1368 2021-09-29 15:35:11.000000 inferelator-0.6.2/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3234 2023-05-08 19:24:20.246469 inferelator-0.6.2/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2633 2023-05-08 19:22:15.000000 inferelator-0.6.2/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.234469 inferelator-0.6.2/inferelator/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      810 2023-02-07 19:27:51.000000 inferelator-0.6.2/inferelator/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.238469 inferelator-0.6.2/inferelator/benchmarking/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2021-08-13 20:14:01.000000 inferelator-0.6.2/inferelator/benchmarking/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5315 2023-02-06 19:10:19.000000 inferelator-0.6.2/inferelator/benchmarking/celloracle.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7340 2023-02-06 19:13:39.000000 inferelator-0.6.2/inferelator/benchmarking/scenic.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    21630 2023-05-08 19:22:24.000000 inferelator-0.6.2/inferelator/crossvalidation_workflow.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.238469 inferelator-0.6.2/inferelator/distributed/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2313 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/distributed/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8444 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/distributed/dask.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18367 2023-02-07 18:51:05.000000 inferelator-0.6.2/inferelator/distributed/dask_cluster_controller.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      251 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/distributed/dask_k8_controller.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2105 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/distributed/dask_local_controller.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5500 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/distributed/inferelator_mp.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1480 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/distributed/joblib_controller.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1307 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/distributed/local_controller.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.238469 inferelator-0.6.2/inferelator/postprocessing/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      395 2020-12-07 20:06:39.000000 inferelator-0.6.2/inferelator/postprocessing/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      810 2023-02-06 16:33:23.000000 inferelator-0.6.2/inferelator/postprocessing/column_names.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3850 2021-09-29 15:35:11.000000 inferelator-0.6.2/inferelator/postprocessing/f1_score.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12223 2023-05-08 18:53:52.000000 inferelator-0.6.2/inferelator/postprocessing/inferelator_results.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4460 2021-09-29 15:35:11.000000 inferelator-0.6.2/inferelator/postprocessing/matthews_correlation.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5423 2021-09-29 15:35:11.000000 inferelator-0.6.2/inferelator/postprocessing/model_metrics.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10839 2023-02-23 17:39:18.000000 inferelator-0.6.2/inferelator/postprocessing/model_performance.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6720 2021-09-29 15:35:11.000000 inferelator-0.6.2/inferelator/postprocessing/precision_recall.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10467 2023-02-23 17:04:57.000000 inferelator-0.6.2/inferelator/postprocessing/results_processor.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9384 2023-02-06 19:20:39.000000 inferelator-0.6.2/inferelator/postprocessing/results_processor_mtl.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.238469 inferelator-0.6.2/inferelator/predict/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       96 2023-02-24 16:07:22.000000 inferelator-0.6.2/inferelator/predict/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4904 2023-05-08 19:22:24.000000 inferelator-0.6.2/inferelator/predict/dynamic.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8676 2023-05-08 19:22:24.000000 inferelator-0.6.2/inferelator/predict/static.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.242469 inferelator-0.6.2/inferelator/preprocessing/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      123 2023-02-09 18:22:12.000000 inferelator-0.6.2/inferelator/preprocessing/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9373 2023-02-23 17:56:12.000000 inferelator-0.6.2/inferelator/preprocessing/data_normalization.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9321 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/preprocessing/design_response_translation.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14408 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/preprocessing/metadata_parser.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    20063 2023-02-07 16:06:43.000000 inferelator-0.6.2/inferelator/preprocessing/priors.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3689 2021-02-05 16:50:26.000000 inferelator-0.6.2/inferelator/preprocessing/simulate_data.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6354 2020-12-07 20:06:39.000000 inferelator-0.6.2/inferelator/preprocessing/single_cell.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)       84 2023-01-03 17:25:51.000000 inferelator-0.6.2/inferelator/preprocessing/tfa.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8588 2023-02-22 15:42:41.000000 inferelator-0.6.2/inferelator/preprocessing/velocity.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.242469 inferelator-0.6.2/inferelator/regression/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-06-04 16:11:42.000000 inferelator-0.6.2/inferelator/regression/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    20677 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/regression/amusr_math.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    16884 2023-02-07 17:59:13.000000 inferelator-0.6.2/inferelator/regression/amusr_regression.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10807 2023-02-08 18:08:17.000000 inferelator-0.6.2/inferelator/regression/base_regression.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10271 2021-09-27 14:15:05.000000 inferelator-0.6.2/inferelator/regression/bayes_stats.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2559 2023-02-06 19:47:26.000000 inferelator-0.6.2/inferelator/regression/bbsr_multitask.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10602 2023-02-07 17:47:48.000000 inferelator-0.6.2/inferelator/regression/bbsr_python.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1530 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/regression/elasticnet_python.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8912 2023-01-03 17:25:51.000000 inferelator-0.6.2/inferelator/regression/mi.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7321 2023-02-07 18:01:32.000000 inferelator-0.6.2/inferelator/regression/sklearn_regression.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12322 2023-02-07 17:34:16.000000 inferelator-0.6.2/inferelator/regression/stability_selection.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.234469 inferelator-0.6.2/inferelator/tests/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.242469 inferelator-0.6.2/inferelator/tests/artifacts/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-06-04 16:11:42.000000 inferelator-0.6.2/inferelator/tests/artifacts/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2277 2022-03-03 16:16:38.000000 inferelator-0.6.2/inferelator/tests/artifacts/test_data.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3357 2023-02-06 19:12:04.000000 inferelator-0.6.2/inferelator/tests/artifacts/test_stubs.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.242469 inferelator-0.6.2/inferelator/tfa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       79 2023-01-03 17:25:51.000000 inferelator-0.6.2/inferelator/tfa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1012 2023-02-09 18:31:30.000000 inferelator-0.6.2/inferelator/tfa/pinv_tfa.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-01-03 17:25:51.000000 inferelator-0.6.2/inferelator/tfa/ridge_tfa.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7310 2023-02-09 18:35:48.000000 inferelator-0.6.2/inferelator/tfa/tfa_base.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4204 2023-01-03 17:25:51.000000 inferelator-0.6.2/inferelator/tfa/velocity_tfa.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.242469 inferelator-0.6.2/inferelator/utils/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      481 2023-02-23 17:50:54.000000 inferelator-0.6.2/inferelator/utils/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10831 2023-02-23 17:48:02.000000 inferelator-0.6.2/inferelator/utils/data.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3128 2023-02-06 15:49:05.000000 inferelator-0.6.2/inferelator/utils/debug.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    30766 2023-05-08 18:55:30.000000 inferelator-0.6.2/inferelator/utils/inferelator_data.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    19259 2023-02-22 20:08:42.000000 inferelator-0.6.2/inferelator/utils/loader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1284 2021-05-03 23:10:24.000000 inferelator-0.6.2/inferelator/utils/profiler.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12912 2023-02-06 15:58:11.000000 inferelator-0.6.2/inferelator/utils/validator.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7823 2023-02-06 16:12:27.000000 inferelator-0.6.2/inferelator/workflow.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.246469 inferelator-0.6.2/inferelator/workflows/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-09-14 16:51:32.000000 inferelator-0.6.2/inferelator/workflows/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    29136 2023-02-23 17:39:49.000000 inferelator-0.6.2/inferelator/workflows/amusr_workflow.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4166 2023-01-03 17:25:51.000000 inferelator-0.6.2/inferelator/workflows/homology_workflow.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3963 2023-02-06 18:03:06.000000 inferelator-0.6.2/inferelator/workflows/single_cell_workflow.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10868 2023-02-06 17:53:58.000000 inferelator-0.6.2/inferelator/workflows/tfa_workflow.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12483 2023-01-03 17:25:51.000000 inferelator-0.6.2/inferelator/workflows/velocity_workflow.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    46788 2023-02-06 20:59:42.000000 inferelator-0.6.2/inferelator/workflows/workflow_base.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-08 19:24:20.234469 inferelator-0.6.2/inferelator.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     3234 2023-05-08 19:24:20.000000 inferelator-0.6.2/inferelator.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     2910 2023-05-08 19:24:20.000000 inferelator-0.6.2/inferelator.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-05-08 19:24:20.000000 inferelator-0.6.2/inferelator.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2019-09-06 16:51:36.000000 inferelator-0.6.2/inferelator.egg-info/not-zip-safe
+-rw-r--r--   0 chris     (1000) chris     (1000)       86 2023-05-08 19:24:20.000000 inferelator-0.6.2/inferelator.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       12 2023-05-08 19:24:20.000000 inferelator-0.6.2/inferelator.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-08 19:24:20.246469 inferelator-0.6.2/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1389 2023-05-08 19:23:38.000000 inferelator-0.6.2/setup.py
```

### Comparing `inferelator-0.6.1/LICENSE` & `inferelator-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/PKG-INFO` & `inferelator-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferelator
-Version: 0.6.1
+Version: 0.6.2
 Summary: Inferelator: Network Inference
 Home-page: https://github.com/flatironinstitute/inferelator
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 Maintainer: Chris Jackson
 Maintainer-email: cj59@nyu.edu
 Project-URL: Documentation, https://inferelator.readthedocs.io/
```

### Comparing `inferelator-0.6.1/README.md` & `inferelator-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/__init__.py` & `inferelator-0.6.2/inferelator/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,8 +7,15 @@
 os.environ["OPENBLAS_NUM_THREADS"] = os.environ.get("OPENBLAS_NUM_THREADS", "1")
 
 from inferelator.workflow import inferelator_workflow
 from inferelator.crossvalidation_workflow import CrossValidationManager
 from inferelator.utils import inferelator_verbose_level
 from inferelator.distributed.inferelator_mp import MPControl
 
-from inferelator.workflows import amusr_workflow, single_cell_workflow, tfa_workflow, velocity_workflow
+from inferelator.workflows import (
+    amusr_workflow,
+    single_cell_workflow,
+    tfa_workflow,
+    velocity_workflow
+)
+
+from inferelator.regression.base_regression import PreprocessData
```

### Comparing `inferelator-0.6.1/inferelator/benchmarking/celloracle.py` & `inferelator-0.6.2/inferelator/benchmarking/celloracle.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,18 +80,33 @@
         base_GRN.drop("value", axis=1, inplace=True)
         return {k: v["Regulator"].tolist() for k, v in base_GRN.groupby("Target")}
 
 
     @staticmethod
     def reprocess_co_output_to_inferelator_results(co_out):
 
-        betas = [r.pivot(index='target', columns='source', values='coef_mean').fillna(0) for k, r in co_out.items()]
-        rankers = [r.pivot(index='target', columns='source', values='-logp').fillna(0) for k, r in co_out.items()]
+        betas = [
+            r.pivot(
+                index='target',
+                columns='source',
+                values='coef_mean'
+            ).fillna(0)
+            for k, r in co_out.items()
+        ]
+
+        rankers = [
+            r.pivot(
+                index='target',
+                columns='source',
+                values='-logp'
+            ).fillna(0)
+            for k, r in co_out.items()
+        ]
 
-        return betas, rankers
+        return betas, rankers, betas[0], rankers[0]
 
 
 class CellOracleRegression(_RegressionWorkflowMixin):
 
     oracle_imputation = True
 
     def run_regression(self):
@@ -104,40 +119,54 @@
                                            cluster_column_name="louvain",
                                            embedding_name="X_pca")
 
         # Apparently PCA is not transferred from the adata object
         oracle.perform_PCA(100)
 
         # Add prior
-        oracle.addTFinfo_dictionary(self.reprocess_prior_to_base_GRN(self.priors_data))
+        oracle.addTFinfo_dictionary(
+            self.reprocess_prior_to_base_GRN(self.priors_data)
+        )
 
         utils.Debug.vprint("Imputation Preprocessing")
 
         if self.oracle_imputation:
 
             # Heuristics from Celloracle documentation
-            n_comps = np.where(np.diff(np.diff(np.cumsum(oracle.pca.explained_variance_ratio_))>0.002))[0][0]
+            n_comps = np.where(
+                np.diff(
+                    np.diff(
+                        np.cumsum(oracle.pca.explained_variance_ratio_)
+                    ) > 0.002
+                )
+            )[0][0]
+
             k = int(0.025 * oracle.adata.shape[0])
 
             # Make sure n_comps is between 10 and 50
             # It likes to go to 0 for noise controls
             n_comps = max(min(n_comps, 50), 10)
 
             # Make sure k is at least 25 too I guess
             k = max(k, 25)
 
-            oracle.knn_imputation(n_pca_dims=n_comps, k=k, balanced=True, b_sight=k*8,
-                                b_maxl=k*4, n_jobs=4)
+            oracle.knn_imputation(
+                n_pca_dims=n_comps,
+                k=k, balanced=True,
+                b_sight=k*8,
+                b_maxl=k*4,
+                n_jobs=4
+            )
 
         # Pretend to do imputation
         else:
             oracle.adata.layers["imputed_count"] = oracle.adata.layers["normalized_count"].copy()
 
         utils.Debug.vprint("CellOracle GRN inference")
-        
+
         # Call GRN inference
         links = oracle.get_links(cluster_name_for_GRN_unit="louvain", alpha=10,
                                  verbose_level=0, test_mode=False)
 
         # Deepcopy the result dict that we want
         result = copy.deepcopy(links.links_dict)
```

### Comparing `inferelator-0.6.1/inferelator/benchmarking/scenic.py` & `inferelator-0.6.2/inferelator/benchmarking/scenic.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,21 +189,21 @@
             mat = [pd.DataFrame(data).set_index(0).rename({1: tf}, axis=1)
                     for tf, data in scenic_df['TargetGenes'].iteritems()]
 
             mat = pd.concat(mat, axis=0).fillna(0)
             mat = mat.groupby(mat.index).agg('max')
             mat = mat.reindex(prior_data.columns, axis=1).reindex(prior_data.index, axis=0).fillna(0)
     
-        return [mat], [mat.copy()]
+        return [mat], [mat.copy()], mat.copy(), mat.copy()
 
     @staticmethod
     def reprocess_adj_to_inferelator_results(adj):
         mat = adj.pivot(index='target', columns='TF', values='importance').fillna(0.)
 
-        return [mat], [mat.copy()]
+        return [mat], [mat.copy()], mat.copy(), mat.copy()
 
 # This code is lifted from https://github.com/aertslab/create_cisTarget_databases/cistarget_db.py
 # It is not reimplemented in order to ensure that the methodology for ranking is identical
 # There's no license on this code so this is just straight up theft
 # Maybe put licenses on your academic code?
 # You can have it back if you want. I really don't want it.
```

### Comparing `inferelator-0.6.1/inferelator/crossvalidation_workflow.py` & `inferelator-0.6.2/inferelator/crossvalidation_workflow.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/distributed/__init__.py` & `inferelator-0.6.2/inferelator/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/distributed/dask.py` & `inferelator-0.6.2/inferelator/distributed/dask.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/distributed/dask_cluster_controller.py` & `inferelator-0.6.2/inferelator/distributed/dask_cluster_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,18 +188,18 @@
                 project=cls._project,
                 interface=cls._interface,
                 walltime=cls._job_time,
                 job_cpu=cls._job_n_workers * cls._worker_n_threads,
                 cores=cls._job_n_workers * cls._worker_n_threads,
                 processes=cls._job_n_workers,
                 job_mem=cls._job_mem,
-                env_extra=cls._config_env(),
+                job_script_prologue=cls._config_env(),
                 local_directory=cls._local_directory,
                 memory=cls._job_mem,
-                job_extra=cls._job_slurm_commands,
+                job_extra_directives=cls._job_slurm_commands,
                 job_cls=SLURMJobNoMemLimit,
                 **kwargs
             )
 
             cls.client = distributed.Client(
                 cls.local_cluster,
                 direct_to_workers=True
@@ -471,66 +471,80 @@
 
 
     @classmethod
     def _config_str(cls):
 
         return (
             f"Dask cluster: Allocated {cls._job_n} jobs ({cls._job_n_workers} "
-            f"workers with {cls._job_mem} memory per job)\n"
-            f"SLURM: -p {cls._queue}, -A {cls._project}, " +
-            ", ".join(cls._job_slurm_commands) + "\n",
-            "ENV: " + "\n\t".join(cls._job_extra_env_commands) + "\n"
+            f"workers with {cls._job_mem} memory per job) "
+            f"plus {cls._num_local_workers} local workers "
+            f"[SLURM]: -p {cls._queue}, -A {cls._project}, "
+            f"{', '.join(cls._job_slurm_commands)} "
+            f"[ENV]: {', '.join(cls._job_extra_env_commands)}"
         )
 
     @classmethod
     def _config_env(cls):
         return [
             s.format(t=cls._worker_n_threads)
             for s in cls._job_threading_commands
         ] + cls._job_extra_env_commands
 
     @classmethod
     def _scale_jobs(cls):
         """
-        Update the worker tracker. If an entire slurm job is dead, start a new one to replace it.
+        Update the worker tracker. If an entire slurm job is dead,
+        start a new one to replace it.
         """
         cls._tracker.update_lists(
             cls.local_cluster.observed,
             cls.local_cluster.worker_spec
         )
 
         new_jobs = cls._job_n + cls._tracker.num_dead
+        max_jobs = cls._runaway_protection * cls._job_n
 
-        if cls._runaway_protection is not None and new_jobs > cls._runaway_protection * cls._job_n:
-            raise RuntimeError("Aborting excessive worker startups / Protecting against runaway job queueing")
+        if cls._runaway_protection is not None and new_jobs > max_jobs:
+            raise RuntimeError(
+                "Aborting excessive worker startups and "
+                "protecting against runaway job queueing")
         elif new_jobs > len(cls.local_cluster.worker_spec):
             cls.local_cluster.scale(jobs=new_jobs)
 
     @classmethod
     def _add_local_node_workers(cls, num_workers):
         """
         Start workers on the local node with the scheduler & client
 
         :param num_workers: The number of workers to start on this node
         :type num_workers: int
         """
-        check.argument_integer(num_workers, low=0, allow_none=True)
+        check.argument_integer(
+            num_workers,
+            low=0,
+            allow_none=True
+        )
 
         if num_workers is not None and num_workers > 0:
 
             # Build a dask-worker command
-            cmd = [cls._local_worker_command,
-                   str(cls.local_cluster.scheduler_address),
-                   "--nprocs", str(num_workers),
-                   "--nthreads", str(cls._worker_n_threads),
-                   "--memory-limit", "0",
-                   "--local-directory", str(cls._local_directory)]
+            cmd = [
+                cls._local_worker_command,
+                str(cls.local_cluster.scheduler_address),
+                "--nprocs", str(num_workers),
+                "--nthreads", str(cls._worker_n_threads),
+                "--memory-limit", "0",
+                "--local-directory", str(cls._local_directory)
+            ]
 
             # Execute it through the Popen ()
-            out_path = cls._log_directory if cls._log_directory is not None else "."
+            if cls._log_directory is not None:
+                out_path = cls._log_directory
+            else:
+                out_path = "."
 
             if not os.path.exists(out_path):
                 os.makedirs(out_path, exist_ok=True)
 
             subprocess.Popen(
                 cmd,
                 stdout=open(
@@ -557,16 +571,16 @@
         :return: Number of worker processes
         :rtype: int
         """
 
         _total = cls._job_n_workers if cls._job_n_workers is not None else 0
         _total *= cls._job_n if cls._job_n is not None else 0
 
-        if include_local:
-            _total += cls._num_local_workers if cls._num_local_workers is not None else 0
+        if include_local and cls._num_local_workers is not None:
+            _total += cls._num_local_workers
 
         return _total
 
 
 class WorkerTracker:
     """
     Keep track of which workers have been started but are now gone
```

### Comparing `inferelator-0.6.1/inferelator/distributed/dask_local_controller.py` & `inferelator-0.6.2/inferelator/distributed/dask_local_controller.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/distributed/inferelator_mp.py` & `inferelator-0.6.2/inferelator/distributed/inferelator_mp.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/distributed/joblib_controller.py` & `inferelator-0.6.2/inferelator/distributed/joblib_controller.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/distributed/local_controller.py` & `inferelator-0.6.2/inferelator/distributed/local_controller.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/postprocessing/column_names.py` & `inferelator-0.6.2/inferelator/postprocessing/column_names.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
-This is a central location for dataframe column names used in the postprocessing modules
+This is a central location for dataframe column names used in the
+postprocessing modules
 
-They're weirdly named for historical reasons and can be changed with no consequence unless you have other
+They're weirdly named for historical reasons and can be changed with
+no consequence unless you have other
 code that uses these names
 """
 
 BETA_SIGN_COLUMN = "beta.sign.sum"
 MEDIAN_EXPLAIN_VAR_COLUMN = "var.exp.median"
 CONFIDENCE_COLUMN = "combined_confidences"
 BETA_THRESHOLD_COLUMN = "beta_threshold"
 GOLD_STANDARD_COLUMN = "gold_standard"
 PRIOR_COLUMN = "prior"
 TARGET_COLUMN = "target"
 REGULATOR_COLUMN = "regulator"
 
+MODEL_COEF_COLUMN = "model_coefficient"
+MODEL_EXP_VAR_COLUMN = "model_exp_var"
+
 # Precision/Recall
 
 PRECISION_COLUMN = "precision"
 RECALL_COLUMN = "recall"
 
 # Matthew Correlation Coef
 
@@ -26,8 +31,7 @@
 # F1 Score
 
 F1_COLUMN = "F1"
 
 # Confusion Matrix
 
 TP, FP, TN, FN = 'TP', 'FP', 'TN', 'FN'
-
```

### Comparing `inferelator-0.6.1/inferelator/postprocessing/f1_score.py` & `inferelator-0.6.2/inferelator/postprocessing/f1_score.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/postprocessing/matthews_correlation.py` & `inferelator-0.6.2/inferelator/postprocessing/matthews_correlation.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/postprocessing/model_metrics.py` & `inferelator-0.6.2/inferelator/postprocessing/model_metrics.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/postprocessing/model_performance.py` & `inferelator-0.6.2/inferelator/postprocessing/model_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 import pandas as pd
 import numpy as np
 import gzip
+
 from inferelator import utils
 from inferelator.utils import Validator as check
 from inferelator.postprocessing import (
     GOLD_STANDARD_COLUMN,
     CONFIDENCE_COLUMN,
     TARGET_COLUMN,
     REGULATOR_COLUMN,
     TN,
     FN,
     TP,
     FP
 )
 
 
-class RankSummingMetric(object):
+class RankSummingMetric:
     """
     This class takes a data set that has some rankable values and
     a gold standard for which elements of that data set
     are true and calculates confidence
     """
 
     # Metric name
@@ -106,27 +107,29 @@
         )
 
         self.confidence_data.reset_index(inplace=True)
 
         # Filter the gold standard and confidences down to a format
         # that can be directly compared
         utils.Debug.vprint(
-            f"GS: {gold_standard.shape[0]} edges; "
-            f"Confidences: {confidence_data.shape[0]} edges",
+            f"GS: {gold_standard.sum().sum()} edges; "
+            f"Confidences: {(confidence_data[CONFIDENCE_COLUMN] > 0).sum()} "
+            "edges",
             level=0
         )
 
         self.filtered_data = self.filter_method(
             GOLD_STANDARD_COLUMN,
             CONFIDENCE_COLUMN,
             self.confidence_data
         ).copy()
 
         utils.Debug.vprint(
-            f"Filtered data to {self.filtered_data.shape[0]} edges",
+            "Filtered network data to "
+            f"{(self.filtered_data[CONFIDENCE_COLUMN] > 0).sum()} edges",
             level=1
         )
 
     def score(self):
         raise NotImplementedError
 
     def all_scores(self):
```

### Comparing `inferelator-0.6.1/inferelator/postprocessing/precision_recall.py` & `inferelator-0.6.2/inferelator/postprocessing/precision_recall.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/postprocessing/results_processor.py` & `inferelator-0.6.2/inferelator/postprocessing/results_processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,242 +1,349 @@
+import warnings
+
 import numpy as np
 import pandas as pd
 
 from inferelator import utils
 from inferelator.utils import Validator as check
-from inferelator.postprocessing.model_metrics import RankSummingMetric, MetricHandler
+from inferelator.postprocessing.model_metrics import (
+    RankSummingMetric,
+    MetricHandler
+)
+
 from inferelator.postprocessing.inferelator_results import InferelatorResults
-from inferelator.postprocessing import (BETA_SIGN_COLUMN, MEDIAN_EXPLAIN_VAR_COLUMN, CONFIDENCE_COLUMN,
-                                        BETA_THRESHOLD_COLUMN, TARGET_COLUMN, REGULATOR_COLUMN, PRIOR_COLUMN)
+from inferelator.postprocessing import (
+    BETA_SIGN_COLUMN,
+    MEDIAN_EXPLAIN_VAR_COLUMN,
+    CONFIDENCE_COLUMN,
+    TARGET_COLUMN,
+    REGULATOR_COLUMN,
+    PRIOR_COLUMN,
+    MODEL_COEF_COLUMN,
+    MODEL_EXP_VAR_COLUMN
+)
 
 FILTER_METHODS = ("overlap", "keep_all_gold_standard")
-DEFAULT_BOOTSTRAP_THRESHOLD = 0.5
 DEFAULT_FILTER_METHOD = "overlap"
 DEFAULT_METRIC = "precision-recall"
 
 
-class ResultsProcessor(object):
+class ResultsProcessor:
+
     # Data
     betas = None
     rescaled_betas = None
     filter_method = DEFAULT_FILTER_METHOD
 
     # Processed Network
     network_data = None
 
-    # Cutoffs
-    threshold = DEFAULT_BOOTSTRAP_THRESHOLD
-
     # Flag to write results
     write_results = True
 
     # Model result object
     result_object = InferelatorResults
 
     # Model metric
     metric = None
 
-    def __init__(self, betas, rescaled_betas, threshold=None, filter_method=None, metric=None):
-        """
-        :param betas: list(pd.DataFrame[G x K]) [B]
-            A list of model weights per bootstrap
-        :param rescaled_betas: list(pd.DataFrame[G x K]) [B]
-            A list of the variance explained by each parameter per bootstrap
-        :param threshold: float
-            The proportion of bootstraps which an model weight must be non-zero for inclusion in the network output
-        :param filter_method: str
-            How to handle gold standard filtering ('overlap' filters to beta, 'keep_all_gold_standard' doesn't filter)
-        :param metric: str / RankSummingMetric
-            The scoring metric to use
-        """
-
-        self.validate_init_args(betas, rescaled_betas, threshold=threshold, filter_method=filter_method, metric=metric)
+    def __init__(
+        self,
+        betas,
+        rescaled_betas,
+        filter_method=None,
+        metric=None
+    ):
+        """
+        :param betas: A list of dataframes [G x K] with model
+            weights per bootstrap
+        :type betas: list(pd.DataFrame)
+        :param rescaled_betas: A list of dataframes [G x K] with
+            the variance explained by each parameter per bootstrap
+        :type rescaled_betas: list(pd.DataFrame)
+        :param filter_method: How to handle gold standard filtering.
+            'overlap' filters to beta
+            'keep_all_gold_standard' doesn't filter and uses the entire
+            gold standard scoring network
+        :type filter_method: str
+        :param metric: The scoring metric to use
+        :type metric: str, RankSummingMetric
+        """
+
+        self.validate_init_args(
+            betas,
+            rescaled_betas,
+            filter_method=filter_method
+        )
 
         self.betas = betas
         self.rescaled_betas = rescaled_betas
-        self.filter_method = self.filter_method if filter_method is None else filter_method
-        self.threshold = self.threshold if threshold is None else threshold
 
-        metric = metric if metric is not None else DEFAULT_METRIC
-        self.metric = MetricHandler.get_metric(metric)
+        if filter_method is not None:
+            self.filter_method = filter_method
+
+        self.metric = MetricHandler.get_metric(
+            metric if metric is not None else DEFAULT_METRIC
+        )
 
     @staticmethod
-    def validate_init_args(betas, rescaled_betas, threshold=None, filter_method=None, metric=None):
+    def validate_init_args(
+        betas,
+        rescaled_betas,
+        filter_method=None
+    ):
         assert check.argument_type(betas, list)
         assert check.argument_type(betas[0], pd.DataFrame)
         assert check.dataframes_align(betas)
+
         assert check.argument_type(rescaled_betas, list)
         assert check.argument_type(rescaled_betas[0], pd.DataFrame)
         assert check.dataframes_align(rescaled_betas)
-        assert check.argument_enum(filter_method, FILTER_METHODS, allow_none=True)
-        assert check.argument_numeric(threshold, 0, 1, allow_none=True)
 
-    def summarize_network(self, output_dir, gold_standard, priors):
-        """
-        Take the betas and rescaled beta_errors, construct a network, and test it against the gold standard
-        :param output_dir: str
-            Path to write files into. Don't write anything if this is None.
-        :param gold_standard: pd.DataFrame [G x K]
-            Gold standard to test the network against
-        :param priors: pd.DataFrame [G x K]
-            Prior data
-        :return result: InferelatorResult
-            Returns an InferelatorResult
+        assert check.argument_enum(
+            filter_method,
+            FILTER_METHODS,
+            allow_none=True
+        )
+
+    def summarize_network(
+        self,
+        output_dir,
+        gold_standard,
+        priors,
+        full_model_betas=None,
+        full_model_var_exp=None,
+        extra_cols=None
+    ):
+        """
+        Take the betas and rescaled beta_errors, construct a network,
+        and test it against the gold standard
+
+        :param output_dir: Path to write files into.
+            Don't write anything if this is None.
+        :type output_dir: str, None
+        :param gold_standard: Gold standard DataFrame [G x K] to test
+            the network against
+        :type gold_standard: pd.DataFrame
+        :param priors: Priors dataframe [G x K]
+        :type priors: pd.DataFrame
+        :param extra_cols: Extra columns to add to the network dataframe,
+            as a dict of G x K dataframes keyed by column name
+        :return result: Result object
+        :rtype: InferelatorResult
         """
 
         assert check.argument_path(output_dir, allow_none=True)
         assert check.argument_type(gold_standard, pd.DataFrame)
         assert check.argument_type(priors, pd.DataFrame)
 
-        rs_calc = self.metric(self.rescaled_betas, gold_standard, filter_method=self.filter_method)
-        beta_threshold, beta_sign, beta_nonzero = self.threshold_and_summarize(self.betas, self.threshold)
-        resc_betas_mean, resc_betas_median = self.mean_and_median(self.rescaled_betas)
-        extra_cols = {BETA_SIGN_COLUMN: beta_sign, MEDIAN_EXPLAIN_VAR_COLUMN: resc_betas_median}
+        rs_calc = self.metric(
+            self.rescaled_betas,
+            gold_standard,
+            filter_method=self.filter_method
+        )
+
+        beta_sign, beta_nonzero = self.summarize(
+            self.betas
+        )
+
+        resc_betas_mean, resc_betas_median = self.mean_and_median(
+            self.rescaled_betas
+        )
+
+        if extra_cols is None:
+            extra_cols = {}
+
+        extra_cols.update({
+            BETA_SIGN_COLUMN: beta_sign,
+            MEDIAN_EXPLAIN_VAR_COLUMN: resc_betas_median
+        })
 
         m_name, score = rs_calc.score()
-        utils.Debug.vprint("Model {metric}:\t{score}".format(metric=m_name, score=score), level=0)
+
+        utils.Debug.vprint(
+            f"Model {m_name}:\t{score:.05f}",
+            level=0
+        )
 
         # Process data into a network dataframe
-        network_data = self.process_network(rs_calc, priors, beta_threshold=beta_threshold, extra_columns=extra_cols)
+        network_data = self.process_network(
+            rs_calc,
+            priors,
+            extra_columns=extra_cols,
+            full_model_betas=full_model_betas,
+            full_model_var_exp=full_model_var_exp
+        )
 
         # Create a InferelatorResult object and have it write output files
-        result = self.result_object(network_data, beta_threshold, rs_calc.all_confidences, rs_calc,
-                                    betas_sign=beta_sign, betas=self.betas)
+        result = self.result_object(
+            network_data,
+            full_model_betas,
+            rs_calc.all_confidences,
+            rs_calc,
+            betas_sign=beta_sign,
+            betas=self.betas,
+            priors=priors,
+            gold_standard=gold_standard
+        )
 
         if self.write_results and output_dir is not None:
             result.write_result_files(output_dir)
 
         return result
 
     @staticmethod
-    def process_network(metric, priors, confidence_threshold=0, beta_threshold=None, extra_columns=None):
+    def process_network(
+        metric,
+        priors,
+        full_model_betas=None,
+        full_model_var_exp=None,
+        confidence_threshold=0,
+        beta_threshold=None,
+        extra_columns=None
+    ):
         """
         Process rank-summed results into a network data frame
-        :param metric: RankSummingMetric
-            The rank-sum object with the math in it
-        :param priors: pd.DataFrame [G x K]
-            Prior data
-        :param confidence_threshold: numeric
-            The minimum confidence score needed to write a network edge
-        :param beta_threshold: pd.DataFrame [G x K]
-            The thresholded betas to include in the network. If None, include everything.
-        :param extra_columns: dict(col_name: pd.DataFrame [G x K])
-            Any additional data to include, keyed by column name and indexable with row and column names
-        :return network_data: pd.DataFrame [(G*K) x 7+]
-            Network edge dataframe
+
+        :param metric: The rank-sum object with the math in it
+        :type metric: RankSummingMetric
+        :param priors: Prior data [G x K]
+        :type priors: pd.DataFrame
+        :param confidence_threshold: The minimum confidence score needed
+            to write a network edge
+        :type confidence_threshold: numeric
+        :param beta_threshold: Deprecated
+        :param extra_columns: Any additional data to include, keyed by
+            column name and indexable with row and column names
+        :type extra_columns:  dict(col_name: pd.DataFrame [G x K])
+        :return network_data: Network edge dataframe [(G*K) x 7+]
+        :rtype: pd.DataFrame
 
         """
 
         assert check.argument_type(metric, RankSummingMetric)
         assert check.argument_type(priors, pd.DataFrame, allow_none=True)
-        assert check.argument_type(beta_threshold, pd.DataFrame, allow_none=True)
         assert check.argument_numeric(confidence_threshold, 0, 1)
 
+        if beta_threshold is not None:
+            warnings.warn(
+                "beta_threshold is deprecated and has no effect",
+                DeprecationWarning
+            )
+
         # Get the combined confidences and subset for confidence threshold
         network_data = metric.confidence_dataframe()
-        network_data = network_data.loc[network_data[CONFIDENCE_COLUMN] > confidence_threshold, :]
-
-        # If beta_threshold has been provided, melt and join it to the network data
-        # Then discard anything which isn't meeting the threshold
-        if beta_threshold is not None and False:
-            beta_data = utils.melt_and_reindex_dataframe(beta_threshold, BETA_THRESHOLD_COLUMN)
-            network_data = network_data.join(beta_data, on=[TARGET_COLUMN, REGULATOR_COLUMN])
-            network_data = network_data.loc[network_data[BETA_THRESHOLD_COLUMN] == 1, :]
-            del network_data[BETA_THRESHOLD_COLUMN]
+        network_data = network_data.loc[
+            network_data[CONFIDENCE_COLUMN] > confidence_threshold,
+            :
+        ]
 
         if priors is not None:
-            prior_data = utils.melt_and_reindex_dataframe(priors, PRIOR_COLUMN)
-            network_data = network_data.join(prior_data, on=[TARGET_COLUMN, REGULATOR_COLUMN])
+            network_data = network_data.join(
+                utils.melt_and_reindex_dataframe(
+                    priors,
+                    PRIOR_COLUMN
+                ),
+                on=[TARGET_COLUMN, REGULATOR_COLUMN]
+            )
+
+        if full_model_betas is not None:
+            network_data = network_data.join(
+                utils.melt_and_reindex_dataframe(
+                    full_model_betas,
+                    MODEL_COEF_COLUMN
+                ),
+                on=[TARGET_COLUMN, REGULATOR_COLUMN]
+            )
+
+        if full_model_var_exp is not None:
+            network_data = network_data.join(
+                utils.melt_and_reindex_dataframe(
+                    full_model_var_exp,
+                    MODEL_EXP_VAR_COLUMN
+                ),
+                on=[TARGET_COLUMN, REGULATOR_COLUMN]
+            )
 
         # Add any extra columns as needed
         if extra_columns is not None:
             for k in sorted(extra_columns.keys()):
-                extra_data = utils.melt_and_reindex_dataframe(extra_columns[k], k)
-                network_data = network_data.join(extra_data, on=[TARGET_COLUMN, REGULATOR_COLUMN])
+                network_data = network_data.join(
+                    utils.melt_and_reindex_dataframe(extra_columns[k], k),
+                    on=[TARGET_COLUMN, REGULATOR_COLUMN]
+                )
 
         # Make sure all missing values are NaN
         network_data[pd.isnull(network_data)] = np.nan
 
         return network_data
 
     @staticmethod
-    def threshold_and_summarize(betas, threshold):
-        """
-        Summarize a stack of betas
-        Returns dataframes
-        :param betas: list(pd.DataFrame)
-            A list of dataframes that are aligned on both axes
-        :param threshold: numeric
-            The proportion of bootstraps an interaction must occur in to be valid
-        :return betas_threshold: pd.DataFrame
-        :return betas_sign: pd.DataFrame
-        :return betas_non_zero: pd.DataFrame
-        """
-        betas_sign, betas_non_zero = ResultsProcessor.summarize(betas)
-        betas_threshold = ResultsProcessor.passes_threshold(betas_non_zero, len(betas), threshold)
-        return betas_threshold, betas_sign, betas_non_zero
-
-    @staticmethod
     def summarize(betas):
         """
         Compute summary information about betas
 
-        :param betas: list(pd.DataFrame) B x [M x N]
-            A list of dataframes that are aligned on both axes
-        :return betas_sign: pd.DataFrame [M x N]
-            A dataframe with the summation of np.sign() for each bootstrap
-        :return betas_non_zero: pd.DataFrame [M x N]
-            A dataframe with a count of the number of non-zero betas for an interaction
+        :param betas: A list of dataframes B x [G x K] that are aligned
+            on both axes
+        :type betas: list(pd.DataFrame)
+        :return: A dataframe [G x K] with the summation of np.sign() for
+            each bootstrap, and a dataframe with a count of the number of
+            non-zero betas for an interaction
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
         assert check.dataframes_align(betas)
 
-        betas_sign = pd.DataFrame(np.zeros(betas[0].shape), index=betas[0].index, columns=betas[0].columns)
-        betas_non_zero = pd.DataFrame(np.zeros(betas[0].shape), index=betas[0].index, columns=betas[0].columns)
+        betas_sign = pd.DataFrame(
+            np.zeros(betas[0].shape),
+            index=betas[0].index,
+            columns=betas[0].columns
+        )
+
+        betas_non_zero = pd.DataFrame(
+            np.zeros(betas[0].shape),
+            index=betas[0].index,
+            columns=betas[0].columns
+        )
+
         for beta in betas:
-            # Convert betas to -1,0,1 based on signing and then sum the results for each bootstrap
-            betas_sign = betas_sign + np.sign(beta.values)
+            # Convert betas to -1,0,1 based on signing
+            # and then sum the results for each bootstrap
+            betas_sign += np.sign(beta.values)
+
             # Tally all non-zeros for each bootstrap
-            betas_non_zero = betas_non_zero + (beta != 0).astype(int)
+            betas_non_zero += (beta != 0).astype(int)
 
         return betas_sign, betas_non_zero
 
     @staticmethod
-    def passes_threshold(betas_non_zero, max_num, threshold):
-        """
-
-        :param betas_non_zero: pd.DataFrame [M x N]
-            A dataframe of integer counts indicating how many times the original data was non-zero
-        :param max_num: int
-            The maximum number of possible counts (# bootstraps)
-        :param threshold: float
-            The proportion of integer counts over max possible in order to consider the interaction valid
-        :return: pd.DataFrame [M x N]
-            A bool dataframe where 1 corresponds to interactions that are in more than the threshold proportion of
-            bootstraps
-        """
-
-        assert check.argument_type(betas_non_zero, pd.DataFrame)
-        assert check.argument_integer(max_num)
-        assert check.argument_numeric(threshold, low=0, high=1)
-
-        return ((betas_non_zero / max_num) >= threshold).astype(int)
-
-    @staticmethod
     def mean_and_median(stack):
         """
         Calculate the mean and median values of a list of dataframes
-        Returns dataframes with the same dimensions as any one of the input stack
+        Returns dataframes with the same dimensions as any one of
+        the input stack
+
         :param stack: list(pd.DataFrame)
             List of dataframes which have the same size and dimensions
         :return mean_data: pd.DataFrame
             Mean values
         :return median_data:
             Median values
         """
 
         assert check.dataframes_align(stack)
 
         matrix_stack = [x.values for x in stack]
-        mean_data = pd.DataFrame(np.mean(matrix_stack, axis=0), index=stack[0].index, columns=stack[0].columns)
-        median_data = pd.DataFrame(np.median(matrix_stack, axis=0), index=stack[0].index, columns=stack[0].columns)
+
+        mean_data = pd.DataFrame(
+            np.mean(matrix_stack, axis=0),
+            index=stack[0].index,
+            columns=stack[0].columns
+        )
+
+        median_data = pd.DataFrame(
+            np.median(matrix_stack, axis=0),
+            index=stack[0].index,
+            columns=stack[0].columns
+        )
+
         return mean_data, median_data
```

### Comparing `inferelator-0.6.1/inferelator/postprocessing/results_processor_mtl.py` & `inferelator-0.6.2/inferelator/postprocessing/results_processor_mtl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import pandas as pd
 import numpy as np
 import os
 
 from inferelator.utils import Debug
 from inferelator.utils import Validator as check
-from inferelator.postprocessing import results_processor
-from inferelator.postprocessing import BETA_SIGN_COLUMN, MEDIAN_EXPLAIN_VAR_COLUMN
+from inferelator.postprocessing.results_processor import (
+    ResultsProcessor,
+    FILTER_METHODS
+)
+from inferelator.postprocessing import (
+    BETA_SIGN_COLUMN,
+    MEDIAN_EXPLAIN_VAR_COLUMN
+)
 
-
-class ResultsProcessorMultiTask(results_processor.ResultsProcessor):
+class ResultsProcessorMultiTask(ResultsProcessor):
     """
-    This results processor should handle the results of the MultiTask inferelator
+    This results processor should handle the results of
+    the MultiTask inferelator
 
     It will output the results for each task, as well as rank-combining to construct a network from all tasks
     """
 
     write_task_files = True
 
     tasks_names = None
     tasks_networks = None
 
     def __init__(
         self,
         betas,
         rescaled_betas,
-        threshold=None,
         filter_method=None,
         metric=None,
         task_names=None
     ):
         """
         :param betas: list(list(pd.DataFrame[G x K]) [B]) [T]
             A list of the task inferelator outputs per bootstrap per task
@@ -41,44 +46,59 @@
         :param metric: str / RankSummingMetric
             The scoring metric to use
         """
 
         super(ResultsProcessorMultiTask, self).__init__(
             betas,
             rescaled_betas,
-            threshold,
             filter_method,
             metric
         )
 
         # Make up some default names
         # The workflow will have to replace these with real names if necessary
         if task_names is None:
             self.tasks_names = list(map(str, range(len(self.betas))))
         else:
             self.tasks_names = task_names
 
     @staticmethod
-    def validate_init_args(betas, rescaled_betas, threshold=None, filter_method=None, metric=None):
+    def validate_init_args(
+        betas,
+        rescaled_betas,
+        filter_method=None
+    ):
         assert check.argument_type(betas, list)
         assert check.argument_list_type(betas, list)
         assert check.argument_list_type(betas[0], pd.DataFrame)
+
         assert check.argument_type(rescaled_betas, list)
         assert check.argument_list_type(rescaled_betas, list)
         assert check.argument_list_type(rescaled_betas[0], pd.DataFrame)
-        assert all([check.dataframes_align(b_task + bresc_task) for b_task, bresc_task in zip(betas, rescaled_betas)])
-        assert check.argument_enum(filter_method, results_processor.FILTER_METHODS, allow_none=True)
-        assert check.argument_numeric(threshold, 0, 1, allow_none=True)
+
+        assert all([
+            check.dataframes_align(b_task + bresc_task)
+            for b_task, bresc_task in zip(betas, rescaled_betas)
+        ])
+
+        assert check.argument_enum(
+            filter_method,
+            FILTER_METHODS,
+            allow_none=True
+        )
 
     def summarize_network(
         self,
         output_dir,
         gold_standard,
         priors,
-        task_gold_standards=None
+        full_model_betas=None,
+        full_model_var_exp=None,
+        task_gold_standards=None,
+        extra_cols=None
     ):
         """
         Take the betas and rescaled beta_errors, construct a network, and test
         it against the gold standard
 
         :param output_dir: Path to write files into. Don't write anything if
             this is None.
@@ -104,30 +124,37 @@
         assert len(self.rescaled_betas) == len(self.tasks_names)
 
         # Create empty lists for task-specific results
         overall_confidences = []
         overall_resc_betas = []
 
         # Get intersection of indices
-        gene_set = list(set([i for df in self.betas for i in df[0].index.tolist()]))
-        tf_set = list(set([i for df in self.betas for i in df[0].columns.tolist()]))
+        gene_set = list(set(
+            [i for df in self.betas for i in df[0].index.tolist()]
+        ))
+
+        tf_set = list(set(
+            [i for df in self.betas for i in df[0].columns.tolist()]
+        ))
+
+        # Use the existing indices if there's no difference from the
+        # intersection
+        if not _is_different(self.betas[0][0].index, gene_set):
+            gene_set = self.betas[0][0].index
 
-        # Use the existing indices if there's no difference from the intersection
-        gene_set = gene_set if _is_different(self.betas[0][0].index, gene_set) else self.betas[0][0].index
-        tf_set = tf_set if _is_different(self.betas[0][0].columns, tf_set) else self.betas[0][0].columns
+        if not _is_different(self.betas[0][0].columns, tf_set):
+            tf_set = self.betas[0][0].columns
 
         # Create empty dataframes for task-specific results
         overall_sign = pd.DataFrame(
             0,
             index=gene_set,
             columns=tf_set
         )
 
-        overall_threshold = overall_sign.copy()
-
         if task_gold_standards is None:
             task_gold_standards = [gold_standard] * len(self.tasks_names)
 
         # Run the result processing on each individual task
         # Keep the confidences from the tasks so that a final aggregate network can be assembled
         # Store the individual task network results in a dict
         self.tasks_networks = {}
@@ -136,69 +163,90 @@
 
             task_rs_calc = self.metric(
                 self.rescaled_betas[task_id],
                 task_gold_standards[task_id],
                 filter_method=self.filter_method
             )
 
-            task_threshold, task_sign, _ = self.threshold_and_summarize(
-                self.betas[task_id],
-                self.threshold
+            task_sign, _ = self.summarize(
+                self.betas[task_id]
             )
 
             _, task_resc_betas_median = self.mean_and_median(
                 self.rescaled_betas[task_id]
             )
 
             task_extra_cols = {
                 BETA_SIGN_COLUMN: task_sign,
                 MEDIAN_EXPLAIN_VAR_COLUMN: task_resc_betas_median
             }
 
+            if full_model_betas is not None:
+                _task_model_betas = full_model_betas[task_id]
+            else:
+                _task_model_betas = None
+
+            if full_model_var_exp is not None:
+                _task_model_var_exp = full_model_var_exp[task_id]
+            else:
+                _task_model_var_exp = None
+
             task_network_data = self.process_network(
                 task_rs_calc,
                 priors[task_id],
-                beta_threshold=task_threshold,
-                extra_columns=task_extra_cols
+                extra_columns=task_extra_cols,
+                full_model_betas=_task_model_betas,
+                full_model_var_exp=_task_model_var_exp
             )
 
             # Pile up data
-            overall_confidences.append(_df_resizer(task_rs_calc.all_confidences, gene_set, tf_set))
-            overall_resc_betas.append(_df_resizer(task_resc_betas_median, gene_set, tf_set))
-            overall_sign += np.sign(_df_resizer(task_sign, gene_set, tf_set))
-            overall_threshold += _df_resizer(task_threshold, gene_set, tf_set)
+            overall_confidences.append(
+                _df_resizer(task_rs_calc.all_confidences, gene_set, tf_set)
+            )
+
+            overall_resc_betas.append(
+                _df_resizer(task_resc_betas_median, gene_set, tf_set)
+            )
+
+            overall_sign += np.sign(
+                _df_resizer(task_sign, gene_set, tf_set)
+            )
 
             m_name, score = task_rs_calc.score()
 
             Debug.vprint(
-                f"Task {task_name} Model {m_name}:\t{score}",
+                f"Task {task_name} Model {m_name}:\t{score:.05f}",
                 level=0
             )
 
+            if _task_model_betas is None:
+                _task_model_betas = task_resc_betas_median
+
             task_result = self.result_object(
                 task_network_data,
-                task_threshold,
+                _task_model_betas,
                 task_rs_calc.all_confidences,
                 task_rs_calc,
                 betas_sign=task_sign,
                 betas=self.betas[task_id]
             )
 
             if self.write_task_files is True and output_dir is not None:
-                task_result.write_result_files(os.path.join(output_dir, task_name))
+                task_result.write_result_files(
+                    os.path.join(output_dir, task_name)
+                )
 
             self.tasks_networks[task_id] = task_result
 
         overall_rs_calc = self.metric(
             overall_confidences,
             gold_standard,
             filter_method=self.filter_method
         )
 
-        overall_threshold = (overall_threshold / len(overall_confidences) > self.threshold).astype(int)
         _, overall_resc_betas_median = self.mean_and_median(overall_resc_betas)
 
         extra_cols = {
             BETA_SIGN_COLUMN: overall_sign,
             MEDIAN_EXPLAIN_VAR_COLUMN: overall_resc_betas_median
         }
 
@@ -207,29 +255,45 @@
             f"Aggregate Model {m_name}:\t{score}",
             level=0
         )
 
         network_data = self.process_network(
             overall_rs_calc,
             None,
-            beta_threshold=overall_threshold,
             extra_columns=extra_cols
         )
 
         overall_result = self.result_object(
-            network_data, overall_threshold,
-            _df_resizer(overall_rs_calc.all_confidences, gene_set, tf_set),
+            network_data,
+            overall_resc_betas_median,
+            _df_resizer(
+                overall_rs_calc.all_confidences,
+                gene_set,
+                tf_set
+            ),
             overall_rs_calc,
             betas_sign=overall_sign
         )
 
         overall_result.write_result_files(output_dir)
         overall_result.tasks = self.tasks_networks
 
         return overall_result
 
 
 def _df_resizer(df, row_labs, col_labs, fill=0):
-    return df.reindex(row_labs, axis=0).reindex(col_labs, axis=1).fillna(fill)
+    """
+    Reindex a dataframe on rows and columns
+    And fill out all NAs
+    """
+
+    return df.reindex(
+        row_labs,
+        axis=0
+    ).reindex(
+        col_labs,
+        axis=1
+    ).fillna(fill)
+
 
 def _is_different(x, y):
     return len(x.symmetric_difference(y)) != 0
```

### Comparing `inferelator-0.6.1/inferelator/preprocessing/design_response_translation.py` & `inferelator-0.6.2/inferelator/preprocessing/design_response_translation.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/preprocessing/metadata_parser.py` & `inferelator-0.6.2/inferelator/preprocessing/metadata_parser.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/preprocessing/priors.py` & `inferelator-0.6.2/inferelator/preprocessing/priors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,122 @@
 import pandas as pd
 import numpy as np
 import warnings
 
-from inferelator import utils
-from inferelator.utils import Validator as check
+from inferelator.utils import (
+    Validator as check,
+    Debug
+)
 
 DEFAULT_CV_AXIS = 0
 DEFAULT_SEED = 2001
 
 
-class ManagePriors(object):
+class ManagePriors:
     """
-    The ManagePriors class has the functions to manipulate prior and gold standard data which are called from workflow
+    The ManagePriors class has the functions to manipulate prior
+    and gold standard data which are called from workflow
     This filters, aligns, crossvalidates, shuffles, etc.
     """
 
     @staticmethod
-    def validate_priors_gold_standard(priors_data, gold_standard):
+    def validate_priors_gold_standard(
+        priors_data,
+        gold_standard
+    ):
         """
         Validate the priors and the gold standard, then pass them through
 
-        :param priors_data: pd.DataFrame [G x K]
-            Prior data
-        :param gold_standard: pd.DataFrame [G x K]
-            Gold standard data
-        :return priors, gold_standard: pd.DataFrame [G x K], pd.DataFrame [G x K]
+        :param priors_data: Prior network data [G x K]
+        :type priors_data: pd.DataFrame
+        :param gold_standard: Gold standard network data [G x K]
+        :type gold_standard: pd.DataFrame
+        :return priors, gold_standard: Prior network data [G x K],
+            Gold standard network data [G x K]
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
         try:
             check.index_values_unique(priors_data.index)
         except ValueError as v_err:
-            utils.Debug.vprint("Duplicate gene(s) in prior index", level=0)
-            utils.Debug.vprint("\t" + str(v_err), level=0)
+            Debug.vprint(
+                "Duplicate gene(s) in prior index: " + str(v_err),
+                level=0
+            )
 
         try:
             check.index_values_unique(priors_data.columns)
         except ValueError as v_err:
-            utils.Debug.vprint("Duplicate tf(s) in prior index", level=0)
-            utils.Debug.vprint("\t" + str(v_err), level=0)
+            Debug.vprint(
+                "Duplicate tf(s) in prior index: " + str(v_err),
+                level=0
+            )
 
         try:
             check.index_values_unique(gold_standard.index)
         except ValueError as v_err:
-            utils.Debug.vprint("Duplicate gene(s) in gold standard index", level=0)
-            utils.Debug.vprint("\t" + str(v_err), level=0)
+            Debug.vprint(
+                "Duplicate gene(s) in gold standard index: " + str(v_err),
+                level=0
+            )
 
         try:
             check.index_values_unique(gold_standard.columns)
         except ValueError as v_err:
-            utils.Debug.vprint("Duplicate tf(s) in gold standard index", level=0)
-            utils.Debug.vprint("\t" + str(v_err), level=0)
+            Debug.vprint(
+                "Duplicate tf(s) in gold standard index" + str(v_err),
+                level=0
+            )
 
         return priors_data, gold_standard
 
     @staticmethod
-    def cross_validate_gold_standard(priors_data, gold_standard, cv_split_axis, cv_split_ratio, random_seed):
-        """
-        Sample the gold standard for crossvalidation, and then remove the new gold standard from the priors (if split
-        on an axis)
-
-        :param priors_data: pd.DataFrame [G x K]
-            Prior data
-        :param gold_standard: pd.DataFrame [G x K]
-            Gold standard data
-        :param cv_split_ratio: float
-            The proportion of the priors that should go into the gold standard
-        :param cv_split_axis: int
-            Splits on rows (when 0), columns (when 1), or on flattened individual data points (when None)
-            Note that if this is None, the returned gold standard will be the same as all_data, and the priors will have
-            half of the data points of all_data
-        :param random_seed: int
-            Random seed
-        :return priors_data, gold_standard: pd.DataFrame [G x K], pd.DataFrame [G x K]
+    def cross_validate_gold_standard(
+        priors_data,
+        gold_standard,
+        cv_split_axis,
+        cv_split_ratio,
+        random_seed
+    ):
+        """
+        Sample the gold standard for crossvalidation, and then remove the
+        new gold standard from the priors (if split on an axis)
+
+        :param priors_data: Prior network data [G x K]
+        :type priors_data: pd.DataFrame
+        :param gold_standard: Gold standard network data [G x K]
+        :type gold_standard: pd.DataFrame
+        :param cv_split_ratio: The proportion of the priors that should go
+            into the gold standard
+        :type cv_split_ratio: float
+        :param cv_split_axis: Splits on rows (when 0),
+            columns (when 1),
+            or on flattened individual data points (when None)
+            Note that if this is None, the returned gold standard will be
+            unchanged, and the priors will have half of the network edges in
+            the gold standard. If a different prior network has been passed in
+            it will be discarded
+        :type cv_split_axis: int, None
+        :param random_seed: Random seed
+        :type random_seed: int
+        :return priors, gold_standard: Prior network data [G x K],
+            Gold standard network data [G x K]
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
-        assert check.argument_enum(cv_split_axis, (0, 1), allow_none=True)
-        assert check.argument_numeric(cv_split_ratio, low=0, high=1)
+        assert check.argument_enum(
+            cv_split_axis,
+            (0, 1),
+            allow_none=True
+        )
+        assert check.argument_numeric(
+            cv_split_ratio,
+            low=0,
+            high=1
+        )
 
         _gs_shape = gold_standard.shape
 
         if cv_split_axis == 1:
             warnings.warn(
                 "Setting a cv_split_axis of 1 means TFs in the gold standard "
                 "will have no prior network knowledge for activity. "
@@ -101,168 +138,285 @@
                 gold_standard,
                 split_axis=cv_split_axis
             )
 
         else:
             if priors_data is not None:
                 warnings.warn(
-                    "Existing prior is being replaced with a downsampled gold standard "
+                    "Existing prior is being replaced with a "
+                    "downsampled gold standard "
                     "because cv_split_axis == None"
                 )
 
             priors_data = gs_to_prior
 
-        utils.Debug.vprint(
+        Debug.vprint(
             f"Gold standard {_gs_shape} split on axis {cv_split_axis}. "
             f"Prior knowledge network {priors_data.shape} "
-            f"[{np.sum(np.sum(priors_data != 0))} edges] is for activity "
+            f"[{np.sum(np.sum(priors_data != 0))} edges] used for activity "
             f"and gold standard network {gold_standard.shape} "
-            f"[{np.sum(np.sum(gold_standard != 0))} edges] is for testing.",
+            f"[{np.sum(np.sum(gold_standard != 0))} edges] used for testing.",
             level=0
         )
 
         return priors_data, gold_standard
 
     @staticmethod
-    def filter_priors_to_genes(priors_data, gene_list):
+    def filter_priors_to_genes(
+        priors_data,
+        gene_list
+    ):
+        """
+        Filter a prior network dataframe to a gene index
+
+        :param priors_data: Prior network data [G x K]
+        :type priors_data: pd.DataFrame
+        :param gene_list: List or index with genes to filter to
+        :type gene_list: list, pd.Index
+        :return priors: Prior network data [G x K] filtered on
+            targets
+        :rtype: pd.DataFrame
+        """
 
         if len(gene_list) == 0:
-            raise ValueError("Filtering to a list of 0 genes is not valid")
+            raise ValueError(
+                "Filtering to a list of 0 genes is not valid"
+            )
 
         if len(priors_data.index) == 0:
-            raise ValueError("Filtering a prior matrix of 0 genes is not valid")
+            raise ValueError(
+                "Filtering a prior matrix of 0 genes is not valid"
+            )
 
         try:
-            priors_data = ManagePriors._filter_df_index(priors_data, gene_list)
+            priors_data = ManagePriors._filter_df_index(
+                priors_data,
+                gene_list
+            )
         except ValueError as err:
             raise ValueError(
                 f"{str(err)} when filtering priors for gene list. "
-                f"Prior matrix genes: {str(priors_data.index[0])} ... "
-                f"Gene list genes: {str(gene_list[0])}"
+                f"Prior matrix genes (e.g. {str(priors_data.index[0])}) "
+                f"and gene list genes (e.g. {str(gene_list[0])}) are "
+                "non-overlapping"
             )
 
         return priors_data
 
     @staticmethod
-    def _filter_df_index(data_frame, index_list):
-        new_index = data_frame.index.intersection(index_list)
+    def filter_to_tf_names_list(
+        priors_data,
+        tf_names
+    ):
+        """
+        Filter the priors to a provided list of regulators
+
+        :param priors_data: Prior network data [G x K]
+        :type priors_data: pd.DataFrame
+        :param tf_names: List or index with tfs (columns) to filter to
+        :type tf_names: list, pd.Index
+        :return priors: Prior network data [G x K] filtered on
+            regulators
+        :rtype: pd.DataFrame
+        """
 
-        if len(new_index) == 0:
-            raise ValueError("Filtering results in 0-length index")
+        if len(tf_names) == 0:
+            raise ValueError(
+                "Filtering to a list of 0 TFs is not valid"
+            )
 
-        return data_frame.loc[new_index, :]
+        if len(priors_data.columns) == 0:
+            raise ValueError(
+                "Filtering a prior matrix of 0 TFs is not valid"
+            )
 
-    @staticmethod
-    def filter_to_tf_names_list(priors_data, tf_names):
-        """
-        Filter the priors the intersection with a provided list of regulators
-        :param priors_data: pd.DataFrame [G x K]
-            Prior data
-        :param tf_names: list [k]
-            List of regulators to restrict the modeling to
-        :return priors_data: pd.DataFrame [G x k]
-            Filtered priors on regulators
-        """
+        try:
+            priors_data = ManagePriors._filter_df_index(
+                priors_data,
+                tf_names,
+                axis=1
+            )
+        except ValueError as err:
+            raise ValueError(
+                f"{str(err)} when filtering priors for TF list. "
+                f"Prior matrix TFs (e.g. {str(priors_data.columns[0])}) "
+                f"and TF list genes (e.g. {str(tf_names[0])}) are "
+                "non-overlapping"
+            )
 
-        tf_keepers = pd.Index(tf_names).intersection(pd.Index(priors_data.columns))
-        priors_data = priors_data.loc[:, tf_keepers]
+        Debug.vprint(
+            f"Filtered prior to {priors_data.shape[1]} TFs from the "
+            "TF name list",
+            level=1
+        )
 
-        utils.Debug.vprint("Filtered to {tfn} TFs from the TF name list".format(tfn=len(tf_keepers)), level=1)
+        return priors_data
 
-        if priors_data.shape[1] == 0:
-            raise ValueError("Prior regulators and regulator list regulators have no overlap")
+    @staticmethod
+    def _filter_df_index(
+        data_frame,
+        index_list,
+        axis=0
+    ):
 
-        return priors_data
+        if axis == 0:
+            new_index = data_frame.index.intersection(
+                index_list
+            )
+        elif axis == 1:
+            new_index = data_frame.columns.intersection(
+                index_list
+            )
+        else:
+            raise ValueError(
+                "_filter_df_index axis must be 0 or 1"
+            )
+
+        if len(new_index) == 0:
+            raise ValueError(
+                "Filtering results in 0-length index"
+            )
+
+        return data_frame.reindex(
+            new_index,
+            axis=axis
+        )
 
     @staticmethod
-    def align_priors_to_expression(priors_data, gene_list):
+    def align_priors_to_expression(
+        priors_data,
+        gene_list
+    ):
+        """
+        Make sure that the priors align to the expression matrix and fill
+        priors that are created with 0s
+
+        :param priors_data: Prior network data [G x K]
+        :type priors_data: pd.DataFrame
+        :param gene_list: List or index with genes to align to
+        :type gene_list: list, pd.Index
+        :return priors: Prior network data [G x K] aligned on genes and
+            filled out with 0s
+        :rtype: pd.DataFrame
         """
-        Make sure that the priors align to the expression matrix and fill priors that are created with 0s
-        :param priors_data: pd.DataFrame [G x K]
-            Prior data
-        :param gene_list: pd.Index [G]
-            Expression matrix genes
-        :return priors_data:
-            Returns priors_data where genes match expression matrix genes
-        """
-
-        if len(priors_data.index.intersection(gene_list)) == 0:
-            err = "Prior genes and expression matrix genes have no overlap."
-            if len(priors_data.index) == 0:
-                err += " (Prior matrix has no genes"
-            else:
-                e_genes = map(str, priors_data.index[0:min(len(priors_data.index), 5)])
-                err += " (Prior genes: " + " ".join(e_genes) + "..."
-            if len(gene_list) == 0:
-                err += " Expression matrix has no genes)"
-            else:
-                e_genes = map(str, gene_list[0:min(len(gene_list), 5)])
-                err += " Expression matrix genes: " + " ".join(e_genes) + ")"
 
-            raise ValueError(err)
+        # Filter to overlap and raise an error if there's no overlap
+        try:
+            priors_data = ManagePriors._filter_df_index(
+                priors_data,
+                gene_list
+            )
+        except ValueError as err:
+            raise ValueError(
+                f"{str(err)} when aligning priors to expression data. "
+                f"Prior matrix genes (e.g. {str(priors_data.index[0])}) "
+                f"and expression data genes (e.g. {str(gene_list[0])}) are "
+                "non-overlapping"
+            )
 
-        return priors_data.reindex(index=gene_list).fillna(value=0)
+        # Reindex to align to the full expression gene index
+        # and fill out with zeros
+        return priors_data.reindex(
+            index=gene_list
+        ).fillna(value=0)
 
     @staticmethod
-    def shuffle_priors(priors_data, shuffle_prior_axis, random_seed):
+    def shuffle_priors(
+        priors_data,
+        shuffle_prior_axis,
+        random_seed
+    ):
         """
         Shuffle the labels on the priors on a specific axis
-        :param priors_data: pd.DataFrame [G x K]
-            Prior data
-        :param shuffle_prior_axis: int
-            Axis to shuffle. 0 is genes, 1 is regulators, -1 is to shuffle both axes. None is skip shuffling.
-        :param random_seed: int
-            Random seed
-        :return priors_data:
-            Returns priors_data the data has been shuffled on a specific axis
+        :param priors_data: Prior network data [G x K]
+        :type priors_data: pd.DataFrame
+        :param shuffle_prior_axis: Prior axis to shuffle.
+            0 is genes,
+            1 is regulators,
+            -1 is to shuffle both axes.
+            None is skip shuffling.
+        :type shuffle_prior_axis: int
+        :param random_seed: Random seed
+        :type random_seed: int
+        :return priors: Prior network data [G x K] shuffled on
+            one or both axes
+        :rtype: pd.DataFrame
         """
 
-        assert check.argument_enum(shuffle_prior_axis, [-1, 0, 1], allow_none=True)
+        assert check.argument_enum(
+            shuffle_prior_axis,
+            [-1, 0, 1],
+            allow_none=True
+        )
 
-        def _shuffle_genes(pd):
+        def _shuffle_axis(pd, axis=0):
             # Shuffle index (genes) in the priors_data
-            utils.Debug.vprint("Randomly shuffling prior [{sh}] gene data".format(sh=pd.shape), level=0)
-            prior_index = pd.index.tolist()
-            pd = pd.sample(frac=1, axis=0, random_state=random_seed)
-            pd.index = prior_index
-            return pd
+            Debug.vprint(
+                f"Randomly shuffling prior {pd.shape} "
+                f"{'gene' if axis == 0 else 'TF'} data",
+                level=0
+            )
+
+            if axis == 0:
+                prior_index = pd.index.tolist()
+            elif axis == 1:
+                prior_index = pd.columns.tolist()
+
+            pd = pd.sample(
+                frac=1,
+                axis=axis,
+                random_state=random_seed
+            )
+
+            if axis == 0:
+                pd.index = prior_index
+            elif axis == 1:
+                pd.columns = prior_index
 
-        def _shuffle_tfs(pd):
-            # Shuffle columns (TFs) in the priors_data
-            utils.Debug.vprint("Randomly shuffling prior [{sh}] TF data".format(sh=pd.shape), level=0)
-            prior_index = pd.columns.tolist()
-            pd = pd.sample(frac=1, axis=1, random_state=random_seed)
-            pd.columns = prior_index
             return pd
 
         if shuffle_prior_axis is None:
             return priors_data
+
         elif shuffle_prior_axis == 0:
-            priors_data = _shuffle_genes(priors_data)
+            priors_data = _shuffle_axis(
+                priors_data
+            )
         elif shuffle_prior_axis == 1:
-            priors_data = _shuffle_tfs(priors_data)
+            priors_data = _shuffle_axis(
+                priors_data, axis=1
+            )
         elif shuffle_prior_axis == -1:
-            priors_data = _shuffle_genes(priors_data)
-            priors_data = _shuffle_tfs(priors_data)
+            priors_data = _shuffle_axis(
+                priors_data
+            )
+            priors_data = _shuffle_axis(
+                priors_data, axis=1
+            )
 
         return priors_data
 
     @staticmethod
-    def add_prior_noise(priors_data, noise_ratio, random_seed):
+    def add_prior_noise(
+        priors_data,
+        noise_ratio,
+        random_seed
+    ):
         """
-        Add random edges to the prior. Note that this will binarize the prior if it was not already binary.
+        Add random edges to the prior. Note that this will binarize the
+        prior if it was not already binary.
 
-        :param priors_data: Prior data
-        :type priors_data: pd.DataFrame [G x K]
+        :param priors_data: Prior data [G x K]
+        :type priors_data: pd.DataFrame
         :param noise_ratio: Ratio of edges to add to the prior
         :type noise_ratio: float
         :param random_seed: Random seed for generator
         :type random_seed: int
-        :return: Prior data
-        :rtype: pd.DataFrame [G x K]
+        :return: Prior data [G x K]
+        :rtype: pd.DataFrame
         """
 
         assert check.argument_numeric(noise_ratio, low=0, high=1)
         assert check.argument_integer(random_seed)
 
         rgen = np.random.default_rng(random_seed)
 
@@ -272,135 +426,228 @@
         priors_data = priors_data != 0
         old_prior_sum = priors_data.sum().sum()
 
         priors_data += new_prior <= cutoff
         priors_data = (priors_data != 0).astype(int)
         new_prior_sum = priors_data.sum().sum()
 
-        _msg = "Prior {sh} [{ol}] modified to {n} noise [{ne}]".format(sh=priors_data.shape, ol=old_prior_sum,
-                                                                       ne=new_prior_sum, n=noise_ratio)
-        utils.Debug.vprint(_msg, level=0)
+        Debug.vprint(
+            f"Prior {priors_data.shape} [{old_prior_sum}] modified "
+            f"to {noise_ratio:.02f} noise [{new_prior_sum}]",
+            level=0
+        )
 
         return priors_data
 
 
     @staticmethod
-    def _split_for_cv(all_data, split_ratio, split_axis=DEFAULT_CV_AXIS, seed=DEFAULT_SEED):
-        """
-        Take a dataframe and split it according to split_ratio on split_axis into two new dataframes. This is for
-        crossvalidation splits of a gold standard.
-
-        :param all_data: pd.DataFrame [G x K]
-            Existing prior or gold standard data
-        :param split_ratio: float
-            The proportion of the priors that should go into the gold standard
-        :param split_axis: int
-            Splits on rows (when 0), columns (when 1), or on flattened individual data points (when None)
-            Note that if this is None, the returned gold standard will be the same as all_data, and the priors will have
-            half of the data points of all_data
-        :param seed: int
-            Seed for the random generator
-        :return prior_data, gold_standard: pd.DataFrame [G/2 x K], pd.DataFrame [G/2 x K]
-            Returns a new prior and gold standard by splitting the old one in half
+    def _split_for_cv(
+        all_data,
+        split_ratio,
+        split_axis=DEFAULT_CV_AXIS,
+        seed=DEFAULT_SEED
+    ):
+        """
+        Take a dataframe and split it according to split_ratio on split_axis
+        into two new dataframes. This is for crossvalidation splits of a gold
+        standard.
+
+        :param all_data: Network edges [G x K] dataframe
+        :type all_data: pd.DataFrame
+        :param split_ratio: The proportion of the priors that should go
+            into the gold standard
+        :type split_ratio: float
+        :param split_axis: Splits on rows (when 0),
+            columns (when 1),
+            or on flattened individual data points (when None)
+            Note that if this is None, the returned gold standard will be
+            unchanged, and the priors will have half of the network edges in
+            the gold standard. If a different prior network has been passed in
+            it will be discarded
+        :type split_axis: int, None
+        :param random_seed: Random seed
+        :type random_seed: int
+        :return: Returns a new prior network [G * (1-split_ratio) x K]
+            and gold standard network [G * (split_ratio) x K]
+            by splitting the old prior1
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
         assert check.argument_numeric(split_ratio, 0, 1)
         assert check.argument_enum(split_axis, [0, 1], allow_none=True)
 
-        # Split the priors into gold standard based on axis (flatten if axis=None)
+        # Split the priors into gold standard based on axis
+        # (flatten if axis=None)
         if split_axis is None:
-            priors_data, _ = ManagePriors._split_flattened(all_data, split_ratio, seed=seed)
+            priors_data, _ = ManagePriors._split_flattened(
+                all_data,
+                split_ratio,
+                seed=seed
+            )
+
+            # Reset the gold standard as the full data
             gold_standard = all_data
+
+        # Split the network on either axis and return the pieces
         else:
-            priors_data, gold_standard = ManagePriors._split_axis(all_data, split_ratio, axis=split_axis, seed=seed)
+            priors_data, gold_standard = ManagePriors._split_axis(
+                all_data,
+                split_ratio,
+                axis=split_axis,
+                seed=seed
+            )
 
         return priors_data, gold_standard
 
     @staticmethod
-    def _remove_prior_circularity(priors, gold_standard, split_axis=DEFAULT_CV_AXIS):
+    def _remove_prior_circularity(
+        priors,
+        gold_standard,
+        split_axis=DEFAULT_CV_AXIS
+    ):
         """
         Remove all axis labels that occur in the gold standard from the prior
-        :param priors: pd.DataFrame [M x N]
-        :param gold_standard: pd.DataFrame [m x n]
-        :param split_axis: int (0,1)
-        :return new_priors: pd.DataFrame [M-m x N]
-        :return gold_standard: pd.DataFrame [m x n]
+
+        :param priors_data: Prior network data [G x K]
+        :type priors_data: pd.DataFrame
+        :param gold_standard: Gold standard network data [G x K]
+        :type gold_standard: pd.DataFrame
+        :param split_axis: Remove overlap on rows (when 0),
+            or on columns (when 1),
+        :type split_axis: int, None
+        :return: New prior network data without any values that are in the
+            gold standard network on the selected axis
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
         assert check.argument_enum(split_axis, [0, 1])
 
-        new_priors = priors.drop(gold_standard.axes[split_axis], axis=split_axis, errors='ignore')
+        new_priors = priors.drop(
+            gold_standard.axes[split_axis],
+            axis=split_axis,
+            errors='ignore'
+        )
 
         return new_priors, gold_standard
 
     @staticmethod
-    def _split_flattened(data, split_ratio, seed=DEFAULT_SEED):
+    def _split_flattened(
+        data,
+        split_ratio,
+        seed=DEFAULT_SEED
+    ):
         """
         Instead of splitting by axis labels, split edges and ignore axes
-        :param data: pd.DataFrame [M x N]
-        :param split_ratio: float
-        :param seed:
-        :return priors_data: pd.DataFrame [M x N]
-        :return gold_standard: pd.DataFrame [M x N]
+
+        :param all_data: Network edges [G x K] dataframe
+        :type all_data: pd.DataFrame
+        :param split_ratio: The proportion of the network data edges
+            that should go into the gold standard
+        :type split_ratio: float
+        :param random_seed: Random seed
+        :type random_seed: int
+        :return: Network edges split into two [G x K] dataframes
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
         assert check.argument_numeric(split_ratio, 0, 1)
 
+        # Get the number of non-zero edges
+        # and order them randomly
         pc = np.sum(data.values != 0)
         gs_count = int(split_ratio * pc)
         idx = ManagePriors._make_shuffled_index(pc, seed=seed)
 
-        pr_idx = data.values[data.values != 0].copy()
-        gs_idx = data.values[data.values != 0].copy()
+        # Get the nonzero edges as a flattened array
+        pr_idx = data.values[data.values != 0]
+        gs_idx = pr_idx.copy()
 
+        # Set some of them to zero in one and the rest to zero in the other
         pr_idx[idx[0:gs_count]] = 0
         gs_idx[idx[gs_count:]] = 0
 
         gs = data.values.copy()
-        pr = data.values.copy()
+        pr = gs.copy()
 
+        # Replace the nonzero values with some nonzero values and some
+        # zero values
         gs[gs != 0] = gs_idx
         pr[pr != 0] = pr_idx
 
-        priors_data = pd.DataFrame(pr, index=data.index, columns=data.columns)
-        gold_standard = pd.DataFrame(gs, index=data.index, columns=data.columns)
+        # Rebuild dataframes
+        priors_data = pd.DataFrame(
+            pr,
+            index=data.index,
+            columns=data.columns
+        )
+
+        gold_standard = pd.DataFrame(
+            gs,
+            index=data.index,
+            columns=data.columns
+        )
 
         return priors_data, gold_standard
 
     @staticmethod
-    def _split_axis(priors, split_ratio, axis=DEFAULT_CV_AXIS, seed=DEFAULT_SEED):
+    def _split_axis(
+        priors,
+        split_ratio,
+        axis=DEFAULT_CV_AXIS,
+        seed=DEFAULT_SEED
+    ):
         """
         Split by axis labels on the chosen axis
-        :param priors: pd.DataFrame [M x N]
-        :param split_ratio: float
-        :param axis: [0, 1]
-        :param seed:
-        :return:
+
+        :param priors: Network edges [G x K] dataframe
+        :type priors: pd.DataFrame
+        :param split_ratio: The proportion of the network data axis
+            that should go into the gold standard
+        :param axis: Split on on rows (when 0), or on columns (when 1)
+        :type axis: int
+        :param random_seed: Random seed
+        :type random_seed: int
+        :return: Network edges split into two dataframes on an axis
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
         assert check.argument_numeric(split_ratio, 0, 1)
         assert check.argument_enum(axis, [0, 1])
 
+        # Get the number of entries on the axis
+        # and decide where to cut it for the split
         pc = priors.shape[axis]
         gs_count = int((1 - split_ratio) * pc)
-        idx = ManagePriors._make_shuffled_index(pc, seed=seed)
+        idx = ManagePriors._make_shuffled_index(
+            pc,
+            seed=seed
+        )
 
         if axis == 0:
             axis_idx = priors.index
         elif axis == 1:
             axis_idx = priors.columns
         else:
             raise ValueError("Axis can only be 0 or 1")
 
+        # Select the axis labels for the prior
+        # and the axis labels for the gold standard,
+        # randomly chosen, not from the existing order
         pr_idx = axis_idx[idx[0:gs_count]]
         gs_idx = axis_idx[idx[gs_count:]]
 
+        # Drop the labels from the appropriate axis
         priors_data = priors.drop(gs_idx, axis=axis)
         gold_standard = priors.drop(pr_idx, axis=axis)
 
         return priors_data, gold_standard
 
     @staticmethod
-    def _make_shuffled_index(idx_len, seed=DEFAULT_SEED):
+    def _make_shuffled_index(
+        idx_len,
+        seed=DEFAULT_SEED
+    ):
+
         idx = list(range(idx_len))
         np.random.RandomState(seed=seed).shuffle(idx)
+
         return idx
```

### Comparing `inferelator-0.6.1/inferelator/preprocessing/simulate_data.py` & `inferelator-0.6.2/inferelator/preprocessing/simulate_data.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/preprocessing/single_cell.py` & `inferelator-0.6.2/inferelator/preprocessing/single_cell.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/regression/amusr_math.py` & `inferelator-0.6.2/inferelator/regression/amusr_math.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/regression/amusr_regression.py` & `inferelator-0.6.2/inferelator/regression/amusr_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import numpy as np
 import pandas as pd
 import itertools
 import functools
 
 from inferelator.distributed.inferelator_mp import MPControl
-from inferelator import utils
-from inferelator.utils import Validator as check
-from .base_regression import (_MultitaskRegressionWorkflowMixin,
-                              BaseRegression, PROGRESS_STR)
+from inferelator.utils import (
+    Debug,
+    Validator as check
+)
+from .base_regression import (
+    _MultitaskRegressionWorkflowMixin,
+    BaseRegression,
+    PreprocessData,
+    PROGRESS_STR
+)
 from .amusr_math import run_regression_EBIC
 
 DEFAULT_prior_weight = 1.0
 
 TOL = 1e-2
 REL_TOL = None
 
@@ -53,15 +59,15 @@
                  lambda_Bs=None,
                  lambda_Ss=None,
                  Cs=None,
                  Ss=None,
                  tol=TOL,
                  rel_tol=REL_TOL,
                  use_numba=False
-        ):
+    ):
         """
         Set up a regression object for multitask regression
         :param X: Design activity data for each task
         :type X: list(InferelatorData)
         :param Y: Response expression data for each task
         :type Y: list(InferelatorData)
         :param priors: Prior network data for each task
@@ -203,15 +209,15 @@
     remove_autoregulation=True,
     **kwargs
 ):
     """ Wrapper for multiprocessing AMuSR """
 
     y_data, gene = y_data_stack
 
-    utils.Debug.vprint(
+    Debug.vprint(
         PROGRESS_STR.format(gn=gene[0], i=j, total=nG),
         level=0 if j % 1000 == 0 else 2
     )
 
     x, y, tf_t, tasks = [], [], [], []
 
     if remove_autoregulation:
@@ -232,15 +238,22 @@
         prior,
         gene,
         tasks,
         prior_weight,
         tfs=tfs
     )
 
-    return run_regression_EBIC(x, y, tf_t, tasks, gene, prior, **kwargs)
+    return run_regression_EBIC(
+        x,
+        y,
+        tf_t,
+        tasks,
+        gene, prior,
+        **kwargs
+    )
 
 
 def _y_generator(y_data, genes):
 
     nG = len(genes)
 
     for i in range(nG):
@@ -385,15 +398,15 @@
 
     :param X: list(InferelatorData) [T]
     :return X: list(InferelatorData) [T]
     """
 
     assert check.argument_type(X, list)
 
-    return [xk.zscore(ddof=0) for xk in X]
+    return [PreprocessData.preprocess_design(xk) for xk in X]
 
 
 class AMUSRRegressionWorkflowMixin(_MultitaskRegressionWorkflowMixin):
     """
     Multi-Task AMuSR regression
 
     https://doi.org/10.1371/journal.pcbi.1006591
@@ -458,20 +471,27 @@
 
     def run_bootstrap(self, bootstrap_idx):
         x, y, tfs = [], [], []
 
         # Select the appropriate bootstrap from each task and stash the
         # data into X and Y
         for k in range(self._n_tasks):
-            x.append(self._task_design[k].get_bootstrap(
-                self._task_bootstraps[k][bootstrap_idx]
-            ))
-            y.append(self._task_response[k].get_bootstrap(
-                self._task_bootstraps[k][bootstrap_idx]
-            ))
+
+            if bootstrap_idx is not None:
+                x.append(self._task_design[k].get_bootstrap(
+                    self._task_bootstraps[k][bootstrap_idx]
+                ))
+                y.append(self._task_response[k].get_bootstrap(
+                    self._task_bootstraps[k][bootstrap_idx]
+                ))
+
+            else:
+                x.append(self._task_design[k])
+                y.append(self._task_response[k])
+
             tfs.append(self._task_design[k].gene_names.tolist())
 
         regress = self._r_class(
             x,
             y,
             tfs=tfs,
             genes=self._task_genes,
@@ -526,14 +546,15 @@
         raise ValueError(
             f"{task_expression_filter} is not an allowed "
             "task_expression_filter value"
         )
 
     return filtered_genes
 
+
 def genes_tasks(list_of_genes, list_of_data):
     """
     Take a list of genes and find them in the task
     response data gene_names.
 
     Returns (task #, gene_id) tuples
```

### Comparing `inferelator-0.6.1/inferelator/regression/base_regression.py` & `inferelator-0.6.2/inferelator/regression/base_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import numpy as np
 import pandas as pd
 import scipy.stats
-import copy
 
-from inferelator.utils import Debug
-from inferelator.utils import Validator as check
+from inferelator.utils import (
+    Debug,
+    Validator as check
+)
+
+from inferelator.preprocessing.data_normalization import PreprocessData
 
 DEFAULT_CHUNK = 25
 PROGRESS_STR = "Regression on {gn} [{i} / {total}]"
 
 
-class BaseRegression(object):
+class BaseRegression:
     # These are all the things that have to be set in a new regression class
 
     chunk = DEFAULT_CHUNK  # int
 
     # Raw Data
     X = None  # [K x N] float
     Y = None  # [G x N] float
@@ -34,47 +37,51 @@
         # Get the IDs and total count for the genes and predictors
         self.K = X.num_genes
         self.tfs = X.gene_names
         self.G = Y.num_genes
         self.genes = Y.gene_names
 
         # Rescale the design expression or activity data on features
-        self.X = X
-        self.X.zscore()
-
+        self.X = PreprocessData.preprocess_design(X)
         self.Y = Y
 
-        Debug.vprint("Predictor matrix {pr} and response matrix {re} ready".format(pr=X.shape, re=Y.shape))
+        Debug.vprint(
+            f"Predictor matrix {X.shape} and response matrix {Y.shape} ready"
+        )
 
     def run(self):
         """
         Execute regression separately on each response variable in the data
 
         :return: pd.DataFrame [G x K], pd.DataFrame [G x K]
-            Returns the regression betas and beta error reductions for all threads if this is the master thread (rank 0)
+            Returns the regression betas and beta error reductions for all
+            threads if this is the master thread (rank 0)
             Returns None, None if it's a subordinate thread
         """
 
         return self.pileup_data(self.regress())
 
     def regress(self):
         """
-        Execute regression and return a list which can be provided to pileup_data
+        Execute regression and return a list which can be provided to
+        pileup_data
         :return: list
         """
         raise NotImplementedError
 
     def pileup_data(self, run_data):
         """
         Take the completed run data and pack it up into a DataFrame of betas
 
-        :param run_data: list
-            A list of regression result dicts ordered by gene. Each regression result should have `ind`, `pp`, `betas`
-            and `betas_resc` keys with the appropriate data.
-        :return betas, betas_rescale: (pd.DataFrame [G x K], pd.DataFrame [G x K])
+        :param run_data: A list of regression result dicts ordered by gene.
+            Each regression result should have `ind`, `pp`, `betas` and
+            `betas_resc` keys with the appropriate data.
+        :type: run_data: list
+        :return betas, betas_rescale: [G x K] DataFrames
+        :rtype: pd.DataFrame, pd.DataFrame
         """
 
         # Create G x K arrays of 0s to populate with the regression data
         betas = np.zeros((self.G, self.K), dtype=np.dtype(float))
         betas_rescale = np.zeros((self.G, self.K), dtype=np.dtype(float))
 
         # Populate the zero arrays with the BBSR betas
@@ -86,83 +93,123 @@
 
             xidx = data['ind']  # Int
             yidx = data['pp']  # Boolean array of size K
             betas[xidx, yidx] = data['betas']
             betas_rescale[xidx, yidx] = data['betas_resc']
 
         d_len, b_avg, null_m = self._summary_stats(betas)
-        Debug.vprint("Regression complete:", end=" ", level=0)
-        Debug.vprint("{d_len} Models, {b_avg} Preds per Model ({nom} Null)".format(d_len=d_len,
-                                                                                   b_avg=round(b_avg, 4),
-                                                                                   nom=null_m), level=0)
+
+        Debug.vprint(
+            "Regression complete: "
+            f"{d_len} Models, {b_avg:.02f} Preds per Model ({null_m} Null)",
+            level=0
+        )
 
         # Convert arrays into pd.DataFrames to return results
-        betas = pd.DataFrame(betas, index=self.Y.gene_names, columns=self.X.gene_names)
-        betas_rescale = pd.DataFrame(betas_rescale, index=self.Y.gene_names, columns=self.X.gene_names)
+        betas = pd.DataFrame(
+            betas,
+            index=self.Y.gene_names,
+            columns=self.X.gene_names
+        )
+
+        betas_rescale = pd.DataFrame(
+            betas_rescale,
+            index=self.Y.gene_names,
+            columns=self.X.gene_names
+        )
 
         return betas, betas_rescale
 
     @staticmethod
     def _summary_stats(arr):
         d_len = arr.shape[0]
         b_avg = np.mean(np.sum(arr != 0, axis=1))
         null_m = np.sum(np.sum(arr != 0, axis=1) == 0)
         return d_len, b_avg, null_m
 
 
 class _RegressionWorkflowMixin(object):
     """
     RegressionWorkflow implements run_regression and run_bootstrap
-    Each regression method needs to extend this to implement run_bootstrap (and also run_regression if necessary)
+    Each regression method needs to extend this to implement
+    run_bootstrap (and also run_regression if necessary)
     """
 
     def set_regression_parameters(self, **kwargs):
         """
-        Set any parameters which are specific to one or another regression method
+        Set any parameters which are specific to one or another
+        regression method
         """
         pass
 
     def run_regression(self):
         betas = []
         rescaled_betas = []
 
         for idx, bootstrap in enumerate(self.get_bootstraps()):
-            Debug.vprint('Bootstrap {} of {}'.format((idx + 1), self.num_bootstraps), level=0)
+
+            Debug.vprint(
+                f'Bootstrap {idx + 1} of {self.num_bootstraps}',
+                level=0
+            )
+
             np.random.seed(self.random_seed + idx)
+
             current_betas, current_rescaled_betas = self.run_bootstrap(bootstrap)
 
             betas.append(current_betas)
             rescaled_betas.append(current_rescaled_betas)
 
-        return betas, rescaled_betas
+        Debug.vprint(
+            'Fitting final full model',
+            level=0
+        )
+
+        full_betas, full_rescaled = self.run_bootstrap(None)
+
+        return betas, rescaled_betas, full_betas, full_rescaled
 
     def run_bootstrap(self, bootstrap):
         raise NotImplementedError
 
 
 class _MultitaskRegressionWorkflowMixin(_RegressionWorkflowMixin):
     """
-    MultitaskRegressionWorkflow implements run_regression and run_bootstrap for multitask workflow
-    Each regression method needs to extend this to implement run_bootstrap (and also run_regression if necessary)
+    MultitaskRegressionWorkflow implements run_regression and
+    run_bootstrap for multitask workflow
+
+    Each regression method needs to extend this to implement
+    run_bootstrap (and also run_regression if necessary)
     """
 
     def run_regression(self):
 
         betas = [[] for _ in range(self._n_tasks)]
         rescaled_betas = [[] for _ in range(self._n_tasks)]
 
         for idx in range(self.num_bootstraps):
-            Debug.vprint('Bootstrap {} of {}'.format((idx + 1), self.num_bootstraps), level=0)
+            Debug.vprint(
+                f'Bootstrap {idx + 1} of {self.num_bootstraps}',
+                level=0
+            )
+
             current_betas, current_rescaled_betas = self.run_bootstrap(idx)
 
             for k in range(self._n_tasks):
                 betas[k].append(current_betas[k])
                 rescaled_betas[k].append(current_rescaled_betas[k])
 
-        return betas, rescaled_betas
+        Debug.vprint(
+            'Fitting final full model',
+            level=0
+        )
+
+        full_betas, full_rescaled = self.run_bootstrap(None)
+
+        return betas, rescaled_betas, full_betas, full_rescaled
 
     def run_bootstrap(self, bootstrap):
         raise NotImplementedError
 
 
 def recalculate_betas_from_selected(x, y, idx=None):
     """
@@ -219,48 +266,68 @@
     (n, k) = x.shape
     pp_idx = index_of_nonzeros(betas).tolist()
 
     # Calculate the variance of the residuals
     ss_all = sigma_squared(x, y, betas)
     error_reduction = np.zeros(k, dtype=np.dtype(float))
 
+    # If there's only one predictor, use the ratio of explained variance
+    # to total variance (a model with zero predictors)
     if len(pp_idx) == 1:
         error_reduction[pp_idx] = 1 - (ss_all / np.var(y, ddof=1))
         return error_reduction
 
     for pp_i in range(len(pp_idx)):
         # Copy the index of predictors
-        leave_out = copy.copy(pp_idx)
+        leave_out = pp_idx.copy()
         # Pull off one of the predictors
         lost = leave_out.pop(pp_i)
 
-        # Reestimate betas for all the predictors except the one that we removed
+        # Reestimate betas for all the predictors except the one
+        # that we removed
         x_leaveout = x[:, leave_out]
+
+        # Do a standard solve holding out one of the predictors
         try:
             xt = x_leaveout.T
-            xtx = np.dot(xt, x_leaveout)
-            xty = np.dot(xt, y)
-            beta_hat = scipy.linalg.solve(xtx, xty, assume_a='sym')
+            beta_hat = scipy.linalg.solve(
+                np.dot(xt, x_leaveout),
+                np.dot(xt, y),
+                assume_a='sym'
+            )
+
+        # But if it fails use all zero coefficients
+        # it shouldn't fail at this stage though
         except np.linalg.LinAlgError:
             beta_hat = np.zeros(len(leave_out), dtype=np.dtype(float))
 
         # Calculate the variance of the residuals for the new estimated betas
         ss_leaveout = sigma_squared(x_leaveout, y, beta_hat)
 
-        # Check to make sure that the ss_all and ss_leaveout differences aren't just precision-related
-        if np.abs(ss_all - ss_leaveout) < np.finfo(float).eps * len(pp_idx):
+        # Check to make sure that the ss_all and ss_leaveout differences
+        # aren't just precision-related
+        _eps = np.finfo(float).eps * len(pp_idx)
+        if np.abs(ss_all - ss_leaveout) < _eps:
             error_reduction[lost] = 0.
+        elif ss_leaveout < _eps:
+            error_reduction[lost] = 1.
         else:
             error_reduction[lost] = 1 - (ss_all / ss_leaveout)
 
     return error_reduction
 
 
 def sigma_squared(x, y, betas):
-    return np.var(np.subtract(y, np.dot(x, betas).reshape(-1, 1)), ddof=1)
+    return np.var(
+        np.subtract(
+            y,
+            np.dot(x, betas).reshape(-1, 1)
+        ),
+        ddof=1
+    )
 
 
 def index_of_nonzeros(arr):
     """
     Returns an array that indexes all the non-zero elements of an array
     :param arr: np.ndarray
     :return: np.ndarray
```

### Comparing `inferelator-0.6.1/inferelator/regression/bayes_stats.py` & `inferelator-0.6.2/inferelator/regression/bayes_stats.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/regression/bbsr_multitask.py` & `inferelator-0.6.2/inferelator/regression/bbsr_multitask.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,87 @@
 import pandas as pd
 
-from inferelator.distributed.inferelator_mp import MPControl
 from inferelator.utils import Debug
-from inferelator.regression.base_regression import _MultitaskRegressionWorkflowMixin
-from inferelator.regression.bbsr_python import BBSR, BBSRRegressionWorkflowMixin
+from inferelator.regression.base_regression import (
+    _MultitaskRegressionWorkflowMixin
+)
+from inferelator.regression.bbsr_python import (
+    BBSR,
+    BBSRRegressionWorkflowMixin
+)
 
 
-class BBSRByTaskRegressionWorkflowMixin(_MultitaskRegressionWorkflowMixin, BBSRRegressionWorkflowMixin):
+class BBSRByTaskRegressionWorkflowMixin(
+    _MultitaskRegressionWorkflowMixin,
+    BBSRRegressionWorkflowMixin
+):
     """
-    This runs BBSR regression on tasks defined by the AMUSR regression (MTL) workflow
+    This runs BBSR regression on tasks defined by the MTL
+    workflow
     """
 
     def run_bootstrap(self, bootstrap_idx):
         betas, betas_resc = [], []
 
-        # Select the appropriate bootstrap from each task and stash the data into X and Y
         for k in range(self._n_tasks):
-            X = self._task_design[k].get_bootstrap(self._task_bootstraps[k][bootstrap_idx])
-            Y = self._task_response[k].get_bootstrap(self._task_bootstraps[k][bootstrap_idx])
+            # Select the appropriate bootstrap from each task
+            # and stash the data into X and Y
+            if bootstrap_idx is not None:
+                x = self._task_design[k].get_bootstrap(
+                    self._task_bootstraps[k][bootstrap_idx]
+                )
+                y = self._task_response[k].get_bootstrap(
+                    self._task_bootstraps[k][bootstrap_idx]
+                )
+            else:
+                x = self._task_design[k]
+                y = self._task_response[k]
 
             # Make sure that the priors align to the expression matrix
-            priors_data = self._task_priors[k].reindex(labels=self._targets, axis=0). \
-                reindex(labels=self._regulators, axis=1). \
-                fillna(value=0)
+            priors_data = self._task_priors[k].reindex(
+                labels=self._targets,
+                axis=0
+            ).reindex(
+                labels=self._regulators,
+                axis=1
+            ).fillna(value=0)
 
             if self.clr_only:
                 # Create a mock prior with no information if clr_only is set
-                priors_data = pd.DataFrame(0, index=priors_data.index, columns=priors_data.columns)
+                priors_data = pd.DataFrame(
+                    0,
+                    index=priors_data.index,
+                    columns=priors_data.columns
+                )
+
+            Debug.vprint(
+                f'Calculating task {k} ({self._task_names[k]}) '
+                'MI, Background MI, and CLR Matrix',
+                level=0
+            )
+
+            clr_matrix, _ = self.mi_driver().run(
+                y,
+                x,
+                return_mi=False
+            )
+
+            Debug.vprint(
+                f'Calculating task {k} ({self._task_names[k]}) betas'
+                'using BBSR',
+                level=0
+            )
+
+            t_beta, t_br = BBSR(
+                x,
+                y,
+                clr_matrix,
+                priors_data,
+                prior_weight=self.prior_weight,
+                no_prior_weight=self.no_prior_weight,
+                nS=self.bsr_feature_num
+            ).run()
 
-            Debug.vprint('Calculating MI, Background MI, and CLR Matrix', level=0)
-            clr_matrix, _ = self.mi_driver().run(Y, X, return_mi=False)
-
-            Debug.vprint('Calculating task {k} betas using BBSR'.format(k=k), level=0)
-            t_beta, t_br = BBSR(X, Y, clr_matrix, priors_data,
-                                prior_weight=self.prior_weight, no_prior_weight=self.no_prior_weight,
-                                nS=self.bsr_feature_num).run()
             betas.append(t_beta)
             betas_resc.append(t_br)
 
         return betas, betas_resc
```

### Comparing `inferelator-0.6.1/inferelator/regression/bbsr_python.py` & `inferelator-0.6.2/inferelator/regression/bbsr_python.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 import pandas as pd
 import numpy as np
 import itertools
 
-from inferelator import utils
+from inferelator.utils import (
+    df_set_diag,
+    Debug
+)
 from inferelator.regression import bayes_stats
-from inferelator.regression import base_regression
-from inferelator.regression import mi
+from inferelator.regression.base_regression import (
+    BaseRegression,
+    PreprocessData,
+    _RegressionWorkflowMixin,
+    gene_data_generator,
+    PROGRESS_STR
+)
+from inferelator.regression.mi import (
+    MIDriver
+)
 from inferelator.distributed.inferelator_mp import MPControl
 
 # Default number of predictors to include in the model
 DEFAULT_nS = 10
 
 # Default weight for priors & Non-priors
 # If prior_weight is the same as no_prior_weight:
-#   Priors will be included in the pp matrix before the number of predictors is reduced to nS
-#   They won't get special treatment in the model though
+# Priors will be included in the pp matrix before the number of
+# predictors is reduced to nS
+# They won't get special treatment in the model though
 DEFAULT_prior_weight = 1
 DEFAULT_no_prior_weight = 1
 
-# Throw away the priors which have a CLR that is 0 before the number of predictors is reduced by BIC
+# Throw away the priors which have a CLR that is 0 before
+# the number of predictors is reduced by BIC
 DEFAULT_filter_priors_for_clr = False
 
 
-class BBSR(base_regression.BaseRegression):
+class BBSR(BaseRegression):
     # Bayseian correlation measurements
 
     # Priors Data
     prior_mat = None  # [G x K] # numeric
     filter_priors_for_clr = DEFAULT_filter_priors_for_clr  # bool
 
     # Weights for Predictors (weights_mat is set with _calc_weight_matrix)
@@ -36,16 +49,25 @@
 
     # Predictors to include in modeling (pp is set with _build_pp_matrix)
     pp = None  # [G x K] bool
     nS = DEFAULT_nS  # int
 
     ols_only = False
 
-    def __init__(self, X, Y, clr_mat, prior_mat, nS=DEFAULT_nS, prior_weight=DEFAULT_prior_weight,
-                 no_prior_weight=DEFAULT_no_prior_weight, ordinary_least_squares=False):
+    def __init__(
+        self,
+        X,
+        Y,
+        clr_mat,
+        prior_mat,
+        nS=DEFAULT_nS,
+        prior_weight=DEFAULT_prior_weight,
+        no_prior_weight=DEFAULT_no_prior_weight,
+        ordinary_least_squares=False
+    ):
         """
         Create a Regression object for Bayes Best Subset Regression
 
         :param X: Expression or Activity data [N x K]
         :type X: InferelatorData
         :param Y: Response expression data [N x G]
         :type Y: InferelatorData
@@ -66,132 +88,189 @@
 
         self.nS = nS
         self.ols_only = ordinary_least_squares
 
         # Calculate the weight matrix
         self.prior_weight = prior_weight
         self.no_prior_weight = no_prior_weight
-        weights_mat = self._calculate_weight_matrix(prior_mat, p_weight=prior_weight, no_p_weight=no_prior_weight)
-        utils.Debug.vprint("Weight matrix {} construction complete".format(weights_mat.shape))
+        weights_mat = self._calculate_weight_matrix(
+            prior_mat,
+            p_weight=prior_weight,
+            no_p_weight=no_prior_weight
+        )
+
+        Debug.vprint(
+            f"Weight matrix {weights_mat.shape} construction complete"
+        )
 
-        # Rebuild weights, priors, and the CLR matrix for the features that are in this bootstrap
+        # Rebuild weights, priors, and the CLR matrix for the features
+        # that are in this bootstrap
         self.weights_mat = weights_mat.loc[self.genes, self.tfs]
         self.prior_mat = prior_mat.loc[self.genes, self.tfs]
         self.clr_mat = clr_mat.loc[self.genes, self.tfs]
 
-        # Build a boolean matrix indicating which tfs should be used as predictors for regression for each gene
+        # Build a boolean matrix indicating which tfs should be
+        # used as predictors for regression for each gene
         self.pp = self._build_pp_matrix()
 
     def regress(self):
         """
         Execute BBSR
 
         :return: pd.DataFrame [G x K], pd.DataFrame [G x K]
-            Returns the regression betas and beta error reductions for all threads if this is the master thread (rank 0)
-            Returns None, None if it's a subordinate thread
+            Returns the regression betas and beta error reductions
         """
 
         nG = self.G
         X = self.X.values
 
         return MPControl.map(
             _bbsr_regression_wrapper,
             itertools.repeat(X, nG),
-            base_regression.gene_data_generator(self.Y, nG),
+            gene_data_generator(self.Y, nG),
             itertools.repeat(self.pp, nG),
             itertools.repeat(self.weights_mat, nG),
             itertools.repeat(self.nS, nG),
             itertools.repeat(self.genes, nG),
             itertools.repeat(nG, nG),
             range(self.G),
             ols_only=self.ols_only,
             scatter=[X, self.pp, self.weights_mat]
         )
 
     def _build_pp_matrix(self):
         """
-        From priors and context likelihood of relatedness, determine which predictors should be included in the model
-        :return pp: pd.DataFrame [G x K]
-            Boolean matrix indicating which predictor variables should be included in BBSR for each response variable
+        From priors and context likelihood of relatedness,
+        determine which predictors should be included in the BSR
+
+        :return pp: Boolean matrix [G x K] indicating which predictor
+            variables should be included in BBSR for each response variable
+        :rtype: pd.DataFrame
         """
 
         # Create a predictor boolean array from priors
-        pp = np.logical_or(self.prior_mat != 0, self.weights_mat != self.no_prior_weight)
+        pp = np.logical_or(
+            self.prior_mat != 0,
+            self.weights_mat != self.no_prior_weight
+        )
 
         pp_idx = pp.index
         pp_col = pp.columns
 
         if self.filter_priors_for_clr:
             # Set priors which have a CLR of 0 to FALSE
             pp = np.logical_and(pp, self.clr_mat != 0).values
         else:
             pp = pp.values
 
-        # Mark the nS predictors with the highest CLR true (Do not include anything with a CLR of 0)
-        mask = np.logical_or(self.clr_mat == 0, ~np.isfinite(self.clr_mat)).values
-        masked_clr = np.ma.array(self.clr_mat.values, mask=mask)
+        # Mark the nS predictors with the highest CLR true
+        # (Do not include anything with a CLR of 0)
+        mask = np.logical_or(
+            self.clr_mat == 0,
+            ~np.isfinite(self.clr_mat)
+        ).values
+
+        masked_clr = np.ma.array(
+            self.clr_mat.values,
+            mask=mask
+        )
+
         for i in range(self.G):
-            n_to_keep = min(self.nS, self.K, mask.shape[1] - np.sum(mask[i, :]))
+            n_to_keep = min(
+                self.nS,
+                self.K,
+                mask.shape[1] - np.sum(mask[i, :])
+            )
+
             if n_to_keep == 0:
                 continue
-            clrs = np.ma.argsort(masked_clr[i, :], endwith=False)[-1 * n_to_keep:]
+
+            clrs = np.ma.argsort(
+                masked_clr[i, :],
+                endwith=False
+            )[-1 * n_to_keep:]
+
             pp[i, clrs] = True
 
         # Rebuild into a DataFrame and set autoregulation to 0
-        pp = pd.DataFrame(pp, index=pp_idx, columns=pp_col, dtype=np.dtype(bool))
-        pp = utils.df_set_diag(pp, False)
+        pp = pd.DataFrame(
+            pp,
+            index=pp_idx,
+            columns=pp_col,
+            dtype=np.dtype(bool)
+        )
+        pp = df_set_diag(pp, False)
 
         return pp
 
     @staticmethod
-    def _calculate_weight_matrix(p_matrix, no_p_weight=DEFAULT_no_prior_weight,
-                                 p_weight=DEFAULT_prior_weight):
+    def _calculate_weight_matrix(
+        p_matrix,
+        no_p_weight=DEFAULT_no_prior_weight,
+        p_weight=DEFAULT_prior_weight
+    ):
         """
-        Create a weights matrix. Everywhere p_matrix is not set to 0, the weights matrix will have p_weight. Everywhere
+        Create a weights matrix. Everywhere p_matrix is not set to 0,
+        the weights matrix will have p_weight. Everywhere
         p_matrix is set to 0, the weights matrix will have no_p_weight
-        :param p_matrix: pd.DataFrame [G x K]
-        :param no_p_weight: int
-            Weight of something which doesn't have a prior
-        :param p_weight: int
-            Weight of something which does have a prior
+
+        :param p_matrix: Predictor matrix [G x K]
+        :type p_matrix: pd.DataFrame
+        :param no_p_weight: Weight of something which doesn't have an existing
+            edge in the predictor matrix
+        :type no_p_weight: numeric
+        :param p_weight: Weight of something which does have an existing
+            edge in the predictor matrix
+        :param p_weight: numeric
         :return weights_mat: pd.DataFrame [G x K]
         """
+
         weights_mat = p_matrix * 0 + no_p_weight
         return weights_mat.mask(p_matrix != 0, other=p_weight)
 
 
-def _bbsr_regression_wrapper(X, y, pp, weights, nS, genes, nG, j, ols_only=False):
+def _bbsr_regression_wrapper(
+    X,
+    y,
+    pp,
+    weights,
+    nS,
+    genes,
+    nG,
+    j,
+    ols_only=False
+):
     """ Wrapper for multiprocessing BBSR """
 
-    utils.Debug.vprint(
-        base_regression.PROGRESS_STR.format(gn=genes[j], i=j, total=nG),
+    Debug.vprint(
+        PROGRESS_STR.format(gn=genes[j], i=j, total=nG),
         level=0 if j % 1000 == 0 else 2
     )
 
     data = bayes_stats.bbsr(
         X,
-        utils.scale_vector(y),
+        PreprocessData.preprocess_response_vector(y),
         pp.iloc[j, :].values.flatten(),
         weights.iloc[j, :].values.flatten(),
         nS,
         ordinary_least_squares=ols_only
     )
 
     data['ind'] = j
     return data
 
 
-class BBSRRegressionWorkflowMixin(base_regression._RegressionWorkflowMixin):
+class BBSRRegressionWorkflowMixin(_RegressionWorkflowMixin):
     """
     Bayesian Best Subset Regression (BBSR)
 
     https://doi.org/10.15252/msb.20156236
     """
 
-    mi_driver = mi.MIDriver
+    mi_driver = MIDriver
     mi_sync_path = None
 
     prior_weight = DEFAULT_prior_weight
     no_prior_weight = DEFAULT_no_prior_weight
     bsr_feature_num = DEFAULT_nS
     clr_only = False
     ols_only = False
@@ -230,27 +309,36 @@
         self._set_without_warning("clr_only", clr_only)
         self._set_without_warning("ols_only", ordinary_least_squares_only)
 
     def run_bootstrap(self, bootstrap):
         X = self.design.get_bootstrap(bootstrap)
         Y = self.response.get_bootstrap(bootstrap)
 
-        utils.Debug.vprint(
-            'Calculating MI, Background MI, and CLR Matrix',
+        Debug.vprint(
+            'Calculating Mutual Information, '
+            'Background Mutual Information, '
+            'and the Context Likelihood of Relatedness (CLR) Matrix',
             level=0
         )
+
         clr_matrix, _ = self.mi_driver().run(Y, X, return_mi=False)
 
-        utils.Debug.vprint(
+        Debug.vprint(
             'Calculating betas using BBSR',
             level=0
         )
 
         # Create a mock prior with no information if clr_only is set
         if self.clr_only:
+            Debug.vprint(
+                'Using Context Likelihood of Relatedness (CLR) '
+                'exclusively to identify predictors for BSR',
+                level=0
+            )
+
             priors = pd.DataFrame(
                 0,
                 index=self.priors_data.index,
                 columns=self.priors_data.columns
             )
         else:
             priors = self.priors_data
```

### Comparing `inferelator-0.6.1/inferelator/regression/elasticnet_python.py` & `inferelator-0.6.2/inferelator/regression/elasticnet_python.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/regression/mi.py` & `inferelator-0.6.2/inferelator/regression/mi.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/regression/sklearn_regression.py` & `inferelator-0.6.2/inferelator/regression/sklearn_regression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,53 @@
-import numpy as np
-from inferelator.utils import Validator as check
-from inferelator import utils
-from inferelator.regression import base_regression
-from inferelator.distributed.inferelator_mp import MPControl
-from sklearn.base import BaseEstimator
-from inferelator.regression.base_regression import _MultitaskRegressionWorkflowMixin
-import copy
 import inspect
 import itertools
+import numpy as np
+from sklearn.base import BaseEstimator
 
-
-def sklearn_gene(x, y, model, min_coef=None, **kwargs):
+from inferelator.utils import (
+    Debug,
+    Validator as check,
+    make_array_2d
+)
+from inferelator.distributed.inferelator_mp import MPControl
+from inferelator.regression.base_regression import (
+    BaseRegression,
+    PreprocessData,
+    _RegressionWorkflowMixin,
+    _MultitaskRegressionWorkflowMixin,
+    recalculate_betas_from_selected,
+    predict_error_reduction,
+    gene_data_generator,
+    PROGRESS_STR
+)
+
+
+def sklearn_gene(
+    x,
+    y,
+    model,
+    min_coef=None,
+    **kwargs
+):
     """
     Use a scikit-learn model for regression
 
     :param x: Feature array
     :type x: np.ndarray [N x K]
     :param y: Response array
     :type y: np.ndarray [N x 1]
     :param model: Instance of a scikit BaseEstimator-derived model
     :type model: BaseEstimator
-    :param min_coef: A minimum coefficient value to include in the model. Any values smaller will be set to 0.
+    :param min_coef: A minimum coefficient value to include in the model.
+        Any values smaller will be set to 0.
     :type min_coef: numeric
     :return: A dict of results for this gene
     :rtype: dict
     """
+
     assert check.argument_type(x, np.ndarray)
     assert check.argument_type(y, np.ndarray)
     assert check.argument_is_subclass(model, BaseEstimator)
 
     (N, K) = x.shape
 
     # Fit the model
@@ -38,149 +57,222 @@
     try:
         coefs = model.coef_
     except AttributeError:
         coefs = model.estimator_.coef_
 
     # Set coefficients below threshold to 0
     if min_coef is not None:
-        coefs[np.abs(coefs) < min_coef] = 0.  # Threshold coefficients
+        coefs[np.abs(coefs) < min_coef] = 0.
 
-    coef_nonzero = coefs != 0  # Create a boolean array where coefficients are nonzero [K, ]
+    # Create a boolean array where coefficients are nonzero [K, ]
+    coef_nonzero = coefs != 0
 
-    # If there are non-zero coefficients, redo the linear regression with them alone
-    # And calculate beta_resc
+    # If there are non-zero coefficients, redo the linear regression
+    # with them alone and calculate beta_resc
     if coef_nonzero.sum() > 0:
         x = x[:, coef_nonzero]
-        utils.make_array_2d(y)
-        betas = base_regression.recalculate_betas_from_selected(x, y)
-        betas_resc = base_regression.predict_error_reduction(x, y, betas)
-        return dict(pp=coef_nonzero,
-                    betas=betas,
-                    betas_resc=betas_resc)
+        make_array_2d(y)
+        betas = recalculate_betas_from_selected(x, y)
+        betas_resc = predict_error_reduction(x, y, betas)
+        return dict(
+            pp=coef_nonzero,
+            betas=betas,
+            betas_resc=betas_resc
+        )
+
     else:
-        return dict(pp=np.repeat(True, K).tolist(),
-                    betas=np.zeros(K),
-                    betas_resc=np.zeros(K))
+        return dict(
+            pp=np.repeat(True, K).tolist(),
+            betas=np.zeros(K),
+            betas_resc=np.zeros(K)
+        )
 
 
-class SKLearnRegression(base_regression.BaseRegression):
+class SKLearnRegression(BaseRegression):
 
     def __init__(self, x, y, model, random_state=None, **kwargs):
         self.params = kwargs
 
         if random_state is not None:
             self.params["random_state"] = random_state
 
         self.min_coef = self.params.pop("min_coef", None)
-        self.model = model(**self.params)
+        self.model = model
 
         super(SKLearnRegression, self).__init__(x, y)
 
     def regress(self):
         """
         Execute Elastic Net
 
         :return: list
-            Returns a list of regression results that base_regression's pileup_data can process
+            Returns a list of regression results that base_regression's
+            pileup_data can process
         """
 
         nG = self.G
         X = self.X.values
 
         return MPControl.map(
             _sklearn_regression_wrapper,
             itertools.repeat(X, nG),
-            base_regression.gene_data_generator(self.Y, nG),
+            gene_data_generator(self.Y, nG),
             itertools.repeat(self.model, nG),
             itertools.repeat(self.genes, nG),
             itertools.repeat(nG, nG),
             range(self.G),
+            params=self.params,
             min_coef=self.min_coef,
             scatter=[X]
         )
 
 
-def _sklearn_regression_wrapper(X, y, model, genes, nG, j, min_coef=None):
+def _sklearn_regression_wrapper(
+    X,
+    y,
+    model,
+    genes,
+    nG,
+    j,
+    params={},
+    min_coef=None
+):
         """ Wrapper for multiprocessing sklearn models """
-        utils.Debug.vprint(
-            base_regression.PROGRESS_STR.format(gn=genes[j], i=j, total=nG),
+        Debug.vprint(
+            PROGRESS_STR.format(gn=genes[j], i=j, total=nG),
             level=0 if j % 1000 == 0 else 2
         )
 
         data = sklearn_gene(
             X,
-            utils.scale_vector(y),
-            copy.copy(model),
+            PreprocessData.preprocess_response_vector(y),
+            model(**params),
             min_coef=min_coef
         )
 
         data['ind'] = j
         return data
 
 
-class SKLearnWorkflowMixin(base_regression._RegressionWorkflowMixin):
+class SKLearnWorkflowMixin(_RegressionWorkflowMixin):
     """
     Use any scikit-learn regression module
     """
 
     _sklearn_model = None
     _sklearn_model_params = None
     _sklearn_add_random_state = False
 
     def __init__(self, *args, **kwargs):
         self._sklearn_model_params = {}
         super(SKLearnWorkflowMixin, self).__init__(*args, **kwargs)
 
-    def set_regression_parameters(self, model=None, add_random_state=None, **kwargs):
+    def set_regression_parameters(
+        self,
+        model=None,
+        add_random_state=None,
+        **kwargs
+    ):
         """
         Set parameters to use a sklearn model for regression
 
         :param model: A scikit-learn model class
         :type model: BaseEstimator subclass
-        :param add_random_state: Flag to include workflow random seed as "random_state" in the model
+        :param add_random_state: Flag to include workflow random seed
+            as "random_state" in the model
         :type add_random_state: bool
-        :param kwargs: Any arguments which should be passed to the scikit-learn model class instantiation
+        :param kwargs: Any arguments which should be passed to the
+            scikit-learn model class instantiation
         :type kwargs: any
         """
 
         if model is not None and not inspect.isclass(model):
-            raise ValueError("Pass an uninstantiated scikit-learn model (i.e. LinearRegression, not LinearRegression()")
-
-        self._set_with_warning("_sklearn_model", model)
-        self._set_without_warning("_sklearn_add_random_state", add_random_state)
-        self._sklearn_model_params.update(kwargs)
+            raise ValueError(
+                "Pass an uninstantiated scikit-learn model "
+                "(i.e. LinearRegression, not LinearRegression()"
+            )
+
+        self._set_with_warning(
+            "_sklearn_model",
+            model
+        )
+        self._set_without_warning(
+            "_sklearn_add_random_state",
+            add_random_state
+        )
+        self._sklearn_model_params.update(
+            kwargs
+        )
 
     def run_bootstrap(self, bootstrap):
         x = self.design.get_bootstrap(bootstrap)
         y = self.response.get_bootstrap(bootstrap)
-        utils.Debug.vprint('Calculating betas using SKLearn model {m}'.format(m=self._sklearn_model.__name__), level=0)
-
-        return SKLearnRegression(x,
-                                 y,
-                                 self._sklearn_model,
-                                 random_state=self.random_seed if self._sklearn_add_random_state else None,
-                                 **self._sklearn_model_params).run()
 
+        Debug.vprint(
+            'Calculating betas using SKLearn model '
+            f'{self._sklearn_model.__name__}',
+            level=0
+        )
 
-class SKLearnByTaskMixin(_MultitaskRegressionWorkflowMixin, SKLearnWorkflowMixin):
+        if self._sklearn_add_random_state:
+            seed = self.random_seed
+        else:
+            seed = None
+
+        return SKLearnRegression(
+            x,
+            y,
+            self._sklearn_model,
+            random_state=seed,
+            **self._sklearn_model_params
+        ).run()
+
+
+class SKLearnByTaskMixin(
+    _MultitaskRegressionWorkflowMixin,
+    SKLearnWorkflowMixin
+):
     """
-    This runs BBSR regression on tasks defined by the AMUSR regression (MTL) workflow
+    This runs scikit models on tasks defined by the MTL workflow
     """
 
     def run_bootstrap(self, bootstrap_idx):
         betas, betas_resc = [], []
 
-        # Select the appropriate bootstrap from each task and stash the data into X and Y
+        if self._sklearn_add_random_state:
+            seed = self.random_seed
+        else:
+            seed = None
+
         for k in range(self._n_tasks):
-            x = self._task_design[k].get_bootstrap(self._task_bootstraps[k][bootstrap_idx])
-            y = self._task_response[k].get_bootstrap(self._task_bootstraps[k][bootstrap_idx])
 
-            utils.Debug.vprint('Calculating task {k} using {n}'.format(k=k, n=self._sklearn_model.__name__), level=0)
-            t_beta, t_br = SKLearnRegression(x,
-                                             y,
-                                             self._sklearn_model,
-                                             random_state=self.random_seed if self._sklearn_add_random_state else None,
-                                             **self._sklearn_model_params).run()
+            # Select the appropriate bootstrap from each task
+            # and stash the data into X and Y
+            if bootstrap_idx is not None:
+                x = self._task_design[k].get_bootstrap(
+                    self._task_bootstraps[k][bootstrap_idx]
+                )
+                y = self._task_response[k].get_bootstrap(
+                    self._task_bootstraps[k][bootstrap_idx]
+                )
+            else:
+                x = self._task_design[k]
+                y = self._task_response[k]
+
+            Debug.vprint(
+                f'Calculating task {k} using '
+                f'{self._sklearn_model.__name__}',
+                level=0
+            )
+
+            t_beta, t_br = SKLearnRegression(
+                x,
+                y,
+                self._sklearn_model,
+                random_state=seed,
+                **self._sklearn_model_params
+            ).run()
+
             betas.append(t_beta)
             betas_resc.append(t_br)
 
         return betas, betas_resc
```

### Comparing `inferelator-0.6.1/inferelator/regression/stability_selection.py` & `inferelator-0.6.2/inferelator/regression/stability_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,25 @@
 from sklearn.linear_model import (
     LinearRegression as _LinearRegression,
     Lasso as _Lasso,
     Ridge as _Ridge,
     lasso_path
 )
 
-from inferelator.regression import base_regression
+from inferelator.regression.base_regression import (
+    BaseRegression,
+    PreprocessData,
+    _RegressionWorkflowMixin,
+    _MultitaskRegressionWorkflowMixin,
+    recalculate_betas_from_selected,
+    predict_error_reduction,
+    gene_data_generator,
+    PROGRESS_STR
+)
+
 from inferelator.distributed.inferelator_mp import MPControl
 from inferelator import utils
 
 _DEFAULT_ALPHAS = np.insert(np.logspace(-2, 1, 20), 0, 0)
 _DEFAULT_NUM_SUBSAMPLES = 20
 _DEFAULT_THRESHOLD = 0.05
 _DEFAULT_SEED = 42
@@ -246,16 +256,16 @@
     if beta_nonzero.sum() == 0:
         return dict(pp=np.repeat(True, k).tolist(),
                     betas=np.zeros(k),
                     betas_resc=np.zeros(k))
     else:
         x = x[:, beta_nonzero]
         utils.make_array_2d(y)
-        betas = base_regression.recalculate_betas_from_selected(x, y)
-        betas_resc = base_regression.predict_error_reduction(x, y, betas)
+        betas = recalculate_betas_from_selected(x, y)
+        betas_resc = predict_error_reduction(x, y, betas)
 
         return dict(pp=beta_nonzero,
                     betas=betas,
                     betas_resc=betas_resc)
 
 
 def _calculate_stability(edges):
@@ -290,15 +300,15 @@
         subsample_index[start:stop] = list(range(num_subsamples))[0:stop - start]
 
     np.random.RandomState(random_seed).shuffle(subsample_index)
 
     return subsample_index
 
 
-class StARS(base_regression.BaseRegression):
+class StARS(BaseRegression):
 
     def __init__(
         self,
         X,
         Y,
         random_seed,
         alphas=_DEFAULT_ALPHAS,
@@ -327,46 +337,46 @@
 
         x = self.X.values
         nG = self.G
 
         return MPControl.map(
             _stars_regression_wrapper,
             itertools.repeat(x, nG),
-            base_regression.gene_data_generator(self.Y, nG),
+            gene_data_generator(self.Y, nG),
             itertools.repeat(self.alphas, nG),
             range(nG),
             self.genes,
             itertools.repeat(nG, nG),
             method=self.method,
             num_subsamples=self.num_subsamples,
             random_seed=self.random_seed,
             **self.params,
             scatter=[x]
         )
 
 
 def _stars_regression_wrapper(x, y, alphas, j, gene, nG, **kwargs):
 
-            utils.Debug.vprint(
-                base_regression.PROGRESS_STR.format(gn=gene, i=j, total=nG),
-                level=0 if j % 1000 == 0 else 2
-            )
+    utils.Debug.vprint(
+        PROGRESS_STR.format(gn=gene, i=j, total=nG),
+        level=0 if j % 1000 == 0 else 2
+    )
 
-            data = stars_model_select(
-                x,
-                utils.scale_vector(y),
-                alphas,
-                **kwargs
-            )
+    data = stars_model_select(
+        x,
+        PreprocessData.preprocess_response_vector(y),
+        alphas,
+        **kwargs
+    )
 
-            data['ind'] = j
-            return data
+    data['ind'] = j
+    return data
 
 
-class StARSWorkflowMixin(base_regression._RegressionWorkflowMixin):
+class StARSWorkflowMixin(_RegressionWorkflowMixin):
     """
     Stability Approach to Regularization Selection (StARS)-LASSO.
     StARS-Ridge is implemented on an experimental basis.
 
     https://arxiv.org/abs/1006.3316
     https://doi.org/10.1016/j.immuni.2019.06.001
     """
@@ -431,57 +441,50 @@
             self.random_seed,
             alphas=self.alphas,
             method=self.regress_method,
             num_subsamples=self.num_subsamples,
             parameters=self.sklearn_params
         ).run()
 
-        return [betas], [resc_betas]
+        return [betas], [resc_betas], betas, resc_betas
 
 
 class StARSWorkflowByTaskMixin(
-    base_regression._MultitaskRegressionWorkflowMixin,
+    _MultitaskRegressionWorkflowMixin,
     StARSWorkflowMixin
 ):
     """
     Stability Approach to Regularization Selection (StARS)-LASSO.
     StARS-Ridge is implemented on an experimental basis.
 
     https://arxiv.org/abs/1006.3316
     https://doi.org/10.1016/j.immuni.2019.06.001
     """
 
-    def run_bootstrap(self, bootstrap_idx):
+    def run_regression(self):
         betas, betas_resc = [], []
 
         # Run tasks individually
         for k in range(self._n_tasks):
 
-            # Select the appropriate bootstrap from each task
-            # and stash the data into X and Y
-            x = self._task_design[k].get_bootstrap(
-                self._task_bootstraps[k][bootstrap_idx]
-            )
-
-            y = self._task_response[k].get_bootstrap(
-                self._task_bootstraps[k][bootstrap_idx]
-            )
-
             utils.Debug.vprint(
                 f'Calculating task {k} betas using StARS',
                 level=0
             )
 
             t_beta, t_br = StARS(
-                x,
-                y,
+                self._task_design[k],
+                self._task_response[k],
                 self.random_seed,
                 alphas=self.alphas,
                 method=self.regress_method,
                 num_subsamples=self.num_subsamples,
                 parameters=self.sklearn_params
             ).run()
 
-            betas.append(t_beta)
-            betas_resc.append(t_br)
+            betas.append([t_beta])
+            betas_resc.append([t_br])
+
+        _unpack_betas = [x[0] for x in betas]
+        _unpack_var_exp = [x[0] for x in betas_resc]
 
-        return betas, betas_resc
+        return betas, betas_resc, _unpack_betas, _unpack_var_exp
```

### Comparing `inferelator-0.6.1/inferelator/tests/artifacts/test_data.py` & `inferelator-0.6.2/inferelator/tests/artifacts/test_data.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/tests/artifacts/test_stubs.py` & `inferelator-0.6.2/inferelator/tests/artifacts/test_stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 class FakeRegressionMixin(_RegressionWorkflowMixin):
 
     def run_regression(self):
         beta = [pd.DataFrame(np.array([[0, 1], [0.5, 0.05]]), index=['gene1', 'gene2'], columns=['tf1', 'tf2'])]
         beta_resc = [pd.DataFrame(np.array([[0, 1], [1, 0.05]]), index=['gene1', 'gene2'], columns=['tf1', 'tf2'])]
-        return beta, beta_resc
+        return beta, beta_resc, beta[0], beta_resc[0]
 
     def run_bootstrap(self, bootstrap):
         return True
 
 
 class FakeResultProcessor:
     network_data = None
```

### Comparing `inferelator-0.6.1/inferelator/tfa/ridge_tfa.py` & `inferelator-0.6.2/inferelator/tfa/ridge_tfa.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/tfa/tfa_base.py` & `inferelator-0.6.2/inferelator/tfa/tfa_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from abc import abstractmethod
 import numpy as np
-from inferelator import utils
+
+from inferelator.utils import (
+    InferelatorData,
+    Debug,
+    df_set_diag
+)
+
+from inferelator.preprocessing import (
+    PreprocessData
+)
 
 class TFABase:
     """
     TFA calculates transcription factor activity
     """
 
     def compute_transcription_factor_activity(
@@ -23,30 +32,31 @@
         prior,
         expression_data,
         keep_self=False,
         use_expression=True
     ):
 
         if not keep_self:
-            prior = utils.df_set_diag(prior, 0)
+            prior = df_set_diag(prior, 0)
 
         activity_tfs, expr_tfs, drop_tfs = self._determine_tf_status(
             prior,
             expression_data
         )
 
         if not use_expression:
             drop_tfs = drop_tfs.append(expr_tfs)
 
         if len(drop_tfs) > 0:
-            utils.Debug.vprint(
-                f"{len(drop_tfs)} TFs are removed from activity ",
+            Debug.vprint(
+                f"{len(drop_tfs)} TFs are removed from activity "
+                f"as they cannot be estimated",
                 level=0
             )
-            utils.Debug.vprint(" ".join(drop_tfs), level=1)
+            Debug.vprint(" ".join(drop_tfs), level=1)
 
         prior = prior.drop(drop_tfs, axis=1)
 
         return prior, activity_tfs, expr_tfs
 
     @staticmethod
     def _determine_tf_status(prior, expression_data):
@@ -72,15 +82,16 @@
         expression_data
     ):
         """
         Calculate activity from prior and expression data
 
         :param prior: Prior knowledge matrix
         :type prior: np.ndarray
-        :param expression_data: Gene expression data
+        :param expression_data: Gene expression data,
+            already normalized
         :type expression_data: np.ndarray, sp.spmatrix
         """
 
         raise NotImplementedError
 
 
 class ActivityExpressionTFA(TFABase):
@@ -126,46 +137,47 @@
             if expression_data_halftau is not None:
                 expr = expression_data_halftau
             else:
                 expr = expression_data
 
             activity[:, a_cols] = self._calculate_activity(
                 trim_prior.loc[:, activity_tfs].values,
-                expr.values
+                PreprocessData.preprocess_expression_array(
+                    expr.values
+                )
             )
 
         # Use TF expression in place of activity for features
         # which don't have activity
         if len(expr_tfs) > 0:
-            activity[
-                :,
-                trim_prior.columns.isin(expr_tfs)
-            ] = expression_data.get_gene_data(
-                expr_tfs,
-                force_dense=True
+            e_cols = trim_prior.columns.isin(expr_tfs)
+            activity[:, e_cols] = PreprocessData.preprocess_expression_array(
+                expression_data.get_gene_data(
+                    expr_tfs,
+                    force_dense=True
+                )
             )
 
         if expression_data.name is None:
             _data_name = "Activity"
         else:
             _data_name = f"{expression_data.name} Activity"
 
-        acti = utils.InferelatorData(
+        activity = InferelatorData(
             activity,
             gene_names=trim_prior.columns,
             sample_names=expression_data.sample_names,
             meta_data=expression_data.meta_data,
             name=_data_name
         )
 
-        acti.prior_data = prior.copy()
-        acti.tfa_prior_data = trim_prior.loc[:, activity_tfs].copy()
-
-        return acti
+        activity.prior_data = prior.copy()
+        activity.tfa_prior_data = trim_prior.loc[:, activity_tfs].copy()
 
+        return activity
 
 
 class ActivityOnlyTFA(TFABase):
 
     def compute_transcription_factor_activity(
         self,
         prior,
@@ -181,63 +193,72 @@
             keep_self=keep_self,
             use_expression=False
         )
 
         if len(activity_tfs) > 0:
             activity = self._calculate_activity(
                 prior.loc[:, activity_tfs].values,
-                expression_data.values
+                PreprocessData.preprocess_expression_array(
+                    expression_data.values
+                )
             )
         else:
             raise ValueError(
                 "TFA cannot be calculated; prior matrix has no edges"
             )
 
         if expression_data.name is None:
             _data_name = "Activity"
         else:
             _data_name = f"{expression_data.name} Activity"
 
-        return utils.InferelatorData(
+        activity = InferelatorData(
             activity,
             gene_names=activity_tfs,
             sample_names=expression_data.sample_names,
             meta_data=expression_data.meta_data,
             name=_data_name
         )
 
+        activity.prior_data = prior.copy()
+        activity.tfa_prior_data = prior.loc[:, activity_tfs].copy()
+
+        return activity
+
 
 class NoTFA(TFABase):
     """ NoTFA creates an activity matrix from the expression data only """
 
     def compute_transcription_factor_activity(
         self,
         prior,
         expression_data,
         expression_data_halftau=None,
         keep_self=False
     ):
 
-        utils.Debug.vprint(
+        Debug.vprint(
             "Setting Activity to Expression Values",
             level=1
         )
 
         tf_gene_overlap = prior.columns[
             prior.columns.isin(expression_data.gene_names)
         ]
 
         if expression_data.name is None:
             _data_name = "Activity"
         else:
             _data_name = f"{expression_data.name} Activity"
 
-        return utils.InferelatorData(
-            expression_data.get_gene_data(
-                tf_gene_overlap,
-                force_dense=True
+        return InferelatorData(
+            PreprocessData.preprocess_expression_array(
+                expression_data.get_gene_data(
+                    tf_gene_overlap,
+                    force_dense=True
+                )
             ),
             sample_names=expression_data.sample_names,
             meta_data=expression_data.meta_data,
             gene_names=tf_gene_overlap,
             name=_data_name
         )
```

### Comparing `inferelator-0.6.1/inferelator/tfa/velocity_tfa.py` & `inferelator-0.6.2/inferelator/tfa/velocity_tfa.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/utils/data.py` & `inferelator-0.6.2/inferelator/utils/inferelator_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,333 +1,30 @@
-import copy as cp
 import gc
-import math
 import pandas as pd
 import numpy as np
-import scipy.sparse as sparse
-import scipy.stats
 import pandas.api.types as pat
+
 from sklearn.preprocessing import StandardScaler
-import scipy.io
 from anndata import AnnData
-from inferelator.utils import Debug
-from inferelator.utils import Validator as check
-
-
-def dot_product(a, b, dense=True, cast=True):
-    """
-    Dot product two matrices together.
-    Allow either matrix (or both or neither) to be sparse.
-
-    :param a:
-    :param b:
-    :param dense:
-    :param cast:
-    :return:
-    """
-    if sparse.isspmatrix(a) and sparse.isspmatrix(b):
-        return a.dot(b).A if dense else a.dot(b)
-    elif sparse.isspmatrix(a) and dense:
-        return a.dot(sparse.csr_matrix(b)).A
-    elif sparse.isspmatrix(a):
-        return a.dot(sparse.csr_matrix(b))
-    elif sparse.isspmatrix(b):
-        return np.dot(a, b.A)
-    else:
-        return np.dot(a, b)
-
-
-class DotProduct:
-
-    _dot_func = dot_product
-
-    @classmethod
-    def set_mkl(cls, mkl=True):
-
-        # If the MKL flag is None, don't change anything
-        if mkl is None:
-            pass
-
-        # If the MKL flag is True, use the dot_product_mkl function
-        # when .dot() is called
-        if mkl:
-            try:
-                from sparse_dot_mkl import (
-                    get_version_string,
-                    dot_product_mkl
-                )
-
-                vstring = get_version_string()
-
-                if vstring is None:
-                    vstring = "Install mkl-service for details"
-
-                Debug.vprint(
-                    "Matrix multiplication will use sparse_dot_mkl "
-                    "package with MKL: {vstring}",
-                    level=2
-                )
-
-                cls._dot_func = dot_product_mkl
-
-            # If it isn't available, use the
-            # scipy/numpy functions instead
-            except ImportError as err:
-                Debug.vprint(
-                    "Unable to load MKL with sparse_dot_mkl:\n" +
-                    str(err),
-                    level=0
-                )
-
-                cls._dot_func = dot_product
-
-        # If the MKL flag is False, use the python (numpy/scipy)
-        # functions when .dot() is called
-        else:
-            Debug.vprint(
-                "Matrix multiplication will use numpy; "
-                "this is not advised for sparse data",
-                level=2
-            )
-            cls._dot_func = dot_product
-
-    @classmethod
-    def dot(cls, *args, **kwargs):
-        return cls._dot_func(*args, **kwargs)
-
-
-def df_from_tsv(file_like, has_index=True):
-    """
-    Read a tsv file or buffer with headers
-    and row ids into a pandas dataframe.
-    """
-
-    return pd.read_csv(
-        file_like,
-        sep="\t",
-        header=0,
-        index_col=0 if has_index else False
-    )
-
-
-def df_set_diag(df, val, copy=True):
-    """
-    Sets the diagonal of a dataframe to a value.
-    Diagonal in this case is anything where row label == column label.
-
-    :param df: pd.DataFrame
-        DataFrame to modify
-    :param val: numeric
-        Value to insert into any cells where row label == column label
-    :param copy: bool
-        Force-copy the dataframe instead of modifying in place
-    :return: pd.DataFrame / int
-        Return either the modified dataframe (if copied) or
-        the number of cells modified (if changed in-place)
-    """
-
-    # Find all the labels that are shared between rows and columns
-    isect = df.index.intersection(df.columns)
-
-    if copy:
-        df = df.copy()
-
-    # Set the value where row and column names are the same
-    for i in range(len(isect)):
-        df.loc[isect[i], isect[i]] = val
-
-    if copy:
-        return df
-    else:
-        return len(isect)
-
-
-def array_set_diag(arr, val, row_labels, col_labels):
-    """
-    Sets the diagonal of an 2D array to a value.
-    Diagonal in this case is anything where row label == column label.
-
-    :param arr: Array to modify in place
-    :type arr: np.ndarray
-    :param val: Value to insert into any cells where
-        row label == column label
-    :type val: numeric
-    :param row_labels: Labels which correspond to the rows
-    :type row_labels: list, pd.Index
-    :param col_labels: Labels which correspond to the columns
-    :type col_labels: list, pd.Index
-    :return: Return the number of common row and column labels
-    :rtype: int
-    """
-
-    if arr.ndim != 2:
-        raise ValueError("Array must be 2D")
-
-    # Find all the labels that are shared between rows and columns
-    isect = set(row_labels).intersection(col_labels)
-
-    # Set the value where row and column names are the same
-    for i in isect:
-        arr[row_labels == i, col_labels == i] = val
-
-    return len(isect)
-
-
-def make_array_2d(arr):
-    """
-    Changes array shape from 1d to 2d if needed (in-place)
-    :param arr:  np.ndarray
-    """
-    if arr.ndim == 1:
-        arr.shape = (arr.shape[0], 1)
-
-
-def melt_and_reindex_dataframe(
-    data_frame,
-    value_name,
-    idx_name="target",
-    col_name="regulator"
-):
-    """
-    Take a pandas dataframe and melt it into a one column dataframe
-        (with the column `value_name`) and a multiindex
-    of the original index + column
-    :param data_frame: pd.DataFrame [M x N]
-        Meltable dataframe
-    :param value_name: str
-        The column name for the values of the dataframe
-    :param idx_name: str
-        The name to assign to the original data_frame index values
-    :param col_name: str
-        The name to assign to the original data_frame column values
-    :return: pd.DataFrame [(M*N) x 1]
-        Melted dataframe with a single column of values and a multiindex
-        that is the original index + column for that value
-    """
-
-    # Copy the dataframe and move the index to a column
-    data_frame = data_frame.copy()
-    data_frame[idx_name] = data_frame.index
-
-    # Melt it into a [(M*N) x 3] dataframe
-    data_frame = data_frame.melt(
-        id_vars=idx_name,
-        var_name=col_name,
-        value_name=value_name
-    )
-
-    # Create a multiindex and then drop the columns
-    # that are now in the index
-    data_frame.index = pd.MultiIndex.from_frame(
-        data_frame.loc[:, [idx_name, col_name]]
-    )
-
-    del data_frame[idx_name]
-    del data_frame[col_name]
-
-    return data_frame
-
-
-def scale_vector(vec, ddof=1):
-    """
-    Take a vector and normalize it to a mean 0 and standard deviation 1 (z-score)
-
-    :param vec: A 1d vector to be normalized
-    :type vec: np.ndarray, sp.sparse.spmatrix
-    :param ddof: The delta degrees of freedom for variance calculation
-    :type ddof: int
-    :return: A centered and scaled vector
-    :rtype: np.ndarray
-    """
-
-    # Convert a sparse vector to a dense vector
-    if sparse.isspmatrix(vec):
-        vec = vec.A
-
-    # Return 0s if the variance is 0
-    if np.var(vec) == 0:
-        return np.zeros(vec.shape, dtype=float)
-
-    # Otherwise scale with scipy.stats.zscore
-    else:
-        return scipy.stats.zscore(vec, axis=None, ddof=ddof)
-
-
-def apply_window_vector(
-    vec,
-    window,
-    func
-):
-    """
-    Apply a function to a 1d array by windows.
-    For logical testing of an array without having
-    to allocate a full array of bools
-
-    :param vec: A 1d vector to be normalized
-    :type vec: np.ndarray, sp.sparse.spmatrix
-    :param window: The window size to process
-    :type window: int
-    :param func: A function that produces an aggregate
-        result for the window
-    :type func: callable
-    :return:
-    """
-
-    return np.array(
-        [func(vec[i * window:min((i + 1) * window, len(vec))])
-        for i in range(math.ceil(len(vec) / window))]
-    )
-
-def safe_apply_to_array(
-    array,
-    func,
-    *args,
-    axis=0,
-    dtype=None,
-    **kwargs
-):
-    """
-    Applies a function to a 2d array
-    Safe for both sparse and dense
-    """
-
-    if sparse.issparse(array):
-
-        if dtype is None:
-            dtype = array.dtype
-
-        out_arr = np.empty(array.shape, dtype=dtype)
-
-        if axis == 0:
-            for i in range(array.shape[1]):
-                out_arr[:, i] = func(
-                    array[:, i].A.ravel(),
-                    *args,
-                    **kwargs
-                )
-
-        elif axis == 1:
-            for i in range(array.shape[0]):
-                out_arr[i, :] = func(
-                    array[i, :].A.ravel(),
-                    *args,
-                    **kwargs
-                )
-
-        return out_arr
-
-    else:
-        return np.apply_along_axis(
-            func,
-            axis,
-            array,
-            *args,
-            **kwargs
-        )
 
+from scipy import (
+    sparse,
+    io
+)
+
+from inferelator.utils import (
+    Debug,
+    Validator as check
+)
+
+from inferelator.utils.data import (
+    apply_window_vector,
+    DotProduct,
+    convert_array_to_float
+)
 
 
 class InferelatorData(object):
     """
     Store inferelator data in an AnnData object.
     This will always be Samples by Genes
     """
@@ -365,19 +62,19 @@
             self._adata.X.data = new_data
         else:
             self._adata.X = new_data
 
     @property
     def _data_mem_usage(self):
         if self.is_sparse:
-            return sum(
+            return np.sum((
                 self._adata.X.data.nbytes,
                 self._adata.X.indices.nbytes,
                 self._adata.X.indptr.nbytes
-            )
+            ))
         else:
             return self._adata.X.nbytes
 
     @property
     def prior_data(self):
 
         if "prior_data" in self._adata.uns:
@@ -631,15 +328,15 @@
         :type dtype: np.dtype
         :param name: Name of this data structure.
         :type name: None, str
         """
 
         # Empty anndata object
         if expression_data is None:
-            self._adata = AnnData(dtype=dtype)
+            self._adata = AnnData()
 
         # Convert a dataframe to an anndata object
         elif isinstance(expression_data, pd.DataFrame):
             object_cols = expression_data.dtypes == object
 
             # Pull out any object columns and use them as metadata
             if sum(object_cols) > 0:
@@ -651,47 +348,57 @@
                     meta_data = pd.concat((meta_data, object_data), axis=1)
 
                 expression_data.drop(
                     expression_data.columns[object_cols],
                     inplace=True, axis=1
                 )
 
+            # If dtype is provided, use it
             if dtype is not None:
                 pass
-            elif all(map(lambda x: pat.is_integer_dtype(x), expression_data.dtypes)):
+
+            # If all dtypes are integer use int32
+            elif all(map(
+                lambda x: pat.is_integer_dtype(x),
+                expression_data.dtypes
+            )):
                 dtype = 'int32'
+
+            # Otherwise use floats
             else:
                 dtype = 'float64'
 
             self._make_idx_str(expression_data)
 
             if transpose_expression:
                 self._adata = AnnData(
-                    X=expression_data.T,
-                    dtype=dtype
+                    X=expression_data.T.values.astype(dtype)
                 )
+                self._adata.obs_names = expression_data.columns
+                self._adata.var_names = expression_data.index
+
             else:
                 self._adata = AnnData(
-                    X=expression_data,
-                    dtype=dtype
+                    X=expression_data.values.astype(dtype)
                 )
+                self._adata.obs_names = expression_data.index
+                self._adata.var_names = expression_data.columns
 
         # Use an anndata object that already exists
         elif isinstance(expression_data, AnnData):
             self._adata = expression_data
 
         # Convert a numpy array to an anndata object
         else:
 
             if transpose_expression:
                 expression_data = expression_data.T
 
             self._adata = AnnData(
-                X=expression_data,
-                dtype=expression_data.dtype
+                X=expression_data
             )
 
         # Use gene_names as var_names
         if gene_names is not None and len(gene_names) > 0:
             self._adata.var_names = gene_names
 
         # Use sample_names as obs_names
@@ -702,68 +409,60 @@
         if meta_data is not None:
             self._make_idx_str(meta_data)
             self.meta_data = meta_data
 
         # Use gene_data as var
         if gene_data is not None:
 
-            if gene_data_idx_column is not None and gene_data_idx_column in gene_data:
-                gene_data.index = gene_data[gene_data_idx_column]
+            if gene_data_idx_column is not None:
 
-            elif gene_data_idx_column is not None:
-                raise ValueError(
-                    f"No gene_data column {gene_data_idx_column} "
-                    f"in {' '.join(gene_data.columns)}"
-                )
+                try:
+                    gene_data.index = gene_data[gene_data_idx_column]
+
+                except KeyError:
+                    raise ValueError(
+                        f"No gene_data column {gene_data_idx_column} "
+                        f"in {' '.join(gene_data.columns)}"
+                    )
 
             self._make_idx_str(gene_data)
             self.gene_data = gene_data
 
         self._cached = {}
         self.name = name
 
     def convert_to_float(self):
         """
         Convert the data in-place to a float dtype
         """
 
-        if pat.is_float_dtype(self._data.dtype):
-            return None
-        elif self._data.dtype == np.int32:
-            dtype = np.float32
-        elif self._data.dtype == np.int64:
-            dtype = np.float64
-        else:
-            raise ValueError("Data is not float, int32, or int64")
-
-        # Create a new memoryview with a specific dtype
-        float_view = self._data.view(dtype)
-
-        # Assign the old data through the memoryview
-        float_view[:] = self._data
-
-        # Replace the old data with the newly converted data
-        self._data = float_view
+        self._data = convert_array_to_float(self._data)
 
     def trim_genes(self, remove_constant_genes=True, trim_gene_list=None):
         """
-        Remove genes (columns) that are unwanted from the data set. Do this in-place.
+        Remove genes (columns) that are unwanted from the data set.
+        Do this in-place.
 
         :param remove_constant_genes:
         :type remove_constant_genes: bool
         :param trim_gene_list: This is a list of genes to KEEP.
         :type trim_gene_list: list, pd.Series, pd.Index
         """
 
         keep_column_bool = np.ones((len(self._adata.var_names),), dtype=bool)
 
         if trim_gene_list is not None:
-            keep_column_bool &= self._adata.var_names.isin(trim_gene_list)
+            keep_column_bool &= self._adata.var_names.isin(
+                trim_gene_list
+            )
+
         if "trim_gene_list" in self._adata.uns:
-            keep_column_bool &= self._adata.var_names.isin(self._adata.uns["trim_gene_list"])
+            keep_column_bool &= self._adata.var_names.isin(
+                self._adata.uns["trim_gene_list"]
+            )
 
         list_trim = len(self._adata.var_names) - np.sum(keep_column_bool)
         comp = 0 if self._is_integer else np.finfo(self.values.dtype).eps * 10
 
         if remove_constant_genes:
             nz_var = self.values.max(axis=0) - self.values.min(axis=0)
             nz_var = nz_var.A.flatten() if self.is_sparse else nz_var
@@ -799,50 +498,39 @@
 
             # This explicit copy allows the original to be deallocated
             # Otherwise the view reference keeps it in memory
             # At some point it will need to copy so why not now
             self._adata = AnnData(
                 self._adata.X[:, keep_column_bool],
                 obs=self._adata.obs.copy(),
-                var=self._adata.var.loc[keep_column_bool, :].copy(),
-                dtype=self._adata.X.dtype
+                var=self._adata.var.loc[keep_column_bool, :].copy()
             )
 
-            # Make sure that there's no hanging reference to the original object
+            # Make sure that there's no hanging reference to the original
             gc.collect()
 
     def get_gene_data(
         self,
         gene_list,
         force_dense=False,
         to_df=False,
-        zscore=False,
         flatten=False
     ):
 
         x = self._adata[:, gene_list]
         labels = x.var_names
 
-        if (force_dense or to_df or zscore) and self.is_sparse:
+        if (force_dense or to_df) and self.is_sparse:
             x = x.X.A
 
         else:
             # Copy is necessary to get the numpy array
             # and not an anndata arrayview
             x = x.X.copy()
 
-        if zscore:
-
-            # Z-score the values
-            z_x = np.subtract(x, self.obs_means.reshape(-1, 1))
-            z_x = np.divide(z_x, self.obs_stdev.reshape(-1, 1))
-
-            # Replace the x reference with the new values
-            x = z_x
-
         if flatten:
             x = x.ravel()
 
         if to_df:
             return pd.DataFrame(
                 x,
                 columns=labels,
@@ -853,30 +541,26 @@
             return x
 
     def get_sample_data(
         self,
         sample_index,
         copy=False,
         force_dense=False,
-        to_df=False,
-        zscore=False
+        to_df=False
     ):
 
         x = self._adata[sample_index, :]
         labels = x.obs_names
 
-        if (force_dense or to_df or zscore) and self.is_sparse:
+        if (force_dense or to_df) and self.is_sparse:
             x = x.X.A
         else:
             x = x.X
 
-        if zscore:
-            x = np.subtract(x, self.obs_means[sample_index].reshape(-1, 1))
-            x = np.divide(x, self.obs_stdev[sample_index].reshape(-1, 1))
-        elif copy:
+        if copy:
             x = x.X.copy()
 
         if to_df:
             x = pd.DataFrame(
                 x,
                 columns=self.gene_names,
                 index=labels
@@ -884,14 +568,18 @@
 
         return x
 
     def get_bootstrap(
         self,
         sample_bootstrap_index
     ):
+
+        if sample_bootstrap_index is None:
+            return self.copy()
+
         return InferelatorData(
             expression_data=self._adata.X[sample_bootstrap_index, :].copy(),
             gene_names=self.gene_names
         )
 
     def get_random_samples(
         self,
@@ -944,30 +632,34 @@
         else:
             keeper_ilocs = random_gen.choice(
                 np.arange(self.num_obs),
                 size=(num_obs,),
                 replace=False
             )
 
+        # Subset AnnData object
+        _new_adata = self._adata[keeper_ilocs, :]
+
+        if _new_adata.is_view:
+            _new_adata = _new_adata.copy()
+
+        # Check names and make unique if set
+        if with_replacement and fix_names:
+            _new_adata.obs_names_make_unique()
+
         # Change this instance's _adata (explicit copy allows the old data to
         # be dereferenced instead of held as view)
         if inplace:
-            self._adata = self._adata[keeper_ilocs, :].copy()
+            self._adata = _new_adata
             return_obj = self
             gc.collect()
 
         # Create a new InferelatorData instance with the _adata slice
         else:
-            return_obj = InferelatorData(
-                self._adata[keeper_ilocs, :].copy()
-            )
-
-        # Fix names
-        if with_replacement and fix_names:
-            return_obj._adata.obs_names_make_unique()
+            return_obj = InferelatorData(_new_adata)
 
         return return_obj
 
     def subset_copy(self, row_index=None, column_index=None):
 
         if row_index is not None and column_index is not None:
             data_view = self._adata[row_index, column_index]
@@ -1008,29 +700,47 @@
                 cast=True,
                 dense=force_dense
             )
 
     def to_csv(self, file_name, sep="\t"):
 
         if self.is_sparse:
-            scipy.io.mmwrite(file_name, self.values)
+            io.mmwrite(file_name, self.values)
         else:
             self._adata.to_df().to_csv(file_name, sep=sep)
 
     def to_h5ad(self, file_name, compression="gzip"):
 
         self._adata.write(file_name, compression=compression)
 
     def transform(
         self,
         func,
         add_pseudocount=False,
         memory_efficient=True,
         chunksize=1000
     ):
+        """
+        Apply a function to each nonzero value of a sparse matrix
+        or each value of a dense matrix
+
+        :param func: Function which takes a scalar or array input
+        :type func: callable
+        :param add_pseudocount: Add a pseudocount before applying function,
+            defaults to False
+        :type add_pseudocount: bool, optional
+        :param memory_efficient: Apply function to chunks of the data and
+            overwrite values in the existing array. Only works if the dtype
+            returned from the function is the same as the dtype of the array.
+            Defaults to True.
+        :type memory_efficient: bool, optional
+        :param chunksize: Number of observations to use as a chunk,
+            defaults to 1000
+        :type chunksize: int, optional
+        """
 
         # Add 1 to every non-zero value
         if add_pseudocount and self.is_sparse:
             self._adata.X.data += 1
         elif add_pseudocount:
             self._adata.X += 1
 
@@ -1047,26 +757,47 @@
 
         # If memory_efficient is True and the data type returned by func is
         # the same as the data type of the data itself,
         # take row-wise chunks of data, transform it, and put it back into
         # the original data, overwriting the original
         elif memory_efficient and _type_match:
 
-            _n_chunks = math.ceil(self._adata.shape[0] / chunksize)
+            _n_chunks = int(np.ceil(self._adata.shape[0] / chunksize))
 
             for i in range(_n_chunks):
                 _start = i * chunksize
                 _stop = min(_start + chunksize, self._adata.shape[0])
                 self._data[_start:_stop, :] = func(self._data[_start:_stop, :])
 
         # Apply function to the data
         # by making a new data object
         else:
             self._data = func(self._data)
 
+    def apply(
+        self,
+        func,
+        **kwargs
+    ):
+        """
+        Apply a function that takes a 2d numpy array or sparse matrix to
+        the underlying data. Replaces the data in place.
+        Will pass any kwargs to the function.
+
+        :param func: Function which takes an array input
+        :type func: callable
+        """
+
+        self._adata.X = func(
+            self._adata.X,
+            **kwargs
+        )
+
+        return self
+
     def add(
         self,
         val,
         axis=None
     ):
         """
         Add a value to the matrix in-place
@@ -1230,39 +961,25 @@
 
         elif axis == 1:
             _mfunc(value[:, None])
 
         else:
             raise ValueError("axis must be 0, 1 or None")
 
-    def zscore(self, axis=0, ddof=1):
-
-        self.convert_to_float()
-        self.to_dense()
-
-        if axis == 0:
-            for i in range(self.shape[1]):
-                self._data[:, i] = scale_vector(self._data[:, i], ddof=ddof)
-        elif axis == 1:
-            for i in range(self.shape[0]):
-                self._data[i, :] = scale_vector(self._data[i, :], ddof=ddof)
-
-        return self
-
     def copy(self):
 
         new_data = InferelatorData(
             self.values.copy(),
             meta_data=self.meta_data.copy(),
             gene_data=self.gene_data.copy()
         )
 
         new_data._adata.var_names = self._adata.var_names.copy()
         new_data._adata.obs_names = self._adata.obs_names.copy()
-        new_data._adata.uns = cp.copy(self._adata.uns)
+        new_data._adata.uns = self._adata.uns.copy()
 
         return new_data
 
     def to_csc(self):
 
         if self.is_sparse and not sparse.isspmatrix_csc(self._adata.X):
             self._adata.X = sparse.csc_matrix(self._adata.X)
@@ -1285,32 +1002,40 @@
             self._adata.X = sparse.csc_matrix(self._adata.X)
         elif not self.is_sparse:
             raise ValueError("Mode must be csc or csr")
 
     def to_df(self):
         return self._adata.to_df()
 
-    def replace_data(self, new_data, new_gene_names=None, new_gene_metadata=None):
+    def replace_data(
+            self,
+            new_data,
+            new_gene_names=None,
+            new_gene_metadata=None
+    ):
 
         if new_gene_metadata is None and new_gene_names is not None:
             new_gene_metadata = pd.DataFrame(index=new_gene_names)
 
         self._adata = AnnData(
             X=new_data,
-            dtype=new_data.dtype,
             var=new_gene_metadata,
             obs=self._adata.obs
         )
 
         gc.collect()
 
     @staticmethod
     def _make_idx_str(df):
-        df.index = df.index.astype(str) if not pat.is_string_dtype(df.index.dtype) else df.index
-        df.columns = df.columns.astype(str) if not pat.is_string_dtype(df.columns.dtype) else df.columns
+
+        if not pat.is_string_dtype(df.index.dtype):
+            df.index = df.index.astype(str)
+
+        if not pat.is_string_dtype(df.columns.dtype):
+            df.columns = df.columns.astype(str)
 
     def _counts(self, axis=None):
         if self.is_sparse:
             return self._adata.X.sum(axis=axis).A.flatten()
         else:
             return self._adata.X.sum(axis=axis)
```

### Comparing `inferelator-0.6.1/inferelator/utils/debug.py` & `inferelator-0.6.2/inferelator/utils/debug.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,141 @@
-from __future__ import print_function, unicode_literals, division
 import os
+import logging
+import sys
 
-SBATCH_VARS = dict(output_dir=('RUNDIR', str, None),
-                   input_dir=('DATADIR', str, None))
+SBATCH_VARS = dict(
+    output_dir=('RUNDIR', str, None),
+    input_dir=('DATADIR', str, None)
+)
 
 
 class Debug:
     """
-    This class is for printing status messages to stdout
-    Just plain print doesn't work so well when there are multiple processes
+    Wrapper for logging
+    Exists for historic reasons
+    Probably wouldn't do it this way from scratch
+    But im not rewriting everything that depends on this
     """
     verbose_level = 0
     default_level = 1
 
-    levels = dict(silent=-1,
-                  normal=0,
-                  verbose=1, v=1,
-                  very_verbose=2, vv=2,
-                  max_output=3, vvv=3)
+    stderr = False
+    logger = None
+
+    levels = dict(
+        silent=-1,
+        normal=0,
+        verbose=1, v=1,
+        very_verbose=2, vv=2,
+        max_output=3, vvv=3
+    )
 
     @classmethod
-    def set_verbose_level(cls, lvl):
+    def set_verbose_level(
+        cls,
+        lvl
+    ):
         if isinstance(lvl, (int, float)):
             cls.verbose_level = lvl
         elif lvl in cls.levels.keys():
             cls.verbose_level = cls.levels[lvl]
 
     @classmethod
-    def vprint(cls, *args, **kwargs):
+    def vprint(
+        cls,
+        *args,
+        **kwargs
+    ):
         cls.print_level(*args, **kwargs)
 
     @classmethod
-    def allprint(cls, *args, **kwargs):
-        cls.print_level(*args, **kwargs)
+    def print_level(
+        cls,
+        *args,
+        **kwargs
+    ):
+        level = kwargs.pop('level', cls.default_level)
 
-    @classmethod
-    def print_level(cls, *args, **kwargs):
-        try:
-            level = kwargs.pop('level')
-        except KeyError:
-            level = cls.default_level
         if level <= cls.verbose_level:
-            print((" " * level), *args, **kwargs)
-        else:
+            cls.create_logger()
+
+            cls.logger.log(
+                level + 1,
+                *args,
+                **kwargs
+            )
+
+    @classmethod
+    def log_to_stderr(
+        cls,
+        stderr_flag
+    ):
+        cls.stderr = stderr_flag
+
+    @classmethod
+    def create_logger(cls):
+
+        if cls.logger is not None:
             return
 
+        cls.logger = logging.Logger('inferelator')
 
-def inferelator_verbose_level(level):
+        logger_handler = logging.StreamHandler(
+            sys.stderr if cls.stderr else sys.stdout
+        )
+
+        logger_handler.setFormatter(
+            logging.Formatter(
+                '%(asctime)-15s %(levelno)s %(message)s',
+                '%Y-%m-%d %H:%M:%S'
+            )
+        )
+
+        cls.logger.addHandler(logger_handler)
+
+
+def inferelator_verbose_level(
+    level,
+    log_to_stderr=None
+):
     """
     Set verbosity.
-    :param level: Verbose level. 0 is normal, 1 is extra information. 2+ is not recommended. -1 silences most outputs.
+    :param level: Verbose level.
+        0 is normal, 1 is extra information.
+        2+ is not recommended.
+        -1 silences most outputs.
     :type level: int
+    :param log_to_stderr: Log to stderr instead of stdout
+    :type log_to_stderr: bool
     """
+
     Debug.set_verbose_level(level)
 
+    if log_to_stderr is not None:
+        Debug.log_to_stderr(log_to_stderr)
+
 
-def slurm_envs(var_names=None):
+def slurm_envs(
+    var_names=None
+):
     """
     Get environment variable names and return them as a dict
-    :param var_names: list
-        A list of environment variable names to get. Will throw an error if they're not keys in the SBATCH_VARS dict
-    :return envs: dict
-        A dict keyed by setattr variable name of the value (or default) from the environment variables
+
+    :param var_names: A list of environment variable names to get.
+        Will throw an error if they're not keys in the SBATCH_VARS dict
+    :type var_names: list
+    :return envs: A dict keyed by setattr variable name of the value
+        (or default) from the environment variables
+    :rtype dict
     """
     var_names = SBATCH_VARS.keys() if var_names is None else var_names
     assert set(var_names).issubset(set(SBATCH_VARS.keys()))
 
     envs = {}
     for cv in var_names:
         os_var, mt, de = SBATCH_VARS[cv]
         try:
             val = mt(os.environ[os_var])
         except (KeyError, TypeError):
             val = de
         envs[cv] = val
-    return envs
+    return envs
```

### Comparing `inferelator-0.6.1/inferelator/utils/loader.py` & `inferelator-0.6.2/inferelator/utils/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import pandas as pd
 import pandas.api.types as pat
 import numpy as np
 import os
 import copy as cp
 import anndata
 import warnings
+from scipy import sparse
 
-from inferelator.utils.data import InferelatorData
-from inferelator.utils.debug import Debug
+from .inferelator_data import InferelatorData
+from .debug import Debug
 from inferelator.preprocessing.metadata_parser import MetadataHandler
 
 DEFAULT_PANDAS_TSV_SETTINGS = dict(sep="\t", index_col=0, header=0)
 DEFAULT_METADATA = "branching"
 
 _TENX_MTX = ("matrix.mtx.gz", "matrix.mtx")
 _TENX_BARCODES = ("barcodes.tsv.gz", "barcodes.tsv")
 _TENX_FEATURES = ("features.tsv.gz", "genes.tsv")
 
+_TENX_H5 = "filtered_feature_bc_matrix.h5"
+_TENX_H5_FEATURES_KEYS = [
+    'id',
+    'name',
+    'genome',
+    'interval',
+    'feature_type'
+]
+
 
 class InferelatorDataLoader(object):
     input_dir = None
     _file_format_settings = None
 
     def __init__(self, input_dir, file_format_settings=None):
         self.input_dir = input_dir
@@ -65,15 +75,16 @@
             layer doesn't exist
         :return: InferelatorData object
         :rtype: InferelatorData
         """
 
         # Read H5AD file
         Debug.vprint(
-            f"Loading AnnData file {h5ad_file}",
+            f"Loading AnnData file {h5ad_file} "
+            f"(Layer: {use_layer if use_layer is not None else 'X'})",
             level=0
         )
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", anndata.OldFormatWarning)
             data = anndata.read_h5ad(self.input_path(h5ad_file))
 
@@ -127,15 +138,15 @@
                 gene_data=pd.concat((data.var, gene_metadata), axis=1)
             )
 
         # Make sure bytestrings are decoded
         _safe_dataframe_decoder(data.gene_data)
         _safe_dataframe_decoder(data.meta_data)
 
-        self._check_loaded_data(data, filename=h5ad_file)
+        self._check_loaded_data(data)
 
         return data
 
     def load_data_mtx(
         self,
         mtx_file,
         mtx_obs=None,
@@ -265,14 +276,67 @@
                 mtx_feature=mtx_feature,
                 meta_data_file=meta_data_file,
                 meta_data_handler=meta_data_handler,
                 gene_data_file=gene_data_file,
                 gene_name_column=gene_name_column
             )
 
+    def load_data_tenx_h5(
+        self,
+        tenx_path,
+        filename=_TENX_H5
+    ):
+
+        import h5py
+
+        h5_file = h5py.File(
+            self.filename_path_join(tenx_path, filename)
+        )
+
+        _matrix = h5_file['matrix']
+        csc_matrix = sparse.csc_matrix(
+            ((
+                _matrix['data'][:],
+                _matrix['indices'][:],
+                _matrix['indptr'][:]
+            )),
+            shape=_matrix['shape'][:]
+        )
+
+        _barcodes = _matrix['barcodes'][:].astype(str)
+        _features = _matrix['features']
+
+        features_dataframe = pd.DataFrame({
+            tag: _features[tag][:].astype(str)
+            for tag in _TENX_H5_FEATURES_KEYS
+        })
+        features_dataframe = features_dataframe.set_index(
+            'name',
+            drop=True
+        )
+
+        # Extract interval data and embed it into new columns
+        _interval = features_dataframe['interval'].str.extract(
+            "([^:]*):([^-]*)-([^-]*)"
+        )
+        features_dataframe[['chrom', 'start', 'end']] = _interval
+
+        # Enforce integer data types
+        for c in ['start', 'end']:
+            features_dataframe[c] = features_dataframe[c].astype(float)
+            features_dataframe.loc[pd.isna(features_dataframe[c]), c] = 0.
+            features_dataframe[c] = features_dataframe[c].astype(int)
+
+        return InferelatorData(
+            csc_matrix.T,
+            gene_data=features_dataframe,
+            gene_names=features_dataframe.index,
+            sample_names=_barcodes
+        )
+
     def load_data_tsv(
         self,
         tsv_matrix_file,
         transpose_data=False,
         meta_data_file=None,
         meta_data_handler=DEFAULT_METADATA,
         tsv_matrix_metadata=None,
@@ -318,15 +382,15 @@
         data = InferelatorData(
             data,
             transpose_expression=transpose_data,
             meta_data=pd.concat((meta_data, slice_meta_data), axis=1),
             gene_data=gene_metadata
         )
 
-        self._check_loaded_data(data, filename=tsv_matrix_file)
+        self._check_loaded_data(data)
 
         return data
 
     def load_metadata_tsv(
         self,
         meta_data_file,
         sample_labels,
@@ -379,15 +443,16 @@
     ):
 
         # Load gene metadata
         if gene_data_file is None and gene_name_column is None:
             return None
         elif gene_data_file is None or gene_name_column is None:
             raise ValueError(
-                "Gene_metadata_file and gene_name_column must both be set if either is"
+                "Gene_metadata_file and gene_name_column must both be set "
+                "if either is set"
             )
 
         Debug.vprint(
             f"Loading gene metadata from file {gene_data_file}",
             level=0
         )
 
@@ -468,30 +533,30 @@
         return pd.read_csv(
             filename,
             sep="\t",
             header=None
         )[0].tolist()
 
     @staticmethod
-    def _check_loaded_data(data, filename=None):
-        msg = f"Loaded {filename if filename is not None else ''}:\n"
+    def _check_loaded_data(data):
+        msg = ""
 
         nnf, non_finite_genes = data.non_finite
 
         if nnf > 0:
             msg += f"\t{nnf} genes with non-finite expression "
-            msg += f"({' '.join(non_finite_genes)})\n"
+            msg += f"({' '.join(non_finite_genes)})"
 
         if not data.gene_names.is_unique:
             _repeated = data.gene_names[data.gene_names.duplicated()]
 
             msg += f"\t{len(_repeated)} genes are duplicated "
-            msg += f"({' '.join(_repeated)})\n"
+            msg += f"({' '.join(_repeated)})"
 
-        msg += "Data loaded: {dt}".format(dt=str(data))
+        msg += f"Data loaded: {str(data)}"
 
         Debug.vprint(msg, level=0)
 
     @staticmethod
     def filename_path_join(path, filename):
         """
         Join filename to path
```

### Comparing `inferelator-0.6.1/inferelator/utils/profiler.py` & `inferelator-0.6.2/inferelator/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/utils/validator.py` & `inferelator-0.6.2/inferelator/utils/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,60 @@
-from __future__ import print_function, unicode_literals, division
-
 import pandas as pd
 import pandas.api.types as pat
 import os
 import inspect
 
-# Python 2/3 compatible string checking
-try:
-    basestring
-except NameError:
-    basestring = str
-
 
-class Validator(object):
+class Validator:
     """
-    Validation module for function arguments. Each function here should return True or it should raise an exception
+    Validation module for function arguments. Each function here should return
+    True or it should raise an exception
     """
 
     @staticmethod
-    def argument_numeric(arg, low=None, high=None, allow_none=False, types=(int, float)):
+    def argument_numeric(
+        arg,
+        low=None,
+        high=None,
+        allow_none=False,
+        types=(int, float)
+    ):
         """
-        Validate an input argument as being numeric (either an int or a float). Also check bounds if set.
+        Validate an input argument as being numeric (either an int or a float).
+        Also check bounds if set.
+
         :param arg:
             Argument to validate
         :param low: numeric
-            Lowest (inclusive) acceptable value of the argument; ignore this if it's None
+            Lowest (inclusive) acceptable value of the argument;
+            ignore this if it's None
         :param high: numeric
-            Lowest (inclusive) acceptable value of the argument; ignore this if it's None
+            Lowest (inclusive) acceptable value of the argument;
+            ignore this if it's None
         :param allow_none: bool
             Allow arg to be None if true
         :return:
             Returns True if valid. Raises an exception otherwise
         """
         if allow_none and arg is None:
             return True
 
         if not isinstance(arg, types):
-            raise ValueError("Argument must be numeric ({arg}, {typ} provided) ".format(arg=arg, typ=type(arg)))
-
-        if low is not None and Validator.argument_numeric(low) and arg < low:
-            raise ValueError("Argument must be at least {low}".format(low=low))
-        if high is not None and Validator.argument_numeric(high) and arg > high:
-            raise ValueError("Argument must be no more than {high}".format(high=high))
+            raise ValueError(
+                f"Argument must be numeric ({arg}, {type(arg)} provided)"
+            )
+
+        if low is not None and arg < low:
+            raise ValueError(
+                f"Argument must be at least {low}, {arg} provided"
+            )
+        if high is not None and arg > high:
+            raise ValueError(
+                f"Argument must be no more than {high}, {arg} provided"
+            )
 
         return True
 
     @staticmethod
     def argument_integer(arg, low=None, high=None, allow_none=False):
         """
         Wrapper for argument_numeric which forces only integers
@@ -141,26 +150,34 @@
             return True
         elif arg.startswith(is_subpath_of + os.sep):
             return True
         else:
             raise ValueError("Path {a} is not a subpath of path {b}".format(a=arg, b=is_subpath_of))
 
     @staticmethod
-    def argument_type(arg, arg_type, allow_none=False):
+    def argument_type(
+        arg,
+        arg_type,
+        allow_none=False
+    ):
+
         if allow_none and arg is None:
             return True
 
         if isinstance(arg, arg_type):
             return True
         else:
-            raise ValueError("Argument {arg} must be of type {typ}".format(arg=arg, typ=arg_type))
+            raise ValueError(
+                f"Argument {arg} must be of type {arg_type} "
+                f"({type(arg)} provided)"
+            )
 
     @staticmethod
     def argument_string(arg, allow_none=False):
-        return Validator.argument_type(arg, basestring, allow_none=allow_none)
+        return Validator.argument_type(arg, str, allow_none=allow_none)
 
     @staticmethod
     def argument_list_type(arg, arg_type, allow_none=False):
         if allow_none and arg is None:
             return True
         for a in arg:
             Validator.argument_type(a, arg_type, allow_none=allow_none)
@@ -335,8 +352,8 @@
 
 def is_string(arg):
     """
     Check if a argument is a string in a python 2/3 compatible way
     :param arg:
     :return:
     """
-    return isinstance(arg, basestring)
+    return isinstance(arg, str)
```

### Comparing `inferelator-0.6.1/inferelator/workflow.py` & `inferelator-0.6.2/inferelator/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,8 +245,11 @@
     :return: This returns an initialized object which has both the
         regression workflow and the preprocessing/postprocessing workflow.
         This object can then have settings assigned to it, and can be run
         with `.run()`
     :rtype: Workflow instance
     """
 
-    return _factory_build_inferelator(regression=regression, workflow=workflow)()
+    return _factory_build_inferelator(
+        regression=regression,
+        workflow=workflow
+    )()
```

### Comparing `inferelator-0.6.1/inferelator/workflows/amusr_workflow.py` & `inferelator-0.6.2/inferelator/workflows/amusr_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Run Multitask Network Inference with TFA-AMuSR.
 """
 import copy
 import gc
 import warnings
 import pandas as pd
-import functools
 
-from inferelator.utils import Debug
+from inferelator.utils import (
+    Debug,
+    join_pandas_index
+)
 from inferelator import workflow
 from inferelator.workflows import single_cell_workflow
 from inferelator.regression import amusr_regression
 from inferelator.postprocessing.results_processor_mtl import (
     ResultsProcessorMultiTask
 )
 
@@ -32,14 +34,15 @@
     "expression_matrix_file",
     "tf_names_file",
     "meta_data_file",
     "priors_file",
     "gold_standard_file"
 ]
 
+
 class MultitaskLearningWorkflow(single_cell_workflow.SingleCellWorkflow):
     """
     Class that implements multitask learning. Handles loading and
     validation of multiple data packages
     """
 
     _regulator_expression_filter = "intersection"
@@ -128,21 +131,18 @@
                 for t in self._task_objects if t.tf_names is not None
             ]
 
         else:
             return None
 
         # Intersect each task's tf indices
-        if len(task_ref) > 0:
-            return functools.reduce(
-                lambda x, y: x.intersection(y),
-                task_ref
-            )
-        else:
-            return None
+        return join_pandas_index(
+            *task_ref,
+            method='intersection'
+        )
 
     @property
     def _gene_names(self):
 
         # Use column names from response data objects which have gene columns
         if self._task_response is not None:
             task_ref = [
@@ -157,21 +157,18 @@
                 for t in self._task_objects if t.data is not None
             ]
 
         else:
             return None
 
         # Intersect each task's gene indices
-        if len(task_ref) > 0:
-            return functools.reduce(
-                lambda x, y: x.intersection(y),
-                task_ref
-            )
-        else:
-            return None
+        return join_pandas_index(
+            *task_ref,
+            method='intersection'
+        )
 
     def set_task_filters(
         self,
         regulator_expression_filter=None,
         target_expression_filter=None
     ):
         """
@@ -210,27 +207,30 @@
         # Set the random seed in the task to the same as the parent
         for tobj in self._task_objects:
             tobj.random_seed = self.random_seed
 
         self.validate_data()
 
     def get_data(self):
-        # Task data has expression & metadata and may have task-specific files for anything else
+        # Task data has expression & metadata and may have task-specific
+        # files for anything else
         self._load_tasks()
 
-        # Priors, gold standard, tf_names, and gene metadata will be loaded if set
+        # Priors, gold standard, tf_names, and gene metadata
+        # will be loaded if set
         self.read_tfs()
         self.read_priors()
         self.read_genes()
 
     def startup_finish(self):
         """
         Process task data and priors.
 
-        This is called when `.startup()` is run. It is not necessary to call separately.
+        This is called when `.startup()` is run.
+        It is not necessary to call separately.
         """
 
         # Make sure tasks are set correctly
         self._process_default_priors()
         self._process_task_priors()
         self._process_task_data()
 
@@ -245,69 +245,84 @@
         gold_standard_file=None,
         gene_names_file=None,
         gene_metadata_file=None,
         workflow_type="single-cell",
         **kwargs
     ):
         """
-        Create a task object and set any arguments to this function as attributes of that task object. TaskData objects
+        Create a task object and set any arguments to this function as
+        attributes of that task object. TaskData objects
         are stored internally in _task_objects.
 
         :param task_name: A descriptive name for this task
         :type task_name: str
         :param input_dir: A path containing the input files
         :type input_dir: str
         :param expression_matrix_file: Path to the expression data
         :type expression_matrix_file: str
         :param meta_data_file: Path to the meta data
         :type meta_data_file: str, optional
-        :param tf_names_file: Path to a list of regulator names to include in the model
+        :param tf_names_file: Path to a list of regulator names to include
+            in the model
         :type tf_names_file: str
         :param priors_file: Path to a prior data file
         :type priors_file: str
         :param gene_metadata_file: Path to a genes annotation file
         :type gene_metadata_file: str, optional
-        :param gene_names_file: Path to a list of genes to include in the model (optional)
+        :param gene_names_file: Path to a list of genes to include in
+            the model (optional)
         :type gene_names_file: str, optional
         :param workflow_type: The type of workflow for data preprocessing.
             "tfa" uses the TFA workflow,
             "single-cell" uses the Single-Cell TFA workflow
         :type workflow_type: str, `inferelator.BaseWorkflow` subclass
-        :param kwargs: Any additional arguments are assigned to the task object.
-        :return: Returns a task reference which can be additionally modified by calling any valid Workflow function to
-            set task parameters
+        :param kwargs: Any additional arguments are assigned to thetask object
+        :return: Returns a task reference which can be additionally modified
+            by calling any valid Workflow function to set task parameters
         :rtype: TaskData instance
         """
 
-        # Create a TaskData object from a workflow and set the formal arguments into it
+        # Create a TaskData object from a workflow and set the
+        # formal arguments into it
         task_object = create_task_data_object(workflow_class=workflow_type)
         task_object.task_name = task_name
-        task_object.input_dir = input_dir if input_dir is not None else self.input_dir
+
+        if input_dir is not None:
+            task_object.input_dir = input_dir
+        else:
+            task_object.input_dir = self.input_dir
+
         task_object.expression_matrix_file = expression_matrix_file
         task_object.meta_data_file = meta_data_file
         task_object.tf_names_file = tf_names_file
         task_object.priors_file = priors_file
         task_object.gene_names_file = gene_names_file
         task_object.gene_metadata_file = gene_metadata_file
         task_object.gold_standard_file = gold_standard_file
 
         # Warn if there is an attempt to set something that isn't supported
-        msg = "Task-specific {} is not supported. This setting will be ignored. Set this in the parent workflow."
         for bad in NON_TASK_ATTRIBUTES:
             if bad in kwargs:
                 del kwargs[bad]
-                warnings.warn(msg.format(bad))
+                warnings.warn(
+                    f"Task-specific {bad} is not supported. "
+                    "This setting will be ignored. "
+                    "Set this in the parent workflow."
+                )
 
-        # Pass forward any kwargs (raising errors if they're for attributes that don't exist)
+        # Pass forward any kwargs (raising errors if they're for
+        # attributes that don't exist)
         for attr, val in kwargs.items():
             if hasattr(task_object, attr):
                 setattr(task_object, attr, val)
                 task_object.str_attrs.append(attr)
             else:
-                raise ValueError(f"Argument {attr} cannot be set as an attribute")
+                raise ValueError(
+                    f"Argument {attr} cannot be set as an attribute"
+                )
 
         if self._task_objects is None:
             self._task_objects = [task_object]
         else:
             self._task_objects.append(task_object)
 
         Debug.vprint(str(task_object), level=0)
@@ -318,31 +333,35 @@
         """
         Run load_task_data in all the TaskData objects created with create_task
         """
         if self._task_objects is None:
             raise ValueError("Tasks have not been created with .create_task()")
 
         for tobj in self._task_objects:
-            # Transfer attributes from parent if they haven't been set in the task
+            # Transfer attributes from parent if they haven't been
+            # set in the task
             for attr in TRANSFER_ATTRIBUTES:
                 try:
-                    if getattr(self, attr) is not None and getattr(tobj, attr) is None:
+                    if getattr(tobj, attr) is None:
                         setattr(tobj, attr, getattr(self, attr))
                 except AttributeError:
                     pass
 
             # Set the num_bootstraps in the task to the same as the parent
             tobj.num_bootstraps = self.num_bootstraps
 
         # Run load_task_data and create a list of lists of TaskData objects
         # This allows a TaskData object to copy and split itself if needed
         self._task_objects = [tobj.get_data() for tobj in self._task_objects]
 
         # Flatten the list
-        self._task_objects = [tobj for tobj_list in self._task_objects for tobj in tobj_list]
+        self._task_objects = [
+            t for t_list in self._task_objects
+            for t in t_list
+        ]
         self._n_tasks = len(self._task_objects)
 
     def validate_data(self):
         """
         Make sure that the data that's loaded is acceptable
 
         This is called when `.startup()` is run. It is not necessary
@@ -379,40 +398,44 @@
                 "(no default prior is set). "
                 "worker.set_network_data_flags(use_no_prior=True) "
                 "will override this error."
             )
 
     def _process_default_priors(self):
         """
-        Process the default priors in the parent workflow for crossvalidation or shuffling
+        Process the default priors in the parent workflow for
+        crossvalidation or shuffling
         """
 
         # Use priors if given to the MTL workflow
         if self.priors_data is not None:
             priors = self.priors_data
 
-        # If they all have priors don't worry about it - use a 0 prior here for crossvalidation selection if needed
+        # If they all have priors don't worry about it -
+        # use a 0 prior here for crossvalidation selection if needed
         elif self.priors_data is None and self.gold_standard is not None:
             priors = pd.DataFrame(
                 0,
                 index=self.gold_standard.index,
                 columns=self.gold_standard.columns
             )
 
         elif self.priors_data is None and self.tf_names is not None:
             priors = pd.DataFrame(
                 0,
                 index=self._gene_names,
                 columns=self.tf_names
             )
 
-        # If there's no gold standard or use_no_prior isn't set, raise a RuntimeError
+        # If there's no gold standard or use_no_prior isn't set,
+        # raise a RuntimeError
         else:
-            _msg = "No base prior or gold standard or TF list has been provided."
-            raise RuntimeError(_msg)
+            raise RuntimeError(
+                "No base prior or gold standard or TF list has been provided."
+            )
 
         # Crossvalidation
         if self.split_gold_standard_for_crossvalidation:
             priors, self.gold_standard = self.prior_manager.cross_validate_gold_standard(
                 priors,
                 self.gold_standard,
                 self.cv_split_axis,
@@ -438,16 +461,18 @@
         if self.shuffle_prior_axis is not None:
             priors = self.prior_manager.shuffle_priors(
                 priors,
                 self.shuffle_prior_axis,
                 self.random_seed
             )
 
-        # Add prior noise now (to the base prior) if add_prior_noise_to_task_priors is False
-        # Otherwise add later to the task priors (will be different for each task)
+        # Add prior noise now (to the base prior)
+        # if add_prior_noise_to_task_priors is False
+        # Otherwise add later to the task priors
+        # (will be different for each task)
         if self.add_prior_noise is not None and not self.add_prior_noise_to_task_priors:
             priors = self.prior_manager.add_prior_noise(
                 priors,
                 self.add_prior_noise,
                 self.random_seed
             )
 
@@ -474,68 +499,84 @@
         """
         Process & align the default priors for crossvalidation or shuffling
         """
         for task_obj in self._task_objects:
 
             # Set priors if task-specific priors are not present
             if task_obj.priors_data is None and self.priors_data is None:
-                raise ValueError("No priors exist in the main workflow or in tasks")
+                raise ValueError(
+                    "No priors exist in the main workflow or in tasks"
+                )
 
             elif task_obj.priors_data is None:
                 task_obj.priors_data = self.priors_data.copy()
 
             # Set gene names if task-specific gene names is not present
             if task_obj.gene_names is None:
                 task_obj.gene_names = copy.deepcopy(self.gene_names)
 
             # Set tf_names if task-specific tf names are not present
             if task_obj.tf_names is None:
                 task_obj.tf_names = copy.deepcopy(self.tf_names)
 
-            _add_prior_noise = self.add_prior_noise if self.add_prior_noise_to_task_priors is True else None
+            if self.add_prior_noise_to_task_priors is True:
+                _add_prior_noise = self.add_prior_noise
+            else:
+                _add_prior_noise = None
             # Process priors in the task data
+
             task_obj.process_priors_and_gold_standard(
                 gold_standard=self.gold_standard,
                 cv_flag=self.split_gold_standard_for_crossvalidation,
                 cv_axis=self.cv_split_axis,
                 shuffle_priors=self.shuffle_prior_axis,
                 add_prior_noise=_add_prior_noise
             )
 
     def _process_task_data(self):
         """
-        Preprocess the individual task data using the TaskData worker into task design and response data. Set
-        self.task_design, self.task_response, self.task_bootstraps with lists which contain
+        Preprocess the individual task data using the TaskData worker
+        into task design and response data. Set self.task_design,
+        self.task_response, self.task_bootstraps with lists which contain
         DataFrames.
 
-        Also set self.regulators and self.targets with pd.Indexes that correspond to the genes and tfs to model
-        This is chosen based on the filtering strategy set in self.target_expression_filter and
-        self.regulator_expression_filter
+        Also set self.regulators and self.targets with pd.Indexes that
+        correspond to the genes and tfs to model.
+
+        This is chosen based on the filtering strategy set in
+        self.target_expression_filter and self.regulator_expression_filter
         """
 
         # Create empty task data lists
         for attr in [
             "_task_design",
             "_task_response",
             "_task_bootstraps",
             "_task_names",
             "_task_priors",
-            "_task_gold_standards"]:
-
+            "_task_gold_standards"
+        ]:
             setattr(self, attr, [])
 
         targets, regulators = [], []
 
         # Iterate through a list of TaskData objects holding data
         for task_id, task_obj in enumerate(self._task_objects):
             # Get task name from Task
-            task_name = task_obj.task_name if task_obj.task_name is not None else str(task_id)
 
-            task_str = "Processing task #{tid} [{t}] {sh}"
-            Debug.vprint(task_str.format(tid=task_id, t=task_name, sh=task_obj.data.shape), level=1)
+            if task_obj.task_name is not None:
+                task_name = task_obj.task_name
+            else:
+                task_name = str(task_id)
+
+            Debug.vprint(
+                f"Processing task #{task_id} [{task_name}] "
+                f"{task_obj.data.shape}",
+                level=1
+            )
 
             # Run the preprocessing workflow
             task_obj.startup_finish()
 
             # Put the processed data into lists
             self._task_design.append(task_obj.design)
             self._task_response.append(task_obj.response)
@@ -568,37 +609,55 @@
         )
 
         self._task_genes = amusr_regression.genes_tasks(
             self._targets,
             self._task_response
         )
 
-        Debug.vprint("Processed data into design/response [{g} x {k}]".format(g=len(self._targets),
-                                                                              k=len(self._regulators)), level=0)
+        Debug.vprint(
+            "Processed data into design/response "
+            f"[{len(self._targets)} x {len(self._regulators)}]",
+            level=0
+        )
 
         # Clean up the TaskData objects and force a cyclic collection
         del self._task_objects
         gc.collect()
 
         self._align_design_response()
 
     def _align_design_response(self):
 
         # Make sure that the task data files have the correct columns
         for d in self._task_design:
-            d.trim_genes(remove_constant_genes=False, trim_gene_list=self._regulators)
+            d.trim_genes(
+                remove_constant_genes=False,
+                trim_gene_list=self._regulators
+            )
 
         for r in self._task_response:
-            r.trim_genes(remove_constant_genes=False, trim_gene_list=self._targets)
+            r.trim_genes(
+                remove_constant_genes=False,
+                trim_gene_list=self._targets
+            )
 
-    def emit_results(self, betas, rescaled_betas, gold_standard, priors_data):
+    def emit_results(
+        self,
+        betas,
+        rescaled_betas,
+        gold_standard,
+        priors_data,
+        full_model=None,
+        full_exp_var=None
+    ):
         """
         Output result report(s) for workflow run.
 
-        This is called when `.startup()` is run. It is not necessary to call separately.
+        This is called when `.startup()` is run.
+        It is not necessary to call separately.
         """
 
         self.create_output_dir()
 
         rp = self._result_processor_driver(
             betas,
             rescaled_betas,
@@ -607,35 +666,48 @@
             task_names=self._task_names
         )
 
         self.results = rp.summarize_network(
             self.output_dir,
             gold_standard,
             self._task_priors,
-            task_gold_standards=self._task_gold_standards
+            task_gold_standards=self._task_gold_standards,
+            full_model_betas=full_model,
+            full_model_var_exp=full_exp_var
         )
 
         self.task_results = rp.tasks_networks
 
         return self.results
 
 
 def create_task_data_object(workflow_class="single-cell"):
     return create_task_data_class(workflow_class=workflow_class)()
 
 
 def create_task_data_class(workflow_class="single-cell"):
+    """
+    Factory function for building task-specific workflows
+
+    :param workflow_class: Task workflow class to build,
+        defaults to "single-cell"
+    :type workflow_class: str, optional
+    :return: TaskData class built from the parent class
+    :rtype: TaskData
+    """
+
     task_parent = workflow._factory_build_inferelator(
         regression="base",
         workflow=workflow_class
     )
 
     class TaskData(task_parent):
         """
-        TaskData is a workflow object which only loads and preprocesses data from files.
+        TaskData is a workflow object which only loads and preprocesses
+        data from files.
         """
 
         task_name = None
         tasks_from_metadata = False
         meta_data_task_column = None
 
         task_workflow_class = str(workflow_class)
@@ -646,15 +718,16 @@
             """
             Create a printable report of the settings in this TaskData object
 
             :return: Settings in str_attrs in a printable string
             :rtype: str
             """
 
-            task_str = f"{self.task_name}:\n\tWorkflow Class: {self.task_workflow_class}\n"
+            task_str = f"{self.task_name}:"
+            task_str += f"\n\tWorkflow Class: {self.task_workflow_class}\n"
             for attr in self.str_attrs:
                 task_str += f"\t{attr}: {getattr(self, attr, 'NA')}\n"
 
             return task_str
 
         def __init__(self):
             if self._file_format_settings is None:
@@ -670,17 +743,22 @@
             raise NotImplementedError
 
         def startup_run(self):
             raise NotImplementedError
 
         def get_data(self):
             """
-            Load all the data and then return a list of references to TaskData objects
-            There will be multiple objects returned if tasks_from_metadata is set.
-            If tasks_from_metadata is not set, the list contains only this task (self)
+            Load all the data and then return a list of references
+            to TaskData objects
+
+            There will be multiple objects returned if
+            tasks_from_metadata is set.
+
+            If tasks_from_metadata is not set, the list contains
+            only this task (self)
 
             :return: List of TaskData objects with loaded data
             :rtype: list(TaskData)
             """
             Debug.vprint(f"Loading data for task {self.task_name}")
             super(TaskData, self).get_data()
 
@@ -699,28 +777,32 @@
             pass
 
         def set_run_parameters(self):
             """
             Set parameters used during runtime
             """
 
-            warnings.warn("Task-specific `num_bootstraps` and `random_seed` is not supported. Set on parent workflow.")
+            warnings.warn(
+                "Task-specific `num_bootstraps` and `random_seed` are not "
+                "supported; set on parent workflow."
+            )
 
         def process_priors_and_gold_standard(
             self,
             gold_standard=None,
             cv_flag=None,
             cv_axis=None,
             shuffle_priors=None,
             add_prior_noise=None
         ):
             """
             Make sure that the priors for this task are correct
 
-            This will remove circularity from the task priors based on the parent gold standard
+            This will remove circularity from the task priors based
+            on the parent gold standard
             """
 
             gold_standard = self.gold_standard if gold_standard is None else gold_standard
             cv_flag = self.split_gold_standard_for_crossvalidation if cv_flag is None else cv_flag
             cv_axis = self.cv_split_axis if cv_axis is None else cv_axis
             shuffle_priors = self.shuffle_prior_axis if shuffle_priors is None else shuffle_priors
             add_prior_noise = self.add_prior_noise if add_prior_noise is None else add_prior_noise
@@ -817,15 +899,14 @@
 
                 # Set task name
                 task_obj.data.name = task
                 task_obj.task_name = task
 
                 return task_obj
 
-
             new_task_objects = [_make_task_subobject(t) for t in tasks]
 
             Debug.vprint(
                 f"Separated data into {len(new_task_objects)} tasks",
                 level=0
             )
```

### Comparing `inferelator-0.6.1/inferelator/workflows/homology_workflow.py` & `inferelator-0.6.2/inferelator/workflows/homology_workflow.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/workflows/single_cell_workflow.py` & `inferelator-0.6.2/inferelator/workflows/single_cell_workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 """
-Run Single Cell Network Inference. This is the same network inference with some extra preprocessing functionality.
+Run Single Cell Network Inference. This is the same TFA network inference
+with some extra preprocessing functionality.
 """
 
-import numpy as np
-
-from inferelator.utils import Validator as check
 from inferelator.workflows import tfa_workflow
 from inferelator.preprocessing import single_cell
 from inferelator import utils
 
-PREPROCESSING_FUNCTIONS = {"log2": single_cell.log2_data,
-                           "ln": single_cell.ln_data,
-                           "log10": single_cell.log10_data,
-                           "ftt": single_cell.tf_sqrt_data}
+PREPROCESSING_FUNCS = {
+    "log2": single_cell.log2_data,
+    "ln": single_cell.ln_data,
+    "log10": single_cell.log10_data,
+    "ftt": single_cell.tf_sqrt_data
+}
 
 
 class SingleCellWorkflow(tfa_workflow.TFAWorkFlow):
     """
-    SingleCellWorkflow has some additional preprocessing prior to calculating TFA and running regression
+    SingleCellWorkflow has some additional preprocessing
+    prior to calculating TFA and running regression
     """
     # Single-cell expression data manipulations
     count_minimum = None  # float
 
     # Preprocessing workflow holder
     preprocessing_workflow = None
 
     # Do not use a design-response driver
     drd_driver = None
 
-    def set_count_minimum(self, count_minimum=None):
-        """
-        Set the minimum count value for each gene (averaged over all samples)
-
-        :param count_minimum: The mean expression value which is required to retain a gene for modeling. Data that
-            has already been normalized should probably be filtered during normalization, not now.
-            Defaults to None (disabled).
+    def set_count_minimum(
+        self,
+        count_minimum=None
+    ):
+        """
+        Set the minimum count value for each gene
+        (averaged over all samples)
+
+        :param count_minimum: The mean expression value which is required
+            to retain a gene for modeling. Data that has already been
+            normalized should probably be filtered during normalization,
+            not now. Defaults to None (disabled).
         :type count_minimum: float
         """
 
         self.count_minimum = count_minimum
 
     def add_preprocess_step(self, fun, **kwargs):
         """
-        Add a preprocessing step after count filtering but before calculating TFA or regression.
+        Add a preprocessing step after count filtering but before
+        calculating TFA or regression.
 
-        :param fun: Preprocessing function. Can be provided as a string or as a function in `preprocessing.single_cell`.
+        :param fun: Preprocessing function. Can be provided as a string
+        or as a function in `preprocessing.single_cell`.
 
             "log10" will take the log10 of pseudocounts
 
             "ln" will take the natural log of pseudocounts
 
             "log2" will take the log2 of pseudocounts
 
@@ -56,39 +64,61 @@
 
         :type fun: str, `preprocessing.single_cell` function
         :param kwargs: Additional arguments to the preprocessing function
         """
         if self.preprocessing_workflow is None:
             self.preprocessing_workflow = []
 
-        if utils.is_string(fun) and fun.lower() in PREPROCESSING_FUNCTIONS:
-            self.preprocessing_workflow.append((PREPROCESSING_FUNCTIONS[fun], kwargs))
-        elif utils.is_string(fun) and fun.lower() not in PREPROCESSING_FUNCTIONS:
-            raise ValueError("Unable to translate {f} into a function to call".format(f=fun))
+        if utils.is_string(fun) and fun.lower() in PREPROCESSING_FUNCS:
+            self.preprocessing_workflow.append(
+                (PREPROCESSING_FUNCS[fun], kwargs)
+            )
+
+        elif utils.is_string(fun) and fun.lower() not in PREPROCESSING_FUNCS:
+            raise ValueError(
+                f"Unable to translate {fun} into a function to call"
+            )
         else:
-            self.preprocessing_workflow.append((fun, kwargs))
+            self.preprocessing_workflow.append(
+                (fun, kwargs)
+            )
 
     def startup_finish(self):
-        # Preprocess the single-cell data based on the preprocessing steps added to the workflow
+        # Preprocess the single-cell data based on the preprocessing
+        # steps added to the workflow
         self.data_white_noise()
         self.single_cell_normalize()
 
         super(SingleCellWorkflow, self).startup_finish()
 
     def single_cell_normalize(self):
         """
-        Single cell normalization. Requires expression_matrix to be all numeric, and to be [N x G].
-        Executes all preprocessing workflow steps from the preprocessing_workflow list that's set by the
+        Single cell normalization. Requires expression_matrix to be
+        all numeric, and to be [N x G].
+
+        Executes all preprocessing workflow steps from the
+        preprocessing_workflow list that's set by the
         add_preprocess_step() class function
         """
 
-        single_cell.filter_genes_for_count(self.data, count_minimum=self.count_minimum)
+        single_cell.filter_genes_for_count(
+            self.data,
+            count_minimum=self.count_minimum
+        )
 
         if self.preprocessing_workflow is not None:
             for sc_func, sc_kwargs in self.preprocessing_workflow:
                 sc_kwargs['random_seed'] = self.random_seed
                 sc_func(self.data, **sc_kwargs)
 
         num_nonfinite, name_nonfinite = self.data.non_finite
+
         if num_nonfinite > 0:
-            utils.Debug.vprint("These genes have non-finite values: " + " ".join(name_nonfinite), level=0)
-            raise ValueError("NaN values have been introduced into the expression matrix by normalization")
+            utils.Debug.vprint(
+                "These genes have non-finite values: "
+                " ".join(name_nonfinite),
+                level=0
+            )
+            raise ValueError(
+                "NaN values have been introduced into the "
+                "expression matrix by normalization"
+            )
```

### Comparing `inferelator-0.6.1/inferelator/workflows/tfa_workflow.py` & `inferelator-0.6.2/inferelator/workflows/tfa_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,22 +160,24 @@
         # Set the random seed (for bootstrap selection)
         np.random.seed(self.random_seed)
 
         # Call the startup workflow
         self.startup()
 
         # Run regression after startup
-        betas, rescaled_betas = self.run_regression()
+        betas, rescaled_betas, full_betas, full_rescale = self.run_regression()
 
         # Write the results out to a file
         return self.emit_results(
             betas,
             rescaled_betas,
             self.gold_standard,
-            self.priors_data
+            self.priors_data,
+            full_model=full_betas,
+            full_exp_var=full_rescale
         )
 
     def startup_run(self):
         self.get_data()
         self.process_priors_and_gold_standard()
 
     def startup_finish(self):
@@ -270,15 +272,23 @@
             level=1
         )
 
         assert check.indexes_align(
             [self.design.sample_names, self.response.sample_names]
         )
 
-    def emit_results(self, betas, rescaled_betas, gold_standard, priors):
+    def emit_results(
+        self,
+        betas,
+        rescaled_betas,
+        gold_standard,
+        priors,
+        full_model=None,
+        full_exp_var=None
+    ):
         """
         Output result report(s) for workflow run.
         """
 
         self.create_output_dir()
 
         rp = self._result_processor_driver(
@@ -286,15 +296,18 @@
             rescaled_betas,
             filter_method=self.gold_standard_filter_method,
             metric=self.metric
         )
 
         self.results = rp.summarize_network(
             self.output_dir,
-            gold_standard, priors
+            gold_standard,
+            priors,
+            full_model_betas=full_model,
+            full_model_var_exp=full_exp_var
         )
 
         return self.results
 
     def compute_common_data(self):
         """
         Compute common data structures like design and response matrices.
```

### Comparing `inferelator-0.6.1/inferelator/workflows/velocity_workflow.py` & `inferelator-0.6.2/inferelator/workflows/velocity_workflow.py`

 * *Files identical despite different names*

### Comparing `inferelator-0.6.1/inferelator/workflows/workflow_base.py` & `inferelator-0.6.2/inferelator/workflows/workflow_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,22 @@
     InferelatorDataLoader,
     DEFAULT_PANDAS_TSV_SETTINGS,
     slurm_envs,
     DotProduct
 )
 
 from inferelator.distributed.inferelator_mp import MPControl
-from inferelator.preprocessing import ManagePriors, make_data_noisy
-from inferelator.postprocessing import ResultsProcessor, InferelatorResults
+from inferelator.preprocessing import (
+    ManagePriors,
+    make_data_noisy
+)
+from inferelator.postprocessing import (
+    ResultsProcessor,
+    InferelatorResults as IR
+)
 
 SBATCH_VARS_FOR_WORKFLOW = ["output_dir", "input_dir"]
 
 _TENX = "tenx"
 _TSV = "tsv"
 _H5AD = "h5ad"
 _HDF5 = "hdf5"
@@ -895,15 +901,16 @@
             filename
         )
 
     def output_path(self, filename):
         """
         Join filename to output_dir
 
-        :param filename: Path to some file that needs to be attached to the output path
+        :param filename: Path to some file that needs to be
+            attached to the output path
         :type filename: str
         :return: File joined to output_dir instance variable
         :rtype: str
         """
         return InferelatorDataLoader.filename_path_join(
             self.output_dir,
             filename
@@ -927,16 +934,17 @@
 
         self.data.to_h5ad(self.output_path(output_file_name))
 
     @staticmethod
     def _create_null_prior(gene_names, tf_names):
         """
         Create a prior data matrix that is all 0s
-        :param gene_names: Anything that can be used as an index for a dataframe
-        :param tf_names: list
+        :param gene_names: Anything that can be used as an index
+            for a dataframe
+        :param tf_names: list, pd.Index
         :return priors: pd.DataFrame
         """
 
         if tf_names is None:
             raise ValueError(
                 "Unable to generate a null prior without a TF list"
             )
@@ -1008,15 +1016,16 @@
             raise ValueError(_msg)
         elif _repeated:
             Debug.vprint(_msg, level=0)
 
 
 class WorkflowBase(WorkflowBaseLoader):
     """
-    WorkflowBase handles crossvalidation, shuffling, and validating priors and gold standards
+    WorkflowBase handles crossvalidation, shuffling, and
+    validating priors and gold standards
     """
     # Flags to control splitting priors into a prior/gold-standard set
     split_gold_standard_for_crossvalidation = False
     cv_split_ratio = None
     cv_split_axis = 0
 
     # Flags to control shuffle and noise baselines
@@ -1053,128 +1062,201 @@
     results = None
 
     def __init__(self):
         super(WorkflowBase, self).__init__()
         # Get environment variables
         self.get_environmentals()
 
-    def set_crossvalidation_parameters(self, split_gold_standard_for_crossvalidation=None, cv_split_ratio=None,
-                                       cv_split_axis=None):
+    def set_crossvalidation_parameters(
+        self,
+        split_gold_standard_for_crossvalidation=None,
+        cv_split_ratio=None,
+        cv_split_axis=None
+    ):
         """
         Set parameters for crossvalidation.
 
-        :param split_gold_standard_for_crossvalidation: Boolean flag indicating if the gold standard should be
-            split. Must be set to True for other crossvalidation settings to have an effect. Defaults to False.
+        :param split_gold_standard_for_crossvalidation: Boolean flag indicating
+            if the gold standard should be split. Must be set to True for other
+            crossvalidation settings to have an effect. Defaults to False.
         :type split_gold_standard_for_crossvalidation: bool
-        :param cv_split_ratio: The proportion of the gold standard which should be retained for scoring. The rest will
-            be used to train the model. Must be set betweeen 0 and 1.
+        :param cv_split_ratio: The proportion of the gold standard which should
+            be retained for scoring. The rest will be used to train the model.
+            Must be set betweeen 0 and 1.
         :type cv_split_ratio: float
-        :param cv_split_axis: How to split the gold standard. If 0, split genes; this will take all the data for certain
-            genes and keep it in the gold standard. These genes will be removed from the prior. If 1, split regulators;
-            this will take all the data for certain regulators and keep it in the gold standard. These regulators will
-            be removed from the prior. Splitting regulators is inadvisable. If None, the prior will be replaced with a
-            downsampled gold standard. Setting this to 0 is generally the best choice.
-            Defaults to None.
+        :param cv_split_axis: How to split the gold standard.
+
+            If 0, split genes; this will take all the data for certain genes
+            and keep it in the gold standard. These genes will be removed from
+            the prior.
+
+            If 1, split regulators; this will take all the data for certain
+            regulatorsnand keep it in the gold standard. These regulators will
+            be removed from the prior. Splitting regulators is inadvisable.
+
+            If None, the prior will be replaced with a downsampled gold
+            standard.
+
+            Setting this to 0 is generally the best choice. Defaults to None.
+
         :type cv_split_axis: int, None
 
         """
 
-        self._set_without_warning("split_gold_standard_for_crossvalidation", split_gold_standard_for_crossvalidation)
-        self._set_with_warning("cv_split_ratio", cv_split_ratio)
-        self._set_with_warning("cv_split_axis", cv_split_axis)
+        self._set_without_warning(
+            "split_gold_standard_for_crossvalidation",
+            split_gold_standard_for_crossvalidation
+        )
+        self._set_with_warning(
+            "cv_split_ratio",
+            cv_split_ratio
+        )
+        self._set_with_warning(
+            "cv_split_axis",
+            cv_split_axis
+        )
 
-        if not split_gold_standard_for_crossvalidation and (cv_split_axis is not None or cv_split_ratio is not None):
-            warnings.warn("The split_gold_standard_for_crossvalidation flag is not set. Other options may be ignored")
+        if cv_split_axis is not None or cv_split_ratio is not None:
 
-    def set_shuffle_parameters(self, shuffle_prior_axis=None, make_data_noise=None, add_prior_noise=None):
+            if not self.split_gold_standard_for_crossvalidation:
+                warnings.warn(
+                    "The split_gold_standard_for_crossvalidation flag is not set. "
+                    "Other options may be ignored"
+                )
+
+    def set_shuffle_parameters(
+        self,
+        shuffle_prior_axis=None,
+        make_data_noise=None,
+        add_prior_noise=None
+    ):
         """
-        Set parameters for shuffling labels on a prior axis. This is useful to establish a baseline.
+        Set parameters for shuffling labels on a prior axis. This is useful
+        to establish a baseline.
 
-        :param shuffle_prior_axis: The axis for shuffling prior labels. 0 shuffles gene labels. 1 shuffles regulator
-            labels. None means labels will not be shuffled. Defaults to None.
+        :param shuffle_prior_axis: The axis for shuffling prior labels.
+            0 shuffles gene labels.
+            1 shuffles regulator labels.
+            None means labels will not be shuffled.
+            Defaults to None.
         :type shuffle_prior_axis: int, None
-        :param make_data_noise: Replace loaded data with simulated data that is entirely random. This retains type;
-            integer data remains integer, float remains float. Gene distributions should be centered around the
-            mean of gene expression in the original data, but is otherwise random.
+        :param make_data_noise: Replace loaded data with simulated data
+            that is entirely random. This retains type; integer data remains
+            integer, float remains float. Gene distributions should be
+            centered around the mean of gene expression in the original data,
+            but is otherwise random.
         :type make_data_noise: bool, None
-        :param add_prior_noise: Add random edges to the prior data. This is a numeric value between 0 and 1 such that 0
-            adds no edges, 1 sets every edge in the prior to True, 0.1 sets 10% of the edges in the prior to True, and
-            so on. Note that this will binarize the prior if it is not already binary.
+        :param add_prior_noise: Add random edges to the prior data.
+            This is a numeric value between 0 and 1 such that
+            0 adds no edges,
+            1 sets every edge in the prior to True,
+            0.1 sets 10% of the edges in the prior to True,
+            and so on.
+            Note that this will binarize the prior if it is not already binary.
         :type add_prior_noise: numeric, None
         """
         self._set_with_warning("shuffle_prior_axis", shuffle_prior_axis)
         self._set_with_warning("make_data_noise", make_data_noise)
         self._set_with_warning("add_prior_noise", add_prior_noise)
 
-    def set_postprocessing_parameters(self, gold_standard_filter_method=None, metric=None):
+    def set_postprocessing_parameters(
+        self,
+        gold_standard_filter_method=None,
+        metric=None
+    ):
         """
         Set parameters for the postprocessing engine
 
-        :param gold_standard_filter_method: A flag that determines if the gold standard should be shrunk to the
-            size of the produced model. "overlap" will only score on overlap between the gold standard and the
-            inferred gene regulatory network. "keep_all_gold_standard" will score on the entire gold standard.
+        :param gold_standard_filter_method: A flag that determines if the
+            old standard should be shrunk to the size of the produced model.
+            "overlap" will only score on overlap between the gold standard
+            and the inferred gene regulatory network.
+            "keep_all_gold_standard" will score on the entire gold standard.
             Defaults to "keep_all_gold_standard".
         :type gold_standard_filter_method: str
-        :param metric: The model metric to use for scoring. Supports "precision-recall", "mcc", "f1", and "combined"
+        :param metric: The model metric to use for scoring. Supports
+            "precision-recall", "mcc", "f1", and "combined"
             Defaults to "combined".
         :type metric: str
         """
 
-        self._set_with_warning("gold_standard_filter_method", gold_standard_filter_method)
-        self._set_with_warning("metric", metric)
+        self._set_with_warning(
+            "gold_standard_filter_method",
+            gold_standard_filter_method
+        )
+        self._set_with_warning(
+            "metric",
+            metric
+        )
 
     @staticmethod
-    def set_output_file_names(network_file_name="", confidence_file_name="", nonzero_coefficient_file_name="",
-                              pdf_curve_file_name="", curve_data_file_name=""):
+    def set_output_file_names(
+        network_file_name="",
+        confidence_file_name="",
+        nonzero_coefficient_file_name="",
+        pdf_curve_file_name="",
+        curve_data_file_name=""
+    ):
         """
         Set output file names. File names that end in '.gz' will be gzipped.
 
-        :param network_file_name: Long-format network TSV file with TF->Gene edge information.
+        :param network_file_name: Long-format network TSV file with
+            TF->Gene edge information.
             Default is "network.tsv".
         :type network_file_name: str
-        :param confidence_file_name: Genes x TFs TSV with confidence scores for each edge.
+        :param confidence_file_name: Genes x TFs TSV with confidence
+            scores for each edge.
             Default is "combined_confidences.tsv"
         :type confidence_file_name: str
-        :param nonzero_coefficient_file_name: Genes x TFs TSV with the number of non-zero model coefficients for each
-            edge. Default is None (this file is not produced).
+        :param nonzero_coefficient_file_name: Genes x TFs TSV with
+            the non-zero model coefficients for each
+            edge. Default is "model_coefficients.tsv.gz"
         :type nonzero_coefficient_file_name: str
-        :param pdf_curve_file_name: PDF file with plotted curve(s). Default is "combined_metrics.pdf".
+        :param pdf_curve_file_name: PDF file with plotted curve(s).
+            Default is "combined_metrics.pdf".
         :type pdf_curve_file_name: str
-        :param curve_data_file_name: TSV file with the data used to plot curves.
-            Default is None (this file is not produced).
+        :param curve_data_file_name: TSV file with the data used to plot
+            curves. Default is None (this file is not produced).
         :type curve_data_file_name: str
         """
 
         if network_file_name != "":
-            InferelatorResults.network_file_name = network_file_name
+            IR.network_file_name = network_file_name
         if confidence_file_name != "":
-            InferelatorResults.confidence_file_name = confidence_file_name
+            IR.confidence_file_name = confidence_file_name
         if nonzero_coefficient_file_name != "":
-            InferelatorResults.threshold_file_name = nonzero_coefficient_file_name
+            IR.threshold_file_name = nonzero_coefficient_file_name
         if pdf_curve_file_name != "":
-            InferelatorResults.curve_file_name = pdf_curve_file_name
+            IR.curve_file_name = pdf_curve_file_name
         if curve_data_file_name != "":
-            InferelatorResults.curve_data_file_name = curve_data_file_name
+            IR.curve_data_file_name = curve_data_file_name
 
-    def set_run_parameters(self, num_bootstraps=None, random_seed=None, use_mkl=None, use_numba=None):
+    def set_run_parameters(
+        self,
+        num_bootstraps=None,
+        random_seed=None,
+        use_mkl=None,
+        use_numba=None
+    ):
         """
         Set parameters used during runtime
 
         :param num_bootstraps: The number of bootstraps to run.
             Defaults to 2.
         :type num_bootstraps: int
         :param random_seed: The random number seed to use.
             Defaults to 42.
         :type random_seed: int
         :param use_mkl: A flag to indicate if the intel MKL library
             should be used for matrix multiplication, defaults to False
         :type use_mkl: bool
         :param use_numba: A flag to indicate if numba should be used
-            to accelerate the calculations. Requires numba to be installed if set.
-            Currently only accelerates AMuSR regression, defaults to True
+            to accelerate the calculations. Requires numba to be installed
+            if set. Currently only accelerates AMuSR regression, defaults
+            to True
         :type use_numba: bool
         """
 
         self._set_without_warning("num_bootstraps", num_bootstraps)
         self._set_without_warning("random_seed", random_seed)
         self._set_without_warning("use_mkl", use_mkl)
         self._set_without_warning("use_numba", use_numba)
@@ -1206,21 +1288,23 @@
             self.initialize_multiprocessing()
 
         self.startup_run()
         self.startup_finish()
 
     def startup_run(self):
         """
-        Execute any data preprocessing necessary before regression. Startup_run is mostly for reading in data
+        Execute any data preprocessing necessary before regression.
+        Startup_run is mostly for reading in data
         """
         raise NotImplementedError  # implement in subclass
 
     def startup_finish(self):
         """
-        Execute any data preprocessing necessary before regression. Startup_finish is mostly for preprocessing data
+        Execute any data preprocessing necessary before regression.
+        Startup_finish is mostly for preprocessing data
         prior to regression
         """
         raise NotImplementedError  # implement in subclass
 
     def run(self):
         """
         Execute workflow, after all configuration.
@@ -1229,61 +1313,84 @@
 
     def process_priors_and_gold_standard(self):
         """
         Run split, shuffle, etc called for by the workflow flags
         This also filters the expression matrix to the list of genes to model
         """
 
+        pm = self.prior_manager
+
         # Split gold standard for cross-validation
         if self.split_gold_standard_for_crossvalidation:
-            self.priors_data, self.gold_standard = self.prior_manager.cross_validate_gold_standard(self.priors_data,
-                                                                                                   self.gold_standard,
-                                                                                                   self.cv_split_axis,
-                                                                                                   self.cv_split_ratio,
-                                                                                                   self.random_seed)
+            self.priors_data, self.gold_standard = pm.cross_validate_gold_standard(
+                self.priors_data,
+                self.gold_standard,
+                self.cv_split_axis,
+                self.cv_split_ratio,
+                self.random_seed
+            )
 
         # Filter priors to a list of regulators
         if self.tf_names is not None:
-            self.priors_data = self.prior_manager.filter_to_tf_names_list(self.priors_data, self.tf_names)
+            self.priors_data = pm.filter_to_tf_names_list(
+                self.priors_data,
+                self.tf_names
+            )
+
         elif self.tf_names is None and self.priors_data is not None:
             self.tf_names = self.priors_data.columns.tolist()
+
         elif self.tf_names is None:
-            raise ValueError("Either a priors_data or a tf_names file must be provided to identify regulators.")
+            raise ValueError(
+                "Either a priors_data or a tf_names file must be provided "
+                "to identify regulators."
+            )
 
         # Filter priors and expression to a list of genes
         self.filter_to_gene_list()
 
         # Shuffle prior labels
         if self.shuffle_prior_axis is not None:
-            self.priors_data = self.prior_manager.shuffle_priors(self.priors_data,
-                                                                 self.shuffle_prior_axis,
-                                                                 self.random_seed)
+            self.priors_data = pm.shuffle_priors(
+                self.priors_data,
+                self.shuffle_prior_axis,
+                self.random_seed
+            )
 
         # Check for duplicates or whatever
-        self.priors_data, self.gold_standard = self.prior_manager.validate_priors_gold_standard(self.priors_data,
-                                                                                                self.gold_standard)
+        self.priors_data, self.gold_standard = pm.validate_priors_gold_standard(
+            self.priors_data,
+            self.gold_standard
+        )
 
         if self.add_prior_noise is not None:
-            self.priors_data = self.prior_manager.add_prior_noise(self.priors_data, self.add_prior_noise,
-                                                                  self.random_seed)
+            self.priors_data = pm.add_prior_noise(
+                self.priors_data,
+                self.add_prior_noise,
+                self.random_seed
+            )
 
     def filter_to_gene_list(self):
         """
         Filter the priors and expression matrix to just genes in gene_metadata
         """
-
-        Debug.vprint("Trimming expression matrix", level=1)
         self.data.trim_genes(trim_gene_list=self.gene_names)
-        self.priors_data = self.prior_manager.filter_priors_to_genes(self.priors_data, self.data.gene_names)
+        self.priors_data = self.prior_manager.filter_priors_to_genes(
+            self.priors_data,
+            self.data.gene_names
+        )
 
     def align_priors_and_expression(self):
         """
         Align prior to the expression matrix
         """
-        self.priors_data = self.prior_manager.align_priors_to_expression(self.priors_data, self.data.gene_names)
+        self.priors_data = self.prior_manager.align_priors_to_expression(
+            self.priors_data,
+            self.data.gene_names
+        )
         self.data_white_noise()
 
     def data_white_noise(self):
         """
         Replace data with white noise data
         """
 
@@ -1291,37 +1398,58 @@
             make_data_noisy(self.data, random_seed=self.random_seed)
             self._data_is_noise = True
 
     def get_bootstraps(self):
         """
         Generate sequence of bootstrap parameter objects for run.
         """
-        col_range = range(self._num_obs)
-        random_state = np.random.RandomState(seed=self.random_seed)
-        return random_state.choice(col_range, size=(self.num_bootstraps, self._num_obs)).tolist()
+        return np.random.RandomState(seed=self.random_seed).choice(
+            range(self._num_obs),
+            size=(self.num_bootstraps, self._num_obs)
+        ).tolist()
 
-    def emit_results(self, betas, rescaled_betas, gold_standard, priors):
+    def emit_results(
+        self,
+        betas,
+        rescaled_betas,
+        gold_standard,
+        priors,
+        full_model=None,
+        full_exp_var=None
+    ):
         """
         Output result report(s) for workflow run.
         """
         raise NotImplementedError  # implement in subclass
 
     def create_output_dir(self):
         """
-        Set a default output_dir if nothing is set. Create the path if it doesn't exist.
+        Set a default output_dir if nothing is set.
+        Create the path if it doesn't exist.
         """
+
         if self.output_dir is None:
-            new_path = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
-            self.output_dir = InferelatorDataLoader.make_path_safe(os.path.join(self.input_dir, new_path))
+            self.output_dir = InferelatorDataLoader.make_path_safe(
+                os.path.join(
+                    self.input_dir,
+                    datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+                )
+            )
+
         else:
-            self.output_dir = InferelatorDataLoader.make_path_safe(self.output_dir)
+            self.output_dir = InferelatorDataLoader.make_path_safe(
+                self.output_dir
+            )
 
+        # Create the output directory
         try:
-            os.makedirs(os.path.expanduser(self.output_dir))
+            os.makedirs(self.output_dir)
         except FileExistsError:
             pass
 
     def create_task(self, **kwargs):
         """
         Create a task data object
         """
-        raise NotImplementedError("This workflow does not support multiple tasks")
+        raise NotImplementedError(
+            "This workflow does not support multiple tasks"
+        )
```

### Comparing `inferelator-0.6.1/inferelator.egg-info/PKG-INFO` & `inferelator-0.6.2/inferelator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferelator
-Version: 0.6.1
+Version: 0.6.2
 Summary: Inferelator: Network Inference
 Home-page: https://github.com/flatironinstitute/inferelator
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 Maintainer: Chris Jackson
 Maintainer-email: cj59@nyu.edu
 Project-URL: Documentation, https://inferelator.readthedocs.io/
```

### Comparing `inferelator-0.6.1/inferelator.egg-info/SOURCES.txt` & `inferelator-0.6.2/inferelator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 inferelator/postprocessing/inferelator_results.py
 inferelator/postprocessing/matthews_correlation.py
 inferelator/postprocessing/model_metrics.py
 inferelator/postprocessing/model_performance.py
 inferelator/postprocessing/precision_recall.py
 inferelator/postprocessing/results_processor.py
 inferelator/postprocessing/results_processor_mtl.py
+inferelator/predict/__init__.py
+inferelator/predict/dynamic.py
+inferelator/predict/static.py
 inferelator/preprocessing/__init__.py
+inferelator/preprocessing/data_normalization.py
 inferelator/preprocessing/design_response_translation.py
 inferelator/preprocessing/metadata_parser.py
 inferelator/preprocessing/priors.py
 inferelator/preprocessing/simulate_data.py
 inferelator/preprocessing/single_cell.py
 inferelator/preprocessing/tfa.py
 inferelator/preprocessing/velocity.py
@@ -57,14 +61,15 @@
 inferelator/tfa/pinv_tfa.py
 inferelator/tfa/ridge_tfa.py
 inferelator/tfa/tfa_base.py
 inferelator/tfa/velocity_tfa.py
 inferelator/utils/__init__.py
 inferelator/utils/data.py
 inferelator/utils/debug.py
+inferelator/utils/inferelator_data.py
 inferelator/utils/loader.py
 inferelator/utils/profiler.py
 inferelator/utils/validator.py
 inferelator/workflows/__init__.py
 inferelator/workflows/amusr_workflow.py
 inferelator/workflows/homology_workflow.py
 inferelator/workflows/single_cell_workflow.py
```

### Comparing `inferelator-0.6.1/setup.py` & `inferelator-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 from setuptools import setup, find_packages
 
 # Current Inferelator Version Number
-version = "0.6.1"
+version = "0.6.2"
 
 
 # Description from README.md
 base_dir = os.path.dirname(os.path.abspath(__file__))
 long_description = "\n\n".join([open(os.path.join(base_dir, "README.md"), "r").read()])
 
 # Required packages
 requires = [
     "numpy >=1.14.0",
     "scipy >=0.9",
     "pandas >=0.24.0",
     "scikit-learn",
     "matplotlib >=1.5.1",
-    "anndata >=0.7.4"
+    "anndata >=0.9.0 "
 ]
 
 setup(
     name="inferelator",
     version=version,
     description="Inferelator: Network Inference",
     long_description=long_description,
```


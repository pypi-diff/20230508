# Comparing `tmp/comet_ml-3.9.0.tar.gz` & `tmp/comet_ml-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/comet_ml-3.9.0.tar", last modified: Thu Apr 15 14:13:28 2021, max compression
+gzip compressed data, was "dist/comet_ml-3.9.1.tar", last modified: Thu May  6 16:12:18 2021, max compression
```

## Comparing `comet_ml-3.9.0.tar` & `comet_ml-3.9.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.114998 comet_ml-3.9.0/
--rw-r--r--   0 jenkins   (1001)      999       48 2020-06-16 13:59:18.000000 comet_ml-3.9.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1001)      999     2611 2021-04-15 14:13:28.114998 comet_ml-3.9.0/PKG-INFO
--rw-r--r--   0 jenkins   (1001)      999     1505 2020-06-16 13:59:18.000000 comet_ml-3.9.0/README.rst
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.110998 comet_ml-3.9.0/comet_ml/
--rw-r--r--   0 jenkins   (1001)      999    37577 2021-03-24 17:13:14.000000 comet_ml-3.9.0/comet_ml/__init__.py
--rw-r--r--   0 jenkins   (1001)      999     1717 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/_jupyter.py
--rw-r--r--   0 jenkins   (1001)      999     9623 2021-04-13 19:25:49.000000 comet_ml-3.9.0/comet_ml/_logging.py
--rw-r--r--   0 jenkins   (1001)      999     1164 2021-02-12 16:48:51.000000 comet_ml-3.9.0/comet_ml/_reporting.py
--rw-r--r--   0 jenkins   (1001)      999     1206 2021-01-13 22:39:34.000000 comet_ml-3.9.0/comet_ml/_typing.py
--rw-r--r--   0 jenkins   (1001)      999   120612 2021-03-29 09:35:53.000000 comet_ml-3.9.0/comet_ml/api.py
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.110998 comet_ml-3.9.0/comet_ml/bootstrap/
--rw-r--r--   0 jenkins   (1001)      999      565 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/bootstrap/__init__.py
--rw-r--r--   0 jenkins   (1001)      999     1208 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/bootstrap/sitecustomize.py
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.110998 comet_ml-3.9.0/comet_ml/callbacks/
--rw-r--r--   0 jenkins   (1001)      999      565 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/callbacks/__init__.py
--rw-r--r--   0 jenkins   (1001)      999    31630 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/callbacks/_base.py
--rw-r--r--   0 jenkins   (1001)      999     1370 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/callbacks/_keras.py
--rw-r--r--   0 jenkins   (1001)      999     2326 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/callbacks/_lgbm.py
--rw-r--r--   0 jenkins   (1001)      999     1910 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/callbacks/_tensorflow.py
--rw-r--r--   0 jenkins   (1001)      999     2183 2021-01-27 21:43:39.000000 comet_ml-3.9.0/comet_ml/callbacks/_tensorflow_estimator.py
--rw-r--r--   0 jenkins   (1001)      999     1036 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/callbacks/_tensorflow_keras.py
--rw-r--r--   0 jenkins   (1001)      999    32227 2021-04-13 19:25:49.000000 comet_ml-3.9.0/comet_ml/comet.py
--rw-r--r--   0 jenkins   (1001)      999     1345 2021-02-17 17:02:37.000000 comet_ml-3.9.0/comet_ml/compat_utils.py
--rw-r--r--   0 jenkins   (1001)      999    32652 2021-04-06 09:19:44.000000 comet_ml-3.9.0/comet_ml/config.py
--rw-r--r--   0 jenkins   (1001)      999    26000 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/confusion_matrix.py
--rw-r--r--   0 jenkins   (1001)      999   124564 2021-04-13 19:25:49.000000 comet_ml-3.9.0/comet_ml/connection.py
--rw-r--r--   0 jenkins   (1001)      999    18682 2021-03-16 18:31:54.000000 comet_ml-3.9.0/comet_ml/console.py
--rw-r--r--   0 jenkins   (1001)      999     7332 2021-03-31 13:13:06.000000 comet_ml-3.9.0/comet_ml/convert_utils.py
--rw-r--r--   0 jenkins   (1001)      999     3271 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/cpu_logging.py
--rw-r--r--   0 jenkins   (1001)      999     9358 2021-03-05 16:16:50.000000 comet_ml-3.9.0/comet_ml/env_logging.py
--rw-r--r--   0 jenkins   (1001)      999     7149 2021-03-16 18:31:54.000000 comet_ml-3.9.0/comet_ml/exceptions.py
--rw-r--r--   0 jenkins   (1001)      999   143650 2021-04-14 17:15:30.000000 comet_ml-3.9.0/comet_ml/experiment.py
--rw-r--r--   0 jenkins   (1001)      999     2357 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/feature_toggles.py
--rw-r--r--   0 jenkins   (1001)      999    32384 2021-03-31 13:13:06.000000 comet_ml-3.9.0/comet_ml/file_uploader.py
--rw-r--r--   0 jenkins   (1001)      999     9191 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/git_logging.py
--rw-r--r--   0 jenkins   (1001)      999     9037 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/gpu_logging.py
--rw-r--r--   0 jenkins   (1001)      999     2644 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/json_encoder.py
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.114998 comet_ml-3.9.0/comet_ml/loggers/
--rw-r--r--   0 jenkins   (1001)      999      565 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/loggers/__init__.py
--rw-r--r--   0 jenkins   (1001)      999     3033 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/fastai_logger.py
--rw-r--r--   0 jenkins   (1001)      999     4175 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/keras_logger.py
--rw-r--r--   0 jenkins   (1001)      999     2030 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/lightgbm_logger.py
--rw-r--r--   0 jenkins   (1001)      999     2827 2021-01-27 21:43:39.000000 comet_ml-3.9.0/comet_ml/loggers/logger_utils.py
--rw-r--r--   0 jenkins   (1001)      999     8215 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/mlflow_logger.py
--rw-r--r--   0 jenkins   (1001)      999     3839 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/prophet_logger.py
--rw-r--r--   0 jenkins   (1001)      999     5464 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/pytorch_logger.py
--rw-r--r--   0 jenkins   (1001)      999     3534 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/shap_logger.py
--rw-r--r--   0 jenkins   (1001)      999    23859 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/sklearn_logger.py
--rw-r--r--   0 jenkins   (1001)      999     8865 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/tensorboard_logger.py
--rw-r--r--   0 jenkins   (1001)      999    11706 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/tensorflow_logger.py
--rw-r--r--   0 jenkins   (1001)      999     3866 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/tfma_logger.py
--rw-r--r--   0 jenkins   (1001)      999     7530 2021-03-17 19:16:39.000000 comet_ml-3.9.0/comet_ml/loggers/xgboost_logger.py
--rw-r--r--   0 jenkins   (1001)      999     9957 2021-04-07 09:47:23.000000 comet_ml-3.9.0/comet_ml/logging_messages.py
--rw-r--r--   0 jenkins   (1001)      999     8214 2021-03-05 16:16:50.000000 comet_ml-3.9.0/comet_ml/messages.py
--rw-r--r--   0 jenkins   (1001)      999     6774 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/metrics.py
--rw-r--r--   0 jenkins   (1001)      999    10396 2021-04-13 19:25:49.000000 comet_ml-3.9.0/comet_ml/monkey_patching.py
--rw-r--r--   0 jenkins   (1001)      999    38656 2021-03-05 16:16:50.000000 comet_ml-3.9.0/comet_ml/offline.py
--rw-r--r--   0 jenkins   (1001)      999    23609 2021-04-13 19:25:49.000000 comet_ml-3.9.0/comet_ml/optimizer.py
--rw-r--r--   0 jenkins   (1001)      999     1018 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/papi.py
--rw-r--r--   0 jenkins   (1001)      999    18895 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/predictor.py
--rw-r--r--   0 jenkins   (1001)      999    16545 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/query.py
--rw-r--r--   0 jenkins   (1001)      999     3950 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/rpc.py
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.114998 comet_ml-3.9.0/comet_ml/schemas/
--rw-r--r--   0 jenkins   (1001)      999     7950 2021-01-13 22:39:34.000000 comet_ml-3.9.0/comet_ml/schemas/3d-points-bounding-box.schema.json
--rw-r--r--   0 jenkins   (1001)      999      926 2020-06-16 13:59:18.000000 comet_ml-3.9.0/comet_ml/schemas/offline-cloud-details-msg.schema.json
--rw-r--r--   0 jenkins   (1001)      999     1813 2020-11-03 20:34:05.000000 comet_ml-3.9.0/comet_ml/schemas/offline-experiment.schema.json
--rw-r--r--   0 jenkins   (1001)      999     3704 2020-08-19 18:28:57.000000 comet_ml-3.9.0/comet_ml/schemas/offline-file-upload-msg.schema.json
--rw-r--r--   0 jenkins   (1001)      999      673 2020-06-16 13:59:18.000000 comet_ml-3.9.0/comet_ml/schemas/offline-graph-msg.schema.json
--rw-r--r--   0 jenkins   (1001)      999      904 2020-06-16 13:59:18.000000 comet_ml-3.9.0/comet_ml/schemas/offline-os-packages-msg.schema.json
--rw-r--r--   0 jenkins   (1001)      999     2068 2021-02-01 10:44:22.000000 comet_ml-3.9.0/comet_ml/schemas/offline-remote-file-msg.schema.json
--rw-r--r--   0 jenkins   (1001)      999     6379 2021-03-05 16:16:50.000000 comet_ml-3.9.0/comet_ml/schemas/offline-system-details-msg.schema.json
--rw-r--r--   0 jenkins   (1001)      999    10559 2020-09-24 21:48:42.000000 comet_ml-3.9.0/comet_ml/schemas/offline-ws-msg.schema.json
--rw-r--r--   0 jenkins   (1001)      999     2666 2021-01-28 21:00:20.000000 comet_ml-3.9.0/comet_ml/schemas.py
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.114998 comet_ml-3.9.0/comet_ml/scripts/
--rw-r--r--   0 jenkins   (1001)      999        0 2020-06-16 13:59:18.000000 comet_ml-3.9.0/comet_ml/scripts/__init__.py
--rw-r--r--   0 jenkins   (1001)      999     4589 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/scripts/comet.py
--rw-r--r--   0 jenkins   (1001)      999    10343 2021-04-13 15:28:40.000000 comet_ml-3.9.0/comet_ml/scripts/comet_check.py
--rw-r--r--   0 jenkins   (1001)      999     4421 2021-04-06 09:19:44.000000 comet_ml-3.9.0/comet_ml/scripts/comet_init.py
--rw-r--r--   0 jenkins   (1001)      999     3923 2021-04-13 19:25:49.000000 comet_ml-3.9.0/comet_ml/scripts/comet_models.py
--rw-r--r--   0 jenkins   (1001)      999    14029 2021-02-09 15:46:11.000000 comet_ml-3.9.0/comet_ml/scripts/comet_offline.py
--rw-r--r--   0 jenkins   (1001)      999     7643 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/scripts/comet_optimize.py
--rw-r--r--   0 jenkins   (1001)      999     2760 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/scripts/comet_python.py
--rw-r--r--   0 jenkins   (1001)      999     1680 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/scripts/comet_upload.py
--rw-r--r--   0 jenkins   (1001)      999     8036 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/summary.py
--rw-r--r--   0 jenkins   (1001)      999     1062 2021-01-13 19:43:28.000000 comet_ml-3.9.0/comet_ml/tf_utils.py
--rw-r--r--   0 jenkins   (1001)      999    57694 2021-04-14 17:15:30.000000 comet_ml-3.9.0/comet_ml/utils.py
-drwxr-xr-x   0 jenkins   (1001)      999        0 2021-04-15 14:13:28.110998 comet_ml-3.9.0/comet_ml.egg-info/
--rw-r--r--   0 jenkins   (1001)      999     2611 2021-04-15 14:13:28.000000 comet_ml-3.9.0/comet_ml.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001)      999     2558 2021-04-15 14:13:28.000000 comet_ml-3.9.0/comet_ml.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001)      999        1 2021-04-15 14:13:28.000000 comet_ml-3.9.0/comet_ml.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001)      999       55 2021-04-15 14:13:28.000000 comet_ml-3.9.0/comet_ml.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001)      999      349 2021-04-15 14:13:28.000000 comet_ml-3.9.0/comet_ml.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001)      999        9 2021-04-15 14:13:28.000000 comet_ml-3.9.0/comet_ml.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001)      999       67 2021-04-15 14:13:28.114998 comet_ml-3.9.0/setup.cfg
--rw-r--r--   0 jenkins   (1001)      999     2214 2021-04-15 14:13:23.000000 comet_ml-3.9.0/setup.py
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.961371 comet_ml-3.9.1/
+-rw-r--r--   0 jenkins   (1001)      999       48 2020-06-16 13:59:18.000000 comet_ml-3.9.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001)      999     2611 2021-05-06 16:12:18.961371 comet_ml-3.9.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001)      999     1505 2020-06-16 13:59:18.000000 comet_ml-3.9.1/README.rst
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.957371 comet_ml-3.9.1/comet_ml/
+-rw-r--r--   0 jenkins   (1001)      999    37577 2021-03-24 17:13:14.000000 comet_ml-3.9.1/comet_ml/__init__.py
+-rw-r--r--   0 jenkins   (1001)      999     1717 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/_jupyter.py
+-rw-r--r--   0 jenkins   (1001)      999     9623 2021-04-13 19:25:49.000000 comet_ml-3.9.1/comet_ml/_logging.py
+-rw-r--r--   0 jenkins   (1001)      999     1164 2021-02-12 16:48:51.000000 comet_ml-3.9.1/comet_ml/_reporting.py
+-rw-r--r--   0 jenkins   (1001)      999     1206 2021-01-13 22:39:34.000000 comet_ml-3.9.1/comet_ml/_typing.py
+-rw-r--r--   0 jenkins   (1001)      999   120612 2021-03-29 09:35:53.000000 comet_ml-3.9.1/comet_ml/api.py
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.957371 comet_ml-3.9.1/comet_ml/bootstrap/
+-rw-r--r--   0 jenkins   (1001)      999      565 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/bootstrap/__init__.py
+-rw-r--r--   0 jenkins   (1001)      999     1208 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/bootstrap/sitecustomize.py
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.957371 comet_ml-3.9.1/comet_ml/callbacks/
+-rw-r--r--   0 jenkins   (1001)      999      565 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/callbacks/__init__.py
+-rw-r--r--   0 jenkins   (1001)      999    31630 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/callbacks/_base.py
+-rw-r--r--   0 jenkins   (1001)      999     1370 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/callbacks/_keras.py
+-rw-r--r--   0 jenkins   (1001)      999     2326 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/callbacks/_lgbm.py
+-rw-r--r--   0 jenkins   (1001)      999     1910 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/callbacks/_tensorflow.py
+-rw-r--r--   0 jenkins   (1001)      999     2183 2021-01-27 21:43:39.000000 comet_ml-3.9.1/comet_ml/callbacks/_tensorflow_estimator.py
+-rw-r--r--   0 jenkins   (1001)      999     1036 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/callbacks/_tensorflow_keras.py
+-rw-r--r--   0 jenkins   (1001)      999    32227 2021-04-13 19:25:49.000000 comet_ml-3.9.1/comet_ml/comet.py
+-rw-r--r--   0 jenkins   (1001)      999     1345 2021-02-17 17:02:37.000000 comet_ml-3.9.1/comet_ml/compat_utils.py
+-rw-r--r--   0 jenkins   (1001)      999    32652 2021-04-06 09:19:44.000000 comet_ml-3.9.1/comet_ml/config.py
+-rw-r--r--   0 jenkins   (1001)      999    26000 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/confusion_matrix.py
+-rw-r--r--   0 jenkins   (1001)      999   124401 2021-05-05 17:51:39.000000 comet_ml-3.9.1/comet_ml/connection.py
+-rw-r--r--   0 jenkins   (1001)      999    18682 2021-03-16 18:31:54.000000 comet_ml-3.9.1/comet_ml/console.py
+-rw-r--r--   0 jenkins   (1001)      999     7332 2021-03-31 13:13:06.000000 comet_ml-3.9.1/comet_ml/convert_utils.py
+-rw-r--r--   0 jenkins   (1001)      999     3271 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/cpu_logging.py
+-rw-r--r--   0 jenkins   (1001)      999     9358 2021-03-05 16:16:50.000000 comet_ml-3.9.1/comet_ml/env_logging.py
+-rw-r--r--   0 jenkins   (1001)      999     7149 2021-03-16 18:31:54.000000 comet_ml-3.9.1/comet_ml/exceptions.py
+-rw-r--r--   0 jenkins   (1001)      999   143650 2021-04-14 17:15:30.000000 comet_ml-3.9.1/comet_ml/experiment.py
+-rw-r--r--   0 jenkins   (1001)      999     2357 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/feature_toggles.py
+-rw-r--r--   0 jenkins   (1001)      999    32384 2021-03-31 13:13:06.000000 comet_ml-3.9.1/comet_ml/file_uploader.py
+-rw-r--r--   0 jenkins   (1001)      999     9191 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/git_logging.py
+-rw-r--r--   0 jenkins   (1001)      999     9037 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/gpu_logging.py
+-rw-r--r--   0 jenkins   (1001)      999     2644 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/json_encoder.py
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.957371 comet_ml-3.9.1/comet_ml/loggers/
+-rw-r--r--   0 jenkins   (1001)      999      565 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/loggers/__init__.py
+-rw-r--r--   0 jenkins   (1001)      999     3033 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/fastai_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     4175 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/keras_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     2030 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/lightgbm_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     2827 2021-01-27 21:43:39.000000 comet_ml-3.9.1/comet_ml/loggers/logger_utils.py
+-rw-r--r--   0 jenkins   (1001)      999     8215 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/mlflow_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     3839 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/prophet_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     5464 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/pytorch_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     3534 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/shap_logger.py
+-rw-r--r--   0 jenkins   (1001)      999    24109 2021-04-26 08:49:45.000000 comet_ml-3.9.1/comet_ml/loggers/sklearn_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     8865 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/tensorboard_logger.py
+-rw-r--r--   0 jenkins   (1001)      999    11706 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/tensorflow_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     3866 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/tfma_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     7530 2021-03-17 19:16:39.000000 comet_ml-3.9.1/comet_ml/loggers/xgboost_logger.py
+-rw-r--r--   0 jenkins   (1001)      999     9957 2021-04-07 09:47:23.000000 comet_ml-3.9.1/comet_ml/logging_messages.py
+-rw-r--r--   0 jenkins   (1001)      999     8214 2021-03-05 16:16:50.000000 comet_ml-3.9.1/comet_ml/messages.py
+-rw-r--r--   0 jenkins   (1001)      999     6774 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/metrics.py
+-rw-r--r--   0 jenkins   (1001)      999    10396 2021-04-13 19:25:49.000000 comet_ml-3.9.1/comet_ml/monkey_patching.py
+-rw-r--r--   0 jenkins   (1001)      999    38656 2021-03-05 16:16:50.000000 comet_ml-3.9.1/comet_ml/offline.py
+-rw-r--r--   0 jenkins   (1001)      999    23609 2021-04-13 19:25:49.000000 comet_ml-3.9.1/comet_ml/optimizer.py
+-rw-r--r--   0 jenkins   (1001)      999     1018 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/papi.py
+-rw-r--r--   0 jenkins   (1001)      999    18895 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/predictor.py
+-rw-r--r--   0 jenkins   (1001)      999    16545 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/query.py
+-rw-r--r--   0 jenkins   (1001)      999     3950 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/rpc.py
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.961371 comet_ml-3.9.1/comet_ml/schemas/
+-rw-r--r--   0 jenkins   (1001)      999     7950 2021-01-13 22:39:34.000000 comet_ml-3.9.1/comet_ml/schemas/3d-points-bounding-box.schema.json
+-rw-r--r--   0 jenkins   (1001)      999      926 2020-06-16 13:59:18.000000 comet_ml-3.9.1/comet_ml/schemas/offline-cloud-details-msg.schema.json
+-rw-r--r--   0 jenkins   (1001)      999     1813 2020-11-03 20:34:05.000000 comet_ml-3.9.1/comet_ml/schemas/offline-experiment.schema.json
+-rw-r--r--   0 jenkins   (1001)      999     3704 2020-08-19 18:28:57.000000 comet_ml-3.9.1/comet_ml/schemas/offline-file-upload-msg.schema.json
+-rw-r--r--   0 jenkins   (1001)      999      673 2020-06-16 13:59:18.000000 comet_ml-3.9.1/comet_ml/schemas/offline-graph-msg.schema.json
+-rw-r--r--   0 jenkins   (1001)      999      904 2020-06-16 13:59:18.000000 comet_ml-3.9.1/comet_ml/schemas/offline-os-packages-msg.schema.json
+-rw-r--r--   0 jenkins   (1001)      999     2068 2021-02-01 10:44:22.000000 comet_ml-3.9.1/comet_ml/schemas/offline-remote-file-msg.schema.json
+-rw-r--r--   0 jenkins   (1001)      999     6379 2021-03-05 16:16:50.000000 comet_ml-3.9.1/comet_ml/schemas/offline-system-details-msg.schema.json
+-rw-r--r--   0 jenkins   (1001)      999    10559 2020-09-24 21:48:42.000000 comet_ml-3.9.1/comet_ml/schemas/offline-ws-msg.schema.json
+-rw-r--r--   0 jenkins   (1001)      999     2666 2021-01-28 21:00:20.000000 comet_ml-3.9.1/comet_ml/schemas.py
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.961371 comet_ml-3.9.1/comet_ml/scripts/
+-rw-r--r--   0 jenkins   (1001)      999        0 2020-06-16 13:59:18.000000 comet_ml-3.9.1/comet_ml/scripts/__init__.py
+-rw-r--r--   0 jenkins   (1001)      999     4589 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/scripts/comet.py
+-rw-r--r--   0 jenkins   (1001)      999    10343 2021-04-13 15:28:40.000000 comet_ml-3.9.1/comet_ml/scripts/comet_check.py
+-rw-r--r--   0 jenkins   (1001)      999     4421 2021-04-06 09:19:44.000000 comet_ml-3.9.1/comet_ml/scripts/comet_init.py
+-rw-r--r--   0 jenkins   (1001)      999     3923 2021-04-13 19:25:49.000000 comet_ml-3.9.1/comet_ml/scripts/comet_models.py
+-rw-r--r--   0 jenkins   (1001)      999    14029 2021-02-09 15:46:11.000000 comet_ml-3.9.1/comet_ml/scripts/comet_offline.py
+-rw-r--r--   0 jenkins   (1001)      999     7643 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/scripts/comet_optimize.py
+-rw-r--r--   0 jenkins   (1001)      999     2760 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/scripts/comet_python.py
+-rw-r--r--   0 jenkins   (1001)      999     1680 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/scripts/comet_upload.py
+-rw-r--r--   0 jenkins   (1001)      999     8036 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/summary.py
+-rw-r--r--   0 jenkins   (1001)      999     1062 2021-01-13 19:43:28.000000 comet_ml-3.9.1/comet_ml/tf_utils.py
+-rw-r--r--   0 jenkins   (1001)      999    57694 2021-04-14 17:15:30.000000 comet_ml-3.9.1/comet_ml/utils.py
+drwxr-xr-x   0 jenkins   (1001)      999        0 2021-05-06 16:12:18.957371 comet_ml-3.9.1/comet_ml.egg-info/
+-rw-r--r--   0 jenkins   (1001)      999     2611 2021-05-06 16:12:18.000000 comet_ml-3.9.1/comet_ml.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001)      999     2558 2021-05-06 16:12:18.000000 comet_ml-3.9.1/comet_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001)      999        1 2021-05-06 16:12:18.000000 comet_ml-3.9.1/comet_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001)      999       55 2021-05-06 16:12:18.000000 comet_ml-3.9.1/comet_ml.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001)      999      349 2021-05-06 16:12:18.000000 comet_ml-3.9.1/comet_ml.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001)      999        9 2021-05-06 16:12:18.000000 comet_ml-3.9.1/comet_ml.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001)      999       67 2021-05-06 16:12:18.961371 comet_ml-3.9.1/setup.cfg
+-rw-r--r--   0 jenkins   (1001)      999     2214 2021-05-06 16:12:13.000000 comet_ml-3.9.1/setup.py
```

### Comparing `comet_ml-3.9.0/PKG-INFO` & `comet_ml-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_ml
-Version: 3.9.0
+Version: 3.9.1
 Summary: Supercharging Machine Learning
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Description: Comet.ml
         ========
```

### Comparing `comet_ml-3.9.0/README.rst` & `comet_ml-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/__init__.py` & `comet_ml-3.9.1/comet_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/_jupyter.py` & `comet_ml-3.9.1/comet_ml/_jupyter.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/_logging.py` & `comet_ml-3.9.1/comet_ml/_logging.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/_reporting.py` & `comet_ml-3.9.1/comet_ml/_reporting.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/_typing.py` & `comet_ml-3.9.1/comet_ml/_typing.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/api.py` & `comet_ml-3.9.1/comet_ml/api.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/bootstrap/__init__.py` & `comet_ml-3.9.1/comet_ml/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/bootstrap/sitecustomize.py` & `comet_ml-3.9.1/comet_ml/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/callbacks/__init__.py` & `comet_ml-3.9.1/comet_ml/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/callbacks/_base.py` & `comet_ml-3.9.1/comet_ml/callbacks/_base.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/callbacks/_keras.py` & `comet_ml-3.9.1/comet_ml/callbacks/_keras.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/callbacks/_lgbm.py` & `comet_ml-3.9.1/comet_ml/callbacks/_lgbm.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/callbacks/_tensorflow.py` & `comet_ml-3.9.1/comet_ml/callbacks/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/callbacks/_tensorflow_estimator.py` & `comet_ml-3.9.1/comet_ml/callbacks/_tensorflow_estimator.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/callbacks/_tensorflow_keras.py` & `comet_ml-3.9.1/comet_ml/callbacks/_tensorflow_keras.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/comet.py` & `comet_ml-3.9.1/comet_ml/comet.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/compat_utils.py` & `comet_ml-3.9.1/comet_ml/compat_utils.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/config.py` & `comet_ml-3.9.1/comet_ml/config.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/confusion_matrix.py` & `comet_ml-3.9.1/comet_ml/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/connection.py` & `comet_ml-3.9.1/comet_ml/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1990,17 +1990,15 @@
         }
         return self.post_from_endpoint("project/query", payload)
 
     def get_project_columns(self, workspace, project_name):
         """
         Given a workspace and project_name return the column names, types, etc.
         """
-        # No "ver" included - signals to the backend that we cannot receive below items:
-        # "ver": 2 - signals to the backend that we can receive "env_details"
-        payload = {"workspaceName": workspace, "projectName": project_name, "ver": 2}
+        payload = {"workspaceName": workspace, "projectName": project_name}
         return self.get_from_endpoint("project/column-names", payload)
 
     # Write methods:
 
     def update_project(
         self,
         workspace,
@@ -3002,15 +3000,15 @@
             comment: optional, a textual comment about the model
             stages: optional, a list of textual tags such as ["production", "staging"] etc.
 
         Returns 200 Response if successful
         """
         models = self.get_experiment_models(experiment_id)
         if len(models) == 0:
-            raise ValueError("There are no models for this experiment")
+            raise ValueError("There are no models for experiment %r" % experiment_id)
         # Look up the model name:
         details = [model for model in models if model["modelName"] == model_name]
         # If model name found:
         if len(details) == 1:
             registry_name = registry_name or proper_registry_model_name(model_name)
             registry_models = [model for model in self.get_registry_models(workspace)]
             model_id = details[0]["experimentModelId"]
```

### Comparing `comet_ml-3.9.0/comet_ml/console.py` & `comet_ml-3.9.1/comet_ml/console.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/convert_utils.py` & `comet_ml-3.9.1/comet_ml/convert_utils.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/cpu_logging.py` & `comet_ml-3.9.1/comet_ml/cpu_logging.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/env_logging.py` & `comet_ml-3.9.1/comet_ml/env_logging.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/exceptions.py` & `comet_ml-3.9.1/comet_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/experiment.py` & `comet_ml-3.9.1/comet_ml/experiment.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/feature_toggles.py` & `comet_ml-3.9.1/comet_ml/feature_toggles.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/file_uploader.py` & `comet_ml-3.9.1/comet_ml/file_uploader.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/git_logging.py` & `comet_ml-3.9.1/comet_ml/git_logging.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/gpu_logging.py` & `comet_ml-3.9.1/comet_ml/gpu_logging.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/json_encoder.py` & `comet_ml-3.9.1/comet_ml/json_encoder.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/__init__.py` & `comet_ml-3.9.1/comet_ml/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/fastai_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/fastai_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/keras_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/keras_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/lightgbm_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/lightgbm_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/logger_utils.py` & `comet_ml-3.9.1/comet_ml/loggers/logger_utils.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/mlflow_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/prophet_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/prophet_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/pytorch_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/pytorch_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/shap_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/shap_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/sklearn_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/sklearn_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,22 @@
 
 
 def _log_estimator_params(experiment, estimator):
     if experiment.auto_param_logging:
         try:
             params = estimator.get_params()
             processed_params = pre_process_params(params)
+            if len(processed_params) == 0:
+                LOGGER.debug(
+                    "Skipping empty params %r from Estimator %r",
+                    processed_params,
+                    estimator,
+                )
+                return
+
             experiment._log_parameters(processed_params, framework="sklearn")
         except Exception:
             LOGGER.error("Failed to extract parameters from estimator", exc_info=True)
 
 
 def fit_logger_before(experiment, original, *args, **kwargs):
     _log_estimator_params(experiment, args[0])
```

### Comparing `comet_ml-3.9.0/comet_ml/loggers/tensorboard_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/tensorflow_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/tensorflow_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/tfma_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/tfma_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/loggers/xgboost_logger.py` & `comet_ml-3.9.1/comet_ml/loggers/xgboost_logger.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/logging_messages.py` & `comet_ml-3.9.1/comet_ml/logging_messages.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/messages.py` & `comet_ml-3.9.1/comet_ml/messages.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/metrics.py` & `comet_ml-3.9.1/comet_ml/metrics.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/monkey_patching.py` & `comet_ml-3.9.1/comet_ml/monkey_patching.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/offline.py` & `comet_ml-3.9.1/comet_ml/offline.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/optimizer.py` & `comet_ml-3.9.1/comet_ml/optimizer.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/papi.py` & `comet_ml-3.9.1/comet_ml/papi.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/predictor.py` & `comet_ml-3.9.1/comet_ml/predictor.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/query.py` & `comet_ml-3.9.1/comet_ml/query.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/rpc.py` & `comet_ml-3.9.1/comet_ml/rpc.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/3d-points-bounding-box.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/3d-points-bounding-box.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-cloud-details-msg.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-cloud-details-msg.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-experiment.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-experiment.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-file-upload-msg.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-file-upload-msg.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-graph-msg.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-graph-msg.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-os-packages-msg.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-os-packages-msg.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-remote-file-msg.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-remote-file-msg.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-system-details-msg.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-system-details-msg.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas/offline-ws-msg.schema.json` & `comet_ml-3.9.1/comet_ml/schemas/offline-ws-msg.schema.json`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/schemas.py` & `comet_ml-3.9.1/comet_ml/schemas.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet.py` & `comet_ml-3.9.1/comet_ml/scripts/comet.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet_check.py` & `comet_ml-3.9.1/comet_ml/scripts/comet_check.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet_init.py` & `comet_ml-3.9.1/comet_ml/scripts/comet_init.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet_models.py` & `comet_ml-3.9.1/comet_ml/scripts/comet_models.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet_offline.py` & `comet_ml-3.9.1/comet_ml/scripts/comet_offline.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet_optimize.py` & `comet_ml-3.9.1/comet_ml/scripts/comet_optimize.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet_python.py` & `comet_ml-3.9.1/comet_ml/scripts/comet_python.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/scripts/comet_upload.py` & `comet_ml-3.9.1/comet_ml/scripts/comet_upload.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/summary.py` & `comet_ml-3.9.1/comet_ml/summary.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/tf_utils.py` & `comet_ml-3.9.1/comet_ml/tf_utils.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml/utils.py` & `comet_ml-3.9.1/comet_ml/utils.py`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/comet_ml.egg-info/PKG-INFO` & `comet_ml-3.9.1/comet_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet-ml
-Version: 3.9.0
+Version: 3.9.1
 Summary: Supercharging Machine Learning
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Description: Comet.ml
         ========
```

### Comparing `comet_ml-3.9.0/comet_ml.egg-info/SOURCES.txt` & `comet_ml-3.9.1/comet_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comet_ml-3.9.0/setup.py` & `comet_ml-3.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,9 +54,9 @@
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
     ],
     license="Proprietary",
-    version="3.9.0",
+    version="3.9.1",
 )
```


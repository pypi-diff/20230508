# Comparing `tmp/pycyclops-0.1.8.tar.gz` & `tmp/pycyclops-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycyclops-0.1.8.tar", max compression
+gzip compressed data, was "pycyclops-0.1.9.tar", max compression
```

## Comparing `pycyclops-0.1.8.tar` & `pycyclops-0.1.9.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0    11347 2022-12-20 03:42:46.813213 pycyclops-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     3327 2022-12-20 03:42:46.813213 pycyclops-0.1.8/README.md
--rw-r--r--   0        0        0       23 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/__init__.py
--rw-r--r--   0        0        0      137 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/constants.py
--rw-r--r--   0        0        0       24 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/__init__.py
--rw-r--r--   0        0        0     4445 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/evaluator.py
--rw-r--r--   0        0        0     1705 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0    12908 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0    13038 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/auroc.py
--rw-r--r--   0        0        0    25489 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/f_beta.py
--rw-r--r--   0        0        0     1807 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/__init__.py
--rw-r--r--   0        0        0    16392 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/accuracy.py
--rw-r--r--   0        0        0    21145 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/auroc.py
--rw-r--r--   0        0        0    26490 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/f_beta.py
--rw-r--r--   0        0        0    26727 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/precision_recall.py
--rw-r--r--   0        0        0    35075 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    21963 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/roc.py
--rw-r--r--   0        0        0    10826 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/sensitivity.py
--rw-r--r--   0        0        0    15501 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/specificity.py
--rw-r--r--   0        0        0    25015 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/functional/stat_scores.py
--rw-r--r--   0        0        0    17862 2022-12-20 03:42:46.817214 pycyclops-0.1.8/cyclops/evaluate/metrics/metric.py
--rw-r--r--   0        0        0    26390 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/evaluate/metrics/precision_recall.py
--rw-r--r--   0        0        0    17462 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/evaluate/metrics/precision_recall_curve.py
--rw-r--r--   0        0        0    12921 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/evaluate/metrics/roc.py
--rw-r--r--   0        0        0    12191 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/evaluate/metrics/sensitivity.py
--rw-r--r--   0        0        0    13627 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/evaluate/metrics/specificity.py
--rw-r--r--   0        0        0    16677 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/evaluate/metrics/stat_scores.py
--rw-r--r--   0        0        0     9851 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/evaluate/metrics/utils.py
--rw-r--r--   0        0        0      669 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/__init__.py
--rw-r--r--   0        0        0     4882 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/catalog.py
--rw-r--r--   0        0        0      590 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/gru.yaml
--rw-r--r--   0        0        0      119 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/logistic_regression.yaml
--rw-r--r--   0        0        0      590 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/lstm.yaml
--rw-r--r--   0        0        0      238 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/mlp.yaml
--rw-r--r--   0        0        0      577 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/mlp_pt.yaml
--rw-r--r--   0        0        0      123 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/random_forest.yaml
--rw-r--r--   0        0        0      590 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/rnn.yaml
--rw-r--r--   0        0        0      288 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/configs/xgb_classifier.yaml
--rw-r--r--   0        0        0      514 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/constants.py
--rw-r--r--   0        0        0     9504 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/data.py
--rw-r--r--   0        0        0      265 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/neural_nets/__init__.py
--rw-r--r--   0        0        0     1972 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/neural_nets/gru.py
--rw-r--r--   0        0        0     2182 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/neural_nets/lstm.py
--rw-r--r--   0        0        0     2824 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/neural_nets/mlp.py
--rw-r--r--   0        0        0     1960 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/neural_nets/rnn.py
--rw-r--r--   0        0        0     6056 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/plotter.py
--rw-r--r--   0        0        0     6049 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/predictor.py
--rw-r--r--   0        0        0     9170 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/utils.py
--rw-r--r--   0        0        0      206 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/wrappers/__init__.py
--rw-r--r--   0        0        0     4414 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/wrappers/base.py
--rw-r--r--   0        0        0    31788 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/wrappers/pt_model.py
--rw-r--r--   0        0        0     7252 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/wrappers/sk_model.py
--rw-r--r--   0        0        0     7590 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/models/wrappers/utils.py
--rw-r--r--   0        0        0      387 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/__init__.py
--rw-r--r--   0        0        0     6049 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/clinical_applicator.py
--rw-r--r--   0        0        0      652 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/configs/gemini/hospital_type_academic.yaml
--rw-r--r--   0        0        0      665 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/baseline.yaml
--rw-r--r--   0        0        0      805 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_gender_F.yaml
--rw-r--r--   0        0        0      804 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_gender_M.yaml
--rw-r--r--   0        0        0      807 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_targets_Mass.yaml
--rw-r--r--   0        0        0      803 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_targets_age_70-100.yaml
--rw-r--r--   0        0        0      531 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/synthetic_gaussian.yaml
--rw-r--r--   0        0        0      467 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/dataframe_mapping.py
--rw-r--r--   0        0        0      104 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/datasets/__init__.py
--rw-r--r--   0        0        0      595 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/datasets/configs/gemini.yaml
--rw-r--r--   0        0        0      615 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/datasets/configs/nihcxr.yaml
--rw-r--r--   0        0        0     3338 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/datasets/gemini.py
--rw-r--r--   0        0        0     2290 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/datasets/nihcxr.py
--rw-r--r--   0        0        0     3074 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/datasets/utils.py
--rw-r--r--   0        0        0     5548 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/detector.py
--rw-r--r--   0        0        0     4159 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/experimenter.py
--rw-r--r--   0        0        0     2184 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/explainer.py
--rw-r--r--   0        0        0       84 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/gemini/__init__.py
--rw-r--r--   0        0        0     1911 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/gemini/mortality/constants.py
--rw-r--r--   0        0        0     8475 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/gemini/query.py
--rw-r--r--   0        0        0    13489 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/gemini/utils.py
--rw-r--r--   0        0        0     6230 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/optimizer.py
--rw-r--r--   0        0        0    10272 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/plotter.py
--rw-r--r--   0        0        0    19148 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/reductor.py
--rw-r--r--   0        0        0    20126 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/retrainers.py
--rw-r--r--   0        0        0     8026 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/rolling_window.py
--rw-r--r--   0        0        0     2056 2022-12-20 03:42:46.821214 pycyclops-0.1.8/cyclops/monitor/run_drift_detection.py
--rw-r--r--   0        0        0    17934 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/monitor/synthetic_applicator.py
--rw-r--r--   0        0        0     6345 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/monitor/tester.py
--rw-r--r--   0        0        0    19907 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/monitor/utils.py
--rw-r--r--   0        0        0     6313 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/plotter.py
--rw-r--r--   0        0        0       26 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/__init__.py
--rw-r--r--   0        0        0    25180 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/aggregate.py
--rw-r--r--   0        0        0     8731 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/clean.py
--rw-r--r--   0        0        0     1817 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/column_names.py
--rw-r--r--   0        0        0     4897 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/constants.py
--rw-r--r--   0        0        0     3242 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/diagnoses.py
--rw-r--r--   0        0        0       39 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/feature/__init__.py
--rw-r--r--   0        0        0    28569 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/feature/feature.py
--rw-r--r--   0        0        0    26405 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/feature/handle_types.py
--rw-r--r--   0        0        0    16914 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/feature/normalize.py
--rw-r--r--   0        0        0    11191 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/feature/split.py
--rw-r--r--   0        0        0    29694 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/feature/vectorized.py
--rw-r--r--   0        0        0    17475 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/impute.py
--rw-r--r--   0        0        0     6494 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/string_ops.py
--rw-r--r--   0        0        0     6604 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/process/util.py
--rw-r--r--   0        0        0       23 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/__init__.py
--rw-r--r--   0        0        0     3689 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/base.py
--rw-r--r--   0        0        0      105 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/configs/config.yaml
--rw-r--r--   0        0        0    27970 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/gemini.py
--rw-r--r--   0        0        0     7259 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/interface.py
--rw-r--r--   0        0        0    18212 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/mimiciv.py
--rw-r--r--   0        0        0    16281 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/omop.py
--rw-r--r--   0        0        0    12825 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/orm.py
--rw-r--r--   0        0        0       49 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/postprocess/__init__.py
--rw-r--r--   0        0        0     1261 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/postprocess/gemini.py
--rw-r--r--   0        0        0     4667 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/postprocess/mimiciv.py
--rw-r--r--   0        0        0     5982 2022-12-20 03:42:46.825214 pycyclops-0.1.8/cyclops/query/postprocess/util.py
--rw-r--r--   0        0        0    54697 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/query/process.py
--rw-r--r--   0        0        0    29504 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/query/util.py
--rw-r--r--   0        0        0       23 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/utils/__init__.py
--rw-r--r--   0        0        0    10531 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/utils/common.py
--rw-r--r--   0        0        0    11948 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/utils/file.py
--rw-r--r--   0        0        0     2314 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/utils/indexing.py
--rw-r--r--   0        0        0     3488 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/utils/log.py
--rw-r--r--   0        0        0      802 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/utils/profile.py
--rw-r--r--   0        0        0       32 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/workflow/__init__.py
--rw-r--r--   0        0        0       96 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/workflow/constants.py
--rw-r--r--   0        0        0     3249 2022-12-20 03:42:46.829214 pycyclops-0.1.8/cyclops/workflow/task.py
--rw-r--r--   0        0        0     3065 2022-12-20 03:42:46.841215 pycyclops-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 pycyclops-0.1.8/setup.py
--rw-r--r--   0        0        0     4966 1970-01-01 00:00:00.000000 pycyclops-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-12-20 19:44:04.365901 pycyclops-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     3322 2022-12-20 19:44:04.365901 pycyclops-0.1.9/README.md
+-rw-r--r--   0        0        0       23 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/__init__.py
+-rw-r--r--   0        0        0      137 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/constants.py
+-rw-r--r--   0        0        0       24 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/__init__.py
+-rw-r--r--   0        0        0     4445 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/evaluator.py
+-rw-r--r--   0        0        0     1705 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0    12908 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0    13038 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/auroc.py
+-rw-r--r--   0        0        0    25489 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/f_beta.py
+-rw-r--r--   0        0        0     1807 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/__init__.py
+-rw-r--r--   0        0        0    16392 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/accuracy.py
+-rw-r--r--   0        0        0    21145 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/auroc.py
+-rw-r--r--   0        0        0    26490 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/f_beta.py
+-rw-r--r--   0        0        0    26727 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/precision_recall.py
+-rw-r--r--   0        0        0    35075 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    21963 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/roc.py
+-rw-r--r--   0        0        0    10826 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/sensitivity.py
+-rw-r--r--   0        0        0    15501 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/specificity.py
+-rw-r--r--   0        0        0    25015 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/functional/stat_scores.py
+-rw-r--r--   0        0        0    17862 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/metric.py
+-rw-r--r--   0        0        0    26390 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/precision_recall.py
+-rw-r--r--   0        0        0    17462 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/precision_recall_curve.py
+-rw-r--r--   0        0        0    12921 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/roc.py
+-rw-r--r--   0        0        0    12191 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/sensitivity.py
+-rw-r--r--   0        0        0    13627 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/specificity.py
+-rw-r--r--   0        0        0    16677 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/stat_scores.py
+-rw-r--r--   0        0        0     9851 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/evaluate/metrics/utils.py
+-rw-r--r--   0        0        0      669 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/__init__.py
+-rw-r--r--   0        0        0     4888 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/catalog.py
+-rw-r--r--   0        0        0      590 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/gru.yaml
+-rw-r--r--   0        0        0      119 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/logistic_regression.yaml
+-rw-r--r--   0        0        0      590 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/lstm.yaml
+-rw-r--r--   0        0        0      238 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/mlp.yaml
+-rw-r--r--   0        0        0      577 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/mlp_pt.yaml
+-rw-r--r--   0        0        0      123 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/random_forest.yaml
+-rw-r--r--   0        0        0      590 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/rnn.yaml
+-rw-r--r--   0        0        0      288 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/configs/xgb_classifier.yaml
+-rw-r--r--   0        0        0      514 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/constants.py
+-rw-r--r--   0        0        0     9504 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/data.py
+-rw-r--r--   0        0        0      265 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/neural_nets/__init__.py
+-rw-r--r--   0        0        0     1972 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/neural_nets/gru.py
+-rw-r--r--   0        0        0     2182 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/neural_nets/lstm.py
+-rw-r--r--   0        0        0     2824 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/neural_nets/mlp.py
+-rw-r--r--   0        0        0     1960 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/neural_nets/rnn.py
+-rw-r--r--   0        0        0     6056 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/plotter.py
+-rw-r--r--   0        0        0     6049 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/predictor.py
+-rw-r--r--   0        0        0     9170 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/utils.py
+-rw-r--r--   0        0        0      206 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/wrappers/__init__.py
+-rw-r--r--   0        0        0     4414 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/wrappers/base.py
+-rw-r--r--   0        0        0    31788 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/wrappers/pt_model.py
+-rw-r--r--   0        0        0     7252 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/wrappers/sk_model.py
+-rw-r--r--   0        0        0     7590 2022-12-20 19:44:04.369901 pycyclops-0.1.9/cyclops/models/wrappers/utils.py
+-rw-r--r--   0        0        0      387 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/__init__.py
+-rw-r--r--   0        0        0     6049 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/clinical_applicator.py
+-rw-r--r--   0        0        0      652 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/configs/gemini/hospital_type_academic.yaml
+-rw-r--r--   0        0        0      665 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/baseline.yaml
+-rw-r--r--   0        0        0      805 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_gender_F.yaml
+-rw-r--r--   0        0        0      804 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_gender_M.yaml
+-rw-r--r--   0        0        0      807 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_targets_Mass.yaml
+-rw-r--r--   0        0        0      803 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_targets_age_70-100.yaml
+-rw-r--r--   0        0        0      531 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/synthetic_gaussian.yaml
+-rw-r--r--   0        0        0      467 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/dataframe_mapping.py
+-rw-r--r--   0        0        0      104 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/datasets/__init__.py
+-rw-r--r--   0        0        0      595 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/datasets/configs/gemini.yaml
+-rw-r--r--   0        0        0      615 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/datasets/configs/nihcxr.yaml
+-rw-r--r--   0        0        0     3338 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/datasets/gemini.py
+-rw-r--r--   0        0        0     2290 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/datasets/nihcxr.py
+-rw-r--r--   0        0        0     3074 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/datasets/utils.py
+-rw-r--r--   0        0        0     5548 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/detector.py
+-rw-r--r--   0        0        0     4159 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/experimenter.py
+-rw-r--r--   0        0        0     2184 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/explainer.py
+-rw-r--r--   0        0        0       84 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/gemini/__init__.py
+-rw-r--r--   0        0        0     1911 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/gemini/mortality/constants.py
+-rw-r--r--   0        0        0     8475 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/gemini/query.py
+-rw-r--r--   0        0        0    13489 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/gemini/utils.py
+-rw-r--r--   0        0        0     6230 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/optimizer.py
+-rw-r--r--   0        0        0    10272 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/plotter.py
+-rw-r--r--   0        0        0    19148 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/reductor.py
+-rw-r--r--   0        0        0    20126 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/retrainers.py
+-rw-r--r--   0        0        0     8026 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/rolling_window.py
+-rw-r--r--   0        0        0     2056 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/run_drift_detection.py
+-rw-r--r--   0        0        0    17934 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/synthetic_applicator.py
+-rw-r--r--   0        0        0     6345 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/tester.py
+-rw-r--r--   0        0        0    19907 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/monitor/utils.py
+-rw-r--r--   0        0        0     6313 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/plotter.py
+-rw-r--r--   0        0        0       26 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/__init__.py
+-rw-r--r--   0        0        0    25180 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/aggregate.py
+-rw-r--r--   0        0        0     8731 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/clean.py
+-rw-r--r--   0        0        0     1817 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/column_names.py
+-rw-r--r--   0        0        0     4897 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/constants.py
+-rw-r--r--   0        0        0     3242 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/diagnoses.py
+-rw-r--r--   0        0        0       39 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/feature/__init__.py
+-rw-r--r--   0        0        0    28569 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/feature/feature.py
+-rw-r--r--   0        0        0    26405 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/feature/handle_types.py
+-rw-r--r--   0        0        0    16914 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/feature/normalize.py
+-rw-r--r--   0        0        0    11191 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/feature/split.py
+-rw-r--r--   0        0        0    29694 2022-12-20 19:44:04.373901 pycyclops-0.1.9/cyclops/process/feature/vectorized.py
+-rw-r--r--   0        0        0    17475 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/process/impute.py
+-rw-r--r--   0        0        0     6494 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/process/string_ops.py
+-rw-r--r--   0        0        0     6604 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/process/util.py
+-rw-r--r--   0        0        0       23 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/__init__.py
+-rw-r--r--   0        0        0     3733 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/base.py
+-rw-r--r--   0        0        0      105 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/configs/config.yaml
+-rw-r--r--   0        0        0    27969 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/gemini.py
+-rw-r--r--   0        0        0     7259 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/interface.py
+-rw-r--r--   0        0        0    18224 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/mimiciv.py
+-rw-r--r--   0        0        0    16342 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/omop.py
+-rw-r--r--   0        0        0    12825 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/orm.py
+-rw-r--r--   0        0        0       49 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/postprocess/__init__.py
+-rw-r--r--   0        0        0     1261 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/postprocess/gemini.py
+-rw-r--r--   0        0        0     4667 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/postprocess/mimiciv.py
+-rw-r--r--   0        0        0     5982 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/postprocess/util.py
+-rw-r--r--   0        0        0    53742 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/process.py
+-rw-r--r--   0        0        0    30565 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/query/util.py
+-rw-r--r--   0        0        0       23 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/utils/__init__.py
+-rw-r--r--   0        0        0    10531 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/utils/common.py
+-rw-r--r--   0        0        0    11948 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/utils/file.py
+-rw-r--r--   0        0        0     2314 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/utils/indexing.py
+-rw-r--r--   0        0        0     3488 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/utils/log.py
+-rw-r--r--   0        0        0      802 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/utils/profile.py
+-rw-r--r--   0        0        0       32 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/workflow/__init__.py
+-rw-r--r--   0        0        0       96 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/workflow/constants.py
+-rw-r--r--   0        0        0     3249 2022-12-20 19:44:04.377901 pycyclops-0.1.9/cyclops/workflow/task.py
+-rw-r--r--   0        0        0     3065 2022-12-20 19:44:04.389901 pycyclops-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5270 1970-01-01 00:00:00.000000 pycyclops-0.1.9/setup.py
+-rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 pycyclops-0.1.9/PKG-INFO
```

### Comparing `pycyclops-0.1.8/LICENSE.md` & `pycyclops-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/README.md` & `pycyclops-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 use cases include:
 
 * Mortality decompensation prediction
 
 
 ## 🐣 Getting Started
 
-### Installing the core cyclops package using pip
+### Installing the cyclops package using pip
 
 ```bash
 python3 -m pip install pycyclops
 ```
 
 ## 🧑🏿‍💻 Developing
```

### Comparing `pycyclops-0.1.8/cyclops/evaluate/evaluator.py` & `pycyclops-0.1.9/cyclops/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/__init__.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/accuracy.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/auroc.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/f_beta.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/__init__.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/accuracy.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/auroc.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/f_beta.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/precision_recall.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/precision_recall_curve.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/roc.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/sensitivity.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/specificity.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/functional/stat_scores.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/functional/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/metric.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/precision_recall.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/precision_recall_curve.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/roc.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/sensitivity.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/specificity.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/stat_scores.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/evaluate/metrics/utils.py` & `pycyclops-0.1.9/cyclops/evaluate/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/__init__.py` & `pycyclops-0.1.9/cyclops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/catalog.py` & `pycyclops-0.1.9/cyclops/models/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Model catalog."""
+
 import logging
 from difflib import get_close_matches
-from typing import Any, Callable, Dict, List, Literal, Union
+from typing import Any, Callable, Dict, List, Literal, Set, Union
 
 import torch.nn.modules
 import torch.optim
 from sklearn.base import BaseEstimator
 
 from cyclops.models.utils import is_pytorch_model, is_sklearn_model
 from cyclops.models.wrappers import PTModel, SKModel, WrappedModel
@@ -14,18 +15,18 @@
 LOGGER = logging.getLogger(__name__)
 setup_logging(print_level="WARN", logger=LOGGER)
 
 ####################
 # Model catalogs   #
 ####################
 _model_catalog: Dict[str, Any] = {}
-_temporal_model_keys: set[str] = set()
-_static_model_keys: set[str] = set()
-_pt_model_keys: set[str] = set()
-_sk_model_keys: set[str] = set()
+_temporal_model_keys: Set[str] = set()
+_static_model_keys: Set[str] = set()
+_pt_model_keys: Set[str] = set()
+_sk_model_keys: Set[str] = set()
 
 
 def register_model(name: str, model_type: Literal["static", "temporal"]) -> Callable:
     """Register model in the catalog.
 
     Parameters
     ----------
@@ -77,15 +78,15 @@
         return model_obj
 
     return decorator
 
 
 def list_models(
     category: Literal["static", "temporal", "pytorch", "sklearn"] = None
-) -> list[str]:
+) -> List[str]:
     """List models.
 
     Parameters
     ----------
     category : "static", "temporal", "pytorch", "sklearn", optional
         The type of model to list. If None, all models are listed.
```

### Comparing `pycyclops-0.1.8/cyclops/models/configs/gru.yaml` & `pycyclops-0.1.9/cyclops/models/configs/gru.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/configs/lstm.yaml` & `pycyclops-0.1.9/cyclops/models/configs/lstm.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/configs/mlp_pt.yaml` & `pycyclops-0.1.9/cyclops/models/configs/mlp_pt.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/configs/rnn.yaml` & `pycyclops-0.1.9/cyclops/models/configs/rnn.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/constants.py` & `pycyclops-0.1.9/cyclops/models/constants.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/data.py` & `pycyclops-0.1.9/cyclops/models/data.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/neural_nets/gru.py` & `pycyclops-0.1.9/cyclops/models/neural_nets/gru.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/neural_nets/lstm.py` & `pycyclops-0.1.9/cyclops/models/neural_nets/lstm.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/neural_nets/mlp.py` & `pycyclops-0.1.9/cyclops/models/neural_nets/mlp.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/neural_nets/rnn.py` & `pycyclops-0.1.9/cyclops/models/neural_nets/rnn.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/plotter.py` & `pycyclops-0.1.9/cyclops/models/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/predictor.py` & `pycyclops-0.1.9/cyclops/models/predictor.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/utils.py` & `pycyclops-0.1.9/cyclops/models/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/wrappers/base.py` & `pycyclops-0.1.9/cyclops/models/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/wrappers/pt_model.py` & `pycyclops-0.1.9/cyclops/models/wrappers/pt_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/wrappers/sk_model.py` & `pycyclops-0.1.9/cyclops/models/wrappers/sk_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/models/wrappers/utils.py` & `pycyclops-0.1.9/cyclops/models/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/clinical_applicator.py` & `pycyclops-0.1.9/cyclops/monitor/clinical_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/configs/gemini/hospital_type_academic.yaml` & `pycyclops-0.1.9/cyclops/monitor/configs/gemini/hospital_type_academic.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/baseline.yaml` & `pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/baseline.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_gender_F.yaml` & `pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_gender_F.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_gender_M.yaml` & `pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_gender_M.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_targets_Mass.yaml` & `pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_targets_Mass.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/categorical_targets_age_70-100.yaml` & `pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/categorical_targets_age_70-100.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/configs/nihcxr/synthetic_gaussian.yaml` & `pycyclops-0.1.9/cyclops/monitor/configs/nihcxr/synthetic_gaussian.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/datasets/configs/gemini.yaml` & `pycyclops-0.1.9/cyclops/monitor/datasets/configs/gemini.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/datasets/configs/nihcxr.yaml` & `pycyclops-0.1.9/cyclops/monitor/datasets/configs/nihcxr.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/datasets/gemini.py` & `pycyclops-0.1.9/cyclops/monitor/datasets/gemini.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/datasets/nihcxr.py` & `pycyclops-0.1.9/cyclops/monitor/datasets/nihcxr.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/datasets/utils.py` & `pycyclops-0.1.9/cyclops/monitor/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/detector.py` & `pycyclops-0.1.9/cyclops/monitor/detector.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/experimenter.py` & `pycyclops-0.1.9/cyclops/monitor/experimenter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/explainer.py` & `pycyclops-0.1.9/cyclops/monitor/explainer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/gemini/mortality/constants.py` & `pycyclops-0.1.9/cyclops/monitor/gemini/mortality/constants.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/gemini/query.py` & `pycyclops-0.1.9/cyclops/monitor/gemini/query.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/gemini/utils.py` & `pycyclops-0.1.9/cyclops/monitor/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/optimizer.py` & `pycyclops-0.1.9/cyclops/monitor/optimizer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/plotter.py` & `pycyclops-0.1.9/cyclops/monitor/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/reductor.py` & `pycyclops-0.1.9/cyclops/monitor/reductor.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/retrainers.py` & `pycyclops-0.1.9/cyclops/monitor/retrainers.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/rolling_window.py` & `pycyclops-0.1.9/cyclops/monitor/rolling_window.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/run_drift_detection.py` & `pycyclops-0.1.9/cyclops/monitor/run_drift_detection.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/synthetic_applicator.py` & `pycyclops-0.1.9/cyclops/monitor/synthetic_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/tester.py` & `pycyclops-0.1.9/cyclops/monitor/tester.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/monitor/utils.py` & `pycyclops-0.1.9/cyclops/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/plotter.py` & `pycyclops-0.1.9/cyclops/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/aggregate.py` & `pycyclops-0.1.9/cyclops/process/aggregate.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/clean.py` & `pycyclops-0.1.9/cyclops/process/clean.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/column_names.py` & `pycyclops-0.1.9/cyclops/process/column_names.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/constants.py` & `pycyclops-0.1.9/cyclops/process/constants.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/diagnoses.py` & `pycyclops-0.1.9/cyclops/process/diagnoses.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/feature/feature.py` & `pycyclops-0.1.9/cyclops/process/feature/feature.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/feature/handle_types.py` & `pycyclops-0.1.9/cyclops/process/feature/handle_types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/feature/normalize.py` & `pycyclops-0.1.9/cyclops/process/feature/normalize.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/feature/split.py` & `pycyclops-0.1.9/cyclops/process/feature/split.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/feature/vectorized.py` & `pycyclops-0.1.9/cyclops/process/feature/vectorized.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/impute.py` & `pycyclops-0.1.9/cyclops/process/impute.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/string_ops.py` & `pycyclops-0.1.9/cyclops/process/string_ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/process/util.py` & `pycyclops-0.1.9/cyclops/process/util.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/query/base.py` & `pycyclops-0.1.9/cyclops/query/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base querier class."""
 
 import logging
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Dict, Optional, Union
 
 from hydra import compose, initialize
 from omegaconf import OmegaConf
 from sqlalchemy.sql.selectable import Subquery
 
 from cyclops.query import process as qp
 from cyclops.query.interface import QueryInterface, QueryInterfaceProcessed
@@ -29,36 +29,36 @@
         A dictionary mapping table names to table objects in the DB.
     _column_map: Dict
         A dictionary mapping column names from the database to map to output
         in a consistent format.
 
     """
 
-    def __init__(
-        self, table_map: Dict, column_map: Dict, config_overrides: Optional[List] = None
-    ) -> None:
+    def __init__(self, table_map: Dict, column_map: Dict, **config_overrides) -> None:
         """Initialize.
 
         Parameters
         ----------
-        config_overrides: list, optional
-            List of override configuration parameters.
         table_map: Dict
             A dictionary mapping table names to table objects in the DB.
         column_map: Dict
             A dictionary mapping column names from the database to map to output
             in a consistent format.
+        **config_overrides
+             Override configuration parameters, specified as kwargs.
 
         """
-        if not config_overrides:
-            config_overrides = []
+        overrides = []
+        if config_overrides:
+            for key, value in config_overrides.items():
+                overrides.append(f"{key}={value}")
         with initialize(
             version_base=None, config_path="configs", job_name="DatasetQuerier"
         ):
-            config = compose(config_name="config", overrides=config_overrides)
+            config = compose(config_name="config", overrides=overrides)
             LOGGER.debug(OmegaConf.to_yaml(config))
 
         self._db = Database(config)
         self._table_map = table_map
         self._column_map = column_map
 
     @table_params_to_type(Subquery)
```

### Comparing `pycyclops-0.1.8/cyclops/query/gemini.py` & `pycyclops-0.1.9/cyclops/query/gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,26 +107,27 @@
 }
 EVENT_CATEGORIES = [LAB, VITALS]
 
 
 class GEMINIQuerier(DatasetQuerier):
     """GEMINI dataset querier."""
 
-    def __init__(self, config_overrides: Optional[List] = None):
+    def __init__(self, **config_overrides):
         """Initialize.
 
         Parameters
         ----------
-        config_overrides: list, optional
-            List of override configuration parameters.
+        **config_overrides
+            Override configuration parameters, specified as kwargs.
 
         """
-        if not config_overrides:
-            config_overrides = []
-        super().__init__(TABLE_MAP, COLUMN_MAP, config_overrides)
+        overrides = {}
+        if config_overrides:
+            overrides = config_overrides
+        super().__init__(TABLE_MAP, COLUMN_MAP, **overrides)
 
     def er_admin(self, **process_kwargs) -> QueryInterface:
         """Query emergency room administrative data.
 
         Returns
         -------
         cyclops.query.interface.QueryInterface
```

### Comparing `pycyclops-0.1.8/cyclops/query/interface.py` & `pycyclops-0.1.9/cyclops/query/interface.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/query/mimiciv.py` & `pycyclops-0.1.9/cyclops/query/mimiciv.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 from cyclops.query import process as qp
 from cyclops.query.base import DatasetQuerier
 from cyclops.query.interface import QueryInterface, QueryInterfaceProcessed
 from cyclops.query.postprocess.mimiciv import process_mimic_care_units
 from cyclops.query.util import (
     TableTypes,
     assert_table_has_columns,
+    ckwarg,
     get_column,
+    remove_kwargs,
     table_params_to_type,
 )
 from cyclops.utils.log import setup_logging
 
 # Logging.
 LOGGER = logging.getLogger(__name__)
 setup_logging(print_level="INFO", logger=LOGGER)
@@ -81,26 +83,27 @@
     "dod": DATE_OF_DEATH,
 }
 
 
 class MIMICIVQuerier(DatasetQuerier):
     """MIMICIV dataset querier."""
 
-    def __init__(self, config_overrides: Optional[List] = None):
+    def __init__(self, **config_overrides):
         """Initialize.
 
         Parameters
         ----------
-        config_overrides: list, optional
-            List of override configuration parameters.
+        **config_overrides
+            Override configuration parameters, specified as kwargs.
 
         """
-        if not config_overrides:
-            config_overrides = []
-        super().__init__(TABLE_MAP, COLUMN_MAP, config_overrides)
+        overrides = {}
+        if config_overrides:
+            overrides = config_overrides
+        super().__init__(TABLE_MAP, COLUMN_MAP, **overrides)
 
     def patients(self, **process_kwargs) -> QueryInterface:
         """Query MIMIC patient data.
 
         Other Parameters
         ----------------
         sex: str or list of string, optional
@@ -281,19 +284,19 @@
 
         # If provided, join with a patients table
         if patients_table is not None:
             table = qp.Join(patients_table, on=SUBJECT_ID)(table)
 
         # Get diagnosis codes.
         diagnoses_table = self.diagnoses(
-            diagnosis_versions=qp.ckwarg(process_kwargs, "diagnosis_versions"),
-            diagnosis_substring=qp.ckwarg(process_kwargs, "diagnosis_substring"),
-            diagnosis_codes=qp.ckwarg(process_kwargs, "diagnosis_codes"),
+            diagnosis_versions=ckwarg(process_kwargs, "diagnosis_versions"),
+            diagnosis_substring=ckwarg(process_kwargs, "diagnosis_substring"),
+            diagnosis_codes=ckwarg(process_kwargs, "diagnosis_codes"),
         ).query
-        process_kwargs = qp.remove_kwargs(
+        process_kwargs = remove_kwargs(
             process_kwargs,
             ["diagnosis_versions", "diagnosis_substring", "diagnosis_codes"],
         )
 
         # Include DIAGNOSIS_TITLE in patient diagnoses.
         table = qp.Join(
             diagnoses_table,
@@ -368,18 +371,18 @@
         ----------------
         encounters : int or list of int, optional
             Get the specific encounter IDs.
 
         """
         table = self.transfers(
             patients_table=patients_table,
-            encounters=qp.ckwarg(process_kwargs, "encounters"),
+            encounters=ckwarg(process_kwargs, "encounters"),
         ).query
 
-        process_kwargs = qp.remove_kwargs(process_kwargs, "encounters")
+        process_kwargs = remove_kwargs(process_kwargs, "encounters")
 
         return QueryInterfaceProcessed(
             self._db,
             table,
             process_fn=lambda x: process_mimic_care_units(x, specific=False),
         )
```

### Comparing `pycyclops-0.1.8/cyclops/query/omop.py` & `pycyclops-0.1.9/cyclops/query/omop.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,27 +92,30 @@
 
 class OMOPQuerier(DatasetQuerier):
     """OMOP querier."""
 
     def __init__(
         self,
         schema_name: str,
-        config_overrides: Optional[List] = None,
+        **config_overrides,
     ):
         """Initialize.
 
         Parameters
         ----------
-        config_overrides: list, optional
-            List of override configuration parameters.
+        schema_name: str
+            Name of database schema.
+        **config_overrides
+            Override configuration parameters, specified as kwargs.
 
         """
-        if not config_overrides:
-            config_overrides = []
-        super().__init__(_get_table_map(schema_name), COLUMN_MAP, config_overrides)
+        overrides = {}
+        if config_overrides:
+            overrides = config_overrides
+        super().__init__(_get_table_map(schema_name), COLUMN_MAP, **overrides)
 
     def _map_concept_ids_to_name(
         self, source_table: Subquery, source_cols: Union[str, List[str]]
     ) -> Subquery:
         """Map concept IDs in a source table to concept names from concept table.
 
         Parameters
```

### Comparing `pycyclops-0.1.8/cyclops/query/orm.py` & `pycyclops-0.1.9/cyclops/query/orm.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/query/postprocess/gemini.py` & `pycyclops-0.1.9/cyclops/query/postprocess/gemini.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/query/postprocess/mimiciv.py` & `pycyclops-0.1.9/cyclops/query/postprocess/mimiciv.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/query/postprocess/util.py` & `pycyclops-0.1.9/cyclops/query/postprocess/util.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/query/process.py` & `pycyclops-0.1.9/cyclops/query/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,57 +98,14 @@
         val = kwargs[self.kwarg_name]
         if self.transform_fn is not None:
             return self.transform_fn(val)
 
         return val
 
 
-def ckwarg(kwargs: dict, kwarg: str):
-    """Get the value of a conditional keyword argument.
-
-    A keyword argument may or may not be specified in some
-    keyword arguments. If specified, return the value,
-    otherwise return None.
-
-    Parameters
-    ----------
-    kwargs: dict
-        Process keyword arguments.
-    kwarg: str
-        The keyword argument of interest.
-
-    Returns
-    -------
-    any, optional
-        The value of the keyword argument if it exists, otherwise None.
-
-    """
-    if kwarg in kwargs:
-        return kwargs[kwarg]
-    return None
-
-
-def remove_kwargs(process_kwargs: dict, kwargs: Union[str, List[str]]):
-    """Remove some keyword arguments from process_kwargs if they exist.
-
-    Parameters
-    ----------
-    process_kwargs: dict
-        Process keyword arguments.
-    kwargs: str or list of str
-        The keyword arguments to remove should they exist.
-
-    """
-    kwargs = to_list(kwargs)
-    for kwarg in kwargs:
-        if kwarg in process_kwargs:
-            del process_kwargs[kwarg]
-    return process_kwargs
-
-
 @table_params_to_type(Subquery)
 def process_operations(  # pylint: disable=too-many-locals
     table: TableTypes, operations: List[tuple], user_kwargs: dict
 ) -> Subquery:
     """Query MIMIC encounter-specific patient data.
 
     Parameters
@@ -264,15 +221,15 @@
         args = process_args(args)
         kwargs = process_kwargs(kwargs)
         table = process_func(*args, **kwargs)(table)
 
     return table
 
 
-def append_if_missing(
+def _append_if_missing(
     table: TableTypes,
     keep_cols: Optional[Union[str, List[str]]] = None,
     force_include_cols: Optional[Union[str, List[str]]] = None,
 ):
     """Keep only certain columns in a table, but must include certain columns.
 
     Parameters
@@ -287,18 +244,19 @@
     """
     if keep_cols is None:
         return table
     keep_cols = to_list(keep_cols)
     force_include_cols = to_list(force_include_cols)
     extend_cols = [col for col in force_include_cols if col not in keep_cols]
     keep_cols = extend_cols + keep_cols
+
     return FilterColumns(keep_cols)(table)
 
 
-def none_add(obj1: Any, obj2: Any):
+def _none_add(obj1: Any, obj2: Any):
     """Add two objects together while ignoring None values.
 
     If both objects are None, returns None.
 
     Parameters
     ----------
     obj1: Any
@@ -308,15 +266,15 @@
     if obj1 is None:
         return obj2
     if obj2 is None:
         return obj1
     return obj1 + obj2
 
 
-def process_checks(
+def _process_checks(
     table: TableTypes,
     cols: Optional[Union[str, List[str]]] = None,
     cols_not_in: Optional[Union[str, List[str]]] = None,
     timestamp_cols: Optional[Union[str, List[str]]] = None,
 ) -> Subquery:
     """Perform checks, and possibly alterations, on a table.
 
@@ -375,15 +333,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.cols)
+        table = _process_checks(table, cols=self.cols)
         return drop_columns(table, self.cols)
 
 
 @dataclass
 class Rename:  # pylint: disable=too-few-public-methods
     """Rename some columns.
 
@@ -411,15 +369,15 @@
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
         if self.check_exists:
-            table = process_checks(table, cols=list(self.rename_map.keys()))
+            table = _process_checks(table, cols=list(self.rename_map.keys()))
         return rename_columns(table, self.rename_map)
 
 
 @dataclass
 class Substring:  # pylint: disable=too-few-public-methods
     """Get substring of a string column.
 
@@ -451,15 +409,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.col)
+        table = _process_checks(table, cols=self.col)
         table = select(
             table,
             func.substr(
                 get_column(table, self.col), self.start_index, self.stop_index
             ).label(self.new_col_label),
         ).subquery()
 
@@ -489,15 +447,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.cols)
+        table = _process_checks(table, cols=self.cols)
         return reorder_columns(table, self.cols)
 
 
 class ReorderAfter:  # pylint: disable=too-few-public-methods
     """Reorder a number of columns to come after a specified column.
 
     cols: list of str
@@ -523,15 +481,15 @@
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
         self.cols = to_list(self.cols)
-        table = process_checks(table, cols=self.cols + [self.after])
+        table = _process_checks(table, cols=self.cols + [self.after])
         names = get_column_names(table)
         names = [name for name in names if name not in self.cols]
         name_after_ind = names.index(self.after) + 1
         new_order = names[:name_after_ind] + self.cols + names[name_after_ind:]
         return Reorder(new_order)(table)
 
 
@@ -558,15 +516,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.cols)
+        table = _process_checks(table, cols=self.cols)
         return filter_columns(table, self.cols)
 
 
 @dataclass
 class Trim:  # pylint: disable=too-few-public-methods
     """Trim the whitespace from some string columns.
 
@@ -593,15 +551,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.cols)
+        table = _process_checks(table, cols=self.cols)
         return trim_columns(table, self.cols, new_col_labels=self.new_col_labels)
 
 
 @dataclass
 class Literal:  # pylint: disable=too-few-public-methods
     """Add a literal column to a table.
 
@@ -627,15 +585,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols_not_in=self.col)
+        table = _process_checks(table, cols_not_in=self.col)
         return select(table, literal(self.value).label(self.col)).subquery()
 
 
 @dataclass
 class ExtractTimestampComponent:  # pylint: disable=too-few-public-methods
     """Extract a component such as year or month from a timestamp column.
 
@@ -664,15 +622,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(
+        table = _process_checks(
             table, timestamp_cols=self.timestamp_col, cols_not_in=self.label
         )
 
         table = select(
             table,
             extract(self.extract_str, get_column(table, self.timestamp_col)).label(
                 self.label
@@ -712,15 +670,17 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.add_to, cols_not_in=self.new_col_labels)
+        table = _process_checks(
+            table, cols=self.add_to, cols_not_in=self.new_col_labels
+        )
         return apply_to_columns(
             table,
             self.add_to,
             lambda x: x + self.num,
             new_col_labels=self.new_col_labels,
         )
 
@@ -755,15 +715,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(
+        table = _process_checks(
             table, timestamp_cols=self.add_to, cols_not_in=self.new_col_labels
         )
 
         return apply_to_columns(
             table,
             self.add_to,
             lambda x: x + self.delta,
@@ -809,19 +769,19 @@
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
         # If the column being added is a timestamp column, ensure the others are too
         if check_timestamp_columns(table, self.col):
-            table = process_checks(
+            table = _process_checks(
                 table, timestamp_cols=self.add_to, cols_not_in=self.new_col_labels
             )
         else:
-            table = process_checks(
+            table = _process_checks(
                 table, cols=self.add_to, cols_not_in=self.new_col_labels
             )
 
         col = get_column(table, self.col)
 
         if self.negative:
             return apply_to_columns(
@@ -881,15 +841,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(
+        table = _process_checks(
             table, timestamp_cols=self.add_to, cols_not_in=self.new_col_labels
         )
 
         delta = get_delta_column(table, **self.delta_kwargs)
 
         if self.negative:
             return apply_to_columns(
@@ -935,15 +895,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.cols)
+        table = _process_checks(table, cols=self.cols)
 
         cast_type_map = {
             "str": "to_str",
             "int": "to_int",
             "float": "to_float",
             "date": "to_date",
             "timestamp": "to_timestamp",
@@ -1046,21 +1006,24 @@
                 col_obj if isinstance(col_obj, str) else col_obj[0]
                 for col_obj in self.on_
             ]
             on_join_table_cols = [
                 col_obj if isinstance(col_obj, str) else col_obj[1]
                 for col_obj in self.on_
             ]
-            table = process_checks(table, cols=none_add(self.table_cols, on_table_cols))
-            self.join_table = process_checks(
-                self.join_table, cols=none_add(self.join_table_cols, on_join_table_cols)
+            table = _process_checks(
+                table, cols=_none_add(self.table_cols, on_table_cols)
+            )
+            self.join_table = _process_checks(
+                self.join_table,
+                cols=_none_add(self.join_table_cols, on_join_table_cols),
             )
             # Filter columns, keeping those being joined on
-            table = append_if_missing(table, self.table_cols, on_table_cols)
-            self.join_table = append_if_missing(
+            table = _append_if_missing(table, self.table_cols, on_table_cols)
+            self.join_table = _append_if_missing(
                 self.join_table, self.join_table_cols, on_join_table_cols
             )
             # Perform type conversions if given
             if self.on_to_type is not None:
                 for i, type_ in enumerate(self.on_to_type):
                     table = Cast(on_table_cols[i], type_)(table)
                     self.join_table = Cast(on_join_table_cols[i], type_)(
@@ -1146,15 +1109,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
+        table = _process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
         cond = equals(get_column(table, self.col), self.value, **self.cond_kwargs)
         if self.not_:
             cond = cond._negate()
 
         if self.binarize_col is not None:
             return select(
                 table, cast(cond, Boolean).label(self.binarize_col)
@@ -1206,15 +1169,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
+        table = _process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
         cond = in_(
             get_column(table, self.col),
             to_list(self.values),
             **self.cond_kwargs,
         )
         if self.not_:
             cond = cond._negate()
@@ -1278,15 +1241,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
+        table = _process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
         conds = [
             has_substring(get_column(table, self.col), sub, **self.cond_kwargs)
             for sub in self.substrings
         ]
 
         if self.any_:
             cond = or_(*conds)
@@ -1347,15 +1310,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
+        table = _process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
         cond = starts_with(get_column(table, self.col), self.string, **self.cond_kwargs)
         if self.not_:
             cond = cond._negate()
 
         if self.binarize_col is not None:
             return select(
                 table, cast(cond, Boolean).label(self.binarize_col)
@@ -1407,15 +1370,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
+        table = _process_checks(table, cols=self.col, cols_not_in=self.binarize_col)
         cond = ends_with(get_column(table, self.col), self.string, **self.cond_kwargs)
         if self.not_:
             cond = cond._negate()
 
         if self.binarize_col is not None:
             return select(
                 table, cast(cond, Boolean).label(self.binarize_col)
@@ -1463,15 +1426,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(
+        table = _process_checks(
             table, cols=self.timestamp_col, cols_not_in=self.binarize_col
         )
         cond = in_(
             extract("year", get_column(table, self.timestamp_col)),
             to_list(self.years),
         )
         if self.not_:
@@ -1524,15 +1487,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(
+        table = _process_checks(
             table, cols=self.timestamp_col, cols_not_in=self.binarize_col
         )
         cond = in_(
             extract("month", get_column(table, self.timestamp_col)),
             to_list(self.months),
         )
         if self.not_:
@@ -1573,15 +1536,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, timestamp_cols=self.timestamp_col)
+        table = _process_checks(table, timestamp_cols=self.timestamp_col)
 
         if isinstance(self.timestamp, str):
             timestamp = to_datetime_format(self.timestamp)
         else:
             timestamp = self.timestamp
 
         return (
@@ -1618,15 +1581,15 @@
 
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
-        table = process_checks(table, timestamp_cols=self.timestamp_col)
+        table = _process_checks(table, timestamp_cols=self.timestamp_col)
 
         if isinstance(self.timestamp, str):
             timestamp = to_datetime_format(self.timestamp)
         else:
             timestamp = self.timestamp
 
         return (
@@ -1723,15 +1686,15 @@
         Returns
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
         self.cols = to_list(self.cols)
-        table = process_checks(table, cols=self.cols)
+        table = _process_checks(table, cols=self.cols)
 
         cond = and_(*[not_equals(get_column(table, col), None) for col in self.cols])
         return select(table).where(cond).subquery()
 
 
 @dataclass
 class OrderBy:
@@ -1762,15 +1725,15 @@
         -------
         sqlalchemy.sql.selectable.Subquery
             Processed table.
 
         """
         self.cols = to_list(self.cols)
         ascending = to_list_optional(self.ascending)
-        table = process_checks(table, cols=self.cols)
+        table = _process_checks(table, cols=self.cols)
 
         if ascending is None:
             ascending = [True] * len(self.cols)
         else:
             if len(ascending) != len(self.cols):
                 raise ValueError(
                     "If ascending is specified. Must specify for all columns."
@@ -1851,15 +1814,15 @@
         # the column being aggregated over
         aggfunc_names = [
             aggfunc_cols[i] if isinstance(item[1], str) else item[1][1]
             for i, item in enumerate(aggfunc_tuples)
         ]
 
         groupby_names = to_list(self.groupby_cols)
-        table = process_checks(table, cols=groupby_names + aggfunc_cols)
+        table = _process_checks(table, cols=groupby_names + aggfunc_cols)
 
         # Error checking
         for i, aggfunc_str in enumerate(aggfunc_strs):
             if aggfunc_str not in str_to_aggfunc:
                 allowed_strs = ", ".join(list(str_to_aggfunc.keys()))
                 raise ValueError(
                     f"Invalid aggfuncs specified. Allowed values are {allowed_strs}."
```

### Comparing `pycyclops-0.1.8/cyclops/query/util.py` & `pycyclops-0.1.9/cyclops/query/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,57 @@
     data: sqlalchemy.sql.schema.MetaData
 
 
 TABLE_OBJECTS = [Table, Select, Subquery, DBTable]
 TableTypes = Union[Select, Subquery, Table, DBTable]
 
 
+def ckwarg(kwargs: dict, kwarg: str):
+    """Get the value of a conditional keyword argument.
+
+    A keyword argument may or may not be specified in some
+    keyword arguments. If specified, return the value,
+    otherwise return None.
+
+    Parameters
+    ----------
+    kwargs: dict
+        Process keyword arguments.
+    kwarg: str
+        The keyword argument of interest.
+
+    Returns
+    -------
+    any, optional
+        The value of the keyword argument if it exists, otherwise None.
+
+    """
+    if kwarg in kwargs:
+        return kwargs[kwarg]
+    return None
+
+
+def remove_kwargs(process_kwargs: dict, kwargs: Union[str, List[str]]):
+    """Remove some keyword arguments from process_kwargs if they exist.
+
+    Parameters
+    ----------
+    process_kwargs: dict
+        Process keyword arguments.
+    kwargs: str or list of str
+        The keyword arguments to remove should they exist.
+
+    """
+    kwargs = to_list(kwargs)
+    for kwarg in kwargs:
+        if kwarg in process_kwargs:
+            del process_kwargs[kwarg]
+    return process_kwargs
+
+
 def _to_subquery(table: TableTypes) -> Subquery:
     """Convert a table from a table type object to the Subquery type.
 
     Parameters
     ----------
     table: cyclops.query.util.TableTypes
         Table to convert.
```

### Comparing `pycyclops-0.1.8/cyclops/utils/common.py` & `pycyclops-0.1.9/cyclops/utils/common.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/utils/file.py` & `pycyclops-0.1.9/cyclops/utils/file.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/utils/indexing.py` & `pycyclops-0.1.9/cyclops/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/utils/log.py` & `pycyclops-0.1.9/cyclops/utils/log.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/utils/profile.py` & `pycyclops-0.1.9/cyclops/utils/profile.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/cyclops/workflow/task.py` & `pycyclops-0.1.9/cyclops/workflow/task.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.1.8/pyproject.toml` & `pycyclops-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycyclops"
-version = "0.1.8"
+version = "0.1.9"
 description = "Framework for healthcare ML implementation"
 authors = ["Vector AI Engineering <cyclops@vectorinstitute.ai>"]
 license = "Apache-2.0"
 repository = "https://github.com/VectorInstitute/cyclops"
 documentation = "https://vectorinstitute.github.io/cyclops/"
 packages = [
     { include = "cyclops" },
```

### Comparing `pycyclops-0.1.8/setup.py` & `pycyclops-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,17 @@
  'tables>=3.7.0,<4.0.0',
  'torch>=1.11.0,<2.0.0',
  'torchxrayvision>=0.0.37,<0.0.38',
  'xgboost>=1.5.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'pycyclops',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Framework for healthcare ML implementation',
-    'long_description': "![cyclops Logo](https://github.com/VectorInstitute/cyclops/blob/main/docs/source/theme/static/cyclops_logo-dark.png?raw=true)\n\n--------------------------------------------------------------------------------\n\n[![PyPI](https://img.shields.io/pypi/v/pycyclops)](https://pypi.org/project/pycyclops)\n[![code checks](https://github.com/VectorInstitute/cyclops/actions/workflows/code_checks.yml/badge.svg)](https://github.com/VectorInstitute/cyclops/actions/workflows/code_checks.yml)\n[![integration tests](https://github.com/VectorInstitute/cyclops/actions/workflows/integration_tests.yml/badge.svg)](https://github.com/VectorInstitute/cyclops/actions/workflows/integration_tests.yml)\n[![docs](https://github.com/VectorInstitute/cyclops/actions/workflows/docs_deploy.yml/badge.svg)](https://github.com/VectorInstitute/cyclops/actions/workflows/docs_deploy.yml)\n[![codecov](https://codecov.io/gh/VectorInstitute/cyclops/branch/main/graph/badge.svg)](https://codecov.io/gh/VectorInstitute/cyclops)\n[![license](https://img.shields.io/github/license/VectorInstitute/cyclops.svg)](https://github.com/VectorInstitute/cyclops/blob/main/LICENSE)\n\n``cyclops`` is a framework for facilitating research and deployment of ML models\nin the health (or clinical) setting. It provides a few high-level APIs namely:\n\n\n* `query` - Querying EHR databases (such as MIMIC-IV)\n* `process` - Process static and temporal EHR data\n* `evaluate` - Evaluate models on clinical prediction tasks\n* `monitor` - Detect data drift relevant for clinical use cases\n\n``cyclops`` also provides a library of use-cases on clinical datasets. The implemented\nuse cases include:\n\n* Mortality decompensation prediction\n\n\n## 🐣 Getting Started\n\n### Installing the core cyclops package using pip\n\n```bash\npython3 -m pip install pycyclops\n```\n\n## 🧑🏿\u200d💻 Developing\n\nThe development environment has been tested on ``python = 3.9``.\n\nThe python virtual environment can be set up using\n[poetry](https://python-poetry.org/docs/#installation). Hence, make sure it is\ninstalled and then run:\n\n```bash\npoetry install\nsource $(poetry env info --path)/bin/activate\n```\n\n## 📚 [Documentation](https://vectorinstitute.github.io/cyclops/)\n\n## 🎓 Notebooks\n\nTo use jupyter notebooks, the python virtual environment can be installed and\nused inside an IPython kernel. After activating the virtual environment, run:\n\n```bash\npython3 -m ipykernel install --user --name <name_of_kernel>\n```\n\nNow, you can navigate to the notebook's ``Kernel`` tab and set it as\n``<name_of_kernel>``.\n\nTutorial notebooks in ``tutorials`` can be useful to view the\nfunctionality of the framework.\n\n## Reference\nReference to cite when you use CyclOps in a project or a research paper:\n```\n@article {Krishnan2022.12.02.22283021,\n\tauthor = {Krishnan, Amrit and Subasri, Vallijah and McKeen, Kaden and Kore, Ali and Ogidi, Franklin and Alinoori, Mahshid and Lalani, Nadim and Dhalla, Azra and Verma, Amol and Razak, Fahad and Pandya, Deval and Dolatabadi, Elham},\n\ttitle = {CyclOps: Cyclical development towards operationalizing ML models for health},\n\telocation-id = {2022.12.02.22283021},\n\tyear = {2022},\n\tdoi = {10.1101/2022.12.02.22283021},\n\tpublisher = {Cold Spring Harbor Laboratory Press},\n\tURL = {https://www.medrxiv.org/content/early/2022/12/08/2022.12.02.22283021},\n\tjournal = {medRxiv}\n}\n```\n",
+    'long_description': "![cyclops Logo](https://github.com/VectorInstitute/cyclops/blob/main/docs/source/theme/static/cyclops_logo-dark.png?raw=true)\n\n--------------------------------------------------------------------------------\n\n[![PyPI](https://img.shields.io/pypi/v/pycyclops)](https://pypi.org/project/pycyclops)\n[![code checks](https://github.com/VectorInstitute/cyclops/actions/workflows/code_checks.yml/badge.svg)](https://github.com/VectorInstitute/cyclops/actions/workflows/code_checks.yml)\n[![integration tests](https://github.com/VectorInstitute/cyclops/actions/workflows/integration_tests.yml/badge.svg)](https://github.com/VectorInstitute/cyclops/actions/workflows/integration_tests.yml)\n[![docs](https://github.com/VectorInstitute/cyclops/actions/workflows/docs_deploy.yml/badge.svg)](https://github.com/VectorInstitute/cyclops/actions/workflows/docs_deploy.yml)\n[![codecov](https://codecov.io/gh/VectorInstitute/cyclops/branch/main/graph/badge.svg)](https://codecov.io/gh/VectorInstitute/cyclops)\n[![license](https://img.shields.io/github/license/VectorInstitute/cyclops.svg)](https://github.com/VectorInstitute/cyclops/blob/main/LICENSE)\n\n``cyclops`` is a framework for facilitating research and deployment of ML models\nin the health (or clinical) setting. It provides a few high-level APIs namely:\n\n\n* `query` - Querying EHR databases (such as MIMIC-IV)\n* `process` - Process static and temporal EHR data\n* `evaluate` - Evaluate models on clinical prediction tasks\n* `monitor` - Detect data drift relevant for clinical use cases\n\n``cyclops`` also provides a library of use-cases on clinical datasets. The implemented\nuse cases include:\n\n* Mortality decompensation prediction\n\n\n## 🐣 Getting Started\n\n### Installing the cyclops package using pip\n\n```bash\npython3 -m pip install pycyclops\n```\n\n## 🧑🏿\u200d💻 Developing\n\nThe development environment has been tested on ``python = 3.9``.\n\nThe python virtual environment can be set up using\n[poetry](https://python-poetry.org/docs/#installation). Hence, make sure it is\ninstalled and then run:\n\n```bash\npoetry install\nsource $(poetry env info --path)/bin/activate\n```\n\n## 📚 [Documentation](https://vectorinstitute.github.io/cyclops/)\n\n## 🎓 Notebooks\n\nTo use jupyter notebooks, the python virtual environment can be installed and\nused inside an IPython kernel. After activating the virtual environment, run:\n\n```bash\npython3 -m ipykernel install --user --name <name_of_kernel>\n```\n\nNow, you can navigate to the notebook's ``Kernel`` tab and set it as\n``<name_of_kernel>``.\n\nTutorial notebooks in ``tutorials`` can be useful to view the\nfunctionality of the framework.\n\n## Reference\nReference to cite when you use CyclOps in a project or a research paper:\n```\n@article {Krishnan2022.12.02.22283021,\n\tauthor = {Krishnan, Amrit and Subasri, Vallijah and McKeen, Kaden and Kore, Ali and Ogidi, Franklin and Alinoori, Mahshid and Lalani, Nadim and Dhalla, Azra and Verma, Amol and Razak, Fahad and Pandya, Deval and Dolatabadi, Elham},\n\ttitle = {CyclOps: Cyclical development towards operationalizing ML models for health},\n\telocation-id = {2022.12.02.22283021},\n\tyear = {2022},\n\tdoi = {10.1101/2022.12.02.22283021},\n\tpublisher = {Cold Spring Harbor Laboratory Press},\n\tURL = {https://www.medrxiv.org/content/early/2022/12/08/2022.12.02.22283021},\n\tjournal = {medRxiv}\n}\n```\n",
     'author': 'Vector AI Engineering',
     'author_email': 'cyclops@vectorinstitute.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/VectorInstitute/cyclops',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pycyclops-0.1.8/PKG-INFO` & `pycyclops-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycyclops
-Version: 0.1.8
+Version: 0.1.9
 Summary: Framework for healthcare ML implementation
 Home-page: https://github.com/VectorInstitute/cyclops
 License: Apache-2.0
 Author: Vector AI Engineering
 Author-email: cyclops@vectorinstitute.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -62,15 +62,15 @@
 use cases include:
 
 * Mortality decompensation prediction
 
 
 ## 🐣 Getting Started
 
-### Installing the core cyclops package using pip
+### Installing the cyclops package using pip
 
 ```bash
 python3 -m pip install pycyclops
 ```
 
 ## 🧑🏿‍💻 Developing
```


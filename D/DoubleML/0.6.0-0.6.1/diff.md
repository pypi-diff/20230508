# Comparing `tmp/DoubleML-0.6.0.tar.gz` & `tmp/DoubleML-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DoubleML-0.6.0.tar", last modified: Tue Apr  4 13:17:04 2023, max compression
+gzip compressed data, was "DoubleML-0.6.1.tar", last modified: Mon May  8 07:40:23 2023, max compression
```

## Comparing `DoubleML-0.6.0.tar` & `DoubleML-0.6.1.tar`

### file list

```diff
@@ -1,100 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:04.044239 DoubleML-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:04.036239 DoubleML-0.6.0/DoubleML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-04 13:17:03.000000 DoubleML-0.6.0/DoubleML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-04 13:17:04.000000 DoubleML-0.6.0/DoubleML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:17:03.000000 DoubleML-0.6.0/DoubleML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 13:17:03.000000 DoubleML-0.6.0/DoubleML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 13:17:03.000000 DoubleML-0.6.0/DoubleML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-04 13:16:41.000000 DoubleML-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 13:16:41.000000 DoubleML-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-04 13:17:04.044239 DoubleML-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-04 13:16:41.000000 DoubleML-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:04.036239 DoubleML-0.6.0/doubleml/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/_utils_resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    27979 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    65216 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_blp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    33370 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_iivm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20063 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_irm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_lpq.py
--rw-r--r--   0 runner    (1001) docker     (123)    35461 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_pliv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_plr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16956 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_pq.py
--rw-r--r--   0 runner    (1001) docker     (123)    30827 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_qte.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/double_ml_score_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:04.044239 DoubleML-0.6.0/doubleml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_blp_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_boot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_cvar_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_dml_cv_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_iivm_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_irm_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_lpq_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_pliv_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_pliv_partial_x_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_pliv_partial_xz_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_pliv_partial_z_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_plr_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_pq_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/_utils_qte_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_blp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_cv_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_cvar_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_dml_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_doubleml_evaluate_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    47142 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_doubleml_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_doubleml_model_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_doubleml_return_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_doubleml_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_doubleml_set_ml_nuisance_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_doubleml_set_sample_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_iivm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_iivm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_iivm_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_iivm_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_iivm_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_irm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_irm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_irm_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_irm_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_irm_with_missings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_lpq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_lpq_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_multiway_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_nonlinear_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_nonlinear_score_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_partial_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_partial_x_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_partial_xz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_partial_xz_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_partial_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_partial_z_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pliv_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_multi_treat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_reestimate_from_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_rep_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_set_ml_nuisance_pars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_set_smpls_externally.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_plr_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_pq_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-04 13:16:41.000000 DoubleML-0.6.0/doubleml/tests/test_qte.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-04 13:16:41.000000 DoubleML-0.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:17:04.044239 DoubleML-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-04 13:16:41.000000 DoubleML-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.437108 DoubleML-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.425108 DoubleML-0.6.1/DoubleML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-08 07:39:55.000000 DoubleML-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 07:39:55.000000 DoubleML-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-08 07:40:23.437108 DoubleML-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-08 07:39:55.000000 DoubleML-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.429108 DoubleML-0.6.1/doubleml/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/_utils_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65216 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_blp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37992 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_did_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_iivm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19981 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_irm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_lpq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35461 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_pliv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_plr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16978 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_pq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_qte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_score_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.437108 DoubleML-0.6.1/doubleml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_blp_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_boot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_cvar_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_did_cs_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_did_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_dml_cv_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_iivm_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_irm_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_lpq_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_x_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_xz_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_z_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_plr_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pq_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_qte_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_blp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_cv_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_cvar_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did_cs_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_dml_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_evaluate_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55575 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_model_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_set_ml_nuisance_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_set_sample_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_with_missings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_lpq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_lpq_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_multiway_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_nonlinear_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_nonlinear_score_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_multi_treat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_reestimate_from_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_rep_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_set_ml_nuisance_pars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_set_smpls_externally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pq_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_qte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 07:39:55.000000 DoubleML-0.6.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:40:23.437108 DoubleML-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 07:39:55.000000 DoubleML-0.6.1/setup.py
```

### Comparing `DoubleML-0.6.0/DoubleML.egg-info/PKG-INFO` & `DoubleML-0.6.1/DoubleML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoubleML
-Version: 0.6.0
+Version: 0.6.1
 Summary: Double Machine Learning in Python
 Home-page: https://docs.doubleml.org
 Author: Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.
 Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Documentation, https://docs.doubleml.org
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DoubleML Version: 0.6.0 Summary: Double Machine
+Metadata-Version: 2.1 Name: DoubleML Version: 0.6.1 Summary: Double Machine
 Learning in Python Home-page: https://docs.doubleml.org Author: Bach, P.,
 Chernozhukov, V., Kurz, M. S., and Spindler, M. Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de License: UNKNOWN Project-URL:
 Documentation, https://docs.doubleml.org Project-URL: Source Code, https://
 github.com/DoubleML/doubleml-for-py Project-URL: Bug Tracker, https://
 github.com/DoubleML/doubleml-for-py/issues Description: # DoubleML - Double
 Machine Learning in Python [https://raw.githubusercontent.com/DoubleML/
```

### Comparing `DoubleML-0.6.0/DoubleML.egg-info/SOURCES.txt` & `DoubleML-0.6.1/DoubleML.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 doubleml/_utils.py
 doubleml/_utils_resampling.py
 doubleml/datasets.py
 doubleml/double_ml.py
 doubleml/double_ml_blp.py
 doubleml/double_ml_cvar.py
 doubleml/double_ml_data.py
+doubleml/double_ml_did.py
+doubleml/double_ml_did_cs.py
 doubleml/double_ml_iivm.py
 doubleml/double_ml_irm.py
 doubleml/double_ml_lpq.py
 doubleml/double_ml_pliv.py
 doubleml/double_ml_plr.py
 doubleml/double_ml_pq.py
 doubleml/double_ml_qte.py
 doubleml/double_ml_score_mixins.py
 doubleml/tests/__init__.py
 doubleml/tests/_utils.py
 doubleml/tests/_utils_blp_manual.py
 doubleml/tests/_utils_boot.py
 doubleml/tests/_utils_cluster.py
 doubleml/tests/_utils_cvar_manual.py
+doubleml/tests/_utils_did_cs_manual.py
+doubleml/tests/_utils_did_manual.py
 doubleml/tests/_utils_dml_cv_predict.py
 doubleml/tests/_utils_iivm_manual.py
 doubleml/tests/_utils_irm_manual.py
 doubleml/tests/_utils_lpq_manual.py
 doubleml/tests/_utils_pliv_manual.py
 doubleml/tests/_utils_pliv_partial_x_manual.py
 doubleml/tests/_utils_pliv_partial_xz_manual.py
@@ -43,14 +47,18 @@
 doubleml/tests/_utils_qte_manual.py
 doubleml/tests/conftest.py
 doubleml/tests/test_blp.py
 doubleml/tests/test_cv_predict.py
 doubleml/tests/test_cvar.py
 doubleml/tests/test_cvar_tune.py
 doubleml/tests/test_datasets.py
+doubleml/tests/test_did.py
+doubleml/tests/test_did_cs.py
+doubleml/tests/test_did_cs_tune.py
+doubleml/tests/test_did_tune.py
 doubleml/tests/test_dml_data.py
 doubleml/tests/test_doubleml_evaluate_learner.py
 doubleml/tests/test_doubleml_exceptions.py
 doubleml/tests/test_doubleml_model_defaults.py
 doubleml/tests/test_doubleml_return_types.py
 doubleml/tests/test_doubleml_scores.py
 doubleml/tests/test_doubleml_set_ml_nuisance_params.py
```

### Comparing `DoubleML-0.6.0/LICENSE` & `DoubleML-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/PKG-INFO` & `DoubleML-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoubleML
-Version: 0.6.0
+Version: 0.6.1
 Summary: Double Machine Learning in Python
 Home-page: https://docs.doubleml.org
 Author: Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.
 Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Documentation, https://docs.doubleml.org
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DoubleML Version: 0.6.0 Summary: Double Machine
+Metadata-Version: 2.1 Name: DoubleML Version: 0.6.1 Summary: Double Machine
 Learning in Python Home-page: https://docs.doubleml.org Author: Bach, P.,
 Chernozhukov, V., Kurz, M. S., and Spindler, M. Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de License: UNKNOWN Project-URL:
 Documentation, https://docs.doubleml.org Project-URL: Source Code, https://
 github.com/DoubleML/doubleml-for-py Project-URL: Bug Tracker, https://
 github.com/DoubleML/doubleml-for-py/issues Description: # DoubleML - Double
 Machine Learning in Python [https://raw.githubusercontent.com/DoubleML/
```

### Comparing `DoubleML-0.6.0/README.md` & `DoubleML-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/__init__.py` & `DoubleML-0.6.1/doubleml/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 
 from .double_ml_plr import DoubleMLPLR
 from .double_ml_pliv import DoubleMLPLIV
 from .double_ml_irm import DoubleMLIRM
 from .double_ml_iivm import DoubleMLIIVM
 from .double_ml_data import DoubleMLData, DoubleMLClusterData
 from .double_ml_blp import DoubleMLBLP
+from .double_ml_did import DoubleMLDID
+from .double_ml_did_cs import DoubleMLDIDCS
 from .double_ml_qte import DoubleMLQTE
 from .double_ml_pq import DoubleMLPQ
 from .double_ml_lpq import DoubleMLLPQ
 from .double_ml_cvar import DoubleMLCVAR
 
 __all__ = ['DoubleMLPLR',
            'DoubleMLPLIV',
            'DoubleMLIRM',
            'DoubleMLIIVM',
            'DoubleMLData',
            'DoubleMLClusterData',
            'DoubleMLBLP',
+           'DoubleMLDID',
+           'DoubleMLDIDCS',
            'DoubleMLPQ',
            'DoubleMLQTE',
            'DoubleMLLPQ',
            'DoubleMLCVAR']
 
 __version__ = get_distribution('doubleml').version
```

### Comparing `DoubleML-0.6.0/doubleml/_utils.py` & `DoubleML-0.6.1/doubleml/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,26 @@
 
 def _get_cond_smpls(smpls, bin_var):
     smpls_0 = [(np.intersect1d(np.where(bin_var == 0)[0], train), test) for train, test in smpls]
     smpls_1 = [(np.intersect1d(np.where(bin_var == 1)[0], train), test) for train, test in smpls]
     return smpls_0, smpls_1
 
 
+def _get_cond_smpls_2d(smpls, bin_var1, bin_var2):
+    subset_00 = (bin_var1 == 0) & (bin_var2 == 0)
+    smpls_00 = [(np.intersect1d(np.where(subset_00)[0], train), test) for train, test in smpls]
+    subset_01 = (bin_var1 == 0) & (bin_var2 == 1)
+    smpls_01 = [(np.intersect1d(np.where(subset_01)[0], train), test) for train, test in smpls]
+    subset_10 = (bin_var1 == 1) & (bin_var2 == 0)
+    smpls_10 = [(np.intersect1d(np.where(subset_10)[0], train), test) for train, test in smpls]
+    subset_11 = (bin_var1 == 1) & (bin_var2 == 1)
+    smpls_11 = [(np.intersect1d(np.where(subset_11)[0], train), test) for train, test in smpls]
+    return smpls_00, smpls_01, smpls_10, smpls_11
+
+
 def _check_is_partition(smpls, n_obs):
     test_indices = np.concatenate([test_index for _, test_index in smpls])
     if len(test_indices) != n_obs:
         return False
     hit = np.zeros(n_obs, dtype=bool)
     hit[test_indices] = True
     if not np.all(hit):
@@ -324,22 +336,27 @@
                         f'Object of type {str(type(trimming_threshold))} passed.')
     if (trimming_threshold <= 0) | (trimming_threshold >= 0.5):
         raise ValueError('Invalid trimming_threshold ' + str(trimming_threshold) + '. ' +
                          'trimming_threshold has to be between 0 and 0.5.')
     return
 
 
-def _check_score(score, valid_score):
+def _check_score(score, valid_score, allow_callable=True):
     if isinstance(score, str):
         if score not in valid_score:
             raise ValueError('Invalid score ' + score + '. ' +
                              'Valid score ' + ' or '.join(valid_score) + '.')
     else:
-        raise TypeError('Invalid score. ' +
-                        'Valid score ' + ' or '.join(valid_score) + '.')
+        if allow_callable:
+            if not callable(score):
+                raise TypeError('score should be either a string or a callable. '
+                                '%r was passed.' % score)
+        else:
+            raise TypeError('score should be a string. '
+                            '%r was passed.' % score)
     return
 
 
 def _get_bracket_guess(score, coef_start, coef_bounds):
     max_bracket_length = coef_bounds[1] - coef_bounds[0]
     b_guess = coef_bounds
     delta = 0.1
```

### Comparing `DoubleML-0.6.0/doubleml/_utils_resampling.py` & `DoubleML-0.6.1/doubleml/_utils_resampling.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/datasets.py` & `DoubleML-0.6.1/doubleml/datasets.py`

 * *Files 15% similar despite different names*

```diff
@@ -374,15 +374,15 @@
         \\mathcal{N}\\left(0, \\left(\\begin{matrix} 1 & 0.3 \\\\ 0.3 & 1 \\end{matrix} \\right) \\right).
 
     The covariates :math:`x_i \\sim \\mathcal{N}(0, \\Sigma)`, where  :math:`\\Sigma` is a matrix with entries
     :math:`\\Sigma_{kj} = 0.5^{|j-k|}` and :math:`\\beta` is a `dim_x`-vector with entries
     :math:`\\beta_j=\\frac{1}{j^2}`.
 
     The data generating process is inspired by a process used in the simulation experiment of Farbmacher, Gruber and
-    Klaaßen (2020).
+    Klaassen (2020).
 
     Parameters
     ----------
     n_obs :
         The number of observations to simulate.
     dim_x :
         The number of covariates.
@@ -701,7 +701,195 @@
                          axis=1)
         if return_type in _data_frame_alias:
             return data
         else:
             return DoubleMLClusterData(data, 'Y', 'D', cluster_cols, x_cols, 'Z')
     else:
         raise ValueError('Invalid return_type.')
+
+
+def make_did_SZ2020(n_obs=500, dgp_type=1, cross_sectional_data=False, return_type='DoubleMLData', **kwargs):
+    """
+    Generates data from a difference-in-differences model used in Sant'Anna and Zhao (2020).
+    The data generating process is defined as follows. For a generic :math:`W=(W_1, W_2, W_3, W_4)^T`, let
+
+    .. math::
+
+        f_{reg}(W) &= 210 + 27.4 \\cdot W_1 +13.7 \\cdot (W_2 + W_3 + W_4),
+
+        f_{ps}(W) &= 0.75 \\cdot (-W_1 + 0.5 \\cdot W_2 -0.25 \\cdot W_3 - 0.1 \\cdot W_4).
+
+
+    Let :math:`X= (X_1, X_2, X_3, X_4)^T \\sim \\mathcal{N}(0, \\Sigma)`, where  :math:`\\Sigma` is a matrix with entries
+    :math:`\\Sigma_{kj} = c^{|j-k|}`. The default value is  :math:`c = 0`, corresponding to the identity matrix.
+    Further, define :math:`Z_j = (\\tilde{Z_j} - \\mathbb{E}[\\tilde{Z}_j]) / \\sqrt{\\text{Var}(\\tilde{Z}_j)}`,
+    where :math:`\\tilde{Z}_1 = \\exp(0.5 \\cdot X_1)`, :math:`\\tilde{Z}_2 = 10 + X_2/(1 + \\exp(X_1))`,
+    :math:`\\tilde{Z}_3 = (0.6 + X_1 \\cdot X_3 / 25)^3` and :math:`\\tilde{Z}_4 = (20 + X_2 + X_4)^2`.
+    At first define
+
+    .. math::
+
+        Y_0(0) &= f_{reg}(W_{reg}) + \\nu(W_{reg}, D) + \\varepsilon_0,
+
+        Y_1(d) &= 2 \\cdot f_{reg}(W_{reg}) + \\nu(W_{reg}, D) + \\varepsilon_1(d),
+
+        p(W_{ps}) &= \\frac{\\exp(f_{ps}(W_{ps}))}{1 + \\exp(f_{ps}(W_{ps}))},
+
+        D &= 1\\{p(W_{ps}) \\ge U\\},
+
+    where :math:`\\varepsilon_0, \\varepsilon_1(d), d=0, 1` are independent standard normal random variables,
+    :math:`U \\sim \\mathcal{U}[0, 1]` is a independent standard uniform
+    and :math:`\\nu(W_{reg}, D)\\sim \\mathcal{N}(D \\cdot f_{reg}(W_{reg}),1)`.
+    The different data generating processes are defined via
+
+    .. math::
+
+        DGP1:\\quad W_{reg} &= Z \\quad W_{ps} = Z
+
+        DGP2:\\quad W_{reg} &= Z \\quad W_{ps} = X
+
+        DGP3:\\quad W_{reg} &= X \\quad W_{ps} = Z
+
+        DGP4:\\quad W_{reg} &= X \\quad W_{ps} = X
+
+        DGP5:\\quad W_{reg} &= Z \\quad W_{ps} = 0
+
+        DGP6:\\quad W_{reg} &= X \\quad W_{ps} = 0,
+
+    such that the last two settings correspond to an experimental setting with treatment probability
+    of :math:`P(D=1) = \\frac{1}{2}.`
+    For the panel data the outcome is already defined as the difference :math:`Y = Y_1(D) - Y_0(0)`.
+    For cross-sectional data the flag ``cross_sectional_data`` has to be set to ``True``.
+    Then the outcome will be defined to be
+
+    .. math::
+
+        Y = T \\cdot Y_1(D) + (1-T) \\cdot Y_0(0),
+
+    where :math:`T = 1\\{U_T\\le \\lambda_T \\}` with :math:`U_T\\sim \\mathcal{U}[0, 1]` and :math:`\\lambda_T=0.5`.
+    The true average treatment effect on the treated is zero for all data generating processes.
+
+    Parameters
+    ----------
+    n_obs :
+        The number of observations to simulate.
+    dgp_type :
+        The DGP to be used. Default value is ``1`` (integer).
+    cross_sectional_data :
+        Indicates whether the setting is uses cross-sectional or panel data. Default value is ``False``.
+    return_type :
+        If ``'DoubleMLData'`` or ``DoubleMLData``, returns a ``DoubleMLData`` object.
+
+        If ``'DataFrame'``, ``'pd.DataFrame'`` or ``pd.DataFrame``, returns a ``pd.DataFrame``.
+
+        If ``'array'``, ``'np.ndarray'``, ``'np.array'`` or ``np.ndarray``, returns ``np.ndarray``'s ``(x, y, d)``
+        or ``(x, y, d, t)``.
+    **kwargs
+        Additional keyword arguments to set non-default values for the parameter
+        :math:`xi=0.75`, :math:`c=0.0` and :math:`\\lambda_T=0.5`.
+
+    References
+    ----------
+    Sant’Anna, P. H. and Zhao, J. (2020),
+    Doubly robust difference-in-differences estimators. Journal of Econometrics, 219(1), 101-122.
+    doi:`10.1016/j.jeconom.2020.06.003 <https://doi.org/10.1016/j.jeconom.2020.06.003>`_.
+    """
+    xi = kwargs.get('xi', 0.75)
+    c = kwargs.get('c', 0.0)
+    lambda_t = kwargs.get('lambda_t', 0.5)
+
+    def f_reg(w):
+        res = 210 + 27.4*w[:, 0] + 13.7*(w[:, 1] + w[:, 2] + w[:, 3])
+        return res
+
+    def f_ps(w, xi):
+        res = xi*(-w[:, 0] + 0.5*w[:, 1] - 0.25*w[:, 2] - 0.1*w[:, 3])
+        return res
+
+    dim_x = 4
+    cov_mat = toeplitz([np.power(c, k) for k in range(dim_x)])
+    x = np.random.multivariate_normal(np.zeros(dim_x), cov_mat, size=[n_obs, ])
+    # x = np.random.normal(loc=0, scale=1, size=[n_obs, 4])
+
+    z_tilde_1 = np.exp(0.5*x[:, 0])
+    z_tilde_2 = 10 + x[:, 1] / (1 + np.exp(x[:, 0]))
+    z_tilde_3 = (0.6 + x[:, 0]*x[:, 2]/25)**3
+    z_tilde_4 = (20 + x[:, 1] + x[:, 3])**2
+
+    z_tilde = np.column_stack((z_tilde_1, z_tilde_2, z_tilde_3, z_tilde_4))
+    z = (z_tilde - np.mean(z_tilde, axis=0)) / np.std(z_tilde, axis=0)
+
+    # error terms
+    epsilon_0 = np.random.normal(loc=0, scale=1, size=n_obs)
+    epsilon_1 = np.random.normal(loc=0, scale=1, size=[n_obs, 2])
+
+    if dgp_type == 1:
+        features_ps = z
+        features_reg = z
+    elif dgp_type == 2:
+        features_ps = x
+        features_reg = z
+    elif dgp_type == 3:
+        features_ps = z
+        features_reg = x
+    elif dgp_type == 4:
+        features_ps = x
+        features_reg = x
+    elif dgp_type == 5:
+        features_ps = None
+        features_reg = z
+    elif dgp_type == 6:
+        features_ps = None
+        features_reg = x
+    else:
+        raise ValueError('The dgp_type is not valid.')
+
+    # treatment and propensities
+    is_experimental = (dgp_type == 5) or (dgp_type == 6)
+    if is_experimental:
+        # Set D to be experimental
+        p = 0.5 * np.ones(n_obs)
+    else:
+        p = np.exp(f_ps(features_ps, xi)) / (1 + np.exp(f_ps(features_ps, xi)))
+    u = np.random.uniform(low=0, high=1, size=n_obs)
+    d = 1.0 * (p >= u)
+
+    # potential outcomes
+    nu = np.random.normal(loc=d*f_reg(features_reg), scale=1, size=n_obs)
+    y0 = f_reg(features_reg) + nu + epsilon_0
+    y1_d0 = 2 * f_reg(features_reg) + nu + epsilon_1[:, 0]
+    y1_d1 = 2 * f_reg(features_reg) + nu + epsilon_1[:, 1]
+    y1 = d * y1_d1 + (1-d) * y1_d0
+
+    if not cross_sectional_data:
+        y = y1 - y0
+
+        if return_type in _array_alias:
+            return z, y, d
+        elif return_type in _data_frame_alias + _dml_data_alias:
+            z_cols = [f'Z{i + 1}' for i in np.arange(dim_x)]
+            data = pd.DataFrame(np.column_stack((z, y, d)),
+                                columns=z_cols + ['y', 'd'])
+            if return_type in _data_frame_alias:
+                return data
+            else:
+                return DoubleMLData(data, 'y', 'd', z_cols)
+        else:
+            raise ValueError('Invalid return_type.')
+
+    else:
+        u_t = np.random.uniform(low=0, high=1, size=n_obs)
+        t = 1.0 * (u_t <= lambda_t)
+        y = t * y1 + (1-t)*y0
+
+        if return_type in _array_alias:
+            return z, y, d, t
+        elif return_type in _data_frame_alias + _dml_data_alias:
+            z_cols = [f'Z{i + 1}' for i in np.arange(dim_x)]
+            data = pd.DataFrame(np.column_stack((z, y, d, t)),
+                                columns=z_cols + ['y', 'd', 't'])
+            if return_type in _data_frame_alias:
+                return data
+            else:
+                return DoubleMLData(data, 'y', 'd', z_cols, t_col='t')
+        else:
+            raise ValueError('Invalid return_type.')
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml.py` & `DoubleML-0.6.1/doubleml/double_ml.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/double_ml_blp.py` & `DoubleML-0.6.1/doubleml/double_ml_blp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import pandas as pd
 
 from scipy.stats import norm
 from scipy.linalg import sqrtm
 
 
 class DoubleMLBLP:
-    """Best linear predictor (BLP) for DoubleML with orthogonal signals. Mainly used for CATE and GATE estimation for IRM models.
+    """Best linear predictor (BLP) for DoubleML with orthogonal signals.
+    Manily used for CATE and GATE estimation for IRM models.
 
-        Parameters
-        ----------
-        orth_signal : :class:`numpy.array`
-            The orthogonal signal to be predicted. Has to be of shape ``(n_obs,)``,
-            where ``n_obs`` is the number of observations.
-
-        basis : :class:`pandas.DataFrame`
-            The basis for estimating the best linear predictor. Has to have the shape ``(n_obs, d)``,
-            where ``n_obs`` is the number of observations and ``d`` is the number of predictors.
-
-        is_gate : bool
-            Indicates whether the basis is constructed for GATEs (dummy-basis).
-            Default is ``False``.
+    Parameters
+    ----------
+    orth_signal : :class:`numpy.array`
+        The orthogonal signal to be predicted. Has to be of shape ``(n_obs,)``,
+        where ``n_obs`` is the number of observations.
+
+    basis : :class:`pandas.DataFrame`
+        The basis for estimating the best linear predictor. Has to have the shape ``(n_obs, d)``,
+        where ``n_obs`` is the number of observations and ``d`` is the number of predictors.
+
+    is_gate : bool
+        Indicates whether the basis is constructed for GATEs (dummy-basis).
+        Default is ``False``.
     """
 
     def __init__(self,
                  orth_signal,
                  basis,
                  is_gate=False):
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_cvar.py` & `DoubleML-0.6.1/doubleml/double_ml_cvar.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
         self._quantile = quantile
         self._treatment = treatment
         self._normalize_ipw = normalize_ipw
 
         self._check_data(self._dml_data)
         valid_score = ['CVaR']
-        _check_score(self.score, valid_score)
+        _check_score(self.score, valid_score, allow_callable=False)
         _check_quantile(self.quantile)
         _check_treatment(self.treatment)
 
         if not isinstance(self.normalize_ipw, bool):
             raise TypeError('Normalization indicator has to be boolean. ' +
                             f'Object of type {str(type(self.normalize_ipw))} passed.')
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_data.py` & `DoubleML-0.6.1/doubleml/double_ml_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -100,14 +100,18 @@
         treatment variables ``d_cols``, nor instrumental variables ``z_cols`` are used as covariates.
         Default is ``None``.
 
     z_cols : None, str or list
         The instrumental variable(s).
         Default is ``None``.
 
+    t_col : None or str
+        The time variable (only relevant/used for DiD Estimators).
+        Default is ``None``.
+
     use_other_treat_as_covariate : bool
         Indicates whether in the multiple-treatment case the other treatment variables should be added as covariates.
         Default is ``True``.
 
     force_all_x_finite : bool or str
         Indicates whether to raise an error on infinite values and / or missings in the covariates ``x``.
         Possible values are: ``True`` (neither missings ``np.nan``, ``pd.NA`` nor infinite values ``np.inf`` are
@@ -130,28 +134,30 @@
     """
     def __init__(self,
                  data,
                  y_col,
                  d_cols,
                  x_cols=None,
                  z_cols=None,
+                 t_col=None,
                  use_other_treat_as_covariate=True,
                  force_all_x_finite=True):
         DoubleMLBaseData.__init__(self, data)
 
         self.y_col = y_col
         self.d_cols = d_cols
         self.z_cols = z_cols
+        self.t_col = t_col
         self.x_cols = x_cols
-        self._check_disjoint_sets_y_d_x_z()
+        self._check_disjoint_sets_y_d_x_z_t()
         self.use_other_treat_as_covariate = use_other_treat_as_covariate
         self.force_all_x_finite = force_all_x_finite
         self._binary_treats = self._check_binary_treats()
         self._binary_outcome = self._check_binary_outcome()
-        self._set_y_z()
+        self._set_y_z_t()
         # by default, we initialize to the first treatment variable
         self.set_x_d(self.d_cols[0])
 
     def __str__(self):
         data_summary = self._data_summary_str()
         buf = io.StringIO()
         self.data.info(verbose=False, buf=buf)
@@ -161,20 +167,23 @@
               '\n------------------ DataFrame info    ------------------\n' + df_info
         return res
 
     def _data_summary_str(self):
         data_summary = f'Outcome variable: {self.y_col}\n' \
                        f'Treatment variable(s): {self.d_cols}\n' \
                        f'Covariates: {self.x_cols}\n' \
-                       f'Instrument variable(s): {self.z_cols}\n' \
-                       f'No. Observations: {self.n_obs}\n'
+                       f'Instrument variable(s): {self.z_cols}\n'
+        if self.t_col is not None:
+            data_summary += f'Time variable: {self.t_col}\n'
+
+        data_summary += f'No. Observations: {self.n_obs}\n'
         return data_summary
 
     @classmethod
-    def from_arrays(cls, x, y, d, z=None, use_other_treat_as_covariate=True,
+    def from_arrays(cls, x, y, d, z=None, t=None, use_other_treat_as_covariate=True,
                     force_all_x_finite=True):
         """
         Initialize :class:`DoubleMLData` from :class:`numpy.ndarray`'s.
 
         Parameters
         ----------
         x : :class:`numpy.ndarray`
@@ -186,14 +195,18 @@
         d : :class:`numpy.ndarray`
             Array of treatment variables.
 
         z : None or :class:`numpy.ndarray`
             Array of instrumental variables.
             Default is ``None``.
 
+        t : :class:`numpy.ndarray`
+            Array of the time variable (only relevant/used for DiD models).
+            Default is ``None``.
+
         use_other_treat_as_covariate : bool
             Indicates whether in the multiple-treatment case the other treatment variables should be added as covariates.
             Default is ``True``.
 
         force_all_x_finite : bool or str
             Indicates whether to raise an error on infinite values and / or missings in the covariates ``x``.
             Possible values are: ``True`` (neither missings ``np.nan``, ``pd.NA`` nor infinite values ``np.inf`` are
@@ -235,29 +248,42 @@
             z = _assure_2d_array(z)
             check_consistent_length(x, y, d, z)
             if z.shape[1] == 1:
                 z_cols = ['z']
             else:
                 z_cols = [f'z{i + 1}' for i in np.arange(z.shape[1])]
 
+        if t is None:
+            t_col = None
+        else:
+            t = column_or_1d(t, warn=True)
+            check_consistent_length(x, y, d, t)
+            t_col = 't'
+
         if d.shape[1] == 1:
             d_cols = ['d']
         else:
             d_cols = [f'd{i+1}' for i in np.arange(d.shape[1])]
 
         x_cols = [f'X{i+1}' for i in np.arange(x.shape[1])]
 
-        if z is None:
+        if (z is None) and (t is None):
             data = pd.DataFrame(np.column_stack((x, y, d)),
                                 columns=x_cols + [y_col] + d_cols)
-        else:
+        elif (z is not None) and (t is None):
             data = pd.DataFrame(np.column_stack((x, y, d, z)),
                                 columns=x_cols + [y_col] + d_cols + z_cols)
+        elif (z is None) and (t is not None):
+            data = pd.DataFrame(np.column_stack((x, y, d, t)),
+                                columns=x_cols + [y_col] + d_cols + [t_col])
+        elif (z is not None) and (t is not None):
+            data = pd.DataFrame(np.column_stack((x, y, d, z, t)),
+                                columns=x_cols + [y_col] + d_cols + z_cols + [t_col])
 
-        return cls(data, y_col, d_cols, x_cols, z_cols, use_other_treat_as_covariate, force_all_x_finite)
+        return cls(data, y_col, d_cols, x_cols, z_cols, t_col, use_other_treat_as_covariate, force_all_x_finite)
 
     @property
     def x(self):
         """
         Array of covariates;
         Dynamic! May depend on the currently set treatment variable;
         To get an array of all covariates (independent of the currently set treatment variable)
@@ -289,14 +315,24 @@
         """
         if self.z_cols is not None:
             return self._z.values
         else:
             return None
 
     @property
+    def t(self):
+        """
+        Array of time variable.
+        """
+        if self.t_col is not None:
+            return self._t.values
+        else:
+            return None
+
+    @property
     def n_treat(self):
         """
         The number of treatment variables.
         """
         return len(self.d_cols)
 
     @property
@@ -352,18 +388,24 @@
                                  'Contains duplicate values.')
             if not set(value).issubset(set(self.all_variables)):
                 raise ValueError('Invalid covariates x_cols. '
                                  'At least one covariate is no data column.')
             assert set(value).issubset(set(self.all_variables))
             self._x_cols = value
         else:
-            # x_cols defaults to all columns but y_col, d_cols and z_cols
-            if self.z_cols is not None:
+            # x_cols defaults to all columns but y_col, d_cols and z_cols (and t_col)
+            if (self.z_cols is not None) & (self.t_col is not None):
+                y_d_z_t = set.union({self.y_col}, set(self.d_cols), set(self.z_cols), {self.t_col})
+                x_cols = [col for col in self.data.columns if col not in y_d_z_t]
+            elif self.z_cols is not None:
                 y_d_z = set.union({self.y_col}, set(self.d_cols), set(self.z_cols))
                 x_cols = [col for col in self.data.columns if col not in y_d_z]
+            elif self.t_col is not None:
+                y_d_t = set.union({self.y_col}, set(self.d_cols), {self.t_col})
+                x_cols = [col for col in self.data.columns if col not in y_d_t]
             else:
                 y_d = set.union({self.y_col}, set(self.d_cols))
                 x_cols = [col for col in self.data.columns if col not in y_d]
             self._x_cols = x_cols
         if reset_value:
             self._check_disjoint_sets()
             # by default, we initialize to the first treatment variable
@@ -411,15 +453,15 @@
                             f'{str(value)} of type {str(type(value))} was passed.')
         if value not in self.all_variables:
             raise ValueError('Invalid outcome variable y_col. '
                              f'{value} is no data column.')
         self._y_col = value
         if reset_value:
             self._check_disjoint_sets()
-            self._set_y_z()
+            self._set_y_z_t()
 
     @property
     def z_cols(self):
         """
         The instrumental variable(s).
         """
         return self._z_cols
@@ -440,15 +482,39 @@
                 raise ValueError('Invalid instrumental variable(s) z_cols. '
                                  'At least one instrumental variable is no data column.')
             self._z_cols = value
         else:
             self._z_cols = None
         if reset_value:
             self._check_disjoint_sets()
-            self._set_y_z()
+            self._set_y_z_t()
+
+    @property
+    def t_col(self):
+        """
+        The time variable.
+        """
+        return self._t_col
+
+    @t_col.setter
+    def t_col(self, value):
+        reset_value = hasattr(self, '_t_col')
+        if value is not None:
+            if not isinstance(value, str):
+                raise TypeError('The time variable t_col must be of str type (or None). '
+                                f'{str(value)} of type {str(type(value))} was passed.')
+            if value not in self.all_variables:
+                raise ValueError('Invalid time variable t_col. '
+                                 f'{value} is no data column.')
+            self._t_col = value
+        else:
+            self._t_col = None
+        if reset_value:
+            self._check_disjoint_sets()
+            self._set_y_z_t()
 
     @property
     def use_other_treat_as_covariate(self):
         """
         Indicates whether in the multiple-treatment case the other treatment variables should be added as covariates.
         """
         return self._use_other_treat_as_covariate
@@ -482,23 +548,29 @@
             raise TypeError("Invalid force_all_x_finite. " +
                             "force_all_x_finite must be True, False or 'allow-nan'.")
         self._force_all_x_finite = value
         if reset_value:
             # by default, we initialize to the first treatment variable
             self.set_x_d(self.d_cols[0])
 
-    def _set_y_z(self):
+    def _set_y_z_t(self):
         assert_all_finite(self.data.loc[:, self.y_col])
         self._y = self.data.loc[:, self.y_col]
         if self.z_cols is None:
             self._z = None
         else:
             assert_all_finite(self.data.loc[:, self.z_cols])
             self._z = self.data.loc[:, self.z_cols]
 
+        if self.t_col is None:
+            self._t = None
+        else:
+            assert_all_finite(self.data.loc[:, self.t_col])
+            self._t = self.data.loc[:, self.t_col]
+
     def set_x_d(self, treatment_var):
         """
         Function that assigns the role for the treatment variables in the multiple-treatment case.
 
         Parameters
         ----------
         treatment_var : str
@@ -538,20 +610,21 @@
         binary_outcome = (type_of_target(y) == 'binary')
         zero_one_outcome = np.all((np.power(y, 2) - y) == 0)
         is_binary = (binary_outcome & zero_one_outcome)
         return is_binary
 
     def _check_disjoint_sets(self):
         # this function can be extended in inherited subclasses
-        self._check_disjoint_sets_y_d_x_z()
+        self._check_disjoint_sets_y_d_x_z_t()
 
-    def _check_disjoint_sets_y_d_x_z(self):
+    def _check_disjoint_sets_y_d_x_z_t(self):
         y_col_set = {self.y_col}
         x_cols_set = set(self.x_cols)
         d_cols_set = set(self.d_cols)
+        t_col_set = {self.t_col}
 
         if not y_col_set.isdisjoint(x_cols_set):
             raise ValueError(f'{str(self.y_col)} cannot be set as outcome variable ``y_col`` and covariate in '
                              '``x_cols``.')
         if not y_col_set.isdisjoint(d_cols_set):
             raise ValueError(f'{str(self.y_col)} cannot be set as outcome variable ``y_col`` and treatment variable in '
                              '``d_cols``.')
@@ -569,14 +642,24 @@
             if not d_cols_set.isdisjoint(z_cols_set):
                 raise ValueError('At least one variable/column is set as treatment variable (``d_cols``) and '
                                  'instrumental variable in ``z_cols``.')
             if not x_cols_set.isdisjoint(z_cols_set):
                 raise ValueError('At least one variable/column is set as covariate (``x_cols``) and instrumental '
                                  'variable in ``z_cols``.')
 
+        if not t_col_set.isdisjoint(x_cols_set):
+            raise ValueError(f'{str(self.t_col)} cannot be set as time variable ``t_col`` and covariate in '
+                             '``x_cols``.')
+        if not t_col_set.isdisjoint(d_cols_set):
+            raise ValueError(f'{str(self.t_col)} cannot be set as time variable ``t_col`` and treatment variable in '
+                             '``d_cols``.')
+        if not t_col_set.isdisjoint(y_col_set):
+            raise ValueError(f'{str(self.t_col)} cannot be set as time variable ``t_col`` and outcome variable '
+                             '``y_col``.')
+
 
 class DoubleMLClusterData(DoubleMLData):
     """Double machine learning data-backend for data with cluster variables.
 
     :class:`DoubleMLClusterData` objects can be initialized from
     :class:`pandas.DataFrame`'s as well as :class:`numpy.ndarray`'s.
 
@@ -600,14 +683,18 @@
         treatment variables ``d_cols``, nor instrumental variables ``z_cols`` are used as covariates.
         Default is ``None``.
 
     z_cols : None, str or list
         The instrumental variable(s).
         Default is ``None``.
 
+    t_col : None or str
+        The time variable (only relevant/used for DiD Estimators).
+        Default is ``None``.
+
     use_other_treat_as_covariate : bool
         Indicates whether in the multiple-treatment case the other treatment variables should be added as covariates.
         Default is ``True``.
 
     force_all_x_finite : bool or str
         Indicates whether to raise an error on infinite values and / or missings in the covariates ``x``.
         Possible values are: ``True`` (neither missings ``np.nan``, ``pd.NA`` nor infinite values ``np.inf`` are
@@ -631,27 +718,29 @@
     def __init__(self,
                  data,
                  y_col,
                  d_cols,
                  cluster_cols,
                  x_cols=None,
                  z_cols=None,
+                 t_col=None,
                  use_other_treat_as_covariate=True,
                  force_all_x_finite=True):
         DoubleMLBaseData.__init__(self, data)
 
         # we need to set cluster_cols (needs _data) before call to the super __init__ because of the x_cols setter
         self.cluster_cols = cluster_cols
         self._set_cluster_vars()
         DoubleMLData.__init__(self,
                               data,
                               y_col,
                               d_cols,
                               x_cols,
                               z_cols,
+                              t_col,
                               use_other_treat_as_covariate,
                               force_all_x_finite)
         self._check_disjoint_sets_cluster_cols()
 
     def __str__(self):
         data_summary = self._data_summary_str()
         buf = io.StringIO()
@@ -663,20 +752,23 @@
         return res
 
     def _data_summary_str(self):
         data_summary = f'Outcome variable: {self.y_col}\n' \
                        f'Treatment variable(s): {self.d_cols}\n' \
                        f'Cluster variable(s): {self.cluster_cols}\n' \
                        f'Covariates: {self.x_cols}\n' \
-                       f'Instrument variable(s): {self.z_cols}\n' \
-                       f'No. Observations: {self.n_obs}\n'
+                       f'Instrument variable(s): {self.z_cols}\n'
+        if self.t_col is not None:
+            data_summary += f'Time variable: {self.t_col}\n'
+
+        data_summary += f'No. Observations: {self.n_obs}\n'
         return data_summary
 
     @classmethod
-    def from_arrays(cls, x, y, d, cluster_vars, z=None, use_other_treat_as_covariate=True,
+    def from_arrays(cls, x, y, d, cluster_vars, z=None, t=None, use_other_treat_as_covariate=True,
                     force_all_x_finite=True):
         """
         Initialize :class:`DoubleMLClusterData` from :class:`numpy.ndarray`'s.
 
         Parameters
         ----------
         x : :class:`numpy.ndarray`
@@ -691,14 +783,18 @@
         cluster_vars : :class:`numpy.ndarray`
             Array of cluster variables.
 
         z : None or :class:`numpy.ndarray`
             Array of instrumental variables.
             Default is ``None``.
 
+        t : :class:`numpy.ndarray`
+            Array of the time variable (only relevant/used for DiD models).
+            Default is ``None``.
+
         use_other_treat_as_covariate : bool
             Indicates whether in the multiple-treatment case the other treatment variables should be added as covariates.
             Default is ``True``.
 
         force_all_x_finite : bool or str
             Indicates whether to raise an error on infinite values and / or missings in the covariates ``x``.
             Possible values are: ``True`` (neither missings ``np.nan``, ``pd.NA`` nor infinite values ``np.inf`` are
@@ -711,26 +807,26 @@
         Examples
         --------
         >>> from doubleml import DoubleMLClusterData
         >>> from doubleml.datasets import make_pliv_multiway_cluster_CKMS2021
         >>> (x, y, d, cluster_vars, z) = make_pliv_multiway_cluster_CKMS2021(return_type='array')
         >>> obj_dml_data_from_array = DoubleMLClusterData.from_arrays(x, y, d, cluster_vars, z)
         """
-        dml_data = DoubleMLData.from_arrays(x, y, d, z, use_other_treat_as_covariate, force_all_x_finite)
+        dml_data = DoubleMLData.from_arrays(x, y, d, z, t, use_other_treat_as_covariate, force_all_x_finite)
         cluster_vars = check_array(cluster_vars, ensure_2d=False, allow_nd=False)
         cluster_vars = _assure_2d_array(cluster_vars)
         if cluster_vars.shape[1] == 1:
             cluster_cols = ['cluster_var']
         else:
             cluster_cols = [f'cluster_var{i + 1}' for i in np.arange(cluster_vars.shape[1])]
 
         data = pd.concat((pd.DataFrame(cluster_vars, columns=cluster_cols), dml_data.data), axis=1)
 
         return (cls(data, dml_data.y_col, dml_data.d_cols, cluster_cols,
-                    dml_data.x_cols, dml_data.z_cols,
+                    dml_data.x_cols, dml_data.z_cols, dml_data.t_col,
                     dml_data.use_other_treat_as_covariate, dml_data.force_all_x_finite))
 
     @property
     def cluster_cols(self):
         """
         The cluster variable(s).
         """
@@ -771,17 +867,23 @@
 
     @DoubleMLData.x_cols.setter
     def x_cols(self, value):
         if value is not None:
             # this call might become much easier with https://github.com/python/cpython/pull/26194
             super(self.__class__, self.__class__).x_cols.__set__(self, value)
         else:
-            if self.z_cols is not None:
+            if (self.z_cols is not None) & (self.t_col is not None):
+                y_d_z_t = set.union({self.y_col}, set(self.d_cols), set(self.z_cols), {self.t_col}, set(self.cluster_cols))
+                x_cols = [col for col in self.data.columns if col not in y_d_z_t]
+            elif self.z_cols is not None:
                 y_d_z = set.union({self.y_col}, set(self.d_cols), set(self.z_cols), set(self.cluster_cols))
                 x_cols = [col for col in self.data.columns if col not in y_d_z]
+            elif self.t_col is not None:
+                y_d_t = set.union({self.y_col}, set(self.d_cols), {self.t_col}, set(self.cluster_cols))
+                x_cols = [col for col in self.data.columns if col not in y_d_t]
             else:
                 y_d = set.union({self.y_col}, set(self.d_cols), set(self.cluster_cols))
                 x_cols = [col for col in self.data.columns if col not in y_d]
             # this call might become much easier with https://github.com/python/cpython/pull/26194
             super(self.__class__, self.__class__).x_cols.__set__(self, x_cols)
 
     def _check_disjoint_sets(self):
@@ -794,14 +896,15 @@
         super(DoubleMLClusterData, self)._check_disjoint_sets()
 
         # special checks for the additional cluster variables
         cluster_cols_set = set(self.cluster_cols)
         y_col_set = {self.y_col}
         x_cols_set = set(self.x_cols)
         d_cols_set = set(self.d_cols)
+        t_col_set = {self.t_col}
 
         if not y_col_set.isdisjoint(cluster_cols_set):
             raise ValueError(f'{str(self.y_col)} cannot be set as outcome variable ``y_col`` and cluster '
                              'variable in ``cluster_cols``.')
         if not d_cols_set.isdisjoint(cluster_cols_set):
             raise ValueError('At least one variable/column is set as treatment variable (``d_cols``) and '
                              'cluster variable in ``cluster_cols``.')
@@ -810,11 +913,15 @@
             raise ValueError('At least one variable/column is set as covariate (``x_cols``) and cluster '
                              'variable in ``cluster_cols``.')
         if self.z_cols is not None:
             z_cols_set = set(self.z_cols)
             if not z_cols_set.isdisjoint(cluster_cols_set):
                 raise ValueError('At least one variable/column is set as instrumental variable (``z_cols``) and '
                                  'cluster variable in ``cluster_cols``.')
+        if self.t_col is not None:
+            if not t_col_set.isdisjoint(cluster_cols_set):
+                raise ValueError(f'{str(self.t_col)} cannot be set as time variable ``t_col`` and '
+                                 'cluster variable in ``cluster_cols``.')
 
     def _set_cluster_vars(self):
         assert_all_finite(self.data.loc[:, self.cluster_cols])
         self._cluster_vars = self.data.loc[:, self.cluster_cols]
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_iivm.py` & `DoubleML-0.6.1/doubleml/double_ml_iivm.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from sklearn.utils import check_X_y
 from sklearn.utils.multiclass import type_of_target
 
 from .double_ml import DoubleML
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
 from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _check_finite_predictions, _check_is_propensity, \
-    _trimm, _normalize_ipw
+    _trimm, _normalize_ipw, _check_score, _check_trimming
 
 
 class DoubleMLIIVM(LinearScoreMixin, DoubleML):
     """Double machine learning for interactive IV regression models
 
     Parameters
     ----------
@@ -143,15 +143,17 @@
                          n_rep,
                          score,
                          dml_procedure,
                          draw_sample_splitting,
                          apply_cross_fitting)
 
         self._check_data(self._dml_data)
-        self._check_score(self.score)
+        valid_scores = ['LATE']
+        _check_score(self.score, valid_scores, allow_callable=True)
+
         # set stratication for resampling
         self._strata = self._dml_data.d.reshape(-1, 1) + 2 * self._dml_data.z.reshape(-1, 1)
         ml_g_is_classifier = self._check_learner(ml_g, 'ml_g', regressor=True, classifier=True)
         _ = self._check_learner(ml_m, 'ml_m', regressor=False, classifier=True)
         _ = self._check_learner(ml_r, 'ml_r', regressor=False, classifier=True)
         self._learner = {'ml_g': ml_g, 'ml_m': ml_m, 'ml_r': ml_r}
         self._normalize_ipw = normalize_ipw
@@ -161,18 +163,20 @@
             else:
                 raise ValueError(f'The ml_g learner {str(ml_g)} was identified as classifier '
                                  'but the outcome variable is not binary with values 0 and 1.')
         else:
             self._predict_method = {'ml_g': 'predict', 'ml_m': 'predict_proba', 'ml_r': 'predict_proba'}
         self._initialize_ml_nuisance_params()
 
-        valid_trimming_rule = ['truncate']
-        if trimming_rule not in valid_trimming_rule:
-            raise ValueError('Invalid trimming_rule ' + trimming_rule + '. ' +
-                             'Valid trimming_rule ' + ' or '.join(valid_trimming_rule) + '.')
+        if not isinstance(self.normalize_ipw, bool):
+            raise TypeError('Normalization indicator has to be boolean. ' +
+                            f'Object of type {str(type(self.normalize_ipw))} passed.')
+        self._trimming_rule = trimming_rule
+        self._trimming_threshold = trimming_threshold
+        _check_trimming(self._trimming_rule, self._trimming_threshold)
 
         if subgroups is None:
             # this is the default for subgroups; via None to prevent a mutable default argument
             subgroups = {'always_takers': True, 'never_takers': True}
         else:
             if not isinstance(subgroups, dict):
                 raise TypeError('Invalid subgroups ' + str(subgroups) + '. ' +
@@ -184,41 +188,41 @@
             if not isinstance(subgroups['always_takers'], bool):
                 raise TypeError("subgroups['always_takers'] must be True or False. "
                                 f'Got {str(subgroups["always_takers"])}.')
             if not isinstance(subgroups['never_takers'], bool):
                 raise TypeError("subgroups['never_takers'] must be True or False. "
                                 f'Got {str(subgroups["never_takers"])}.')
         self.subgroups = subgroups
-        self.trimming_rule = trimming_rule
-        self.trimming_threshold = trimming_threshold
 
     @property
     def normalize_ipw(self):
         """
         Indicates whether the inverse probability weights are normalized.
         """
         return self._normalize_ipw
 
+    @property
+    def trimming_rule(self):
+        """
+        Specifies the used trimming rule.
+        """
+        return self._trimming_rule
+
+    @property
+    def trimming_threshold(self):
+        """
+        Specifies the used trimming threshold.
+        """
+        return self._trimming_threshold
+
     def _initialize_ml_nuisance_params(self):
         valid_learner = ['ml_g0', 'ml_g1', 'ml_m', 'ml_r0', 'ml_r1']
         self._params = {learner: {key: [None] * self.n_rep for key in self._dml_data.d_cols}
                         for learner in valid_learner}
 
-    def _check_score(self, score):
-        if isinstance(score, str):
-            valid_score = ['LATE']
-            if score not in valid_score:
-                raise ValueError('Invalid score ' + score + '. '
-                                 'Valid score ' + ' or '.join(valid_score) + '.')
-        else:
-            if not callable(score):
-                raise TypeError('score should be either a string or a callable. '
-                                '%r was passed.' % score)
-        return
-
     def _check_data(self, obj_dml_data):
         if not isinstance(obj_dml_data, DoubleMLData):
             raise TypeError('The data must be of DoubleMLData type. '
                             f'{str(obj_dml_data)} of type {str(type(obj_dml_data))} was passed.')
         one_treat = (obj_dml_data.n_treat == 1)
         binary_treat = (type_of_target(obj_dml_data.d) == 'binary')
         zero_one_treat = np.all((np.power(obj_dml_data.d, 2) - obj_dml_data.d) == 0)
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_irm.py` & `DoubleML-0.6.1/doubleml/double_ml_irm.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .double_ml import DoubleML
 
 from .double_ml_blp import DoubleMLBLP
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
 
 from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _check_finite_predictions, _check_is_propensity, \
-    _trimm, _normalize_ipw
+    _trimm, _normalize_ipw, _check_score, _check_trimming
 
 
 class DoubleMLIRM(LinearScoreMixin, DoubleML):
     """Double machine learning for interactive regression models
 
     Parameters
     ----------
@@ -128,15 +128,17 @@
                          n_rep,
                          score,
                          dml_procedure,
                          draw_sample_splitting,
                          apply_cross_fitting)
 
         self._check_data(self._dml_data)
-        self._check_score(self.score)
+        valid_scores = ['ATE', 'ATTE']
+        _check_score(self.score, valid_scores, allow_callable=True)
+
         # set stratication for resampling
         self._strata = self._dml_data.d
         ml_g_is_classifier = self._check_learner(ml_g, 'ml_g', regressor=True, classifier=True)
         _ = self._check_learner(ml_m, 'ml_m', regressor=False, classifier=True)
         self._learner = {'ml_g': ml_g, 'ml_m': ml_m}
         self._normalize_ipw = normalize_ipw
         if ml_g_is_classifier:
@@ -145,45 +147,47 @@
             else:
                 raise ValueError(f'The ml_g learner {str(ml_g)} was identified as classifier '
                                  'but the outcome variable is not binary with values 0 and 1.')
         else:
             self._predict_method = {'ml_g': 'predict', 'ml_m': 'predict_proba'}
         self._initialize_ml_nuisance_params()
 
-        valid_trimming_rule = ['truncate']
-        if trimming_rule not in valid_trimming_rule:
-            raise ValueError('Invalid trimming_rule ' + trimming_rule + '. ' +
-                             'Valid trimming_rule ' + ' or '.join(valid_trimming_rule) + '.')
-        self.trimming_rule = trimming_rule
-        self.trimming_threshold = trimming_threshold
+        if not isinstance(self.normalize_ipw, bool):
+            raise TypeError('Normalization indicator has to be boolean. ' +
+                            f'Object of type {str(type(self.normalize_ipw))} passed.')
+        self._trimming_rule = trimming_rule
+        self._trimming_threshold = trimming_threshold
+        _check_trimming(self._trimming_rule, self._trimming_threshold)
 
     @property
     def normalize_ipw(self):
         """
         Indicates whether the inverse probability weights are normalized.
         """
         return self._normalize_ipw
 
+    @property
+    def trimming_rule(self):
+        """
+        Specifies the used trimming rule.
+        """
+        return self._trimming_rule
+
+    @property
+    def trimming_threshold(self):
+        """
+        Specifies the used trimming threshold.
+        """
+        return self._trimming_threshold
+
     def _initialize_ml_nuisance_params(self):
         valid_learner = ['ml_g0', 'ml_g1', 'ml_m']
         self._params = {learner: {key: [None] * self.n_rep for key in self._dml_data.d_cols}
                         for learner in valid_learner}
 
-    def _check_score(self, score):
-        if isinstance(score, str):
-            valid_score = ['ATE', 'ATTE']
-            if score not in valid_score:
-                raise ValueError('Invalid score ' + score + '. ' +
-                                 'Valid score ' + ' or '.join(valid_score) + '.')
-        else:
-            if not callable(score):
-                raise TypeError('score should be either a string or a callable. '
-                                '%r was passed.' % score)
-        return
-
     def _check_data(self, obj_dml_data):
         if not isinstance(obj_dml_data, DoubleMLData):
             raise TypeError('The data must be of DoubleMLData type. '
                             f'{str(obj_dml_data)} of type {str(type(obj_dml_data))} was passed.')
         if obj_dml_data.z_cols is not None:
             raise ValueError('Incompatible data. ' +
                              ' and '.join(obj_dml_data.z_cols) +
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_lpq.py` & `DoubleML-0.6.1/doubleml/double_ml_lpq.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                                 '%r was passed.' % kde)
             self._kde = kde
         self._normalize_ipw = normalize_ipw
 
         self._check_data(self._dml_data)
 
         valid_score = ['LPQ']
-        _check_score(self.score, valid_score)
+        _check_score(self.score, valid_score, allow_callable=False)
         _check_quantile(self.quantile)
         _check_treatment(self.treatment)
 
         if not isinstance(self.normalize_ipw, bool):
             raise TypeError('Normalization indicator has to be boolean. ' +
                             f'Object of type {str(type(self.normalize_ipw))} passed.')
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_pliv.py` & `DoubleML-0.6.1/doubleml/double_ml_pliv.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/double_ml_plr.py` & `DoubleML-0.6.1/doubleml/double_ml_plr.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sklearn.base import clone
 
 import warnings
 
 from .double_ml import DoubleML
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
-from ._utils import _dml_cv_predict, _dml_tune, _check_finite_predictions, _check_is_propensity
+from ._utils import _dml_cv_predict, _dml_tune, _check_finite_predictions, _check_is_propensity, _check_score
 
 
 class DoubleMLPLR(LinearScoreMixin, DoubleML):
     """Double machine learning for partially linear regression models
 
     Parameters
     ----------
@@ -110,15 +110,16 @@
                          n_rep,
                          score,
                          dml_procedure,
                          draw_sample_splitting,
                          apply_cross_fitting)
 
         self._check_data(self._dml_data)
-        self._check_score(self.score)
+        valid_scores = ['IV-type', 'partialling out']
+        _check_score(self.score, valid_scores, allow_callable=True)
 
         _ = self._check_learner(ml_l, 'ml_l', regressor=True, classifier=False)
         ml_m_is_classifier = self._check_learner(ml_m, 'ml_m', regressor=True, classifier=True)
         self._learner = {'ml_l': ml_l, 'ml_m': ml_m}
 
         if ml_g is not None:
             if (isinstance(self.score, str) & (self.score == 'IV-type')) | callable(self.score):
@@ -147,26 +148,14 @@
 
         self._initialize_ml_nuisance_params()
 
     def _initialize_ml_nuisance_params(self):
         self._params = {learner: {key: [None] * self.n_rep for key in self._dml_data.d_cols}
                         for learner in self._learner}
 
-    def _check_score(self, score):
-        if isinstance(score, str):
-            valid_score = ['IV-type', 'partialling out']
-            if score not in valid_score:
-                raise ValueError('Invalid score ' + score + '. ' +
-                                 'Valid score ' + ' or '.join(valid_score) + '.')
-        else:
-            if not callable(score):
-                raise TypeError('score should be either a string or a callable. '
-                                '%r was passed.' % score)
-        return
-
     def _check_data(self, obj_dml_data):
         if not isinstance(obj_dml_data, DoubleMLData):
             raise TypeError('The data must be of DoubleMLData type. '
                             f'{str(obj_dml_data)} of type {str(type(obj_dml_data))} was passed.')
         if obj_dml_data.z_cols is not None:
             raise ValueError('Incompatible data. ' +
                              ' and '.join(obj_dml_data.z_cols) +
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_pq.py` & `DoubleML-0.6.1/doubleml/double_ml_pq.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                                 '%r was passed.' % kde)
             self._kde = kde
 
         self._normalize_ipw = normalize_ipw
         self._check_data(self._dml_data)
 
         valid_score = ['PQ']
-        _check_score(self.score, valid_score)
+        _check_score(self.score, valid_score, allow_callable=False)
         _check_quantile(self.quantile)
         _check_treatment(self.treatment)
 
         if not isinstance(self.normalize_ipw, bool):
             raise TypeError('Normalization indicator has to be boolean. ' +
                             f'Object of type {str(type(self.normalize_ipw))} passed.')
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_qte.py` & `DoubleML-0.6.1/doubleml/double_ml_qte.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         self._n_folds = n_folds
         self._n_rep = n_rep
         self._dml_procedure = dml_procedure
 
         # check score
         self._score = score
         valid_scores = ['PQ', 'LPQ', 'CVaR']
-        _check_score(self.score, valid_scores)
+        _check_score(self.score, valid_scores, allow_callable=False)
 
         # check data
         self._is_cluster_data = False
         if isinstance(obj_dml_data, DoubleMLClusterData):
             self._is_cluster_data = True
         self._check_data(self._dml_data)
 
@@ -563,15 +563,15 @@
 
         if not isinstance(joint, bool):
             raise TypeError('joint must be True or False. '
                             f'Got {str(joint)}.')
 
         if not isinstance(level, float):
             raise TypeError('The confidence level must be of float type. '
-                            f'Object of type {str(type(level))} was passed.')
+                            f'{str(level)} of type {str(type(level))} was passed.')
         if (level <= 0) | (level >= 1):
             raise ValueError('The confidence level must be in (0,1). '
                              f'{str(level)} was passed.')
 
         a = (1 - level)
         ab = np.array([a / 2, 1. - a / 2])
         if joint:
```

### Comparing `DoubleML-0.6.0/doubleml/double_ml_score_mixins.py` & `DoubleML-0.6.1/doubleml/double_ml_score_mixins.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils.py` & `DoubleML-0.6.1/doubleml/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_blp_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_blp_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_boot.py` & `DoubleML-0.6.1/doubleml/tests/_utils_boot.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_cluster.py` & `DoubleML-0.6.1/doubleml/tests/_utils_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_cvar_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_cvar_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_dml_cv_predict.py` & `DoubleML-0.6.1/doubleml/tests/_utils_dml_cv_predict.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_iivm_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_iivm_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_irm_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_irm_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_lpq_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_lpq_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_pliv_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_pliv_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_pliv_partial_x_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_x_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_pliv_partial_xz_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_xz_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_pliv_partial_z_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_z_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_plr_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_plr_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_pq_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_pq_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/_utils_qte_manual.py` & `DoubleML-0.6.1/doubleml/tests/_utils_qte_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/conftest.py` & `DoubleML-0.6.1/doubleml/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import pytest
 from scipy.linalg import toeplitz
 
 from sklearn.datasets import make_spd_matrix
 from sklearn.datasets import make_regression, make_classification
 
-from doubleml.datasets import make_plr_turrell2018, make_irm_data, make_iivm_data, make_pliv_CHS2015
+from doubleml.datasets import make_plr_turrell2018, make_irm_data, make_iivm_data, make_pliv_CHS2015, \
+    make_did_SZ2020
 
 
 def _g(x):
     return np.power(np.sin(x), 2)
 
 
 def _m(x, nu=0., gamma=1.):
@@ -409,7 +410,41 @@
     d = generate_treatment(z, x, x_conf)
     epsilon = np.random.normal(size=n)
 
     y = f_loc(d, x, x_conf) + f_scale(d, x, x_conf)*epsilon
     data = (x, y, d, z)
 
     return data
+
+
+@pytest.fixture(scope='session',
+                params=[(500, 1),
+                        (1000, 1),
+                        (1000, 2)])
+def generate_data_did(request):
+    params = request.param
+    np.random.seed(1111)
+    # setting parameters
+    n = params[0]
+    dpg = params[1]
+
+    # generating data
+    data = make_did_SZ2020(n, dgp_type=dpg, return_type='array')
+
+    return data
+
+
+@pytest.fixture(scope='session',
+                params=[(500, 1),
+                        (1000, 1),
+                        (1000, 2)])
+def generate_data_did_cs(request):
+    params = request.param
+    np.random.seed(1111)
+    # setting parameters
+    n = params[0]
+    dpg = params[1]
+
+    # generating data
+    data = make_did_SZ2020(n, dgp_type=dpg, cross_sectional_data=True, return_type='array')
+
+    return data
```

### Comparing `DoubleML-0.6.0/doubleml/tests/test_blp.py` & `DoubleML-0.6.1/doubleml/tests/test_blp.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_cv_predict.py` & `DoubleML-0.6.1/doubleml/tests/test_cv_predict.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_cvar.py` & `DoubleML-0.6.1/doubleml/tests/test_cvar.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_cvar_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_cvar_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_datasets.py` & `DoubleML-0.6.1/doubleml/tests/test_datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 import pandas as pd
 import numpy as np
 
 from doubleml import DoubleMLData, DoubleMLClusterData
 from doubleml.datasets import fetch_401K, fetch_bonus, make_plr_CCDDHNR2018, make_plr_turrell2018, \
-    make_irm_data, make_iivm_data, _make_pliv_data, make_pliv_CHS2015, make_pliv_multiway_cluster_CKMS2021
+    make_irm_data, make_iivm_data, _make_pliv_data, make_pliv_CHS2015, make_pliv_multiway_cluster_CKMS2021, \
+    make_did_SZ2020
 
 msg_inv_return_type = 'Invalid return_type.'
 
 
 def test_fetch_401K_return_types():
     res = fetch_401K('DoubleMLData')
     assert isinstance(res, DoubleMLData)
@@ -144,7 +145,42 @@
     assert isinstance(x, np.ndarray)
     assert isinstance(y, np.ndarray)
     assert isinstance(d, np.ndarray)
     assert isinstance(cluster_vars, np.ndarray)
     assert isinstance(z, np.ndarray)
     with pytest.raises(ValueError, match=msg_inv_return_type):
         _ = make_pliv_multiway_cluster_CKMS2021(N=10, M=10, return_type='matrix')
+
+
+@pytest.fixture(scope='function',
+                params=[False, True])
+def cross_sectional(request):
+    return request.param
+
+
+@pytest.fixture(scope='function',
+                params=[1, 2, 3, 4, 5, 6])
+def dgp_type(request):
+    return request.param
+
+
+@pytest.mark.ci
+def test_make_did_SZ2020_return_types(cross_sectional, dgp_type):
+    np.random.seed(3141)
+    res = make_did_SZ2020(n_obs=100, dgp_type=dgp_type, cross_sectional_data=cross_sectional, return_type=DoubleMLData)
+    assert isinstance(res, DoubleMLData)
+    res = make_did_SZ2020(n_obs=100, dgp_type=dgp_type, cross_sectional_data=cross_sectional, return_type=pd.DataFrame)
+    assert isinstance(res, pd.DataFrame)
+    if cross_sectional:
+        x, y, d, t = make_did_SZ2020(n_obs=100, dgp_type=dgp_type, cross_sectional_data=cross_sectional,
+                                     return_type=np.ndarray)
+        assert isinstance(t, np.ndarray)
+    else:
+        x, y, d = make_did_SZ2020(n_obs=100, dgp_type=dgp_type, cross_sectional_data=cross_sectional, return_type=np.ndarray)
+    assert isinstance(x, np.ndarray)
+    assert isinstance(y, np.ndarray)
+    assert isinstance(d, np.ndarray)
+    with pytest.raises(ValueError, match=msg_inv_return_type):
+        _ = make_did_SZ2020(n_obs=100, dgp_type=dgp_type, cross_sectional_data=cross_sectional, return_type='matrix')
+    msg = 'The dgp_type is not valid.'
+    with pytest.raises(ValueError, match=msg):
+        _ = make_did_SZ2020(n_obs=100, dgp_type="5", cross_sectional_data=cross_sectional, return_type='matrix')
```

### Comparing `DoubleML-0.6.0/doubleml/tests/test_dml_data.py` & `DoubleML-0.6.1/doubleml/tests/test_dml_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import numpy as np
 import pandas as pd
 
-from doubleml import DoubleMLData, DoubleMLPLR, DoubleMLClusterData
+from doubleml import DoubleMLData, DoubleMLPLR, DoubleMLClusterData, DoubleMLDIDCS
 from doubleml.datasets import make_plr_CCDDHNR2018, _make_pliv_data, make_pliv_CHS2015,\
-    make_pliv_multiway_cluster_CKMS2021
-from sklearn.linear_model import Lasso
+    make_pliv_multiway_cluster_CKMS2021, make_did_SZ2020
+from sklearn.linear_model import Lasso, LogisticRegression
 
 
 @pytest.fixture(scope="module")
 def dml_data_fixture(generate_data1):
     data = generate_data1
     np.random.seed(3141)
     x_cols = data.columns[data.columns.str.startswith('X')].tolist()
@@ -72,14 +72,37 @@
     df.columns = [f'X{i+1}' for i in np.arange(7)] + ['y', 'd1', 'd2']
     dml_data = DoubleMLData(df, 'y', ['d1', 'd2'], [f'X{i+1}' for i in np.arange(7)])
     dml_data_from_array = DoubleMLData.from_arrays(dml_data.data[dml_data.x_cols],
                                                    dml_data.data[dml_data.y_col],
                                                    dml_data.data[dml_data.d_cols])
     assert np.array_equal(dml_data_from_array.data, dml_data.data)
 
+    dml_data = make_did_SZ2020(n_obs=100, cross_sectional_data=False)
+    dml_data_from_array = DoubleMLData.from_arrays(x=dml_data.data[dml_data.x_cols],
+                                                   y=dml_data.data[dml_data.y_col],
+                                                   d=dml_data.data[dml_data.d_cols])
+    assert np.array_equal(dml_data_from_array.data, dml_data.data)
+
+    dml_data = make_did_SZ2020(n_obs=100, cross_sectional_data=True)
+    dml_data_from_array = DoubleMLData.from_arrays(x=dml_data.data[dml_data.x_cols],
+                                                   y=dml_data.data[dml_data.y_col],
+                                                   d=dml_data.data[dml_data.d_cols],
+                                                   t=dml_data.data[dml_data.t_col])
+    assert np.array_equal(dml_data_from_array.data, dml_data.data)
+
+    # check with instrument and time variable
+    dml_data = make_did_SZ2020(n_obs=100, cross_sectional_data=True)
+    dml_data.data['z'] = dml_data.data['t']
+    dml_data_from_array = DoubleMLData.from_arrays(x=dml_data.data[dml_data.x_cols],
+                                                   y=dml_data.data[dml_data.y_col],
+                                                   d=dml_data.data[dml_data.d_cols],
+                                                   z=dml_data.data['z'],
+                                                   t=dml_data.data[dml_data.t_col])
+    assert np.array_equal(dml_data_from_array.data, dml_data.data)
+
     dml_data = make_pliv_multiway_cluster_CKMS2021(N=10, M=10)
     dml_data_from_array = DoubleMLClusterData.from_arrays(dml_data.data[dml_data.x_cols],
                                                           dml_data.data[dml_data.y_col],
                                                           dml_data.data[dml_data.d_cols],
                                                           dml_data.data[dml_data.cluster_cols],
                                                           dml_data.data[dml_data.z_cols])
     df = dml_data.data.copy()
@@ -115,49 +138,92 @@
     dml_plr_full_df.fit()
     dml_plr_subset.fit()
     assert np.allclose(dml_plr_full_df.coef, dml_plr_subset.coef, rtol=1e-9, atol=1e-4)
     assert np.allclose(dml_plr_full_df.se, dml_plr_subset.se, rtol=1e-9, atol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_data_no_instr():
+def test_dml_data_no_instr_no_time():
     np.random.seed(3141)
     dml_data = make_plr_CCDDHNR2018(n_obs=100)
     assert dml_data.z is None
     assert dml_data.n_instr == 0
+    assert dml_data.t is None
 
     x, y, d = make_plr_CCDDHNR2018(n_obs=100, return_type='array')
     dml_data = DoubleMLData.from_arrays(x, y, d)
     assert dml_data.z is None
     assert dml_data.n_instr == 0
+    assert dml_data.t is None
+
+
+@pytest.mark.ci
+def test_dml_cluster_summary_with_time():
+    dml_data_did_cs = make_did_SZ2020(n_obs=200, cross_sectional_data=True)
+    dml_did_cs = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression())
+    assert isinstance(dml_did_cs.__str__(), str)
+    assert isinstance(dml_did_cs.summary, pd.DataFrame)
 
 
 @pytest.mark.ci
 def test_x_cols_setter_defaults():
     df = pd.DataFrame(np.tile(np.arange(4), (4, 1)),
                       columns=['yy', 'dd', 'xx1', 'xx2'])
     dml_data = DoubleMLData(df, y_col='yy', d_cols='dd')
     assert dml_data.x_cols == ['xx1', 'xx2']
 
+    # with instrument
+    df = pd.DataFrame(np.tile(np.arange(5), (4, 1)),
+                      columns=['yy', 'dd', 'xx1', 'xx2', 'zz'])
+    dml_data = DoubleMLData(df, y_col='yy', d_cols='dd', z_cols='zz')
+    assert dml_data.x_cols == ['xx1', 'xx2']
+
+    # without instrument with time
+    df = pd.DataFrame(np.tile(np.arange(5), (4, 1)),
+                      columns=['yy', 'dd', 'xx1', 'xx2', 'tt'])
+    dml_data = DoubleMLData(df, y_col='yy', d_cols='dd', t_col='tt')
+    assert dml_data.x_cols == ['xx1', 'xx2']
+
+    # with instrument with time
+    df = pd.DataFrame(np.tile(np.arange(6), (4, 1)),
+                      columns=['yy', 'dd', 'xx1', 'xx2', 'zz', 'tt'])
+    dml_data = DoubleMLData(df, y_col='yy', d_cols='dd', z_cols='zz', t_col='tt')
+    assert dml_data.x_cols == ['xx1', 'xx2']
+
 
 @pytest.mark.ci
 def test_x_cols_setter_defaults_w_cluster():
     df = pd.DataFrame(np.tile(np.arange(6), (6, 1)),
                       columns=['yy', 'dd', 'xx1', 'xx2', 'xx3', 'cluster1'])
     dml_data = DoubleMLClusterData(df, y_col='yy', d_cols='dd', cluster_cols='cluster1')
     assert dml_data.x_cols == ['xx1', 'xx2', 'xx3']
     dml_data.x_cols = ['xx1', 'xx3']
     assert dml_data.x_cols == ['xx1', 'xx3']
     dml_data.x_cols = None
     assert dml_data.x_cols == ['xx1', 'xx2', 'xx3']
+
+    # with instrument
     df = pd.DataFrame(np.tile(np.arange(6), (6, 1)),
                       columns=['yy', 'dd', 'xx1', 'xx2', 'z', 'cluster1'])
     dml_data = DoubleMLClusterData(df, y_col='yy', d_cols='dd', cluster_cols='cluster1', z_cols='z')
     assert dml_data.x_cols == ['xx1', 'xx2']
 
+    # without instrument and with time
+    df = pd.DataFrame(np.tile(np.arange(6), (6, 1)),
+                      columns=['yy', 'dd', 'xx1', 'xx2', 'tt', 'cluster1'])
+    dml_data = DoubleMLClusterData(df, y_col='yy', d_cols='dd', cluster_cols='cluster1', t_col='tt')
+    assert dml_data.x_cols == ['xx1', 'xx2']
+
+    # with instrument and with time
+    df = pd.DataFrame(np.tile(np.arange(7), (6, 1)),
+                      columns=['yy', 'dd', 'xx1', 'xx2', 'zz', 'tt', 'cluster1'])
+    dml_data = DoubleMLClusterData(df, y_col='yy', d_cols='dd', cluster_cols='cluster1',
+                                   z_cols='zz', t_col='tt')
+    assert dml_data.x_cols == ['xx1', 'xx2']
+
 
 @pytest.mark.ci
 def test_x_cols_setter():
     np.random.seed(3141)
     dml_data = make_plr_CCDDHNR2018(n_obs=100)
     orig_x_cols = dml_data.x_cols
 
@@ -251,14 +317,42 @@
     # check None
     dml_data.z_cols = None
     assert dml_data.n_instr == 0
     assert dml_data.z is None
 
 
 @pytest.mark.ci
+def test_t_col_setter():
+    np.random.seed(3141)
+    df = make_did_SZ2020(n_obs=100, cross_sectional_data=True, return_type=pd.DataFrame)
+    df['t_new'] = np.ones(shape=(100,))
+    dml_data = DoubleMLData(df, 'y', 'd',
+                            [f'Z{i + 1}' for i in np.arange(4)],
+                            t_col='t')
+
+    # check that after changing t_col, the t array gets updated
+    t_comp = dml_data.data['t_new'].values
+    dml_data.t_col = 't_new'
+    assert np.array_equal(dml_data.t, t_comp)
+
+    msg = r'Invalid time variable t_col. a13 is no data column.'
+    with pytest.raises(ValueError, match=msg):
+        dml_data.t_col = 'a13'
+
+    msg = (r'The time variable t_col must be of str type \(or None\). '
+           "5 of type <class 'int'> was passed.")
+    with pytest.raises(TypeError, match=msg):
+        dml_data.t_col = 5
+
+    # check None
+    dml_data.t_col = None
+    assert dml_data.t is None
+
+
+@pytest.mark.ci
 def test_cluster_cols_setter():
     np.random.seed(3141)
     dml_data = make_plr_CCDDHNR2018(n_obs=100)
     df = dml_data.data.copy().iloc[:, :10]
     df.columns = [f'X{i + 1}' for i in np.arange(7)] + ['y', 'd1', 'd2']
     dml_data = DoubleMLClusterData(df, 'y', ['d1', 'd2'],
                                    cluster_cols=[f'X{i + 1}' for i in [5, 6]],
@@ -379,15 +473,25 @@
            '``z_cols``.')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], z_cols=['dd1'])
     msg = (r'At least one variable/column is set as covariate \(``x_cols``\) and instrumental variable in '
            '``z_cols``.')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], z_cols='xx2')
+    msg = 'xx2 cannot be set as time variable ``t_col`` and covariate in ``x_cols``.'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], t_col='xx2')
+    msg = 'dd1 cannot be set as time variable ``t_col`` and treatment variable in ``d_cols``.'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], t_col='dd1')
+    msg = 'yy cannot be set as time variable ``t_col`` and outcome variable ``y_col``.'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], t_col='yy')
 
+    # cluster data
     msg = 'yy cannot be set as outcome variable ``y_col`` and cluster variable in ``cluster_cols``'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLClusterData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], cluster_cols='yy')
     msg = (r'At least one variable/column is set as treatment variable \(``d_cols``\) and cluster variable in '
            '``cluster_cols``.')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLClusterData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], cluster_cols='dd1')
@@ -395,14 +499,17 @@
            '``cluster_cols``.')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLClusterData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1', 'xx2'], cluster_cols='xx2')
     msg = (r'At least one variable/column is set as instrumental variable \(``z_cols``\) and cluster variable in '
            '``cluster_cols``.')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLClusterData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1'], z_cols=['xx2'], cluster_cols='xx2')
+    msg = 'xx2 cannot be set as time variable ``t_col`` and cluster variable in ``cluster_cols``.'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLClusterData(df, y_col='yy', d_cols=['dd1'], x_cols=['xx1'], t_col='xx2', cluster_cols='xx2')
 
 
 @pytest.mark.ci
 def test_duplicates():
     np.random.seed(3141)
     dml_data = make_plr_CCDDHNR2018(n_obs=100)
     dml_cluster_data = make_pliv_multiway_cluster_CKMS2021(N=10, M=10)
```

### Comparing `DoubleML-0.6.0/doubleml/tests/test_doubleml_evaluate_learner.py` & `DoubleML-0.6.1/doubleml/tests/test_doubleml_evaluate_learner.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_doubleml_exceptions.py` & `DoubleML-0.6.1/doubleml/tests/test_doubleml_exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import pandas as pd
 import numpy as np
 
 from doubleml import DoubleMLPLR, DoubleMLIRM, DoubleMLIIVM, DoubleMLPLIV, DoubleMLData,\
-    DoubleMLClusterData, DoubleMLPQ, DoubleMLLPQ, DoubleMLCVAR, DoubleMLQTE
+    DoubleMLClusterData, DoubleMLPQ, DoubleMLLPQ, DoubleMLCVAR, DoubleMLQTE, DoubleMLDID, DoubleMLDIDCS
 from doubleml.datasets import make_plr_CCDDHNR2018, make_irm_data, make_pliv_CHS2015, make_iivm_data, \
-    make_pliv_multiway_cluster_CKMS2021
+    make_pliv_multiway_cluster_CKMS2021, make_did_SZ2020
 from doubleml.double_ml_data import DoubleMLBaseData
 
 from sklearn.linear_model import Lasso, LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.base import BaseEstimator
 
 np.random.seed(3141)
@@ -24,14 +24,16 @@
 
 dml_data_pliv = make_pliv_CHS2015(n_obs=n, dim_z=1)
 dml_pliv = DoubleMLPLIV(dml_data_pliv, ml_l, ml_m, ml_r)
 
 dml_data_irm = make_irm_data(n_obs=n)
 dml_data_iivm = make_iivm_data(n_obs=n)
 dml_cluster_data_pliv = make_pliv_multiway_cluster_CKMS2021(N=10, M=10)
+dml_data_did = make_did_SZ2020(n_obs=n)
+dml_data_did_cs = make_did_SZ2020(n_obs=n, cross_sectional_data=True)
 (x, y, d, z) = make_iivm_data(n_obs=n, return_type="array")
 y[y > 0] = 1
 y[y < 0] = 0
 dml_data_irm_binary_outcome = DoubleMLData.from_arrays(x, y, d)
 dml_data_iivm_binary_outcome = DoubleMLData.from_arrays(x, y, d, z)
 
 
@@ -64,14 +66,20 @@
         _ = DoubleMLPQ(DummyDataClass(pd.DataFrame(np.zeros((100, 10)))), ml_g, ml_m, treatment=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLLPQ(DummyDataClass(pd.DataFrame(np.zeros((100, 10)))), ml_g, ml_m, treatment=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLCVAR(DummyDataClass(pd.DataFrame(np.zeros((100, 10)))), ml_g, ml_m, treatment=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLQTE(DummyDataClass(pd.DataFrame(np.zeros((100, 10)))), ml_g, ml_m)
+    msg = 'For repeated outcomes the data must be of DoubleMLData type.'
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDID(DummyDataClass(pd.DataFrame(np.zeros((100, 10)))), ml_g, ml_m)
+    msg = 'For repeated cross sections the data must be of DoubleMLData type. '
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDIDCS(DummyDataClass(pd.DataFrame(np.zeros((100, 10)))), ml_g, ml_m)
 
     # PLR with IV
     msg = (r'Incompatible data. Z1 have been set as instrumental variable\(s\). '
            'To fit a partially linear IV regression model use DoubleMLPLIV instead of DoubleMLPLR.')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLPLR(dml_data_pliv, ml_l, ml_m)
 
@@ -173,28 +181,28 @@
         # non-binary Z for LPQ
         _ = DoubleMLLPQ(DoubleMLData(df_iivm, 'y', 'd', 'z'),
                         LogisticRegression(), LogisticRegression(), treatment=1)
 
     # CVAR with IV
     msg = r'Incompatible data. z have been set as instrumental variable\(s\).'
     with pytest.raises(ValueError, match=msg):
-        _ = DoubleMLCVAR(dml_data_iivm, LogisticRegression(), LogisticRegression(), treatment=1)
+        _ = DoubleMLCVAR(dml_data_iivm, Lasso(), LogisticRegression(), treatment=1)
     msg = ('Incompatible data. To fit an CVaR model with DML exactly one binary variable with values 0 and 1 '
            'needs to be specified as treatment variable.')
     df_irm = dml_data_irm.data.copy()
     df_irm['d'] = df_irm['d'] * 2
     with pytest.raises(ValueError, match=msg):
         # non-binary D for CVAR
         _ = DoubleMLCVAR(DoubleMLData(df_irm, 'y', 'd'),
-                         LogisticRegression(), LogisticRegression(), treatment=1)
+                         Lasso(), LogisticRegression(), treatment=1)
     df_irm = dml_data_irm.data.copy()
     with pytest.raises(ValueError, match=msg):
         # multiple D for CVAR
         _ = DoubleMLCVAR(DoubleMLData(df_irm, 'y', ['d', 'X1']),
-                         LogisticRegression(), LogisticRegression(), treatment=1)
+                         Lasso(), LogisticRegression(), treatment=1)
 
     # QTE
     msg = ('Incompatible data. To fit an PQ model with DML exactly one binary variable with values 0 and 1 '
            'needs to be specified as treatment variable.')
     df_irm = dml_data_irm.data.copy()
     df_irm['d'] = df_irm['d'] * 2
     with pytest.raises(ValueError, match=msg):
@@ -203,14 +211,62 @@
                         LogisticRegression(), LogisticRegression())
     df_irm = dml_data_irm.data.copy()
     with pytest.raises(ValueError, match=msg):
         # multiple D for QTE
         _ = DoubleMLQTE(DoubleMLData(df_irm, 'y', ['d', 'X1']),
                         LogisticRegression(), LogisticRegression())
 
+    # DID with IV
+    msg = r'Incompatible data. z have been set as instrumental variable\(s\).'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDID(dml_data_iivm, Lasso(), LogisticRegression())
+    msg = ('Incompatible data. To fit an DID model with DML exactly one binary variable with values 0 and 1 '
+           'needs to be specified as treatment variable.')
+    df_irm = dml_data_irm.data.copy()
+    df_irm['d'] = df_irm['d'] * 2
+    with pytest.raises(ValueError, match=msg):
+        # non-binary D for DID
+        _ = DoubleMLDID(DoubleMLData(df_irm, 'y', 'd'),
+                        Lasso(), LogisticRegression())
+    df_irm = dml_data_irm.data.copy()
+    with pytest.raises(ValueError, match=msg):
+        # multiple D for DID
+        _ = DoubleMLDID(DoubleMLData(df_irm, 'y', ['d', 'X1']),
+                        Lasso(), LogisticRegression())
+
+    # DIDCS with IV
+    msg = r'Incompatible data. z have been set as instrumental variable\(s\).'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_iivm, Lasso(), LogisticRegression())
+
+    # DIDCS treatment exceptions
+    msg = ('Incompatible data. To fit an DIDCS model with DML exactly one binary variable with values 0 and 1 '
+           'needs to be specified as treatment variable.')
+    df_did_cs = dml_data_did_cs.data.copy()
+    df_did_cs['d'] = df_did_cs['d'] * 2
+    with pytest.raises(ValueError, match=msg):
+        # non-binary D for DIDCS
+        _ = DoubleMLDIDCS(DoubleMLData(df_did_cs, y_col='y', d_cols='d', t_col='t'),
+                          Lasso(), LogisticRegression())
+    df_did_cs = dml_data_did_cs.data.copy()
+    with pytest.raises(ValueError, match=msg):
+        # multiple D for DIDCS
+        _ = DoubleMLDIDCS(DoubleMLData(df_did_cs, y_col='y', d_cols=['d', 'Z1'], t_col='t'),
+                          Lasso(), LogisticRegression())
+
+    # DIDCS time exceptions
+    msg = ('Incompatible data. To fit an DIDCS model with DML exactly one binary variable with values 0 and 1 '
+           'needs to be specified as time variable.')
+    df_did_cs = dml_data_did_cs.data.copy()
+    df_did_cs['t'] = df_did_cs['t'] * 2
+    with pytest.raises(ValueError, match=msg):
+        # non-binary t for DIDCS
+        _ = DoubleMLDIDCS(DoubleMLData(df_did_cs, y_col='y', d_cols='d', t_col='t'),
+                          Lasso(), LogisticRegression())
+
 
 @pytest.mark.ci
 def test_doubleml_exception_scores():
     # PLR
     msg = 'Invalid score IV. Valid score IV-type or partialling out.'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLPLR(dml_data, ml_l, ml_m, score='IV')
@@ -242,42 +298,58 @@
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLPLIV(dml_data_pliv, Lasso(), Lasso(), Lasso(), score=0)
 
     # PQ
     msg = 'Invalid score IV. Valid score PQ.'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1, score='IV')
-    msg = 'Invalid score. Valid score PQ.'
+    msg = 'score should be a string. 2 was passed.'
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1, score=2)
 
     # LPQ
     msg = 'Invalid score IV. Valid score LPQ.'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLLPQ(dml_data_iivm, LogisticRegression(), LogisticRegression(), treatment=1, score='IV')
-    msg = 'Invalid score. Valid score LPQ.'
+    msg = 'score should be a string. 2 was passed.'
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLLPQ(dml_data_iivm, LogisticRegression(), LogisticRegression(), treatment=1, score=2)
 
     # CVaR
     msg = 'Invalid score IV. Valid score CVaR.'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLCVAR(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1, score='IV')
-    msg = 'Invalid score. Valid score CVaR.'
+    msg = 'score should be a string. 2 was passed.'
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLCVAR(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1, score=2)
 
     # QTE
-    msg = 'Invalid score IV. Valid score PQ or LPQ.'
+    msg = 'Invalid score IV. Valid score PQ or LPQ or CVaR.'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLQTE(dml_data_irm, LogisticRegression(), LogisticRegression(), score='IV')
-    msg = 'Invalid score. Valid score PQ or LPQ.'
+    msg = 'score should be a string. 2 was passed.'
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLQTE(dml_data_irm, LogisticRegression(), LogisticRegression(), score=2)
 
+    # DID
+    msg = 'Invalid score IV. Valid score observational or experimental.'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDID(dml_data_did, Lasso(), LogisticRegression(), score='IV')
+    msg = 'score should be a string. 2 was passed.'
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDID(dml_data_did, Lasso(), LogisticRegression(), score=2)
+
+    # DIDCS
+    msg = 'Invalid score IV. Valid score observational or experimental.'
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression(), score='IV')
+    msg = 'score should be a string. 2 was passed.'
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression(), score=2)
+
 
 @pytest.mark.ci
 def test_doubleml_exception_trimming_rule():
     msg = 'Invalid trimming_rule discard. Valid trimming_rule truncate.'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression(), trimming_rule='discard')
     with pytest.raises(ValueError, match=msg):
@@ -286,24 +358,71 @@
         _ = DoubleMLPQ(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1, trimming_rule='discard')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLLPQ(dml_data_iivm, LogisticRegression(), LogisticRegression(), treatment=1, trimming_rule='discard')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLCVAR(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1, trimming_rule='discard')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLQTE(dml_data_irm, LogisticRegression(), LogisticRegression(), trimming_rule='discard')
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDID(dml_data_did, Lasso(), LogisticRegression(), trimming_rule='discard')
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression(), trimming_rule='discard')
 
     # check the trimming_threshold exceptions
     msg = "trimming_threshold has to be a float. Object of type <class 'str'> passed."
     with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression(),
+                        trimming_rule='truncate', trimming_threshold="0.1")
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLIIVM(dml_data_iivm, Lasso(), LogisticRegression(), LogisticRegression(),
+                         trimming_rule='truncate', trimming_threshold="0.1")
+    with pytest.raises(TypeError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1,
                        trimming_rule='truncate', trimming_threshold="0.1")
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLLPQ(dml_data_iivm, LogisticRegression(), LogisticRegression(), treatment=1,
+                        trimming_rule='truncate', trimming_threshold="0.1")
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLCVAR(dml_data_irm, Lasso(), LogisticRegression(), treatment=1,
+                         trimming_rule='truncate', trimming_threshold="0.1")
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLQTE(dml_data_irm, LogisticRegression(), LogisticRegression(),
+                        trimming_rule='truncate', trimming_threshold="0.1")
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDID(dml_data_did, Lasso(), LogisticRegression(),
+                        trimming_rule='truncate', trimming_threshold="0.1")
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression(),
+                          trimming_rule='truncate', trimming_threshold="0.1")
+
     msg = 'Invalid trimming_threshold 0.6. trimming_threshold has to be between 0 and 0.5.'
     with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression(),
+                        trimming_rule='truncate', trimming_threshold=0.6)
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLIIVM(dml_data_iivm, Lasso(), LogisticRegression(), LogisticRegression(),
+                         trimming_rule='truncate', trimming_threshold=0.6)
+    with pytest.raises(ValueError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, LogisticRegression(), LogisticRegression(), treatment=1,
                        trimming_rule='truncate', trimming_threshold=0.6)
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLLPQ(dml_data_iivm, LogisticRegression(), LogisticRegression(), treatment=1,
+                        trimming_rule='truncate', trimming_threshold=0.6)
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLCVAR(dml_data_irm, Lasso(), LogisticRegression(), treatment=1,
+                         trimming_rule='truncate', trimming_threshold=0.6)
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLQTE(dml_data_irm, LogisticRegression(), LogisticRegression(),
+                        trimming_rule='truncate', trimming_threshold=0.6)
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDID(dml_data_did, Lasso(), LogisticRegression(),
+                        trimming_rule='truncate', trimming_threshold=0.6)
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression(),
+                          trimming_rule='truncate', trimming_threshold=0.6)
 
 
 @pytest.mark.ci
 def test_doubleml_exception_quantiles():
     msg = "Quantile has to be a float. Object of type <class 'str'> passed."
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, ml_g, ml_m, treatment=1, quantile="0.4")
@@ -353,20 +472,31 @@
         _ = DoubleMLLPQ(dml_data_iivm, ml_g, ml_m, treatment=1, kde="0.1")
 
 
 @pytest.mark.ci
 def test_doubleml_exception_normalization():
     msg = "Normalization indicator has to be boolean. Object of type <class 'int'> passed."
     with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLIRM(dml_data_irm, ml_g, LogisticRegression(), normalize_ipw=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLIIVM(dml_data_iivm, ml_g, LogisticRegression(), LogisticRegression(), normalize_ipw=1)
+    with pytest.raises(TypeError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, ml_g, ml_m, treatment=1, normalize_ipw=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLQTE(dml_data_irm, ml_g, ml_m, normalize_ipw=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLLPQ(dml_data_iivm, ml_g, ml_m, treatment=1, normalize_ipw=1)
 
+    # DID models in_sample_normalization
+    msg = "in_sample_normalization indicator has to be boolean. Object of type <class 'int'> passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDID(dml_data_did, ml_g, ml_m, in_sample_normalization=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_did_cs, ml_g, ml_m, in_sample_normalization=1)
+
 
 @pytest.mark.ci
 def test_doubleml_exception_subgroups():
     msg = 'Invalid subgroups True. subgroups must be of type dictionary.'
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLIIVM(dml_data_iivm, Lasso(), LogisticRegression(), LogisticRegression(),
                          subgroups=True)
@@ -510,37 +640,55 @@
     with pytest.raises(ValueError, match=msg):
         dml_qte_boot.bootstrap(n_rep_boot=0)
 
 
 @pytest.mark.ci
 def test_doubleml_exception_confint():
     dml_plr_confint = DoubleMLPLR(dml_data, ml_l, ml_m)
+    dml_qte_confint = DoubleMLQTE(dml_data_irm, RandomForestClassifier(), RandomForestClassifier())
 
     msg = 'joint must be True or False. Got 1.'
     with pytest.raises(TypeError, match=msg):
         dml_plr_confint.confint(joint=1)
+    with pytest.raises(TypeError, match=msg):
+        dml_qte_confint.confint(joint=1)
     msg = "The confidence level must be of float type. 5% of type <class 'str'> was passed."
     with pytest.raises(TypeError, match=msg):
         dml_plr_confint.confint(level='5%')
+    msg = "The confidence level must be of float type. 5% of type <class 'str'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        dml_qte_confint.confint(level='5%')
     msg = r'The confidence level must be in \(0,1\). 0.0 was passed.'
     with pytest.raises(ValueError, match=msg):
         dml_plr_confint.confint(level=0.)
+    with pytest.raises(ValueError, match=msg):
+        dml_qte_confint.confint(level=0.)
 
     msg = r'Apply fit\(\) before confint\(\).'
     with pytest.raises(ValueError, match=msg):
         dml_plr_confint.confint()
+    with pytest.raises(ValueError, match=msg):
+        dml_qte_confint.confint()
     msg = r'Apply fit\(\) & bootstrap\(\) before confint\(joint=True\).'
     with pytest.raises(ValueError, match=msg):
         dml_plr_confint.confint(joint=True)
+    with pytest.raises(ValueError, match=msg):
+        dml_qte_confint.confint(joint=True)
     dml_plr_confint.fit()  # error message should still appear till bootstrap was applied as well
+    dml_qte_confint.fit()
     with pytest.raises(ValueError, match=msg):
         dml_plr_confint.confint(joint=True)
+    with pytest.raises(ValueError, match=msg):
+        dml_qte_confint.confint(joint=True)
     dml_plr_confint.bootstrap()
-    df_ci = dml_plr_confint.confint(joint=True)
-    assert isinstance(df_ci, pd.DataFrame)
+    dml_qte_confint.bootstrap()
+    df_plr_ci = dml_plr_confint.confint(joint=True)
+    df_qte_ci = dml_qte_confint.confint(joint=True)
+    assert isinstance(df_plr_ci, pd.DataFrame)
+    assert isinstance(df_qte_ci, pd.DataFrame)
 
 
 @pytest.mark.ci
 def test_doubleml_exception_p_adjust():
     dml_plr_p_adjust = DoubleMLPLR(dml_data, ml_l, ml_m)
 
     msg = r'Apply fit\(\) before p_adjust\(\).'
```

### Comparing `DoubleML-0.6.0/doubleml/tests/test_doubleml_model_defaults.py` & `DoubleML-0.6.1/doubleml/tests/test_doubleml_model_defaults.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 import pytest
 import numpy as np
 
-from doubleml import DoubleMLPLR, DoubleMLIRM, DoubleMLIIVM, DoubleMLPLIV, DoubleMLCVAR, DoubleMLPQ, DoubleMLLPQ, DoubleMLQTE
-from doubleml.datasets import make_plr_CCDDHNR2018, make_irm_data, make_pliv_CHS2015, make_iivm_data
+from doubleml import DoubleMLPLR, DoubleMLIRM, DoubleMLIIVM, DoubleMLPLIV, DoubleMLCVAR, DoubleMLPQ, \
+    DoubleMLLPQ, DoubleMLQTE, DoubleMLDID, DoubleMLDIDCS
+from doubleml.datasets import make_plr_CCDDHNR2018, make_irm_data, make_pliv_CHS2015, make_iivm_data, make_did_SZ2020
 
 from sklearn.linear_model import Lasso, LogisticRegression
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 
 np.random.seed(3141)
 dml_data_plr = make_plr_CCDDHNR2018(n_obs=100)
 dml_data_pliv = make_pliv_CHS2015(n_obs=100, dim_z=1)
 dml_data_irm = make_irm_data(n_obs=500)
 dml_data_iivm = make_iivm_data(n_obs=1000)
+dml_data_did = make_did_SZ2020(n_obs=100)
+dml_data_did_cs = make_did_SZ2020(n_obs=100, cross_sectional_data=True)
 
 # linear models
 dml_plr = DoubleMLPLR(dml_data_plr, Lasso(), Lasso())
 dml_pliv = DoubleMLPLIV(dml_data_pliv, Lasso(), Lasso(), Lasso())
 dml_irm = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression())
 dml_iivm = DoubleMLIIVM(dml_data_iivm, Lasso(), LogisticRegression(), LogisticRegression())
 dml_cvar = DoubleMLCVAR(dml_data_irm, ml_g=RandomForestRegressor(), ml_m=RandomForestClassifier())
+dml_did = DoubleMLDID(dml_data_did, Lasso(), LogisticRegression())
+dml_did_cs = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression())
 
 dml_plr.fit()
 dml_pliv.fit()
 dml_irm.fit()
 dml_iivm.fit()
 dml_cvar.fit()
+dml_did.fit()
+dml_did_cs.fit()
 
 dml_plr.bootstrap()
 dml_pliv.bootstrap()
 dml_irm.bootstrap()
 dml_iivm.bootstrap()
 dml_cvar.bootstrap()
+dml_did.bootstrap()
+dml_did_cs.bootstrap()
 
 # nonlinear models
 dml_pq = DoubleMLPQ(dml_data_irm, ml_g=LogisticRegression(), ml_m=LogisticRegression())
 dml_lpq = DoubleMLLPQ(dml_data_iivm, ml_g=RandomForestClassifier(), ml_m=RandomForestClassifier())
 dml_qte = DoubleMLQTE(dml_data_irm, ml_g=RandomForestClassifier(), ml_m=RandomForestClassifier())
 
 dml_pq.fit()
@@ -144,7 +153,26 @@
     # not fix since its a differen object added in future versions _assert_resampling_default_settings(dml_qte)
     assert dml_qte.quantiles == 0.5
     assert dml_qte.score == 'PQ'
     assert dml_qte.dml_procedure == 'dml2'
     assert dml_qte.trimming_rule == 'truncate'
     assert dml_qte.trimming_threshold == 1e-2
     assert dml_qte.normalize_ipw
+
+
+@pytest.mark.ci
+def test_did_defaults():
+    _assert_resampling_default_settings(dml_did)
+    assert dml_did.score == 'observational'
+    assert dml_did.in_sample_normalization
+    assert dml_did.trimming_rule == 'truncate'
+    assert dml_did.trimming_threshold == 1e-2
+
+
+@pytest.mark.ci
+def test_did_cs_defaults():
+    _assert_resampling_default_settings(dml_did_cs)
+    assert dml_did.score == 'observational'
+    assert dml_did_cs.in_sample_normalization
+    assert dml_did_cs.dml_procedure == 'dml2'
+    assert dml_did_cs.trimming_rule == 'truncate'
+    assert dml_did_cs.trimming_threshold == 1e-2
```

### Comparing `DoubleML-0.6.0/doubleml/tests/test_doubleml_scores.py` & `DoubleML-0.6.1/doubleml/tests/test_doubleml_scores.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_doubleml_set_ml_nuisance_params.py` & `DoubleML-0.6.1/doubleml/tests/test_doubleml_set_ml_nuisance_params.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_doubleml_set_sample_splitting.py` & `DoubleML-0.6.1/doubleml/tests/test_doubleml_set_sample_splitting.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_iivm.py` & `DoubleML-0.6.1/doubleml/tests/test_iivm.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_iivm_classifier.py` & `DoubleML-0.6.1/doubleml/tests/test_iivm_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_iivm_no_cross_fit.py` & `DoubleML-0.6.1/doubleml/tests/test_iivm_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_iivm_subgroups.py` & `DoubleML-0.6.1/doubleml/tests/test_iivm_subgroups.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_iivm_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_iivm_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_irm.py` & `DoubleML-0.6.1/doubleml/tests/test_irm.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_irm_classifier.py` & `DoubleML-0.6.1/doubleml/tests/test_irm_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_irm_no_cross_fit.py` & `DoubleML-0.6.1/doubleml/tests/test_irm_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_irm_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_irm_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_irm_with_missings.py` & `DoubleML-0.6.1/doubleml/tests/test_irm_with_missings.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_lpq.py` & `DoubleML-0.6.1/doubleml/tests/test_lpq.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_lpq_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_lpq_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_multiway_cluster.py` & `DoubleML-0.6.1/doubleml/tests/test_multiway_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_nonlinear_cluster.py` & `DoubleML-0.6.1/doubleml/tests/test_nonlinear_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_nonlinear_score_mixin.py` & `DoubleML-0.6.1/doubleml/tests/test_nonlinear_score_mixin.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_no_cross_fit.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_partial_x.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_partial_x_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_partial_xz.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_partial_xz_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_partial_z.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_partial_z_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pliv_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_pliv_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr.py` & `DoubleML-0.6.1/doubleml/tests/test_plr.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_classifier.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_multi_treat.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_multi_treat.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_no_cross_fit.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_reestimate_from_scores.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_reestimate_from_scores.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_rep_cross.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_rep_cross.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_set_ml_nuisance_pars.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_set_ml_nuisance_pars.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_set_smpls_externally.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_set_smpls_externally.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_plr_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_plr_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pq.py` & `DoubleML-0.6.1/doubleml/tests/test_pq.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_pq_tune.py` & `DoubleML-0.6.1/doubleml/tests/test_pq_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/doubleml/tests/test_qte.py` & `DoubleML-0.6.1/doubleml/tests/test_qte.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.0/setup.py` & `DoubleML-0.6.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'Documentation': 'https://docs.doubleml.org',
     'Source Code': 'https://github.com/DoubleML/doubleml-for-py',
     'Bug Tracker': 'https://github.com/DoubleML/doubleml-for-py/issues',
 }
 
 setup(
     name='DoubleML',
-    version='0.6.0',
+    version='0.6.1',
     author='Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.',
     maintainer='Malte S. Kurz',
     maintainer_email='malte.simon.kurz@uni-hamburg.de',
     description='Double Machine Learning in Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://docs.doubleml.org',
```


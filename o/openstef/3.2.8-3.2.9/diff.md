# Comparing `tmp/openstef-3.2.8.tar.gz` & `tmp/openstef-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef-3.2.8.tar", last modified: Tue May 31 13:22:39 2022, max compression
+gzip compressed data, was "openstef-3.2.9.tar", last modified: Wed Jul  6 13:16:44 2022, max compression
```

## Comparing `openstef-3.2.8.tar` & `openstef-3.2.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)    14907 2022-05-31 13:22:30.000000 openstef-3.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-05-31 13:22:39.539657 openstef-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-05-31 13:22:30.000000 openstef-3.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.531657 openstef-3.2.8/openstef/
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.535657 openstef-3.2.8/openstef/data/
--rw-r--r--   0 runner    (1001) docker     (121)    23704 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data/dutch_holidays_2020-2022.csv
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data/dutch_holidays_2020-2022.csv.license
--rw-r--r--   0 runner    (1001) docker     (121)    24779 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data/pv_single_coefs.csv
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data/pv_single_coefs.csv.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.535657 openstef-3.2.8/openstef/data_classes/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data_classes/model_specifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data_classes/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/data_classes/split_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.535657 openstef-3.2.8/openstef/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/apply_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     5655 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/feature_adder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6793 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/feature_applicator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/general.py
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/historic_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     7346 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/holiday_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     5784 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/lag_features.py
--rw-r--r--   0 runner    (1001) docker     (121)    11231 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/feature_engineering/weather_features.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.535657 openstef-3.2.8/openstef/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7472 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/metrics/figure.py
--rw-r--r--   0 runner    (1001) docker     (121)    11751 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/metrics/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.535657 openstef-3.2.8/openstef/model/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2946 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/basecase.py
--rw-r--r--   0 runner    (1001) docker     (121)     9022 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/confidence_interval_applicator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/fallback.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.535657 openstef-3.2.8/openstef/model/metamodels/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/metamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8262 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/metamodels/grouped_regressor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5117 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/metamodels/missing_values_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/model_creator.py
--rw-r--r--   0 runner    (1001) docker     (121)    14026 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/objective.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/objective_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.535657 openstef-3.2.8/openstef/model/regressors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/custom_regressor.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     9169 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/proloaf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/regressor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/regressor_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/xgb.py
--rw-r--r--   0 runner    (1001) docker     (121)     7230 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/regressors/xgb_quantile.py
--rw-r--r--   0 runner    (1001) docker     (121)    14610 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model/standard_deviation_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/model_selection/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10949 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/model_selection/model_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/monitoring/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/monitoring/performance_meter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6208 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/monitoring/teams.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/create_basecase_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/create_component_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/create_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     9742 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/optimize_hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5694 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/train_create_forecast_backtest.py
--rw-r--r--   0 runner    (1001) docker     (121)    17614 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/train_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7623 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/postprocessing/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/preprocessing/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/calculate_kpi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/create_basecase_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/create_components_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/create_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)    14933 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/create_solar_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/create_wind_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/optimize_hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4703 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/run_tracy.py
--rw-r--r--   0 runner    (1001) docker     (121)     8812 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/split_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/train_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/tasks/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     9767 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/utils/predictionjobloop.py
--rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/tasks/utils/taskcontext.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.539657 openstef-3.2.8/openstef/validation/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14498 2022-05-31 13:22:30.000000 openstef-3.2.8/openstef/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 13:22:39.531657 openstef-3.2.8/openstef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-05-31 13:22:39.000000 openstef-3.2.8/openstef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-05-31 13:22:39.000000 openstef-3.2.8/openstef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 13:22:39.000000 openstef-3.2.8/openstef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-05-31 13:22:39.000000 openstef-3.2.8/openstef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-31 13:22:39.000000 openstef-3.2.8/openstef.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-05-31 13:22:30.000000 openstef-3.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-05-31 13:22:39.539657 openstef-3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-05-31 13:22:30.000000 openstef-3.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.180264 openstef-3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    14907 2022-07-06 13:16:36.000000 openstef-3.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-07-06 13:16:44.180264 openstef-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-07-06 13:16:36.000000 openstef-3.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.172264 openstef-3.2.9/openstef/
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.172264 openstef-3.2.9/openstef/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    23704 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data/dutch_holidays_2020-2022.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data/dutch_holidays_2020-2022.csv.license
+-rw-r--r--   0 runner    (1001) docker     (121)    24779 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data/pv_single_coefs.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data/pv_single_coefs.csv.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.172264 openstef-3.2.9/openstef/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data_classes/model_specifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data_classes/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/data_classes/split_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.172264 openstef-3.2.9/openstef/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/apply_features.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5655 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/feature_adder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6793 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/feature_applicator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/general.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/historic_features.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7346 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/holiday_features.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5784 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/lag_features.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11231 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/feature_engineering/weather_features.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.172264 openstef-3.2.9/openstef/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7472 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/metrics/figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11751 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/metrics/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2946 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/basecase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9022 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/confidence_interval_applicator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/fallback.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/model/metamodels/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/metamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8262 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/metamodels/grouped_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5117 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/metamodels/missing_values_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/model_creator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14026 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/objective.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/objective_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/model/regressors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/custom_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9169 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/proloaf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/regressor_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7230 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/regressors/xgb_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14610 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model/standard_deviation_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10949 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/model_selection/model_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/monitoring/performance_meter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6208 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/monitoring/teams.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/create_basecase_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/create_component_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/create_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9741 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/optimize_hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5693 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/train_create_forecast_backtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17614 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/train_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7623 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/postprocessing/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.176264 openstef-3.2.9/openstef/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/preprocessing/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.180264 openstef-3.2.9/openstef/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/calculate_kpi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/create_basecase_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/create_components_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/create_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14933 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/create_solar_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/create_wind_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/optimize_hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4703 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/run_tracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8812 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/split_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/train_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.180264 openstef-3.2.9/openstef/tasks/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9767 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/utils/predictionjobloop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/tasks/utils/taskcontext.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.180264 openstef-3.2.9/openstef/validation/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14498 2022-07-06 13:16:36.000000 openstef-3.2.9/openstef/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:16:44.172264 openstef-3.2.9/openstef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-07-06 13:16:44.000000 openstef-3.2.9/openstef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-07-06 13:16:44.000000 openstef-3.2.9/openstef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 13:16:44.000000 openstef-3.2.9/openstef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-06 13:16:44.000000 openstef-3.2.9/openstef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-06 13:16:44.000000 openstef-3.2.9/openstef.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-07-06 13:16:36.000000 openstef-3.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-06 13:16:44.180264 openstef-3.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-07-06 13:16:36.000000 openstef-3.2.9/setup.py
```

### Comparing `openstef-3.2.8/LICENSE` & `openstef-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/PKG-INFO` & `openstef-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef
-Version: 3.2.8
+Version: 3.2.9
 Summary: Open short term energy forecaster
 Home-page: https://github.com/OpenSTEF/openstef
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: energy,forecasting,machinelearning
 Platform: UNKNOWN
```

### Comparing `openstef-3.2.8/README.md` & `openstef-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/__main__.py` & `openstef-3.2.9/openstef/__main__.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/data/dutch_holidays_2020-2022.csv` & `openstef-3.2.9/openstef/data/dutch_holidays_2020-2022.csv`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/data/pv_single_coefs.csv` & `openstef-3.2.9/openstef/data/pv_single_coefs.csv`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/data_classes/model_specifications.py` & `openstef-3.2.9/openstef/data_classes/model_specifications.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/data_classes/prediction_job.py` & `openstef-3.2.9/openstef/data_classes/prediction_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com> # noqa E501>
 #
 # SPDX-License-Identifier: MPL-2.0
 
-from typing import Union, Optional, List, Dict, Any
+from typing import Any, Dict, List, Optional, Union
+
 from pydantic import BaseModel
-from .split_function import SplitFuncDataClass
+
 from .model_specifications import ModelSpecificationDataClass
+from .split_function import SplitFuncDataClass
 
 
 class PredictionJobDataClass(BaseModel):
     id: Union[int, str]
     model: str
     forecast_type: str
     horizon_minutes: int
```

### Comparing `openstef-3.2.8/openstef/data_classes/split_function.py` & `openstef-3.2.9/openstef/data_classes/split_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com> # noqa E501>
 #
 # SPDX-License-Identifier: MPL-2.0
 
+import inspect
 import json
 from importlib import import_module
-from typing import Union, Dict, Callable, Any, Sequence
+from typing import Any, Callable, Dict, Sequence, Union
 
-import inspect
 from pydantic import BaseModel
 
 
 class SplitFuncDataClass(BaseModel):
     function: Union[str, Callable]
     arguments: Union[
         str, Dict[str, Any]
```

### Comparing `openstef-3.2.8/openstef/enums.py` & `openstef-3.2.9/openstef/enums.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/exceptions.py` & `openstef-3.2.9/openstef/exceptions.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/apply_features.py` & `openstef-3.2.9/openstef/feature_engineering/apply_features.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/feature_adder.py` & `openstef-3.2.9/openstef/feature_engineering/feature_adder.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/feature_applicator.py` & `openstef-3.2.9/openstef/feature_engineering/feature_applicator.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/general.py` & `openstef-3.2.9/openstef/feature_engineering/general.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/historic_features.py` & `openstef-3.2.9/openstef/feature_engineering/historic_features.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/holiday_features.py` & `openstef-3.2.9/openstef/feature_engineering/holiday_features.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/lag_features.py` & `openstef-3.2.9/openstef/feature_engineering/lag_features.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/feature_engineering/weather_features.py` & `openstef-3.2.9/openstef/feature_engineering/weather_features.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/metrics/figure.py` & `openstef-3.2.9/openstef/metrics/figure.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/metrics/metrics.py` & `openstef-3.2.9/openstef/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/metrics/reporter.py` & `openstef-3.2.9/openstef/metrics/reporter.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/basecase.py` & `openstef-3.2.9/openstef/model/basecase.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/confidence_interval_applicator.py` & `openstef-3.2.9/openstef/model/confidence_interval_applicator.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/fallback.py` & `openstef-3.2.9/openstef/model/fallback.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/metamodels/grouped_regressor.py` & `openstef-3.2.9/openstef/model/metamodels/grouped_regressor.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/metamodels/missing_values_handler.py` & `openstef-3.2.9/openstef/model/metamodels/missing_values_handler.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/model_creator.py` & `openstef-3.2.9/openstef/model/model_creator.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/objective.py` & `openstef-3.2.9/openstef/model/objective.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/objective_creator.py` & `openstef-3.2.9/openstef/model/objective_creator.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/custom_regressor.py` & `openstef-3.2.9/openstef/model/regressors/custom_regressor.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/lgbm.py` & `openstef-3.2.9/openstef/model/regressors/lgbm.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/linear.py` & `openstef-3.2.9/openstef/model/regressors/linear.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/proloaf.py` & `openstef-3.2.9/openstef/model/regressors/proloaf.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/regressor.py` & `openstef-3.2.9/openstef/model/regressors/regressor.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/regressor_interface.py` & `openstef-3.2.9/openstef/model/regressors/regressor_interface.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/xgb.py` & `openstef-3.2.9/openstef/model/regressors/xgb.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/regressors/xgb_quantile.py` & `openstef-3.2.9/openstef/model/regressors/xgb_quantile.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/serializer.py` & `openstef-3.2.9/openstef/model/serializer.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model/standard_deviation_generator.py` & `openstef-3.2.9/openstef/model/standard_deviation_generator.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/model_selection/model_selection.py` & `openstef-3.2.9/openstef/model_selection/model_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com> # noqa E501>
 #
 # SPDX-License-Identifier: MPL-2.0
 import random
 import secrets
 from datetime import timedelta
 from itertools import accumulate
-from typing import List, Tuple, Iterable
+from typing import Iterable, List, Tuple
 
 import numpy as np
 import pandas as pd
 
 AMOUNT_DAY = 96  # Duration of the periods (in T-15) that are in a day (default = 96)
 PERIOD_TIMEDELTA = 1  # Duration of the periods (in days) that will be sampled as validation data for each split.
 PEAK_FRACTION = 0.15
```

### Comparing `openstef-3.2.8/openstef/monitoring/performance_meter.py` & `openstef-3.2.9/openstef/monitoring/performance_meter.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/monitoring/teams.py` & `openstef-3.2.9/openstef/monitoring/teams.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/pipeline/create_basecase_forecast.py` & `openstef-3.2.9/openstef/pipeline/create_basecase_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/pipeline/create_component_forecast.py` & `openstef-3.2.9/openstef/pipeline/create_component_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/pipeline/create_forecast.py` & `openstef-3.2.9/openstef/pipeline/create_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/pipeline/optimize_hyperparameters.py` & `openstef-3.2.9/openstef/pipeline/optimize_hyperparameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com> # noqa E501>
 #
 # SPDX-License-Identifier: MPL-2.0
-from typing import List, Tuple, Any
+from typing import Any, List, Tuple
 
 import optuna
 import pandas as pd
 import structlog
 
 from openstef.data_classes.model_specifications import ModelSpecificationDataClass
 from openstef.data_classes.prediction_job import PredictionJobDataClass
 from openstef.exceptions import (
     InputDataInsufficientError,
     InputDataWrongColumnOrderError,
 )
 from openstef.feature_engineering.feature_applicator import TrainFeatureApplicator
-from openstef.metrics.reporter import Reporter, Report
+from openstef.metrics.reporter import Report, Reporter
 from openstef.model.model_creator import ModelCreator
-from openstef.model.regressors.regressor import OpenstfRegressor
-
 from openstef.model.objective import RegressorObjective
 from openstef.model.objective_creator import ObjectiveCreator
+from openstef.model.regressors.regressor import OpenstfRegressor
 from openstef.model.serializer import MLflowSerializer
 from openstef.pipeline.train_model import (
     DEFAULT_TRAIN_HORIZONS,
     train_model_pipeline_core,
 )
 from openstef.validation import validation
```

### Comparing `openstef-3.2.8/openstef/pipeline/train_create_forecast_backtest.py` & `openstef-3.2.9/openstef/pipeline/train_create_forecast_backtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from openstef.model.regressors.regressor import OpenstfRegressor
 from openstef.model_selection.model_selection import backtest_split_default
 from openstef.pipeline import train_model
 from openstef.postprocessing.postprocessing import (
     add_prediction_job_properties_to_forecast,
 )
 
-
 DEFAULT_TRAIN_HORIZONS: List[float] = [0.25, 24.0]
 DEFAULT_EARLY_STOPPING_ROUNDS: int = 10
 
 
 def train_model_and_forecast_back_test(
     pj: PredictionJobDataClass,
     modelspecs: ModelSpecificationDataClass,
```

### Comparing `openstef-3.2.8/openstef/pipeline/train_model.py` & `openstef-3.2.9/openstef/pipeline/train_model.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/pipeline/utils.py` & `openstef-3.2.9/openstef/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/postprocessing/postprocessing.py` & `openstef-3.2.9/openstef/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/calculate_kpi.py` & `openstef-3.2.9/openstef/tasks/calculate_kpi.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/create_basecase_forecast.py` & `openstef-3.2.9/openstef/tasks/create_basecase_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/create_components_forecast.py` & `openstef-3.2.9/openstef/tasks/create_components_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/create_forecast.py` & `openstef-3.2.9/openstef/tasks/create_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/create_solar_forecast.py` & `openstef-3.2.9/openstef/tasks/create_solar_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/create_wind_forecast.py` & `openstef-3.2.9/openstef/tasks/create_wind_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/optimize_hyperparameters.py` & `openstef-3.2.9/openstef/tasks/optimize_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/run_tracy.py` & `openstef-3.2.9/openstef/tasks/run_tracy.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/split_forecast.py` & `openstef-3.2.9/openstef/tasks/split_forecast.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/train_model.py` & `openstef-3.2.9/openstef/tasks/train_model.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/utils/dependencies.py` & `openstef-3.2.9/openstef/tasks/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/utils/predictionjobloop.py` & `openstef-3.2.9/openstef/tasks/utils/predictionjobloop.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/tasks/utils/taskcontext.py` & `openstef-3.2.9/openstef/tasks/utils/taskcontext.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef/validation/validation.py` & `openstef-3.2.9/openstef/validation/validation.py`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/openstef.egg-info/PKG-INFO` & `openstef-3.2.9/openstef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef
-Version: 3.2.8
+Version: 3.2.9
 Summary: Open short term energy forecaster
 Home-page: https://github.com/OpenSTEF/openstef
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: energy,forecasting,machinelearning
 Platform: UNKNOWN
```

### Comparing `openstef-3.2.8/openstef.egg-info/SOURCES.txt` & `openstef-3.2.9/openstef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef-3.2.8/setup.py` & `openstef-3.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef",
-    version="3.2.8",
+    version="3.2.9",
     packages=find_packages(include=["openstef", "openstef.*"]),
     description="Open short term energy forecaster",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/OpenSTEF/openstef",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```


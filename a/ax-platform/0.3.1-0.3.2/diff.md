# Comparing `tmp/ax-platform-0.3.1.tar.gz` & `tmp/ax-platform-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ax-platform-0.3.1.tar", last modified: Wed Mar 15 22:22:33 2023, max compression
+gzip compressed data, was "ax-platform-0.3.2.tar", last modified: Mon May  8 20:45:14 2023, max compression
```

## Comparing `ax-platform-0.3.1.tar` & `ax-platform-0.3.2.tar`

### file list

```diff
@@ -1,723 +1,727 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.611970 ax-platform-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-15 22:19:22.000000 ax-platform-0.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.339962 ax-platform-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.347963 ax-platform-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-15 22:19:22.000000 ax-platform-0.3.1/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-03-15 22:19:22.000000 ax-platform-0.3.1/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-15 22:19:22.000000 ax-platform-0.3.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-15 22:19:22.000000 ax-platform-0.3.1/.github/workflows/reusable_tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-15 22:19:22.000000 ax-platform-0.3.1/.github/workflows/tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-15 22:19:22.000000 ax-platform-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-15 22:19:22.000000 ax-platform-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-15 22:19:22.000000 ax-platform-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-03-15 22:19:22.000000 ax-platform-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-15 22:19:22.000000 ax-platform-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-03-15 22:22:33.611970 ax-platform-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-15 22:19:22.000000 ax-platform-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.347963 ax-platform-0.3.1/ax/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.351963 ax-platform-0.3.1/ax/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/benchmark_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/benchmark_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/benchmark_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.351963 ax-platform-0.3.1/ax/benchmark/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/methods/choose_generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/methods/gpei_and_moo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/methods/modular_botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/methods/saasbo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.351963 ax-platform-0.3.1/ax/benchmark/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/hd_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.351963 ax-platform-0.3.1/ax/benchmark/problems/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/hpo/pytorch_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/hpo/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/surrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.351963 ax-platform-0.3.1/ax/benchmark/problems/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.351963 ax-platform-0.3.1/ax/benchmark/problems/synthetic/discretized/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/synthetic/discretized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/synthetic/discretized/mixed_integer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.355963 ax-platform-0.3.1/ax/benchmark/problems/synthetic/hss/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/synthetic/hss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/problems/synthetic/hss/jenatton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.359963 ax-platform-0.3.1/ax/benchmark/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/test_benchmark_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/test_benchmark_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/test_mixed_integer_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/test_problem_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/benchmark/tests/test_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.367963 ax-platform-0.3.1/ax/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/arm.py
--rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/base_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    27070 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/batch_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    60991 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/formatting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/generator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    16503 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/map_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/map_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/multi_type_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/optimization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/outcome_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24375 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/parameter_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/parameter_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    45577 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/search_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.375963 ax-platform-0.3.1/ax/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_arm.py
--rw-r--r--   0 runner    (1001) docker     (123)    30323 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_batch_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    48974 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_formatting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_generator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_map_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_map_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_multi_type_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    31569 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_optimization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_outcome_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_parameter_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_parameter_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    44614 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.375963 ax-platform-0.3.1/ax/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.375963 ax-platform-0.3.1/ax/early_stopping/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23992 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/strategies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/strategies/logical.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/strategies/percentile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/strategies/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.379963 ax-platform-0.3.1/ax/early_stopping/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28469 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/tests/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/early_stopping/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.379963 ax-platform-0.3.1/ax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/exceptions/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/exceptions/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/exceptions/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/exceptions/generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/exceptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/exceptions/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.379963 ax-platform-0.3.1/ax/global_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/global_stopping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.379963 ax-platform-0.3.1/ax/global_stopping/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/global_stopping/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/global_stopping/strategies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/global_stopping/strategies/improvement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.379963 ax-platform-0.3.1/ax/global_stopping/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/global_stopping/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/global_stopping/tests/tests_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.387964 ax-platform-0.3.1/ax/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/botorch_test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/branin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/branin_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/chemistry.py
--rw-r--r--   0 runner    (1001) docker     (123)    31150 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/chemistry_data.zip
--rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/dict_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/factorial.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/hartmann6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/jenatton.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/l2norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/noisy_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/noisy_function_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.387964 ax-platform-0.3.1/ax/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tests/test_chemistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tests/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tests/test_dict_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tests/test_noisy_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/tests/test_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/metrics/torchx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.395964 ax-platform-0.3.1/ax/modelbridge/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42100 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/completion_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    27655 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/dispatch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/generation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    40066 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/map_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/model_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    57919 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/modelbridge_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.395964 ax-platform-0.3.1/ax/modelbridge/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/strategies/alebo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/strategies/rembo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.415964 ax-platform-0.3.1/ax/modelbridge/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_alebo_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    29268 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_base_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_base_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_cap_parameter_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_cast_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_centered_unit_x_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_choice_encode_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_completion_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_convert_metric_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_derelativize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_discrete_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_dispatch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22595 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_generation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35740 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_int_range_to_choice_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_int_to_float_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_ivw_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_log_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_log_y_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_logit_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_map_torch_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_map_unit_x_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_metrics_as_task_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_modelbridge_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_one_hot_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_pairwise_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_percentile_y_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_power_transform_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_random_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    20005 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_relativize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_rembo_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_remove_fixed_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_robust.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_search_space_to_choice_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_standardize_y_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_stratified_standardize_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_task_encode_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    29980 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_torch_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_torch_modelbridge_moo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_transform_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_trial_as_task_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_unit_x_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29969 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_winsorize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/tests/test_winsorize_transform_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    38826 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.427965 ax-platform-0.3.1/ax/modelbridge/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/cap_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/centered_unit_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/choice_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/convert_metric_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/derelativize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/int_range_to_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/int_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/ivw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/log_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/logit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/map_unit_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/metrics_as_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/percentile_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/power_transform_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/relativize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/remove_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/search_space_to_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/standardize_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/stratified_standardize_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/task_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/trial_as_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/unit_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/modelbridge/transforms/winsorize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.431965 ax-platform-0.3.1/ax/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.435965 ax-platform-0.3.1/ax/models/discrete/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/discrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/discrete/eb_thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/discrete/full_factorial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/discrete/thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/discrete_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22672 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.435965 ax-platform-0.3.1/ax/models/random/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/random/alebo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/random/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/random/rembo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/random/sobol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/random/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.451965 ax-platform-0.3.1/ax/models/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_alebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_alebo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_botorch_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_botorch_kg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_botorch_mes.py
--rw-r--r--   0 runner    (1001) docker     (123)    28898 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_botorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_botorch_moo_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    33596 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_botorch_moo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_cbo_lcea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_cbo_lcem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_cbo_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_eb_thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_full_factorial.py
--rw-r--r--   0 runner    (1001) docker     (123)    48544 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_posterior_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_randomforest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_rembo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_rembo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_sobol.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_torch_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/tests/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.463966 ax-platform-0.3.1/ax/models/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29602 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/alebo.py
--rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_kg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_mes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.467966 ax-platform-0.3.1/ax/models/torch/botorch_modular/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24650 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/list_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    27220 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/optimizer_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    34817 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_modular/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_moo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/botorch_moo_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/cbo_lcea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/cbo_lcem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/cbo_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/frontier_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24192 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/fully_bayesian_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/posterior_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/randomforest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/rembo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.471966 ax-platform-0.3.1/ax/models/torch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25176 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/tests/test_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    35313 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/tests/test_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/tests/test_optimizer_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    46748 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/tests/test_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/torch_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/models/winsorization_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.479966 ax-platform-0.3.1/ax/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/bandit_rollout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    32727 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/contour.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.483966 ax-platform-0.3.1/ax/plot/css/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/feature_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.483966 ax-platform-0.3.1/ax/plot/js/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.487966 ax-platform-0.3.1/ax/plot/js/common/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/common/css.js
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/common/helpers.js
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/common/plotly_offline.js
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/common/plotly_online.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/common/plotly_requires.js
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/js/generic_plotly.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/marginal_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    38198 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/pareto_frontier.py
--rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/pareto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    58188 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/table_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.491967 ax-platform-0.3.1/ax/plot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.491967 ax-platform-0.3.1/ax/plot/tests/long_running/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/long_running/test_pareto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_contours.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_feature_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_fitted_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_pareto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_tile_fitted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/tests/test_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/plot/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.495967 ax-platform-0.3.1/ax/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/runners/botorch_test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/runners/simulated_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/runners/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.495967 ax-platform-0.3.1/ax/runners/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/runners/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/runners/tests/test_torchx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/runners/torchx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.499967 ax-platform-0.3.1/ax/service/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78094 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/ax_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/interactive_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/managed_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    77068 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.507967 ax-platform-0.3.1/ax/service/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119626 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_ax_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_best_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_best_point_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_global_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_instantiation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_interactive_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_managed_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51857 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/tests/test_with_db_settings_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.511967 ax-platform-0.3.1/ax/service/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34580 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/best_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/best_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    37549 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/instantiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/scheduler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/service/utils/with_db_settings_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.515967 ax-platform-0.3.1/ax/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/botorch_modular_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.519967 ax-platform-0.3.1/ax/storage/json_store/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28491 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.519967 ax-platform-0.3.1/ax/storage/json_store/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/json_store/tests/test_json_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/metric_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/registry_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/runner_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.531968 ax-platform-0.3.1/ax/storage/sqa_store/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    49885 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    44346 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/reduced_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/save.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/sqa_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/sqa_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/sqa_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.531968 ax-platform-0.3.1/ax/storage/sqa_store/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73083 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/tests/test_sqa_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/sqa_store/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.531968 ax-platform-0.3.1/ax/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/tests/test_registry_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/transform_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.535968 ax-platform-0.3.1/ax/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.535968 ax-platform-0.3.1/ax/telemetry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/tests/test_generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/telemetry/tests/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.535968 ax-platform-0.3.1/ax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.543968 ax-platform-0.3.1/ax/utils/common/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/docutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/equality.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/executils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.543968 ax-platform-0.3.1/ax/utils/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_docutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_executils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_kwargutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/tests/test_typeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/timeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/typeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/common/typeutils_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.547968 ax-platform-0.3.1/ax/utils/flake8_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/flake8_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/flake8_plugins/docstring_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.547968 ax-platform-0.3.1/ax/utils/measurement/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/measurement/synthetic_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.547968 ax-platform-0.3.1/ax/utils/measurement/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/measurement/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/measurement/tests/test_synthetic_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.547968 ax-platform-0.3.1/ax/utils/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/notebook/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.547968 ax-platform-0.3.1/ax/utils/report/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.551968 ax-platform-0.3.1/ax/utils/report/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/resources/base_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/resources/report.css
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/resources/simple_template.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/resources/sufficient_statistic.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.551968 ax-platform-0.3.1/ax/utils/report/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/report/tests/test_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.551968 ax-platform-0.3.1/ax/utils/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/sensitivity/derivative_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/sensitivity/derivative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    29864 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/sensitivity/sobol_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.551968 ax-platform-0.3.1/ax/utils/sensitivity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/sensitivity/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/sensitivity/tests/test_sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.551968 ax-platform-0.3.1/ax/utils/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/stats/statstools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.555968 ax-platform-0.3.1/ax/utils/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/stats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/stats/tests/test_statstools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.559968 ax-platform-0.3.1/ax/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/backend_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/backend_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/benchmark_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65879 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/core_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.559968 ax-platform-0.3.1/ax/utils/testing/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/metrics/backend_simulator_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/metrics/branin_backend_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/modeling_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/test_init_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.559968 ax-platform-0.3.1/ax/utils/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/tests/test_backend_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/torch_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.559968 ax-platform-0.3.1/ax/utils/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/tutorials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-03-15 22:19:22.000000 ax-platform-0.3.1/ax/utils/tutorials/cnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-15 22:22:32.000000 ax-platform-0.3.1/ax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.559968 ax-platform-0.3.1/ax_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-03-15 22:22:33.000000 ax-platform-0.3.1/ax_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-03-15 22:22:33.000000 ax-platform-0.3.1/ax_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:22:33.000000 ax-platform-0.3.1/ax_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-15 22:22:33.000000 ax-platform-0.3.1/ax_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-15 22:22:33.000000 ax-platform-0.3.1/ax_platform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.563969 ax-platform-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/algo-overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.579969 ax-platform-0.3.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    81587 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/bandit_allocation.png
--rw-r--r--   0 runner    (1001) docker     (123)   345484 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/bo_1d_opt.gif
--rw-r--r--   0 runner    (1001) docker     (123)   156260 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/contour.js
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/cv.js
--rw-r--r--   0 runner    (1001) docker     (123)   131612 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/example_shrinkage.png
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/fitted.js
--rw-r--r--   0 runner    (1001) docker     (123)    65905 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/gp_opt.png
--rw-r--r--   0 runner    (1001) docker     (123)   349223 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/gp_posterior.png
--rw-r--r--   0 runner    (1001) docker     (123)   121838 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/mab_animate.gif
--rw-r--r--   0 runner    (1001) docker     (123)   132372 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/mab_probs.png
--rw-r--r--   0 runner    (1001) docker     (123)   325134 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/mab_regret.png
--rw-r--r--   0 runner    (1001) docker     (123)    26226 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/assets/slice.js
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/banditopt.md
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/bayesopt.md
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/core.md
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/data.md
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/glossary.md
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)    22509 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/models.md
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/storage.md
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/trial-evaluation.md
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-15 22:19:22.000000 ax-platform-0.3.1/docs/why-ax.md
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-15 22:19:22.000000 ax-platform-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-15 22:19:22.000000 ax-platform-0.3.1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.583969 ax-platform-0.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/build_ax.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/docker_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/import_ax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/insert_api_refs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4160 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/make_docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/make_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/parse_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/patch_site_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/publish_site.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/update_versions_html.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/validate_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/versions.js
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-15 22:19:22.000000 ax-platform-0.3.1/scripts/wheels_build.ps1
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 22:22:33.611970 ax-platform-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-15 22:19:22.000000 ax-platform-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.583969 ax-platform-0.3.1/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.587969 ax-platform-0.3.1/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/ax.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/early_stopping.rst
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/global_stopping.rst
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/modelbridge.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/plot.rst
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/runners.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/telemetry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-03-15 22:19:22.000000 ax-platform-0.3.1/sphinx/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.599969 ax-platform-0.3.1/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    39419 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.599969 ax-platform-0.3.1/tutorials/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)   224156 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/early_stopping/early_stopping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/early_stopping/mnist_train_nas.py
--rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/factorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25591 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/generation_strategy.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/gpei_hartmann_developer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   273139 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/gpei_hartmann_loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/gpei_hartmann_service.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.603970 ax-platform-0.3.1/tutorials/human_in_the_loop/
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/human_in_the_loop/hitl_data.json
--rw-r--r--   0 runner    (1001) docker     (123)   634579 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/human_in_the_loop/hitl_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)   276956 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/human_in_the_loop/human_in_the_loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    51566 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/modular_botax.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/multi_task.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   462391 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/multiobjective_optimization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/raytune_pytorch_cnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    63574 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/saasbo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/saasbo_nehvi.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   286300 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/scheduler.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   138095 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/tune_cnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-03-15 22:19:22.000000 ax-platform-0.3.1/tutorials/visualizations.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.603970 ax-platform-0.3.1/website/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.607970 ax-platform-0.3.1/website/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/core/Footer.js
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/core/Tutorial.js
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/core/TutorialSidebar.js
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.343963 ax-platform-0.3.1/website/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.607970 ax-platform-0.3.1/website/pages/en/
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/pages/en/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.607970 ax-platform-0.3.1/website/pages/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/pages/tutorials/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/sidebars.json
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/siteConfig.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.607970 ax-platform-0.3.1/website/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.607970 ax-platform-0.3.1/website/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/css/base_sphinx.css
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/css/custom_sphinx.css
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/css/pygments.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.611970 ax-platform-0.3.1/website/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/ax.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/ax_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/ax_lockup_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/ax_logo_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/ax_wireframe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/database-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/dice-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.611970 ax-platform-0.3.1/website/static/img/favicon/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/oss_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/img/th-large-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.611970 ax-platform-0.3.1/website/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/js/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/static/js/plotUtils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/tutorials.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.611970 ax-platform-0.3.1/website/versioned_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/versioned_docs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:22:33.611970 ax-platform-0.3.1/website/versioned_sidebars/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:19:22.000000 ax-platform-0.3.1/website/versioned_sidebars/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.856656 ax-platform-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.864657 ax-platform-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/reusable_tutorials.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/tutorials.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 20:41:24.000000 ax-platform-0.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-08 20:41:24.000000 ax-platform-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-08 20:41:24.000000 ax-platform-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-08 20:41:24.000000 ax-platform-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-08 20:45:14.172678 ax-platform-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-08 20:41:24.000000 ax-platform-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.868657 ax-platform-0.3.2/ax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.868657 ax-platform-0.3.2/ax/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.872657 ax-platform-0.3.2/ax/benchmark/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/choose_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/gpei_and_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/modular_botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/saasbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.872657 ax-platform-0.3.2/ax/benchmark/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hd_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.872657 ax-platform-0.3.2/ax/benchmark/problems/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hpo/pytorch_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hpo/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/surrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.876658 ax-platform-0.3.2/ax/benchmark/problems/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.876658 ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/mixed_integer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.876658 ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/jenatton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.880658 ax-platform-0.3.2/ax/benchmark/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_mixed_integer_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_problem_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.892659 ax-platform-0.3.2/ax/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/base_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27143 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/batch_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60990 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/formatting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/generator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/map_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/map_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/multi_type_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/optimization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/outcome_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25465 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/parameter_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/parameter_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45577 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/search_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.900659 ax-platform-0.3.2/ax/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_batch_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48974 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_formatting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_generator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_map_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_map_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_multi_type_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31569 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_optimization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_outcome_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17549 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_parameter_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_parameter_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44614 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.904660 ax-platform-0.3.2/ax/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.904660 ax-platform-0.3.2/ax/early_stopping/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/logical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/percentile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.904660 ax-platform-0.3.2/ax/early_stopping/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/tests/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.908660 ax-platform-0.3.2/ax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.908660 ax-platform-0.3.2/ax/global_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.908660 ax-platform-0.3.2/ax/global_stopping/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/strategies/improvement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.912660 ax-platform-0.3.2/ax/global_stopping/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/tests/tests_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.916660 ax-platform-0.3.2/ax/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/botorch_test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/branin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/branin_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/chemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31150 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/chemistry_data.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    20145 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/dict_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/hartmann6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/jenatton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/l2norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/noisy_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/noisy_function_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.920661 ax-platform-0.3.2/ax/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_chemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_dict_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_noisy_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/torchx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.932662 ax-platform-0.3.2/ax/modelbridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44868 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/completion_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/dispatch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/generation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40066 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/map_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58315 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/modelbridge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.932662 ax-platform-0.3.2/ax/modelbridge/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/strategies/alebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/strategies/rembo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.960663 ax-platform-0.3.2/ax/modelbridge/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_alebo_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32245 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_base_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_base_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_cap_parameter_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_cast_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_centered_unit_x_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_choice_encode_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_completion_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_convert_metric_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_derelativize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_discrete_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33932 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_dispatch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22595 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_generation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36153 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_int_range_to_choice_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_int_to_float_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_ivw_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_log_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_log_y_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_logit_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_map_torch_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_map_unit_x_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_merge_repeated_measurements_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_metrics_as_task_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_modelbridge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_one_hot_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_pairwise_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_percentile_y_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_power_transform_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_random_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_relativize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_rembo_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_remove_fixed_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_robust.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_search_space_to_choice_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_search_space_to_float_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_standardize_y_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_stratified_standardize_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_task_encode_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29980 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33129 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_transform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_trial_as_task_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_unit_x_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29969 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39444 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.972664 ax-platform-0.3.2/ax/modelbridge/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/cap_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/centered_unit_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/choice_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/convert_metric_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/derelativize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/int_range_to_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/int_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/ivw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/log_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/map_unit_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/merge_repeated_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/metrics_as_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/percentile_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/power_transform_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/relativize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/remove_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/search_space_to_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/search_space_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/standardize_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/stratified_standardize_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/task_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/trial_as_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/unit_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/winsorize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.976665 ax-platform-0.3.2/ax/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.976665 ax-platform-0.3.2/ax/models/discrete/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/eb_thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/full_factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22672 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.980665 ax-platform-0.3.2/ax/models/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/alebo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/rembo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/sobol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.992666 ax-platform-0.3.2/ax/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_alebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_alebo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_kg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_mes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_moo_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33596 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_moo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_cbo_lcea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_cbo_lcem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_cbo_sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_eb_thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_full_factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49865 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_posterior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_randomforest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_rembo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_rembo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_sobol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_torch_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.000666 ax-platform-0.3.2/ax/models/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29602 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/alebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24182 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_kg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_mes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.004667 ax-platform-0.3.2/ax/models/torch/botorch_modular/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/list_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/optimizer_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_moo_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/cbo_lcea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/cbo_lcem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/cbo_sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/frontier_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/fully_bayesian_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/posterior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/randomforest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/rembo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.004667 ax-platform-0.3.2/ax/models/torch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39724 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_optimizer_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/winsorization_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/bandit_rollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/contour.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/feature_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/js/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/css.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/helpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/plotly_offline.js
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/plotly_online.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/plotly_requires.js
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/generic_plotly.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/marginal_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38724 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/pareto_frontier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/pareto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58188 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/table_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.020668 ax-platform-0.3.2/ax/plot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.020668 ax-platform-0.3.2/ax/plot/tests/long_running/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/long_running/test_pareto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_contours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_feature_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_fitted_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_pareto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_tile_fitted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.024668 ax-platform-0.3.2/ax/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/botorch_test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/simulated_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.024668 ax-platform-0.3.2/ax/runners/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/tests/test_torchx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/torchx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.028668 ax-platform-0.3.2/ax/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78094 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/interactive_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/managed_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76782 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.032668 ax-platform-0.3.2/ax/service/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119626 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_best_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_best_point_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_global_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_instantiation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_interactive_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_managed_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19334 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51692 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_with_db_settings_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.036669 ax-platform-0.3.2/ax/service/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34580 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/best_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23798 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/best_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37588 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42578 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/scheduler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/with_db_settings_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.040669 ax-platform-0.3.2/ax/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/botorch_modular_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.044669 ax-platform-0.3.2/ax/storage/json_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28491 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.044669 ax-platform-0.3.2/ax/storage/json_store/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/tests/test_json_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/metric_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/registry_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/runner_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.052670 ax-platform-0.3.2/ax/storage/sqa_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49885 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44346 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/reduced_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/sqa_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/sqa_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/sqa_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.056670 ax-platform-0.3.2/ax/storage/sqa_store/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73084 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/test_sqa_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.056670 ax-platform-0.3.2/ax/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/tests/test_registry_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/transform_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.056670 ax-platform-0.3.2/ax/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.060670 ax-platform-0.3.2/ax/telemetry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.060670 ax-platform-0.3.2/ax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.068671 ax-platform-0.3.2/ax/utils/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/docutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/executils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.072671 ax-platform-0.3.2/ax/utils/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_docutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_executils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_kwargutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_typeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/typeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/typeutils_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/flake8_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/flake8_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/flake8_plugins/docstring_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/measurement/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/synthetic_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/measurement/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/tests/test_synthetic_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/notebook/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.080672 ax-platform-0.3.2/ax/utils/report/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/base_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/simple_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/sufficient_statistic.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.080672 ax-platform-0.3.2/ax/utils/report/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/tests/test_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.084672 ax-platform-0.3.2/ax/utils/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/derivative_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/derivative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35734 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/sobol_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.084672 ax-platform-0.3.2/ax/utils/sensitivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/tests/test_sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.084672 ax-platform-0.3.2/ax/utils/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/statstools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.088672 ax-platform-0.3.2/ax/utils/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/tests/test_statstools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.092673 ax-platform-0.3.2/ax/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/backend_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/backend_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/benchmark_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65879 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/core_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.092673 ax-platform-0.3.2/ax/utils/testing/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/metrics/backend_simulator_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/metrics/branin_backend_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/modeling_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/test_init_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.096673 ax-platform-0.3.2/ax/utils/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/tests/test_backend_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/torch_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.096673 ax-platform-0.3.2/ax/utils/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/tutorials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/tutorials/cnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.096673 ax-platform-0.3.2/ax_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.104674 ax-platform-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/algo-overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.116675 ax-platform-0.3.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    81587 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/bandit_allocation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   345484 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/bo_1d_opt.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   156260 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/contour.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/cv.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131612 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/example_shrinkage.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/fitted.js
+-rw-r--r--   0 runner    (1001) docker     (123)    65905 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/gp_opt.png
+-rw-r--r--   0 runner    (1001) docker     (123)   349223 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/gp_posterior.png
+-rw-r--r--   0 runner    (1001) docker     (123)   121838 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/mab_animate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   132372 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/mab_probs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   325134 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/mab_regret.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26226 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/slice.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/banditopt.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/bayesopt.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/core.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/data.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/glossary.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22509 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/storage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/trial-evaluation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/why-ax.md
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 20:41:24.000000 ax-platform-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 20:41:24.000000 ax-platform-0.3.2/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.124675 ax-platform-0.3.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/build_ax.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/docker_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/import_ax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/insert_api_refs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4160 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/make_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/make_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/parse_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/patch_site_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/publish_site.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/update_versions_html.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/validate_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/versions.js
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/wheels_build.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:45:14.172678 ax-platform-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-08 20:41:24.000000 ax-platform-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.124675 ax-platform-0.3.2/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.132676 ax-platform-0.3.2/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/ax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/early_stopping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/global_stopping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/modelbridge.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/runners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.148677 ax-platform-0.3.2/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    39419 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.148677 ax-platform-0.3.2/tutorials/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)   224156 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/early_stopping/early_stopping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/early_stopping/mnist_train_nas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/factorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25591 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/generation_strategy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/gpei_hartmann_developer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   273139 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/gpei_hartmann_loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/gpei_hartmann_service.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.160678 ax-platform-0.3.2/tutorials/human_in_the_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   634579 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)   276956 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/human_in_the_loop/human_in_the_loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    51566 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/modular_botax.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/multi_task.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   462391 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/multiobjective_optimization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/raytune_pytorch_cnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    63574 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/saasbo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/saasbo_nehvi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   286300 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/scheduler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   138095 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/tune_cnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/visualizations.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.160678 ax-platform-0.3.2/website/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.160678 ax-platform-0.3.2/website/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/core/Footer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/core/Tutorial.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/core/TutorialSidebar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.860656 ax-platform-0.3.2/website/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/pages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/pages/en/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/pages/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/pages/tutorials/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/sidebars.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/siteConfig.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/base_sphinx.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/custom_sphinx.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/pygments.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.168678 ax-platform-0.3.2/website/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_lockup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_lockup_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_logo_lockup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_wireframe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/database-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/dice-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.168678 ax-platform-0.3.2/website/static/img/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/favicon/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/oss_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/th-large-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/website/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/js/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/js/plotUtils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/tutorials.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/website/versioned_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/versioned_docs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/website/versioned_sidebars/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/versioned_sidebars/.gitkeep
```

### Comparing `ax-platform-0.3.1/.github/workflows/build-and-test.yml` & `ax-platform-0.3.2/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/.github/workflows/cron.yml` & `ax-platform-0.3.2/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/.github/workflows/deploy.yml` & `ax-platform-0.3.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/.github/workflows/reusable_tutorials.yml` & `ax-platform-0.3.2/.github/workflows/reusable_tutorials.yml`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/.gitignore` & `ax-platform-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/CODE_OF_CONDUCT.md` & `ax-platform-0.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/CONTRIBUTING.md` & `ax-platform-0.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/LICENSE` & `ax-platform-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/PKG-INFO` & `ax-platform-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ax-platform
-Version: 0.3.1
+Version: 0.3.2
 Summary: Adaptive Experimentation
 Home-page: https://github.com/facebook/Ax
 Author: Facebook, Inc.
 License: MIT
 Description: <img width="300" src="https://ax.dev/img/ax_logo_lockup.svg" alt="Ax Logo" />
         
         <hr/>
@@ -171,15 +171,15 @@
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
         export ALLOW_LATEST_GPYTORCH_LINOP=true
         pip install git+https://github.com/pytorch/botorch.git
         export ALLOW_BOTORCH_LATEST=true
         git clone https://github.com/facebook/ax.git --depth 1
         cd ax
-        pip install -e .[notebook,mysql,dev]
+        pip install -e .[unittest]
         ```
         
         See recommendation for installing PyTorch for MacOS users above.
         
         The above example limits the cloned directory size via the
         [`--depth`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---depthltdepthgt)
         argument to `git clone`. If you require the entire commit history you may remove this
```

### Comparing `ax-platform-0.3.1/README.md` & `ax-platform-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 pip install git+https://github.com/cornellius-gp/linear_operator.git
 pip install git+https://github.com/cornellius-gp/gpytorch.git
 export ALLOW_LATEST_GPYTORCH_LINOP=true
 pip install git+https://github.com/pytorch/botorch.git
 export ALLOW_BOTORCH_LATEST=true
 git clone https://github.com/facebook/ax.git --depth 1
 cd ax
-pip install -e .[notebook,mysql,dev]
+pip install -e .[unittest]
 ```
 
 See recommendation for installing PyTorch for MacOS users above.
 
 The above example limits the cloned directory size via the
 [`--depth`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---depthltdepthgt)
 argument to `git clone`. If you require the entire commit history you may remove this
```

### Comparing `ax-platform-0.3.1/ax/__init__.py` & `ax-platform-0.3.2/ax/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/benchmark.py` & `ax-platform-0.3.2/ax/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/benchmark_method.py` & `ax-platform-0.3.2/ax/benchmark/benchmark_method.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/benchmark_problem.py` & `ax-platform-0.3.2/ax/benchmark/benchmark_problem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/benchmark_result.py` & `ax-platform-0.3.2/ax/benchmark/benchmark_result.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/methods/choose_generation_strategy.py` & `ax-platform-0.3.2/ax/benchmark/methods/choose_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/methods/gpei_and_moo.py` & `ax-platform-0.3.2/ax/benchmark/methods/gpei_and_moo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/methods/modular_botorch.py` & `ax-platform-0.3.2/ax/benchmark/methods/modular_botorch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/methods/saasbo.py` & `ax-platform-0.3.2/ax/benchmark/methods/saasbo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/problems/hd_embedding.py` & `ax-platform-0.3.2/ax/benchmark/problems/hd_embedding.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/problems/hpo/pytorch_cnn.py` & `ax-platform-0.3.2/ax/benchmark/problems/hpo/pytorch_cnn.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/problems/hpo/torchvision.py` & `ax-platform-0.3.2/ax/benchmark/problems/hpo/torchvision.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/problems/registry.py` & `ax-platform-0.3.2/ax/benchmark/problems/registry.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,38 +10,38 @@
     BenchmarkProblem,
     MultiObjectiveBenchmarkProblem,
     SingleObjectiveBenchmarkProblem,
 )
 from ax.benchmark.problems.hd_embedding import embed_higher_dimension
 from ax.benchmark.problems.hpo.torchvision import PyTorchCNNTorchvisionBenchmarkProblem
 from ax.benchmark.problems.synthetic.hss.jenatton import get_jenatton_benchmark_problem
+from botorch.test_functions import synthetic
 from botorch.test_functions.multi_objective import BraninCurrin
-from botorch.test_functions.synthetic import Ackley, Branin, Hartmann, Powell
 
 
 @dataclass
 class BenchmarkProblemRegistryEntry:
     factory_fn: Callable[..., BenchmarkProblem]
     factory_kwargs: Dict[str, Any]
 
 
 BENCHMARK_PROBLEM_REGISTRY = {
-    "ackley": BenchmarkProblemRegistryEntry(
+    "ackley4": BenchmarkProblemRegistryEntry(
         factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
         factory_kwargs={
-            "test_problem_class": Ackley,
-            "test_problem_kwargs": {},
-            "num_trials": 50,
+            "test_problem_class": synthetic.Ackley,
+            "test_problem_kwargs": {"dim": 4},
+            "num_trials": 40,
             "infer_noise": True,
         },
     ),
     "branin": BenchmarkProblemRegistryEntry(
         factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
         factory_kwargs={
-            "test_problem_class": Branin,
+            "test_problem_class": synthetic.Branin,
             "test_problem_kwargs": {},
             "num_trials": 30,
             "infer_noise": True,
         },
     ),
     "branin_currin": BenchmarkProblemRegistryEntry(
         factory_fn=MultiObjectiveBenchmarkProblem.from_botorch_multi_objective,
@@ -60,27 +60,45 @@
                 num_trials=100,
                 infer_noise=True,
             ),
             total_dimensionality=n,
         ),
         factory_kwargs={"n": 30},
     ),
+    "griewank4": BenchmarkProblemRegistryEntry(
+        factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
+        factory_kwargs={
+            "test_problem_class": synthetic.Griewank,
+            "test_problem_kwargs": {"dim": 4},
+            "num_trials": 40,
+            "infer_noise": True,
+        },
+    ),
+    "hartmann3": BenchmarkProblemRegistryEntry(
+        factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
+        factory_kwargs={
+            "test_problem_class": synthetic.Hartmann,
+            "test_problem_kwargs": {"dim": 3},
+            "num_trials": 30,
+            "infer_noise": True,
+        },
+    ),
     "hartmann6": BenchmarkProblemRegistryEntry(
         factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
         factory_kwargs={
-            "test_problem_class": Hartmann,
+            "test_problem_class": synthetic.Hartmann,
             "test_problem_kwargs": {"dim": 6},
             "num_trials": 50,
             "infer_noise": True,
         },
     ),
     "hartmann30": BenchmarkProblemRegistryEntry(
         factory_fn=lambda n: embed_higher_dimension(
             problem=SingleObjectiveBenchmarkProblem.from_botorch_synthetic(
-                test_problem_class=Hartmann,
+                test_problem_class=synthetic.Hartmann,
                 test_problem_kwargs={"dim": 6},
                 num_trials=100,
                 infer_noise=True,
             ),
             total_dimensionality=n,
         ),
         factory_kwargs={"n": 30},
@@ -93,28 +111,64 @@
         factory_fn=PyTorchCNNTorchvisionBenchmarkProblem.from_dataset_name,
         factory_kwargs={"name": "FashionMNIST", "num_trials": 50, "infer_noise": True},
     ),
     "jenatton": BenchmarkProblemRegistryEntry(
         factory_fn=get_jenatton_benchmark_problem,
         factory_kwargs={"num_trials": 50, "infer_noise": True},
     ),
-    "powell": BenchmarkProblemRegistryEntry(
+    "levy4": BenchmarkProblemRegistryEntry(
         factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
         factory_kwargs={
-            "test_problem_class": Powell,
+            "test_problem_class": synthetic.Levy,
+            "test_problem_kwargs": {"dim": 4},
+            "num_trials": 40,
+            "infer_noise": True,
+        },
+    ),
+    "powell4": BenchmarkProblemRegistryEntry(
+        factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
+        factory_kwargs={
+            "test_problem_class": synthetic.Powell,
+            "test_problem_kwargs": {"dim": 4},
+            "num_trials": 40,
+            "infer_noise": True,
+        },
+    ),
+    "rosenbrock4": BenchmarkProblemRegistryEntry(
+        factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
+        factory_kwargs={
+            "test_problem_class": synthetic.Rosenbrock,
+            "test_problem_kwargs": {"dim": 4},
+            "num_trials": 40,
+            "infer_noise": True,
+        },
+    ),
+    "six_hump_camel": BenchmarkProblemRegistryEntry(
+        factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
+        factory_kwargs={
+            "test_problem_class": synthetic.SixHumpCamel,
             "test_problem_kwargs": {},
-            "num_trials": 50,
+            "num_trials": 30,
+            "infer_noise": True,
+        },
+    ),
+    "three_hump_camel": BenchmarkProblemRegistryEntry(
+        factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
+        factory_kwargs={
+            "test_problem_class": synthetic.ThreeHumpCamel,
+            "test_problem_kwargs": {},
+            "num_trials": 30,
             "infer_noise": True,
         },
     ),
     # Problems without inferred noise
     "branin_fixed_noise": BenchmarkProblemRegistryEntry(
         factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
         factory_kwargs={
-            "test_problem_class": Branin,
+            "test_problem_class": synthetic.Branin,
             "test_problem_kwargs": {},
             "num_trials": 30,
             "infer_noise": False,
         },
     ),
     "branin_currin_fixed_noise": BenchmarkProblemRegistryEntry(
         factory_fn=MultiObjectiveBenchmarkProblem.from_botorch_multi_objective,
@@ -136,24 +190,24 @@
             total_dimensionality=n,
         ),
         factory_kwargs={"n": 30},
     ),
     "hartmann6_fixed_noise": BenchmarkProblemRegistryEntry(
         factory_fn=SingleObjectiveBenchmarkProblem.from_botorch_synthetic,
         factory_kwargs={
-            "test_problem_class": Hartmann,
+            "test_problem_class": synthetic.Hartmann,
             "test_problem_kwargs": {"dim": 6},
             "num_trials": 50,
             "infer_noise": False,
         },
     ),
     "hartmann30_fixed_noise": BenchmarkProblemRegistryEntry(
         factory_fn=lambda n: embed_higher_dimension(
             problem=SingleObjectiveBenchmarkProblem.from_botorch_synthetic(
-                test_problem_class=Hartmann,
+                test_problem_class=synthetic.Hartmann,
                 test_problem_kwargs={"dim": 6},
                 num_trials=100,
                 infer_noise=False,
             ),
             total_dimensionality=n,
         ),
         factory_kwargs={"n": 30},
```

### Comparing `ax-platform-0.3.1/ax/benchmark/problems/synthetic/discretized/mixed_integer.py` & `ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/mixed_integer.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,28 +37,29 @@
     bounds: List[Tuple[float, float]],
     dim_int: int,
     metric_name: str,
     infer_noise: bool,
     test_problem_class: Type[SyntheticTestFunction],
     benchmark_name: str,
     num_trials: int,
-    modified_bounds: Optional[List[Tuple[float, float]]] = None,
+    test_problem_bounds: Optional[List[Tuple[float, float]]] = None,
 ) -> BenchmarkProblem:
     """This is a helper that deduplicates common bits of the below problems.
 
     Args:
         bounds: The parameter bounds.
         dim_int: The number of integer dimensions. First `dim_int` parameters
             are assumed to be integers.
         metric_name: The name of the metric.
         infer_noise: Whether to infer noise or assume noise-free objective.
         test_problem_class: The BoTorch test problem class.
         benchmark_name: The name of the benchmark problem.
         num_trials: The number of trials.
-        modified_bounds: Optional bounds to evaluate the base test problem on.
+        test_problem_bounds: Optional bounds to evaluate the base test problem on.
+            These are passed in as `bounds` while initializing the test problem.
 
     Returns:
         A mixed-integer BenchmarkProblem constructed from the given inputs.
     """
     dim = len(bounds)
     search_space = SearchSpace(
         parameters=[
@@ -79,19 +80,20 @@
                 name=metric_name,
                 noise_sd=None if infer_noise else 0.0,
             ),
             minimize=True,
         )
     )
     test_problem_kwargs: Dict[str, Any] = {"dim": dim}
-    if modified_bounds is not None:
-        test_problem_kwargs["bounds"] = modified_bounds
+    if test_problem_bounds is not None:
+        test_problem_kwargs["bounds"] = test_problem_bounds
     runner = BotorchTestProblemRunner(
         test_problem_class=test_problem_class,
         test_problem_kwargs=test_problem_kwargs,
+        modified_bounds=bounds,
     )
     return BenchmarkProblem(
         name=benchmark_name,
         search_space=search_space,
         optimization_config=optimization_config,
         runner=runner,
         num_trials=num_trials,
@@ -147,15 +149,15 @@
         bounds=bounds,
         dim_int=dim_int,
         metric_name="Ackley",
         infer_noise=infer_noise,
         test_problem_class=Ackley,
         benchmark_name="Discrete Ackley",
         num_trials=num_trials,
-        modified_bounds=[(0.0, 1.0)] * dim,
+        test_problem_bounds=[(0.0, 1.0)] * dim,
     )
 
 
 def get_discrete_rosenbrock(
     num_trials: int = 50,
     infer_noise: bool = True,
     bounds: Optional[List[Tuple[float, float]]] = None,
```

### Comparing `ax-platform-0.3.1/ax/benchmark/problems/synthetic/hss/jenatton.py` & `ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/jenatton.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/tests/test_benchmark.py` & `ax-platform-0.3.2/ax/benchmark/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/tests/test_benchmark_method.py` & `ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_method.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/tests/test_benchmark_problem.py` & `ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_problem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/tests/test_problem_storage.py` & `ax-platform-0.3.2/ax/benchmark/tests/test_problem_storage.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/benchmark/tests/test_problems.py` & `ax-platform-0.3.2/ax/benchmark/tests/test_problems.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/__init__.py` & `ax-platform-0.3.2/ax/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/arm.py` & `ax-platform-0.3.2/ax/core/arm.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/base_trial.py` & `ax-platform-0.3.2/ax/core/base_trial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/batch_trial.py` & `ax-platform-0.3.2/ax/core/batch_trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,17 +304,18 @@
             GeneratorRunStruct(generator_run=generator_run, weight=multiplier)
         )
         generator_run.index = len(self._generator_run_structs) - 1
 
         if self.status_quo is not None and self.optimize_for_power:
             self.set_status_quo_and_optimize_power(status_quo=not_none(self.status_quo))
 
-        self._set_generation_step_index(
-            generation_step_index=generator_run._generation_step_index
-        )
+        if generator_run._generation_step_index is not None:
+            self._set_generation_step_index(
+                generation_step_index=generator_run._generation_step_index
+            )
         self._refresh_arms_by_name()
         return self
 
     @property
     def status_quo(self) -> Optional[Arm]:
         """The control arm for this batch."""
         return self._status_quo
```

### Comparing `ax-platform-0.3.1/ax/core/data.py` & `ax-platform-0.3.2/ax/core/data.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/experiment.py` & `ax-platform-0.3.2/ax/core/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -830,21 +830,21 @@
             if isinstance(result, Err):
                 logger.error(
                     "Discovered Metric fetching Err while attaching data "
                     f"{result.err}. "
                     "Ignoring for now -- will retry query on next call to fetch."
                 )
 
+        if len(oks) < 1:
+            return None
+
         data = self.default_data_constructor.from_multiple_data(
             data=[ok.ok for ok in oks]
         )
 
-        if data.df.empty:
-            return None
-
         return self.attach_data(
             data=data,
             combine_with_last_data=combine_with_last_data,
             overwrite_existing_data=overwrite_existing_data,
         )
 
     def lookup_data_for_ts(self, timestamp: int) -> Data:
```

### Comparing `ax-platform-0.3.1/ax/core/formatting_utils.py` & `ax-platform-0.3.2/ax/core/formatting_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/generator_run.py` & `ax-platform-0.3.2/ax/core/generator_run.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/map_data.py` & `ax-platform-0.3.2/ax/core/map_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from logging import Logger
-from typing import Any, Dict, Generic, Iterable, List, Optional, Type, TypeVar
+from typing import Any, Dict, Generic, Iterable, List, Optional, Sequence, Type, TypeVar
 
 import numpy as np
 
 import pandas as pd
 from ax.core.data import Data
 from ax.core.types import TMapTrialEvaluation
 from ax.exceptions.core import UnsupportedError
@@ -158,17 +158,20 @@
     # pyre-fixme[24]: Generic type `type` expects 1 type parameter, use
     #  `typing.Type` to avoid runtime subscripting errors.
     def map_key_to_type(self) -> Dict[str, Type]:
         return {mki.key: mki.value_type for mki in self.map_key_infos}
 
     @staticmethod
     def from_multiple_map_data(
-        data: Iterable[MapData],
+        data: Sequence[MapData],
         subset_metrics: Optional[Iterable[str]] = None,
     ) -> MapData:
+        if len(data) == 0:
+            return MapData()
+
         unique_map_key_infos = []
         for mki in (mki for datum in data for mki in datum.map_key_infos):
             if any(
                 mki.key == unique.key and mki.default_value != unique.default_value
                 for unique in unique_map_key_infos
             ):
                 logger.warning(f"MapKeyInfo conflict for {mki.key}, eliding {mki}.")
@@ -179,19 +182,19 @@
                     unique_map_key_infos.append(mki)
 
         df = pd.concat(
             [pd.DataFrame(columns=[mki.key for mki in unique_map_key_infos])]
             + [datum.map_df for datum in data]
         ).fillna(value={mki.key: mki.default_value for mki in unique_map_key_infos})
 
-        subset_metrics_mask = df["metric_name"].isin(
-            subset_metrics if subset_metrics else df["metric_name"]
-        )
+        if subset_metrics:
+            subset_metrics_mask = df["metric_name"].isin(subset_metrics)
+            df = df[subset_metrics_mask]
 
-        return MapData(df=df[subset_metrics_mask], map_key_infos=unique_map_key_infos)
+        return MapData(df=df, map_key_infos=unique_map_key_infos)
 
     @staticmethod
     def from_map_evaluations(
         evaluations: Dict[str, TMapTrialEvaluation],
         trial_index: int,
         # pyre-fixme[24]: Generic type `MapKeyInfo` expects 1 type parameter.
         map_key_infos: Optional[Iterable[MapKeyInfo]] = None,
```

### Comparing `ax-platform-0.3.1/ax/core/map_metric.py` & `ax-platform-0.3.2/ax/core/map_metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from typing import Type
 
-from ax.core.map_data import MapData
+from ax.core.map_data import MapData, MapKeyInfo
 from ax.core.metric import Metric, MetricFetchE
 from ax.utils.common.result import Result
 
 MapMetricFetchResult = Result[MapData, MetricFetchE]
 
 
 class MapMetric(Metric):
@@ -26,7 +26,8 @@
 
     Attributes:
         lower_is_better: Flag for metrics which should be minimized.
         properties: Properties specific to a particular metric.
     """
 
     data_constructor: Type[MapData] = MapData
+    map_key_info: MapKeyInfo[float] = MapKeyInfo(key="steps", default_value=0.0)
```

### Comparing `ax-platform-0.3.1/ax/core/metric.py` & `ax-platform-0.3.2/ax/core/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,18 @@
             try:
                 fetched_trial_data = cls.fetch_experiment_data_multi(
                     experiment=experiment,
                     metrics=metrics_to_fetch,
                     trials=[trial],
                     **kwargs,
                 )[trial.index]
-                contains_new_data = True
+
+                contains_new_data = any(
+                    result.is_ok() for result in fetched_trial_data.values()
+                )
             except NotImplementedError:
                 # Metric does not implement fetching logic and only uses lookup.
                 fetched_trial_data = {}
 
             trials_results[trial.index] = {
                 **cls._wrap_trial_data_multi(data=cached_trial_data),
                 **fetched_trial_data,
```

### Comparing `ax-platform-0.3.1/ax/core/multi_type_experiment.py` & `ax-platform-0.3.2/ax/core/multi_type_experiment.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/objective.py` & `ax-platform-0.3.2/ax/core/objective.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/observation.py` & `ax-platform-0.3.2/ax/core/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,17 +266,19 @@
             be included in the observations, returned from this function.
         map_keys_as_parameters: Whether map_keys should be returned as part of
             the parameters of the Observation objects.
 
     Returns:
         List of Observation objects.
     """
+    if len(cols) == 0:
+        return []
     observations = []
     abandoned_arms_dict = {}
-    for g, d in df.groupby(by=cols):
+    for g, d in df.groupby(by=cols if len(cols) > 1 else cols[0]):
         obs_kwargs = {}
         if arm_name_only:
             features = {"arm_name": g}
             arm_name = g
             trial_index = None
         else:
             features = dict(zip(cols, g))
@@ -488,15 +490,19 @@
     )
 
     if set(feature_cols) == set(complete_feature_cols):
         complete_df = map_data.map_df
         incomplete_df = None
     else:
         # The groupby and filter is expensive, so do it only if we have to.
-        grouped = map_data.map_df.groupby(by=complete_feature_cols)
+        grouped = map_data.map_df.groupby(
+            by=complete_feature_cols
+            if len(complete_feature_cols) > 1
+            else complete_feature_cols[0]
+        )
         complete_df = grouped.filter(lambda r: ~r[feature_cols].isnull().any().any())
         incomplete_df = grouped.filter(lambda r: r[feature_cols].isnull().any().any())
 
     # Get Observations from complete_df
     observations.extend(
         _observations_from_dataframe(
             experiment=experiment,
```

### Comparing `ax-platform-0.3.1/ax/core/optimization_config.py` & `ax-platform-0.3.2/ax/core/optimization_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/outcome_constraint.py` & `ax-platform-0.3.2/ax/core/outcome_constraint.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/parameter.py` & `ax-platform-0.3.2/ax/core/parameter.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 from warnings import warn
 
 from ax.core.types import TParamValue
 from ax.exceptions.core import UserInputError
 from ax.utils.common.base import SortableBase
 from ax.utils.common.typeutils import not_none
 
+# Tolerance for floating point comparisons. This is relatively permissive,
+# and allows for serializing at rather low numerical precision.
+# TODO: Do a more comprehensive audit of how floating point precision issues
+# may creep up and implement a more principled fix
+EPS = 1.5e-7
 
 FIXED_CHOICE_PARAM_ERROR = (
     "ChoiceParameters require multiple feasible values. "
     "Please use FixedParameter instead when setting a single possible value."
 )
 
 
@@ -224,14 +229,23 @@
         # pyre-fixme[58]: `>=` is not supported for operand types `Union[None, bool,
         #  float, int, str]` and `Union[None, bool, float, int, str]`.
         if lower >= upper:
             raise UserInputError(
                 f"Upper bound of {self.name} must be strictly larger than lower."
                 f"Got: ({lower}, {upper})."
             )
+        # pyre-fixme[58]: `-` is not supported for operand types `Union[None, bool,
+        #  float, int, str]` and `Union[None, bool, float, int, str]`.
+        width: float = upper - lower
+        if width < 100 * EPS:
+            raise UserInputError(
+                f"Parameter range ({width}) is very small and likely "
+                "to cause numerical errors. Consider reparameterizing your "
+                "problem by scaling the parameter."
+            )
         if log_scale and logit_scale:
             raise UserInputError("Can't use both log and logit.")
         # pyre-fixme[58]: `<=` is not supported for operand types `Union[None, bool,
         #  float, int, str]` and `int`.
         if log_scale and lower <= 0:
             raise UserInputError("Cannot take log when min <= 0.")
         # pyre-fixme[58]: `<=` is not supported for operand types `Union[None, bool,
@@ -328,32 +342,37 @@
         self._log_scale = log_scale
         return self
 
     def set_logit_scale(self, logit_scale: bool) -> RangeParameter:
         self._logit_scale = logit_scale
         return self
 
-    def validate(self, value: TParamValue) -> bool:
+    def validate(self, value: TParamValue, tol: float = EPS) -> bool:
         """Returns True if input is a valid value for the parameter.
 
         Checks that value is of the right type and within
         the valid range for the parameter. Returns False if value is None.
 
         Args:
             value: Value being checked.
+            tol: Absolute tolerance for floating point comparisons.
 
         Returns:
             True if valid, False otherwise.
         """
         if value is None:
             return False
 
         if not self.is_valid_type(value):
             return False
-        return value >= self._lower and value <= self._upper
+        # pyre-fixme[58]: `>=` is not supported for operand types `Union[bool,
+        #  float, int, str]` and `float`.
+        # pyre-fixme[58]: `<=` is not supported for operand types `Union[bool,
+        #  float, int, str]` and `float`.
+        return value >= self._lower - tol and value <= self._upper + tol
 
     def is_valid_type(self, value: TParamValue) -> bool:
         """Same as default except allows floats whose value is an int
         for Int parameters.
         """
         if not (isinstance(value, float) or isinstance(value, int)):
             return False
```

### Comparing `ax-platform-0.3.1/ax/core/parameter_constraint.py` & `ax-platform-0.3.2/ax/core/parameter_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,19 @@
         return self._constraint_dict
 
     @property
     def op(self) -> ComparisonOp:
         """Whether the sum is constrained by a <= or >= inequality."""
         return ComparisonOp.LEQ if self._is_upper_bound else ComparisonOp.GEQ
 
+    @property
+    def is_upper_bound(self) -> bool:
+        """Whether the bound is an upper or lower bound on the sum."""
+        return self._is_upper_bound
+
     def clone(self) -> SumConstraint:
         """Clone.
 
         To use the same constraint, we need to reconstruct the original bound.
         We do this by re-applying the original bound weighting.
         """
         return SumConstraint(
```

### Comparing `ax-platform-0.3.1/ax/core/parameter_distribution.py` & `ax-platform-0.3.2/ax/core/parameter_distribution.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/risk_measures.py` & `ax-platform-0.3.2/ax/core/risk_measures.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/runner.py` & `ax-platform-0.3.2/ax/core/runner.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/search_space.py` & `ax-platform-0.3.2/ax/core/search_space.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_arm.py` & `ax-platform-0.3.2/ax/core/tests/test_arm.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_batch_trial.py` & `ax-platform-0.3.2/ax/core/tests/test_batch_trial.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,32 +92,37 @@
         self.batch.add_arm(Arm(arm_parameters), 3)
 
         self.assertEqual(self.batch.arms_by_name["0_2"], self.batch.arms[2])
         self.assertEqual(len(self.batch.arms), len(self.arms) + 1)
         self.assertEqual(len(self.batch.generator_run_structs), 2)
         self.assertEqual(sum(self.batch.weights), sum(self.weights) + 3)
 
-    def testAddGeneratorRun(self) -> None:
+    def test_add_generator_run(self) -> None:
         self.assertEqual(len(self.batch.arms), len(self.arms))
         self.assertEqual(len(self.batch.generator_run_structs), 1)
         self.assertEqual(sum(self.batch.weights), sum(self.weights))
 
+        # Overwrite the GS index to not-None.
+        self.batch._generation_step_index = 0
+
         # one of these arms already exists on the BatchTrial,
         # so we should just update its weight
         new_arms = [
             Arm(parameters={"w": 0.75, "x": 1, "y": "foo", "z": True}),
             Arm(parameters={"w": 1.4, "x": 5, "y": "bar", "z": False}),
         ]
         new_weights = [0.75, 0.25]
         gr = GeneratorRun(arms=new_arms, weights=new_weights)
         self.batch.add_generator_run(gr, 2.0)
 
         self.assertEqual(len(self.batch.arms), len(self.arms) + 1)
         self.assertEqual(len(self.batch.generator_run_structs), 2)
         self.assertEqual(sum(self.batch.weights), sum(self.weights) + 2)
+        # Check the GS index was not overwritten to None.
+        self.assertEqual(self.batch._generation_step_index, 0)
 
     def testInitWithGeneratorRun(self) -> None:
         generator_run = GeneratorRun(arms=self.arms, weights=self.weights)
         batch = self.experiment.new_batch_trial(generator_run=generator_run)
         batch.add_arms_and_weights(arms=self.arms, weights=self.weights)
         self.assertEqual(self.batch.arms_by_name["0_0"], self.batch.arms[0])
         self.assertEqual(self.batch.arms_by_name["0_1"], self.batch.arms[1])
```

### Comparing `ax-platform-0.3.1/ax/core/tests/test_data.py` & `ax-platform-0.3.2/ax/core/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_experiment.py` & `ax-platform-0.3.2/ax/core/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_formatting_utils.py` & `ax-platform-0.3.2/ax/core/tests/test_formatting_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_generator_run.py` & `ax-platform-0.3.2/ax/core/tests/test_generator_run.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_map_data.py` & `ax-platform-0.3.2/ax/core/tests/test_map_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 
     def test_properties(self) -> None:
         self.assertEqual(self.mmd.map_key_infos, self.map_key_infos)
         self.assertEqual(self.mmd.map_keys, ["epoch"])
         self.assertEqual(self.mmd.map_key_to_type, {"epoch": int})
 
     def test_combine(self) -> None:
+        data = MapData.from_multiple_map_data([])
+        self.assertEqual(data.map_df.size, 0)
+
         mmd_double = MapData.from_multiple_map_data([self.mmd, self.mmd])
         self.assertEqual(mmd_double.map_df.size, 2 * self.mmd.map_df.size)
         self.assertEqual(mmd_double.map_key_infos, self.mmd.map_key_infos)
 
         different_map_df = pd.DataFrame(
             [
                 {
```

### Comparing `ax-platform-0.3.1/ax/core/tests/test_map_metric.py` & `ax-platform-0.3.2/ax/core/tests/test_map_metric.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_metric.py` & `ax-platform-0.3.2/ax/core/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_multi_type_experiment.py` & `ax-platform-0.3.2/ax/core/tests/test_multi_type_experiment.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_objective.py` & `ax-platform-0.3.2/ax/core/tests/test_objective.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_observation.py` & `ax-platform-0.3.2/ax/core/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_optimization_config.py` & `ax-platform-0.3.2/ax/core/tests/test_optimization_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_outcome_constraint.py` & `ax-platform-0.3.2/ax/core/tests/test_outcome_constraint.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_parameter.py` & `ax-platform-0.3.2/ax/core/tests/test_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from ax.core.parameter import (
     _get_parameter_type,
     ChoiceParameter,
+    EPS,
     FixedParameter,
     ParameterType,
     RangeParameter,
 )
 from ax.exceptions.core import UserInputError
 from ax.utils.common.testutils import TestCase
 
@@ -69,14 +70,18 @@
         self.assertIsNone(self.param2.target_value)
 
     def testValidate(self) -> None:
         self.assertFalse(self.param1.validate(None))
         self.assertFalse(self.param1.validate("foo"))
         self.assertTrue(self.param1.validate(1))
         self.assertTrue(self.param1.validate(1.3))
+        self.assertFalse(self.param1.validate(3.5))
+        # Check with tolerances
+        self.assertTrue(self.param1.validate(1 - 0.5 * EPS))
+        self.assertTrue(self.param1.validate(3 + 0.5 * EPS))
 
     def testRepr(self) -> None:
         self.assertEqual(str(self.param1), self.param1_repr)
         self.assertEqual(str(self.param2), self.param2_repr)
 
     def testBadCreations(self) -> None:
         with self.assertRaises(UserInputError):
@@ -90,14 +95,20 @@
 
         with self.assertRaises(UserInputError):
             RangeParameter("x", ParameterType.INT, 0.5, 1)
 
         with self.assertRaises(UserInputError):
             RangeParameter("x", ParameterType.INT, 0.5, 1, is_fidelity=True)
 
+        with self.assertRaisesRegex(
+            UserInputError,
+            "likely to cause numerical errors. Consider reparameterizing",
+        ):
+            RangeParameter("x", ParameterType.FLOAT, EPS, 2 * EPS)
+
     def testBadSetter(self) -> None:
         with self.assertRaises(ValueError):
             # pyre-fixme[6]: For 1st param expected `Optional[float]` but got `str`.
             self.param1.update_range(upper="foo")
 
         with self.assertRaises(ValueError):
             # pyre-fixme[6]: For 1st param expected `Optional[float]` but got `str`.
```

### Comparing `ax-platform-0.3.1/ax/core/tests/test_parameter_constraint.py` & `ax-platform-0.3.2/ax/core/tests/test_parameter_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,18 @@
             # pyre-fixme[16]: `SumConstraintTest` has no attribute `constraint`.
             self.constraint = SumConstraint(
                 parameters=[self.x, z], is_upper_bound=False, bound=-5.0
             )
 
     def testProperties(self) -> None:
         self.assertEqual(self.constraint1.op, ComparisonOp.LEQ)
+        self.assertTrue(self.constraint1._is_upper_bound)
+
         self.assertEqual(self.constraint2.op, ComparisonOp.GEQ)
+        self.assertFalse(self.constraint2._is_upper_bound)
 
     def testRepr(self) -> None:
         self.assertEqual(str(self.constraint1), self.constraint_repr1)
         self.assertEqual(str(self.constraint2), self.constraint_repr2)
 
     def testValidate(self) -> None:
         self.assertTrue(self.constraint1.check({"x": 1, "y": 4}))
```

### Comparing `ax-platform-0.3.1/ax/core/tests/test_parameter_distribution.py` & `ax-platform-0.3.2/ax/core/tests/test_parameter_distribution.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_risk_measures.py` & `ax-platform-0.3.2/ax/core/tests/test_risk_measures.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_runner.py` & `ax-platform-0.3.2/ax/core/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_search_space.py` & `ax-platform-0.3.2/ax/core/tests/test_search_space.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_trial.py` & `ax-platform-0.3.2/ax/core/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/tests/test_types.py` & `ax-platform-0.3.2/ax/core/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/trial.py` & `ax-platform-0.3.2/ax/core/trial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/types.py` & `ax-platform-0.3.2/ax/core/types.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/core/utils.py` & `ax-platform-0.3.2/ax/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Dict, Iterable, NamedTuple, Set, Tuple
+from typing import Dict, Iterable, List, NamedTuple, Optional, Set, Tuple
 
 import numpy as np
+from ax.core.base_trial import BaseTrial
 from ax.core.batch_trial import BatchTrial
 from ax.core.data import Data
 from ax.core.experiment import Experiment
+from ax.core.generator_run import GeneratorRun
 from ax.core.objective import MultiObjective
 from ax.core.optimization_config import OptimizationConfig
 
 from ax.core.trial import Trial
 from ax.core.types import ComparisonOp
-from ax.utils.common.typeutils import not_none
+from pyre_extensions import none_throws
 
 TArmTrial = Tuple[str, int]
 
 
 # --------------------------- Data intergrity utils. ---------------------------
 
 
@@ -144,25 +146,45 @@
 
     # Get cumulative best
     minimize = objective.minimize
     accumulate = np.minimum.accumulate if minimize else np.maximum.accumulate
     return accumulate(f)
 
 
+def _extract_generator_run(trial: BaseTrial) -> GeneratorRun:
+    if isinstance(trial, BatchTrial):
+        if len(trial.generator_run_structs) > 1:
+            raise NotImplementedError(
+                "Run time is not supported with multiple generator runs per trial."
+            )
+        return trial._generator_run_structs[0].generator_run
+    if isinstance(trial, Trial):
+        return none_throws(trial.generator_run)
+    raise ValueError("Unexpected trial type")  # pragma: no cover
+
+
+def get_model_trace_of_times(
+    experiment: Experiment,
+) -> Tuple[List[Optional[float]], List[Optional[float]]]:
+    """
+    Get time spent fitting the model and generating candidates during each trial.
+    Not cumulative.
+
+    Returns:
+        List of fit times, list of gen times.
+    """
+    generator_runs = [
+        _extract_generator_run(trial=trial) for trial in experiment.trials.values()
+    ]
+    fit_times = [gr.fit_time for gr in generator_runs]
+    gen_times = [gr.gen_time for gr in generator_runs]
+    return fit_times, gen_times
+
+
 def get_model_times(experiment: Experiment) -> Tuple[float, float]:  # pragma: no cover
     """Get total times spent fitting the model and generating candidates in the
     course of the experiment.
     """
-    fit_time = 0.0
-    gen_time = 0.0
-    for trial in experiment.trials.values():
-        if isinstance(trial, BatchTrial):  # pragma: no cover
-            gr = trial._generator_run_structs[0].generator_run
-        elif isinstance(trial, Trial):
-            gr = not_none(trial.generator_run)
-        else:
-            raise ValueError("Unexpected trial type")  # pragma: no cover
-        if gr.fit_time is not None:
-            fit_time += not_none(gr.fit_time)
-        if gr.gen_time is not None:
-            gen_time += not_none(gr.gen_time)
+    fit_times, gen_times = get_model_trace_of_times(experiment)
+    fit_time = sum((t for t in fit_times if t is not None))
+    gen_time = sum((t for t in gen_times if t is not None))
     return fit_time, gen_time
```

### Comparing `ax-platform-0.3.1/ax/early_stopping/strategies/__init__.py` & `ax-platform-0.3.2/ax/early_stopping/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/early_stopping/strategies/base.py` & `ax-platform-0.3.2/ax/early_stopping/strategies/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import numpy as np
 import pandas as pd
 from ax.core.base_trial import TrialStatus
 from ax.core.data import Data
 from ax.core.experiment import Experiment
 from ax.core.map_data import MapData
+from ax.core.objective import MultiObjective
 from ax.modelbridge.map_torch import MapTorchModelBridge
 from ax.modelbridge.modelbridge_utils import (
     _unpack_observations,
     observation_data_to_array,
     observation_features_to_array,
 )
 
@@ -363,16 +364,23 @@
         return True, None
 
     def _default_objective_and_direction(
         self, experiment: Experiment
     ) -> Tuple[str, bool]:
         if self.metric_names is None:
             optimization_config = not_none(experiment.optimization_config)
-            metric_name = optimization_config.objective.metric.name
-            minimize = optimization_config.objective.minimize
+            objective = optimization_config.objective
+
+            # if multi-objective optimization, infer as first objective
+            # although it is recommended to specify a metric name(s) explicitly.
+            if isinstance(objective, MultiObjective):
+                objective = objective.objectives[0]
+
+            metric_name = objective.metric.name
+            minimize = objective.minimize
         else:
             metric_name = list(self.metric_names)[0]
             minimize = experiment.metrics[metric_name].lower_is_better or False
         return metric_name, minimize
 
 
 class ModelBasedEarlyStoppingStrategy(BaseEarlyStoppingStrategy):
```

### Comparing `ax-platform-0.3.1/ax/early_stopping/strategies/logical.py` & `ax-platform-0.3.2/ax/early_stopping/strategies/logical.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/early_stopping/strategies/percentile.py` & `ax-platform-0.3.2/ax/early_stopping/strategies/percentile.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/early_stopping/strategies/threshold.py` & `ax-platform-0.3.2/ax/early_stopping/strategies/threshold.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/early_stopping/tests/test_strategies.py` & `ax-platform-0.3.2/ax/early_stopping/tests/test_strategies.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,26 +26,117 @@
 from ax.exceptions.core import UnsupportedError
 from ax.utils.common.testutils import TestCase
 from ax.utils.common.typeutils import checked_cast
 from ax.utils.testing.core_stubs import (
     get_branin_arms,
     get_branin_experiment,
     get_branin_experiment_with_timestamp_map_metric,
+    get_experiment_with_multi_objective,
     get_test_map_data_experiment,
 )
+from pyre_extensions import none_throws
 
 
 class TestBaseEarlyStoppingStrategy(TestCase):
     def test_early_stopping_strategy(self) -> None:
         # can't instantiate abstract class
         with self.assertRaises(TypeError):
             # pyre-fixme[45]: Cannot instantiate abstract class
             #  `BaseEarlyStoppingStrategy`.
             BaseEarlyStoppingStrategy()
 
+    def test_default_objective_and_direction(self) -> None:
+        class FakeStrategy(BaseEarlyStoppingStrategy):
+            def should_stop_trials_early(
+                self,
+                trial_indices: Set[int],
+                experiment: Experiment,
+                **kwargs: Dict[str, Any],
+            ) -> Dict[int, Optional[str]]:
+                return {}
+
+        test_experiment = get_test_map_data_experiment(
+            num_trials=3, num_fetches=5, num_complete=3
+        )
+        test_objective = none_throws(test_experiment.optimization_config).objective
+        with self.subTest("provide metric names"):
+            es_strategy = FakeStrategy(metric_names=[test_objective.metric.name])
+            (
+                actual_metric_name,
+                actual_minimize,
+            ) = es_strategy._default_objective_and_direction(experiment=test_experiment)
+
+            self.assertEqual(
+                actual_metric_name,
+                test_objective.metric.name,
+            )
+            self.assertEqual(
+                actual_minimize,
+                test_objective.minimize,
+            )
+
+        with self.subTest("infer from optimization config"):
+            # should be the same as above
+            es_strategy = FakeStrategy()
+            (
+                actual_metric_name,
+                actual_minimize,
+            ) = es_strategy._default_objective_and_direction(experiment=test_experiment)
+
+            self.assertEqual(
+                actual_metric_name,
+                test_objective.metric.name,
+            )
+            self.assertEqual(
+                actual_minimize,
+                test_objective.minimize,
+            )
+
+        test_multi_objective_experiment = get_experiment_with_multi_objective()
+        test_multi_objective = none_throws(
+            test_multi_objective_experiment.optimization_config
+        ).objective
+        with self.subTest("infer from optimization config -- multi-objective"):
+            es_strategy = FakeStrategy()
+            (
+                actual_metric_name,
+                actual_minimize,
+            ) = es_strategy._default_objective_and_direction(
+                experiment=test_multi_objective_experiment
+            )
+            self.assertEqual(
+                actual_metric_name,
+                # pyre-fixme[16]: we know this is a MultiObjective
+                # which has attribute `objectives`
+                test_multi_objective.objectives[0].metric.name,
+            )
+            self.assertEqual(
+                actual_minimize,
+                test_multi_objective.objectives[0].minimize,
+            )
+
+        with self.subTest("provide metric names -- multi-objective"):
+            es_strategy = FakeStrategy(
+                metric_names=[test_multi_objective.objectives[1].metric.name]
+            )
+            (
+                actual_metric_name,
+                actual_minimize,
+            ) = es_strategy._default_objective_and_direction(
+                experiment=test_multi_objective_experiment
+            )
+            self.assertEqual(
+                actual_metric_name,
+                test_multi_objective.objectives[1].metric.name,
+            )
+            self.assertEqual(
+                actual_minimize,
+                test_multi_objective.objectives[1].minimize,
+            )
+
     def test_is_eligible(self) -> None:
         class FakeStrategy(BaseEarlyStoppingStrategy):
             def should_stop_trials_early(
                 self,
                 trial_indices: Set[int],
                 experiment: Experiment,
                 **kwargs: Dict[str, Any],
```

### Comparing `ax-platform-0.3.1/ax/early_stopping/utils.py` & `ax-platform-0.3.2/ax/early_stopping/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/exceptions/constants.py` & `ax-platform-0.3.2/ax/exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/exceptions/core.py` & `ax-platform-0.3.2/ax/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/exceptions/data_provider.py` & `ax-platform-0.3.2/ax/exceptions/data_provider.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/exceptions/generation_strategy.py` & `ax-platform-0.3.2/ax/exceptions/generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/exceptions/storage.py` & `ax-platform-0.3.2/ax/exceptions/storage.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/global_stopping/strategies/base.py` & `ax-platform-0.3.2/ax/global_stopping/strategies/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/global_stopping/strategies/improvement.py` & `ax-platform-0.3.2/ax/global_stopping/strategies/improvement.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/global_stopping/tests/tests_strategies.py` & `ax-platform-0.3.2/ax/global_stopping/tests/tests_strategies.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/botorch_test_problem.py` & `ax-platform-0.3.2/ax/metrics/botorch_test_problem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/branin.py` & `ax-platform-0.3.2/ax/metrics/branin.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/branin_map.py` & `ax-platform-0.3.2/ax/metrics/branin_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 
 
 class BraninTimestampMapMetric(NoisyFunctionMapMetric):
     def __init__(
         self,
         name: str,
         param_names: Iterable[str],
-        # pyre-fixme[24]: Generic type `MapKeyInfo` expects 1 type parameter.
-        map_key_infos: Optional[Iterable[MapKeyInfo]] = None,
         noise_sd: float = 0.0,
         lower_is_better: Optional[bool] = None,
         rate: Optional[float] = None,
         cache_evaluations: bool = True,
     ) -> None:
         """A Branin map metric with an optional multiplicative factor
         of `1 + exp(-rate * t)` where `t` is the runtime of the trial.
@@ -54,28 +52,24 @@
         self.rate = rate
         # pyre-fixme[4]: Attribute must be annotated.
         self._trial_index_to_timestamp = defaultdict(int)
 
         super().__init__(
             name=name,
             param_names=param_names,
-            map_key_infos=map_key_infos
-            if map_key_infos is not None
-            else [MapKeyInfo(key="timestamp", default_value=0.0)],
             noise_sd=noise_sd,
             lower_is_better=lower_is_better,
             cache_evaluations=cache_evaluations,
         )
 
     def __eq__(self, o: BraninTimestampMapMetric) -> bool:
         """Ignore _timestamp on equality checks"""
         return (
             self.name == o.name
             and self.param_names == o.param_names
-            and self.map_key_infos == o.map_key_infos
             and self.noise_sd == o.noise_sd
             and self.lower_is_better == o.lower_is_better
         )
 
     def fetch_trial_data(
         self, trial: BaseTrial, noisy: bool = True, **kwargs: Any
     ) -> MapMetricFetchResult:
@@ -99,22 +93,21 @@
                 df = pd.DataFrame(
                     {
                         "arm_name": [arm.name for arm in trial.arms],
                         "metric_name": self.name,
                         "sem": self.noise_sd if noisy else 0.0,
                         "trial_index": trial.index,
                         "mean": [item["mean"] for item in res],
-                        **{
-                            mki.key: [item[mki.key] for item in res]
-                            for mki in self.map_key_infos
-                        },
+                        self.map_key_info.key: [
+                            item[self.map_key_info.key] for item in res
+                        ],
                     }
                 )
 
-                datas.append(MapData(df=df, map_key_infos=self.map_key_infos))
+                datas.append(MapData(df=df, map_key_infos=[self.map_key_info]))
 
             return Ok(value=MapData.from_multiple_map_data(datas))
 
         except Exception as e:
             return Err(
                 MetricFetchE(message=f"Failed to fetch {self.name}", exception=e)
             )
@@ -129,25 +122,27 @@
 
         mean = checked_cast(float, branin(x1=x1, x2=x2)) * weight
 
         return {"mean": mean, "timestamp": timestamp}
 
 
 class BraninFidelityMapMetric(NoisyFunctionMapMetric):
+
+    map_key_info: MapKeyInfo[float] = MapKeyInfo(key="fidelity", default_value=0.0)
+
     def __init__(
         self,
         name: str,
         param_names: Iterable[str],
         noise_sd: float = 0.0,
         lower_is_better: Optional[bool] = None,
     ) -> None:
         super().__init__(
             name=name,
             param_names=param_names,
-            map_key_infos=[MapKeyInfo(key="fidelity", default_value=0.0)],
             noise_sd=noise_sd,
             lower_is_better=lower_is_better,
         )
 
         self.index = -1
 
     def fetch_trial_data(
```

### Comparing `ax-platform-0.3.1/ax/metrics/chemistry.py` & `ax-platform-0.3.2/ax/metrics/chemistry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/chemistry_data.zip` & `ax-platform-0.3.2/ax/metrics/chemistry_data.zip`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/curve.py` & `ax-platform-0.3.2/ax/metrics/curve.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
 logger: Logger = get_logger(__name__)
 
 
 class AbstractCurveMetric(MapMetric, ABC):
     """Metric representing (partial) learning curves of ML model training jobs."""
 
-    # pyre-fixme[4]: Attribute must be annotated.
-    MAP_KEY = MapKeyInfo(key="training_rows", default_value=0.0)
+    map_key_info: MapKeyInfo[float] = MapKeyInfo(key="training_rows", default_value=0.0)
 
     def __init__(
         self,
         name: str,
         curve_name: str,
         lower_is_better: bool = True,
         cumulative_best: bool = False,
@@ -162,15 +161,15 @@
                         value=MapData(
                             df=(
                                 df.loc[
                                     (df["metric_name"] == metric.name)
                                     & (df["trial_index"] == trial.index)
                                 ]
                             ),
-                            map_key_infos=[cls.MAP_KEY],
+                            map_key_infos=[cls.map_key_info],
                         )
                     )
                     for metric in metrics
                 }
                 for trial in (trials if trials is not None else [])
             }
         except Exception as e:
@@ -215,15 +214,15 @@
             curve_series = all_curve_series[id_]
             for m in metrics:
                 if m.curve_name in curve_series:  # pyre-ignore[16]
                     dfi = _get_single_curve(
                         curve_series=curve_series,
                         curve_name=m.curve_name,
                         metric_name=m.name,
-                        map_key=cls.MAP_KEY.key,
+                        map_key=cls.map_key_info.key,
                         trial=experiment.trials[trial_idx],
                         cumulative_best=m.cumulative_best,  # pyre-ignore[16]
                         lower_is_better=m.lower_is_better,  # pyre-ignore[6]
                         smoothing_window=m.smoothing_window,  # pyre-ignore[16]
                     )
                     dfs.append(dfi)
                 else:
@@ -266,17 +265,17 @@
             ids: The ids of the backend runs for which to fetch the
                 partial result curves.
 
         Returns:
             A dictionary mapping the backend id to the partial result
             curves, each of which is represented as a mapping from
             the metric name to a pandas Series indexed by the progression
-            (which will be mapped to the `MAP_KEY` of the metric class).
-            E.g. if `curve_name=loss` and `MAP_KEY=training_rows`, then a
-            Series should look like:
+            (which will be mapped to the `map_key_info.key` of the metric class).
+            E.g. if `curve_name=loss` and `map_key_info.key = training_rows`,
+            then a Series should look like:
 
                  training_rows (index) | loss
                 -----------------------|------
                                    100 | 0.5
                                    200 | 0.2
         """
         ...  # pragma: nocover
@@ -356,15 +355,15 @@
             for m in metrics:
                 curve_dfs = []
                 for curve_name in m.coefficients.keys():  # pyre-ignore[16]
                     if curve_name in curve_series:
                         curve_df = _get_single_curve(
                             curve_series=curve_series,
                             curve_name=curve_name,
-                            map_key=cls.MAP_KEY.key,
+                            map_key=cls.map_key_info.key,
                             trial=experiment.trials[trial_idx],
                             cumulative_best=m.cumulative_best,  # pyre-ignore[16]
                             lower_is_better=m.lower_is_better,  # pyre-ignore[6]
                             smoothing_window=m.smoothing_window,  # pyre-ignore[16]
                         )
                         curve_dfs.append(curve_df)
                     else:
@@ -390,15 +389,15 @@
         for trial_idx, dfi in all_data_df.groupby("trial_index"):
             # the `do_forward_fill = True` pads with the latest
             # observation to handle situations where learning curves
             # report different amounts of data.
             trial_curves = dfi["metric_name"].unique().tolist()
             dfs_mean, dfs_sem = align_partial_results(
                 dfi,
-                progr_key=cls.MAP_KEY.key,
+                progr_key=cls.map_key_info.key,
                 metrics=trial_curves,
                 do_forward_fill=True,
             )
             for metric in complete_metrics_by_trial[trial_idx]:
                 sub_df = _get_scalarized_curve_metric_sub_df(
                     dfs_mean=dfs_mean,
                     dfs_sem=dfs_sem,
```

### Comparing `ax-platform-0.3.1/ax/metrics/dict_lookup.py` & `ax-platform-0.3.2/ax/metrics/dict_lookup.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/factorial.py` & `ax-platform-0.3.2/ax/metrics/factorial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/hartmann6.py` & `ax-platform-0.3.2/ax/metrics/hartmann6.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/jenatton.py` & `ax-platform-0.3.2/ax/metrics/jenatton.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/noisy_function.py` & `ax-platform-0.3.2/ax/metrics/noisy_function.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/noisy_function_map.py` & `ax-platform-0.3.2/ax/metrics/noisy_function_map.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,41 +4,39 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from logging import Logger
 
-from typing import Any, Dict, Iterable, Mapping, Optional
+from typing import Any, Iterable, Mapping, Optional
 
 import numpy as np
 import pandas as pd
 from ax.core.base_trial import BaseTrial
 from ax.core.map_data import MapData, MapKeyInfo
 from ax.core.map_metric import MapMetric, MapMetricFetchResult
 from ax.core.metric import MetricFetchE
 from ax.utils.common.logger import get_logger
 from ax.utils.common.result import Err, Ok
-from ax.utils.common.serialization import serialize_init_args
-from ax.utils.common.typeutils import checked_cast
 
 logger: Logger = get_logger(__name__)
 
 
 class NoisyFunctionMapMetric(MapMetric):
     """A metric defined by a generic deterministic function, with normal noise
     with mean 0 and mean_sd scale added to the result.
     """
 
+    map_key_info: MapKeyInfo[float] = MapKeyInfo(key="timestamp", default_value=0.0)
+
     def __init__(
         self,
         name: str,
         param_names: Iterable[str],
-        # pyre-fixme[24]: Generic type `MapKeyInfo` expects 1 type parameter.
-        map_key_infos: Iterable[MapKeyInfo],
         noise_sd: float = 0.0,
         lower_is_better: Optional[bool] = None,
         cache_evaluations: bool = True,
     ) -> None:
         """
         Metric is computed by evaluating a deterministic function, implemented
         in f.
@@ -55,15 +53,14 @@
             lower_is_better: Flag for metrics which should be minimized.
             cache_evaluations: Flag for whether previous evaluations should
                 be cached. If so, those values are returned for previously
                 evaluated parameters using the same realization of the
                 observation noise.
         """
         self.param_names = param_names
-        self.map_key_infos = map_key_infos
         self.noise_sd = noise_sd
         # pyre-fixme[4]: Attribute must be annotated.
         self.cache = {}
         self.cache_evaluations = cache_evaluations
         super().__init__(name=name, lower_is_better=lower_is_better)
 
     @classmethod
@@ -74,15 +71,14 @@
     def overwrite_existing_data(cls) -> bool:
         return True
 
     def clone(self) -> NoisyFunctionMapMetric:
         return self.__class__(
             name=self._name,
             param_names=self.param_names,
-            map_key_infos=self.map_key_infos,
             noise_sd=self.noise_sd,
             lower_is_better=self.lower_is_better,
             cache_evaluations=self.cache_evaluations,
         )
 
     def fetch_trial_data(
         self, trial: BaseTrial, noisy: bool = True, **kwargs: Any
@@ -96,41 +92,22 @@
             df = pd.DataFrame(
                 {
                     "arm_name": [arm.name for arm in trial.arms],
                     "metric_name": self.name,
                     "sem": self.noise_sd if noisy else 0.0,
                     "trial_index": trial.index,
                     "mean": [item["mean"] for item in res],
-                    **{
-                        mki.key: [item[mki.key] for item in res]
-                        for mki in self.map_key_infos
-                    },
+                    self.map_key_info.key: [
+                        item[self.map_key_info.key] for item in res
+                    ],
                 }
             )
-
-            return Ok(value=MapData(df=df, map_key_infos=self.map_key_infos))
+            return Ok(value=MapData(df=df, map_key_infos=[self.map_key_info]))
 
         except Exception as e:
             return Err(
                 MetricFetchE(message=f"Failed to fetch {self.name}", exception=e)
             )
 
     def f(self, x: np.ndarray) -> Mapping[str, Any]:
         """The deterministic function that produces the metric outcomes."""
         raise NotImplementedError
-
-    @classmethod
-    # pyre-fixme[2]: Parameter annotation cannot be `Any`.
-    def serialize_init_args(cls, obj: Any) -> Dict[str, Any]:
-        nf_map_metric = checked_cast(NoisyFunctionMapMetric, obj)
-        init_args = serialize_init_args(
-            object=nf_map_metric, exclude_fields=["map_key_infos"]
-        )
-        init_args["map_key_infos"] = [
-            serialize_init_args(object=mki) for mki in nf_map_metric.map_key_infos
-        ]
-        return init_args
-
-    @classmethod
-    def deserialize_init_args(cls, args: Dict[str, Any]) -> Dict[str, Any]:
-        args["map_key_infos"] = [MapKeyInfo(**mki) for mki in args["map_key_infos"]]
-        return super().deserialize_init_args(args=args)
```

### Comparing `ax-platform-0.3.1/ax/metrics/sklearn.py` & `ax-platform-0.3.2/ax/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/tensorboard.py` & `ax-platform-0.3.2/ax/metrics/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     from tensorboard.compat.proto import types_pb2
 
     logging.getLogger("tensorboard").setLevel(logging.CRITICAL)
 
     class TensorboardCurveMetric(AbstractCurveMetric):
         """A `CurveMetric` for getting Tensorboard curves."""
 
-        # pyre-fixme[4]: Attribute must be annotated.
-        MAP_KEY = MapKeyInfo(key="steps", default_value=0.0)
+        map_key_info: MapKeyInfo[float] = MapKeyInfo(key="steps", default_value=0.0)
 
         @classmethod
         def get_curves_from_ids(
             cls, ids: Iterable[Union[int, str]]
         ) -> Dict[Union[int, str], Dict[str, pd.Series]]:
             """Get curve data from tensorboard logs.
```

### Comparing `ax-platform-0.3.1/ax/metrics/tests/test_chemistry.py` & `ax-platform-0.3.2/ax/metrics/tests/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/tests/test_curve.py` & `ax-platform-0.3.2/ax/metrics/tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/tests/test_dict_lookup.py` & `ax-platform-0.3.2/ax/metrics/tests/test_dict_lookup.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/tests/test_noisy_function.py` & `ax-platform-0.3.2/ax/metrics/tests/test_noisy_function.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/tests/test_sklearn.py` & `ax-platform-0.3.2/ax/metrics/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/tests/test_tensorboard.py` & `ax-platform-0.3.2/ax/metrics/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/metrics/torchx.py` & `ax-platform-0.3.2/ax/metrics/torchx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/__init__.py` & `ax-platform-0.3.2/ax/modelbridge/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/base.py` & `ax-platform-0.3.2/ax/modelbridge/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import time
+import warnings
 from abc import ABC
 from collections import OrderedDict
 from copy import deepcopy
 from dataclasses import dataclass, field
 
 from logging import Logger
 from typing import Any, Dict, List, MutableMapping, Optional, Set, Tuple, Type
@@ -31,14 +32,15 @@
 from ax.core.types import TCandidateMetadata, TModelCov, TModelMean, TModelPredict
 from ax.exceptions.core import UserInputError
 from ax.modelbridge.transforms.base import Transform
 from ax.modelbridge.transforms.cast import Cast
 from ax.models.types import TConfig
 from ax.utils.common.logger import get_logger
 from ax.utils.common.typeutils import checked_cast, not_none
+from botorch.exceptions.warnings import InputDataWarning
 
 logger: Logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class BaseGenArgs:
     search_space: SearchSpace
@@ -90,14 +92,15 @@
         data: Optional[Data] = None,
         transform_configs: Optional[Dict[str, TConfig]] = None,
         status_quo_name: Optional[str] = None,
         status_quo_features: Optional[ObservationFeatures] = None,
         optimization_config: Optional[OptimizationConfig] = None,
         fit_out_of_design: bool = False,
         fit_abandoned: bool = False,
+        fit_on_init: bool = True,
     ) -> None:
         """
         Applies transforms and fits model.
 
         Args:
             experiment: Is used to get arm parameters. Is not mutated.
             search_space: Search space for fitting the model. Constraints need
@@ -118,80 +121,129 @@
             optimization_config: Optimization config defining how to optimize
                 the model.
             fit_out_of_design: If specified, all training data is returned.
                 Otherwise, only in design points are returned.
             fit_abandoned: Whether data for abandoned arms or trials should be
                 included in model training data. If ``False``, only
                 non-abandoned points are returned.
+            fit_on_init: Whether to fit the model on initialization. This can
+                be used to skip model fitting when a fitted model is not needed.
+                To fit the model afterwards, use `_process_and_transform_data`
+                to get the transformed inputs and call `_fit_if_implemented` with
+                the transformed inputs.
         """
-        t_fit_start = time.time()
+        t_fit_start = time.monotonic()
         transforms = transforms or []
         # pyre-ignore: Cast is a Tranform
         transforms: List[Type[Transform]] = [Cast] + transforms
 
+        self.fit_time: float = 0.0
+        self.fit_time_since_gen: float = 0.0
         self._metric_names: Set[str] = set()
         self._training_data: List[Observation] = []
         self._optimization_config: Optional[OptimizationConfig] = optimization_config
         self._training_in_design: List[bool] = []
         self._status_quo: Optional[Observation] = None
         self._arms_by_signature: Optional[Dict[str, Arm]] = None
         self.transforms: MutableMapping[str, Transform] = OrderedDict()
         self._model_key: Optional[str] = None
         self._model_kwargs: Optional[Dict[str, Any]] = None
         self._bridge_kwargs: Optional[Dict[str, Any]] = None
-
-        # pyre-fixme[4]: Attribute must be annotated.
-        self._model_space = search_space.clone()
+        self._model_space: SearchSpace = search_space.clone()
         self._raw_transforms = transforms
         self._transform_configs: Optional[Dict[str, TConfig]] = transform_configs
         self._fit_out_of_design = fit_out_of_design
         self._fit_abandoned = fit_abandoned
-        imm = experiment and experiment.immutable_search_space_and_opt_config
-        # pyre-fixme[4]: Attribute must be annotated.
-        self._experiment_has_immutable_search_space_and_opt_config = imm
+        self._experiment_has_immutable_search_space_and_opt_config: bool = (
+            experiment is not None and experiment.immutable_search_space_and_opt_config
+        )
         if experiment is not None:
             if self._optimization_config is None:
                 self._optimization_config = experiment.optimization_config
             self._arms_by_signature = experiment.arms_by_signature
 
-        # Convert Data to Observations
-        observations = self._prepare_observations(experiment=experiment, data=data)
-
+        # Set training data (in the raw / untransformed space). This also omits
+        # out-of-design and abandoned observations depending on the corresponding flags.
+        observations_raw = self._prepare_observations(experiment=experiment, data=data)
         observations_raw = self._set_training_data(
-            observations=observations, search_space=search_space
+            observations=observations_raw, search_space=self._model_space
         )
-        # Set model status quo
+
+        # Set model status quo.
         # NOTE: training data must be set before setting the status quo.
         self._set_status_quo(
             experiment=experiment,
             status_quo_name=status_quo_name,
             status_quo_features=status_quo_features,
         )
-        observations, search_space = self._transform_data(
-            observations=observations_raw,
-            search_space=search_space,
-            transforms=transforms,
-            transform_configs=transform_configs,
-        )
 
-        # Save model, apply terminal transform, and fit
+        # Save model, apply terminal transform, and fit.
         self.model = model
+        if fit_on_init:
+            observations, search_space = self._transform_data(
+                observations=observations_raw,
+                search_space=self._model_space,
+                transforms=self._raw_transforms,
+                transform_configs=self._transform_configs,
+            )
+            self._fit_if_implemented(
+                search_space=search_space,
+                observations=observations,
+                time_so_far=time.monotonic() - t_fit_start,
+            )
+
+    def _fit_if_implemented(
+        self,
+        search_space: SearchSpace,
+        observations: List[Observation],
+        time_so_far: float,
+    ) -> None:
+        r"""Fits the model if `_fit` is implemented and stores fit time.
+
+        Args:
+            search_space: A transformed search space for fitting the model.
+            observations: The observations to fit the model with. These should
+                also be transformed.
+            time_so_far: Time spent in initializing the model up to
+                `_fit_if_implemented` call.
+        """
         try:
+            t_fit_start = time.monotonic()
             self._fit(
-                model=model,
+                model=self.model,
                 search_space=search_space,
                 observations=observations,
             )
-            # pyre-fixme[4]: Attribute must be annotated.
-            self.fit_time = time.time() - t_fit_start
-            # pyre-fixme[4]: Attribute must be annotated.
-            self.fit_time_since_gen = float(self.fit_time)
+            increment = time.monotonic() - t_fit_start + time_so_far
+            self.fit_time += increment
+            self.fit_time_since_gen += increment
         except NotImplementedError:
-            self.fit_time = 0.0
-            self.fit_time_since_gen = 0.0
+            pass
+
+    def _process_and_transform_data(
+        self,
+        experiment: Optional[Experiment] = None,
+        data: Optional[Data] = None,
+    ) -> Tuple[List[Observation], SearchSpace]:
+        r"""Processes the data into observations and returns transformed
+        observations and the search space. This packages the following methods:
+        * self._prepare_observations
+        * self._set_training_data
+        * self._transform_data
+        """
+        observations = self._prepare_observations(experiment=experiment, data=data)
+        observations_raw = self._set_training_data(
+            observations=observations, search_space=self._model_space
+        )
+        return self._transform_data(
+            observations=observations_raw,
+            search_space=self._model_space,
+            transforms=self._raw_transforms,
+            transform_configs=self._transform_configs,
+        )
 
     def _prepare_observations(
         self, experiment: Optional[Experiment], data: Optional[Data]
     ) -> List[Observation]:
         if experiment is None or data is None:
             return []
         return observations_from_data(
@@ -200,14 +252,15 @@
 
     def _transform_data(
         self,
         observations: List[Observation],
         search_space: SearchSpace,
         transforms: Optional[List[Type[Transform]]],
         transform_configs: Optional[Dict[str, TConfig]],
+        assign_transforms: bool = True,
     ) -> Tuple[List[Observation], SearchSpace]:
         """Initialize transforms and apply them to provided data."""
         # Initialize transforms
         search_space = search_space.clone()
         if transforms is not None:
             if transform_configs is None:
                 transform_configs = {}
@@ -217,25 +270,26 @@
                     search_space=search_space,
                     observations=observations,
                     modelbridge=self,
                     config=transform_configs.get(t.__name__, None),
                 )
                 search_space = t_instance.transform_search_space(search_space)
                 observations = t_instance.transform_observations(observations)
-                self.transforms[t.__name__] = t_instance
+                if assign_transforms:
+                    self.transforms[t.__name__] = t_instance
 
         return observations, search_space
 
     def _prepare_training_data(
         self, observations: List[Observation]
     ) -> List[Observation]:
         observation_features, observation_data = separate_observations(observations)
         if len(observation_features) != len(set(observation_features)):
             raise ValueError(
-                "Observation features not unique."
+                "Observation features are not unique. "
                 "Something went wrong constructing training data..."
             )
         return observations
 
     def _set_training_data(
         self, observations: List[Observation], search_space: SearchSpace
     ) -> List[Observation]:
@@ -562,29 +616,29 @@
         or last update) to be passed in, not all data in the experiment.
 
         Args:
             new_data: Data from the experiment obtained since the last call to
                 `update`.
             experiment: Experiment, in which this data was obtained.
         """
-        t_update_start = time.time()
+        t_update_start = time.monotonic()
         observations = self._prepare_observations(experiment=experiment, data=new_data)
         obs_raw = self._extend_training_data(observations=observations)
         observations, search_space = self._transform_data(
             observations=obs_raw,
             search_space=self._model_space,
             transforms=self._raw_transforms,
             transform_configs=self._transform_configs,
         )
         self._update(
             search_space=search_space,
             observations=observations,
         )
-        self.fit_time += time.time() - t_update_start
-        self.fit_time_since_gen += time.time() - t_update_start
+        self.fit_time += time.monotonic() - t_update_start
+        self.fit_time_since_gen += time.monotonic() - t_update_start
 
     def _update(
         self,
         search_space: SearchSpace,
         observations: List[Observation],
     ) -> None:
         """Apply terminal transform and update model.
@@ -824,21 +878,29 @@
         cv_training_data = deepcopy(cv_training_data)
         search_space = self._model_space.clone()
         for t in self.transforms.values():
             cv_training_data = t.transform_observations(cv_training_data)
             cv_test_points = t.transform_observation_features(cv_test_points)
             search_space = t.transform_search_space(search_space)
 
-        obs_feats, obs_data = separate_observations(observations=cv_training_data)
         # Apply terminal transform, and get predictions.
-        cv_predictions = self._cross_validate(
-            search_space=search_space,
-            cv_training_data=cv_training_data,
-            cv_test_points=cv_test_points,
-        )
+        with warnings.catch_warnings():
+            # Since each CV fold removes points from the training data, the remaining
+            # observations will not pass the standardization test. To avoid confusing
+            # users with this warning, we filter it out.
+            warnings.filterwarnings(
+                "ignore",
+                message="Input data is not standardized.",
+                category=InputDataWarning,
+            )
+            cv_predictions = self._cross_validate(
+                search_space=search_space,
+                cv_training_data=cv_training_data,
+                cv_test_points=cv_test_points,
+            )
         # Apply reverse transforms, in reverse order
         cv_test_observations = [
             Observation(features=obsf, data=cv_predictions[i])
             for i, obsf in enumerate(cv_test_points)
         ]
 
         for t in reversed(list(self.transforms.values())):
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/completion_criterion.py` & `ax-platform-0.3.2/ax/modelbridge/completion_criterion.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/cross_validation.py` & `ax-platform-0.3.2/ax/modelbridge/cross_validation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/discrete.py` & `ax-platform-0.3.2/ax/modelbridge/discrete.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/dispatch_utils.py` & `ax-platform-0.3.2/ax/modelbridge/dispatch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import torch
 from ax.core.experiment import Experiment
 from ax.core.optimization_config import OptimizationConfig
 from ax.core.parameter import ChoiceParameter, ParameterType, RangeParameter
 from ax.core.search_space import SearchSpace
 from ax.exceptions.core import UnsupportedError
 from ax.modelbridge.generation_strategy import GenerationStep, GenerationStrategy
-from ax.modelbridge.registry import Cont_X_trans, Models, Y_trans
+from ax.modelbridge.registry import Models
 from ax.modelbridge.transforms.base import Transform
 from ax.modelbridge.transforms.winsorize import Winsorize
 from ax.models.types import TConfig
 from ax.models.winsorization_config import WinsorizationConfig
 from ax.utils.common.logger import get_logger
 from ax.utils.common.typeutils import not_none
 
@@ -73,14 +73,15 @@
     winsorization_config: Optional[
         Union[WinsorizationConfig, Dict[str, WinsorizationConfig]]
     ] = None,
     no_winsorization: bool = False,
     should_deduplicate: bool = False,
     verbose: Optional[bool] = None,
     disable_progbar: Optional[bool] = None,
+    jit_compile: Optional[bool] = None,
     derelativize_with_raw_status_quo: bool = False,
     use_update: Optional[bool] = None,
 ) -> GenerationStep:
     """Shortcut for creating a BayesOpt generation step."""
     model_kwargs = model_kwargs or {}
 
     winsorization_transform_config = _get_winsorization_transform_config(
@@ -94,25 +95,29 @@
     }
     model_kwargs["transform_configs"] = model_kwargs.get("transform_configs", {})
     model_kwargs["transform_configs"][
         "Derelativize"
     ] = derelativization_transform_config
 
     if not no_winsorization:
-        transforms = model_kwargs.get("transforms", Cont_X_trans + Y_trans)
+        _, default_bridge_kwargs = model.view_defaults()
+        default_transforms = default_bridge_kwargs["transforms"]
+        transforms = model_kwargs.get("transforms", default_transforms)
         model_kwargs["transforms"] = [cast(Type[Transform], Winsorize)] + transforms
         if winsorization_transform_config is not None:
             model_kwargs["transform_configs"][
                 "Winsorize"
             ] = winsorization_transform_config
 
     if verbose is not None:
         model_kwargs.update({"verbose": verbose})
     if disable_progbar is not None:
         model_kwargs.update({"disable_progbar": disable_progbar})
+    if jit_compile is not None:
+        model_kwargs.update({"jit_compile": jit_compile})
     return GenerationStep(
         model=model,
         num_trials=num_trials,
         # NOTE: ceil(-1 / 2) = 0, so this is safe to do when num trials is -1.
         min_trials_observed=min_trials_observed or ceil(num_trials / 2),
         enforce_num_trials=enforce_num_trials,
         max_parallelism=max_parallelism,
@@ -290,14 +295,15 @@
     max_parallelism_cap: Optional[int] = None,
     max_parallelism_override: Optional[int] = None,
     optimization_config: Optional[OptimizationConfig] = None,
     should_deduplicate: bool = False,
     use_saasbo: bool = False,
     verbose: Optional[bool] = None,
     disable_progbar: Optional[bool] = None,
+    jit_compile: Optional[bool] = None,
     experiment: Optional[Experiment] = None,
     use_update: Optional[bool] = None,
 ) -> GenerationStrategy:
     """Select an appropriate generation strategy based on the properties of
     the search space and expected settings of the experiment, such as number of
     arms per trial, optimization algorithm settings, expected number of trials
     in the experiment, etc.
@@ -381,14 +387,15 @@
             a warning.
         disable_progbar: Whether GP model should produce a progress bar. If not
             ``None``, its value gets added to ``model_kwargs`` during
             ``generation_strategy`` construction. Defaults to ``True`` for SAASBO, else
             ``None``. Progress bars are currently only available for SAASBO, so if
             ``disable_probar is not None`` for a different model type, it will be
             overridden to ``None`` with a warning.
+        jit_compile: Whether to use jit compilation in Pyro when SAASBO is used.
         experiment: If specified, ``_experiment`` attribute of the generation strategy
             will be set to this experiment (useful for associating a generation
             strategy with a given experiment before it's first used to ``gen`` with
             that experiment). Can also provide `optimization_config` if it is not
             provided as an arg to this function.
         use_update: Whether to use ``ModelBridge.update`` to update the model with
             new data rather than fitting it from scratch. This is much more efficient,
@@ -492,14 +499,20 @@
             verbose = None
         if disable_progbar is not None and not model_is_saasbo:
             logger.warning(
                 f"Overriding `disable_progbar = {disable_progbar}` to `None` for "
                 "non-SAASBO GP step."
             )
             disable_progbar = None
+        if jit_compile is not None and not model_is_saasbo:
+            logger.warning(
+                f"Overriding `jit_compile = {jit_compile}` to `None` for "
+                "non-SAASBO GP step."
+            )
+            jit_compile = None
 
         # Create `generation_strategy`, adding first Sobol step
         # if `num_remaining_initialization_trials` is > 0.
         if num_remaining_initialization_trials > 0:
             steps.append(
                 _make_sobol_step(
                     num_trials=num_remaining_initialization_trials,
@@ -516,14 +529,15 @@
                 derelativize_with_raw_status_quo=derelativize_with_raw_status_quo,
                 no_winsorization=no_winsorization,
                 max_parallelism=bo_parallelism,
                 model_kwargs={"torch_device": torch_device},
                 should_deduplicate=should_deduplicate,
                 verbose=verbose,
                 disable_progbar=disable_progbar,
+                jit_compile=jit_compile,
                 use_update=use_update,
             ),
         )
         gs = GenerationStrategy(steps=steps)
         logger.info(
             f"Using Bayesian Optimization generation strategy: {gs}. Iterations after"
             f" {num_remaining_initialization_trials} will take longer to generate due"
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/factory.py` & `ax-platform-0.3.2/ax/modelbridge/factory.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/generation_node.py` & `ax-platform-0.3.2/ax/modelbridge/generation_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from logging import Logger
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 from ax.core.arm import Arm
 from ax.core.data import Data
 from ax.core.experiment import Experiment
 from ax.core.generator_run import GeneratorRun
 from ax.core.observation import ObservationFeatures
@@ -21,16 +22,18 @@
 from ax.exceptions.generation_strategy import GenerationStrategyRepeatedPoints
 from ax.modelbridge.base import ModelBridge
 from ax.modelbridge.completion_criterion import CompletionCriterion
 from ax.modelbridge.cross_validation import BestModelSelector, CVDiagnostics, CVResult
 from ax.modelbridge.model_spec import FactoryFunctionModelSpec, ModelSpec
 from ax.modelbridge.registry import ModelRegistryBase
 from ax.utils.common.base import SortableBase
+from ax.utils.common.logger import get_logger
 from ax.utils.common.typeutils import not_none
 
+logger: Logger = get_logger(__name__)
 
 TModelFactory = Callable[..., ModelBridge]
 CANNOT_SELECT_ONE_MODEL_MSG = """
 Base `GenerationNode` does not implement selection among fitted
 models, so exactly one `ModelSpec` must be specified when using
 `GenerationNode._pick_fitted_model_to_gen_from` (usually called
 by `GenerationNode.gen`.
@@ -183,16 +186,14 @@
         model_spec = self.model_spec_to_gen_from
         should_generate_run = True
         generator_run = None
         n_gen_draws = 0
         # Keep generating until each of `generator_run.arms` is not a duplicate
         # of a previous arm, if `should_deduplicate is True`
         while should_generate_run:
-            if n_gen_draws > max_gen_draws_for_deduplication:
-                raise GenerationStrategyRepeatedPoints(MAX_GEN_DRAWS_EXCEEDED_MESSAGE)
             generator_run = model_spec.gen(
                 # If `n` is not specified, ensure that the `None` value does not
                 # override the one set in `model_spec.model_gen_kwargs`.
                 n=model_spec.model_gen_kwargs.get("n")
                 if n is None and model_spec.model_gen_kwargs
                 else n,
                 # For `pending_observations`, prefer the input to this function, as
@@ -207,14 +208,26 @@
                 and arms_by_signature_for_deduplication
                 and any(
                     arm.signature in arms_by_signature_for_deduplication
                     for arm in generator_run.arms
                 )
             )
             n_gen_draws += 1
+            if should_generate_run:
+                if n_gen_draws > max_gen_draws_for_deduplication:
+                    raise GenerationStrategyRepeatedPoints(
+                        MAX_GEN_DRAWS_EXCEEDED_MESSAGE
+                    )
+                else:
+                    logger.info(
+                        "The generator run produced duplicate arms. Re-running the "
+                        "generation step in an attempt to deduplicate. Candidates "
+                        f"produced in the last generator run: {generator_run.arms}."
+                    )
+
         return not_none(generator_run)
 
     def _pick_fitted_model_to_gen_from(self) -> ModelSpec:
         """Select one model to generate from among the fitted models on this
         generation node.
 
         NOTE: In base ``GenerationNode`` class, this method does the following:
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/generation_strategy.py` & `ax-platform-0.3.2/ax/modelbridge/generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/map_torch.py` & `ax-platform-0.3.2/ax/modelbridge/map_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Dict, List, Optional, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type
 
 import numpy as np
 
 import torch
 from ax.core.data import Data
 from ax.core.experiment import Experiment
 from ax.core.map_data import MapData
@@ -59,14 +59,15 @@
         transform_configs: Optional[Dict[str, TConfig]] = None,
         torch_dtype: Optional[torch.dtype] = None,
         torch_device: Optional[torch.device] = None,
         status_quo_name: Optional[str] = None,
         status_quo_features: Optional[ObservationFeatures] = None,
         optimization_config: Optional[OptimizationConfig] = None,
         fit_out_of_design: bool = False,
+        fit_on_init: bool = True,
         default_model_gen_options: Optional[TConfig] = None,
         map_data_limit_rows_per_metric: Optional[int] = None,
         map_data_limit_rows_per_group: Optional[int] = None,
     ) -> None:
         """
         Applies transforms and fits model.
 
@@ -89,14 +90,19 @@
                 that arm.
             status_quo_features: ObservationFeatures to use as status quo.
                 Either this or status_quo_name should be specified, not both.
             optimization_config: Optimization config defining how to optimize
                 the model.
             fit_out_of_design: If specified, all training data is returned.
                 Otherwise, only in design points are returned.
+            fit_on_init: Whether to fit the model on initialization. This can
+                be used to skip model fitting when a fitted model is not needed.
+                To fit the model afterwards, use `_process_and_transform_data`
+                to get the transformed inputs and call `_fit_if_implemented` with
+                the transformed inputs.
             default_model_gen_options: Options passed down to `model.gen(...)`.
             map_data_limit_rows_per_metric: Subsample the map data so that the
                 total number of rows per metric is limited by this value.
             map_data_limit_rows_per_group: Subsample the map data so that the
                 number of rows in the `map_key` column for each (arm, metric)
                 is limited by this value.
         """
@@ -119,14 +125,15 @@
             transform_configs=transform_configs,
             torch_dtype=torch_dtype,
             torch_device=torch_device,
             status_quo_name=status_quo_name,
             status_quo_features=status_quo_features,
             optimization_config=optimization_config,
             fit_out_of_design=fit_out_of_design,
+            fit_on_init=fit_on_init,
             default_model_gen_options=default_model_gen_options,
         )
 
     @property
     def parameters_with_map_keys(self) -> List[str]:
         return self.parameters + self._map_key_features
 
@@ -162,26 +169,28 @@
 
     def _fit(
         self,
         model: TorchModel,
         search_space: SearchSpace,
         observations: List[Observation],
         parameters: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> None:
         """The difference from `TorchModelBridge._fit(...)` is that we use
         `self.parameters_with_map_keys` instead of `self.parameters`.
         """
         self.parameters = list(search_space.parameters.keys())
         if parameters is None:
             parameters = self.parameters_with_map_keys
         super()._fit(
             model=model,
             search_space=search_space,
             observations=observations,
             parameters=parameters,
+            **kwargs,
         )
 
     def _gen(
         self,
         n: int,
         search_space: SearchSpace,
         pending_observations: Dict[str, List[ObservationFeatures]],
@@ -268,28 +277,30 @@
 
     def _cross_validate(
         self,
         search_space: SearchSpace,
         cv_training_data: List[Observation],
         cv_test_points: List[ObservationFeatures],
         parameters: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> List[ObservationData]:
         """Make predictions at cv_test_points using only the data in obs_feats
         and obs_data. The difference from `TorchModelBridge._cross_validate`
         is that here we do cross validation on the parameters + map_keys. There
         is some extra logic to filter out out-of-design points in the map_key
         dimension.
         """
         if parameters is None:
             parameters = self.parameters_with_map_keys
         cv_test_data = super()._cross_validate(
             search_space=search_space,
             cv_training_data=cv_training_data,
             cv_test_points=cv_test_points,
             parameters=parameters,  # we pass the map_keys too by default
+            **kwargs,
         )
         observation_features, observation_data = separate_observations(cv_training_data)
         # Since map_keys are used as features, there can be the possibility that
         # models for different outcomes were fit on different ranges of map_key
         # values; for example, this is the case if we (1) mix learning curve data with
         # standard data (taking default map value), or (2) are in a situation where
         # some learning curves start later than others. These prediction results are
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/model_spec.py` & `ax-platform-0.3.2/ax/modelbridge/model_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 
     # stored cross validation results set in cross validate
     _cv_results: Optional[List[CVResult]] = None
 
     # stored cross validation diagnostics set in cross validate
     _diagnostics: Optional[CVDiagnostics] = None
 
+    # Stored to check if the model can be safely updated in fit.
+    _last_fit_arg_ids: Optional[Dict[str, int]] = None
+
     def __post_init__(self) -> None:
         self.model_kwargs = self.model_kwargs or {}
         self.model_gen_kwargs = self.model_gen_kwargs or {}
         self.model_cv_kwargs = self.model_cv_kwargs or {}
 
     @property
     def fitted_model(self) -> ModelBridge:
@@ -121,19 +124,36 @@
         """
         # unset any cross validation cache
         self._cv_results, self._diagnostics = None, None
         # NOTE: It's important to copy `self.model_kwargs` here to avoid actually
         # adding contents of `model_kwargs` passed to this method, to
         # `self.model_kwargs`.
         combined_model_kwargs = {**(self.model_kwargs or {}), **model_kwargs}
-        self._fitted_model = self.model_enum(
-            experiment=experiment,
-            data=data,
-            **combined_model_kwargs,
-        )
+        if self._fitted_model is not None and self._safe_to_update(
+            experiment=experiment, combined_model_kwargs=combined_model_kwargs
+        ):
+            # Update the data on the modelbridge and call `_fit`.
+            # This will skip model fitting if the data has not changed.
+            observations, search_space = self.fitted_model._process_and_transform_data(
+                experiment=experiment, data=data
+            )
+            self.fitted_model._fit_if_implemented(
+                search_space=search_space, observations=observations, time_so_far=0.0
+            )
+
+        else:
+            # Fit from scratch.
+            self._fitted_model = self.model_enum(
+                experiment=experiment,
+                data=data,
+                **combined_model_kwargs,
+            )
+            self._last_fit_arg_ids = self._get_fit_arg_ids(
+                experiment=experiment, combined_model_kwargs=combined_model_kwargs
+            )
 
     def cross_validate(
         self,
     ) -> Tuple[Optional[List[CVResult]], Optional[CVDiagnostics]]:
         """
         Call cross_validate, compute_diagnostics and cache the results
         If the model cannot be cross validated, warn and return None
@@ -211,14 +231,40 @@
         return self.__class__(  # pragma: no cover
             model_enum=self.model_enum,
             model_kwargs=deepcopy(self.model_kwargs),
             model_gen_kwargs=deepcopy(self.model_gen_kwargs),
             model_cv_kwargs=deepcopy(self.model_cv_kwargs),
         )
 
+    def _safe_to_update(
+        self,
+        experiment: Experiment,
+        combined_model_kwargs: Dict[str, Any],
+    ) -> bool:
+        """Checks if the object id of any of the non-data fit arguments has changed.
+
+        This is a cheap way of checking that we're attempting to re-fit the same
+        model for the same experiment, which is a very reasonable expectation
+        since this all happens on the same `ModelSpec` instance.
+        """
+        return self._last_fit_arg_ids == self._get_fit_arg_ids(
+            experiment=experiment, combined_model_kwargs=combined_model_kwargs
+        )
+
+    def _get_fit_arg_ids(
+        self,
+        experiment: Experiment,
+        combined_model_kwargs: Dict[str, Any],
+    ) -> Dict[str, int]:
+        """Construct a dictionary mapping arg name to object id."""
+        return {
+            "experiment": id(experiment),
+            **{k: id(v) for k, v in combined_model_kwargs.items()},
+        }
+
     def _assert_fitted(self) -> None:
         """Helper that verifies a model was fitted, raising an error if not"""
         if self._fitted_model is None:
             raise UserInputError("No fitted model found. Call fit() to generate one")
 
     def __repr__(self) -> str:
         model_kwargs = json.dumps(
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/modelbridge_utils.py` & `ax-platform-0.3.2/ax/modelbridge/modelbridge_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 
 from collections import defaultdict
 from copy import deepcopy
 from functools import partial
 
 from logging import Logger
 from typing import (
+    Any,
     Callable,
     Dict,
-    Iterator,
+    Iterable,
     List,
+    Mapping,
     MutableMapping,
     Optional,
     Tuple,
     Type,
     TYPE_CHECKING,
     Union,
 )
@@ -52,15 +54,15 @@
     RobustSearchSpace,
     RobustSearchSpaceDigest,
     SearchSpace,
     SearchSpaceDigest,
 )
 from ax.core.trial import Trial
 from ax.core.types import TBounds, TCandidateMetadata
-from ax.exceptions.core import UnsupportedError, UserInputError
+from ax.exceptions.core import DataRequiredError, UnsupportedError, UserInputError
 from ax.modelbridge.transforms.base import Transform
 from ax.modelbridge.transforms.utils import (
     derelativize_optimization_config_with_raw_status_quo,
 )
 from ax.models.torch.botorch_moo_defaults import pareto_frontier_evaluator
 from ax.models.torch.frontier_utils import (
     get_weighted_mc_objective_and_objective_thresholds,
@@ -1325,53 +1327,35 @@
         An array of n ObservationData, each containing
             - f: An (n x m) array
             - cov: An (n x m x m) array
     """
     means = []
     cov = []
     for obsd in observation_data:
-        metric_idxs = np.array([obsd.metric_names.index(m) for m in outcomes])
+        try:
+            metric_idxs = np.array([obsd.metric_names.index(m) for m in outcomes])
+        except ValueError:
+            missing = set(outcomes).difference(set(obsd.metric_names))
+            logger.warning(
+                f"{obsd} is missing the metrics {missing}. Ignoring the data "
+                "for the remaining metrics."
+            )
+            continue
         means.append(obsd.means[metric_idxs])
         cov.append(obsd.covariance[metric_idxs][:, metric_idxs])
     return np.array(means), np.array(cov)
 
 
 def observation_features_to_array(
     parameters: List[str], obsf: List[ObservationFeatures]
 ) -> np.ndarray:
     """Convert a list of Observation features to arrays."""
     return np.array([[of.parameters[p] for p in parameters] for of in obsf])
 
 
-def detect_duplicates(
-    X: Tensor,
-    rtol: float = 1e-5,
-    atol: float = 1e-8,
-) -> Iterator[Tuple[int, int]]:
-    """Returns an iterator over index pairs `(duplicate index, original index)` for all
-    duplicate entries of `X`.
-    """
-    tols = atol
-    if rtol:
-        rval = X.abs().max(dim=-1, keepdim=True).values
-        tols = tols + rtol * rval.max(rval.transpose(-1, -2))
-
-    n = X.shape[-2]
-    dist = torch.full((n, n), float("inf"), device=X.device, dtype=X.dtype)
-    dist[torch.triu_indices(n, n, offset=1).unbind()] = torch.nn.functional.pdist(
-        X, p=float("inf")
-    )
-    return (
-        (i, int(j))
-        # pyre-fixme[19]: Expected 1 positional argument.
-        for diff, j, i in zip(*(dist - tols).min(dim=-2), range(n))
-        if diff < 0
-    )
-
-
 def feasible_hypervolume(  # pragma: no cover
     optimization_config: MultiObjectiveOptimizationConfig, values: Dict[str, np.ndarray]
 ) -> np.ndarray:
     """Compute the feasible hypervolume each iteration.
 
     Args:
         optimization_config: Optimization config.
@@ -1443,7 +1427,35 @@
 ) -> Tuple[List[ObservationFeatures], List[ObservationData], List[Optional[str]]]:
     obs_feats, obs_data, arm_names = [], [], []
     for ob in obs:
         obs_feats.append(ob.features)
         obs_data.append(ob.data)
         arm_names.append(ob.arm_name)
     return obs_feats, obs_data, arm_names
+
+
+def transform_search_space(
+    search_space: SearchSpace,
+    transforms: Iterable[Type[Transform]],
+    transform_configs: Mapping[str, Any],
+) -> SearchSpace:
+    """
+    Apply all given transforms to a copy of the SearchSpace iteratively.
+    """
+    search_space = search_space.clone()
+
+    for t in transforms:
+        try:
+            t_instance = t(
+                search_space=search_space,
+                observations=[],
+                modelbridge=None,
+                config=transform_configs.get(t.__name__),
+            )
+
+            search_space = t_instance.transform_search_space(search_space=search_space)
+        except DataRequiredError:
+            # Skip this transform if data is required. Data is only required for
+            # transforms that operate on Observations.
+            pass
+
+    return search_space
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/pairwise.py` & `ax-platform-0.3.2/ax/modelbridge/pairwise.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
 from ax.core.observation import ObservationData, ObservationFeatures
 from ax.core.types import TCandidateMetadata
-from ax.modelbridge.modelbridge_utils import detect_duplicates
 from ax.modelbridge.torch import TorchModelBridge
+from botorch.models.utils.assorted import consolidate_duplicates
 from botorch.utils.containers import SliceContainer
 from botorch.utils.datasets import RankingDataset, SupervisedDataset
 from torch import Tensor
 
 
 class PairwiseModelBridge(TorchModelBridge):
     def _convert_observations(
@@ -90,44 +90,25 @@
     idx_shift = (torch.arange(0, Y.shape[-2]) * 2).unsqueeze(-1).expand_as(Y)
     comparison_pairs = idx_shift + (1 - Y)
     return comparison_pairs
 
 
 def _consolidate_comparisons(X: Tensor, Y: Tensor) -> Tuple[Tensor, Tensor]:
     """Drop duplicated Xs and update the indices in Ys accordingly"""
-    if len(X.shape) != 2:
-        raise ValueError("X must have 2 dimensions.")  # pragma: no cover
-    if len(Y.shape) != 2:
-        raise ValueError("Y must have 2 dimensions.")  # pragma: no cover
     if Y.shape[-1] != 2:
         raise ValueError(  # pragma: no cover
             "The last dimension of Y must contain 2 elements "
             "representing the pairwise comparison."
         )
 
-    n = X.shape[-2]
-    dupplicates = list(detect_duplicates(X=X))
-    if len(dupplicates) != 0:
-        dup_indices, kept_indices = zip(*dupplicates)
-        unique_indices = set(range(n)) - set(dup_indices)
-
-        # After dropping the duplicates,
-        # the kept ones' indices may also change by being shifted up
-        new_idx_map = dict(zip(unique_indices, range(len(unique_indices))))
-        new_indices_for_dup = (new_idx_map[idx] for idx in kept_indices)
-        new_idx_map.update(dict(zip(dup_indices, new_indices_for_dup)))
-
-        consolidated_X = X[list(unique_indices), :]
-        consolidated_Y = torch.tensor(
-            [(new_idx_map[y1.item()], new_idx_map[y2.item()]) for y1, y2 in Y],
-            dtype=torch.long,
-        )
-        return consolidated_X, consolidated_Y
-    else:
-        return X, Y
+    if len(Y.shape) != 2:
+        raise ValueError("Y must have 2 dimensions.")
+
+    X, Y, _ = consolidate_duplicates(X, Y)
+    return X, Y
 
 
 def _validate_Y_values(Y: Tensor) -> None:
     """Check if Ys have valid values"""
     # Y must have even number of elements
     if Y.shape[-1] != 2:
         raise ValueError(  # pragma: no cover
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/prediction_utils.py` & `ax-platform-0.3.2/ax/modelbridge/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/random.py` & `ax-platform-0.3.2/ax/modelbridge/random.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/registry.py` & `ax-platform-0.3.2/ax/modelbridge/registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/strategies/alebo.py` & `ax-platform-0.3.2/ax/modelbridge/strategies/alebo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/strategies/rembo.py` & `ax-platform-0.3.2/ax/modelbridge/strategies/rembo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_alebo_strategy.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_alebo_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_base_modelbridge.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_base_modelbridge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import warnings
+from typing import Any, List
 from unittest import mock
 from unittest.mock import Mock
 
 import numpy as np
 import pandas as pd
 from ax.core.arm import Arm
 from ax.core.data import Data
@@ -26,20 +27,21 @@
 from ax.modelbridge.base import (
     clamp_observation_features,
     gen_arms,
     GenResults,
     ModelBridge,
     unwrap_observation_data,
 )
-from ax.modelbridge.registry import Models
+from ax.modelbridge.registry import Models, Y_trans
 from ax.modelbridge.transforms.log import Log
 from ax.models.base import Model
 from ax.utils.common.constants import Keys
 from ax.utils.common.testutils import TestCase
 from ax.utils.testing.core_stubs import (
+    get_branin_experiment,
     get_branin_experiment_with_multi_objective,
     get_experiment,
     get_experiment_with_repeated_arms,
     get_non_monolithic_branin_moo_data,
     get_optimization_config,
     get_optimization_config_no_constraints,
     get_search_space_for_range_value,
@@ -53,14 +55,15 @@
     get_observation2,
     get_observation2trans,
     get_observation_status_quo0,
     get_observation_status_quo1,
     transform_1,
     transform_2,
 )
+from botorch.exceptions.warnings import InputDataWarning
 
 
 class BaseModelBridgeTest(TestCase):
     @mock.patch(
         "ax.modelbridge.base.observations_from_data",
         autospec=True,
         return_value=([get_observation1(), get_observation2()]),
@@ -208,25 +211,42 @@
             search_space=SearchSpace([FixedParameter("x", ParameterType.FLOAT, 8.0)]),
             optimization_config=oc2,
             pending_observations={},
             fixed_features=None,
             model_gen_options=None,
         )
 
-        # Test transforms applied on cross_validate
+        # Test transforms applied on cross_validate and the warning is suppressed.
+        called = False
+
+        def warn_and_return_mock_obs(
+            *args: Any, **kwargs: Any
+        ) -> List[ObservationData]:
+            nonlocal called
+            called = True
+            warnings.warn(
+                "Input data is not standardized. Please consider scaling the "
+                "input to zero mean and unit variance.",
+                InputDataWarning,
+            )
+            return [get_observation1trans().data]
+
         modelbridge._cross_validate = mock.MagicMock(
             "ax.modelbridge.base.ModelBridge._cross_validate",
             autospec=True,
-            return_value=[get_observation1trans().data],
+            side_effect=warn_and_return_mock_obs,
         )
         cv_training_data = [get_observation2()]
         cv_test_points = [get_observation1().features]
-        cv_predictions = modelbridge.cross_validate(
-            cv_training_data=cv_training_data, cv_test_points=cv_test_points
-        )
+        with warnings.catch_warnings(record=True) as ws:
+            cv_predictions = modelbridge.cross_validate(
+                cv_training_data=cv_training_data, cv_test_points=cv_test_points
+            )
+        self.assertTrue(called)
+        self.assertFalse(any(w.category is InputDataWarning for w in ws))
         # pyre-fixme[16]: Callable `_cross_validate` has no attribute
         #  `assert_called_with`.
         modelbridge._cross_validate.assert_called_with(
             search_space=SearchSpace([FixedParameter("x", ParameterType.FLOAT, 8.0)]),
             cv_training_data=[get_observation2trans()],
             cv_test_points=[get_observation1().features],  # untransformed after
         )
@@ -254,14 +274,71 @@
         with mock.patch(
             "ax.modelbridge.base.ModelBridge._transform_observation_features",
             autospec=True,
         ) as mock_tr:
             modelbridge.transform_observation_features([get_observation2().features])
         mock_tr.assert_called_with(modelbridge, [get_observation2trans().features])
 
+        # Test that fit is not called when fit_on_init = False.
+        mock_fit.reset_mock()
+        modelbridge = ModelBridge(
+            search_space=ss,
+            model=Model(),
+            fit_on_init=False,
+        )
+        self.assertEqual(mock_fit.call_count, 0)
+
+    @mock.patch(
+        "ax.modelbridge.base.gen_arms",
+        autospec=True,
+        return_value=([Arm(parameters={"x1": 0.0, "x2": 0.0})], None),
+    )
+    @mock.patch("ax.modelbridge.base.ModelBridge._fit", autospec=True)
+    def test_with_status_quo(self, mock_fit: Mock, mock_gen_arms: Mock) -> None:
+        # Test init with a status quo.
+        exp = get_branin_experiment(
+            with_trial=True,
+            with_status_quo=True,
+            with_completed_trial=True,
+        )
+        modelbridge = ModelBridge(
+            search_space=exp.search_space,
+            model=Model(),
+            transforms=Y_trans,
+            experiment=exp,
+            data=exp.lookup_data(),
+        )
+        self.assertIsNotNone(modelbridge.status_quo)
+        self.assertEqual(
+            modelbridge.status_quo.features.parameters, {"x1": 0.0, "x2": 0.0}
+        )
+
+    @mock.patch("ax.modelbridge.base.ModelBridge._fit", autospec=True)
+    @mock.patch("ax.modelbridge.base.ModelBridge._gen", autospec=True)
+    def test_timing(self, mock_fit: Mock, mock_gen: Mock) -> None:
+        search_space = get_search_space_for_value()
+        modelbridge = ModelBridge(
+            search_space=search_space, model=Model(), fit_on_init=False
+        )
+        self.assertEqual(modelbridge.fit_time, 0.0)
+        modelbridge._fit_if_implemented(
+            search_space=search_space, observations=[], time_so_far=3.0
+        )
+        modelbridge._fit_if_implemented(
+            search_space=search_space, observations=[], time_so_far=2.0
+        )
+        modelbridge._fit_if_implemented(
+            search_space=search_space, observations=[], time_so_far=1.0
+        )
+        self.assertAlmostEqual(modelbridge.fit_time, 6.0, places=1)
+        self.assertAlmostEqual(modelbridge.fit_time_since_gen, 6.0, places=1)
+        modelbridge.gen(1)
+        self.assertAlmostEqual(modelbridge.fit_time, 6.0, places=1)
+        self.assertAlmostEqual(modelbridge.fit_time_since_gen, 0.0, places=1)
+
     @mock.patch(
         "ax.modelbridge.base.observations_from_data",
         autospec=True,
         return_value=([get_observation1(), get_observation2()]),
     )
     def test_ood_gen(self, _) -> None:
         # Test fit_out_of_design by returning OOD candidats
@@ -472,17 +549,17 @@
 
     @mock.patch(
         "ax.modelbridge.base.observations_from_data",
         autospec=True,
         return_value=([get_observation1(), get_observation1()]),
     )
     @mock.patch("ax.modelbridge.base.ModelBridge._fit", autospec=True)
-    # pyre-fixme[3]: Return type must be annotated.
-    # pyre-fixme[2]: Parameter must be annotated.
-    def testSetTrainingDataDupFeatures(self, mock_fit, mock_observations_from_data):
+    def testSetTrainingDataDupFeatures(
+        self, mock_fit: Mock, mock_observations_from_data: Mock
+    ) -> None:
         # Throws an error if repeated features in observations.
         with self.assertRaises(ValueError):
             ModelBridge(
                 get_search_space_for_value(),
                 0,
                 [],
                 get_experiment_for_value(),
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_base_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_base_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_cap_parameter_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_cap_parameter_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_cast_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_cast_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_centered_unit_x_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_centered_unit_x_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_choice_encode_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_choice_encode_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_completion_criterion.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_completion_criterion.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_convert_metric_names.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_convert_metric_names.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_cross_validation.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_derelativize_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_derelativize_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_discrete_modelbridge.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_discrete_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_dispatch_utils.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_dispatch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ax.modelbridge.dispatch_utils import (
     _make_botorch_step,
     calculate_num_initialization_trials,
     choose_generation_strategy,
     DEFAULT_BAYESIAN_PARALLELISM,
 )
 from ax.modelbridge.factory import Cont_X_trans, Y_trans
-from ax.modelbridge.registry import Models
+from ax.modelbridge.registry import Mixed_transforms, Models
 from ax.modelbridge.transforms.log_y import LogY
 from ax.modelbridge.transforms.winsorize import Winsorize
 from ax.models.winsorization_config import WinsorizationConfig
 from ax.utils.common.testutils import TestCase
 from ax.utils.common.typeutils import not_none
 from ax.utils.testing.core_stubs import (
     get_branin_experiment,
@@ -179,29 +179,29 @@
                 search_space=get_factorial_search_space()
             )
             self.assertEqual(bo_mixed._steps[0].model, Models.SOBOL)
             self.assertEqual(bo_mixed._steps[0].num_trials, 6)
             self.assertEqual(bo_mixed._steps[1].model, Models.BO_MIXED)
             expected_model_kwargs = {
                 "torch_device": None,
-                "transforms": expected_transforms,
+                "transforms": [Winsorize] + Mixed_transforms + Y_trans,
                 "transform_configs": expected_transform_configs,
             }
             self.assertEqual(bo_mixed._steps[1].model_kwargs, expected_model_kwargs)
         with self.subTest("BO_MIXED (mixed search space)"):
             ss = get_branin_search_space(with_choice_parameter=True)
             # pyre-fixme[16]: `Parameter` has no attribute `_is_ordered`.
             ss.parameters["x2"]._is_ordered = False
             bo_mixed_2 = choose_generation_strategy(search_space=ss)
             self.assertEqual(bo_mixed_2._steps[0].model, Models.SOBOL)
             self.assertEqual(bo_mixed_2._steps[0].num_trials, 5)
             self.assertEqual(bo_mixed_2._steps[1].model, Models.BO_MIXED)
             expected_model_kwargs = {
                 "torch_device": None,
-                "transforms": expected_transforms,
+                "transforms": [Winsorize] + Mixed_transforms + Y_trans,
                 "transform_configs": expected_transform_configs,
             }
             self.assertEqual(bo_mixed._steps[1].model_kwargs, expected_model_kwargs)
         with self.subTest("BO_MIXED (mixed multi-objective optimization)"):
             search_space = get_branin_search_space(with_choice_parameter=True)
             search_space.parameters["x2"]._is_ordered = False
             optimization_config = MultiObjectiveOptimizationConfig(
@@ -722,7 +722,46 @@
         # Default to False.
         self.assertFalse(gs._steps[1].use_update)
         # Error with True.
         with self.assertRaisesRegex(UnsupportedError, "use_update"):
             choose_generation_strategy(
                 search_space=search_space, experiment=experiment, use_update=True
             )
+
+    def test_jit_compile(self) -> None:
+        for jit_compile in (True, False):
+            with self.subTest(str(jit_compile)):
+                sobol_saasbo = choose_generation_strategy(
+                    search_space=get_branin_search_space(),
+                    jit_compile=jit_compile,
+                    use_saasbo=True,
+                )
+                self.assertEqual(sobol_saasbo._steps[0].model, Models.SOBOL)
+                self.assertNotIn(
+                    "jit_compile",
+                    not_none(sobol_saasbo._steps[0].model_kwargs),
+                )
+                self.assertEqual(sobol_saasbo._steps[1].model, Models.FULLYBAYESIAN)
+                self.assertEqual(
+                    not_none(sobol_saasbo._steps[1].model_kwargs)["jit_compile"],
+                    jit_compile,
+                )
+
+    def test_jit_compile_for_non_saasbo_discards_the_model_kwarg(self) -> None:
+        for jit_compile in (True, False):
+            with self.subTest(str(jit_compile)):
+                gp_saasbo = choose_generation_strategy(
+                    search_space=get_branin_search_space(),
+                    jit_compile=jit_compile,
+                    use_saasbo=False,
+                )
+                self.assertEqual(len(gp_saasbo._steps), 2)
+                self.assertEqual(gp_saasbo._steps[0].model, Models.SOBOL)
+                self.assertNotIn(
+                    "jit_compile",
+                    not_none(gp_saasbo._steps[0].model_kwargs),
+                )
+                self.assertEqual(gp_saasbo._steps[1].model, Models.GPEI)
+                self.assertNotIn(
+                    "jit_compile",
+                    not_none(gp_saasbo._steps[1].model_kwargs),
+                )
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_factory.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_generation_node.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_generation_node.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_generation_strategy.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_generation_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import cast, List
+from unittest import mock
 from unittest.mock import MagicMock, patch
 
 import numpy as np
 
 from ax.core.arm import Arm
 from ax.core.base_trial import TrialStatus
 from ax.core.experiment import Experiment
@@ -55,15 +56,17 @@
         self.gr = GeneratorRun(arms=[Arm(parameters={"x1": 1, "x2": 2})])
 
         # Mock out slow GPEI.
         self.torch_model_bridge_patcher = patch(
             f"{TorchModelBridge.__module__}.TorchModelBridge", spec=True
         )
         self.mock_torch_model_bridge = self.torch_model_bridge_patcher.start()
-        self.mock_torch_model_bridge.return_value.gen.return_value = self.gr
+        mock_mb = self.mock_torch_model_bridge.return_value
+        mock_mb.gen.return_value = self.gr
+        mock_mb._process_and_transform_data.return_value = (None, None)
 
         # Mock out slow TS.
         self.discrete_model_bridge_patcher = patch(
             f"{DiscreteModelBridge.__module__}.DiscreteModelBridge", spec=True
         )
         self.mock_discrete_model_bridge = self.discrete_model_bridge_patcher.start()
         self.mock_discrete_model_bridge.return_value.gen.return_value = self.gr
@@ -298,14 +301,15 @@
                         "optimization_config": None,
                         "status_quo_features": None,
                         "status_quo_name": None,
                         "transform_configs": None,
                         "transforms": Cont_X_trans,
                         "fit_out_of_design": False,
                         "fit_abandoned": False,
+                        "fit_on_init": True,
                     },
                 )
                 ms = g._model_state_after_gen
                 self.assertIsNotNone(ms)
                 # Generated points are randomized, so just checking that they are there.
                 self.assertIn("generated_points", ms)
                 # Remove the randomized generated points to compare the rest.
@@ -616,16 +620,20 @@
             g = sobol.gen(exp)
             exp.new_trial(generator_run=g).run()
 
         self.assertEqual(len(exp.arms_by_signature), 2)
 
         with self.assertRaisesRegex(
             GenerationStrategyRepeatedPoints, "exceeded `MAX_GEN_DRAWS`"
-        ):
+        ), mock.patch("ax.modelbridge.generation_node.logger.info") as mock_logger:
             g = sobol.gen(exp)
+        self.assertEqual(mock_logger.call_count, 5)
+        self.assertIn(
+            "The generator run produced duplicate arms.", mock_logger.call_args[0][0]
+        )
 
     def test_current_generator_run_limit(self) -> None:
         NUM_INIT_TRIALS = 5
         SECOND_STEP_PARALLELISM = 3
         NUM_ROUNDS = 4
         exp = get_branin_experiment()
         sobol_gs_with_parallelism_limits = GenerationStrategy(
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_int_range_to_choice_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_int_range_to_choice_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_int_to_float_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_int_to_float_transform.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ax.core.observation import ObservationFeatures
 from ax.core.parameter import ChoiceParameter, ParameterType, RangeParameter
 from ax.core.parameter_constraint import OrderConstraint, SumConstraint
 from ax.core.search_space import RobustSearchSpace, SearchSpace
 from ax.exceptions.core import UnsupportedError
 from ax.modelbridge.transforms.int_to_float import IntToFloat
 from ax.utils.common.testutils import TestCase
+from ax.utils.common.typeutils import checked_cast
 from ax.utils.testing.core_stubs import get_robust_search_space
 
 
 class IntToFloatTransformTest(TestCase):
     def setUp(self) -> None:
         parameters = [
             RangeParameter("x", lower=1, upper=3, parameter_type=ParameterType.FLOAT),
@@ -47,14 +48,23 @@
             config={"rounding": "randomized"},
         )
         self.t3 = IntToFloat(
             search_space=self.search_space,
             observations=[],
             config={"min_choices": 3},
         )
+        self.search_space_with_log = self.search_space.clone()
+        checked_cast(
+            RangeParameter, self.search_space_with_log.parameters["a"]
+        )._log_scale = True
+        self.t4 = IntToFloat(
+            search_space=self.search_space_with_log,
+            observations=[],
+            config={"min_choices": 3},
+        )
 
     def testInit(self) -> None:
         self.assertEqual(self.t.transform_parameters, {"a", "d"})
 
     def test_transform_observation_features(self) -> None:
         observation_features = [
             ObservationFeatures(parameters={"x": 2.2, "a": 2, "b": "b", "d": 3})
@@ -75,15 +85,27 @@
         obs_ft2 = self.t3.transform_observation_features(obs_ft2)
         self.assertEqual(
             obs_ft2,
             [ObservationFeatures(parameters={"x": 2.2, "a": 2, "b": "b", "d": 3})],
         )
         self.assertTrue(isinstance(obs_ft2[0].parameters["a"], int))
         self.assertTrue(isinstance(obs_ft2[0].parameters["d"], float))
-        obs_ft2 = self.t.untransform_observation_features(obs_ft2)
+        obs_ft2 = self.t3.untransform_observation_features(obs_ft2)
+        self.assertEqual(obs_ft2, observation_features)
+
+        # With log_scale & min_choices. Both a & d should get transformed.
+        obs_ft2 = deepcopy(observation_features)
+        obs_ft2 = self.t4.transform_observation_features(obs_ft2)
+        self.assertEqual(
+            obs_ft2,
+            [ObservationFeatures(parameters={"x": 2.2, "a": 2, "b": "b", "d": 3})],
+        )
+        self.assertTrue(isinstance(obs_ft2[0].parameters["a"], float))
+        self.assertTrue(isinstance(obs_ft2[0].parameters["d"], float))
+        obs_ft2 = self.t4.untransform_observation_features(obs_ft2)
         self.assertEqual(obs_ft2, observation_features)
 
         # Let the transformed space be a float, verify it becomes an int.
         obs_ft3 = [
             ObservationFeatures(parameters={"x": 2.2, "a": 2.2, "b": "b", "d": 2.9})
         ]
         obs_ft3 = self.t.untransform_observation_features(obs_ft3)
@@ -95,14 +117,24 @@
         ]
         obs_ft3 = self.t3.untransform_observation_features(obs_ft3)
         self.assertEqual(
             obs_ft3,
             [ObservationFeatures(parameters={"x": 2.2, "a": 2.2, "b": "b", "d": 3})],
         )
 
+        # With log_scale & min_choices. Both a & d should become ints.
+        obs_ft3 = [
+            ObservationFeatures(parameters={"x": 2.2, "a": 2.2, "b": "b", "d": 2.9})
+        ]
+        obs_ft3 = self.t4.untransform_observation_features(obs_ft3)
+        self.assertEqual(
+            obs_ft3,
+            [ObservationFeatures(parameters={"x": 2.2, "a": 2, "b": "b", "d": 3})],
+        )
+
         # Test forward transform on partial observation
         obs_ft4 = [ObservationFeatures(parameters={"x": 2.2, "d": 3})]
         obs_ft4 = self.t.transform_observation_features(obs_ft4)
         self.assertEqual(obs_ft4, [ObservationFeatures(parameters={"x": 2.2, "d": 3})])
         self.assertTrue(isinstance(obs_ft4[0].parameters["d"], float))
         obs_ft5 = self.t.transform_observation_features([ObservationFeatures({})])
         self.assertEqual(obs_ft5[0], ObservationFeatures({}))
@@ -139,14 +171,19 @@
         self.assertTrue(ss2.parameters["a"].parameter_type, ParameterType.FLOAT)
         self.assertTrue(ss2.parameters["d"].parameter_type, ParameterType.FLOAT)
         # With min_choices, only d should be transformed.
         ss2 = deepcopy(self.search_space)
         ss2 = self.t3.transform_search_space(ss2)
         self.assertTrue(ss2.parameters["a"].parameter_type, ParameterType.INT)
         self.assertTrue(ss2.parameters["d"].parameter_type, ParameterType.FLOAT)
+        # With log_scale & min_choices. Both a & d should get transformed.
+        ss2 = deepcopy(self.search_space)
+        ss2 = self.t4.transform_search_space(ss2)
+        self.assertTrue(ss2.parameters["a"].parameter_type, ParameterType.FLOAT)
+        self.assertTrue(ss2.parameters["d"].parameter_type, ParameterType.FLOAT)
 
     def testRoundingWithConstrainedIntRanges(self) -> None:
         parameters = [
             RangeParameter("x", lower=1, upper=3, parameter_type=ParameterType.INT),
             RangeParameter("y", lower=1, upper=3, parameter_type=ParameterType.INT),
         ]
         constrained_int_search_space = SearchSpace(
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_ivw_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_ivw_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_log_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_log_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_log_y_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_log_y_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_logit_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_logit_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_map_torch_modelbridge.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_map_torch_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_map_unit_x_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_map_unit_x_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_metrics_as_task_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_metrics_as_task_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_model_spec.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_model_spec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import warnings
-from unittest.mock import Mock, patch
+from unittest import mock
+from unittest.mock import MagicMock, Mock, patch
 
 from ax.core.observation import ObservationFeatures
 from ax.exceptions.core import UserInputError
 from ax.modelbridge.factory import get_sobol
 from ax.modelbridge.model_spec import FactoryFunctionModelSpec, ModelSpec
+from ax.modelbridge.modelbridge_utils import extract_search_space_digest
 from ax.modelbridge.registry import Models
 from ax.utils.common.testutils import TestCase
 from ax.utils.testing.core_stubs import get_branin_experiment
 from ax.utils.testing.mock import fast_botorch_optimize
 
 
 class BaseModelSpecTest(TestCase):
@@ -35,31 +37,57 @@
         with self.assertRaises(UserInputError):
             ms.gen(n=1)
         ms.fit(experiment=self.experiment, data=self.data)
         ms.gen(n=1)
         with self.assertRaises(NotImplementedError):
             ms.update(experiment=self.experiment, new_data=self.data)
 
+    @fast_botorch_optimize
+    # We can use `extract_search_space_digest` as a surrogate for executing
+    # the full TorchModelBridge._fit.
+    @mock.patch(
+        "ax.modelbridge.torch.extract_search_space_digest",
+        wraps=extract_search_space_digest,
+    )
+    def test_fit(self, wrapped_extract_ssd: Mock) -> None:
+        ms = ModelSpec(model_enum=Models.GPEI)
+        # This should fit the model as usual.
+        ms.fit(experiment=self.experiment, data=self.data)
+        wrapped_extract_ssd.assert_called_once()
+        self.assertIsNotNone(ms._last_fit_arg_ids)
+        self.assertEqual(ms._last_fit_arg_ids["experiment"], id(self.experiment))
+        # This should skip the model fit.
+        with mock.patch("ax.modelbridge.torch.logger") as mock_logger:
+            ms.fit(experiment=self.experiment, data=self.data)
+        mock_logger.info.assert_called_with(
+            "The observations are identical to the last set of observations "
+            "used to fit the model. Skipping model fitting."
+        )
+        wrapped_extract_ssd.assert_called_once()
+
     def test_model_key(self) -> None:
         ms = ModelSpec(model_enum=Models.GPEI)
         self.assertEqual(ms.model_key, "GPEI")
 
     @patch(f"{ModelSpec.__module__}.compute_diagnostics")
     @patch(f"{ModelSpec.__module__}.cross_validate", return_value=["fake-cv-result"])
-    # pyre-fixme[3]: Return type must be annotated.
-    def test_cross_validate_with_GP_model(self, mock_cv: Mock, mock_diagnostics: Mock):
+    def test_cross_validate_with_GP_model(
+        self, mock_cv: Mock, mock_diagnostics: Mock
+    ) -> None:
         mock_enum = Mock()
-        mock_enum.return_value = "fake-modelbridge"
+        fake_mb = MagicMock()
+        fake_mb._process_and_transform_data = MagicMock(return_value=(None, None))
+        mock_enum.return_value = fake_mb
         ms = ModelSpec(model_enum=mock_enum, model_cv_kwargs={"test_key": "test-value"})
         ms.fit(
             experiment=self.experiment,
             data=self.experiment.trials[0].fetch_data(),
         )
         cv_results, cv_diagnostics = ms.cross_validate()
-        mock_cv.assert_called_with(model="fake-modelbridge", test_key="test-value")
+        mock_cv.assert_called_with(model=fake_mb, test_key="test-value")
         mock_diagnostics.assert_called_with(["fake-cv-result"])
 
         self.assertIsNotNone(cv_results)
         self.assertIsNotNone(cv_diagnostics)
 
         with self.subTest("it caches CV results"):
             mock_cv.reset_mock()
@@ -80,23 +108,22 @@
                 experiment=self.experiment,
                 data=self.experiment.trials[0].fetch_data(),
             )
             cv_results, cv_diagnostics = ms.cross_validate()
 
             self.assertIsNotNone(cv_results)
             self.assertIsNotNone(cv_diagnostics)
-            mock_cv.assert_called_with(model="fake-modelbridge", test_key="test-value")
+            mock_cv.assert_called_with(model=fake_mb, test_key="test-value")
             mock_diagnostics.assert_called_with(["fake-cv-result"])
 
     @patch(f"{ModelSpec.__module__}.compute_diagnostics")
     @patch(f"{ModelSpec.__module__}.cross_validate", side_effect=NotImplementedError)
-    # pyre-fixme[3]: Return type must be annotated.
     def test_cross_validate_with_non_GP_model(
         self, mock_cv: Mock, mock_diagnostics: Mock
-    ):
+    ) -> None:
         mock_enum = Mock()
         mock_enum.return_value = "fake-modelbridge"
         ms = ModelSpec(model_enum=mock_enum, model_cv_kwargs={"test_key": "test-value"})
         ms.fit(
             experiment=self.experiment,
             data=self.experiment.trials[0].fetch_data(),
         )
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_modelbridge_utils.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_modelbridge_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 from typing import List, Union
 
 import numpy as np
 from ax.core.metric import Metric
 from ax.core.objective import MultiObjective
 from ax.core.optimization_config import MultiObjectiveOptimizationConfig
 from ax.core.outcome_constraint import ObjectiveThreshold, OutcomeConstraint
+from ax.core.parameter import ChoiceParameter, ParameterType, RangeParameter
 from ax.core.risk_measures import RiskMeasure
-from ax.core.search_space import RobustSearchSpace
+from ax.core.search_space import RobustSearchSpace, SearchSpace
 from ax.core.types import ComparisonOp
 from ax.exceptions.core import UserInputError
 from ax.modelbridge.modelbridge_utils import (
     _array_to_tensor,
     extract_risk_measure,
     extract_robust_digest,
     feasible_hypervolume,
     RISK_MEASURE_NAME_TO_CLASS,
+    transform_search_space,
 )
+from ax.modelbridge.registry import Cont_X_trans, Y_trans
 from ax.utils.common.testutils import TestCase
 from ax.utils.common.typeutils import not_none
 from ax.utils.testing.core_stubs import get_robust_search_space, get_search_space
 from botorch.acquisition.risk_measures import VaR
 
 
 class TestModelBridgeUtils(TestCase):
@@ -207,7 +210,60 @@
                         1.0,
                         -2.0,
                     ]
                 ),
             },
         )
         self.assertEqual(list(feas_hv), [0.0, 0.0, 1.0, 1.0])
+
+    def test_get_transformed_dimensionality(self) -> None:
+        search_space = SearchSpace(
+            parameters=[
+                RangeParameter(
+                    name="range",
+                    parameter_type=ParameterType.FLOAT,
+                    lower=1,
+                    upper=8,
+                ),
+                ChoiceParameter(
+                    name="choice",
+                    parameter_type=ParameterType.INT,
+                    values=[11, 18, 1998],
+                    is_ordered=False,
+                ),
+            ]
+        )
+
+        transformed_search_space = transform_search_space(
+            search_space=search_space,
+            transforms=Cont_X_trans + Y_trans,
+            transform_configs={},
+        )
+
+        expected = SearchSpace(
+            parameters=[
+                RangeParameter(
+                    name="range", parameter_type=ParameterType.FLOAT, lower=0, upper=1
+                ),
+                RangeParameter(
+                    name="choice_OH_PARAM__0",
+                    parameter_type=ParameterType.FLOAT,
+                    lower=0,
+                    upper=1,
+                ),
+                RangeParameter(
+                    name="choice_OH_PARAM__1",
+                    parameter_type=ParameterType.FLOAT,
+                    lower=0,
+                    upper=1,
+                ),
+                RangeParameter(
+                    name="choice_OH_PARAM__2",
+                    parameter_type=ParameterType.FLOAT,
+                    lower=0,
+                    upper=1,
+                ),
+            ],
+            parameter_constraints=[],
+        )
+
+        self.assertEqual(transformed_search_space, expected)
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_one_hot_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_one_hot_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_pairwise_modelbridge.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_pairwise_modelbridge.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,7 +112,12 @@
         with self.assertRaises(ValueError):
             _binary_pref_to_comp_pair(Y=bad_Y)
 
         # `_consolidate_comparisons`.
         consolidated_X, consolidated_Y = _consolidate_comparisons(X=X, Y=comp_pair_Y)
         self.assertTrue(torch.equal(consolidated_X, expected_X))
         self.assertTrue(torch.equal(consolidated_Y, expected_Y))
+
+        with self.assertRaises(ValueError):
+            _consolidate_comparisons(
+                X=X.expand(2, *X.shape), Y=comp_pair_Y.expand(2, *comp_pair_Y.shape)
+            )
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_percentile_y_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_percentile_y_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_power_transform_y.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_power_transform_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_prediction_utils.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_prediction_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_random_modelbridge.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_random_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_registry.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
                 "torch_device": None,
                 "status_quo_name": None,
                 "status_quo_features": None,
                 "optimization_config": None,
                 "transforms": Cont_X_trans + Y_trans,
                 "fit_out_of_design": False,
                 "fit_abandoned": False,
+                "fit_on_init": True,
                 "default_model_gen_options": None,
             },
         )
         prior_kwargs = {"lengthscale_prior": GammaPrior(6.0, 6.0)}
         gpei = Models.GPEI(
             experiment=exp,
             data=exp.fetch_data(),
@@ -226,14 +227,15 @@
                     "optimization_config": None,
                     "transforms": Cont_X_trans,
                     "transform_configs": None,
                     "status_quo_name": None,
                     "status_quo_features": None,
                     "fit_out_of_design": False,
                     "fit_abandoned": False,
+                    "fit_on_init": True,
                 },
             ),
         )
         self.assertTrue(
             all(
                 kw in Models.SOBOL.view_kwargs()[0]
                 for kw in ["seed", "deduplicate", "init_position", "scramble"]
@@ -247,14 +249,15 @@
                     "experiment",
                     "data",
                     "transform_configs",
                     "status_quo_name",
                     "status_quo_features",
                     "fit_out_of_design",
                     "fit_abandoned",
+                    "fit_on_init",
                 ]
             ),
         )
 
     @fast_botorch_optimize
     def test_get_model_from_generator_run(self) -> None:
         """Tests that it is possible to restore a model from a generator run it
@@ -311,15 +314,15 @@
             self.assertIn(key, gpei_restored.model.__dict__)
             original, restored = (
                 gpei.model.__dict__[key],
                 gpei_restored.model.__dict__[key],
             )
             # Botorch model equality is tough to compare and training data
             # is unnecessary to compare, because data passed to model was the same
-            if key in ["model", "warm_start_refitting", "Xs", "Ys"]:
+            if key in ["_model", "warm_start_refitting", "Xs", "Ys"]:
                 continue
             self.assertEqual(original, restored)
 
     def test_ModelSetups_do_not_share_kwargs(self) -> None:
         """Tests that none of the preset model and bridge combinations share a
         kwarg.
         """
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_relativize_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_relativize_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_rembo_strategy.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_rembo_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_remove_fixed_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_remove_fixed_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_robust.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_robust.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_rounding.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_rounding.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_search_space_to_choice_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_search_space_to_choice_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_standardize_y_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_standardize_y_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_stratified_standardize_y.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_stratified_standardize_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_task_encode_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_task_encode_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_torch_modelbridge.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_torch_modelbridge_moo.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge_moo.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     observed_pareto_frontier,
     pareto_frontier,
     predicted_hypervolume,
     predicted_pareto_frontier,
 )
 from ax.modelbridge.registry import Cont_X_trans, ST_MTGP_trans, Y_trans
 from ax.modelbridge.torch import TorchModelBridge
+from ax.models.torch.botorch_modular.model import BoTorchModel
 from ax.models.torch.botorch_moo import MultiObjectiveBotorchModel
 from ax.models.torch.botorch_moo_defaults import (
     infer_objective_thresholds,
     pareto_frontier_evaluator,
 )
 from ax.service.utils.report_utils import exp_to_df
 from ax.utils.common.testutils import TestCase
@@ -689,14 +690,49 @@
         self.assertEqual(obj_thresholds[0].metric.name, "branin_a")
         self.assertEqual(obj_thresholds[1].metric.name, "branin_b")
         self.assertEqual(obj_thresholds[0].op, ComparisonOp.GEQ)
         self.assertEqual(obj_thresholds[1].op, ComparisonOp.GEQ)
         self.assertFalse(obj_thresholds[0].relative)
         self.assertFalse(obj_thresholds[1].relative)
 
+        # test with MBM
+        exp = get_branin_experiment_with_multi_objective(
+            has_optimization_config=True,
+            with_batch=True,
+            with_status_quo=True,
+        )
+        for trial in exp.trials.values():
+            trial.mark_running(no_runner_required=True).mark_completed()
+        exp.attach_data(
+            get_branin_data_multi_objective(trial_indices=exp.trials.keys())
+        )
+        data = exp.fetch_data()
+        modelbridge = TorchModelBridge(
+            search_space=exp.search_space,
+            model=BoTorchModel(),
+            optimization_config=exp.optimization_config,
+            transforms=Cont_X_trans + Y_trans,
+            torch_device=torch.device("cuda" if cuda else "cpu"),
+            experiment=exp,
+            data=data,
+            # [T143911996] The trials get ignored without fit_out_of_design.
+            fit_out_of_design=True,
+        )
+        obj_thresholds = modelbridge.infer_objective_thresholds(
+            search_space=exp.search_space,
+            optimization_config=exp.optimization_config,
+            fixed_features=None,
+        )
+        self.assertEqual(obj_thresholds[0].metric.name, "branin_a")
+        self.assertEqual(obj_thresholds[1].metric.name, "branin_b")
+        self.assertEqual(obj_thresholds[0].op, ComparisonOp.GEQ)
+        self.assertEqual(obj_thresholds[1].op, ComparisonOp.GEQ)
+        self.assertFalse(obj_thresholds[0].relative)
+        self.assertFalse(obj_thresholds[1].relative)
+
     @fast_botorch_optimize
     def test_status_quo_for_non_monolithic_data(self) -> None:
         exp = get_branin_experiment_with_multi_objective(with_status_quo=True)
         sobol_generator = get_sobol(
             search_space=exp.search_space,
         )
         sobol_run = sobol_generator.gen(n=5)
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_transform_utils.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_transform_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_trial_as_task_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_trial_as_task_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_unit_x_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_unit_x_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_utils.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from unittest import mock
 from unittest.mock import patch
 
 import numpy as np
 from ax.core.arm import Arm
 from ax.core.base_trial import TrialStatus
 from ax.core.data import Data
 from ax.core.generator_run import GeneratorRun
@@ -602,19 +603,35 @@
         with self.assertRaises(ValueError):
             extract_objective_thresholds(
                 objective_thresholds=objective_thresholds,
                 objective=objective,
                 outcomes=outcomes,
             )
 
-    def testObservationDataToArray(self) -> None:
+    def test_observation_data_to_array(self) -> None:
         outcomes = ["a", "b", "c"]
         obsd = ObservationData(
             metric_names=["c", "a", "b"],
             means=np.array([1, 2, 3]),
             covariance=np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]),
         )
         Y, Ycov = observation_data_to_array(outcomes=outcomes, observation_data=[obsd])
         self.assertTrue(np.array_equal(Y, np.array([[2, 3, 1]])))
         self.assertTrue(
             np.array_equal(Ycov, np.array([[[5, 6, 4], [8, 9, 7], [2, 3, 1]]]))
         )
+
+        # With missing metrics.
+        obsd2 = ObservationData(
+            metric_names=["c", "a"],
+            means=np.array([1, 2]),
+            covariance=np.array([[1, 2], [4, 5]]),
+        )
+        with mock.patch("ax.modelbridge.modelbridge_utils.logger.warning") as mock_warn:
+            Y, Ycov = observation_data_to_array(
+                outcomes=outcomes, observation_data=[obsd, obsd2]
+            )
+        self.assertTrue(np.array_equal(Y, np.array([[2, 3, 1]])))
+        self.assertTrue(
+            np.array_equal(Ycov, np.array([[[5, 6, 4], [8, 9, 7], [2, 3, 1]]]))
+        )
+        mock_warn.assert_called_once()
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_winsorize_transform.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/tests/test_winsorize_transform_legacy.py` & `ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform_legacy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/torch.py` & `ax-platform-0.3.2/ax/modelbridge/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 from ax.modelbridge.transforms.cast import Cast
 from ax.models.torch.botorch_modular.model import BoTorchModel
 from ax.models.torch.botorch_moo import MultiObjectiveBotorchModel
 from ax.models.torch.botorch_moo_defaults import infer_objective_thresholds
 from ax.models.torch_base import TorchModel, TorchOptConfig
 from ax.models.types import TConfig
 from ax.utils.common.logger import get_logger
-from ax.utils.common.typeutils import checked_cast, not_none
+from ax.utils.common.typeutils import not_none
 from botorch.utils.datasets import FixedNoiseDataset, SupervisedDataset
 from torch import Tensor
 
 logger: Logger = get_logger(__name__)
 
 FIT_MODEL_ERROR = "Model must be fit before {action}."
 
@@ -103,14 +103,15 @@
         torch_dtype: Optional[torch.dtype] = None,
         torch_device: Optional[torch.device] = None,
         status_quo_name: Optional[str] = None,
         status_quo_features: Optional[ObservationFeatures] = None,
         optimization_config: Optional[OptimizationConfig] = None,
         fit_out_of_design: bool = False,
         fit_abandoned: bool = False,
+        fit_on_init: bool = True,
         default_model_gen_options: Optional[TConfig] = None,
     ) -> None:
         self.dtype: torch.dtype = torch.double if torch_dtype is None else torch_dtype
         self.device = torch_device
         self._default_model_gen_options = default_model_gen_options or {}
 
         # Handle init for multi-objective optimization.
@@ -129,14 +130,15 @@
             transforms=transforms,
             transform_configs=transform_configs,
             status_quo_name=status_quo_name,
             status_quo_features=status_quo_features,
             optimization_config=optimization_config,
             fit_out_of_design=fit_out_of_design,
             fit_abandoned=fit_abandoned,
+            fit_on_init=fit_on_init,
         )
 
     def feature_importances(self, metric_name: str) -> Dict[str, float]:
         importances_tensor = not_none(self.model).feature_importances()
         importances_dict = dict(zip(self.outcomes, importances_tensor))
         importances_arr = importances_dict[metric_name].flatten()
         return dict(zip(self.parameters, importances_arr))
@@ -178,23 +180,35 @@
             optimization_config=base_gen_args.optimization_config,
         )
         if torch_opt_config.risk_measure is not None:  # pragma: no cover
             raise UnsupportedError(
                 "`infer_objective_thresholds` does not support risk measures."
             )
         # Infer objective thresholds.
-        model = checked_cast(MultiObjectiveBotorchModel, self.model)
+        if isinstance(self.model, MultiObjectiveBotorchModel):
+            model = self.model.model
+            Xs = self.model.Xs
+        elif isinstance(self.model, BoTorchModel):
+            model = self.model.surrogate.model
+            Xs = self.model.surrogate.Xs
+        else:
+            raise UnsupportedError(  # pragma: no cover
+                "Model must be a MultiObjectiveBotorchModel or an appropriate Modular "
+                "Botorch Model to infer_objective_thresholds. Found "
+                f"{type(self.model)}."
+            )
+
         obj_thresholds = infer_objective_thresholds(
-            model=not_none(model.model),
+            model=not_none(model),
             objective_weights=torch_opt_config.objective_weights,
             bounds=search_space_digest.bounds,
             outcome_constraints=torch_opt_config.outcome_constraints,
             linear_constraints=torch_opt_config.linear_constraints,
             fixed_features=torch_opt_config.fixed_features,
-            Xs=model.Xs,
+            Xs=Xs,
         )
 
         return self._untransform_objective_thresholds(
             objective_thresholds=obj_thresholds,
             objective_weights=torch_opt_config.objective_weights,
             bounds=search_space_digest.bounds,
             # we should never be in a situation where we call this without there
@@ -324,14 +338,15 @@
 
     def _cross_validate(
         self,
         search_space: SearchSpace,
         cv_training_data: List[Observation],
         cv_test_points: List[ObservationFeatures],
         parameters: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> List[ObservationData]:
         """Make predictions at cv_test_points using only the data in obs_feats
         and obs_data.
         """
         if self.model is None:
             raise ValueError(  # pragma: no cover
                 FIT_MODEL_ERROR.format(action="_cross_validate")
@@ -361,14 +376,15 @@
         )
         # Use the model to do the cross validation
         f_test, cov_test = not_none(self.model).cross_validate(
             datasets=[not_none(dataset) for dataset in datasets],
             metric_names=self.outcomes,
             X_test=torch.as_tensor(X_test, dtype=self.dtype, device=self.device),
             search_space_digest=search_space_digest,
+            **kwargs,
         )
         # Convert array back to ObservationData
         return array_to_observation_data(
             f=f_test.detach().cpu().clone().numpy(),
             cov=cov_test.detach().cpu().clone().numpy(),
             outcomes=self.outcomes,
         )
@@ -475,14 +491,15 @@
 
     def _fit(
         self,
         model: TorchModel,
         search_space: SearchSpace,
         observations: List[Observation],
         parameters: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> None:  # pragma: no cover
         if self.model is not None and observations == self._last_observations:
             logger.info(
                 "The observations are identical to the last set of observations "
                 "used to fit the model. Skipping model fitting."
             )
             return
@@ -510,14 +527,15 @@
         self.model = model
         self.model.fit(
             # datasets are guaranteed to have all outcomes here by construction
             datasets=[not_none(dataset) for dataset in datasets],
             metric_names=self.outcomes,
             search_space_digest=search_space_digest,
             candidate_metadata=candidate_metadata,
+            **kwargs,
         )
 
     def _gen(
         self,
         n: int,
         search_space: SearchSpace,
         pending_observations: Dict[str, List[ObservationFeatures]],
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/base.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/cap_parameter.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/cap_parameter.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/cast.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/cast.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/choice_encode.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/choice_encode.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/convert_metric_names.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/convert_metric_names.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/derelativize.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/derelativize.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/int_range_to_choice.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/int_range_to_choice.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/int_to_float.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/int_to_float.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 class IntToFloat(Transform):
     """Convert a RangeParameter of type int to type float.
 
     Uses either randomized_rounding or default python rounding,
     depending on 'rounding' flag.
 
     The `min_choices` config can be used to transform only the parameters
-    with cardinality greater than or equal to `min_choices`.
+    with cardinality greater than or equal to `min_choices`; with the exception
+    of `log_scale` parameters, which are always transformed.
 
     Transform is done in-place.
     """
 
     def __init__(
         self,
         search_space: Optional[SearchSpace] = None,
@@ -62,15 +63,15 @@
 
         # Identify parameters that should be transformed
         self.transform_parameters: Set[str] = {
             p_name
             for p_name, p in self.search_space.parameters.items()
             if isinstance(p, RangeParameter)
             and p.parameter_type == ParameterType.INT
-            and p.upper - p.lower + 1 >= self.min_choices
+            and (p.upper - p.lower + 1 >= self.min_choices or p.log_scale)
         }
         if contains_constrained_integer(self.search_space, self.transform_parameters):
             self.rounding = "randomized"
 
     def transform_observation_features(
         self, observation_features: List[ObservationFeatures]
     ) -> List[ObservationFeatures]:
```

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/ivw.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/ivw.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/log.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/log.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/log_y.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/log_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/logit.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/logit.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/map_unit_x.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/map_unit_x.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/metrics_as_task.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/metrics_as_task.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/one_hot.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/one_hot.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/percentile_y.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/percentile_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/power_transform_y.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/power_transform_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/relativize.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/relativize.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/remove_fixed.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/remove_fixed.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/rounding.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/rounding.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/search_space_to_choice.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/search_space_to_choice.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/standardize_y.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/standardize_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/stratified_standardize_y.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/stratified_standardize_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/task_encode.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/task_encode.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/trial_as_task.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/trial_as_task.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/unit_x.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/unit_x.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/utils.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/modelbridge/transforms/winsorize.py` & `ax-platform-0.3.2/ax/modelbridge/transforms/winsorize.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/base.py` & `ax-platform-0.3.2/ax/models/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/discrete/eb_thompson.py` & `ax-platform-0.3.2/ax/models/discrete/eb_thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/discrete/full_factorial.py` & `ax-platform-0.3.2/ax/models/discrete/full_factorial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/discrete/thompson.py` & `ax-platform-0.3.2/ax/models/discrete/thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/discrete_base.py` & `ax-platform-0.3.2/ax/models/discrete_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/model_utils.py` & `ax-platform-0.3.2/ax/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/random/alebo_initializer.py` & `ax-platform-0.3.2/ax/models/random/alebo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/random/base.py` & `ax-platform-0.3.2/ax/models/random/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/random/rembo_initializer.py` & `ax-platform-0.3.2/ax/models/random/rembo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/random/sobol.py` & `ax-platform-0.3.2/ax/models/random/sobol.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/random/uniform.py` & `ax-platform-0.3.2/ax/models/random/uniform.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,27 @@
     the fit or predict methods.
 
     Attributes:
         seed: An optional seed value for the underlying PRNG.
 
     """
 
-    def __init__(self, deduplicate: bool = True, seed: Optional[int] = None) -> None:
-        super().__init__(deduplicate=deduplicate, seed=seed)
+    def __init__(
+        self,
+        deduplicate: bool = True,
+        seed: Optional[int] = None,
+        generated_points: Optional[np.ndarray] = None,
+        fallback_to_sample_polytope: bool = False,
+    ) -> None:
+        super().__init__(
+            deduplicate=deduplicate,
+            seed=seed,
+            generated_points=generated_points,
+            fallback_to_sample_polytope=fallback_to_sample_polytope,
+        )
         self._rs = np.random.RandomState(seed=self.seed)
 
     def _gen_samples(self, n: int, tunable_d: int) -> np.ndarray:
         """Generate samples from the scipy uniform distribution.
 
         Args:
             n: Number of samples to generate.
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_alebo.py` & `ax-platform-0.3.2/ax/models/tests/test_alebo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_alebo_initializer.py` & `ax-platform-0.3.2/ax/models/tests/test_alebo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_base.py` & `ax-platform-0.3.2/ax/models/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_botorch_defaults.py` & `ax-platform-0.3.2/ax/models/tests/test_botorch_defaults.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_botorch_kg.py` & `ax-platform-0.3.2/ax/models/tests/test_botorch_kg.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,15 +127,14 @@
                 n=n,
                 search_space_digest=self.search_space_digest,
                 torch_opt_config=torch_opt_config,
             )
             mock_warmstart_initialization.assert_called_once()
 
         posterior_tf = ScalarizedPosteriorTransform(weights=self.objective_weights)
-        # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
         dummy_acq = PosteriorMean(model=model.model, posterior_transform=posterior_tf)
         with mock.patch(
             "ax.models.torch.utils.PosteriorMean", return_value=dummy_acq
         ) as mock_posterior_mean, mock.patch(
             "ax.models.torch.utils.get_botorch_objective_and_transform",
             return_value=(
                 None,
@@ -182,15 +181,14 @@
         model.fit(
             datasets=[self.dataset],
             search_space_digest=self.search_space_digest,
             metric_names=self.metric_names,
         )
         self.assertTrue(model.use_input_warping)
         self.assertTrue(hasattr(model.model, "input_transform"))
-        # pyre-fixme[16]: Optional type has no attribute `input_transform`.
         self.assertIsInstance(model.model.input_transform, Warp)
 
         # test loocv pseudo likelihood
         self.assertFalse(model.use_loocv_pseudo_likelihood)
         model = KnowledgeGradient(use_loocv_pseudo_likelihood=True)
         model.fit(
             datasets=[self.dataset],
@@ -279,15 +277,14 @@
         model.fit(
             datasets=[self.dataset],
             metric_names=["L2NormMetric"],
             search_space_digest=search_space_digest,
         )
         self.assertTrue(model.use_input_warping)
         self.assertTrue(hasattr(model.model, "input_transform"))
-        # pyre-fixme[16]: Optional type has no attribute `input_transform`.
         self.assertIsInstance(model.model.input_transform, Warp)
 
         # test loocv pseudo likelihood
         self.assertFalse(model.use_loocv_pseudo_likelihood)
         model = KnowledgeGradient(use_loocv_pseudo_likelihood=True)
         model.fit(
             datasets=[self.dataset],
@@ -309,45 +306,41 @@
         )
 
         # test _instantiate_KG
         posterior_tf = ScalarizedPosteriorTransform(weights=self.objective_weights)
 
         # test acquisition setting
         acq_function = _instantiate_KG(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             posterior_transform=posterior_tf,
             n_fantasies=10,
             qmc=True,
         )
         self.assertIsInstance(acq_function.sampler, SobolQMCNormalSampler)
         self.assertIsInstance(
             acq_function.posterior_transform, ScalarizedPosteriorTransform
         )
         self.assertEqual(acq_function.num_fantasies, 10)
 
         acq_function = _instantiate_KG(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             posterior_transform=posterior_tf,
             n_fantasies=10,
             qmc=False,
         )
         self.assertIsInstance(acq_function.sampler, IIDNormalSampler)
 
         acq_function = _instantiate_KG(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             posterior_transform=posterior_tf,
             qmc=False,
         )
         self.assertIsNone(acq_function.inner_sampler)
 
         acq_function = _instantiate_KG(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             posterior_transform=posterior_tf,
             qmc=True,
             X_pending=self.X_dummy,
         )
         self.assertIsNone(acq_function.inner_sampler)
         self.assertTrue(torch.equal(acq_function.X_pending, self.X_dummy))
@@ -389,35 +382,31 @@
                 feature_names=self.feature_names,
                 bounds=self.bounds,
                 fidelity_features=[-1],
             ),
         )
 
         acq_function = _instantiate_KG(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             posterior_transform=posterior_tf,
             target_fidelities={2: 1.0},
             # pyre-fixme[6]: For 4th param expected `Optional[Tensor]` but got `int`.
             current_value=0,
         )
         self.assertIsInstance(acq_function, qMultiFidelityKnowledgeGradient)
 
         acq_function = _instantiate_KG(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             objective=LinearMCObjective(weights=self.objective_weights),
         )
         self.assertIsInstance(acq_function.inner_sampler, SobolQMCNormalSampler)
 
         # test error that target fidelity and fidelity weight indices must match
         with self.assertRaises(RuntimeError):
             _instantiate_KG(
-                # pyre-fixme[6]: For 1st param expected `Model` but got
-                #  `Optional[Model]`.
                 model=model.model,
                 posterior_transform=posterior_tf,
                 target_fidelities={1: 1.0},
                 fidelity_weights={2: 1.0},
                 # pyre-fixme[6]: For 5th param expected `Optional[Tensor]` but got
                 #  `int`.
                 current_value=0,
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_botorch_mes.py` & `ax-platform-0.3.2/ax/models/tests/test_botorch_mes.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,14 @@
             #  got `List[FixedNoiseDataset]`.
             datasets=self.training_data,
             metric_names=self.metric_names,
             search_space_digest=self.search_space_digest,
         )
         self.assertTrue(model.use_input_warping)
         self.assertTrue(hasattr(model.model, "input_transform"))
-        # pyre-fixme[16]: Optional type has no attribute `input_transform`.
         self.assertIsInstance(model.model.input_transform, Warp)
 
         # test loocv pseudo likelihood
         self.assertFalse(model.use_loocv_pseudo_likelihood)
         model = MaxValueEntropySearch(use_loocv_pseudo_likelihood=True)
         model.fit(
             # pyre-fixme[6]: For 1st param expected `List[SupervisedDataset]` but
@@ -246,15 +245,14 @@
                 feature_names=self.feature_names,
                 bounds=self.bounds,
                 fidelity_features=[-1],
             ),
         )
         self.assertTrue(model.use_input_warping)
         self.assertTrue(hasattr(model.model, "input_transform"))
-        # pyre-fixme[16]: Optional type has no attribute `input_transform`.
         self.assertIsInstance(model.model.input_transform, Warp)
 
         # test loocv pseudo likelihood
         self.assertFalse(model.use_loocv_pseudo_likelihood)
         model = MaxValueEntropySearch(use_loocv_pseudo_likelihood=True)
         model.fit(
             # pyre-fixme[6]: For 1st param expected `List[SupervisedDataset]` but
@@ -279,27 +277,25 @@
                 bounds=self.bounds,
             ),
         )
 
         # test acquisition setting
         X_dummy = torch.ones(1, 3, **self.tkwargs)
         candidate_set = torch.rand(10, 3, **self.tkwargs)
-        # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
         acq_function = _instantiate_MES(model=model.model, candidate_set=candidate_set)
 
         self.assertIsInstance(acq_function, qMaxValueEntropy)
         self.assertIsInstance(acq_function.sampler, SobolQMCNormalSampler)
         self.assertIsInstance(acq_function.fantasies_sampler, SobolQMCNormalSampler)
         self.assertEqual(acq_function.num_fantasies, 16)
         self.assertEqual(acq_function.num_mv_samples, 10)
         self.assertEqual(acq_function.use_gumbel, True)
         self.assertEqual(acq_function.maximize, True)
 
         acq_function = _instantiate_MES(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             candidate_set=candidate_set,
             X_pending=X_dummy,
         )
         self.assertTrue(torch.equal(acq_function.X_pending, X_dummy))
 
         # multi-fidelity tests
@@ -314,28 +310,25 @@
                 bounds=self.bounds,
                 fidelity_features=[-1],
             ),
         )
 
         candidate_set = torch.rand(10, 3, **self.tkwargs)
         acq_function = _instantiate_MES(
-            # pyre-fixme[6]: For 1st param expected `Model` but got `Optional[Model]`.
             model=model.model,
             candidate_set=candidate_set,
             target_fidelities={2: 1.0},
         )
         self.assertIsInstance(acq_function, qMultiFidelityMaxValueEntropy)
         Xs = [self.training_data[0].X()]
         # pyre-fixme[29]: `Union[torch._tensor.Tensor,
         #  torch.nn.modules.module.Module]` is not a function.
         self.assertEqual(acq_function.expand(Xs), Xs)
 
         # test error that target fidelity and fidelity weight indices must match
         with self.assertRaises(RuntimeError):
             _instantiate_MES(
-                # pyre-fixme[6]: For 1st param expected `Model` but got
-                #  `Optional[Model]`.
                 model=model.model,
                 candidate_set=candidate_set,
                 target_fidelities={1: 1.0},
                 fidelity_weights={2: 1.0},
             )
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_botorch_model.py` & `ax-platform-0.3.2/ax/models/tests/test_botorch_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,39 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import dataclasses
 from itertools import chain, product
-from typing import Any, Dict
+from typing import Any, cast, Dict
 from unittest import mock
 
+import numpy as np
+
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.exceptions.core import DataRequiredError
-from ax.models.torch.botorch import BotorchModel, get_rounding_func
+from ax.models.torch.botorch import (
+    BotorchModel,
+    get_feature_importances_from_botorch_model,
+    get_rounding_func,
+)
 from ax.models.torch.botorch_defaults import (
     get_and_fit_model,
     get_chebyshev_scalarization,
     recommend_best_out_of_sample_point,
 )
 from ax.models.torch.utils import sample_simplex
 from ax.models.torch_base import TorchOptConfig
 from ax.utils.common.testutils import TestCase
 from ax.utils.testing.mock import fast_botorch_optimize
 from ax.utils.testing.torch_stubs import get_torch_test_data
 from botorch.acquisition.utils import get_infeasible_cost
-from botorch.models import FixedNoiseGP, ModelListGP
+from botorch.models import FixedNoiseGP, ModelListGP, SingleTaskGP
 from botorch.models.transforms.input import Warp
 from botorch.utils.datasets import FixedNoiseDataset
 from botorch.utils.objective import get_objective_weights_transform
 from gpytorch.likelihoods import _GaussianLikelihoodBase
 from gpytorch.mlls import ExactMarginalLogLikelihood, LeaveOneOutPseudoLikelihood
 from gpytorch.priors import GammaPrior
 from gpytorch.priors.lkj_prior import LKJCovariancePrior
@@ -57,30 +63,41 @@
             dtype=dtype, cuda=cuda, constant_noise=True
         )
         model = BotorchModel(multitask_gp_ranks={"y": 2, "w": 1})
         datasets = [
             FixedNoiseDataset(X=Xs1[0], Y=Ys1[0], Yvar=Yvars1[0]),
             FixedNoiseDataset(X=Xs2[0], Y=Ys2[0], Yvar=Yvars2[0]),
         ]
+        with self.assertRaisesRegex(RuntimeError, "Please fit the model first"):
+            model.model
+
+        with self.assertRaisesRegex(RuntimeError, "Please fit the model first"):
+            model.search_space_digest
+
+        search_space_digest = SearchSpaceDigest(
+            feature_names=fns,
+            bounds=bounds,
+            task_features=[0],
+        )
+        with self.assertRaisesRegex(RuntimeError, "manually is disallowed"):
+            model.search_space_digest = search_space_digest
 
         with mock.patch(FIT_MODEL_MO_PATH) as _mock_fit_model:
             model.fit(
                 datasets=datasets,
                 metric_names=["y", "w"],
-                search_space_digest=SearchSpaceDigest(
-                    feature_names=fns,
-                    bounds=bounds,
-                    task_features=[0],
-                ),
+                search_space_digest=search_space_digest,
             )
+            self.assertTrue(isinstance(model.search_space_digest, SearchSpaceDigest))
+            self.assertEqual(model.search_space_digest, search_space_digest)
             _mock_fit_model.assert_called_once()
 
+        model.model = model.model  # property assignment isn't blocked
         # Check ranks
-        # pyre-fixme[16]: Optional type has no attribute `models`.
-        model_list = model.model.models
+        model_list = cast(ModelListGP, model.model).models
         self.assertEqual(model_list[0]._rank, 2)
         self.assertEqual(model_list[1]._rank, 1)
 
     def test_fixed_prior_BotorchModel(
         self, dtype: torch.dtype = torch.float, cuda: bool = False
     ) -> None:
         Xs1, Ys1, Yvars1, bounds, _, fns, _ = get_torch_test_data(
@@ -115,16 +132,15 @@
                     bounds=bounds,
                     task_features=[0],
                 ),
             )
             _mock_fit_model.assert_called_once()
 
         # Check ranks
-        # pyre-fixme[16]: Optional type has no attribute `models`.
-        model_list = model.model.models
+        model_list = cast(ModelListGP, model.model).models
         for i in range(1):
             self.assertEqual(
                 model_list[i].covar_module.base_kernel.lengthscale_prior.concentration,
                 6.0,
             )
             self.assertEqual(
                 model_list[i].covar_module.base_kernel.lengthscale_prior.rate,
@@ -201,16 +217,15 @@
                 self.assertTrue(torch.equal(model.Xs[0], Xs1[0]))
                 self.assertTrue(torch.equal(model.Xs[1], Xs2_diff[0]))
                 self.assertEqual(model.dtype, Xs1[0].dtype)
                 self.assertEqual(model.device, Xs1[0].device)
                 self.assertIsInstance(model.model, ModelListGP)
 
                 # Check fitting
-                # pyre-fixme[16]: Optional type has no attribute `models`.
-                model_list = model.model.models
+                model_list = cast(ModelListGP, model.model).models
                 self.assertTrue(torch.equal(model_list[0].train_inputs[0], Xs1[0]))
                 self.assertTrue(torch.equal(model_list[1].train_inputs[0], Xs2_diff[0]))
                 self.assertTrue(
                     torch.equal(model_list[0].train_targets, Ys1[0].view(-1))
                 )
                 self.assertTrue(
                     torch.equal(model_list[1].train_targets, Ys2[0].view(-1))
@@ -481,25 +496,32 @@
                 model.update(
                     datasets=[FixedNoiseDataset(Xs2[0], Y=Ys2[0], Yvar=Yvars2[0])] * 2,
                     metric_names=["y1", "y2"],
                 )
 
             # test unfit model CV, update, and feature_importances
             unfit_model = BotorchModel()
-            with self.assertRaises(RuntimeError):
+            with self.assertRaisesRegex(
+                RuntimeError, r"Cannot cross-validate model that has not been fitted"
+            ):
                 unfit_model.cross_validate(
                     datasets=combined_datasets,
                     metric_names=["y1", "y2"],
                     X_test=Xs1[0],
                 )
-            with self.assertRaises(RuntimeError):
+            with self.assertRaisesRegex(
+                RuntimeError, r"Cannot update model that has not been fitted"
+            ):
                 unfit_model.update(
                     datasets=combined_datasets, metric_names=["y1", "y2"]
                 )
-            with self.assertRaises(RuntimeError):
+            with self.assertRaisesRegex(
+                RuntimeError,
+                r"Cannot calculate feature_importances without a fitted model",
+            ):
                 unfit_model.feature_importances()
 
             # Test loading state dict
             true_state_dict = {
                 "mean_module.raw_constant": 3.5004,
                 "covar_module.raw_outputscale": 2.2438,
                 "covar_module.base_kernel.raw_lengthscale": [
@@ -618,15 +640,14 @@
                 )
             X = torch.rand(2, 3, dtype=torch.float)
             f_mean, f_cov = model.predict(X)
             self.assertTrue(f_mean.shape == torch.Size([2, 1]))
             self.assertTrue(f_cov.shape == torch.Size([2, 1, 1]))
             if use_input_warping:
                 self.assertTrue(hasattr(model.model, "input_transform"))
-                # pyre-fixme[16]: Optional type has no attribute `input_transform`.
                 self.assertIsInstance(model.model.input_transform, Warp)
             else:
                 self.assertFalse(hasattr(model.model, "input_transform"))
 
     def test_BotorchModelConstraints(self) -> None:
         Xs1, Ys1, Yvars1, bounds, tfs, fns, mns = get_torch_test_data(
             dtype=torch.float, cuda=False, constant_noise=True
@@ -677,7 +698,32 @@
         model = BotorchModel()
         with self.assertRaisesRegex(
             DataRequiredError, "BotorchModel.fit requires non-empty data sets."
         ):
             model.fit(
                 datasets=[], metric_names=mns, search_space_digest=search_space_digest
             )
+
+    def test_get_feature_importances_from_botorch_model(self) -> None:
+        tkwargs = {"dtype": torch.double}
+        train_X = torch.rand(5, 3, **tkwargs)  # pyre-ignore [6]
+        train_Y = train_X.sum(dim=-1, keepdim=True)
+        simple_gp = SingleTaskGP(train_X=train_X, train_Y=train_Y)
+        simple_gp.covar_module.base_kernel.lengthscale = torch.tensor(
+            [1, 3, 5], **tkwargs  # pyre-ignore [6]
+        )
+        importances = get_feature_importances_from_botorch_model(simple_gp)
+        self.assertTrue(np.allclose(importances, np.array([15 / 23, 5 / 23, 3 / 23])))
+        self.assertEqual(importances.shape, (1, 1, 3))
+        # Model with no base kernel
+        simple_gp.covar_module.base_kernel = None  # pyre-ignore [16]
+        with self.assertRaisesRegex(
+            NotImplementedError,
+            "Failed to extract lengthscales from `m.covar_module.base_kernel`",
+        ):
+            get_feature_importances_from_botorch_model(simple_gp)
+
+        with self.assertRaisesRegex(
+            RuntimeError,
+            "Cannot calculate feature_importances without a fitted model",
+        ):
+            get_feature_importances_from_botorch_model(None)
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_botorch_moo_defaults.py` & `ax-platform-0.3.2/ax/models/tests/test_botorch_moo_defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         objective_thresholds = torch.zeros(2)
         with self.assertRaisesRegex(
             ValueError, "There are no feasible observed points."
         ):
             get_NEHVI(
                 # pyre-fixme[6]: For 1st param expected `Model` but got
                 #  `Optional[Model]`.
-                model=model.model,
+                model=model._model,
                 objective_weights=weights,
                 objective_thresholds=objective_thresholds,
             )
 
     @mock.patch(  # pyre-ignore
         "ax.models.torch.botorch_moo_defaults._check_posterior_type",
         wraps=lambda y: y,
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_botorch_moo_model.py` & `ax-platform-0.3.2/ax/models/tests/test_botorch_moo_model.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_cbo_lcea.py` & `ax-platform-0.3.2/ax/models/tests/test_cbo_lcea.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 
+from typing import cast
+
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.models.torch.cbo_lcea import LCEABO
 from ax.utils.common.testutils import TestCase
 from ax.utils.testing.mock import fast_botorch_optimize
 from botorch.models.contextual import LCEAGP
 from botorch.models.model_list_gp_regression import ModelListGP
@@ -77,16 +79,17 @@
             datasets=training_data,
             metric_names=["y"],
             search_space_digest=SearchSpaceDigest(
                 feature_names=["x1", "x2", "x3", "x4"],
                 bounds=[(0.0, 1.0) for _ in range(4)],
             ),
         )
-        # pyre-fixme[16]: Optional type has no attribute `decomposition`.
-        self.assertDictEqual(m2.model.decomposition, {"1": [0, 2], "2": [1, 3]})
+        self.assertDictEqual(
+            cast(LCEAGP, m2.model).decomposition, {"1": [0, 2], "2": [1, 3]}
+        )
 
         # Test decomposition validation in get_and_fit_model
         # does not pass feature names when decomposition uses feature names
         with self.assertRaises(ValueError):
             m2.fit(
                 datasets=training_data,
                 metric_names=["y"],
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_cbo_lcem.py` & `ax-platform-0.3.2/ax/models/tests/test_cbo_lcem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_cbo_sac.py` & `ax-platform-0.3.2/ax/models/tests/test_cbo_sac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 
+from typing import cast
+
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.models.torch.cbo_sac import SACBO, SACGP
 from ax.utils.common.testutils import TestCase
 from ax.utils.testing.mock import fast_botorch_optimize
+from botorch.models.contextual import LCEAGP
 from botorch.models.model_list_gp_regression import ModelListGP
 from botorch.utils.datasets import FixedNoiseDataset
 
 
 class SACBOTest(TestCase):
     @fast_botorch_optimize
     def test_SACBO(self) -> None:
@@ -72,16 +75,17 @@
             datasets=[dataset],
             metric_names=["y"],
             search_space_digest=SearchSpaceDigest(
                 feature_names=["x1", "x2", "x3", "x4"],
                 bounds=[(0.0, 1.0) for _ in range(4)],
             ),
         )
-        # pyre-fixme[16]: Optional type has no attribute `decomposition`.
-        self.assertDictEqual(m2.model.decomposition, {"1": [0, 2], "2": [1, 3]})
+        self.assertDictEqual(
+            cast(LCEAGP, m2.model).decomposition, {"1": [0, 2], "2": [1, 3]}
+        )
 
         # test decomposition validation in get_and_fit_model
         # the feature_names is not passed
         with self.assertRaises(ValueError):
             m2.fit(
                 datasets=[dataset],
                 metric_names=["y"],
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_discrete.py` & `ax-platform-0.3.2/ax/models/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_eb_thompson.py` & `ax-platform-0.3.2/ax/models/tests/test_eb_thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_full_factorial.py` & `ax-platform-0.3.2/ax/models/tests/test_full_factorial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_fully_bayesian.py` & `ax-platform-0.3.2/ax/models/tests/test_fully_bayesian.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import dataclasses
 import warnings
 from abc import ABC
 from contextlib import ExitStack
 from itertools import product
 from logging import Logger
 from math import sqrt
-from typing import Any, Dict, Type
+from typing import Any, cast, Dict, Type
 from unittest import mock
 
 import pyro
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.exceptions.core import AxError
 from ax.models.torch.fully_bayesian import (
@@ -29,18 +29,22 @@
 from ax.utils.common.constants import Keys
 from ax.utils.common.logger import get_logger
 from ax.utils.common.testutils import TestCase
 from ax.utils.testing.torch_stubs import get_torch_test_data
 from botorch.acquisition.utils import get_infeasible_cost
 from botorch.models import ModelListGP
 from botorch.models.gp_regression import MIN_INFERRED_NOISE_LEVEL
+from botorch.models.model import ModelList
 from botorch.models.transforms.input import Warp
 from botorch.optim.optimize import optimize_acqf
+from botorch.posteriors.gpytorch import GPyTorchPosterior
 from botorch.utils import get_objective_weights_transform
 from botorch.utils.datasets import FixedNoiseDataset
+from gpytorch.constraints import GreaterThan, Positive
+from gpytorch.kernels import MaternKernel, RBFKernel, ScaleKernel
 from gpytorch.likelihoods import _GaussianLikelihoodBase
 from pyro.infer.mcmc import MCMC, NUTS
 from pyro.ops.integrator import potential_grad
 
 
 RUN_INFERENCE_PATH = "ax.models.torch.fully_bayesian.run_inference"
 NUTS_PATH = "pyro.infer.mcmc.NUTS"
@@ -164,15 +168,47 @@
                     search_space_digest=SearchSpaceDigest(
                         feature_names=fns,
                         bounds=bounds,
                         task_features=tfs,
                     ),
                     metric_names=["y1", "y2"],
                 )
-                # pyre-fixme[16]: `BaseFullyBayesianBotorchModelTest` has no
+
+                # Check that there are no unexpected constraints on the hyperparameters
+                for _, m in enumerate(cast(ModelList, model.model).models):
+                    if inferred_noise:
+                        noise_covar = m.likelihood.noise_covar
+                        self.assertEqual(  # pyre-fixme[16]
+                            noise_covar.raw_noise_constraint.__class__, GreaterThan
+                        )
+                        self.assertTrue(
+                            torch.allclose(
+                                noise_covar.raw_noise_constraint.lower_bound,
+                                torch.tensor(1e-4, dtype=dtype),
+                            )
+                        )
+                    else:
+                        self.assertFalse(  # pyre-fixme[16]
+                            hasattr(m.likelihood.noise_covar, "raw_noise_constraint")
+                        )
+
+                    self.assertEqual(m.covar_module.__class__, ScaleKernel)
+                    self.assertEqual(
+                        m.covar_module.raw_outputscale_constraint.__class__, Positive
+                    )
+                    self.assertEqual(
+                        m.covar_module.base_kernel.__class__,
+                        RBFKernel if gp_kernel == "rbf" else MaternKernel,
+                    )
+                    self.assertEqual(m.covar_module.base_kernel.ard_num_dims, 3)
+                    self.assertEqual(
+                        m.covar_module.base_kernel.raw_lengthscale_constraint.__class__,
+                        Positive,
+                    )
+
                 #  attribute `assertEqual`.
                 self.assertEqual(_mock_fit_model.call_count, 2)
                 for i, call in enumerate(_mock_fit_model.call_args_list):
                     _, ckwargs = call
                     X = Xs[i]
                     Y = Ys[i]
                     Yvar = Yvars[i]
@@ -186,14 +222,15 @@
                         self.assertTrue(torch.isnan(ckwargs["Yvar"]).all())
                     else:
                         self.assertTrue(torch.equal(ckwargs["Yvar"], Yvar))
                     self.assertEqual(ckwargs["num_samples"], 4)
                     self.assertEqual(ckwargs["warmup_steps"], 512)
                     self.assertEqual(ckwargs["max_tree_depth"], 1)
                     self.assertTrue(ckwargs["disable_progbar"])
+                    self.assertFalse(ckwargs["jit_compile"])
                     self.assertEqual(ckwargs["use_input_warping"], use_input_warping)
                     self.assertEqual(ckwargs["gp_kernel"], gp_kernel)
                     self.assertTrue(ckwargs["verbose"])
 
                     # Check attributes
                     self.assertTrue(torch.equal(model.Xs[i], Xs[i]))
                     self.assertEqual(model.dtype, Xs[i].dtype)
@@ -201,16 +238,15 @@
                     # pyre-fixme[16]: `BaseFullyBayesianBotorchModelTest` has no
                     #  attribute `assertIsInstance`.
                     self.assertIsInstance(model.model, ModelListGP)
 
                     # Check fitting
                     # Note each model in the model list is a batched model, where
                     # the batch dim corresponds to the MCMC samples
-                    # pyre-fixme[16]: Optional type has no attribute `models`.
-                    model_list = model.model.models
+                    model_list = cast(ModelList, model.model).models
                     # Put model in `eval` mode to transform the train inputs.
                     m = model_list[i].eval()
                     # check mcmc samples
                     # pyre-fixme[6]: For 1st param expected `str` but got `int`.
                     dummy_samples = dummy_samples_list[i]
                     expected_train_inputs = Xs[i].expand(4, *Xs[i].shape)
                     if use_input_warping:
@@ -300,16 +336,14 @@
                                 #  `Union[None, List[typing.Any], int, slice,
                                 #  Tensor, typing.Tuple[typing.Any, ...]]` but got
                                 #  `str`.
                                 dummy_samples_list[i]["c1"],
                             )
                         )
                     else:
-                        # pyre-fixme[16]: `BaseFullyBayesianBotorchModelTest`
-                        #  has no attribute `assertFalse`.
                         self.assertFalse(hasattr(m, "input_transform"))
             # test that multi-task is not implemented
             (
                 Xs_mt,
                 Ys_mt,
                 Yvars_mt,
                 bounds_mt,
@@ -380,16 +414,17 @@
                         feature_names=fns,
                         bounds=bounds,
                         task_features=tfs,
                     ),
                 )
 
             # Check the hyperparameters and shapes
-            self.assertEqual(len(model.model.models), 2)
-            m1, m2 = model.model.models[0], model.model.models[1]
+            models = cast(ModelList, model.model).models
+            self.assertEqual(len(models), 2)
+            m1, m2 = models
             # Mean
             self.assertEqual(m1.mean_module.constant.shape, (4,))
             self.assertFalse(
                 torch.isclose(m1.mean_module.constant, m2.mean_module.constant).any()
             )
             # Outputscales
             self.assertEqual(m1.covar_module.outputscale.shape, (4,))
@@ -410,28 +445,25 @@
             # Check infeasible cost can be computed on the model
             device = torch.device("cuda") if cuda else torch.device("cpu")
             objective_weights = torch.tensor([1.0, 0.0], dtype=dtype, device=device)
             objective_transform = get_objective_weights_transform(objective_weights)
             infeasible_cost = (
                 get_infeasible_cost(
                     X=Xs1[0],
-                    # pyre-fixme[6]: For 2nd param expected `Model` but got
-                    #  `Optional[Model]`.
                     model=model.model,
                     objective=objective_transform,
                 )
                 .detach()
                 .clone()
             )
+            posterior = cast(GPyTorchPosterior, model.model.posterior(Xs1[0]))
             expected_infeasible_cost = -1 * torch.min(
                 # pyre-fixme[20]: Argument `1` expected.
                 objective_transform(
-                    # pyre-fixme[16]: Optional type has no attribute `posterior`.
-                    model.model.posterior(Xs1[0]).mean
-                    - 6 * model.model.posterior(Xs1[0]).variance.sqrt()
+                    posterior.mean - 6 * posterior.variance.sqrt()
                 ).min(),
                 torch.tensor(0.0, dtype=dtype, device=device),
             )
             self.assertTrue(
                 torch.abs(infeasible_cost - expected_infeasible_cost) < 1e-5
             )
 
@@ -804,27 +836,28 @@
                 # pyre-fixme[16]: `BaseFullyBayesianBotorchModelTest` has no
                 #  attribute `assertEqual`.
                 self.assertEqual(_mock_fit_model.call_count, 2)
                 _, ckwargs = _mock_fit_model.call_args
                 # pyre-fixme[16]: `BaseFullyBayesianBotorchModelTest` has no
                 #  attribute `assertIs`.
                 self.assertIs(ckwargs["pyro_model"], single_task_pyro_model)
-
+                self.assertFalse(ckwargs["jit_compile"])  # pyre-fixme[16]
                 # pyre-fixme[16]: `BaseFullyBayesianBotorchModelTest` has no
                 #  attribute `assertTrue`.
                 self.assertTrue(torch.equal(ckwargs["X"], Xs1[0]))
                 self.assertTrue(torch.equal(ckwargs["Y"], Ys1[0]))
                 if inferred_noise:
                     self.assertTrue(torch.isnan(ckwargs["Yvar"]).all())
                 else:
                     self.assertTrue(torch.equal(ckwargs["Yvar"], Yvars1[0]))
                 self.assertEqual(ckwargs["num_samples"], 4)
                 self.assertEqual(ckwargs["warmup_steps"], 0)
                 self.assertEqual(ckwargs["max_tree_depth"], 1)
                 self.assertTrue(ckwargs["disable_progbar"])
+                self.assertFalse(ckwargs["jit_compile"])
                 self.assertEqual(ckwargs["use_input_warping"], use_input_warping)
                 self.assertEqual(ckwargs["gp_kernel"], gp_kernel)
                 self.assertTrue(ckwargs["verbose"])
 
             with ExitStack() as es:
                 _mock_mcmc = es.enter_context(mock.patch(MCMC_PATH))
                 _mock_mcmc.return_value.get_samples.side_effect = dummy_samples
@@ -869,16 +902,15 @@
                         feature_names=fns,
                         bounds=bounds,
                         task_features=tfs,
                     ),
                 )
 
                 for m, X, Y, Yvar in zip(
-                    # pyre-fixme[16]: Optional type has no attribute `models`.
-                    model.model.models,
+                    cast(ModelList, model.model).models,
                     Xs1 + Xs2,
                     Ys1 + Ys2,
                     Yvars1 + Yvars2,
                 ):
                     self.assertTrue(
                         torch.equal(
                             m.train_inputs[0],
@@ -921,16 +953,14 @@
                             torch.Size([4, 1, 3]),
                         )
                         self.assertEqual(
                             m.input_transform.concentration1.shape,
                             torch.Size([4, 1, 3]),
                         )
                     else:
-                        # pyre-fixme[16]: `BaseFullyBayesianBotorchModelTest`
-                        #  has no attribute `assertFalse`.
                         self.assertFalse(hasattr(m, "input_transform"))
 
     def test_FullyBayesianBotorchModelPyro_float(self) -> None:
         self.test_FullyBayesianBotorchModelPyro(dtype=torch.float, cuda=False)
 
     def test_FullyBayesianBotorchModelPyro_cuda_double(self) -> None:
         if torch.cuda.is_available():
@@ -981,16 +1011,15 @@
                     ),
                 )
                 _mock_fit_model.assert_called_once()
             X = torch.rand(2, 3, dtype=torch.float)
             f_mean, f_cov = model.predict(X)
             self.assertTrue(f_mean.shape == torch.Size([2, 1]))
             self.assertTrue(f_cov.shape == torch.Size([2, 1, 1]))
-            # pyre-fixme[16]: Optional type has no attribute `models`.
-            model_list = model.model.models
+            model_list = cast(ModelList, model.model).models
             self.assertTrue(len(model_list) == 1)
             if use_input_warping:
                 self.assertTrue(hasattr(model_list[0], "input_transform"))
                 self.assertIsInstance(model_list[0].input_transform, Warp)
             else:
                 self.assertFalse(hasattr(model_list[0], "input_transform"))
```

### Comparing `ax-platform-0.3.1/ax/models/tests/test_model_utils.py` & `ax-platform-0.3.2/ax/models/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_posterior_mean.py` & `ax-platform-0.3.2/ax/models/tests/test_posterior_mean.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_random.py` & `ax-platform-0.3.2/ax/models/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_randomforest.py` & `ax-platform-0.3.2/ax/models/tests/test_randomforest.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_rembo.py` & `ax-platform-0.3.2/ax/models/tests/test_rembo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_rembo_initializer.py` & `ax-platform-0.3.2/ax/models/tests/test_rembo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_sobol.py` & `ax-platform-0.3.2/ax/models/tests/test_sobol.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_thompson.py` & `ax-platform-0.3.2/ax/models/tests/test_thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_torch.py` & `ax-platform-0.3.2/ax/models/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_torch_model_utils.py` & `ax-platform-0.3.2/ax/models/tests/test_torch_model_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_torch_utils.py` & `ax-platform-0.3.2/ax/models/tests/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/tests/test_uniform.py` & `ax-platform-0.3.2/ax/models/tests/test_uniform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/alebo.py` & `ax-platform-0.3.2/ax/models/torch/alebo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch.py` & `ax-platform-0.3.2/ax/models/torch/botorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from copy import deepcopy
 
 from logging import Logger
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.core.types import TCandidateMetadata
 from ax.exceptions.core import DataRequiredError
 from ax.models.torch.botorch_defaults import (
@@ -31,20 +31,22 @@
     subset_model,
 )
 from ax.models.torch_base import TorchGenResults, TorchModel, TorchOptConfig
 from ax.models.types import TConfig
 from ax.utils.common.constants import Keys
 from ax.utils.common.docutils import copy_doc
 from ax.utils.common.logger import get_logger
-from ax.utils.common.typeutils import checked_cast, not_none
+from ax.utils.common.typeutils import checked_cast
 from botorch.acquisition.acquisition import AcquisitionFunction
+from botorch.models import ModelList
 from botorch.models.model import Model
-from botorch.models.model_list_gp_regression import ModelListGP
 from botorch.utils.datasets import SupervisedDataset
+from botorch.utils.transforms import is_fully_bayesian
 from torch import Tensor
+from torch.nn import ModuleList  # @manual
 
 logger: Logger = get_logger(__name__)
 
 
 # pyre-fixme[33]: Aliased annotation cannot contain `Any`.
 TModelConstructor = Callable[
     [
@@ -240,15 +242,16 @@
     """
 
     dtype: Optional[torch.dtype]
     device: Optional[torch.device]
     Xs: List[Tensor]
     Ys: List[Tensor]
     Yvars: List[Tensor]
-    model: Optional[Model]
+    _model: Optional[Model]
+    _search_space_digest: Optional[SearchSpaceDigest] = None
 
     def __init__(
         self,
         model_constructor: TModelConstructor = get_and_fit_model,
         model_predictor: TModelPredictor = predict_from_model,
         # pyre-fixme[9]: acqf_constructor has type `Callable[[Model, Tensor,
         #  Optional[Tuple[Tensor, Tensor]], Optional[Tensor], Optional[Tensor], Any],
@@ -276,15 +279,15 @@
         self._kwargs = kwargs
         self.refit_on_cv = refit_on_cv
         self.refit_on_update = refit_on_update
         self.warm_start_refitting = warm_start_refitting
         self.use_input_warping = use_input_warping
         self.use_loocv_pseudo_likelihood = use_loocv_pseudo_likelihood
         self.prior = prior
-        self.model: Optional[Model] = None
+        self._model: Optional[Model] = None
         self.Xs = []
         self.Ys = []
         self.Yvars = []
         self.dtype = None
         self.device = None
         self.task_features: List[int] = []
         self.fidelity_features: List[int] = []
@@ -296,26 +299,27 @@
         datasets: List[SupervisedDataset],
         metric_names: List[str],
         search_space_digest: SearchSpaceDigest,
         candidate_metadata: Optional[List[List[TCandidateMetadata]]] = None,
     ) -> None:
         if len(datasets) == 0:
             raise DataRequiredError("BotorchModel.fit requires non-empty data sets.")
-        Xs, Ys, Yvars = _datasets_to_legacy_inputs(datasets=datasets)
+        self.Xs, self.Ys, self.Yvars = _datasets_to_legacy_inputs(datasets=datasets)
         self.metric_names = metric_names
-        self.Xs, self.Ys, self.Yvars = Xs, Ys, Yvars
+        # Store search space info for later use (e.g. during generation)
+        self._search_space_digest = search_space_digest
         self.dtype = self.Xs[0].dtype
         self.device = self.Xs[0].device
         self.task_features = normalize_indices(
             search_space_digest.task_features, d=self.Xs[0].size(-1)
         )
         self.fidelity_features = normalize_indices(
             search_space_digest.fidelity_features, d=self.Xs[0].size(-1)
         )
-        self.model = self.model_constructor(  # pyre-ignore [28]
+        self._model = self.model_constructor(  # pyre-ignore [28]
             Xs=self.Xs,
             Ys=self.Ys,
             Yvars=self.Yvars,
             task_features=self.task_features,
             fidelity_features=self.fidelity_features,
             metric_names=self.metric_names,
             use_input_warping=self.use_input_warping,
@@ -352,15 +356,15 @@
             linear_constraints=torch_opt_config.linear_constraints,
             fixed_features=torch_opt_config.fixed_features,
         )
         model = self.model
         # subset model only to the outcomes we need for the optimization	357
         if options.get(Keys.SUBSET_MODEL, True):
             subset_model_results = subset_model(
-                model=model,  # pyre-ignore [6]
+                model=model,
                 objective_weights=torch_opt_config.objective_weights,
                 outcome_constraints=torch_opt_config.outcome_constraints,
             )
             model = subset_model_results.model
             objective_weights = subset_model_results.objective_weights
             outcome_constraints = subset_model_results.outcome_constraints
         else:
@@ -460,16 +464,16 @@
     @copy_doc(TorchModel.cross_validate)
     def cross_validate(  # pyre-ignore [14]: `search_space_digest` arg not needed here
         self,
         datasets: List[SupervisedDataset],
         X_test: Tensor,
         **kwargs: Any,
     ) -> Tuple[Tensor, Tensor]:
-        if self.model is None:
-            raise RuntimeError("Cannot cross-validate model that has not been fitted")
+        if self._model is None:
+            raise RuntimeError("Cannot cross-validate model that has not been fitted.")
         if self.refit_on_cv:
             state_dict = None
         else:
             state_dict = deepcopy(self.model.state_dict())
         Xs, Ys, Yvars = _datasets_to_legacy_inputs(datasets=datasets)
         model = self.model_constructor(  # pyre-ignore: [28]
             Xs=Xs,
@@ -489,57 +493,64 @@
     @copy_doc(TorchModel.update)
     def update(  # pyre-ignore [14]: `search_space_digest` arg not needed here
         self,
         datasets: List[SupervisedDataset],
         candidate_metadata: Optional[List[List[TCandidateMetadata]]] = None,
         **kwargs: Any,
     ) -> None:
-        if self.model is None:
-            raise RuntimeError("Cannot update model that has not been fitted")
+        if self._model is None:
+            raise RuntimeError("Cannot update model that has not been fitted.")
         Xs, Ys, Yvars = _datasets_to_legacy_inputs(datasets=datasets)
         self.Xs = Xs
         self.Ys = Ys
         self.Yvars = Yvars
         if self.refit_on_update and not self.warm_start_refitting:
             state_dict = None  # pragma: no cover
         else:
-            state_dict = deepcopy(not_none(self.model).state_dict())
-        self.model = self.model_constructor(  # pyre-ignore: [28]
+            state_dict = deepcopy(self.model.state_dict())
+        self._model = self.model_constructor(  # pyre-ignore: [28]
             Xs=self.Xs,
             Ys=self.Ys,
             Yvars=self.Yvars,
             task_features=self.task_features,
             state_dict=state_dict,
             fidelity_features=self.fidelity_features,
             metric_names=self.metric_names,
             refit_model=self.refit_on_update,
             use_input_warping=self.use_input_warping,
             use_loocv_pseudo_likelihood=self.use_loocv_pseudo_likelihood,
             **self._kwargs,
         )
 
     def feature_importances(self) -> np.ndarray:
-        if self.model is None:
+        return get_feature_importances_from_botorch_model(model=self._model)
+
+    @property
+    def search_space_digest(self) -> SearchSpaceDigest:
+        if self._search_space_digest is None:
             raise RuntimeError(
-                "Cannot calculate feature_importances without a fitted model"
+                "`search_space_digest` is not initialized. Please fit the model first."
             )
-        elif isinstance(self.model, ModelListGP):
-            models = self.model.models
-        else:
-            models = [self.model]
-        lengthscales = []
-        for m in models:
-            ls = m.covar_module.base_kernel.lengthscale
-            if ls.ndim == 2:
-                ls = ls.unsqueeze(0)
-            lengthscales.append(ls)
-        lengthscales = torch.cat(lengthscales, dim=0)
-        # pyre-fixme[16]: `float` has no attribute `detach`.
-        # pyre-fixme[58]: `/` is not supported for operand types `int` and `Tensor`.
-        return (1 / lengthscales).detach().cpu().numpy()
+        return self._search_space_digest
+
+    @search_space_digest.setter
+    def search_space_digest(self, value: SearchSpaceDigest) -> None:
+        raise RuntimeError("Setting search_space_digest manually is disallowed.")
+
+    @property
+    def model(self) -> Model:
+        if self._model is None:
+            raise RuntimeError(
+                "`model` is not initialized. Please fit the model first."
+            )
+        return self._model
+
+    @model.setter
+    def model(self, model: Model) -> None:
+        self._model = model  # there are a few places that set model directly
 
 
 def get_rounding_func(
     rounding_func: Optional[Callable[[Tensor], Tensor]]
 ) -> Optional[Callable[[Tensor], Tensor]]:
     if rounding_func is None:
         botorch_rounding_func = rounding_func
@@ -549,7 +560,52 @@
             batch_shape, d = X.shape[:-1], X.shape[-1]
             X_round = torch.stack(
                 [rounding_func(x) for x in X.view(-1, d)]  # pyre-ignore: [16]
             )
             return X_round.view(*batch_shape, d)
 
     return botorch_rounding_func
+
+
+def get_feature_importances_from_botorch_model(
+    model: Union[Model, ModuleList, None],
+) -> np.ndarray:
+    """Get feature importances from a list of BoTorch models.
+
+    Args:
+        models: BoTorch model to get feature importances from.
+
+    Returns:
+        The feature importances as a numpy array where each row sums to 1.
+    """
+    if model is None:
+        raise RuntimeError(
+            "Cannot calculate feature_importances without a fitted model."
+            "Call `fit` first."
+        )
+    elif isinstance(model, ModelList):
+        models = model.models
+    else:
+        models = [model]
+    lengthscales = []
+    for m in models:
+        try:
+            ls = m.covar_module.base_kernel.lengthscale
+        except AttributeError:
+            ls = None
+        if ls is None or ls.shape[-1] != m.train_inputs[0].shape[-1]:
+            # TODO: We could potentially set the feature importances to NaN in this
+            # case, but this require knowing the batch dimension of this model.
+            # Consider supporting in the future.
+            raise NotImplementedError(
+                "Failed to extract lengthscales from `m.covar_module.base_kernel`"
+            )
+        if ls.ndim == 2:
+            ls = ls.unsqueeze(0)
+        if is_fully_bayesian(m):  # Take the median over the MCMC samples
+            ls = torch.quantile(ls, q=0.5, dim=0, keepdim=True)
+        lengthscales.append(ls)
+    lengthscales = torch.cat(lengthscales, dim=0)
+    feature_importances = (1 / lengthscales).detach().cpu()  # pyre-ignore
+    # Make sure the sum of feature importances is 1.0 for each metric
+    feature_importances /= feature_importances.sum(dim=-1, keepdim=True)
+    return feature_importances.numpy()
```

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_defaults.py` & `ax-platform-0.3.2/ax/models/torch/botorch_defaults.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_kg.py` & `ax-platform-0.3.2/ax/models/torch/botorch_kg.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_mes.py` & `ax-platform-0.3.2/ax/models/torch/botorch_mes.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         )
 
         model = self.model
 
         # subset model only to the outcomes we need for the optimization
         if options.get("subset_model", True):
             subset_model_results = subset_model(
-                model=model,  # pyre-ignore [6]
+                model=model,
                 objective_weights=torch_opt_config.objective_weights,
                 outcome_constraints=torch_opt_config.outcome_constraints,
             )
             model = subset_model_results.model
             objective_weights = subset_model_results.objective_weights
         else:
             objective_weights = torch_opt_config.objective_weights
@@ -127,15 +127,15 @@
         )
         bounds_ = bounds_.transpose(0, 1)
 
         candidate_set = torch.rand(candidate_size, bounds_.size(1))
         candidate_set = bounds_[0] + (bounds_[1] - bounds_[0]) * candidate_set
 
         acq_function = _instantiate_MES(
-            model=model,  # pyre-ignore [6]
+            model=model,
             candidate_set=candidate_set,
             num_fantasies=num_fantasies,
             num_trace_observations=options.get("num_trace_observations", 0),
             num_mv_samples=num_mv_samples,
             num_y_samples=num_y_samples,
             X_pending=X_pending,
             maximize=True if objective_weights[0] == 1 else False,
```

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_modular/acquisition.py` & `ax-platform-0.3.2/ax/models/torch/botorch_modular/acquisition.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.exceptions.core import AxWarning, SearchSpaceExhausted
 from ax.models.model_utils import enumerate_discrete_combinations, mk_discrete_choices
 from ax.models.torch.botorch_modular.optimizer_argparse import optimizer_argparse
 from ax.models.torch.botorch_modular.surrogate import Surrogate
-from ax.models.torch.botorch_modular.utils import _tensor_difference
+from ax.models.torch.botorch_modular.utils import (
+    _tensor_difference,
+    get_post_processing_func,
+)
 from ax.models.torch.botorch_moo_defaults import infer_objective_thresholds
 from ax.models.torch.utils import (
     _get_X_pending_and_observed,
     get_botorch_objective_and_transform,
     subset_model,
 )
 from ax.models.torch_base import TorchOptConfig
@@ -378,48 +381,64 @@
                 properties, e.g. ``bounds`` for optimization.
             inequality_constraints: A list of tuples (indices, coefficients, rhs),
                 with each tuple encoding an inequality constraint of the form
                 ``sum_i (X[indices[i]] * coefficients[i]) >= rhs``.
             fixed_features: A map `{feature_index: value}` for features that
                 should be fixed to a particular value during generation.
             rounding_func: A function that post-processes an optimization
-                result appropriately (i.e., according to `round-trip`
-                transformations).
+                result appropriately. This is typically passed down from
+                `ModelBridge` to ensure compatibility of the candidates with
+                with Ax transforms. For additional post processing, use
+                `post_processing_func` option in `optimizer_options`.
             optimizer_options: Options for the optimizer function, e.g. ``sequential``
-                or ``raw_samples``.
+                or ``raw_samples``. This can also include a `post_processing_func`
+                which is applied to the candidates before the `rounding_func`.
+                `post_processing_func` can be used to support more customized options
+                that typically only exist in MBM, such as BoTorch transforms.
+                See the docstring of `TorchOptConfig` for more information on passing
+                down these options while constructing a generation strategy.
+
+        Returns:
+            A two-element tuple containing an `n x d`-dim tensor of generated candidates
+            and a tensor with the associated acquisition value.
         """
         # NOTE: Could make use of `optimizer_class` when it's added to BoTorch
         # instead of calling `optimizer_acqf` or `optimize_acqf_discrete` etc.
         _tensorize = partial(torch.tensor, dtype=self.dtype, device=self.device)
         ssd = search_space_digest
         bounds = _tensorize(ssd.bounds).t()
 
         # Prepare arguments for optimizer
         optimizer_options_with_defaults = optimizer_argparse(
             self.acqf,
             bounds=bounds,
             q=n,
             optimizer_options=optimizer_options,
         )
-
+        post_processing_func = get_post_processing_func(
+            rounding_func=rounding_func,
+            optimizer_options=optimizer_options_with_defaults,
+        )
         discrete_features = sorted(ssd.ordinal_features + ssd.categorical_features)
         if fixed_features is not None:
             for i in fixed_features:
                 if not 0 <= i < len(ssd.feature_names):
                     raise ValueError(f"Invalid fixed_feature index: {i}")
 
         # 1. Handle the fully continuous search space.
-        if not discrete_features:
+        if not discrete_features or optimizer_options_with_defaults.pop(
+            "force_use_optimize_acqf", False
+        ):
             return optimize_acqf(
                 acq_function=self.acqf,
                 bounds=bounds,
                 q=n,
                 inequality_constraints=inequality_constraints,
                 fixed_features=fixed_features,
-                post_processing_func=rounding_func,
+                post_processing_func=post_processing_func,
                 **optimizer_options_with_defaults,
             )
 
         # 2. Handle search spaces with discrete features.
         discrete_choices = mk_discrete_choices(ssd=ssd, fixed_features=fixed_features)
 
         # 2a. Handle the fully discrete search space.
@@ -501,15 +520,15 @@
             # For now we just enumerate all possible discrete combinations. This is not
             # scalable and and only works for a reasonably small number of choices. A
             # slowdown warning is logged in `enumerate_discrete_combinations` if needed.
             fixed_features_list=enumerate_discrete_combinations(
                 discrete_choices=discrete_choices
             ),
             inequality_constraints=inequality_constraints,
-            post_processing_func=rounding_func,
+            post_processing_func=post_processing_func,
             **optimizer_options_with_defaults,
         )
 
     def evaluate(self, X: Tensor) -> Tensor:
         """Evaluate the acquisition function on the candidate set `X`.
 
         Args:
```

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_modular/model.py` & `ax-platform-0.3.2/ax/models/torch/botorch_modular/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,36 @@
 
 import dataclasses
 from copy import deepcopy
 from dataclasses import dataclass, field
 from functools import wraps
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Type, TypeVar
 
+import numpy as np
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.core.types import TCandidateMetadata, TGenMetadata
 from ax.exceptions.core import UnsupportedError, UserInputError
-from ax.models.torch.botorch import get_rounding_func
+from ax.models.torch.botorch import (
+    get_feature_importances_from_botorch_model,
+    get_rounding_func,
+)
 from ax.models.torch.botorch_modular.acquisition import Acquisition
 from ax.models.torch.botorch_modular.surrogate import Surrogate
 from ax.models.torch.botorch_modular.utils import (
     choose_botorch_acqf_class,
     construct_acquisition_and_optimizer_options,
     convert_to_block_design,
 )
 from ax.models.torch.utils import _to_inequality_constraints
 from ax.models.torch_base import TorchGenResults, TorchModel, TorchOptConfig
 from ax.utils.common.base import Base
 from ax.utils.common.constants import Keys
 from ax.utils.common.docutils import copy_doc
-from ax.utils.common.typeutils import checked_cast, not_none
+from ax.utils.common.typeutils import checked_cast
 from botorch.acquisition.acquisition import AcquisitionFunction
 from botorch.models import ModelList
 from botorch.models.deterministic import FixedSingleSampleModel
 from botorch.models.model import Model
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
 from botorch.utils.datasets import SupervisedDataset
@@ -228,25 +232,26 @@
     @property
     def botorch_acqf_class(self) -> Type[AcquisitionFunction]:
         """BoTorch ``AcquisitionFunction`` class, associated with this model.
         Raises an error if one is not yet set.
         """
         if not self._botorch_acqf_class:
             raise ValueError("BoTorch `AcquisitionFunction` has not yet been set.")
-        return not_none(self._botorch_acqf_class)
+        return self._botorch_acqf_class
 
     def fit(
         self,
         datasets: List[SupervisedDataset],
         metric_names: List[str],
         search_space_digest: SearchSpaceDigest,
         candidate_metadata: Optional[List[List[TCandidateMetadata]]] = None,
         # state dict by surrogate label
         state_dicts: Optional[Mapping[str, Dict[str, Tensor]]] = None,
         refit: bool = True,
+        **kwargs: Any,
     ) -> None:
         """Fit model to m outcomes.
 
         Args:
             datasets: A list of ``SupervisedDataset`` containers, each
                 corresponding to the data of one metric (outcome).
             metric_names: A list of metric names, with the i-th metric
@@ -279,14 +284,15 @@
                 metric_names=metric_names,
                 search_space_digest=search_space_digest,
                 candidate_metadata=candidate_metadata,
                 state_dict=state_dicts.get(Keys.ONLY_SURROGATE)
                 if state_dicts
                 else None,
                 refit=refit,
+                **kwargs,
             )
             return
 
         # Step 1. Initialize a Surrogate for every SurrogateSpec
         self._surrogates = {
             label: Surrogate(
                 # if None, Surrogate will autoset class per outcome at construct time
@@ -350,23 +356,25 @@
             surrogate.fit(
                 datasets=subset_datasets,
                 metric_names=subset_metric_names,
                 search_space_digest=search_space_digest,
                 candidate_metadata=candidate_metadata,
                 state_dict=(state_dicts or {}).get(label),
                 refit=refit,
+                **kwargs,
             )
 
     @copy_doc(TorchModel.update)
     def update(
         self,
         datasets: List[Optional[SupervisedDataset]],
         metric_names: List[str],
         search_space_digest: SearchSpaceDigest,
         candidate_metadata: Optional[List[List[TCandidateMetadata]]] = None,
+        **kwargs: Any,
     ) -> None:
         if len(self.surrogates) == 0:
             raise UnsupportedError("Cannot update model that has not been fitted.")
 
         # store search space info  for later use (e.g. during generation)
         self._search_space_digest = search_space_digest
 
@@ -403,14 +411,15 @@
             surrogate.update(
                 datasets=subset_datasets,
                 metric_names=subset_metric_names,
                 search_space_digest=search_space_digest,
                 candidate_metadata=candidate_metadata,
                 state_dict=state_dict,
                 refit=self.refit_on_update,
+                **kwargs,
             )
 
     @single_surrogate_only
     def predict(self, X: Tensor) -> Tuple[Tensor, Tensor]:
         """Predict if only one Surrogate, Error if there are many"""
 
         return self.surrogate.predict(X=X)
@@ -424,28 +433,25 @@
     @copy_doc(TorchModel.gen)
     def gen(
         self,
         n: int,
         search_space_digest: SearchSpaceDigest,
         torch_opt_config: TorchOptConfig,
     ) -> TorchGenResults:
-        if self._search_space_digest is None:
-            raise RuntimeError("Must `fit` the model before calling `gen`.")
         acq_options, opt_options = construct_acquisition_and_optimizer_options(
             acqf_options=self.acquisition_options,
             model_gen_options=torch_opt_config.model_gen_options,
         )
         # update bounds / target fidelities
-        search_space_digest = not_none(
-            dataclasses.replace(
-                self._search_space_digest,
-                bounds=search_space_digest.bounds,
-                target_fidelities=search_space_digest.target_fidelities or {},
-            )
+        search_space_digest = dataclasses.replace(
+            self.search_space_digest,
+            bounds=search_space_digest.bounds,
+            target_fidelities=search_space_digest.target_fidelities or {},
         )
+
         acqf = self._instantiate_acquisition(
             search_space_digest=search_space_digest,
             torch_opt_config=torch_opt_config,
             acq_options=acq_options,
         )
         botorch_rounding_func = get_rounding_func(torch_opt_config.rounding_func)
         candidates, expected_acquisition_value = acqf.optimize(
@@ -524,14 +530,15 @@
     @copy_doc(TorchModel.cross_validate)
     def cross_validate(
         self,
         datasets: List[SupervisedDataset],
         metric_names: List[str],
         X_test: Tensor,
         search_space_digest: SearchSpaceDigest,
+        **kwargs: Any,
     ) -> Tuple[Tensor, Tensor]:
         # Will fail if metric_names exist across multiple models
         surrogate_labels = (
             [
                 label
                 for label, spec in self.surrogate_specs.items()
                 if any(metric in spec.outcomes for metric in metric_names)
@@ -576,14 +583,15 @@
         try:
             self.fit(
                 datasets=datasets,
                 metric_names=metric_names,
                 search_space_digest=search_space_digest,
                 state_dicts=state_dicts,
                 refit=self.refit_on_cv,
+                **kwargs,
             )
             X_test_prediction = self.predict_from_surrogate(
                 surrogate_label=surrogate_label, X=X_test
             )
         finally:
             # Reset the surrogates back to this model's surrogate, make
             # sure the cloned surrogate doesn't stay around if fit or
@@ -656,7 +664,43 @@
         return self.acquisition_class(
             surrogates=self.surrogates,
             botorch_acqf_class=self.botorch_acqf_class,
             search_space_digest=search_space_digest,
             torch_opt_config=torch_opt_config,
             options=acq_options,
         )
+
+    def feature_importances(self) -> np.ndarray:
+        """Compute feature importances from the model.
+
+        Caveat: This assumes the following:
+            1. There is a single surrogate model (potentially a `ModelList`).
+            2. We can get model lengthscales from `covar_module.base_kernel.lengthscale`
+
+        Returns:
+            The feature importances as a numpy array of size len(metrics) x 1 x dim
+            where each row sums to 1.
+        """
+        if list(self.surrogates.keys()) != [Keys.ONLY_SURROGATE]:
+            raise NotImplementedError("Only support a single surrogate model for now")
+        surrogate = self.surrogates[Keys.ONLY_SURROGATE]
+        return get_feature_importances_from_botorch_model(model=surrogate.model)
+
+    @property
+    def search_space_digest(self) -> SearchSpaceDigest:
+        if self._search_space_digest is None:
+            raise RuntimeError(
+                "`search_space_digest` is not initialized. Must `fit` the model first."
+            )
+        return self._search_space_digest
+
+    @search_space_digest.setter
+    def search_space_digest(self, value: SearchSpaceDigest) -> None:
+        raise RuntimeError("Setting search_space_digest manually is disallowed.")
+
+    @property
+    def outcomes_by_surrogate_label(self) -> Dict[str, List[str]]:
+        """Retuns a dictionary mapping from surrogate label to a list of outcomes."""
+        outcomes_by_surrogate_label = {}
+        for k, v in self.surrogates.items():
+            outcomes_by_surrogate_label[k] = v.outcomes
+        return outcomes_by_surrogate_label
```

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_modular/multi_fidelity.py` & `ax-platform-0.3.2/ax/models/torch/botorch_modular/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_modular/optimizer_argparse.py` & `ax-platform-0.3.2/ax/models/torch/botorch_modular/optimizer_argparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     name="optimizer_argparse", encoder=_optimizerArgparse_encoder
 )
 
 
 @optimizer_argparse.register(AcquisitionFunction)
 def _argparse_base(
     acqf: MaybeType[AcquisitionFunction],
-    num_restarts: int = 40,
+    sequential: bool = True,
+    num_restarts: int = 20,
     raw_samples: int = 1024,
     init_batch_limit: int = 32,
     batch_limit: int = 5,
     optimizer_options: Optional[Dict[str, Any]] = None,
     optimizer_is_discrete: bool = False,
     **ignore: Any,
 ) -> Dict[str, Any]:
@@ -60,14 +61,15 @@
     NOTE: Since `optimizer_options` is how the user would typically pass in these
     options, it takes precedence over other arguments. E.g., if both `num_restarts`
     and `optimizer_options["num_restarts"]` are provided, this will use
     `num_restarts` from `optimizer_options`.
 
     Args:
         acqf: The acquisition function being optimized.
+        sequential: Whether we choose one candidate at a time in a sequential manner.
         num_restarts: The number of starting points for multistart acquisition
             function optimization.
         raw_samples: The number of samples for initialization.
         init_batch_limit: The size of mini-batches used to evaluate the `raw_samples`.
             This helps reduce peak memory usage.
         batch_limit: The size of mini-batches used while optimizing the `acqf`.
             This helps reduce peak memory usage.
@@ -87,14 +89,15 @@
         optimizer_is_discrete: True if the optimizer is `optimizer_acqf_discrete`,
             which supports a limited set of arguments.
     """
     optimizer_options = optimizer_options or {}
     if optimizer_is_discrete:
         return optimizer_options
     return {
+        "sequential": sequential,
         "num_restarts": num_restarts,
         "raw_samples": raw_samples,
         "options": {
             "init_batch_limit": init_batch_limit,
             "batch_limit": batch_limit,
             **optimizer_options.get("options", {}),
         },
@@ -124,15 +127,15 @@
 
 
 @optimizer_argparse.register(qKnowledgeGradient)
 def _argparse_kg(
     acqf: qKnowledgeGradient,
     q: int,
     bounds: torch.Tensor,
-    num_restarts: int = 40,
+    num_restarts: int = 20,
     raw_samples: int = 1024,
     frac_random: float = 0.1,
     optimizer_options: Optional[Dict[str, Any]] = None,
     **kwargs: Any,
 ) -> Dict[str, Any]:
 
     optimizer_options = optimizer_options or {}
```

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_modular/surrogate.py` & `ax-platform-0.3.2/ax/models/torch/botorch_modular/surrogate.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,21 +143,21 @@
     @property
     def model(self) -> Model:
         if self._model is None:
             raise ValueError(
                 "BoTorch `Model` has not yet been constructed, please fit the "
                 "surrogate first (done via `BoTorchModel.fit`)."
             )
-        return not_none(self._model)
+        return self._model
 
     @property
     def training_data(self) -> List[SupervisedDataset]:
         if self._training_data is None:
             raise ValueError(NOT_YET_FIT_MSG)
-        return not_none(self._training_data)
+        return self._training_data
 
     @property
     def Xs(self) -> List[Tensor]:
         # Handles multi-output models. TODO: Improve this!
         training_data = self.training_data
         Xs = []
         for dataset in training_data:
@@ -347,18 +347,20 @@
                 ``ModelListGP``.
             search_space_digest: SearchSpaceDigest must be provided if no
                 botorch_submodel_class is provided so the appropriate botorch model
                 class can be automatically selected.
 
             **kwargs: Keyword arguments, accepts:
                 - ``fidelity_features``: Indices of columns in X that represent
-                    fidelity
-                - ``task_features``: Indices of columns in X that represent tasks
+                    fidelity features.
+                - ``task_features``: Indices of columns in X that represent tasks.
+                - ``categorical_features``: Indices of columns in X that represent
+                    categorical features.
                 - ``robust_digest``: An optional `RobustSearchSpaceDigest` that carries
-                    additional attributes if using a `RobustSearchSpace`
+                    additional attributes if using a `RobustSearchSpace`.
         """
         if self.botorch_model_class is None and search_space_digest is None:
             raise UserInputError(
                 "Must either provide `botorch_submodel_class` or "
                 "`search_space_digest` so an appropriate submodel class can be "
                 "chosen."
             )
@@ -385,34 +387,35 @@
                 logger.warning(f"Metric {m} not in training data.")
                 continue
 
             formatted_model_inputs = model_cls.construct_inputs(
                 training_data=dataset,
                 fidelity_features=fidelity_features,
                 task_feature=task_feature,
+                categorical_features=kwargs.get("categorical_features", None),
                 **self.model_options,
             )
             # Add input / outcome transforms.
             # TODO: The use of `inspect` here is not ideal. We should find a better
             # way to filter the arguments. See the comment in `Surrogate.construct`
             # regarding potential use of a `ModelFactory` in the future.
             model_cls_args = inspect.getfullargspec(model_cls).args
             self._set_formatted_inputs(
                 formatted_model_inputs=formatted_model_inputs,
                 inputs=[
                     [
                         "covar_module",
                         self.covar_module_class,
-                        self.covar_module_options,
+                        deepcopy(self.covar_module_options),
                         None,
                     ],
                     [
                         "likelihood",
                         self.likelihood_class,
-                        self.likelihood_options,
+                        deepcopy(self.likelihood_options),
                         None,
                     ],
                     [
                         "outcome_transform",
                         None,
                         None,
                         deepcopy(self.outcome_transform),
@@ -491,14 +494,15 @@
         datasets: List[SupervisedDataset],
         metric_names: List[str],
         search_space_digest: SearchSpaceDigest,
         candidate_metadata: Optional[List[List[TCandidateMetadata]]] = None,
         state_dict: Optional[Dict[str, Tensor]] = None,
         refit: bool = True,
         original_metric_names: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> None:
         """Fits the underlying BoTorch ``Model`` to ``m`` outcomes.
 
         NOTE: ``state_dict`` and ``refit`` keyword arguments control how the
         undelying BoTorch ``Model`` will be fit: whether its parameters will
         be reoptimized and whether it will be warm-started from a given state.
 
@@ -536,19 +540,21 @@
         if self._constructed_manually:
             logger.debug(
                 "For manually constructed surrogates (via `Surrogate.from_botorch`), "
                 "`fit` skips setting the training data on model and only reoptimizes "
                 "its parameters if `refit=True`."
             )
         else:
+            _kwargs = dataclasses.asdict(search_space_digest)
+            _kwargs.update(kwargs)
             self.construct(
                 datasets=datasets,
                 metric_names=metric_names,
                 search_space_digest=search_space_digest,
-                **dataclasses.asdict(search_space_digest),
+                **_kwargs,
             )
             self._outcomes = (
                 original_metric_names
                 if original_metric_names is not None
                 else metric_names
             )
         if state_dict:
@@ -658,14 +664,15 @@
         self,
         datasets: List[SupervisedDataset],
         metric_names: List[str],
         search_space_digest: SearchSpaceDigest,
         candidate_metadata: Optional[List[List[TCandidateMetadata]]] = None,
         state_dict: Optional[Dict[str, Tensor]] = None,
         refit: bool = True,
+        **kwargs: Any,
     ) -> None:
         """Updates the surrogate model with new data. In the base ``Surrogate``,
         just calls ``fit`` after checking that this surrogate was not created
         via ``Surrogate.from_botorch`` (in which case the ``Model`` comes premade,
         constructed manually and then supplied to ``Surrogate``).
 
         NOTE: Expects `training_data` to be all available data,
@@ -695,14 +702,15 @@
         self.fit(
             datasets=datasets,
             metric_names=metric_names,
             search_space_digest=search_space_digest,
             candidate_metadata=candidate_metadata,
             state_dict=state_dict,
             refit=refit,
+            **kwargs,
         )
 
     def pareto_frontier(self) -> Tuple[Tensor, Tensor]:
         """For multi-objective optimization, retrieve Pareto frontier instead
         of best point.
 
         Returns: A two-tuple of:
@@ -787,7 +795,17 @@
                     "in robust optimization."
                 )
             submodel_input_transforms = perturbation
         else:
             submodel_input_transforms = self.input_transform
 
         return list(fidelity_features), task_feature, submodel_input_transforms
+
+    @property
+    def outcomes(self) -> List[str]:
+        if self._outcomes is None:
+            raise RuntimeError("outcomes not initialized. Please call `fit` first.")
+        return self._outcomes
+
+    @outcomes.setter
+    def outcomes(self, value: List[str]) -> None:
+        raise RuntimeError("Setting outcomes manually is disallowed.")
```

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_modular/utils.py` & `ax-platform-0.3.2/ax/models/torch/botorch_modular/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import warnings
 from contextlib import contextmanager
 from logging import Logger
-from typing import Any, Dict, Generator, List, Optional, Tuple, Type
+from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Type
 
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.exceptions.core import AxWarning, UnsupportedError
 from ax.models.types import TConfig
 from ax.utils.common.constants import Keys
 from ax.utils.common.logger import get_logger
@@ -324,7 +324,39 @@
     C = torch.cat((A, B), dim=0)
     D, inverse_ind = torch.unique(C, return_inverse=True, dim=0)
     n = A.shape[0]
     A_indices = inverse_ind[:n].tolist()
     B_indices = inverse_ind[n:].tolist()
     Bi_set = set(B_indices) - set(A_indices)
     return D[list(Bi_set)]
+
+
+def get_post_processing_func(
+    rounding_func: Optional[Callable[[Tensor], Tensor]],
+    optimizer_options: Dict[str, Any],
+) -> Optional[Callable[[Tensor], Tensor]]:
+    """Get the post processing function by combining the rounding function
+    with the post processing function provided as part of the optimizer
+    options. If both are given, the post processing function is applied before
+    applying the rounding function. If only one of them is given, then
+    it is used as the post processing function.
+    """
+    if "post_processing_func" in optimizer_options:
+        provided_func: Callable[[Tensor], Tensor] = optimizer_options.pop(
+            "post_processing_func"
+        )
+        if rounding_func is None:
+            # No rounding function is given. We can use the post processing
+            # function directly.
+            return provided_func
+        else:
+            # Both post processing and rounding functions are given. We need
+            # to chain them and apply the post processing function first.
+            base_rounding_func: Callable[[Tensor], Tensor] = rounding_func
+
+            def combined_func(x: Tensor) -> Tensor:
+                return base_rounding_func(provided_func(x))
+
+            return combined_func
+
+    else:
+        return rounding_func
```

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_moo.py` & `ax-platform-0.3.2/ax/models/torch/botorch_moo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/botorch_moo_defaults.py` & `ax-platform-0.3.2/ax/models/torch/botorch_moo_defaults.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/cbo_lcea.py` & `ax-platform-0.3.2/ax/models/torch/cbo_lcea.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from logging import Logger
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, cast, Dict, List, Optional, Tuple, Union
 
 from ax.core.search_space import SearchSpaceDigest
 from ax.core.types import TCandidateMetadata
 from ax.models.torch.alebo import ei_or_nei
 from ax.models.torch.botorch import BotorchModel
 from ax.models.torch.cbo_sac import generate_model_space_decomposition
 from ax.models.torch_base import TorchModel, TorchOptConfig
@@ -180,7 +180,11 @@
 
         if len(models) == 1:
             model = models[0]
         else:
             model = ModelListGP(*models)
         model.to(Xs[0])
         return model
+
+    @property
+    def model(self) -> Union[LCEAGP, ModelListGP]:
+        return cast(Union[LCEAGP, ModelListGP], super().model)
```

### Comparing `ax-platform-0.3.1/ax/models/torch/cbo_lcem.py` & `ax-platform-0.3.2/ax/models/torch/cbo_lcem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/cbo_sac.py` & `ax-platform-0.3.2/ax/models/torch/cbo_sac.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/fully_bayesian.py` & `ax-platform-0.3.2/ax/models/torch/fully_bayesian.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,14 +231,15 @@
     num_samples: int = 256,
     warmup_steps: int = 512,
     thinning: int = 16,
     max_tree_depth: int = 6,
     disable_progbar: bool = False,
     gp_kernel: str = "matern",
     verbose: bool = False,
+    jit_compile: bool = False,
     # pyre-fixme[24]: Generic type `Callable` expects 2 type parameters.
     pyro_model: Callable = single_task_pyro_model,
     # pyre-fixme[24]: Generic type `Callable` expects 2 type parameters.
     get_gpytorch_model: Callable = _get_single_task_gpytorch_model,
     rank: Optional[int] = 1,
     **kwargs: Any,
     # pyre-fixme[24]: Generic type `dict` expects 2 type parameters, use `typing.Dict`
@@ -288,14 +289,15 @@
                 use_input_warping=use_input_warping,
                 max_tree_depth=max_tree_depth,
                 disable_progbar=disable_progbar,
                 gp_kernel=gp_kernel,
                 verbose=verbose,
                 task_feature=task_feature,
                 rank=rank,
+                jit_compile=jit_compile,
             )
             mcmc_samples_list.append(mcmc_samples)
     return model, mcmc_samples_list
 
 
 def get_and_fit_model_mcmc(
     Xs: List[Tensor],
@@ -311,14 +313,15 @@
     num_samples: int = 256,
     warmup_steps: int = 512,
     thinning: int = 16,
     max_tree_depth: int = 6,
     disable_progbar: bool = False,
     gp_kernel: str = "matern",
     verbose: bool = False,
+    jit_compile: bool = False,
     **kwargs: Any,
 ) -> GPyTorchModel:
     r"""Instantiates a batched GPyTorchModel(ModelListGP) based on the given data and
     fit the model based on MCMC in pyro. The batch dimension corresponds to sampled
     hyperparameters from MCMC.
     """
     model, mcmc_samples_list = _get_model_mcmc_samples(
@@ -335,14 +338,15 @@
         num_samples=num_samples,
         warmup_steps=warmup_steps,
         thinning=thinning,
         max_tree_depth=max_tree_depth,
         disable_progbar=disable_progbar,
         gp_kernel=gp_kernel,
         verbose=verbose,
+        jit_compile=jit_compile,
         pyro_model=single_task_pyro_model,
         get_gpytorch_model=_get_single_task_gpytorch_model,
     )
     for i, mcmc_samples in enumerate(mcmc_samples_list):
         load_mcmc_samples_to_model(model=model.models[i], mcmc_samples=mcmc_samples)
     return model
 
@@ -467,25 +471,25 @@
         X_pending=X_pending,
         acqf_constructor=get_NEHVI,  # pyre-ignore [6]
         **kwargs,
     )
 
 
 class FullyBayesianBotorchModelMixin:
-    model: Optional[Model] = None
+    _model: Optional[Model] = None
 
     def feature_importances(self) -> np.ndarray:
-        if self.model is None:
+        if self._model is None:
             raise RuntimeError(
                 "Cannot calculate feature_importances without a fitted model"
             )
-        elif isinstance(self.model, ModelListGP):
-            models = self.model.models
+        elif isinstance(self._model, ModelListGP):
+            models = self._model.models
         else:
-            models = [self.model]
+            models = [self._model]
         lengthscales = []
         for m in models:
             ls = m.covar_module.base_kernel.lengthscale
             lengthscales.append(ls)
         lengthscales = torch.stack(lengthscales, dim=0)
         # take mean over MCMC samples
         lengthscales = torch.quantile(lengthscales, 0.5, dim=1)
@@ -518,14 +522,15 @@
         num_samples: int = 256,
         warmup_steps: int = 512,
         thinning: int = 16,
         max_tree_depth: int = 6,
         disable_progbar: bool = False,
         gp_kernel: str = "matern",
         verbose: bool = False,
+        jit_compile: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize Fully Bayesian Botorch Model.
 
         Args:
             model_constructor: A callable that instantiates and fits a model on data,
                 with signature as described below.
@@ -573,14 +578,15 @@
             num_samples=num_samples,
             warmup_steps=warmup_steps,
             thinning=thinning,
             max_tree_depth=max_tree_depth,
             disable_progbar=disable_progbar,
             gp_kernel=gp_kernel,
             verbose=verbose,
+            jit_compile=jit_compile,
         )
 
 
 class FullyBayesianMOOBotorchModel(
     FullyBayesianBotorchModelMixin, MultiObjectiveBotorchModel
 ):
     r"""Fully Bayesian Model that uses qNEHVI.
@@ -617,14 +623,15 @@
         thinning: int = 16,
         max_tree_depth: int = 6,
         # use_saas is deprecated. TODO: remove
         use_saas: Optional[bool] = None,
         disable_progbar: bool = False,
         gp_kernel: str = "matern",
         verbose: bool = False,
+        jit_compile: bool = False,
         **kwargs: Any,
     ) -> None:
         # use_saas is deprecated. TODO: remove
         if use_saas is not None:
             warnings.warn(SAAS_DEPRECATION_MSG, DeprecationWarning)
         MultiObjectiveBotorchModel.__init__(
             self,
@@ -641,8 +648,9 @@
             num_samples=num_samples,
             warmup_steps=warmup_steps,
             thinning=thinning,
             max_tree_depth=max_tree_depth,
             disable_progbar=disable_progbar,
             gp_kernel=gp_kernel,
             verbose=verbose,
+            jit_compile=jit_compile,
         )
```

### Comparing `ax-platform-0.3.1/ax/models/torch/fully_bayesian_model_utils.py` & `ax-platform-0.3.2/ax/models/torch/fully_bayesian_model_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,34 @@
 
 import pyro
 import torch
 from ax.models.torch.botorch_defaults import _get_model
 from botorch.models.gp_regression import MIN_INFERRED_NOISE_LEVEL
 from botorch.models.gpytorch import GPyTorchModel
 from botorch.models.model_list_gp_regression import ModelListGP
-from gpytorch.kernels import RBFKernel, ScaleKernel
+from gpytorch.kernels import MaternKernel, RBFKernel, ScaleKernel
 from torch import Tensor
 
 
 def _get_rbf_kernel(num_samples: int, dim: int) -> ScaleKernel:
     return ScaleKernel(
         base_kernel=RBFKernel(ard_num_dims=dim, batch_shape=torch.Size([num_samples])),
         batch_shape=torch.Size([num_samples]),
     )
 
 
+def _get_matern_kernel(num_samples: int, dim: int) -> ScaleKernel:
+    return ScaleKernel(
+        base_kernel=MaternKernel(
+            ard_num_dims=dim, batch_shape=torch.Size([num_samples])
+        ),
+        batch_shape=torch.Size([num_samples]),
+    )
+
+
 def _get_single_task_gpytorch_model(
     Xs: List[Tensor],
     Ys: List[Tensor],
     Yvars: List[Tensor],
     task_features: List[int],
     fidelity_features: List[int],
     state_dict: Optional[Dict[str, Tensor]] = None,
@@ -49,15 +58,15 @@
             "Fidelity MF-GP models are not currently supported with MCMC!"
         )
 
     num_mcmc_samples = num_samples // thinning
     covar_modules = [
         _get_rbf_kernel(num_samples=num_mcmc_samples, dim=Xs[0].shape[-1])
         if gp_kernel == "rbf"
-        else None
+        else _get_matern_kernel(num_samples=num_mcmc_samples, dim=Xs[0].shape[-1])
         for _ in range(len(Xs))
     ]
 
     models = [
         _get_model(
             X=X.unsqueeze(0).expand(num_mcmc_samples, X.shape[0], -1),
             Y=Y.unsqueeze(0).expand(num_mcmc_samples, Y.shape[0], -1),
```

### Comparing `ax-platform-0.3.1/ax/models/torch/posterior_mean.py` & `ax-platform-0.3.2/ax/models/torch/posterior_mean.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/randomforest.py` & `ax-platform-0.3.2/ax/models/torch/randomforest.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/rembo.py` & `ax-platform-0.3.2/ax/models/torch/rembo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/tests/test_acquisition.py` & `ax-platform-0.3.2/ax/models/torch/tests/test_acquisition.py`

 * *Files 12% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         self.linear_constraints = None
         self.fixed_features = {1: 2.0}
         self.options = {"best_f": 0.0, "cache_root": False, "prune_baseline": False}
         self.inequality_constraints = [
             (torch.tensor([0, 1], **tkwargs), torch.tensor([-1.0, 1.0], **tkwargs), 1)
         ]
         self.rounding_func = lambda x: x
-        self.optimizer_options = {Keys.NUM_RESTARTS: 40, Keys.RAW_SAMPLES: 1024}
+        self.optimizer_options = {Keys.NUM_RESTARTS: 20, Keys.RAW_SAMPLES: 1024}
         self.tkwargs = tkwargs
         self.torch_opt_config = TorchOptConfig(
             objective_weights=self.objective_weights,
             objective_thresholds=self.objective_thresholds,
             pending_observations=self.pending_observations,
             outcome_constraints=self.outcome_constraints,
             linear_constraints=self.linear_constraints,
@@ -260,14 +260,15 @@
             inequality_constraints=self.inequality_constraints,
             fixed_features=self.fixed_features,
             rounding_func=self.rounding_func,
             optimizer_options=self.optimizer_options,
         )
         mock_optimize_acqf.assert_called_with(
             acq_function=acquisition.acqf,
+            sequential=True,
             bounds=mock.ANY,
             q=3,
             options={"init_batch_limit": 32, "batch_limit": 5},
             inequality_constraints=self.inequality_constraints,
             fixed_features=self.fixed_features,
             post_processing_func=self.rounding_func,
             **self.optimizer_options,
@@ -277,14 +278,56 @@
             self.search_space_digest.bounds,
             dtype=acquisition.dtype,
             device=acquisition.device,
         ).transpose(0, 1)
         self.assertTrue(
             torch.equal(mock_optimize_acqf.call_args[1]["bounds"], expected_bounds)
         )
+        # Test with custom post processing function.
+        # First, without the rounding func.
+        post_processing_func = Mock(side_effect=lambda x: x**2)
+        optimizer_options = self.optimizer_options.copy()
+        optimizer_options["post_processing_func"] = post_processing_func
+        mock_optimize_acqf.reset_mock()
+        acquisition.optimize(
+            n=3,
+            search_space_digest=self.search_space_digest,
+            inequality_constraints=self.inequality_constraints,
+            fixed_features=self.fixed_features,
+            rounding_func=None,
+            optimizer_options=optimizer_options,
+        )
+        mock_optimize_acqf.assert_called_with(
+            acq_function=acquisition.acqf,
+            sequential=True,
+            bounds=mock.ANY,
+            q=3,
+            options={"init_batch_limit": 32, "batch_limit": 5},
+            inequality_constraints=self.inequality_constraints,
+            fixed_features=self.fixed_features,
+            post_processing_func=post_processing_func,
+            **self.optimizer_options,
+        )
+        # Now using both rounding func and post processing func.
+        mock_optimize_acqf.reset_mock()
+        rounding_func = Mock(side_effect=lambda x: x // 4)
+        acquisition.optimize(
+            n=3,
+            search_space_digest=self.search_space_digest,
+            inequality_constraints=self.inequality_constraints,
+            fixed_features=self.fixed_features,
+            rounding_func=rounding_func,
+            optimizer_options=optimizer_options,
+        )
+        actual_func = mock_optimize_acqf.call_args[-1]["post_processing_func"]
+        # Call it with a known input to check that the functions are called in
+        # the correct order.
+        self.assertEqual(actual_func(3.0), 2)  # (3 ** 2) // 4 = 2
+        post_processing_func.assert_called_once_with(3.0)
+        rounding_func.assert_called_once_with(9.0)
 
     def test_optimize_discrete(self) -> None:
         ssd1 = SearchSpaceDigest(
             feature_names=["a", "b", "c"],
             # pyre-fixme[6]: For 2nd param expected `List[Tuple[Union[float, int],
             #  Union[float, int]]]` but got `List[Tuple[int, int, int]]`.
             bounds=[(1, 2, 3), (2, 3, 4)],
@@ -447,14 +490,15 @@
             inequality_constraints=self.inequality_constraints,
             fixed_features=None,
             rounding_func=self.rounding_func,
             optimizer_options=self.optimizer_options,
         )
         mock_optimize_acqf_mixed.assert_called_with(
             acq_function=acquisition.acqf,
+            sequential=True,
             bounds=mock.ANY,
             q=3,
             options={"init_batch_limit": 32, "batch_limit": 5},
             fixed_features_list=[{1: 0}, {1: 1}, {1: 2}],
             inequality_constraints=self.inequality_constraints,
             post_processing_func=self.rounding_func,
             **self.optimizer_options,
@@ -462,14 +506,40 @@
         # can't use assert_called_with on bounds due to ambiguous bool comparison
         expected_bounds = torch.tensor(ssd.bounds, **tkwargs).transpose(0, 1)
         self.assertTrue(
             torch.equal(
                 mock_optimize_acqf_mixed.call_args[1]["bounds"], expected_bounds
             )
         )
+        # Check that we don't use mixed optimizer if force_use_optimize_acqf is True.
+        mock_optimize_acqf_mixed.reset_mock()
+        optimizer_options = self.optimizer_options.copy()
+        optimizer_options["force_use_optimize_acqf"] = True
+        with mock.patch(f"{ACQUISITION_PATH}.optimize_acqf") as mock_optimize_acqf:
+            acquisition.optimize(
+                n=3,
+                search_space_digest=ssd,
+                inequality_constraints=self.inequality_constraints,
+                fixed_features=None,
+                rounding_func=self.rounding_func,
+                optimizer_options=optimizer_options,
+            )
+        self.assertEqual(mock_optimize_acqf_mixed.call_count, 0)
+        mock_optimize_acqf.assert_called_once()
+        mock_optimize_acqf.assert_called_with(
+            acq_function=acquisition.acqf,
+            sequential=True,
+            bounds=mock.ANY,
+            q=3,
+            options={"init_batch_limit": 32, "batch_limit": 5},
+            inequality_constraints=self.inequality_constraints,
+            fixed_features=None,
+            post_processing_func=self.rounding_func,
+            **self.optimizer_options,
+        )
 
     @mock.patch(
         f"{DummyOneShotAcquisitionFunction.__module__}."
         "DummyOneShotAcquisitionFunction.evaluate",
         return_value=None,
     )
     @mock.patch(
```

### Comparing `ax-platform-0.3.1/ax/models/torch/tests/test_model.py` & `ax-platform-0.3.2/ax/models/torch/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import dataclasses
 import warnings
 from contextlib import ExitStack
+from copy import deepcopy
 from typing import Dict
 from unittest import mock
-from unittest.mock import Mock
+from unittest.mock import Mock, patch
 
 import numpy as np
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.exceptions.core import AxWarning, UnsupportedError
 from ax.models.torch.botorch_modular.acquisition import Acquisition
 from ax.models.torch.botorch_modular.model import BoTorchModel, SurrogateSpec
@@ -31,14 +32,15 @@
     get_acqf_input_constructor,
 )
 from botorch.acquisition.monte_carlo import qExpectedImprovement
 from botorch.acquisition.multi_objective.monte_carlo import (
     qNoisyExpectedHypervolumeImprovement,
 )
 from botorch.acquisition.multi_objective.objective import WeightedMCMultiOutputObjective
+from botorch.models.fully_bayesian import SaasFullyBayesianSingleTaskGP
 from botorch.models.gp_regression import FixedNoiseGP, SingleTaskGP
 from botorch.models.gp_regression_fidelity import FixedNoiseMultiFidelityGP
 from botorch.models.model import ModelList
 from botorch.sampling.normal import SobolQMCNormalSampler
 from botorch.utils.datasets import FixedNoiseDataset, SupervisedDataset
 from gpytorch.mlls.exact_marginal_log_likelihood import ExactMarginalLogLikelihood
 
@@ -68,14 +70,15 @@
             botorch_acqf_class=self.botorch_acqf_class,
             acquisition_options=self.acquisition_options,
         )
 
         self.dtype = torch.float
         self.device = torch.device("cpu")
         tkwargs = {"dtype": self.dtype, "device": self.device}
+        self.tkwargs = tkwargs
         Xs1, Ys1, Yvars1, self.bounds, _, _, _ = get_torch_test_data(dtype=self.dtype)
         Xs2, Ys2, Yvars2, _, _, _, _ = get_torch_test_data(dtype=self.dtype, offset=1.0)
         self.Xs = Xs1
         self.Ys = Ys1
         self.Yvars = Yvars1
         self.X_test = Xs2[0]
         self.block_design_training_data = [
@@ -255,21 +258,30 @@
             search_space_digest=self.mf_search_space_digest,
         )
 
     @mock.patch(f"{SURROGATE_PATH}.Surrogate.fit")
     def test_fit(self, mock_fit: Mock) -> None:
         # If surrogate is not yet set, initialize it with dispatcher functions.
         self.model._surrogates = {}
+        with self.assertRaisesRegex(RuntimeError, "is not initialized. Must `fit`"):
+            self.model.search_space_digest  # can't access before fit
+
+        with self.assertRaisesRegex(RuntimeError, "manually is disallowed"):
+            self.model.search_space_digest = self.mf_search_space_digest
+
         self.model.fit(
             datasets=self.block_design_training_data,
             metric_names=self.metric_names,
             search_space_digest=self.mf_search_space_digest,
             candidate_metadata=self.candidate_metadata,
         )
 
+        self.assertIsInstance(self.model.search_space_digest, SearchSpaceDigest)
+        self.assertEqual(self.model.search_space_digest, self.mf_search_space_digest)
+
         # Since we want to refit on updates but not warm start refit, we clear the
         # state dict.
         mock_fit.assert_called_with(
             datasets=self.block_design_training_data,
             metric_names=self.metric_names,
             search_space_digest=self.mf_search_space_digest,
             candidate_metadata=self.candidate_metadata,
@@ -281,14 +293,24 @@
             ValueError, "Length of datasets and metric_names must match"
         ):
             self.model.fit(
                 datasets=self.block_design_training_data,
                 metric_names=self.metric_names * 2,
                 search_space_digest=self.mf_search_space_digest,
             )
+        # since Surrogate.fit is mocked, it didn't actually assign the outcomes
+        with patch.object(
+            self.model.surrogate,
+            "_outcomes",
+            self.metric_names,
+        ):
+            labels_to_outcomes = self.model.outcomes_by_surrogate_label
+        self.assertIsInstance(labels_to_outcomes, dict)
+        self.assertEqual(len(labels_to_outcomes), 1)
+        self.assertEqual(next(iter(labels_to_outcomes.values())), self.metric_names)
 
     @mock.patch(f"{SURROGATE_PATH}.Surrogate.update")
     def test_update(self, mock_update: Mock) -> None:
         # test assertion that model needs to be fit first
         empty_model = BoTorchModel()
         with self.assertRaisesRegex(
             UnsupportedError, "Cannot update model that has not been fitted."
@@ -539,14 +561,88 @@
             search_space_digest=self.mf_search_space_digest,
             inequality_constraints=[],
             fixed_features=self.fixed_features,
             rounding_func="func",
             optimizer_options=self.optimizer_options,
         )
 
+    def test_feature_importances(self) -> None:
+        for botorch_model_class in [SingleTaskGP, SaasFullyBayesianSingleTaskGP]:
+            surrogate = Surrogate(botorch_model_class=botorch_model_class)
+            model = BoTorchModel(
+                surrogate=surrogate,
+                acquisition_class=Acquisition,
+                acquisition_options=self.acquisition_options,
+            )
+            model.surrogates[Keys.ONLY_SURROGATE].construct(
+                datasets=self.block_design_training_data,
+                metric_names=["metric"],
+                search_space_digest=SearchSpaceDigest(feature_names=[], bounds=[]),
+            )
+            if botorch_model_class == SaasFullyBayesianSingleTaskGP:
+                mcmc_samples = {
+                    "lengthscale": torch.tensor(
+                        [[1, 2, 3], [2, 3, 4], [3, 4, 5]], **self.tkwargs
+                    ),
+                    "outputscale": torch.rand(3, **self.tkwargs),
+                    "mean": torch.randn(3, **self.tkwargs),
+                    "noise": torch.rand(3, **self.tkwargs),
+                }
+                model.surrogate.model.load_mcmc_samples(mcmc_samples)  # pyre-ignore
+                importances = model.feature_importances()
+                self.assertTrue(
+                    np.allclose(importances, np.array([6 / 13, 4 / 13, 3 / 13]))
+                )
+                self.assertEqual(importances.shape, (1, 1, 3))
+                saas_model = deepcopy(model.surrogate.model)
+            else:
+                model.surrogate.model.covar_module.base_kernel.lengthscale = (
+                    torch.tensor([1, 2, 3], **self.tkwargs)
+                )
+                importances = model.feature_importances()
+                self.assertTrue(
+                    np.allclose(importances, np.array([6 / 11, 3 / 11, 2 / 11]))
+                )
+                self.assertEqual(importances.shape, (1, 1, 3))
+                vanilla_model = deepcopy(model.surrogate.model)
+
+        # Mixed model
+        model.surrogate._model = ModelList(saas_model, vanilla_model)  # pyre-ignore
+        importances = model.feature_importances()
+        self.assertTrue(
+            np.allclose(
+                importances,
+                np.expand_dims(
+                    np.array([[6 / 13, 4 / 13, 3 / 13], [6 / 11, 3 / 11, 2 / 11]]),
+                    axis=1,
+                ),
+            )
+        )
+        self.assertEqual(importances.shape, (2, 1, 3))
+        # Add model we don't support
+        vanilla_model.covar_module.base_kernel = None
+        model.surrogate._model = vanilla_model  # pyre-ignore
+        with self.assertRaisesRegex(
+            NotImplementedError,
+            "Failed to extract lengthscales from `m.covar_module.base_kernel`",
+        ):
+            model.feature_importances()
+        # Test model is None
+        model.surrogate._model = None
+        with self.assertRaisesRegex(
+            ValueError, "BoTorch `Model` has not yet been constructed"
+        ):
+            model.feature_importances()
+        # Test unsupported surrogate
+        model._surrogates = {"vanilla": None, "saas": None}
+        with self.assertRaisesRegex(
+            NotImplementedError, "Only support a single surrogate model for now"
+        ):
+            model.feature_importances()
+
     @fast_botorch_optimize
     def test_best_point(self) -> None:
         self.model._surrogates = {}
         self.model.fit(
             datasets=self.block_design_training_data,
             metric_names=self.metric_names,
             search_space_digest=self.mf_search_space_digest,
```

### Comparing `ax-platform-0.3.1/ax/models/torch/tests/test_multi_fidelity.py` & `ax-platform-0.3.2/ax/models/torch/tests/test_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/tests/test_optimizer_argparse.py` & `ax-platform-0.3.2/ax/models/torch/tests/test_optimizer_argparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,29 +98,27 @@
         for acqf in (
             qExpectedHypervolumeImprovement,
             qNoisyExpectedHypervolumeImprovement,
         ):
             with self.subTest(acqf=acqf):
                 options = optimizer_argparse(
                     acqf,
-                    sequential=False,
                     optimizer_options=user_options,
                     **inner_options,
                 )
-                self.assertEqual(options.pop("sequential"), False)
+                self.assertEqual(options["sequential"], True)
                 self.assertEqual(options.pop("options"), inner_options)
                 self.assertEqual(options, generic_options)
 
                 # Defaults
                 options = optimizer_argparse(
                     acqf,
-                    sequential=False,
+                    sequential=True,
                     optimizer_options=user_options,
                 )
-                self.assertEqual(options.pop("sequential"), False)
                 self.assertEqual(
                     options.pop("options"), {"init_batch_limit": 32, "batch_limit": 5}
                 )
                 self.assertEqual(options, generic_options)
 
     def test_kg(self) -> None:
         with patch(
@@ -145,12 +143,11 @@
     def test_mes(self) -> None:
         user_options = {"foo": "bar", "num_restarts": 83}
         generic_options = _argparse_base(None, optimizer_options=user_options)
         for acqf in (qMaxValueEntropy, qMultiFidelityMaxValueEntropy):
             with self.subTest(acqf=acqf):
                 options = optimizer_argparse(
                     acqf,
-                    sequential=False,
                     optimizer_options=user_options,
                 )
-                self.assertEqual(options.pop("sequential"), False)
+                self.assertEqual(options["sequential"], True)
                 self.assertEqual(options, generic_options)
```

### Comparing `ax-platform-0.3.1/ax/models/torch/tests/test_surrogate.py` & `ax-platform-0.3.2/ax/models/torch/tests/test_surrogate.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,36 +6,37 @@
 
 import dataclasses
 import math
 from typing import Any, Dict, Tuple, Type
 from unittest.mock import MagicMock, Mock, patch
 
 import numpy as np
-
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.exceptions.core import UnsupportedError, UserInputError
 from ax.models.torch.botorch_modular.acquisition import Acquisition
 from ax.models.torch.botorch_modular.surrogate import Surrogate
 from ax.models.torch.botorch_modular.utils import choose_model_class, fit_botorch_model
 from ax.models.torch_base import TorchOptConfig
 from ax.utils.common.constants import Keys
 from ax.utils.common.testutils import TestCase
 from ax.utils.common.typeutils import checked_cast, not_none
+from ax.utils.testing.mock import fast_botorch_optimize
 from ax.utils.testing.torch_stubs import get_torch_test_data
 from ax.utils.testing.utils import generic_equals
 from botorch.acquisition.monte_carlo import qSimpleRegret
 from botorch.models import (
     FixedNoiseGP,
     ModelListGP,
     SaasFullyBayesianSingleTaskGP,
     SingleTaskGP,
 )
 from botorch.models.deterministic import GenericDeterministicModel
 from botorch.models.fully_bayesian_multitask import SaasFullyBayesianMultiTaskGP
+from botorch.models.gp_regression_mixed import MixedSingleTaskGP
 from botorch.models.model import Model, ModelList  # noqa: F401
 from botorch.models.multitask import FixedNoiseMultiTaskGP, MultiTaskGP
 from botorch.models.pairwise_gp import PairwiseGP, PairwiseLaplaceMarginalLogLikelihood
 from botorch.models.transforms.input import InputPerturbation, Normalize
 from botorch.models.transforms.outcome import Standardize
 from botorch.sampling.normal import SobolQMCNormalSampler
 from botorch.utils.datasets import FixedNoiseDataset, SupervisedDataset
@@ -44,14 +45,15 @@
 from gpytorch.likelihoods import (  # noqa: F401
     FixedNoiseGaussianLikelihood,
     GaussianLikelihood,
     Likelihood,  # noqa: F401
 )
 from gpytorch.mlls import ExactMarginalLogLikelihood, LeaveOneOutPseudoLikelihood
 from torch import Tensor
+from torch.nn import ModuleList  # @manual
 
 
 ACQUISITION_PATH = f"{Acquisition.__module__}"
 CURRENT_PATH = f"{__name__}"
 SURROGATE_PATH = f"{Surrogate.__module__}"
 UTILS_PATH = f"{fit_botorch_model.__module__}"
 
@@ -63,14 +65,15 @@
         super().__init__(train_X=train_X, train_Y=train_Y)
 
 
 class SurrogateTest(TestCase):
     def setUp(self) -> None:
         self.device = torch.device("cpu")
         self.dtype = torch.float
+        self.tkwargs = {"device": self.device, "dtype": self.dtype}
         self.Xs, self.Ys, self.Yvars, self.bounds, _, _, _ = get_torch_test_data(
             dtype=self.dtype
         )
         self.metric_names = ["metric"]
         self.training_data = [SupervisedDataset(X=self.Xs[0], Y=self.Ys[0])]
         self.mll_class = ExactMarginalLogLikelihood
         self.search_space_digest = SearchSpaceDigest(
@@ -117,30 +120,95 @@
             self.assertTrue(surrogate.allow_batched_models)  # True by default
 
     def test_clone_reset(self) -> None:
         surrogate = self._get_surrogate(botorch_model_class=SingleTaskGP)[0]
         self.assertEqual(surrogate, surrogate.clone_reset())
 
     @patch(f"{UTILS_PATH}.fit_gpytorch_mll")
-    # pyre-fixme[3]: Return type must be annotated.
-    def test_mll_options(self, _):
+    def test_mll_options(self, _) -> None:
         mock_mll = MagicMock(self.mll_class)
         surrogate = Surrogate(
             botorch_model_class=SingleTaskGP,
             mll_class=mock_mll,
             mll_options={"some_option": "some_value"},
         )
         surrogate.fit(
             datasets=self.training_data,
             metric_names=self.metric_names,
             search_space_digest=self.search_space_digest,
             refit=self.refit,
         )
         self.assertEqual(mock_mll.call_args[1]["some_option"], "some_value")
 
+    @fast_botorch_optimize
+    def test_copy_options(self) -> None:
+        training_data = [
+            SupervisedDataset(X=self.Xs[0], Y=self.Ys[0]),
+            SupervisedDataset(X=2 * self.Xs[0], Y=2 * self.Ys[0]),
+        ]
+        d = self.Xs[0].shape[-1]
+        surrogate = Surrogate(
+            botorch_model_class=SingleTaskGP,
+            likelihood_class=GaussianLikelihood,
+            likelihood_options={"noise_constraint": GreaterThan(1e-3)},
+            mll_class=ExactMarginalLogLikelihood,
+            covar_module_class=ScaleKernel,
+            covar_module_options={"base_kernel": MaternKernel(ard_num_dims=d)},
+            input_transform=Normalize(d=d),
+            outcome_transform=Standardize(m=1),
+            allow_batched_models=False,
+        )
+        surrogate.fit(
+            datasets=training_data,
+            metric_names=["m1", "m2"],
+            search_space_digest=self.search_space_digest,
+            refit=True,
+        )
+        models = checked_cast(ModuleList, surrogate.model.models)
+        # Change the lengthscales of one model and make sure the other isn't changed
+        models[0].covar_module.base_kernel.lengthscale += 1
+        self.assertTrue(
+            torch.allclose(
+                models[0].covar_module.base_kernel.lengthscale,
+                models[1].covar_module.base_kernel.lengthscale + 1.0,  # pyre-ignore
+            )
+        )
+        # Test the same thing with the likelihood noise constraint
+        models[0].likelihood.noise_covar.raw_noise_constraint.lower_bound.fill_(1e-4)
+        self.assertEqual(
+            models[0].likelihood.noise_covar.raw_noise_constraint.lower_bound, 1e-4
+        )
+        self.assertEqual(
+            models[1].likelihood.noise_covar.raw_noise_constraint.lower_bound, 1e-3
+        )
+        # Check input transform
+        self.assertTrue(
+            torch.allclose(
+                models[0].input_transform.offset,
+                torch.tensor([1, 2, 3], **self.tkwargs),
+            )
+        )
+        self.assertTrue(
+            torch.allclose(
+                models[1].input_transform.offset,
+                torch.tensor([2, 4, 6], **self.tkwargs),
+            )
+        )
+        # Check outcome transform
+        self.assertTrue(
+            torch.allclose(
+                models[0].outcome_transform.means, torch.tensor([3.5], **self.tkwargs)
+            )
+        )
+        self.assertTrue(
+            torch.allclose(
+                models[1].outcome_transform.means, torch.tensor([7], **self.tkwargs)
+            )
+        )
+
     def test_botorch_transforms(self) -> None:
         # Successfully passing down the transforms
         input_transform = Normalize(d=self.Xs[0].shape[-1])
         outcome_transform = Standardize(m=self.Ys[0].shape[-1])
         surrogate = Surrogate(
             botorch_model_class=SingleTaskGP,
             outcome_transform=outcome_transform,
@@ -338,14 +406,20 @@
             [SaasFullyBayesianSingleTaskGP, SingleTaskGP],
         ):
             surrogate, surrogate_kwargs = self._get_surrogate(
                 botorch_model_class=botorch_model_class
             )
             # Checking that model is None before `fit` (and `construct`) calls.
             self.assertIsNone(surrogate._model)
+            with self.assertRaisesRegex(RuntimeError, "outcomes not initialized."):
+                surrogate.outcomes
+            with self.assertRaisesRegex(
+                RuntimeError, "Setting outcomes manually is disallowed."
+            ):
+                surrogate.outcomes = self.metric_names
             # Should instantiate mll and `fit_gpytorch_mll` when `state_dict`
             # is `None`.
             surrogate.fit(
                 datasets=self.training_data,
                 metric_names=self.metric_names,
                 search_space_digest=self.search_space_digest,
                 refit=self.refit,
@@ -374,15 +448,15 @@
             surrogate.fit(
                 datasets=self.training_data,
                 metric_names=self.metric_names,
                 search_space_digest=self.search_space_digest,
                 refit=self.refit,
                 original_metric_names=self.original_metric_names,
             )
-            self.assertEqual(surrogate._outcomes, self.original_metric_names)
+            self.assertEqual(surrogate.outcomes, self.original_metric_names)
             mock_state_dict.reset_mock()
             mock_MLL.reset_mock()
             mock_fit.reset_mock()
             # Should `load_state_dict` when `state_dict` is not `None`
             # and `refit` is `False`.
             state_dict = {"state_attribute": torch.zeros(1)}
             surrogate.fit(
@@ -627,14 +701,58 @@
             metric_names=self.metric_names,
             robust_digest=robust_digest,
         )
         intf = checked_cast(InputPerturbation, surrogate.model.input_transform)
         self.assertIsInstance(intf, InputPerturbation)
         self.assertTrue(torch.equal(intf.perturbation_set, torch.zeros(2, 2)))
 
+    def test_fit_mixed(self) -> None:
+        # Test model construction with categorical variables.
+        surrogate = Surrogate()
+        search_space_digest = dataclasses.replace(
+            self.search_space_digest,
+            categorical_features=[0],
+        )
+        surrogate.fit(
+            datasets=self.training_data,
+            metric_names=self.metric_names,
+            search_space_digest=search_space_digest,
+        )
+        self.assertIsInstance(surrogate.model, MixedSingleTaskGP)
+        # _ignore_X_dims_scaling_check is the easiest way to check cat dims.
+        self.assertEqual(surrogate.model._ignore_X_dims_scaling_check, [0])
+        covar_module = checked_cast(Kernel, surrogate.model.covar_module)
+        self.assertEqual(
+            covar_module.kernels[0].base_kernel.kernels[1].active_dims.tolist(), [0]
+        )
+        self.assertEqual(
+            covar_module.kernels[0].base_kernel.kernels[0].active_dims.tolist(), [1, 2]
+        )
+        self.assertEqual(
+            covar_module.kernels[1].base_kernel.kernels[1].active_dims.tolist(), [0]
+        )
+        self.assertEqual(
+            covar_module.kernels[1].base_kernel.kernels[0].active_dims.tolist(), [1, 2]
+        )
+        # With modellist.
+        training_data = [self.training_data[0], self.training_data[0]]
+        surrogate = Surrogate(allow_batched_models=False)
+        surrogate.fit(
+            datasets=training_data,
+            metric_names=self.original_metric_names,
+            search_space_digest=search_space_digest,
+        )
+        self.assertIsInstance(surrogate.model, ModelListGP)
+        self.assertTrue(
+            all(
+                isinstance(m, MixedSingleTaskGP)
+                for m in checked_cast(ModelListGP, surrogate.model).models
+            )
+        )
+
 
 class SurrogateWithModelListTest(TestCase):
     def setUp(self) -> None:
         self.outcomes = ["outcome_1", "outcome_2"]
         self.mll_class = ExactMarginalLogLikelihood
         self.dtype = torch.float
         self.search_space_digest = SearchSpaceDigest(
@@ -720,14 +838,15 @@
         for idx in range(len(mock_MTGP_construct_inputs.call_args_list)):
             self.assertEqual(
                 # `call_args` is a tuple of (args, kwargs), and we check kwargs.
                 mock_MTGP_construct_inputs.call_args_list[idx][1],
                 {
                     "fidelity_features": [],
                     "task_feature": self.task_features[0],
+                    "categorical_features": None,
                     # TODO: Figure out how to handle Multitask GPs and construct-inputs.
                     # I believe this functionality with modlular botorch model is
                     # currently broken as MultiTaskGP.construct_inputs expects a dict
                     # mapping string keys (outcomes) to input datasets
                     "training_data": FixedNoiseDataset(
                         X=self.Xs[idx], Y=self.Ys[idx], Yvar=self.Yvars[idx]
                     ),
```

### Comparing `ax-platform-0.3.1/ax/models/torch/tests/test_utils.py` & `ax-platform-0.3.2/ax/models/torch/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch/utils.py` & `ax-platform-0.3.2/ax/models/torch/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/torch_base.py` & `ax-platform-0.3.2/ax/models/torch_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/types.py` & `ax-platform-0.3.2/ax/models/types.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/models/winsorization_config.py` & `ax-platform-0.3.2/ax/models/winsorization_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/bandit_rollout.py` & `ax-platform-0.3.2/ax/plot/bandit_rollout.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/base.py` & `ax-platform-0.3.2/ax/plot/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/benchmark.py` & `ax-platform-0.3.2/ax/plot/benchmark.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/color.py` & `ax-platform-0.3.2/ax/plot/color.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/contour.py` & `ax-platform-0.3.2/ax/plot/contour.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         model=model,
         x_param_name=param_x,
         y_param_name=param_y,
         metric=metric_name,
         generator_runs_dict=generator_runs_dict,
         density=density,
         slice_values=slice_values,
+        fixed_features=fixed_features,
     )
     config = {
         "arm_data": data,
         "blue_scale": BLUE_SCALE,
         "density": density,
         "f": f_plt,
         "green_scale": GREEN_SCALE,
```

### Comparing `ax-platform-0.3.1/ax/plot/css/base.css` & `ax-platform-0.3.2/ax/plot/css/base.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/diagnostic.py` & `ax-platform-0.3.2/ax/plot/diagnostic.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/feature_importances.py` & `ax-platform-0.3.2/ax/plot/feature_importances.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/helper.py` & `ax-platform-0.3.2/ax/plot/helper.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/js/common/helpers.js` & `ax-platform-0.3.2/ax/plot/js/common/helpers.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/marginal_effects.py` & `ax-platform-0.3.2/ax/plot/marginal_effects.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/parallel_coordinates.py` & `ax-platform-0.3.2/ax/plot/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/pareto_frontier.py` & `ax-platform-0.3.2/ax/plot/pareto_frontier.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     all_metrics = frontier.means.keys()
     if frontier.arm_names is None:
         arm_names = [f"Parameterization {i}" for i in range(len(frontier.param_dicts))]
     else:
         arm_names = [f"Arm {name}" for name in frontier.arm_names]
 
     if CI_level is not None:
-        Z = 0.5 * norm.ppf(1 - (1 - CI_level) / 2)
+        Z = norm.ppf(1 - (1 - CI_level) / 2)
     else:
         Z = None
 
     labels = []
 
     for i, param_dict in enumerate(frontier.param_dicts):
         label = f"<b>{arm_names[i]}</b><br>"
@@ -519,18 +519,29 @@
     return AxPlotConfig(data=fig, plot_type=AxPlotTypes.GENERIC)
 
 
 def interact_pareto_frontier(
     frontier_list: List[ParetoFrontierResults],
     CI_level: float = DEFAULT_CI_LEVEL,
     show_parameterization_on_hover: bool = True,
+    label_dict: Optional[Dict[str, str]] = None,
 ) -> AxPlotConfig:
-    """Plot a pareto frontier from a list of objects"""
+    """Plot a pareto frontier from a list of objects
+
+    Args:
+        frontier_list: List of ParetoFrontierResults objects to be plotted.
+        CI_level: CI level for error bars.
+        show_parameterization_on_hover: Show parameterization on hover.
+        label_dict: Map from metric name to shortened alias to use on plot.
+    """
     if not frontier_list:
         raise ValueError("Must receive a non-empty list of pareto frontiers to plot.")
+    label_dict_use = {k: k for k in frontier_list[0].means}
+    if label_dict is not None:
+        label_dict_use.update(label_dict)
 
     traces = []
     shapes = []
     for frontier in frontier_list:
         config = plot_pareto_frontier(
             frontier=frontier,
             CI_level=CI_level,
@@ -551,39 +562,39 @@
         trace_cnt = 1
         # Only one plot trace is visible at a given time.
         visible = [False] * (len(frontier_list) * trace_cnt)
         for j in range(i * trace_cnt, (i + 1) * trace_cnt):
             visible[j] = True
         rel_y = frontier.primary_metric not in frontier.absolute_metrics
         rel_x = frontier.secondary_metric not in frontier.absolute_metrics
-        primary_metric = frontier.primary_metric
-        secondary_metric = frontier.secondary_metric
+        primary_metric = label_dict_use[frontier.primary_metric]
+        secondary_metric = label_dict_use[frontier.secondary_metric]
         dropdown.append(
             {
                 "method": "update",
                 "args": [
                     {"visible": visible, "method": "restyle"},
                     {
                         "yaxis.title": primary_metric,
                         "xaxis.title": secondary_metric,
                         "yaxis.ticksuffix": "%" if rel_y else "",
                         "xaxis.ticksuffix": "%" if rel_x else "",
                         "shapes": shapes[i],
                     },
                 ],
-                "label": f"{primary_metric} vs {secondary_metric}",
+                "label": f"{primary_metric}<br>vs {secondary_metric}",
             }
         )
 
     # Set initial layout arguments.
     initial_frontier = frontier_list[0]
     rel_x = initial_frontier.secondary_metric not in initial_frontier.absolute_metrics
     rel_y = initial_frontier.primary_metric not in initial_frontier.absolute_metrics
-    secondary_metric = initial_frontier.secondary_metric
-    primary_metric = initial_frontier.primary_metric
+    secondary_metric = label_dict_use[initial_frontier.secondary_metric]
+    primary_metric = label_dict_use[initial_frontier.primary_metric]
 
     layout = go.Layout(
         title="Pareto Frontier",
         xaxis={
             "title": secondary_metric,
             "ticksuffix": "%" if rel_x else "",
             "zeroline": True,
```

### Comparing `ax-platform-0.3.1/ax/plot/pareto_utils.py` & `ax-platform-0.3.2/ax/plot/pareto_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,28 +22,23 @@
 from ax.core.outcome_constraint import (
     ComparisonOp,
     ObjectiveThreshold,
     OutcomeConstraint,
 )
 from ax.core.search_space import RobustSearchSpace, SearchSpace
 from ax.core.types import TParameterization
-from ax.exceptions.core import AxError, UnsupportedError
+from ax.exceptions.core import AxError, UnsupportedError, UserInputError
 from ax.modelbridge.modelbridge_utils import (
     _get_modelbridge_training_data,
     get_pareto_frontier_and_configs,
     observed_pareto_frontier,
 )
 from ax.modelbridge.registry import Models
 from ax.modelbridge.torch import TorchModelBridge
-from ax.modelbridge.transforms.choice_encode import OrderedChoiceEncode
-from ax.modelbridge.transforms.derelativize import Derelativize
-from ax.modelbridge.transforms.int_to_float import IntToFloat
-from ax.modelbridge.transforms.one_hot import OneHot
-from ax.modelbridge.transforms.remove_fixed import RemoveFixed
-from ax.modelbridge.transforms.search_space_to_choice import SearchSpaceToChoice
+from ax.modelbridge.transforms.search_space_to_float import SearchSpaceToFloat
 from ax.models.torch.posterior_mean import get_PosteriorMean
 from ax.models.torch_base import TorchModel
 from ax.utils.common.logger import get_logger
 from ax.utils.stats.statstools import relativize
 from botorch.utils.multi_objective import is_non_dominated
 from botorch.utils.multi_objective.hypervolume import infer_reference_point
 
@@ -116,20 +111,62 @@
     primary_metric: str
     secondary_metric: str
     absolute_metrics: List[str]
     objective_thresholds: Optional[Dict[str, float]]
     arm_names: Optional[List[Optional[str]]]
 
 
+def _extract_sq_data(
+    experiment: Experiment, data: Data
+) -> Tuple[Dict[str, float], Dict[str, float]]:
+    """
+    Returns sq_means and sq_sems, each a mapping from metric name to, respectively, mean
+    and sem of the status quo arm. Empty dictionaries if no SQ arm.
+    """
+    sq_means = {}
+    sq_sems = {}
+    if experiment.status_quo is not None:
+        # Extract SQ values
+        sq_df = data.df[
+            data.df["arm_name"] == experiment.status_quo.name  # pyre-ignore
+        ]
+        for metric, metric_df in sq_df.groupby("metric_name"):
+            sq_means[metric] = metric_df["mean"].values[0]
+            sq_sems[metric] = metric_df["sem"].values[0]
+    return sq_means, sq_sems
+
+
+def _relativize_values(
+    means: List[float], sq_mean: float, sems: List[float], sq_sem: float
+) -> Tuple[List[float], List[float]]:
+    """
+    Relativize values, using delta method if SEMs provided, or just by relativizing
+    means if not. Relativization is as percent.
+    """
+    if np.isnan(sq_sem) or np.isnan(sems).any():
+        # Just relativize means
+        means = [(mu / sq_mean - 1) * 100 for mu in means]
+    else:
+        # Use delta method
+        means_arr, sems_arr = relativize(
+            means_t=np.array(means),
+            sems_t=np.array(sems),
+            mean_c=sq_mean,
+            sem_c=sq_sem,
+            as_percent=True,
+        )
+        means, sems = list(means), list(sems)
+    return means, sems
+
+
 def get_observed_pareto_frontiers(
     experiment: Experiment,
     data: Optional[Data] = None,
-    rel: bool = True,
+    rel: Optional[bool] = None,
     arm_names: Optional[List[str]] = None,
-    is_pex: Optional[bool] = False,
 ) -> List[ParetoFrontierResults]:
     """
     Find all Pareto points from an experiment.
 
     Uses only values as observed in the data; no modeling is involved. Makes no
     assumption about the search space or types of parameters. If "data" is provided will
     use that, otherwise will use all data already attached to the experiment.
@@ -144,15 +181,17 @@
     Will generate a ParetoFrontierResults for every pair of metrics in the experiment's
     multiobjective optimization config.
 
     Args:
         experiment: The experiment.
         data: Data to use for computing Pareto frontier. If not provided, will lookup
             data from experiment.
-        rel: Relativize, if status quo on experiment.
+        rel: Relativize results wrt experiment status quo. If None, then rel will be
+            taken for each objective separately from its own objective threshold.
+            `rel` must be specified if there are missing objective thresholds.
         arm_names: If provided, computes Pareto frontier only from among the provided
             list of arm names, plus status quo if set on experiment.
 
     Returns: ParetoFrontierResults that can be used with interact_pareto_frontier.
     """
     if data is None:
         data = experiment.lookup_data()
@@ -162,18 +201,15 @@
         if (
             experiment.status_quo is not None
             and experiment.status_quo.name not in arm_names
         ):
             # Make sure status quo is always included, for derelativization
             arm_names.append(experiment.status_quo.name)
         data = Data(data.df[data.df["arm_name"].isin(arm_names)])
-    if is_pex:
-        mb = pex_get_tensor_converter_model(experiment=experiment, data=data)
-    else:
-        mb = get_tensor_converter_model(experiment=experiment, data=data)
+    mb = get_tensor_converter_model(experiment=experiment, data=data)
     pareto_observations = observed_pareto_frontier(modelbridge=mb)
     # Convert to ParetoFrontierResults
     objective_metric_names = {
         metric.name
         for metric in experiment.optimization_config.objective.metrics  # pyre-ignore
     }
     obj_metr_list = sorted(objective_metric_names)
@@ -182,59 +218,63 @@
 
     for obs in pareto_observations:
         for i, name in enumerate(obs.data.metric_names):
             if name in objective_metric_names:
                 pfr_means[name].append(obs.data.means[i])
                 pfr_sems[name].append(np.sqrt(obs.data.covariance[i, i]))
 
-    # Relativize as needed
-    if rel and experiment.status_quo is not None:
-        # Get status quo values
-        # pyre-fixme[16]: `Optional` has no attribute `name`.
-        sq_df = data.df[data.df["arm_name"] == experiment.status_quo.name]
-        sq_df = sq_df.to_dict(orient="list")
-        sq_means = {}
-        sq_sems = {}
-        # pyre-fixme[6]: Expected `_SupportsIndex` for 1st param but got `str`.
-        for i, metric in enumerate(sq_df["metric_name"]):
-            # pyre-fixme[6]: Expected `_SupportsIndex` for 1st param but got `str`.
-            sq_means[metric] = sq_df["mean"][i]
-            # pyre-fixme[6]: Expected `_SupportsIndex` for 1st param but got `str`.
-            sq_sems[metric] = sq_df["sem"][i]
-        # Relativize
-        for name in pfr_means:
-            if np.isnan(sq_sems[name]) or np.isnan(pfr_sems[name]).any():
-                # Just relativize means
-                pfr_means[name] = [
-                    (mu / sq_means[name] - 1) * 100 for mu in pfr_means[name]
-                ]
-            else:
-                # Use delta method
-                pfr_means[name], pfr_sems[name] = relativize(
-                    means_t=pfr_means[name],
-                    sems_t=pfr_sems[name],
-                    mean_c=sq_means[name],
-                    sem_c=sq_sems[name],
-                    as_percent=True,
-                )
-        absolute_metrics = []
-    else:
-        absolute_metrics = obj_metr_list
-
+    # Get objective thresholds
+    rel_objth = {}
     objective_thresholds = {}
     if experiment.optimization_config.objective_thresholds is not None:  # pyre-ignore
         for objth in experiment.optimization_config.objective_thresholds:
-            is_rel = objth.metric.name not in absolute_metrics
-            if objth.relative != is_rel:
-                raise ValueError(
-                    f"Objective threshold for {objth.metric.name} has "
-                    f"rel={objth.relative} but was specified here as rel={is_rel}"
-                )
+            rel_objth[objth.metric.name] = objth.relative
             objective_thresholds[objth.metric.name] = objth.bound
 
+    # Identify which metrics should be relativized
+    if rel in [True, False]:
+        metric_is_rel = {name: rel for name in pfr_means}
+    else:
+        if len(rel_objth) != len(pfr_means):
+            raise UserInputError(
+                "At least one objective is missing an objective threshold. "
+                "`rel` must be specified as True or False when there are missing "
+                "objective thresholds."
+            )
+        # Default to however the threshold is specified
+        metric_is_rel = rel_objth
+
+    # Compute SQ values
+    sq_means, sq_sems = _extract_sq_data(experiment, data)
+
+    # Relativize data and thresholds as needed
+    for name in pfr_means:
+        if metric_is_rel[name]:
+            pfr_means[name], pfr_sems[name] = _relativize_values(
+                means=pfr_means[name],
+                sq_mean=sq_means[name],
+                sems=pfr_sems[name],
+                sq_sem=sq_sems[name],
+            )
+            if name in objective_thresholds and not rel_objth[name]:
+                # Metric is rel but obj th is not.
+                # Need to relativize the objective threshold
+                objective_thresholds[name] = _relativize_values(
+                    means=[objective_thresholds[name]],
+                    sq_mean=sq_means[name],
+                    sems=[np.nan],
+                    sq_sem=np.nan,
+                )[0][0]
+        elif name in objective_thresholds and rel_objth[name]:
+            # Metric is not rel but obj th is, so need to derelativize obj th
+            objective_thresholds[name] = (
+                1 + objective_thresholds[name] / 100.0
+            ) * sq_means[name]
+
+    absolute_metrics = [name for name, val in metric_is_rel.items() if not val]
     # Construct ParetoFrontResults for each pair
     pfr_list = []
     param_dicts = [obs.features.parameters for obs in pareto_observations]
     pfr_arm_names = [obs.arm_name for obs in pareto_observations]
 
     for metric_a, metric_b in combinations(obj_metr_list, 2):
         pfr_list.append(
@@ -264,43 +304,14 @@
                 pc.clone() for pc in search_space._parameter_constraints
             ],
         )
     else:
         return search_space
 
 
-# TODO: delete this function after merging with get_tensor_converter_model
-def pex_get_tensor_converter_model(
-    experiment: Experiment, data: Data
-) -> TorchModelBridge:
-    """
-    Copy of get_tensor_converter_model which retains the old transforms for pex usage
-
-    Args:
-        experiment: Experiment.
-        data: Data for fitting the model.
-
-    Returns: A torch modelbridge with transforms set.
-    """
-    # Transforms is the minimal set that will work for converting any search
-    # space to tensors.
-    return TorchModelBridge(
-        experiment=experiment,
-        search_space=to_nonrobust_search_space(experiment.search_space),
-        data=data,
-        model=TorchModel(),
-        transforms=[Derelativize, SearchSpaceToChoice, OrderedChoiceEncode, IntToFloat],
-        transform_configs={
-            "Derelativize": {"use_raw_status_quo": True},
-            "SearchSpaceToChoice": {"use_ordered": True},
-        },
-        fit_out_of_design=True,
-    )
-
-
 def get_tensor_converter_model(experiment: Experiment, data: Data) -> TorchModelBridge:
     """
     Constructs a minimal model for converting things to tensors.
 
     Model fitting will instantiate all of the transforms but will not do any
     expensive (i.e. GP) fitting beyond that. The model will raise an error if
     it is used for predicting or generating.
@@ -316,15 +327,15 @@
     # Transforms is the minimal set that will work for converting any search
     # space to tensors.
     return TorchModelBridge(
         experiment=experiment,
         search_space=to_nonrobust_search_space(experiment.search_space),
         data=data,
         model=TorchModel(),
-        transforms=[RemoveFixed, OrderedChoiceEncode, OneHot, IntToFloat],
+        transforms=[SearchSpaceToFloat],
         fit_out_of_design=True,
     )
 
 
 def compute_posterior_pareto_frontier(
     experiment: Experiment,
     primary_objective: Metric,
```

### Comparing `ax-platform-0.3.1/ax/plot/render.py` & `ax-platform-0.3.2/ax/plot/render.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/scatter.py` & `ax-platform-0.3.2/ax/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/slice.py` & `ax-platform-0.3.2/ax/plot/slice.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/table_view.py` & `ax-platform-0.3.2/ax/plot/table_view.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/long_running/test_pareto_utils.py` & `ax-platform-0.3.2/ax/plot/tests/long_running/test_pareto_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_contours.py` & `ax-platform-0.3.2/ax/plot/tests/test_contours.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_diagnostic.py` & `ax-platform-0.3.2/ax/plot/tests/test_diagnostic.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_feature_importances.py` & `ax-platform-0.3.2/ax/plot/tests/test_feature_importances.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_fitted_scatter.py` & `ax-platform-0.3.2/ax/plot/tests/test_fitted_scatter.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_helper.py` & `ax-platform-0.3.2/ax/plot/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_parallel_coordinates.py` & `ax-platform-0.3.2/ax/plot/tests/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_pareto_utils.py` & `ax-platform-0.3.2/ax/plot/tests/test_pareto_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 from ax.core.data import Data
 from ax.core.objective import MultiObjective, Objective
 from ax.core.observation import Observation, ObservationData, ObservationFeatures
 from ax.core.optimization_config import MultiObjectiveOptimizationConfig
 from ax.core.outcome_constraint import ObjectiveThreshold
 from ax.core.search_space import SearchSpace
 from ax.core.types import ComparisonOp
+from ax.exceptions.core import UserInputError
 from ax.metrics.branin import BraninMetric, NegativeBraninMetric
 from ax.modelbridge.registry import Models
-from ax.plot.pareto_frontier import interact_multiple_pareto_frontier
+from ax.plot.pareto_frontier import (
+    interact_multiple_pareto_frontier,
+    interact_pareto_frontier,
+)
 from ax.plot.pareto_utils import (
     _extract_observed_pareto_2d,
     get_observed_pareto_frontiers,
     infer_reference_point_from_experiment,
     to_nonrobust_search_space,
 )
 
@@ -44,15 +48,15 @@
         )
         sobol = Models.SOBOL(experiment.search_space)
         a = sobol.gen(5)
         experiment.new_batch_trial(generator_run=a).run()
         self.experiment = experiment
         self.metrics = list(experiment.metrics.values())
 
-    def testObservedParetoFrontiers(self) -> None:
+    def test_get_observed_pareto_frontiers(self) -> None:
         experiment = get_branin_experiment_with_multi_objective(
             with_batch=True, has_optimization_config=False, with_status_quo=True
         )
 
         # Optimization config is not optional
         with self.assertRaises(ValueError):
             get_observed_pareto_frontiers(experiment=experiment, data=Data())
@@ -73,20 +77,21 @@
             Objective(
                 metric=BraninMetric(
                     name="m3", param_names=["x1", "x2"], lower_is_better=True
                 ),
                 minimize=True,
             ),
         ]
-        bounds = [0, -100, 0]
+        bounds = [0, -100, 1000]
+        rels = [True, True, False]
         objective_thresholds = [
             ObjectiveThreshold(
                 metric=objective.metric,
                 bound=bounds[i],
-                relative=True,
+                relative=rels[i],
                 op=ComparisonOp.LEQ,
             )
             for i, objective in enumerate(objectives)
         ]
         objective = MultiObjective(objectives=objectives)
         optimization_config = MultiObjectiveOptimizationConfig(
             objective=objective,
@@ -111,47 +116,82 @@
         pfrs = get_observed_pareto_frontiers(experiment=experiment, data=data)
         # We have all pairs of metrics
         self.assertEqual(len(pfrs), 3)
         true_pairs = [("m1", "m2"), ("m1", "m3"), ("m2", "m3")]
         for i, pfr in enumerate(pfrs):
             self.assertEqual(pfr.primary_metric, true_pairs[i][0])
             self.assertEqual(pfr.secondary_metric, true_pairs[i][1])
-            self.assertEqual(pfr.absolute_metrics, [])
+            self.assertEqual(pfr.absolute_metrics, ["m3"])
             self.assertEqual(list(pfr.means.keys()), ["m1", "m2", "m3"])
             self.assertEqual(len(pfr.means["m1"]), len(pareto_arms))
             self.assertTrue(np.isnan(pfr.sems["m1"]).all())
-            # pyre-fixme[6]: For 1st param expected `Sized` but got
-            #  `Optional[List[Optional[str]]]`.
-            self.assertEqual(len(pfr.arm_names), len(pareto_arms))
+            self.assertEqual(len(pfr.arm_names), len(pareto_arms))  # pyre-ignore
+            self.assertEqual(
+                pfr.objective_thresholds, {"m1": 0, "m2": -100, "m3": 1000}
+            )
             arm_idx = np.argsort(pfr.arm_names)
             for i, idx in enumerate(arm_idx):
                 name = pareto_arms[i]
-                # pyre-fixme[16]: Optional type has no attribute `__getitem__`.
-                self.assertEqual(pfr.arm_names[idx], name)
+                self.assertEqual(pfr.arm_names[idx], name)  # pyre-ignore
                 self.assertEqual(
                     pfr.param_dicts[idx], experiment.arms_by_name[name].parameters
                 )
-
+        pfrs = get_observed_pareto_frontiers(experiment=experiment, data=data, rel=True)
+        pfr = pfrs[0]
+        self.assertEqual(pfr.absolute_metrics, [])
+        self.assertEqual(
+            pfr.objective_thresholds,
+            {"m1": 0, "m2": -100, "m3": (1000 / sq_val - 1) * 100},
+        )
+        pfrs = get_observed_pareto_frontiers(
+            experiment=experiment, data=data, rel=False
+        )
+        pfr = pfrs[0]
+        self.assertEqual(pfr.absolute_metrics, ["m1", "m2", "m3"])
+        self.assertEqual(pfr.objective_thresholds, {"m1": sq_val, "m2": 0, "m3": 1000})
         pfrs = get_observed_pareto_frontiers(
             experiment=experiment, data=data, arm_names=["0_1"]
         )
         for pfr in pfrs:
-            # pyre-fixme[58]: `in` is not supported for right operand type
-            #  `Optional[typing.List[typing.Optional[str]]]`.
-            self.assertTrue("status_quo" in pfr.arm_names)
+            self.assertTrue("status_quo" in pfr.arm_names)  # pyre-ignore
+
+        # Test with missing objective thresholds.
+        optimization_config._objective_thresholds = []
+        with self.assertRaisesRegex(UserInputError, "`rel` must be"):
+            get_observed_pareto_frontiers(experiment=experiment, data=data)
+        pfr = get_observed_pareto_frontiers(
+            experiment=experiment, data=data, rel=False
+        )[0]
+        self.assertEqual(pfr.absolute_metrics, ["m1", "m2", "m3"])
+        self.assertEqual(pfr.primary_metric, "m1")
+        self.assertEqual(pfr.secondary_metric, "m2")
+        self.assertEqual(len(pfr.means["m1"]), sum(df["metric_name"] == "m1"))
+        self.assertEqual(pfr.objective_thresholds, {})
+        pfr = get_observed_pareto_frontiers(experiment=experiment, data=data, rel=True)[
+            0
+        ]
+        self.assertEqual(pfr.absolute_metrics, [])
 
-    def testPlotMultipleParetoFrontiers(self) -> None:
+    def testPlotParetoFrontiers(self) -> None:
         experiment = get_branin_experiment_with_multi_objective(
             has_objective_thresholds=True,
         )
         sobol = Models.SOBOL(experiment.search_space)
         a = sobol.gen(5)
         experiment.new_batch_trial(generator_run=a).run()
         experiment.fetch_data()
         pfrs = get_observed_pareto_frontiers(experiment=experiment)
+        label_dict = {"branin_a": "a_new_metric"}
+        b = interact_pareto_frontier(pfrs, label_dict=label_dict)
+        self.assertEqual(
+            b.data["layout"]["updatemenus"][0]["buttons"][0]["label"],
+            "a_new_metric<br>vs branin_b",
+        )
+        self.assertEqual(b.data["layout"]["xaxis"]["title"]["text"], "branin_b")
+        self.assertEqual(b.data["layout"]["yaxis"]["title"]["text"], "a_new_metric")
         pfrs2 = copy.deepcopy(pfrs)
         pfr_lists = {"pfrs 1": pfrs, "pfrs 2": pfrs2}
         self.assertIsNotNone(interact_multiple_pareto_frontier(pfr_lists))
 
     def test_extract_observed_pareto_2d(self) -> None:
         Y = np.array([[1.0, 2.0], [2.1, 1.0], [1.0, 1.0], [2.0, 2.0], [3.0, 0.0]])
         reference_point = (1.5, 0.5)
```

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_slices.py` & `ax-platform-0.3.2/ax/plot/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_tile_fitted.py` & `ax-platform-0.3.2/ax/plot/tests/test_tile_fitted.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/tests/test_traces.py` & `ax-platform-0.3.2/ax/plot/tests/test_traces.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/plot/trace.py` & `ax-platform-0.3.2/ax/plot/trace.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/runners/simulated_backend.py` & `ax-platform-0.3.2/ax/runners/simulated_backend.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/runners/synthetic.py` & `ax-platform-0.3.2/ax/runners/synthetic.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/runners/tests/test_torchx.py` & `ax-platform-0.3.2/ax/runners/tests/test_torchx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/runners/torchx.py` & `ax-platform-0.3.2/ax/runners/torchx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/ax_client.py` & `ax-platform-0.3.2/ax/service/ax_client.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/interactive_loop.py` & `ax-platform-0.3.2/ax/service/interactive_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/managed_loop.py` & `ax-platform-0.3.2/ax/service/managed_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/scheduler.py` & `ax-platform-0.3.2/ax/service/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,17 +385,17 @@
             f"generation_strategy={self.generation_strategy}, options="
             f"{self.options})"
         )
 
     # ----------------- User-defined, optional. -----------------
 
     def completion_criterion(self) -> Tuple[bool, str]:
-        """Optional stopping criterion for optimization, which checks
-        of whether `total_trials` trials have been run and checks whether
-        the global_stopping_strategy suggests stopping the optimization.
+        """Optional stopping criterion for optimization, which checks whether
+        ``total_trials`` trials have been run or the ``global_stopping_strategy``
+        suggests stopping the optimization.
 
         Returns:
             A boolean representing whether the optimization should be stopped,
             and a string describing the reason for stopping.
         """
         if (
             not self.__ignore_global_stopping_strategy
@@ -418,22 +418,21 @@
                 objective_thresholds=self.__inferred_reference_point,
             )
             if stop_optimization:
                 return True, global_stopping_msg
 
         if self.options.total_trials is None:
             # We validate that `total_trials` is set in `run_all_trials`,
-            # so it will not run infinitely.
+            # so it will not run indefinitely.
             return False, ""
 
-        expecting_data = sum(  # Number of `RUNNING` + `COMPLETED` trials
-            1 for t in self.experiment.trials.values() if t.status.expecting_data
-        )
-        should_stop = expecting_data >= not_none(self.options.total_trials)
-        return should_stop, "Exceeding the total number of trials."
+        num_trials = len(self.experiment.trials)
+        should_stop = num_trials >= not_none(self.options.total_trials)
+        message = "Exceeding the total number of trials." if should_stop else ""
+        return should_stop, message
 
     @copy_doc(BestPointMixin.get_best_trial)
     def get_best_trial(
         self,
         optimization_config: Optional[OptimizationConfig] = None,
         trial_indices: Optional[Iterable[int]] = None,
         use_model_predictions: bool = True,
@@ -1299,19 +1298,14 @@
             ):
                 raise ValueError(
                     "Can only specify an early stopping strategy if at least one "
                     "metric is marked as `is_available_while_running`. Otherwise, we "
                     "will be unable to fetch intermediate results with which to "
                     "evaluate early stopping criteria."
                 )
-            if self.experiment.optimization_config is not None:
-                if self.experiment.optimization_config.is_moo_problem:
-                    raise UnsupportedError(
-                        "Early stopping is not supported on multi-objective problems."
-                    )
 
     def _get_max_pending_trials(self) -> int:
         return self.options.max_pending_trials
 
     def _prepare_trials(
         self, max_new_trials: int
     ) -> Tuple[List[BaseTrial], List[BaseTrial]]:
@@ -1667,50 +1661,50 @@
 
         results = self.experiment.fetch_trials_data_results(
             trial_indices=trial_indices, overwrite_existing_data=overwrite_existing_data
         )
 
         for trial_index, results_by_metric_name in results.items():
             for metric_name, result in results_by_metric_name.items():
-                # If the fetch call succeded continue.
+                # If the fetch call succeeded, continue.
                 if result.is_ok():
                     continue
 
-                self._num_metric_fetch_e_encountered += 1
-                metric_fetch_e = result.unwrap_err()
-
-                self._report_metric_fetch_e(
-                    trial=self.experiment.trials[trial_index],
-                    metric_name=metric_name,
-                    metric_fetch_e=metric_fetch_e,
-                )
-
                 # Log the Err so the user is aware that something has failed, even if
                 # we do not do anything
+                metric_fetch_e = result.unwrap_err()
                 self.logger.warning(
                     f"Failed to fetch {metric_name} for trial {trial_index}, found "
                     f"{metric_fetch_e}."
                 )
 
                 # If the metric is available while running just continue (we can try
                 # again later).
+                # NOTE: We don't need to report fetching errors in this case either
                 metric = self.experiment.metrics[metric_name]
                 status = self.experiment.trials[trial_index].status
                 if (
                     metric.is_available_while_running()
                     and status == TrialStatus.RUNNING
                 ):
                     self.logger.info(
                         f"MetricFetchE INFO: Because {metric_name} is "
                         f"available_while_running and trial {trial_index} is still "
                         "RUNNING continuing the experiment and retrying on next "
                         "poll..."
                     )
                     continue
 
+                self._num_metric_fetch_e_encountered += 1
+                self._report_metric_fetch_e(
+                    trial=self.experiment.trials[trial_index],
+                    metric_name=metric_name,
+                    metric_fetch_e=metric_fetch_e,
+                )
+
                 # If the fetch failure was for a metric in the optimization config (an
                 # objective or constraint) the trial as failed
                 optimization_config = self.experiment.optimization_config
                 if (
                     optimization_config is not None
                     and metric_name in optimization_config.metrics.keys()
                 ):
```

### Comparing `ax-platform-0.3.1/ax/service/tests/test_ax_client.py` & `ax-platform-0.3.2/ax/service/tests/test_ax_client.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/tests/test_best_point_utils.py` & `ax-platform-0.3.2/ax/service/tests/test_best_point_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/tests/test_early_stopping.py` & `ax-platform-0.3.2/ax/service/tests/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/tests/test_global_stopping.py` & `ax-platform-0.3.2/ax/service/tests/test_global_stopping.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/tests/test_instantiation_utils.py` & `ax-platform-0.3.2/ax/service/tests/test_instantiation_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from typing import Any, Dict
+
 from ax.core.metric import Metric
 from ax.core.optimization_config import MultiObjectiveOptimizationConfig
 from ax.core.parameter import FixedParameter, ParameterType, RangeParameter
 from ax.core.search_space import HierarchicalSearchSpace
 from ax.exceptions.core import UnsupportedError
 from ax.service.utils.instantiation import InstantiationBase
 from ax.utils.common.testutils import TestCase
@@ -60,14 +62,30 @@
         with self.assertRaisesRegex(ValueError, "Parameter constraint should"):
             InstantiationBase.constraint_from_str(
                 "x1 + x2 + x3 = 3",
                 # pyre-fixme[6]: For 2nd param expected `Dict[str, Parameter]` but
                 #  got `Dict[str, None]`.
                 {"x1": None, "x2": None, "x3": None},
             )
+        one_val_constraint = InstantiationBase.constraint_from_str(
+            "x1 <= 0",
+            # pyre-fixme[6]: For 2nd param expected `Dict[str, Parameter]` but
+            #  got `Dict[str, None]`.
+            {"x1": None, "x2": None},
+        )
+        self.assertEqual(one_val_constraint.bound, 0.0)
+        self.assertEqual(one_val_constraint.constraint_dict, {"x1": 1.0})
+        one_val_constraint = InstantiationBase.constraint_from_str(
+            "-0.5*x1 >= -0.1",
+            # pyre-fixme[6]: For 2nd param expected `Dict[str, Parameter]` but
+            #  got `Dict[str, None]`.
+            {"x1": None, "x2": None},
+        )
+        self.assertEqual(one_val_constraint.bound, 0.1)
+        self.assertEqual(one_val_constraint.constraint_dict, {"x1": 0.5})
         three_val_constaint2 = InstantiationBase.constraint_from_str(
             "-x1 + 2.1*x2 - 4*x3 <= 3",
             {
                 "x1": RangeParameter(
                     name="x1", parameter_type=ParameterType.FLOAT, lower=0.1, upper=4.0
                 ),
                 "x2": RangeParameter(
@@ -206,26 +224,29 @@
                 objective_thresholds=[],
                 outcome_constraints=[],
                 status_quo_defined=False,
             )
             self.assertEqual(single_optimization_config.objective.metric.name, "branin")
 
     def test_single_valued_choice_to_fixed_param_conversion(self) -> None:
-        representation = {
-            "name": "test",
-            "type": "choice",
-            "values": [1.0],
-        }
-        # pyre-fixme[6]: For 1st param expected `Dict[str, Union[None, Dict[str,
-        #  List[str]], List[Union[None, bool, float, int, str]], bool, float, int,
-        #  str]]` but got `Dict[str, Union[List[float], str]]`.
-        output = InstantiationBase.parameter_from_json(representation)
-        self.assertIsInstance(output, FixedParameter)
-        # pyre-fixme[16]: `Parameter` has no attribute `value`.
-        self.assertEqual(output.value, 1.0)
+        for use_dependents in [True, False]:
+            representation: Dict[str, Any] = {
+                "name": "test",
+                "type": "choice",
+                "values": [1.0],
+            }
+            if use_dependents:
+                representation["dependents"] = {1.0: ["foo_or_bar", "bazz"]}
+            output = checked_cast(
+                FixedParameter, InstantiationBase.parameter_from_json(representation)
+            )
+            self.assertIsInstance(output, FixedParameter)
+            self.assertEqual(output.value, 1.0)
+            if use_dependents:
+                self.assertEqual(output.dependents, {1.0: ["foo_or_bar", "bazz"]})
 
     def test_hss(self) -> None:
         parameter_dicts = [
             {
                 "name": "root",
                 "type": "fixed",
                 "value": "HierarchicalSearchSpace",
```

### Comparing `ax-platform-0.3.1/ax/service/tests/test_interactive_loop.py` & `ax-platform-0.3.2/ax/service/tests/test_interactive_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/tests/test_managed_loop.py` & `ax-platform-0.3.2/ax/service/tests/test_managed_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/tests/test_report_utils.py` & `ax-platform-0.3.2/ax/service/tests/test_report_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import itertools
 from collections import namedtuple
-from logging import WARN
+from logging import INFO, WARN
 from typing import Dict, List
 from unittest.mock import patch
 
 import pandas as pd
 from ax.core.arm import Arm
 from ax.core.metric import Metric
 from ax.core.objective import MultiObjective, Objective
@@ -320,20 +320,24 @@
                     experiment=exp, model=get_generation_strategy().model
                 )
             ),
             0,
         )
         exp = get_branin_experiment(with_batch=True, minimize=True)
         exp.trials[0].run()
-        plots = get_standard_plots(
-            experiment=exp,
-            model=Models.BOTORCH(experiment=exp, data=exp.fetch_data()),
-        )
-        self.assertEqual(len(plots), 6)
-        self.assertTrue(all(isinstance(plot, go.Figure) for plot in plots))
+        model = Models.BOTORCH(experiment=exp, data=exp.fetch_data())
+        for gsa in [False, True]:
+            with self.subTest(global_sensitivity_analysis=gsa):
+                plots = get_standard_plots(
+                    experiment=exp,
+                    model=model,
+                    global_sensitivity_analysis=gsa,
+                )
+                self.assertEqual(len(plots), 6)
+                self.assertTrue(all(isinstance(plot, go.Figure) for plot in plots))
 
     @fast_botorch_optimize
     def test_get_standard_plots_moo(self) -> None:
         exp = get_branin_experiment_with_multi_objective(with_batch=True)
         exp.optimization_config.objective.objectives[0].minimize = False
         exp.optimization_config.objective.objectives[1].minimize = True
         checked_cast(
@@ -343,24 +347,32 @@
                 metric=exp.metrics["branin_a"], op=ComparisonOp.GEQ, bound=-100.0
             ),
             ObjectiveThreshold(
                 metric=exp.metrics["branin_b"], op=ComparisonOp.LEQ, bound=100.0
             ),
         ]
         exp.trials[0].run()
-        with self.assertLogs(logger="ax", level=WARN) as log:
+        # NOTE: level set to INFO in this block, because the global sensitivity
+        # analysis raises an INFO level log entry here. Leaving level=WARN here
+        # actually passes on Python 3.8 because of a language internal bug. See
+        # https://bugs.python.org/issue41943 for more information.
+        with self.assertLogs(logger="ax", level=INFO) as log:
             plots = get_standard_plots(
                 experiment=exp, model=Models.MOO(experiment=exp, data=exp.fetch_data())
             )
-            self.assertEqual(len(log.output), 1)
+            self.assertEqual(len(log.output), 2)
             self.assertIn(
                 "Pareto plotting not supported for experiments with relative objective "
                 "thresholds.",
                 log.output[0],
             )
+            self.assertIn(
+                "Failed to compute global feature sensitivities:",
+                log.output[1],
+            )
         self.assertEqual(len(plots), 6)
 
     @fast_botorch_optimize
     def test_get_standard_plots_moo_relative_constraints(self) -> None:
         exp = get_branin_experiment_with_multi_objective(with_batch=True)
         exp.optimization_config.objective.objectives[0].minimize = False
         exp.optimization_config.objective.objectives[1].minimize = True
```

### Comparing `ax-platform-0.3.1/ax/service/tests/test_scheduler.py` & `ax-platform-0.3.2/ax/service/tests/test_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # LICENSE file in the root directory of this source tree.
 
 import os
 from logging import WARNING
 from math import ceil
 from random import randint
 from tempfile import NamedTemporaryFile
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Tuple
-from unittest.mock import patch
+from typing import Any, Callable, Dict, Iterable, Optional, Set
+from unittest.mock import Mock, patch
 
 from ax.core.arm import Arm
 from ax.core.base_trial import BaseTrial, TrialStatus
 from ax.core.experiment import Experiment
 from ax.core.metric import Metric
 from ax.core.objective import Objective
 from ax.core.optimization_config import OptimizationConfig
@@ -54,14 +54,15 @@
     DummyGlobalStoppingStrategy,
     get_branin_experiment,
     get_branin_experiment_with_multi_objective,
     get_branin_experiment_with_timestamp_map_metric,
     get_branin_multi_objective_optimization_config,
     get_branin_search_space,
     get_generator_run,
+    get_sobol,
 )
 
 from pyre_extensions import none_throws
 
 from sqlalchemy.orm.exc import StaleDataError
 
 
@@ -81,21 +82,15 @@
 
 
 class TestScheduler(Scheduler):
     """Test scheduler that only implements ``report_results`` for convenience in
     testing.
     """
 
-    # pyre-fixme[15]: `report_results` overrides method defined in `Scheduler`
-    #  inconsistently.
-    def report_results(
-        self, force_refit: bool = False
-    ) -> Tuple[bool, Dict[str, Set[int]]]:
-        # pyre-fixme[7]: Expected `Tuple[bool, Dict[str, Set[int]]]` but got
-        #  `Dict[str, Set[int]]`.
+    def report_results(self, force_refit: bool = False) -> Dict[str, Any]:
         return {
             # Use `set` constructor to copy the set, else the value
             # will be a pointer and all will be the same.
             "trials_completed_so_far": set(
                 self.experiment.trial_indices_by_status[TrialStatus.COMPLETED]
             ),
             "trials_early_stopped_so_far": set(
@@ -103,16 +98,17 @@
             ),
         }
 
 
 class EarlyStopsInsteadOfNormalCompletionScheduler(TestScheduler):
     """Test scheduler that marks all trials as ones that should be early-stopped."""
 
-    # pyre-fixme[3]: Return type must be annotated.
-    def should_stop_trials_early(self, trial_indices: Set[int]):
+    def should_stop_trials_early(
+        self, trial_indices: Set[int]
+    ) -> Dict[int, Optional[str]]:
         return {i: None for i in trial_indices}
 
 
 # ---- Runners below simulate different usage and failure modes for scheduler ----
 
 
 class RunnerWithFrequentFailedTrials(SyntheticRunner):
@@ -146,24 +142,26 @@
         if randint(0, 3) > 0:
             running = [t.index for t in trials]
             return {TrialStatus.COMPLETED: {running[randint(0, len(running) - 1)]}}
         return {}
 
 
 class InfinitePollRunner(SyntheticRunner):
-    # pyre-fixme[3]: Return type must be annotated.
-    def poll_trial_status(self, trials: Iterable[BaseTrial]):
+    def poll_trial_status(
+        self, trials: Iterable[BaseTrial]
+    ) -> Dict[TrialStatus, Set[int]]:
         return {}
 
 
 class RunnerWithEarlyStoppingStrategy(SyntheticRunner):
     poll_trial_status_count = 0
 
-    # pyre-fixme[3]: Return type must be annotated.
-    def poll_trial_status(self, trials: Iterable[BaseTrial]):
+    def poll_trial_status(
+        self, trials: Iterable[BaseTrial]
+    ) -> Dict[TrialStatus, Set[int]]:
         self.poll_trial_status_count += 1
 
         # In the first step, don't complete any trials
         # Trial #1 will be early stopped
         if self.poll_trial_status_count == 1:
             return {}
 
@@ -173,32 +171,24 @@
         return {TrialStatus.COMPLETED: {0}}
 
 
 class BrokenRunnerValueError(SyntheticRunnerWithStatusPolling):
 
     run_trial_call_count = 0
 
-    # pyre-fixme[14]: `run_multiple` overrides method defined in `Runner`
-    #  inconsistently.
-    # pyre-fixme[15]: `run_multiple` overrides method defined in `Runner`
-    #  inconsistently.
-    def run_multiple(self, trials: List[BaseTrial]) -> Dict[str, Any]:
+    def run_multiple(self, trials: Iterable[BaseTrial]) -> Dict[int, Dict[str, Any]]:
         self.run_trial_call_count += 1
         raise ValueError("Failing for testing purposes.")
 
 
 class BrokenRunnerRuntimeError(SyntheticRunnerWithStatusPolling):
 
     run_trial_call_count = 0
 
-    # pyre-fixme[14]: `run_multiple` overrides method defined in `Runner`
-    #  inconsistently.
-    # pyre-fixme[15]: `run_multiple` overrides method defined in `Runner`
-    #  inconsistently.
-    def run_multiple(self, trials: List[BaseTrial]) -> Dict[str, Any]:
+    def run_multiple(self, trials: Iterable[BaseTrial]) -> Dict[int, Dict[str, Any]]:
         self.run_trial_call_count += 1
         raise RuntimeError("Failing for testing purposes.")
 
 
 class TestAxScheduler(TestCase):
     """Tests base `Scheduler` functionality."""
 
@@ -322,44 +312,28 @@
                 experiment=self.branin_experiment,
                 generation_strategy=self.sobol_GPEI_GS,
                 options=SchedulerOptions(
                     early_stopping_strategy=DummyEarlyStoppingStrategy()
                 ),
             )
 
-        with patch.object(
-            OptimizationConfig, "is_moo_problem", return_value=True
-        ), self.assertRaisesRegex(
-            UnsupportedError,
-            "Early stopping is not supported on multi-objective problems",
-        ):
-            Scheduler(
-                experiment=self.branin_experiment,
-                generation_strategy=self.sobol_GPEI_GS,
-                options=SchedulerOptions(
-                    early_stopping_strategy=DummyEarlyStoppingStrategy()
-                ),
-            )
-
         # should not error
         Scheduler(
             experiment=self.branin_experiment,
             generation_strategy=self.sobol_GPEI_GS,
             options=SchedulerOptions(
                 early_stopping_strategy=DummyEarlyStoppingStrategy()
             ),
         )
 
     @patch(
         f"{GenerationStrategy.__module__}.GenerationStrategy._gen_multiple",
         return_value=[get_generator_run()],
     )
-    # pyre-fixme[3]: Return type must be annotated.
-    # pyre-fixme[2]: Parameter must be annotated.
-    def test_run_multi_arm_generator_run_error(self, mock_gen):
+    def test_run_multi_arm_generator_run_error(self, mock_gen: Mock) -> None:
         scheduler = Scheduler(
             experiment=self.branin_experiment,
             generation_strategy=self.sobol_GPEI_GS,
             options=SchedulerOptions(total_trials=1),
         )
         with self.assertRaisesRegex(SchedulerInternalError, ".* only one was expected"):
             scheduler.run_all_trials()
@@ -368,17 +342,17 @@
         # Record calls to function, but still execute it.
         (
             f"{Scheduler.__module__}."
             "get_pending_observation_features_based_on_trial_status"
         ),
         side_effect=get_pending_observation_features_based_on_trial_status,
     )
-    # pyre-fixme[3]: Return type must be annotated.
-    # pyre-fixme[2]: Parameter must be annotated.
-    def test_run_all_trials_using_runner_and_metrics(self, mock_get_pending):
+    def test_run_all_trials_using_runner_and_metrics(
+        self, mock_get_pending: Mock
+    ) -> None:
         # With runners & metrics, `Scheduler.run_all_trials` should run.
         scheduler = Scheduler(
             experiment=self.branin_experiment,  # Has runner and metrics.
             generation_strategy=self.two_sobol_steps_GS,
             options=SchedulerOptions(
                 total_trials=8,
                 # pyre-fixme[6]: For 2nd param expected `Optional[int]` but got `float`.
@@ -436,17 +410,19 @@
         def write_n_trials(scheduler: Scheduler) -> None:
             trials_info["n_completed"] = len(scheduler.experiment.trials)
 
         self.assertTrue(trials_info["n_completed"] == 0)
         scheduler.run_all_trials(idle_callback=write_n_trials)
         self.assertTrue(trials_info["n_completed"] == n_total_trials)
 
-    # pyre-fixme[3]: Return type must be annotated.
-    # pyre-fixme[2]: Parameter annotation cannot contain `Any`.
-    def base_run_n_trials(self, idle_callback: Optional[Callable[[Scheduler], Any]]):
+    def base_run_n_trials(
+        self,
+        # pyre-fixme[2]: Parameter annotation cannot contain `Any`.
+        idle_callback: Optional[Callable[[Scheduler], Any]],
+    ) -> None:
         # With runners & metrics, `Scheduler.run_all_trials` should run.
         scheduler = Scheduler(
             experiment=self.branin_experiment,  # Has runner and metrics.
             generation_strategy=self.two_sobol_steps_GS,
             options=SchedulerOptions(
                 # pyre-fixme[6]: For 1st param expected `Optional[int]` but got `float`.
                 init_seconds_between_polls=0.1,  # Short between polls so test is fast.
@@ -974,16 +950,15 @@
         )
         self.assertEqual(scheduler.run_n_trials(max_trials=3), OptimizationResult())
 
     @patch(
         f"{GenerationStrategy.__module__}.GenerationStrategy._gen_multiple",
         side_effect=OptimizationComplete("test error"),
     )
-    # pyre-fixme[3]: Return type must be annotated.
-    def test_optimization_complete(self, _):
+    def test_optimization_complete(self, _) -> None:
         # With runners & metrics, `Scheduler.run_all_trials` should run.
         scheduler = Scheduler(
             experiment=self.branin_experiment,  # Has runner and metrics.
             generation_strategy=self.two_sobol_steps_GS,
             options=SchedulerOptions(
                 max_pending_trials=100,
                 # pyre-fixme[6]: For 2nd param expected `Optional[int]` but got `float`.
@@ -999,17 +974,15 @@
             f"{WithDBSettingsBase.__module__}.WithDBSettingsBase."
             "_save_generation_strategy_to_db_if_possible"
         )
     )
     @patch(
         f"{WithDBSettingsBase.__module__}._save_experiment", side_effect=StaleDataError
     )
-    # pyre-fixme[3]: Return type must be annotated.
-    # pyre-fixme[2]: Parameter must be annotated.
-    def test_suppress_all_storage_errors(self, mock_save_exp, _):
+    def test_suppress_all_storage_errors(self, mock_save_exp: Mock, _) -> None:
         init_test_engine_and_session_factory(force_init=True)
         config = SQAConfig()
         encoder = Encoder(config=config)
         decoder = Decoder(config=config)
         db_settings = DBSettings(encoder=encoder, decoder=decoder)
         Scheduler(
             experiment=self.branin_experiment,  # Has runner and metrics.
@@ -1190,7 +1163,37 @@
                 any(
                     "Because branin is an objective, marking trial 0 as "
                     "TrialStatus.FAILED" in warning
                     for warning in lg.output
                 )
             )
             self.assertEqual(scheduler.experiment.trials[0].status, TrialStatus.FAILED)
+
+    def test_completion_criterion(self) -> None:
+        # Tests non-GSS parts of the completion criterion.
+        scheduler = Scheduler(
+            experiment=self.branin_experiment,
+            generation_strategy=self.sobol_GPEI_GS,
+            options=SchedulerOptions(
+                total_trials=None,
+            ),
+        )
+        # With total_trials=None.
+        should_stop, message = scheduler.completion_criterion()
+        self.assertFalse(should_stop)
+        self.assertEqual(message, "")
+
+        # With total_trials=5.
+        scheduler.options = SchedulerOptions(total_trials=5)
+        # Experiment has fewer trials.
+        should_stop, message = scheduler.completion_criterion()
+        self.assertFalse(should_stop)
+        self.assertEqual(message, "")
+        # Experiment has 5 trials.
+        sobol_generator = get_sobol(search_space=self.branin_experiment.search_space)
+        for _ in range(5):
+            sobol_run = sobol_generator.gen(n=1)
+            self.branin_experiment.new_trial(generator_run=sobol_run)
+        self.assertEqual(len(self.branin_experiment.trials), 5)
+        should_stop, message = scheduler.completion_criterion()
+        self.assertTrue(should_stop)
+        self.assertEqual(message, "Exceeding the total number of trials.")
```

### Comparing `ax-platform-0.3.1/ax/service/tests/test_with_db_settings_base.py` & `ax-platform-0.3.2/ax/service/tests/test_with_db_settings_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/utils/best_point.py` & `ax-platform-0.3.2/ax/service/utils/best_point.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/utils/best_point_mixin.py` & `ax-platform-0.3.2/ax/service/utils/best_point_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,16 +395,17 @@
 
         # Derelativize the optimization config.
         tf = Derelativize(
             search_space=None, observations=None, config={"use_raw_status_quo": True}
         )
         optimization_config = tf.transform_optimization_config(
             optimization_config=optimization_config.clone(),
-            # pyre-ignore -- experiment works here since we only need the status quo.
-            modelbridge=experiment,
+            modelbridge=get_tensor_converter_model(
+                experiment=experiment, data=experiment.lookup_data()
+            ),
             fixed_features=None,
         )
 
         # Extract weights, constraints, and objective_thresholds.
         objective_weights = extract_objective_weights(
             objective=optimization_config.objective, outcomes=metric_names
         )
```

### Comparing `ax-platform-0.3.1/ax/service/utils/early_stopping.py` & `ax-platform-0.3.2/ax/service/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/utils/instantiation.py` & `ax-platform-0.3.2/ax/service/utils/instantiation.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,18 +283,14 @@
 
         if parameter_class == "choice":
             assert (
                 "values" in representation
             ), "Values are required for choice parameters."
             values = representation["values"]
             if isinstance(values, list) and len(values) == 1:
-                if representation.get("dependents"):
-                    raise NotImplementedError(
-                        "Support for hierarchical fixed parameters coming soon."
-                    )
                 logger.info(
                     f"Choice parameter {name} contains only one value, converting to a"
                     + " fixed parameter instead."
                 )
                 # update the representation to a fixed parameter class
                 parameter_class = "fixed"
                 representation["type"] = parameter_class
@@ -322,28 +318,34 @@
     @staticmethod
     def constraint_from_str(
         representation: str, parameters: Dict[str, Parameter]
     ) -> ParameterConstraint:
         """Parse string representation of a parameter constraint."""
         tokens = representation.split()
         parameter_names = parameters.keys()
+        try:
+            float(tokens[-1])
+            last_token_is_numeric = True
+        except ValueError:
+            last_token_is_numeric = False
         order_const = len(tokens) == 3 and tokens[1] in COMPARISON_OPS
         sum_const = (
             len(tokens) >= 5 and len(tokens) % 2 == 1 and tokens[-2] in COMPARISON_OPS
         )
         if not (order_const or sum_const):
             raise ValueError(
                 "Parameter constraint should be of form <parameter_name> >= "
                 "<other_parameter_name> for order constraints or `<parameter_name> "
                 "+ <other_parameter_name> >= x, where any number of terms can be "
                 "added and `x` is a float bound. Acceptable comparison operators "
                 'are ">=" and "<=".'
             )
 
-        if len(tokens) == 3:  # Case "x1 >= x2" => order constraint.
+        # Case "x1 >= x2" => order constraint.
+        if len(tokens) == 3 and not last_token_is_numeric:
             left, right = tokens[0], tokens[2]
             assert (
                 left in parameter_names
             ), f"Parameter {left} not in {parameter_names}."
             assert (
                 right in parameter_names
             ), f"Parameter {right} not in {parameter_names}."
@@ -352,33 +354,34 @@
                     lower_parameter=parameters[left], upper_parameter=parameters[right]
                 )
                 if COMPARISON_OPS[tokens[1]] is ComparisonOp.LEQ
                 else OrderConstraint(
                     lower_parameter=parameters[right], upper_parameter=parameters[left]
                 )
             )
-        try:  # Case "x1 - 2*x2 + x3 >= 2" => parameter constraint.
-            bound = float(tokens[-1])
-        except ValueError:
+        if not last_token_is_numeric:
             raise ValueError(
                 f"Bound for the constraint must be a number; got {tokens[-1]}"
             )
+        bound = float(tokens[-1])
         if any(token[0] == "*" or token[-1] == "*" for token in tokens):
             raise ValueError(
                 "A linear constraint should be the form a*x + b*y - c*z <= d"
                 ", where a,b,c,d are float constants and x,y,z are parameters. "
                 "There should be no space in each term around the operator * while "
                 "there should be a single space around each operator +, -, <= and >=."
             )
         parameter_weight = {}
         comparison_multiplier = (
             1.0 if COMPARISON_OPS[tokens[-2]] is ComparisonOp.LEQ else -1.0
         )
         operator_sign = 1.0  # Determines whether the operator is + or -
+        # tokens are alternating monomials and operators
         for idx, token in enumerate(tokens[:-2]):
+            # for monomials
             if idx % 2 == 0:
                 split_token = token.split("*")
                 parameter = ""  # Initializing the parameter
                 multiplier = 1.0  # Initializing the multiplier
                 if len(split_token) == 2:  # There is a non-unit multiplier
                     try:
                         multiplier = float(split_token[0])
@@ -394,14 +397,15 @@
                         multiplier = -1.0
                     else:
                         multiplier = 1.0
                 assert (
                     parameter in parameter_names
                 ), f"Parameter {parameter} not in {parameter_names}."
                 parameter_weight[parameter] = operator_sign * multiplier
+            # for operators
             else:
                 assert (
                     token == "+" or token == "-"
                 ), f"Expected a mixed constraint, found operator {token}."
                 operator_sign = 1.0 if token == "+" else -1.0
         return ParameterConstraint(
             constraint_dict={
```

### Comparing `ax-platform-0.3.1/ax/service/utils/report_utils.py` & `ax-platform-0.3.2/ax/service/utils/report_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,23 +27,24 @@
 import pandas as pd
 import plotly.graph_objects as go
 from ax.core.base_trial import TrialStatus
 from ax.core.data import Data
 from ax.core.experiment import Experiment
 from ax.core.generator_run import GeneratorRunType
 from ax.core.map_data import MapData
+from ax.core.map_metric import MapMetric
 from ax.core.metric import Metric
 from ax.core.multi_type_experiment import MultiTypeExperiment
 from ax.core.objective import MultiObjective, ScalarizedObjective
 from ax.core.trial import BaseTrial
 from ax.early_stopping.strategies.base import BaseEarlyStoppingStrategy
 from ax.exceptions.core import UserInputError
-from ax.metrics.curve import AbstractCurveMetric
 from ax.modelbridge import ModelBridge
 from ax.modelbridge.cross_validation import cross_validate
+from ax.modelbridge.torch import TorchModelBridge
 from ax.plot.contour import interact_contour_plotly
 from ax.plot.diagnostic import interact_cross_validation_plotly
 from ax.plot.feature_importances import plot_feature_importance_by_feature_plotly
 from ax.plot.helper import get_range_parameters_from_list
 from ax.plot.pareto_frontier import (
     _pareto_frontier_plot_input_processing,
     _validate_experiment_and_get_optimization_config,
@@ -57,14 +58,15 @@
     map_data_multiple_metrics_dropdown_plotly,
     optimization_trace_single_method_plotly,
 )
 from ax.service.utils.best_point import _derel_opt_config_wrapper, _is_row_feasible
 from ax.service.utils.early_stopping import get_early_stopping_metrics
 from ax.utils.common.logger import get_logger
 from ax.utils.common.typeutils import checked_cast, not_none
+from ax.utils.sensitivity.sobol_measures import ax_parameter_sens
 from pandas.core.frame import DataFrame
 
 if TYPE_CHECKING:
     from ax.service.scheduler import Scheduler
 
 
 logger: Logger = get_logger(__name__)
@@ -141,16 +143,16 @@
 
     return [plot for plot in plots if plot is not None]
 
 
 def _get_objective_v_param_plots(
     experiment: Experiment,
     model: ModelBridge,
-    max_num_slice_plots: int = 100,
-    max_num_contour_plots: int = 100,
+    max_num_slice_plots: int = 50,
+    max_num_contour_plots: int = 20,
 ) -> List[go.Figure]:
     search_space = experiment.search_space
 
     range_params = get_range_parameters_from_list(
         list(search_space.range_parameters.values()), min_num_values=5
     )
     if len(range_params) < 1:
@@ -280,14 +282,15 @@
     experiment: Experiment,
     model: Optional[ModelBridge],
     data: Optional[Data] = None,
     model_transitions: Optional[List[int]] = None,
     true_objective_metric_name: Optional[str] = None,
     early_stopping_strategy: Optional[BaseEarlyStoppingStrategy] = None,
     limit_points_per_plot: Optional[int] = None,
+    global_sensitivity_analysis: bool = True,
 ) -> List[go.Figure]:
     """Extract standard plots for single-objective optimization.
 
     Extracts a list of plots from an ``Experiment`` and ``ModelBridge`` of general
     interest to an Ax user. Currently not supported are
     - TODO: multi-objective optimization
     - TODO: ChoiceParameter plots
@@ -299,15 +302,17 @@
         - model_transitions: The arm numbers at which shifts in generation_strategy
             occur.
         - true_objective_metric_name: Name of the metric to use as the true objective.
         - early_stopping_strategy: Early stopping strategy used throughout the
             experiment; used for visualizing when curves are stopped.
         - limit_points_per_plot: Limit the number of points used per metric in
             each curve plot. Passed to `_get_curve_plot_dropdown`.
-
+        - global_sensitivity_analysis: If True, plot total Sobol indices for the model
+            parameters. If False, plot sensitivities based on GP kernel lengthscales.
+            Defaults to True.
     Returns:
         - a plot of objective value vs. trial index, to show experiment progression
         - a plot of objective value vs. range parameter values, only included if the
           model associated with generation_strategy can create predictions. This
           consists of:
 
             - a plot_slice plot if the search space contains one range parameter
@@ -375,42 +380,57 @@
             output_plot_list.extend(
                 _get_objective_v_param_plots(
                     experiment=experiment,
                     model=model,
                 )
             )
             output_plot_list.extend(_get_cross_validation_plots(model=model))
+
+            # sensitivity plot
+            sens = None
+            importance_measure = ""
+            if global_sensitivity_analysis and isinstance(model, TorchModelBridge):
+                try:
+                    sens = ax_parameter_sens(model, order="total")
+                    importance_measure = "Total Sobol Indices"
+                except NotImplementedError as e:
+                    logger.info(f"Failed to compute global feature sensitivities: {e}")
             feature_importance_plot = plot_feature_importance_by_feature_plotly(
-                model=model, relative=False, caption=FEATURE_IMPORTANCE_CAPTION
+                model=model,
+                # pyre-ignore [6]: In call for argument `sensitivity_values`,
+                # expected `Optional[Dict[str, Dict[str, Union[float, ndarray]]]]`
+                # but got `Dict[str, Dict[str, ndarray]]`.
+                sensitivity_values=sens,
+                relative=False,
+                caption=FEATURE_IMPORTANCE_CAPTION if importance_measure == "" else "",
+                importance_measure=importance_measure,
             )
             feature_importance_plot.layout.title = "[ADVANCED] " + str(
                 # pyre-fixme[16]: go.Figure has no attribute `layout`
                 feature_importance_plot.layout.title.text
             )
             output_plot_list.append(feature_importance_plot)
             output_plot_list.append(interact_fitted_plotly(model=model, rel=False))
         except NotImplementedError:
             # Model does not implement `predict` method.
             pass
 
-    # Get plots for AbstractCurveMetrics
-    curve_metrics = [
-        m for m in experiment.metrics.values() if isinstance(m, AbstractCurveMetric)
-    ]
-    if curve_metrics:
+    # Get plots for MapMetrics
+    map_metrics = [m for m in experiment.metrics.values() if isinstance(m, MapMetric)]
+    if map_metrics:
         # Sort so that objective metrics appear first
-        curve_metrics.sort(
+        map_metrics.sort(
             key=lambda e: e.name in [m.name for m in objective.metrics],
             reverse=True,
         )
         for by_walltime in [False, True]:
             output_plot_list.append(
                 _get_curve_plot_dropdown(
                     experiment=experiment,
-                    curve_metrics=curve_metrics,
+                    map_metrics=map_metrics,
                     data=data,  # pyre-ignore
                     early_stopping_strategy=early_stopping_strategy,
                     by_walltime=by_walltime,
                     limit_points_per_plot=limit_points_per_plot,
                 )
             )
     return [plot for plot in output_plot_list if plot is not None]
@@ -432,25 +452,25 @@
     except Exception as e:
         logger.info(f"Failed to transform progression to walltime: {e}")
         return None
 
 
 def _get_curve_plot_dropdown(
     experiment: Experiment,
-    curve_metrics: Iterable[AbstractCurveMetric],
+    map_metrics: Iterable[MapMetric],
     data: MapData,
     early_stopping_strategy: Optional[BaseEarlyStoppingStrategy],
     by_walltime: bool = False,
     limit_points_per_plot: Optional[int] = None,
 ) -> Optional[go.Figure]:
     """Plot curve metrics by either progression or walltime.
 
     Args:
         experiment: The experiment to generate plots for.
-        curve_metrics: The list of metrics to generate plots for. Each metric
+        map_metrics: The list of metrics to generate plots for. Each metric
             will be one entry in the dropdown.
         data: The map data used to generate the plots.
         early_stopping_strategy: An instance of ``BaseEarlyStoppingStrategy``. This
             is used to check which metrics are being used for early stopping.
         by_walltime: If true, the x-axis will be walltime. If false, the x-axis is
             the progression of the trials (trials are 'stacked').
         limit_points_per_plot: Limit the total number of data points used per plot
@@ -467,16 +487,16 @@
     exp_df = pd.DataFrame()
     if by_walltime:
         exp_df = exp_to_df(
             exp=experiment,
             trial_attribute_fields=["time_run_started", "time_completed"],
             always_include_field_columns=True,
         )
-    for m in curve_metrics:
-        map_key = m.MAP_KEY.key
+    for m in map_metrics:
+        map_key = m.map_key_info.key
         subsampled_data = (
             data
             if limit_points_per_plot is None
             else data.subsample(
                 limit_rows_per_metric=limit_points_per_plot, map_key=map_key
             )
         )
@@ -519,24 +539,25 @@
 
     title = (
         "Curve metrics (i.e., learning curves) by walltime"
         if by_walltime
         else "Curve metrics (i.e., learning curves) by progression"
     )
     return map_data_multiple_metrics_dropdown_plotly(
-        metric_names=[m.name for m in curve_metrics],
+        metric_names=[m.name for m in map_metrics],
         xs_by_metric=xs_by_metric,
         ys_by_metric=ys_by_metric,
         legend_labels_by_metric=legend_labels_by_metric,
         stopping_markers_by_metric=stopping_markers_by_metric,
         title=title,
         xlabels_by_metric={
-            m.name: "wall time" if by_walltime else m.MAP_KEY.key for m in curve_metrics
+            m.name: "wall time" if by_walltime else m.map_key_info.key
+            for m in map_metrics
         },
-        lower_is_better_by_metric={m.name: m.lower_is_better for m in curve_metrics},
+        lower_is_better_by_metric={m.name: m.lower_is_better for m in map_metrics},
     )
 
 
 def _merge_trials_dict_with_df(
     df: pd.DataFrame,
     # pyre-fixme[2]: Parameter annotation cannot contain `Any`.
     trials_dict: Dict[int, Any],
```

### Comparing `ax-platform-0.3.1/ax/service/utils/scheduler_options.py` & `ax-platform-0.3.2/ax/service/utils/scheduler_options.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/service/utils/with_db_settings_base.py` & `ax-platform-0.3.2/ax/service/utils/with_db_settings_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/botorch_modular_registry.py` & `ax-platform-0.3.2/ax/storage/botorch_modular_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/decoder.py` & `ax-platform-0.3.2/ax/storage/json_store/decoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/decoders.py` & `ax-platform-0.3.2/ax/storage/json_store/decoders.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/encoder.py` & `ax-platform-0.3.2/ax/storage/json_store/encoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/encoders.py` & `ax-platform-0.3.2/ax/storage/json_store/encoders.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/load.py` & `ax-platform-0.3.2/ax/storage/json_store/load.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/registry.py` & `ax-platform-0.3.2/ax/storage/json_store/registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/save.py` & `ax-platform-0.3.2/ax/storage/json_store/save.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/json_store/tests/test_json_store.py` & `ax-platform-0.3.2/ax/storage/json_store/tests/test_json_store.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/metric_registry.py` & `ax-platform-0.3.2/ax/storage/metric_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/registry_bundle.py` & `ax-platform-0.3.2/ax/storage/registry_bundle.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/runner_registry.py` & `ax-platform-0.3.2/ax/storage/runner_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/__init__.py` & `ax-platform-0.3.2/ax/storage/sqa_store/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/db.py` & `ax-platform-0.3.2/ax/storage/sqa_store/db.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/decoder.py` & `ax-platform-0.3.2/ax/storage/sqa_store/decoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/delete.py` & `ax-platform-0.3.2/ax/storage/sqa_store/delete.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/encoder.py` & `ax-platform-0.3.2/ax/storage/sqa_store/encoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/json.py` & `ax-platform-0.3.2/ax/storage/sqa_store/json.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/load.py` & `ax-platform-0.3.2/ax/storage/sqa_store/load.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/reduced_state.py` & `ax-platform-0.3.2/ax/storage/sqa_store/reduced_state.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/save.py` & `ax-platform-0.3.2/ax/storage/sqa_store/save.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/sqa_classes.py` & `ax-platform-0.3.2/ax/storage/sqa_store/sqa_classes.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/sqa_config.py` & `ax-platform-0.3.2/ax/storage/sqa_store/sqa_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/sqa_enum.py` & `ax-platform-0.3.2/ax/storage/sqa_store/sqa_enum.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/structs.py` & `ax-platform-0.3.2/ax/storage/sqa_store/structs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/tests/test_sqa_store.py` & `ax-platform-0.3.2/ax/storage/sqa_store/tests/test_sqa_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
         side_effect=Decoder(SQAConfig()).trial_from_sqa,
     )
     # pyre-fixme[56]: Pyre was not able to infer the type of argument `ax.storage.sqa...
     @patch(
         f"{Decoder.__module__}.Decoder.experiment_from_sqa",
         side_effect=Decoder(SQAConfig()).experiment_from_sqa,
     )
-    def testExperimentSaveAndLoadReducedState(
+    def test_ExperimentSaveAndLoadReducedState(
         self, _mock_exp_from_sqa, _mock_trial_from_sqa, _mock_gr_from_sqa
     ) -> None:
         # 1. No abandoned arms + no trials case, reduced state should be the
         # same as non-reduced state.
         exp = get_experiment_with_multi_objective()
         save_experiment(exp)
         loaded_experiment = load_experiment(exp.name, reduced_state=True)
@@ -312,15 +312,15 @@
         # scramble, generated_points, fallback_to_sample_polytope)
         # and the rest of model-state info on generator run to have values too.
         mkw = gr._model_kwargs
         self.assertIsNotNone(mkw)
         self.assertEqual(len(mkw), 6)
         bkw = gr._bridge_kwargs
         self.assertIsNotNone(bkw)
-        self.assertEqual(len(bkw), 7)
+        self.assertEqual(len(bkw), 8)
         ms = gr._model_state_after_gen
         self.assertIsNotNone(ms)
         self.assertEqual(len(ms), 2)
         gm = gr._gen_metadata
         self.assertIsNotNone(gm)
         self.assertEqual(len(gm), 0)
         self.assertIsNotNone(gr._search_space, gr.optimization_config)
```

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/tests/test_utils.py` & `ax-platform-0.3.2/ax/storage/sqa_store/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/tests/utils.py` & `ax-platform-0.3.2/ax/storage/sqa_store/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/timestamp.py` & `ax-platform-0.3.2/ax/storage/sqa_store/timestamp.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/utils.py` & `ax-platform-0.3.2/ax/storage/sqa_store/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/sqa_store/validation.py` & `ax-platform-0.3.2/ax/storage/sqa_store/validation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/tests/test_registry_bundle.py` & `ax-platform-0.3.2/ax/storage/tests/test_registry_bundle.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/transform_registry.py` & `ax-platform-0.3.2/ax/storage/transform_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/storage/utils.py` & `ax-platform-0.3.2/ax/storage/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/telemetry/experiment.py` & `ax-platform-0.3.2/ax/telemetry/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     num_unordered_choice_parameters_small: int  # 2 - 3 elements
     num_unordered_choice_parameters_medium: int  # 4 - 7 elements
     num_unordered_choice_parameters_large: int  # 8 or more elements
 
     num_fixed_parameters: int
 
     dimensionality: int
-    heirerarchical_tree_height: int  # Height of tree for HSS, 1 for base SearchSpace
+    hierarchical_tree_height: int  # Height of tree for HSS, 1 for base SearchSpace
     num_parameter_constraints: int
 
     # OptimizationConfig info
     num_objectives: int
     num_tracking_metrics: int
     num_outcome_constraints: int  # Includes ObjectiveThresholds in MOO
 
@@ -102,15 +102,15 @@
                 num_unordered_choice_parameters_medium
             ),
             num_unordered_choice_parameters_large=num_unordered_choice_parameters_large,
             num_fixed_parameters=num_fixed_parameters,
             dimensionality=sum(
                 1 for param in experiment.parameters.values() if param.cardinality() > 1
             ),
-            heirerarchical_tree_height=experiment.search_space.height
+            hierarchical_tree_height=experiment.search_space.height
             if isinstance(experiment.search_space, HierarchicalSearchSpace)
             else 1,
             num_parameter_constraints=len(
                 experiment.search_space.parameter_constraints
             ),
             num_objectives=len(experiment.optimization_config.objective.metrics)
             if experiment.optimization_config is not None
```

### Comparing `ax-platform-0.3.1/ax/telemetry/generation_strategy.py` & `ax-platform-0.3.2/ax/telemetry/generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/telemetry/optimization.py` & `ax-platform-0.3.2/ax/telemetry/optimization.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/telemetry/tests/test_experiment.py` & `ax-platform-0.3.2/ax/telemetry/tests/test_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             num_int_range_parameters_large=1,
             num_log_scale_range_parameters=0,
             num_unordered_choice_parameters_small=1,
             num_unordered_choice_parameters_medium=0,
             num_unordered_choice_parameters_large=0,
             num_fixed_parameters=1,
             dimensionality=3,
-            heirerarchical_tree_height=1,
+            hierarchical_tree_height=1,
             num_parameter_constraints=3,
             num_objectives=1,
             num_tracking_metrics=1,
             num_outcome_constraints=1,
             num_map_metrics=0,
             metric_cls_to_quantity={"Metric": 2, "CustomTestMetric": 1},
             runner_cls="CustomTestRunner",
```

### Comparing `ax-platform-0.3.1/ax/telemetry/tests/test_generation_strategy.py` & `ax-platform-0.3.2/ax/telemetry/tests/test_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/telemetry/tests/test_optimization.py` & `ax-platform-0.3.2/ax/telemetry/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/telemetry/tests/test_scheduler.py` & `ax-platform-0.3.2/ax/telemetry/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 )
             ),
             scheduler_total_trials=0,
             scheduler_max_pending_trials=10,
             arms_per_trial=1,
             early_stopping_strategy_cls=None,
             global_stopping_strategy_cls=None,
-            transformed_dimensionality=-1,
+            transformed_dimensionality=2,
         )
         self.assertEqual(record, expected)
 
         flat = record.flatten()
         expected_dict = {
             **ExperimentCreatedRecord.from_experiment(
                 experiment=scheduler.experiment
@@ -54,15 +54,15 @@
                 generation_strategy=scheduler.generation_strategy
             ).__dict__,
             "scheduler_total_trials": 0,
             "scheduler_max_pending_trials": 10,
             "arms_per_trial": 1,
             "early_stopping_strategy_cls": None,
             "global_stopping_strategy_cls": None,
-            "transformed_dimensionality": -1,
+            "transformed_dimensionality": 2,
         }
         self.assertEqual(flat, expected_dict)
 
     def test_scheduler_completed_record_from_scheduler(self) -> None:
         scheduler = Scheduler(
             experiment=get_branin_experiment(),
             generation_strategy=get_generation_strategy(),
```

### Comparing `ax-platform-0.3.1/ax/utils/common/base.py` & `ax-platform-0.3.2/ax/utils/common/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/constants.py` & `ax-platform-0.3.2/ax/utils/common/constants.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/decorator.py` & `ax-platform-0.3.2/ax/utils/common/decorator.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/docutils.py` & `ax-platform-0.3.2/ax/utils/common/docutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/equality.py` & `ax-platform-0.3.2/ax/utils/common/equality.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,16 +145,16 @@
     """
     unequal_type, unequal_value = {}, {}
     for field in one_dict:
         one_val = one_dict.get(field)
         other_val = other_dict.get(field)
         one_val = numpy_type_to_python_type(one_val)
         other_val = numpy_type_to_python_type(other_val)
-
-        if type(one_val) != type(other_val):
+        skip_type_check = skip_db_id_check and field == "_db_id"
+        if not skip_type_check and (type(one_val) != type(other_val)):
             unequal_type[field] = (one_val, other_val)
             if fast_return:
                 return unequal_type, unequal_value
 
         if field == "_experiment":
             # prevent infinite loop when checking equality of Trials
             equal = one_val is other_val is None or (one_val._name == other_val._name)
```

### Comparing `ax-platform-0.3.1/ax/utils/common/executils.py` & `ax-platform-0.3.2/ax/utils/common/executils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/kwargs.py` & `ax-platform-0.3.2/ax/utils/common/kwargs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/logger.py` & `ax-platform-0.3.2/ax/utils/common/logger.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/mock.py` & `ax-platform-0.3.2/ax/utils/common/mock.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/result.py` & `ax-platform-0.3.2/ax/utils/common/result.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/serialization.py` & `ax-platform-0.3.2/ax/utils/common/serialization.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_docutils.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_docutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_equality.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_equality.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_executils.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_executils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_kwargutils.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_kwargutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_logger.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_result.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_serialization.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_testutils.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/tests/test_typeutils.py` & `ax-platform-0.3.2/ax/utils/common/tests/test_typeutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/testutils.py` & `ax-platform-0.3.2/ax/utils/common/testutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,17 @@
                 skip_db_id_check=skip_db_id_check,
             )
     return msg
 
 
 def setup_import_mocks(mocked_import_paths: List[str]) -> None:
     for import_path in mocked_import_paths:
-        if import_path in sys.modules:
+        if import_path in sys.modules and not isinstance(
+            sys.modules[import_path], MagicMock
+        ):
             raise Exception(f"{import_path} has already been imported!")
         sys.modules[import_path] = MagicMock()
 
 
 class TestCase(fake_filesystem_unittest.TestCase):
     """The base Ax test case, contains various helper functions to write unittests."""
 
@@ -351,15 +353,15 @@
         self.assertIsInstance(
             first, Base, "First argument is not a subclass of Ax `Base`."
         )
         self.assertIsInstance(
             second, Base, "Second argument is not a subclass of Ax `Base`."
         )
         if (
-            first._eq_skip_db_id_check(other=second)
+            not first._eq_skip_db_id_check(other=second)
             if skip_db_id_check
             else first != second
         ):
             raise self.failureException(
                 _build_comparison_str(
                     first=first, second=second, skip_db_id_check=skip_db_id_check
                 ),
```

### Comparing `ax-platform-0.3.1/ax/utils/common/timeutils.py` & `ax-platform-0.3.2/ax/utils/common/timeutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/typeutils.py` & `ax-platform-0.3.2/ax/utils/common/typeutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/common/typeutils_torch.py` & `ax-platform-0.3.2/ax/utils/common/typeutils_torch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/flake8_plugins/docstring_checker.py` & `ax-platform-0.3.2/ax/utils/flake8_plugins/docstring_checker.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/measurement/synthetic_functions.py` & `ax-platform-0.3.2/ax/utils/measurement/synthetic_functions.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/measurement/tests/test_synthetic_functions.py` & `ax-platform-0.3.2/ax/utils/measurement/tests/test_synthetic_functions.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/notebook/plotting.py` & `ax-platform-0.3.2/ax/utils/notebook/plotting.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/report/render.py` & `ax-platform-0.3.2/ax/utils/report/render.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/report/resources/base_template.html` & `ax-platform-0.3.2/ax/utils/report/resources/base_template.html`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/report/resources/report.css` & `ax-platform-0.3.2/ax/utils/report/resources/report.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/report/resources/sufficient_statistic.html` & `ax-platform-0.3.2/ax/utils/report/resources/sufficient_statistic.html`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/report/tests/test_render.py` & `ax-platform-0.3.2/ax/utils/report/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/sensitivity/derivative_gp.py` & `ax-platform-0.3.2/ax/utils/sensitivity/derivative_gp.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/sensitivity/derivative_measures.py` & `ax-platform-0.3.2/ax/utils/sensitivity/derivative_measures.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/sensitivity/sobol_measures.py` & `ax-platform-0.3.2/ax/utils/sensitivity/sobol_measures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from copy import deepcopy
-from typing import Callable, List, Optional
+
+from typing import Any, Callable, Dict, List, Optional, Union
+
+import numpy as np
 
 import torch
+
+from ax.modelbridge.torch import TorchModelBridge
+from ax.models.torch.botorch import BotorchModel
+from ax.models.torch.botorch_modular.model import BoTorchModel as ModularBoTorchModel
 from ax.utils.common.typeutils import checked_cast
 from botorch.models.model import Model
 from botorch.posteriors.gpytorch import GPyTorchPosterior
 from botorch.sampling.normal import SobolQMCNormalSampler
 from botorch.utils.sampling import draw_sobol_samples
 from botorch.utils.transforms import unnormalize
-from torch._tensor import Tensor
+from gpytorch.models import IndependentModelList
+from torch import Tensor
 
 
 class SobolSensitivity(object):
     def __init__(
         self,
         dim: int,
         bounds: torch.Tensor,
@@ -52,18 +60,20 @@
         self.bootstrap = num_bootstrap_samples > 1
         # pyre-fixme[4]: Attribute must be annotated.
         self.num_bootstrap_samples = (
             num_bootstrap_samples - 1
         )  # deduct 1 because the first is meant to be the full grid
         self.bootstrap_array = bootstrap_array
         if input_qmc:
-            # pyre-fixme[4]: Attribute must be annotated.
-            self.A = draw_sobol_samples(bounds=bounds, n=num_mc_samples, q=1).squeeze(1)
-            # pyre-fixme[4]: Attribute must be annotated.
-            self.B = draw_sobol_samples(bounds=bounds, n=num_mc_samples, q=1).squeeze(1)
+            sobol_kwargs = {"bounds": bounds, "n": num_mc_samples, "q": 1}
+            seed_A, seed_B = 1234, 5678  # to make it reproducible
+            # pyre-ignore
+            self.A = draw_sobol_samples(**sobol_kwargs, seed=seed_A).squeeze(1)
+            # pyre-ignore
+            self.B = draw_sobol_samples(**sobol_kwargs, seed=seed_B).squeeze(1)
         else:
             self.A = unnormalize(torch.rand(num_mc_samples, dim), bounds=bounds)
             self.B = unnormalize(torch.rand(num_mc_samples, dim), bounds=bounds)
         # pyre-fixme[4]: Attribute must be annotated.
         self.A_B_ABi = self.generate_all_input_matrix().to(torch.double)
 
         if self.bootstrap:
@@ -96,24 +106,25 @@
         # pyre-fixme[24]: Generic type `list` expects 1 type parameter, use
         #  `typing.List` to avoid runtime subscripting errors.
         self.f_BAis_btsp: Optional[List] = None
         self.first_order_idxs: Optional[torch.Tensor] = None
         self.first_order_idxs_btsp: Optional[torch.Tensor] = None
 
     def generate_all_input_matrix(self) -> torch.Tensor:
-        A_B_ABi = torch.cat((self.A, self.B), dim=0)
+        A_B_ABi_list = [self.A, self.B]
         for i in range(self.dim):
             AB_i = deepcopy(self.A)
             AB_i[:, i] = self.B[:, i]
-            A_B_ABi = torch.cat((A_B_ABi, AB_i), dim=0)
+            A_B_ABi_list.append(AB_i)
         if self.second_order:
             for i in range(self.dim):
                 BA_i = deepcopy(self.B)
                 BA_i[:, i] = self.A[:, i]
-                A_B_ABi = torch.cat((A_B_ABi, BA_i), dim=0)
+                A_B_ABi_list.append(BA_i)
+        A_B_ABi = torch.cat(A_B_ABi_list, dim=0)
         return A_B_ABi
 
     def evalute_function(self, f_A_B_ABi: Optional[torch.Tensor] = None) -> None:
         r"""evaluates the objective function and devides the evaluation into
             torch.Tensors needed for the indices computation.
         Args:
             f_A_B_ABi: Function evaluations on the entire grid of size M(d+2).
@@ -374,15 +385,15 @@
     a = mean / torch.sqrt(1 + var)
     return torch.distributions.Normal(0, 1).cdf(a)
 
 
 class SobolSensitivityGPMean(object):
     def __init__(
         self,
-        model: Model,
+        model: Model,  # TODO: narrow type down. E.g. ModelListGP does not work.
         bounds: torch.Tensor,
         num_mc_samples: int = 10**4,
         second_order: bool = False,
         input_qmc: bool = False,
         num_bootstrap_samples: int = 1,
         link_function: Callable[
             [torch.Tensor, torch.Tensor], torch.Tensor
@@ -522,17 +533,17 @@
                 self.samples = posterior.rsample(torch.Size([self.num_gp_samples]))
 
     def first_order_indices(self) -> Tensor:
         r"""Computes the first order Sobol indices:
 
         Returns:
             if num_bootstrap_samples>1
-                Tensor: (values,var_gp,stderr_gp,var_mc,stderr_mc)x dim
+                Tensor: (values, var_gp, stderr_gp, var_mc, stderr_mc) x dim
             else
-                Tensor: (values,var,stderr)x dim
+                Tensor: (values, var, stderr) x dim
         """
         first_order_idxs_list = []
         for j in range(self.num_gp_samples):
             self.sensitivity.evalute_function(self.samples[j])
             first_order_idxs = self.sensitivity.first_order_indices()
             first_order_idxs_list.append(first_order_idxs.unsqueeze(0))
         # pyre-fixme[16]: `SobolSensitivityGPSampling` has no attribute
@@ -577,17 +588,17 @@
             return first_order_idxs_mean_vargp_segp_varmc_segp
 
     def total_order_indices(self) -> Tensor:
         r"""Computes the total Sobol indices:
 
         Returns:
             if num_bootstrap_samples>1
-                Tensor: (values,var_gp,stderr_gp,var_mc,stderr_mc)x dim
+                Tensor: (values, var_gp, stderr_gp, var_mc, stderr_mc) x dim
             else
-                Tensor: (values,var,stderr)x dim
+                Tensor: (values, var, stderr) x dim
         """
         total_order_idxs_list = []
         for j in range(self.num_gp_samples):
             self.sensitivity.evalute_function(self.samples[j])
             total_order_idxs = self.sensitivity.total_order_indices()
             total_order_idxs_list.append(total_order_idxs.unsqueeze(0))
         total_order_idxs_list = torch.cat(total_order_idxs_list, dim=0)
@@ -628,17 +639,17 @@
             return total_order_idxs_mean_vargp_segp_varmc_segp
 
     def second_order_indices(self) -> Tensor:
         r"""Computes the Second order Sobol indices:
 
         Returns:
             if num_bootstrap_samples>1
-                Tensor: (values,var_gp,stderr_gp,var_mc,stderr_mc)x dim(dim-1)/2
+                Tensor: (values, var_gp, stderr_gp, var_mc, stderr_mc) x dim(dim-1) / 2
             else
-                Tensor: (values,var,stderr)x dim(dim-1)/2
+                Tensor: (values, var, stderr) x dim(dim-1) / 2
         """
         if not (self.bootstrap):
             second_order_idxs_list = []
             for j in range(self.num_gp_samples):
                 self.sensitivity.evalute_function(self.samples[j])
                 second_order_idxs = self.sensitivity.second_order_indices(
                     # pyre-fixme[16]: `SobolSensitivityGPSampling` has no attribute
@@ -689,7 +700,143 @@
                         [total_mean[i], gp_var[i], gp_se[i], mc_var[i], mc_se[i]]
                     ).unsqueeze(0)
                     for i in range(num_second_order)
                 ],
                 dim=0,
             )
             return second_order_idxs_mean_vargp_segp_varmc_segp
+
+
+def compute_sobol_indices_from_model_list(
+    model_list: List[Model],
+    bounds: Tensor,
+    order: str = "first",
+    **sobol_kwargs: Any,
+) -> Tensor:
+    """
+    Computes Sobol indices of a list of models on a bounded domain.
+
+    Args:
+        model_list: A list of botorch.models.model.Model types for which to compute
+            the Sobol indices.
+        bounds: A 2 x d Tensor of lower and upper bounds of the domain of the models.
+        order: A string specifying the order of the Sobol indices to be computed.
+            Supports "first" and "total" and defaults to "first".
+        sobol_kwargs: keyword arguments passed on to SobolSensitivityGPMean.
+
+    Returns:
+        With m GPs, returns a (m x d) tensor of `order`-order Sobol indices.
+    """
+    indices = []
+    method = getattr(SobolSensitivityGPMean, f"{order}_order_indices")
+    for model in model_list:
+        sens_class = SobolSensitivityGPMean(
+            model=model,
+            bounds=bounds,
+            **sobol_kwargs,
+        )
+        indices.append(method(sens_class))
+    return torch.stack(indices)
+
+
+def ax_parameter_sens(
+    model_bridge: TorchModelBridge,
+    metrics: Optional[List[str]] = None,
+    order: str = "first",
+    **sobol_kwargs: Any,
+) -> Dict[str, Dict[str, np.ndarray]]:
+    """
+    Compute sensitivity for all metrics on an TorchModelBridge.
+
+    Args:
+        model_bridge: A ModelBridge object with models that were fit.
+        metrics: The names of the metrics and outcomes for which to compute
+            sensitivities. This should preferably be metrics with a good model fit.
+            Defaults to model_bridge.outcomes.
+        order: A string specifying the order of the Sobol indices to be computed.
+            Supports "first" and "total" and defaults to "first".
+        sobol_kwargs: keyword arguments passed on to SobolSensitivityGPMean.
+
+    Returns:
+        Dictionary {'metric_name': {'parameter_name': sensitivity_value}}, where the
+            `sensitivity` value is cast to a Numpy array in order to be compatible with
+            `plot_feature_importance_by_feature`.
+    """
+    if metrics is None:
+        metrics = model_bridge.outcomes
+    # can safely access _search_space_digest after type check
+    torch_model = _get_torch_model(model_bridge)
+    digest = torch_model.search_space_digest
+    ind = compute_sobol_indices_from_model_list(
+        model_list=_get_model_per_metric(torch_model, metrics),
+        bounds=torch.tensor(digest.bounds).T,  # transposing to make it 2 x d
+        order=order,
+        **sobol_kwargs,
+    )
+    return _array_with_string_indices_to_dict(
+        rows=metrics, cols=digest.feature_names, A=ind.numpy()
+    )
+
+
+def _get_torch_model(
+    model_bridge: TorchModelBridge,
+) -> Union[BotorchModel, ModularBoTorchModel]:
+    """Returns the TorchModel of the model_bridge, if it is a type that stores
+    SearchSpaceDigest during model fitting. At this point, this is BotorchModel, and
+    ModularBoTorchModel.
+    """
+    if not isinstance(model_bridge, TorchModelBridge):
+        raise NotImplementedError(
+            f"{type(model_bridge) = }, but only TorchModelBridge is supported."
+        )
+    model = model_bridge.model  # should be of type TorchModel
+    if not (isinstance(model, BotorchModel) or isinstance(model, ModularBoTorchModel)):
+        raise NotImplementedError(
+            f"{type(model_bridge.model) = }, but only "
+            "Union[BotorchModel, ModularBoTorchModel] is supported."
+        )
+    return model
+
+
+def _get_model_per_metric(
+    model: Union[BotorchModel, ModularBoTorchModel], metrics: List[str]
+) -> List[Model]:
+    """For a given TorchModel model, returns a list of botorch.models.model.Model
+    objects corresponding to - and in the same order as - the given metrics.
+    """
+    if isinstance(model, BotorchModel):
+        # guaranteed not to be None after accessing search_space_digest
+        gp_model = model.model
+        model_idx = [model.metric_names.index(m) for m in metrics]
+        if not isinstance(gp_model, IndependentModelList):
+            if gp_model.num_outputs == 1:  # can accept single output models
+                return [gp_model for _ in model_idx]
+            raise NotImplementedError(
+                f"type(model_bridge.model.model) = {type(gp_model)}, "
+                "but only IndependentModelList is supported."
+            )
+        return [gp_model.models[i] for i in model_idx]
+    else:  # isinstance(model, ModularBoTorchModel):
+        model_list = []
+        for m in metrics:
+            for label, outcomes in model.outcomes_by_surrogate_label.items():
+                if m in outcomes:
+                    metric_model = model.surrogates[label].model
+                    # if metric_model.num_outputs > 1:
+                    #     raise RuntimeError("Batched models currently not supported.")
+                    model_list.append(metric_model)
+        return model_list
+
+
+def _array_with_string_indices_to_dict(
+    rows: List[str], cols: List[str], A: np.ndarray
+) -> Dict[str, Dict[str, np.ndarray]]:
+    """
+    Args:
+        - rows: A list of strings with which to index rows of A.
+        - cols: A list of strings with which to index columns of A.
+        - A: A matrix, with `len(rows)` rows and `len(cols)` columns.
+
+    Returns:
+        A dictionary dict that satisfies dict[rows[i]][cols[j]] = A[i, j].
+    """
+    return {r: dict(zip(cols, a)) for r, a in zip(rows, A)}
```

### Comparing `ax-platform-0.3.1/ax/utils/stats/statstools.py` & `ax-platform-0.3.2/ax/utils/stats/statstools.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/stats/tests/test_statstools.py` & `ax-platform-0.3.2/ax/utils/stats/tests/test_statstools.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/backend_scheduler.py` & `ax-platform-0.3.2/ax/utils/testing/backend_scheduler.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/backend_simulator.py` & `ax-platform-0.3.2/ax/utils/testing/backend_simulator.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/benchmark_stubs.py` & `ax-platform-0.3.2/ax/utils/testing/benchmark_stubs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/core_stubs.py` & `ax-platform-0.3.2/ax/utils/testing/core_stubs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/metrics/backend_simulator_map.py` & `ax-platform-0.3.2/ax/utils/testing/metrics/backend_simulator_map.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/metrics/branin_backend_map.py` & `ax-platform-0.3.2/ax/utils/testing/metrics/branin_backend_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Iterable, List, Optional
+from typing import List, Optional
 
 import numpy as np
-from ax.core.map_data import MapKeyInfo
 from ax.metrics.branin_map import BraninTimestampMapMetric
 from ax.utils.testing.metrics.backend_simulator_map import (
     BackendSimulatorTimestampMapMetric,
 )
 
 
 class BraninBackendMapMetric(
@@ -20,16 +19,14 @@
     """A Branin ``BackendSimulatorTimestampMapMetric`` with a multiplicative
     factor of ``1 - exp(-rate * t)`` where ``t`` is the runtime of the trial."""
 
     def __init__(
         self,
         name: str,
         param_names: List[str],
-        # pyre-fixme[24]: Generic type `MapKeyInfo` expects 1 type parameter.
-        map_key_infos: Optional[Iterable[MapKeyInfo]] = None,
         noise_sd: float = 0.0,
         lower_is_better: Optional[bool] = True,
         cache_evaluations: bool = True,
         rate: float = 0.5,
         delta_t: float = 1.0,
     ) -> None:
         """The ``BraninTimestampMapMetric`` integrated with the backend simulator.
@@ -44,17 +41,14 @@
             delta_t: The time delta between intermediate results, used in
                 ``convert_to_timestamps``.
         """
         BackendSimulatorTimestampMapMetric.__init__(
             self,
             name=name,
             param_names=param_names,
-            map_key_infos=map_key_infos
-            if map_key_infos is not None
-            else [MapKeyInfo(key="timestamp", default_value=0.0)],
             noise_sd=noise_sd,
             lower_is_better=lower_is_better,
             cache_evaluations=cache_evaluations,
         )
         self.rate = rate
         self.delta_t = delta_t
         self._timestamp = -1
```

### Comparing `ax-platform-0.3.1/ax/utils/testing/mock.py` & `ax-platform-0.3.2/ax/utils/testing/mock.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/modeling_stubs.py` & `ax-platform-0.3.2/ax/utils/testing/modeling_stubs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/test_init_files.py` & `ax-platform-0.3.2/ax/utils/testing/test_init_files.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/tests/test_backend_simulator.py` & `ax-platform-0.3.2/ax/utils/testing/tests/test_backend_simulator.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/tests/test_utils.py` & `ax-platform-0.3.2/ax/utils/testing/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/torch_stubs.py` & `ax-platform-0.3.2/ax/utils/testing/torch_stubs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/testing/utils.py` & `ax-platform-0.3.2/ax/utils/testing/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax/utils/tutorials/cnn_utils.py` & `ax-platform-0.3.2/ax/utils/tutorials/cnn_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/ax_platform.egg-info/PKG-INFO` & `ax-platform-0.3.2/ax_platform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ax-platform
-Version: 0.3.1
+Version: 0.3.2
 Summary: Adaptive Experimentation
 Home-page: https://github.com/facebook/Ax
 Author: Facebook, Inc.
 License: MIT
 Description: <img width="300" src="https://ax.dev/img/ax_logo_lockup.svg" alt="Ax Logo" />
         
         <hr/>
@@ -171,15 +171,15 @@
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
         export ALLOW_LATEST_GPYTORCH_LINOP=true
         pip install git+https://github.com/pytorch/botorch.git
         export ALLOW_BOTORCH_LATEST=true
         git clone https://github.com/facebook/ax.git --depth 1
         cd ax
-        pip install -e .[notebook,mysql,dev]
+        pip install -e .[unittest]
         ```
         
         See recommendation for installing PyTorch for MacOS users above.
         
         The above example limits the cloned directory size via the
         [`--depth`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---depthltdepthgt)
         argument to `git clone`. If you require the entire commit history you may remove this
```

### Comparing `ax-platform-0.3.1/ax_platform.egg-info/SOURCES.txt` & `ax-platform-0.3.2/ax_platform.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py
 ax/modelbridge/tests/test_ivw_transform.py
 ax/modelbridge/tests/test_log_transform.py
 ax/modelbridge/tests/test_log_y_transform.py
 ax/modelbridge/tests/test_logit_transform.py
 ax/modelbridge/tests/test_map_torch_modelbridge.py
 ax/modelbridge/tests/test_map_unit_x_transform.py
+ax/modelbridge/tests/test_merge_repeated_measurements_transform.py
 ax/modelbridge/tests/test_metrics_as_task_transform.py
 ax/modelbridge/tests/test_model_spec.py
 ax/modelbridge/tests/test_modelbridge_utils.py
 ax/modelbridge/tests/test_one_hot_transform.py
 ax/modelbridge/tests/test_pairwise_modelbridge.py
 ax/modelbridge/tests/test_percentile_y_transform.py
 ax/modelbridge/tests/test_power_transform_y.py
@@ -199,14 +200,15 @@
 ax/modelbridge/tests/test_registry.py
 ax/modelbridge/tests/test_relativize_transform.py
 ax/modelbridge/tests/test_rembo_strategy.py
 ax/modelbridge/tests/test_remove_fixed_transform.py
 ax/modelbridge/tests/test_robust.py
 ax/modelbridge/tests/test_rounding.py
 ax/modelbridge/tests/test_search_space_to_choice_transform.py
+ax/modelbridge/tests/test_search_space_to_float_transform.py
 ax/modelbridge/tests/test_standardize_y_transform.py
 ax/modelbridge/tests/test_stratified_standardize_y.py
 ax/modelbridge/tests/test_task_encode_transform.py
 ax/modelbridge/tests/test_torch_modelbridge.py
 ax/modelbridge/tests/test_torch_modelbridge_moo.py
 ax/modelbridge/tests/test_transform_utils.py
 ax/modelbridge/tests/test_trial_as_task_transform.py
@@ -226,22 +228,24 @@
 ax/modelbridge/transforms/int_to_float.py
 ax/modelbridge/transforms/inverse_gaussian_cdf_y.py
 ax/modelbridge/transforms/ivw.py
 ax/modelbridge/transforms/log.py
 ax/modelbridge/transforms/log_y.py
 ax/modelbridge/transforms/logit.py
 ax/modelbridge/transforms/map_unit_x.py
+ax/modelbridge/transforms/merge_repeated_measurements.py
 ax/modelbridge/transforms/metrics_as_task.py
 ax/modelbridge/transforms/one_hot.py
 ax/modelbridge/transforms/percentile_y.py
 ax/modelbridge/transforms/power_transform_y.py
 ax/modelbridge/transforms/relativize.py
 ax/modelbridge/transforms/remove_fixed.py
 ax/modelbridge/transforms/rounding.py
 ax/modelbridge/transforms/search_space_to_choice.py
+ax/modelbridge/transforms/search_space_to_float.py
 ax/modelbridge/transforms/standardize_y.py
 ax/modelbridge/transforms/stratified_standardize_y.py
 ax/modelbridge/transforms/task_encode.py
 ax/modelbridge/transforms/trial_as_task.py
 ax/modelbridge/transforms/unit_x.py
 ax/modelbridge/transforms/utils.py
 ax/modelbridge/transforms/winsorize.py
```

### Comparing `ax-platform-0.3.1/ax_platform.egg-info/requires.txt` & `ax-platform-0.3.2/ax_platform.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-botorch==0.8.3
+botorch==0.8.5
 jinja2
 pandas
 scipy
 scikit-learn
 ipywidgets
 plotly>=5.12.0
 typeguard==2.13.3
```

### Comparing `ax-platform-0.3.1/docs/api.md` & `ax-platform-0.3.2/docs/api.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/bandit_allocation.png` & `ax-platform-0.3.2/docs/assets/bandit_allocation.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/bo_1d_opt.gif` & `ax-platform-0.3.2/docs/assets/bo_1d_opt.gif`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/contour.js` & `ax-platform-0.3.2/docs/assets/contour.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/cv.js` & `ax-platform-0.3.2/docs/assets/cv.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/example_shrinkage.png` & `ax-platform-0.3.2/docs/assets/example_shrinkage.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/fitted.js` & `ax-platform-0.3.2/docs/assets/fitted.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/gp_opt.png` & `ax-platform-0.3.2/docs/assets/gp_opt.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/gp_posterior.png` & `ax-platform-0.3.2/docs/assets/gp_posterior.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/mab_animate.gif` & `ax-platform-0.3.2/docs/assets/mab_animate.gif`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/mab_probs.png` & `ax-platform-0.3.2/docs/assets/mab_probs.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/mab_regret.png` & `ax-platform-0.3.2/docs/assets/mab_regret.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/assets/slice.js` & `ax-platform-0.3.2/docs/assets/slice.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/banditopt.md` & `ax-platform-0.3.2/docs/banditopt.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/bayesopt.md` & `ax-platform-0.3.2/docs/bayesopt.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/core.md` & `ax-platform-0.3.2/docs/core.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/data.md` & `ax-platform-0.3.2/docs/data.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/glossary.md` & `ax-platform-0.3.2/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/installation.md` & `ax-platform-0.3.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/models.md` & `ax-platform-0.3.2/docs/models.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/storage.md` & `ax-platform-0.3.2/docs/storage.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/trial-evaluation.md` & `ax-platform-0.3.2/docs/trial-evaluation.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/docs/why-ax.md` & `ax-platform-0.3.2/docs/why-ax.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/build_ax.sh` & `ax-platform-0.3.2/scripts/build_ax.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/docker_install.sh` & `ax-platform-0.3.2/scripts/docker_install.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/insert_api_refs.py` & `ax-platform-0.3.2/scripts/insert_api_refs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/make_docs.sh` & `ax-platform-0.3.2/scripts/make_docs.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/make_tutorials.py` & `ax-platform-0.3.2/scripts/make_tutorials.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/parse_sphinx.py` & `ax-platform-0.3.2/scripts/parse_sphinx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/patch_site_config.py` & `ax-platform-0.3.2/scripts/patch_site_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/publish_site.sh` & `ax-platform-0.3.2/scripts/publish_site.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/update_versions_html.py` & `ax-platform-0.3.2/scripts/update_versions_html.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/validate_sphinx.py` & `ax-platform-0.3.2/scripts/validate_sphinx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/versions.js` & `ax-platform-0.3.2/scripts/versions.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/scripts/wheels_build.ps1` & `ax-platform-0.3.2/scripts/wheels_build.ps1`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/setup.py` & `ax-platform-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import os
 
 from setuptools import find_packages, setup
 
 # TODO: read pinned Botorch version from a shared source
-PINNED_BOTORCH_VERSION = "0.8.3"
+PINNED_BOTORCH_VERSION = "0.8.5"
 
 if os.environ.get("ALLOW_BOTORCH_LATEST"):
     # allows a more recent previously installed version of botorch to remain
     # if there is no previously installed version, installs the latest release
     botorch_req = f"botorch>={PINNED_BOTORCH_VERSION}"
 else:
     botorch_req = f"botorch=={PINNED_BOTORCH_VERSION}"
```

### Comparing `ax-platform-0.3.1/sphinx/Makefile` & `ax-platform-0.3.2/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/make.bat` & `ax-platform-0.3.2/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/benchmark.rst` & `ax-platform-0.3.2/sphinx/source/benchmark.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/conf.py` & `ax-platform-0.3.2/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/core.rst` & `ax-platform-0.3.2/sphinx/source/core.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/early_stopping.rst` & `ax-platform-0.3.2/sphinx/source/early_stopping.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/exceptions.rst` & `ax-platform-0.3.2/sphinx/source/exceptions.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/global_stopping.rst` & `ax-platform-0.3.2/sphinx/source/global_stopping.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/index.rst` & `ax-platform-0.3.2/sphinx/source/index.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/metrics.rst` & `ax-platform-0.3.2/sphinx/source/metrics.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/modelbridge.rst` & `ax-platform-0.3.2/sphinx/source/modelbridge.rst`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,22 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.modelbridge.transforms.map_unit_x
     :members:
     :undoc-members:
     :show-inheritance:
 
+`ax.modelbridge.transforms.merge_repeated_measurements`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. automodule:: ax.modelbridge.transforms.merge_repeated_measurements
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
 `ax.modelbridge.transforms.metrics_as_task`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.modelbridge.transforms.metrics_as_task
     :members:
     :undoc-members:
     :show-inheritance:
@@ -311,15 +319,23 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.modelbridge.transforms.search_space_to_choice
     :members:
     :undoc-members:
     :show-inheritance:
 
-`ax.modelbridge.transforms.standardize\_y`
+`ax.modelbridge.transforms.search\_space\_to\_float`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. automodule:: ax.modelbridge.transforms.search_space_to_float
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+ `ax.modelbridge.transforms.standardize\_y`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.modelbridge.transforms.standardize_y
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `ax-platform-0.3.1/sphinx/source/models.rst` & `ax-platform-0.3.2/sphinx/source/models.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/plot.rst` & `ax-platform-0.3.2/sphinx/source/plot.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/runners.rst` & `ax-platform-0.3.2/sphinx/source/runners.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/service.rst` & `ax-platform-0.3.2/sphinx/source/service.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/storage.rst` & `ax-platform-0.3.2/sphinx/source/storage.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/telemetry.rst` & `ax-platform-0.3.2/sphinx/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/sphinx/source/utils.rst` & `ax-platform-0.3.2/sphinx/source/utils.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb` & `ax-platform-0.3.2/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/early_stopping/early_stopping.ipynb` & `ax-platform-0.3.2/tutorials/early_stopping/early_stopping.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/early_stopping/mnist_train_nas.py` & `ax-platform-0.3.2/tutorials/early_stopping/mnist_train_nas.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     parser.add_argument("--batch_size", type=int, required=True, help="batch size")
     return parser.parse_args()
 
 
 args = parse_args()
 
 PATH_DATASETS = os.environ.get("PATH_DATASETS", ".")
-AVAIL_GPUS = min(1, torch.cuda.device_count())
 
 
 class MnistModel(LightningModule):
     def __init__(self):
         super().__init__()
 
         # Tunable parameters
@@ -141,15 +140,14 @@
     mnist_model = MnistModel()
 
     # Initialize a trainer
     logger = pl_loggers.TensorBoardLogger(args.log_path)
     trainer = Trainer(
         logger=logger,
         log_every_n_steps=1,
-        gpus=AVAIL_GPUS,
         max_epochs=args.epochs,
         enable_progress_bar=False,
         deterministic=True,  # Do we want a bit of noise?
         default_root_dir=args.log_path,
     )
     logger.save()
```

### Comparing `ax-platform-0.3.1/tutorials/factorial.ipynb` & `ax-platform-0.3.2/tutorials/factorial.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/generation_strategy.ipynb` & `ax-platform-0.3.2/tutorials/generation_strategy.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/gpei_hartmann_developer.ipynb` & `ax-platform-0.3.2/tutorials/gpei_hartmann_developer.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/gpei_hartmann_loop.ipynb` & `ax-platform-0.3.2/tutorials/gpei_hartmann_loop.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/gpei_hartmann_service.ipynb` & `ax-platform-0.3.2/tutorials/gpei_hartmann_service.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/human_in_the_loop/hitl_data.json` & `ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_data.json`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/human_in_the_loop/hitl_exp.json` & `ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_exp.json`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/human_in_the_loop/human_in_the_loop.ipynb` & `ax-platform-0.3.2/tutorials/human_in_the_loop/human_in_the_loop.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/modular_botax.ipynb` & `ax-platform-0.3.2/tutorials/modular_botax.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/multi_task.ipynb` & `ax-platform-0.3.2/tutorials/multi_task.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/multiobjective_optimization.ipynb` & `ax-platform-0.3.2/tutorials/multiobjective_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/raytune_pytorch_cnn.ipynb` & `ax-platform-0.3.2/tutorials/raytune_pytorch_cnn.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/saasbo.ipynb` & `ax-platform-0.3.2/tutorials/saasbo.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/saasbo_nehvi.ipynb` & `ax-platform-0.3.2/tutorials/saasbo_nehvi.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/scheduler.ipynb` & `ax-platform-0.3.2/tutorials/scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/tune_cnn.ipynb` & `ax-platform-0.3.2/tutorials/tune_cnn.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/tutorials/visualizations.ipynb` & `ax-platform-0.3.2/tutorials/visualizations.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/core/Footer.js` & `ax-platform-0.3.2/website/core/Footer.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/core/Tutorial.js` & `ax-platform-0.3.2/website/core/Tutorial.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/core/TutorialSidebar.js` & `ax-platform-0.3.2/website/core/TutorialSidebar.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/pages/en/index.js` & `ax-platform-0.3.2/website/pages/en/index.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/pages/tutorials/index.js` & `ax-platform-0.3.2/website/pages/tutorials/index.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/siteConfig.js` & `ax-platform-0.3.2/website/siteConfig.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/css/base_sphinx.css` & `ax-platform-0.3.2/website/static/css/base_sphinx.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/css/custom.css` & `ax-platform-0.3.2/website/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/css/custom_sphinx.css` & `ax-platform-0.3.2/website/static/css/custom_sphinx.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/css/pygments.css` & `ax-platform-0.3.2/website/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/ax.svg` & `ax-platform-0.3.2/website/static/img/ax.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/ax_lockup.svg` & `ax-platform-0.3.2/website/static/img/ax_lockup.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/ax_lockup_white.svg` & `ax-platform-0.3.2/website/static/img/ax_lockup_white.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/ax_logo_lockup.svg` & `ax-platform-0.3.2/website/static/img/ax_logo_lockup.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/database-solid.svg` & `ax-platform-0.3.2/website/static/img/database-solid.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/dice-solid.svg` & `ax-platform-0.3.2/website/static/img/dice-solid.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/favicon/favicon.ico` & `ax-platform-0.3.2/website/static/img/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/favicon.png` & `ax-platform-0.3.2/website/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/oss_logo.png` & `ax-platform-0.3.2/website/static/img/oss_logo.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/img/th-large-solid.svg` & `ax-platform-0.3.2/website/static/img/th-large-solid.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/js/mathjax.js` & `ax-platform-0.3.2/website/static/js/mathjax.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/static/js/plotUtils.js` & `ax-platform-0.3.2/website/static/js/plotUtils.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.1/website/tutorials.json` & `ax-platform-0.3.2/website/tutorials.json`

 * *Files identical despite different names*


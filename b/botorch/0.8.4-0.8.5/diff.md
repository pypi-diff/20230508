# Comparing `tmp/botorch-0.8.4.tar.gz` & `tmp/botorch-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botorch-0.8.4.tar", last modified: Mon Apr 24 15:50:22 2023, max compression
+gzip compressed data, was "botorch-0.8.5.tar", last modified: Mon May  8 17:50:32 2023, max compression
```

## Comparing `botorch-0.8.4.tar` & `botorch-0.8.5.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.958487 botorch-0.8.4/.conda/
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-04-24 15:47:10.000000 botorch-0.8.4/.conda/build_conda.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-24 15:47:10.000000 botorch-0.8.4/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.958487 botorch-0.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.962487 botorch-0.8.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.966487 botorch-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/deploy_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/reusable_tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/reusable_website.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/test_stable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/tutorials_smoke_test_on_pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/tutorials_smoke_test_on_push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-24 15:47:10.000000 botorch-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    49792 2023-04-24 15:47:10.000000 botorch-0.8.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-24 15:47:10.000000 botorch-0.8.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-24 15:47:10.000000 botorch-0.8.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-24 15:47:10.000000 botorch-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 15:47:10.000000 botorch-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-24 15:50:22.006487 botorch-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-24 15:47:10.000000 botorch-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.966487 botorch-0.8.4/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.974487 botorch-0.8.4/botorch/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)    47072 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/cached_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/cost_aware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/fixed_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    45121 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/input_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    26678 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/knowledge_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    42039 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23047 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/monte_carlo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.978487 botorch-0.8.4/botorch/acquisition/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)    31296 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    33366 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/multi_output_risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    48822 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_step_lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/penalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/proximal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.978487 botorch-0.8.4/botorch/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/exceptions/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/exceptions/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.978487 botorch-0.8.4/botorch/generation/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.982487 botorch-0.8.4/botorch/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/approximate_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/contextual_multioutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/fully_bayesian_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gp_regression_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gp_regression_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/higher_order_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/contextual_lcea.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/contextual_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/downsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/linear_truncated_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/likelihoods/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/model_list_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    46666 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/pairwise_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    63408 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    30085 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/assorted.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/inducing_point_allocators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/parse_training_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.990487 botorch-0.8.4/botorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.990487 botorch-0.8.4/botorch/optim/closures/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/closures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/closures/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/closures/model_closures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    42398 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/numpy_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.990487 botorch-0.8.4/botorch/optim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/acquisition_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.994487 botorch-0.8.4/botorch/posteriors/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/base_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/higher_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/posterior_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.994487 botorch-0.8.4/botorch/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/get_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/index_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/list_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pairwise_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.998487 botorch-0.8.4/botorch/sampling/pathwise/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.998487 botorch-0.8.4/botorch/sampling/pathwise/features/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/features/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/features/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/posterior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/prior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/update_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/qmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/stochastic_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.998487 botorch-0.8.4/botorch/test_functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    48773 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/multi_objective_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/sensitivity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.002487 botorch-0.8.4/botorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/feasible_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    20040 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/gp_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/low_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.002487 botorch-0.8.4/botorch/utils/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/dominated.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/non_dominated.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/scalarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/botorch/utils/probability/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/bvn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/lin_ess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/mvnxpb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/truncated_multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/unified_skew_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/safe_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    36647 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.970487 botorch-0.8.4/botorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    79395 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch_logo_lockup.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    63261 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch_logo_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 15:47:10.000000 botorch-0.8.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-24 15:47:10.000000 botorch-0.8.4/notebooks/tutorials_performance_tracking.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 15:47:10.000000 botorch-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 15:47:10.000000 botorch-0.8.4/requirements-fmt.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 15:47:10.000000 botorch-0.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 15:50:22.010487 botorch-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-24 15:47:10.000000 botorch-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.636422 botorch-0.8.5/.conda/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-05-08 17:48:07.000000 botorch-0.8.5/.conda/build_conda.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 17:48:07.000000 botorch-0.8.5/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.636422 botorch-0.8.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.636422 botorch-0.8.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.640423 botorch-0.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/deploy_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/reusable_tutorials.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/reusable_website.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/test_stable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/tutorials_smoke_test_on_pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/tutorials_smoke_test_on_push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 17:48:07.000000 botorch-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    50315 2023-05-08 17:48:07.000000 botorch-0.8.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-08 17:48:07.000000 botorch-0.8.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-08 17:48:07.000000 botorch-0.8.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-08 17:48:07.000000 botorch-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 17:48:07.000000 botorch-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-08 17:50:32.704423 botorch-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-05-08 17:48:07.000000 botorch-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.644423 botorch-0.8.5/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.648423 botorch-0.8.5/botorch/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47072 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/cached_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/cost_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/fixed_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45389 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/input_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/joint_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26678 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/knowledge_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42642 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/max_value_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23047 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/monte_carlo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.652423 botorch-0.8.5/botorch/acquisition/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31296 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/joint_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/max_value_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33366 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/multi_output_risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48822 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/predictive_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_step_lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/penalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/predictive_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.652423 botorch-0.8.5/botorch/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/exceptions/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/exceptions/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.652423 botorch-0.8.5/botorch/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.660423 botorch-0.8.5/botorch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/approximate_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/contextual_multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/fully_bayesian_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gp_regression_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gp_regression_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gpytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/higher_order_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.664423 botorch-0.8.5/botorch/models/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/contextual_lcea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/contextual_sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/linear_truncated_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.664423 botorch-0.8.5/botorch/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/likelihoods/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/model_list_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46993 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/pairwise_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.668423 botorch-0.8.5/botorch/models/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63408 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30293 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.668423 botorch-0.8.5/botorch/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/assorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/inducing_point_allocators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/parse_training_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.672423 botorch-0.8.5/botorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.676423 botorch-0.8.5/botorch/optim/closures/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/closures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/closures/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/closures/model_closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42398 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/numpy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56043 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.676423 botorch-0.8.5/botorch/optim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/acquisition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.680423 botorch-0.8.5/botorch/posteriors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/base_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/gpytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/higher_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/posterior_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.684423 botorch-0.8.5/botorch/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/get_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/index_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/list_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pairwise_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.688423 botorch-0.8.5/botorch/sampling/pathwise/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.688423 botorch-0.8.5/botorch/sampling/pathwise/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/features/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/features/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/posterior_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/prior_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/update_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/qmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/stochastic_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.692423 botorch-0.8.5/botorch/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48773 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/multi_objective_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.700423 botorch-0.8.5/botorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/feasible_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20040 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/gp_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/low_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.700423 botorch-0.8.5/botorch/utils/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/dominated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/non_dominated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/botorch/utils/probability/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/bvn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/lin_ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/mvnxpb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/truncated_multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/unified_skew_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/safe_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36647 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.644423 botorch-0.8.5/botorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79395 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch_logo_lockup.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63261 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch_logo_lockup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 17:48:07.000000 botorch-0.8.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-05-08 17:48:07.000000 botorch-0.8.5/notebooks/tutorials_performance_tracking.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 17:48:07.000000 botorch-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 17:48:07.000000 botorch-0.8.5/requirements-fmt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 17:48:07.000000 botorch-0.8.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 17:50:32.704423 botorch-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 17:48:07.000000 botorch-0.8.5/setup.py
```

### Comparing `botorch-0.8.4/.conda/meta.yaml` & `botorch-0.8.5/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/ISSUE_TEMPLATE/bug_report.md` & `botorch-0.8.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md` & `botorch-0.8.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/ISSUE_TEMPLATE.md` & `botorch-0.8.5/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/PULL_REQUEST_TEMPLATE.md` & `botorch-0.8.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/deploy_on_release.yml` & `botorch-0.8.5/.github/workflows/deploy_on_release.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/docs.yml` & `botorch-0.8.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/lint.yml` & `botorch-0.8.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/nightly.yml` & `botorch-0.8.5/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/reusable_tutorials.yml` & `botorch-0.8.5/.github/workflows/reusable_tutorials.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/reusable_website.yml` & `botorch-0.8.5/.github/workflows/reusable_website.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/test.yml` & `botorch-0.8.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.github/workflows/test_stable.yml` & `botorch-0.8.5/.github/workflows/test_stable.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/.gitignore` & `botorch-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/CHANGELOG.md` & `botorch-0.8.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Changelog
 
 The release log for BoTorch.
 
+## [0.8.5] - May 8, 2023
+
+#### New Features
+* Support inferred noise in `SaasFullyBayesianMultiTaskGP` (#1809).
+
+#### Other Changes
+* More informative error message when `Standardize` has wrong batch shape (#1807).
+* Make GIBBON robust to numerical instability (#1814).
+* Add `sample_multiplier` in EUBO's `acqf_input_constructor` (#1816).
+
+#### Bug Fixes
+* Only do checks for `_optimize_acqf_sequential_q` when it will be used (#1808).
+* Fix an issue where `PairwiseGP` comparisons might be implicitly modified (#1811).
+
+
 ## [0.8.4] - Apr 24, 2023
 
 #### Compatibility
 * Require GPyTorch == 1.10 and linear_operator == 0.4.0 (#1803).
 
 #### New Features
 * Polytope sampling for linear constraints along the q-dimension (#1757).
```

### Comparing `botorch-0.8.4/CODE_OF_CONDUCT.md` & `botorch-0.8.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/CONTRIBUTING.md` & `botorch-0.8.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/LICENSE` & `botorch-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/PKG-INFO` & `botorch-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.8.4
+Version: 0.8.5
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.8.4 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.8.5 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
```

### Comparing `botorch-0.8.4/README.md` & `botorch-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/__init__.py` & `botorch-0.8.5/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/__init__.py` & `botorch-0.8.5/botorch/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/acquisition.py` & `botorch-0.8.5/botorch/acquisition/acquisition.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/active_learning.py` & `botorch-0.8.5/botorch/acquisition/active_learning.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/analytic.py` & `botorch-0.8.5/botorch/acquisition/analytic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/cached_cholesky.py` & `botorch-0.8.5/botorch/acquisition/cached_cholesky.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/cost_aware.py` & `botorch-0.8.5/botorch/acquisition/cost_aware.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/fixed_feature.py` & `botorch-0.8.5/botorch/acquisition/fixed_feature.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/input_constructors.py` & `botorch-0.8.5/botorch/acquisition/input_constructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1037,29 +1037,33 @@
 
 
 @acqf_input_constructor(AnalyticExpectedUtilityOfBestOption)
 def construct_inputs_analytic_eubo(
     model: Model,
     pref_model: Model,
     previous_winner: Optional[Tensor] = None,
+    sample_multiplier: Optional[float] = 1.0,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for the `AnalyticExpectedUtilityOfBestOption` constructor.
 
     Args:
         model: The outcome model to be used in the acquisition function.
-        pref_model: The preference model to be used in preference exploration
+        pref_model: The preference model to be used in preference exploration.
+        previous_winner: The previous winner of the best option.
+        sample_multiplier: The scale factor for the single-sample model.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
     # construct a deterministic fixed single sample model from `model`
     # i.e., performing EUBO-zeta by default as described
     # in https://arxiv.org/abs/2203.11382
-    one_sample_outcome_model = FixedSingleSampleModel(model=model)
+    w = torch.randn(model.num_outputs) * sample_multiplier
+    one_sample_outcome_model = FixedSingleSampleModel(model=model, w=w)
 
     return {
         "pref_model": pref_model,
         "outcome_model": one_sample_outcome_model,
         "previous_winner": previous_winner,
     }
 
@@ -1243,15 +1247,15 @@
     )
 
 
 @acqf_input_constructor(qJointEntropySearch)
 def construct_inputs_qJES(
     model: Model,
     training_data: MaybeDict[SupervisedDataset],
-    bounds: Tensor,
+    bounds: List[Tuple[float, float]],
     num_optima: int = 64,
     maximize: bool = True,
     condition_noiseless: bool = True,
     X_pending: Optional[Tensor] = None,
     estimation_type: str = "LB",
     num_samples: int = 64,
     **kwargs: Any,
```

### Comparing `botorch-0.8.4/botorch/acquisition/joint_entropy_search.py` & `botorch-0.8.5/botorch/acquisition/joint_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/knowledge_gradient.py` & `botorch-0.8.5/botorch/acquisition/knowledge_gradient.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/max_value_entropy_search.py` & `botorch-0.8.5/botorch/acquisition/max_value_entropy_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -643,19 +643,27 @@
             self.X_pending,
             observation_noise=True,
             posterior_transform=self.posterior_transform,
         ).distribution.covariance_matrix.unsqueeze(0)
         # 1 x m x m
 
         # use determinant of block matrix formula
-        V_determinant = variance_m - inv_quad(B, A.transpose(1, 2)).unsqueeze(1)
+        inv_quad_term = inv_quad(B, A.transpose(1, 2)).unsqueeze(1)
+        # NOTE: Even when using Cholesky to compute inv_quad, `V_determinant` can be
+        # negative due to numerical issues. To avoid this, we clamp the variance
+        # so that `V_determinant` > 0, while still allowing gradients to be
+        # propagated through `inv_quad_term`, as well as through `variance_m`
+        # in the expression for `r` below.
+        # choosing eps to be small while avoiding numerical underflow
+        eps = 1e-6 if inv_quad_term.dtype == torch.float32 else 1e-12
+        V_determinant = variance_m.clamp(inv_quad_term * (1 + eps)) - inv_quad_term
         # batch_shape x 1
 
         # Take logs and convert covariances to correlations.
-        r = V_determinant.log() - variance_m.log()
+        r = V_determinant.log() - variance_m.log()  # = log(1 - inv_quad / var)
         r = 0.5 * r.transpose(0, 1)
         return acq + r
 
 
 class qMultiFidelityMaxValueEntropy(qMaxValueEntropy):
     r"""Multi-fidelity max-value entropy.
```

### Comparing `botorch-0.8.4/botorch/acquisition/monte_carlo.py` & `botorch-0.8.5/botorch/acquisition/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/__init__.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/analytic.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/analytic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/joint_entropy_search.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/joint_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/max_value_entropy_search.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/max_value_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/monte_carlo.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/multi_fidelity.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/multi_output_risk_measures.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/multi_output_risk_measures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/objective.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/objective.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/predictive_entropy_search.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/predictive_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_objective/utils.py` & `botorch-0.8.5/botorch/acquisition/multi_objective/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/multi_step_lookahead.py` & `botorch-0.8.5/botorch/acquisition/multi_step_lookahead.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/objective.py` & `botorch-0.8.5/botorch/acquisition/objective.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/penalized.py` & `botorch-0.8.5/botorch/acquisition/penalized.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/predictive_entropy_search.py` & `botorch-0.8.5/botorch/acquisition/predictive_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/preference.py` & `botorch-0.8.5/botorch/acquisition/preference.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/proximal.py` & `botorch-0.8.5/botorch/acquisition/proximal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/risk_measures.py` & `botorch-0.8.5/botorch/acquisition/risk_measures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/acquisition/utils.py` & `botorch-0.8.5/botorch/acquisition/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/cross_validation.py` & `botorch-0.8.5/botorch/cross_validation.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/exceptions/__init__.py` & `botorch-0.8.5/botorch/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/exceptions/errors.py` & `botorch-0.8.5/botorch/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/exceptions/warnings.py` & `botorch-0.8.5/botorch/exceptions/warnings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/fit.py` & `botorch-0.8.5/botorch/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/generation/__init__.py` & `botorch-0.8.5/botorch/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/generation/gen.py` & `botorch-0.8.5/botorch/generation/gen.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/generation/sampling.py` & `botorch-0.8.5/botorch/generation/sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/generation/utils.py` & `botorch-0.8.5/botorch/generation/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/logging.py` & `botorch-0.8.5/botorch/logging.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/__init__.py` & `botorch-0.8.5/botorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/approximate_gp.py` & `botorch-0.8.5/botorch/models/approximate_gp.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/contextual.py` & `botorch-0.8.5/botorch/models/contextual.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/contextual_multioutput.py` & `botorch-0.8.5/botorch/models/contextual_multioutput.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/converter.py` & `botorch-0.8.5/botorch/models/converter.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/cost.py` & `botorch-0.8.5/botorch/models/cost.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/deterministic.py` & `botorch-0.8.5/botorch/models/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/ensemble.py` & `botorch-0.8.5/botorch/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/fully_bayesian.py` & `botorch-0.8.5/botorch/models/fully_bayesian.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/fully_bayesian_multitask.py` & `botorch-0.8.5/botorch/models/fully_bayesian_multitask.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,33 +43,29 @@
     is a Matern-5/2 kernel using learned task embeddings as the input.
     """
 
     def set_inputs(
         self,
         train_X: Tensor,
         train_Y: Tensor,
-        train_Yvar: Tensor,
+        train_Yvar: Optional[Tensor],
         task_feature: int,
         task_rank: Optional[int] = None,
     ):
         """Set the training data.
 
         Args:
             train_X: Training inputs (n x (d + 1))
             train_Y: Training targets (n x 1)
-            train_Yvar: Observed noise variance (n x 1).
+            train_Yvar: Observed noise variance (n x 1). If None, we infer the noise.
+                Note that the inferred noise is common across all tasks.
             task_feature: The index of the task feature (`-d <= task_feature <= d`).
             task_rank: The num of learned task embeddings to be used in the task kernel.
                 If omitted, set it to be 1.
         """
-        if (train_Yvar is None) or (torch.isnan(train_Yvar).all()):
-            # TODO: revisit inferred noise for batched MTGP
-            raise NotImplementedError(
-                "Currently do not support inferred noise for multitask GP with MCMC!"
-            )
         super().set_inputs(train_X, train_Y, train_Yvar)
         # obtain a list of task indicies
         all_tasks = train_X[:, task_feature].unique().to(dtype=torch.long).tolist()
         self.task_feature = task_feature
         self.num_tasks = len(all_tasks)
         self.task_rank = task_rank or 1
         # assume there is one column for task feature
@@ -193,62 +189,59 @@
         >>> posterior = mtsaas_gp.posterior(test_X)
     """
 
     def __init__(
         self,
         train_X: Tensor,
         train_Y: Tensor,
-        train_Yvar: Tensor,
+        train_Yvar: Optional[Tensor],
         task_feature: int,
         output_tasks: Optional[List[int]] = None,
         rank: Optional[int] = None,
         outcome_transform: Optional[OutcomeTransform] = None,
         input_transform: Optional[InputTransform] = None,
         pyro_model: Optional[PyroModel] = None,
     ) -> None:
         r"""Initialize the fully Bayesian multi-task GP model.
 
         Args:
             train_X: Training inputs (n x (d + 1))
             train_Y: Training targets (n x 1)
-            train_Yvar: Observed noise variance (n x 1).
+            train_Yvar: Observed noise variance (n x 1). If None, we infer the noise.
+                Note that the inferred noise is common across all tasks.
             task_feature: The index of the task feature (`-d <= task_feature <= d`).
             rank: The num of learned task embeddings to be used in the task kernel.
                 If omitted, set it to be 1.
         """
         if not (
             train_X.ndim == train_Y.ndim == 2
             and len(train_X) == len(train_Y)
             and train_Y.shape[-1] == 1
         ):
             raise ValueError(
                 "Expected train_X to have shape n x d and train_Y to have shape n x 1"
             )
-        if train_Yvar is None:
-            raise NotImplementedError(
-                "Inferred Noise is not supported in multitask SAAS GP."
+        if train_Yvar is not None and train_Y.shape != train_Yvar.shape:
+            raise ValueError(
+                "Expected train_Yvar to be None or have the same shape as train_Y"
             )
-        else:
-            if train_Y.shape != train_Yvar.shape:
-                raise ValueError(
-                    "Expected train_Yvar to be None or have the same shape as train_Y"
-                )
         with torch.no_grad():
             transformed_X = self.transform_inputs(
                 X=train_X, input_transform=input_transform
             )
         if outcome_transform is not None:
             train_Y, train_Yvar = outcome_transform(train_Y, train_Yvar)
-
-        train_Yvar = train_Yvar.clamp(MIN_INFERRED_NOISE_LEVEL)
+        if train_Yvar is not None:  # Clamp after transforming
+            train_Yvar = train_Yvar.clamp(MIN_INFERRED_NOISE_LEVEL)
 
         super().__init__(
             train_X=train_X,
             train_Y=train_Y,
-            train_Yvar=train_Yvar,
+            # Using train_Y as a dummy input here when train_Yvar is None.
+            train_Yvar=train_Yvar if train_Yvar is not None else train_Y,
             task_feature=task_feature,
             output_tasks=output_tasks,
         )
         self.to(train_X)
 
         self.mean_module = None
         self.covar_module = None
@@ -291,15 +284,16 @@
         self._check_if_fitted()
         return len(self.covar_module.outputscale)
 
     @property
     def batch_shape(self) -> torch.Size:
         r"""Batch shape of the model, equal to the number of MCMC samples.
         Note that `SaasFullyBayesianMultiTaskGP` does not support batching
-        over input data at this point."""
+        over input data at this point.
+        """
         self._check_if_fitted()
         return torch.Size([self.num_mcmc_samples])
 
     def fantasize(self, *args, **kwargs) -> NoReturn:
         raise NotImplementedError("Fantasize is not implemented!")
 
     def _check_if_fitted(self):
@@ -310,26 +304,24 @@
                 "`fit_fully_bayesian_model_nuts` to fit the model."
             )
 
     def load_mcmc_samples(self, mcmc_samples: Dict[str, Tensor]) -> None:
         r"""Load the MCMC hyperparameter samples into the model.
 
         This method will be called by `fit_fully_bayesian_model_nuts` when the model
-        has been fitted in order to create a batched SingleTaskGP model.
+        has been fitted in order to create a batched MultiTaskGP model.
         """
         (
             self.mean_module,
             self.covar_module,
             self.likelihood,
             self.task_covar_module,
             self.latent_features,
         ) = self.pyro_model.load_mcmc_samples(mcmc_samples=mcmc_samples)
 
-    # pyre-fixme[14]: Inconsistent override of
-    # BatchedMultiOutputGPyTorchModel.posterior
     def posterior(
         self,
         X: Tensor,
         output_indices: Optional[List[int]] = None,
         observation_noise: bool = False,
         posterior_transform: Optional[PosteriorTransform] = None,
         **kwargs: Any,
@@ -346,15 +338,14 @@
             observation_noise=observation_noise,
             posterior_transform=posterior_transform,
             **kwargs,
         )
         posterior = FullyBayesianPosterior(distribution=posterior.distribution)
         return posterior
 
-    # pyre-fixme[14]: Inconsistent override
     def forward(self, X: Tensor) -> MultivariateNormal:
         self._check_if_fitted()
         X = X.unsqueeze(MCMC_DIM)
 
         x_basic, task_idcs = self._split_inputs(X)
 
         mean_x = self.mean_module(x_basic)
@@ -375,15 +366,14 @@
 
         # Combine the two in an ICM fashion
         covar_i = self.task_covar_module(latent_features)
         covar = covar_x.mul(covar_i)
         return MultivariateNormal(mean_x, covar)
 
     @classmethod
-    # pyre-fixme[14]: Inconsistent override of `MultiTaskGP.construct_inputs`
     def construct_inputs(
         cls,
         training_data: Dict[str, SupervisedDataset],
         task_feature: int,
         rank: Optional[int] = None,
         **kwargs: Any,
     ) -> Dict[str, Any]:
@@ -391,13 +381,14 @@
 
         Args:
             training_data: Dictionary of `SupervisedDataset`.
             task_feature: Column index of embedded task indicator features. For details,
                 see `parse_training_data`.
             rank: The rank of the cross-task covariance matrix.
         """
-
         inputs = super().construct_inputs(
             training_data=training_data, task_feature=task_feature, rank=rank, **kwargs
         )
         inputs.pop("task_covar_prior")
+        if "train_Yvar" not in inputs:
+            inputs["train_Yvar"] = None
         return inputs
```

### Comparing `botorch-0.8.4/botorch/models/gp_regression.py` & `botorch-0.8.5/botorch/models/gp_regression.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/gp_regression_fidelity.py` & `botorch-0.8.5/botorch/models/gp_regression_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/gp_regression_mixed.py` & `botorch-0.8.5/botorch/models/gp_regression_mixed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/gpytorch.py` & `botorch-0.8.5/botorch/models/gpytorch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/higher_order_gp.py` & `botorch-0.8.5/botorch/models/higher_order_gp.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/kernels/__init__.py` & `botorch-0.8.5/botorch/models/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/kernels/categorical.py` & `botorch-0.8.5/botorch/models/kernels/categorical.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/kernels/contextual_lcea.py` & `botorch-0.8.5/botorch/models/kernels/contextual_lcea.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/kernels/contextual_sac.py` & `botorch-0.8.5/botorch/models/kernels/contextual_sac.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/kernels/downsampling.py` & `botorch-0.8.5/botorch/models/kernels/downsampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/kernels/exponential_decay.py` & `botorch-0.8.5/botorch/models/kernels/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/kernels/linear_truncated_fidelity.py` & `botorch-0.8.5/botorch/models/kernels/linear_truncated_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/likelihoods/pairwise.py` & `botorch-0.8.5/botorch/models/likelihoods/pairwise.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/model.py` & `botorch-0.8.5/botorch/models/model.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/model_list_gp_regression.py` & `botorch-0.8.5/botorch/models/model_list_gp_regression.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/multitask.py` & `botorch-0.8.5/botorch/models/multitask.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/pairwise_gp.py` & `botorch-0.8.5/botorch/models/pairwise_gp.py`

 * *Files 1% similar despite different names*

```diff
@@ -910,15 +910,19 @@
 
             if datapoints is not self.unconsolidated_datapoints:
                 raise RuntimeError("Must train on training data")
 
             # We pass in the untransformed datapoints into set_train_data
             # as we will be setting self.datapoints as the untransformed datapoints
             # self.transform_inputs will be called inside before calling _update()
-            self.set_train_data(datapoints, self.comparisons, update_model=True)
+            self.set_train_data(
+                datapoints=datapoints,
+                comparisons=self.unconsolidated_comparisons,
+                update_model=True,
+            )
 
             transformed_dp = self.transform_inputs(self.datapoints)
 
             hl = self.likelihood_hess
             covar = self.covar
 
             # Apply matrix inversion lemma on eq. in page 27 of [Brochu2010tutorial]_
@@ -1095,17 +1099,21 @@
             model: Used as in args to GPyTorch MarginalLogLikelihood
         """
         super().__init__(likelihood, model)
 
     def forward(self, post: Posterior, comp: Tensor) -> Tensor:
         r"""Calculate approximated log evidence, i.e., log(P(D|theta))
 
+        Note that post will be based on the consolidated/deduped datapoints for
+        numerical stability, but comp will still be the unconsolidated comparisons
+        so that it's still compatible with fit_gpytorch_*.
+
         Args:
-            post: training posterior distribution from self.model
-            comp: Comparisons pairs, see PairwiseGP.__init__ for more details
+            post: training posterior distribution from self.model (after consolidation)
+            comp: Comparisons pairs (before consolidation)
 
         Returns:
             The approximated evidence, i.e., the marginal log likelihood
         """
 
         model = self.model
         likelihood = self.likelihood
```

### Comparing `botorch-0.8.4/botorch/models/transforms/__init__.py` & `botorch-0.8.5/botorch/models/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/transforms/factory.py` & `botorch-0.8.5/botorch/models/transforms/factory.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/transforms/input.py` & `botorch-0.8.5/botorch/models/transforms/input.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/transforms/outcome.py` & `botorch-0.8.5/botorch/models/transforms/outcome.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,19 @@
             A two-tuple with the transformed outcomes:
 
             - The transformed outcome observations.
             - The transformed observation noise (if applicable).
         """
         if self.training:
             if Y.shape[:-2] != self._batch_shape:
-                raise RuntimeError("wrong batch shape")
+                raise RuntimeError(
+                    f"Expected Y.shape[:-2] to be {self._batch_shape}, matching "
+                    "the `batch_shape` argument to `Standardize`, but got "
+                    f"Y.shape[:-2]={Y.shape[:-2]}."
+                )
             if Y.size(-1) != self._m:
                 raise RuntimeError(
                     f"Wrong output dimension. Y.size(-1) is {Y.size(-1)}; expected "
                     f"{self._m}."
                 )
             stdvs = Y.std(dim=-2, keepdim=True)
             stdvs = stdvs.where(stdvs >= self._min_stdv, torch.full_like(stdvs, 1.0))
```

### Comparing `botorch-0.8.4/botorch/models/transforms/utils.py` & `botorch-0.8.5/botorch/models/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/utils/__init__.py` & `botorch-0.8.5/botorch/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/utils/assorted.py` & `botorch-0.8.5/botorch/models/utils/assorted.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/utils/inducing_point_allocators.py` & `botorch-0.8.5/botorch/models/utils/inducing_point_allocators.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/models/utils/parse_training_data.py` & `botorch-0.8.5/botorch/models/utils/parse_training_data.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/__init__.py` & `botorch-0.8.5/botorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/closures/__init__.py` & `botorch-0.8.5/botorch/optim/closures/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/closures/core.py` & `botorch-0.8.5/botorch/optim/closures/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/closures/model_closures.py` & `botorch-0.8.5/botorch/optim/closures/model_closures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/core.py` & `botorch-0.8.5/botorch/optim/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/fit.py` & `botorch-0.8.5/botorch/optim/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/initializers.py` & `botorch-0.8.5/botorch/optim/initializers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/numpy_converter.py` & `botorch-0.8.5/botorch/optim/numpy_converter.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/optimize.py` & `botorch-0.8.5/botorch/optim/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,41 +93,14 @@
         if self.inequality_constraints is None and not (
             self.bounds.ndim == 2 and self.bounds.shape[0] == 2
         ):
             raise ValueError(
                 "bounds should be a `2 x d` tensor, current shape: "
                 f"{list(self.bounds.shape)}."
             )
-        # validate that linear constraints across the q-dim and
-        # self.sequential are not present together
-        if self.inequality_constraints is not None and self.sequential is True:
-            for constraint in self.inequality_constraints:
-                if len(constraint[0].shape) > 1:
-                    raise UnsupportedError(
-                        "Linear inequality constraints across the q-dimension are not "
-                        "supported for sequential optimization."
-                    )
-        if self.equality_constraints is not None and self.sequential is True:
-            for constraint in self.equality_constraints:
-                if len(constraint[0].shape) > 1:
-                    raise UnsupportedError(
-                        "Linear equality constraints across the q-dimension are not "
-                        "supported for sequential optimization."
-                    )
-
-        # TODO: Validate constraints if provided:
-        # https://github.com/pytorch/botorch/pull/1231
-        if self.batch_initial_conditions is not None and self.sequential:
-            raise UnsupportedError(
-                "`batch_initial_conditions` is not supported for sequential "
-                "optimization. Either avoid specifying "
-                "`batch_initial_conditions` to use the custom initializer or "
-                "use the `ic_generator` kwarg to generate initial conditions "
-                "for the case of nonlinear inequality constraints."
-            )
 
         d = self.bounds.shape[1]
         if self.batch_initial_conditions is not None:
             batch_initial_conditions_shape = self.batch_initial_conditions.shape
             if len(batch_initial_conditions_shape) not in (2, 3):
                 raise ValueError(
                     "batch_initial_conditions must be 2-dimensional or "
@@ -148,25 +121,14 @@
                 )
             if self.raw_samples is None:
                 raise ValueError(
                     "Must specify `raw_samples` when "
                     "`batch_initial_conditions` is None`."
                 )
 
-        if self.sequential and self.q > 1:
-            if not self.return_best_only:
-                raise NotImplementedError(
-                    "`return_best_only=False` only supported for joint optimization."
-                )
-            if isinstance(self.acq_function, OneShotAcquisitionFunction):
-                raise NotImplementedError(
-                    "sequential optimization currently not supported for one-shot "
-                    "acquisition functions. Must have `sequential=False`."
-                )
-
     def get_ic_generator(self) -> TGenInitialConditions:
         if self.ic_generator is not None:
             return self.ic_generator
         elif isinstance(self.acq_function, qKnowledgeGradient):
             return gen_one_shot_kg_initial_conditions
         return gen_batch_initial_conditions
 
@@ -207,20 +169,61 @@
     )
     X = X.expand(q, *X.shape)
     with torch.no_grad():
         acq_value = acq_function(X)
     return X, acq_value
 
 
+def _validate_sequential_inputs(opt_inputs: OptimizeAcqfInputs) -> None:
+    # validate that linear constraints across the q-dim and
+    # self.sequential are not present together
+    if opt_inputs.inequality_constraints is not None:
+        for constraint in opt_inputs.inequality_constraints:
+            if len(constraint[0].shape) > 1:
+                raise UnsupportedError(
+                    "Linear inequality constraints across the q-dimension are not "
+                    "supported for sequential optimization."
+                )
+    if opt_inputs.equality_constraints is not None:
+        for constraint in opt_inputs.equality_constraints:
+            if len(constraint[0].shape) > 1:
+                raise UnsupportedError(
+                    "Linear equality constraints across the q-dimension are not "
+                    "supported for sequential optimization."
+                )
+
+    # TODO: Validate constraints if provided:
+    # https://github.com/pytorch/botorch/pull/1231
+    if opt_inputs.batch_initial_conditions is not None:
+        raise UnsupportedError(
+            "`batch_initial_conditions` is not supported for sequential "
+            "optimization. Either avoid specifying "
+            "`batch_initial_conditions` to use the custom initializer or "
+            "use the `ic_generator` kwarg to generate initial conditions "
+            "for the case of nonlinear inequality constraints."
+        )
+
+    if not opt_inputs.return_best_only:
+        raise NotImplementedError(
+            "`return_best_only=False` only supported for joint optimization."
+        )
+    if isinstance(opt_inputs.acq_function, OneShotAcquisitionFunction):
+        raise NotImplementedError(
+            "sequential optimization currently not supported for one-shot "
+            "acquisition functions. Must have `sequential=False`."
+        )
+
+
 def _optimize_acqf_sequential_q(
     opt_inputs: OptimizeAcqfInputs, timeout_sec: Optional[float], start_time: float
 ) -> Tuple[Tensor, Tensor]:
     """
     Helper function for `optimize_acqf` when sequential=True and q > 1.
     """
+    _validate_sequential_inputs(opt_inputs)
     if timeout_sec is not None:
         # When using sequential optimization, we allocate the total timeout
         # evenly across the individual acquisition optimizations.
         timeout_sec = (timeout_sec - start_time) / opt_inputs.q
 
     candidate_list, acq_value_list = [], []
     base_X_pending = opt_inputs.acq_function.X_pending
```

### Comparing `botorch-0.8.4/botorch/optim/parameter_constraints.py` & `botorch-0.8.5/botorch/optim/parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/stopping.py` & `botorch-0.8.5/botorch/optim/stopping.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/utils/__init__.py` & `botorch-0.8.5/botorch/optim/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/utils/acquisition_utils.py` & `botorch-0.8.5/botorch/optim/utils/acquisition_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/utils/common.py` & `botorch-0.8.5/botorch/optim/utils/common.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/utils/model_utils.py` & `botorch-0.8.5/botorch/optim/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/utils/numpy_utils.py` & `botorch-0.8.5/botorch/optim/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/optim/utils/timeout.py` & `botorch-0.8.5/botorch/optim/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/__init__.py` & `botorch-0.8.5/botorch/posteriors/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/base_samples.py` & `botorch-0.8.5/botorch/posteriors/base_samples.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/deterministic.py` & `botorch-0.8.5/botorch/posteriors/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/ensemble.py` & `botorch-0.8.5/botorch/posteriors/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/fully_bayesian.py` & `botorch-0.8.5/botorch/posteriors/fully_bayesian.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/gpytorch.py` & `botorch-0.8.5/botorch/posteriors/gpytorch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/higher_order.py` & `botorch-0.8.5/botorch/posteriors/higher_order.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/multitask.py` & `botorch-0.8.5/botorch/posteriors/multitask.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/posterior.py` & `botorch-0.8.5/botorch/posteriors/posterior.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/posterior_list.py` & `botorch-0.8.5/botorch/posteriors/posterior_list.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/torch.py` & `botorch-0.8.5/botorch/posteriors/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/posteriors/transformed.py` & `botorch-0.8.5/botorch/posteriors/transformed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/__init__.py` & `botorch-0.8.5/botorch/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/base.py` & `botorch-0.8.5/botorch/sampling/base.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/deterministic.py` & `botorch-0.8.5/botorch/sampling/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/get_sampler.py` & `botorch-0.8.5/botorch/sampling/get_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/index_sampler.py` & `botorch-0.8.5/botorch/sampling/index_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/list_sampler.py` & `botorch-0.8.5/botorch/sampling/list_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/normal.py` & `botorch-0.8.5/botorch/sampling/normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pairwise_samplers.py` & `botorch-0.8.5/botorch/sampling/pairwise_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/__init__.py` & `botorch-0.8.5/botorch/sampling/pathwise/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/features/__init__.py` & `botorch-0.8.5/botorch/sampling/pathwise/features/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/features/generators.py` & `botorch-0.8.5/botorch/sampling/pathwise/features/generators.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/features/maps.py` & `botorch-0.8.5/botorch/sampling/pathwise/features/maps.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/paths.py` & `botorch-0.8.5/botorch/sampling/pathwise/paths.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/posterior_samplers.py` & `botorch-0.8.5/botorch/sampling/pathwise/posterior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/prior_samplers.py` & `botorch-0.8.5/botorch/sampling/pathwise/prior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/update_strategies.py` & `botorch-0.8.5/botorch/sampling/pathwise/update_strategies.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/pathwise/utils.py` & `botorch-0.8.5/botorch/sampling/pathwise/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/qmc.py` & `botorch-0.8.5/botorch/sampling/qmc.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/sampling/stochastic_samplers.py` & `botorch-0.8.5/botorch/sampling/stochastic_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/settings.py` & `botorch-0.8.5/botorch/settings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/test_functions/__init__.py` & `botorch-0.8.5/botorch/test_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/test_functions/base.py` & `botorch-0.8.5/botorch/test_functions/base.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/test_functions/multi_fidelity.py` & `botorch-0.8.5/botorch/test_functions/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/test_functions/multi_objective.py` & `botorch-0.8.5/botorch/test_functions/multi_objective.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/test_functions/multi_objective_multi_fidelity.py` & `botorch-0.8.5/botorch/test_functions/multi_objective_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/test_functions/sensitivity_analysis.py` & `botorch-0.8.5/botorch/test_functions/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/test_functions/synthetic.py` & `botorch-0.8.5/botorch/test_functions/synthetic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/__init__.py` & `botorch-0.8.5/botorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/constants.py` & `botorch-0.8.5/botorch/utils/constants.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/constraints.py` & `botorch-0.8.5/botorch/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/containers.py` & `botorch-0.8.5/botorch/utils/containers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/context_managers.py` & `botorch-0.8.5/botorch/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/datasets.py` & `botorch-0.8.5/botorch/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/dispatcher.py` & `botorch-0.8.5/botorch/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/feasible_volume.py` & `botorch-0.8.5/botorch/utils/feasible_volume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/gp_sampling.py` & `botorch-0.8.5/botorch/utils/gp_sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/low_rank.py` & `botorch-0.8.5/botorch/utils/low_rank.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/__init__.py` & `botorch-0.8.5/botorch/utils/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/__init__.py` & `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition.py` & `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py` & `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/dominated.py` & `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/dominated.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/non_dominated.py` & `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/non_dominated.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/utils.py` & `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/hypervolume.py` & `botorch-0.8.5/botorch/utils/multi_objective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/pareto.py` & `botorch-0.8.5/botorch/utils/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/multi_objective/scalarization.py` & `botorch-0.8.5/botorch/utils/multi_objective/scalarization.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/objective.py` & `botorch-0.8.5/botorch/utils/objective.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/__init__.py` & `botorch-0.8.5/botorch/utils/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/bvn.py` & `botorch-0.8.5/botorch/utils/probability/bvn.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/lin_ess.py` & `botorch-0.8.5/botorch/utils/probability/lin_ess.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/linalg.py` & `botorch-0.8.5/botorch/utils/probability/linalg.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/mvnxpb.py` & `botorch-0.8.5/botorch/utils/probability/mvnxpb.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/truncated_multivariate_normal.py` & `botorch-0.8.5/botorch/utils/probability/truncated_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/unified_skew_normal.py` & `botorch-0.8.5/botorch/utils/probability/unified_skew_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/probability/utils.py` & `botorch-0.8.5/botorch/utils/probability/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/rounding.py` & `botorch-0.8.5/botorch/utils/rounding.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/safe_math.py` & `botorch-0.8.5/botorch/utils/safe_math.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/sampling.py` & `botorch-0.8.5/botorch/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/testing.py` & `botorch-0.8.5/botorch/utils/testing.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/torch.py` & `botorch-0.8.5/botorch/utils/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/transforms.py` & `botorch-0.8.5/botorch/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch/utils/types.py` & `botorch-0.8.5/botorch/utils/types.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch.egg-info/PKG-INFO` & `botorch-0.8.5/botorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.8.4
+Version: 0.8.5
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.8.4 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.8.5 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
```

### Comparing `botorch-0.8.4/botorch.egg-info/SOURCES.txt` & `botorch-0.8.5/botorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch_logo_lockup.png` & `botorch-0.8.5/botorch_logo_lockup.png`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/botorch_logo_lockup.svg` & `botorch-0.8.5/botorch_logo_lockup.svg`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/notebooks/tutorials_performance_tracking.ipynb` & `botorch-0.8.5/notebooks/tutorials_performance_tracking.ipynb`

 * *Files identical despite different names*

### Comparing `botorch-0.8.4/setup.py` & `botorch-0.8.5/setup.py`

 * *Files identical despite different names*


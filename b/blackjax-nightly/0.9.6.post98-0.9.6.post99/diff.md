# Comparing `tmp/blackjax-nightly-0.9.6.post98.tar.gz` & `tmp/blackjax-nightly-0.9.6.post99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackjax-nightly-0.9.6.post98.tar", last modified: Sun Jan  1 15:12:07 2023, max compression
+gzip compressed data, was "blackjax-nightly-0.9.6.post99.tar", last modified: Sun Jan  1 15:20:56 2023, max compression
```

## Comparing `blackjax-nightly-0.9.6.post98.tar` & `blackjax-nightly-0.9.6.post99.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.395051 blackjax-nightly-0.9.6.post98/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.379051 blackjax-nightly-0.9.6.post98/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.379051 blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/sampler_proposal.md
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.383051 blackjax-nightly-0.9.6.post98/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-01-01 15:12:07.395051 blackjax-nightly-0.9.6.post98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.383051 blackjax-nightly-0.9.6.post98/blackjax/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-01 15:12:07.000000 blackjax-nightly-0.9.6.post98/blackjax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.383051 blackjax-nightly-0.9.6.post98/blackjax/adaptation/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/adaptation/mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/adaptation/meads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/adaptation/pathfinder_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/adaptation/step_size.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/adaptation/window_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    42127 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.387051 blackjax-nightly-0.9.6.post98/blackjax/mcmc/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/elliptical_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/ghmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/irmh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/mala.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/marginal_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/periodic_orbital.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/rmh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/mcmc/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.387051 blackjax-nightly-0.9.6.post98/blackjax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/optimizers/dual_averaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/optimizers/lbfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.387051 blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/sghmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/sgld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.387051 blackjax-nightly-0.9.6.post98/blackjax/smc/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/smc/adaptive_tempered.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/smc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/smc/ess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/smc/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/smc/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/smc/tempered.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.387051 blackjax-nightly-0.9.6.post98/blackjax/vi/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/blackjax/vi/pathfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.387051 blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-01-01 15:12:07.000000 blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-01-01 15:12:07.000000 blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 15:12:07.000000 blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-01 15:12:07.000000 blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-01 15:12:07.000000 blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.387051 blackjax-nightly-0.9.6.post98/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.391051 blackjax-nightly-0.9.6.post98/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   161829 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/_static/blackjax.png
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/adaptation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/diagnostics.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.391051 blackjax-nightly-0.9.6.post98/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/GP_EllipticalSliceSampler.md
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/GP_Marginal.md
--rw-r--r--   0 runner    (1001) docker     (123)   479185 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/HierarchicalBNN.md
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/Introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/LogisticRegression.md
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/LogisticRegressionWithLatentGaussianSampler.md
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/Pathfinder.md
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/PeriodicOrbitalMCMC.md
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/RegimeSwitchingModel.md
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/SGMCMC.md
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/SparseLogisticRegression.md
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/TemperedSMC.md
--rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/change_of_variable_hmc.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.391051 blackjax-nightly-0.9.6.post98/docs/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    63251 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/data/google.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_custom_gradients.md
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_other_frameworks.md
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_sample_multiple_chains.md
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_use_aesara.md
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_use_numpyro.md
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_use_oryx.md
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_use_pymc.md
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples/howto_use_tfp.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/howto_use_ppl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/mcmc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/sgmcmc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/smc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/docs/vi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/jupytex.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-01-01 15:11:57.000000 blackjax-nightly-0.9.6.post98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-01 15:12:07.395051 blackjax-nightly-0.9.6.post98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:12:07.395051 blackjax-nightly-0.9.6.post98/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_compilation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_smc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_smc_ess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_step_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_tempered_smc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-01-01 15:11:55.000000 blackjax-nightly-0.9.6.post98/tests/test_uturn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.352807 blackjax-nightly-0.9.6.post99/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.340807 blackjax-nightly-0.9.6.post99/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.340807 blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/sampler_proposal.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.340807 blackjax-nightly-0.9.6.post99/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/workflows/publish_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-01-01 15:20:56.352807 blackjax-nightly-0.9.6.post99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.340807 blackjax-nightly-0.9.6.post99/blackjax/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-01 15:20:56.000000 blackjax-nightly-0.9.6.post99/blackjax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.340807 blackjax-nightly-0.9.6.post99/blackjax/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/adaptation/mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/adaptation/meads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/adaptation/pathfinder_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/adaptation/step_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/adaptation/window_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42127 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.344807 blackjax-nightly-0.9.6.post99/blackjax/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/elliptical_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/ghmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/irmh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/mala.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/marginal_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/periodic_orbital.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/rmh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/mcmc/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.344807 blackjax-nightly-0.9.6.post99/blackjax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/optimizers/dual_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/optimizers/lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.344807 blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/sghmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/sgld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.344807 blackjax-nightly-0.9.6.post99/blackjax/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/smc/adaptive_tempered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/smc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/smc/ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/smc/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/smc/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/smc/tempered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.344807 blackjax-nightly-0.9.6.post99/blackjax/vi/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/blackjax/vi/pathfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.344807 blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-01-01 15:20:56.000000 blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-01-01 15:20:56.000000 blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 15:20:56.000000 blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-01 15:20:56.000000 blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-01 15:20:56.000000 blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.348807 blackjax-nightly-0.9.6.post99/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.348807 blackjax-nightly-0.9.6.post99/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   161829 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/_static/blackjax.png
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/adaptation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/diagnostics.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.348807 blackjax-nightly-0.9.6.post99/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/GP_EllipticalSliceSampler.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/GP_Marginal.md
+-rw-r--r--   0 runner    (1001) docker     (123)   479185 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/HierarchicalBNN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/Introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/LogisticRegression.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/LogisticRegressionWithLatentGaussianSampler.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/Pathfinder.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/PeriodicOrbitalMCMC.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/RegimeSwitchingModel.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/SGMCMC.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/SparseLogisticRegression.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/TemperedSMC.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/change_of_variable_hmc.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.348807 blackjax-nightly-0.9.6.post99/docs/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    63251 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/data/google.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_custom_gradients.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_other_frameworks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_sample_multiple_chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_use_aesara.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_use_numpyro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_use_oryx.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_use_pymc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples/howto_use_tfp.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/howto_use_ppl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/mcmc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/sgmcmc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/smc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/docs/vi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/jupytex.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-01-01 15:20:40.000000 blackjax-nightly-0.9.6.post99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-01 15:20:56.352807 blackjax-nightly-0.9.6.post99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:56.352807 blackjax-nightly-0.9.6.post99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_compilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_smc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_smc_ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_step_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_tempered_smc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-01-01 15:20:38.000000 blackjax-nightly-0.9.6.post99/tests/test_uturn.py
```

### Comparing `blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/bug_report.yml` & `blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/enhancement.md` & `blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/ISSUE_TEMPLATE/sampler_proposal.md` & `blackjax-nightly-0.9.6.post99/.github/ISSUE_TEMPLATE/sampler_proposal.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/PULL_REQUEST_TEMPLATE.md` & `blackjax-nightly-0.9.6.post99/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/workflows/benchmark.yml` & `blackjax-nightly-0.9.6.post99/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/workflows/build_documentation.yml` & `blackjax-nightly-0.9.6.post99/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/workflows/nightly.yml` & `blackjax-nightly-0.9.6.post99/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/workflows/publish_documentation.yml` & `blackjax-nightly-0.9.6.post99/.github/workflows/publish_documentation.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/workflows/release.yml` & `blackjax-nightly-0.9.6.post99/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.github/workflows/test.yml` & `blackjax-nightly-0.9.6.post99/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.gitignore` & `blackjax-nightly-0.9.6.post99/.gitignore`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.gitlint` & `blackjax-nightly-0.9.6.post99/.gitlint`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/.pre-commit-config.yaml` & `blackjax-nightly-0.9.6.post99/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/LICENSE` & `blackjax-nightly-0.9.6.post99/LICENSE`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/PKG-INFO` & `blackjax-nightly-0.9.6.post99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax-nightly
-Version: 0.9.6.post98
+Version: 0.9.6.post99
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
```

### Comparing `blackjax-nightly-0.9.6.post98/README.md` & `blackjax-nightly-0.9.6.post99/README.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/__init__.py` & `blackjax-nightly-0.9.6.post99/blackjax/__init__.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/adaptation/mass_matrix.py` & `blackjax-nightly-0.9.6.post99/blackjax/adaptation/mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/adaptation/meads.py` & `blackjax-nightly-0.9.6.post99/blackjax/adaptation/meads.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/adaptation/pathfinder_adaptation.py` & `blackjax-nightly-0.9.6.post99/blackjax/adaptation/pathfinder_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/adaptation/step_size.py` & `blackjax-nightly-0.9.6.post99/blackjax/adaptation/step_size.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/adaptation/window_adaptation.py` & `blackjax-nightly-0.9.6.post99/blackjax/adaptation/window_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/base.py` & `blackjax-nightly-0.9.6.post99/blackjax/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/diagnostics.py` & `blackjax-nightly-0.9.6.post99/blackjax/diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/kernels.py` & `blackjax-nightly-0.9.6.post99/blackjax/kernels.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/diffusions.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/elliptical_slice.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/elliptical_slice.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/ghmc.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/ghmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/hmc.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/hmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/integrators.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/irmh.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/irmh.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/mala.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/mala.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/marginal_latent_gaussian.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/marginal_latent_gaussian.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/metrics.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/nuts.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/periodic_orbital.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/periodic_orbital.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/proposal.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/proposal.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/rmh.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/rmh.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/termination.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/termination.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/mcmc/trajectory.py` & `blackjax-nightly-0.9.6.post99/blackjax/mcmc/trajectory.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/optimizers/dual_averaging.py` & `blackjax-nightly-0.9.6.post99/blackjax/optimizers/dual_averaging.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/optimizers/lbfgs.py` & `blackjax-nightly-0.9.6.post99/blackjax/optimizers/lbfgs.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/progress_bar.py` & `blackjax-nightly-0.9.6.post99/blackjax/progress_bar.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/diffusions.py` & `blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/gradients.py` & `blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/gradients.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/sghmc.py` & `blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/sghmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/sgmcmc/sgld.py` & `blackjax-nightly-0.9.6.post99/blackjax/sgmcmc/sgld.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/smc/adaptive_tempered.py` & `blackjax-nightly-0.9.6.post99/blackjax/smc/adaptive_tempered.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/smc/base.py` & `blackjax-nightly-0.9.6.post99/blackjax/smc/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/smc/ess.py` & `blackjax-nightly-0.9.6.post99/blackjax/smc/ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/smc/resampling.py` & `blackjax-nightly-0.9.6.post99/blackjax/smc/resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/smc/solver.py` & `blackjax-nightly-0.9.6.post99/blackjax/smc/solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/smc/tempered.py` & `blackjax-nightly-0.9.6.post99/blackjax/smc/tempered.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/types.py` & `blackjax-nightly-0.9.6.post99/blackjax/types.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/util.py` & `blackjax-nightly-0.9.6.post99/blackjax/util.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax/vi/pathfinder.py` & `blackjax-nightly-0.9.6.post99/blackjax/vi/pathfinder.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/PKG-INFO` & `blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax-nightly
-Version: 0.9.6.post98
+Version: 0.9.6.post99
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
```

### Comparing `blackjax-nightly-0.9.6.post98/blackjax_nightly.egg-info/SOURCES.txt` & `blackjax-nightly-0.9.6.post99/blackjax_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/_static/blackjax.png` & `blackjax-nightly-0.9.6.post99/docs/_static/blackjax.png`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/_static/custom.css` & `blackjax-nightly-0.9.6.post99/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/conf.py` & `blackjax-nightly-0.9.6.post99/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 # line breaks in the signature when the typehints are present.
 autosummary_generate = True
 autodoc_typehints = "description"
 add_module_names = False
 
 source_suffix = {".rst": "restructuredtext", ".ipynb": "myst-nb", ".md": "myst-nb"}
 
-nb_execution_mode = "off"
+nb_execution_mode = "auto"
 nb_execution_timeout = 300
 suppress_warnings = ["mystnb.unknown_mime_type"]
 
 nb_custom_formats = {
     ".md": ["jupytext.reads", {"fmt": "mystnb"}],
 }
 myst_enable_extensions = ["colon_fence"]
```

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/GP_EllipticalSliceSampler.md` & `blackjax-nightly-0.9.6.post99/docs/examples/GP_EllipticalSliceSampler.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/GP_Marginal.md` & `blackjax-nightly-0.9.6.post99/docs/examples/GP_Marginal.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/HierarchicalBNN.md` & `blackjax-nightly-0.9.6.post99/docs/examples/HierarchicalBNN.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/Introduction.md` & `blackjax-nightly-0.9.6.post99/docs/examples/Introduction.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/LogisticRegression.md` & `blackjax-nightly-0.9.6.post99/docs/examples/LogisticRegression.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/LogisticRegressionWithLatentGaussianSampler.md` & `blackjax-nightly-0.9.6.post99/docs/examples/LogisticRegressionWithLatentGaussianSampler.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/Pathfinder.md` & `blackjax-nightly-0.9.6.post99/docs/examples/Pathfinder.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/PeriodicOrbitalMCMC.md` & `blackjax-nightly-0.9.6.post99/docs/examples/PeriodicOrbitalMCMC.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/README.md` & `blackjax-nightly-0.9.6.post99/docs/examples/README.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/RegimeSwitchingModel.md` & `blackjax-nightly-0.9.6.post99/docs/examples/RegimeSwitchingModel.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/SGMCMC.md` & `blackjax-nightly-0.9.6.post99/docs/examples/SGMCMC.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/SparseLogisticRegression.md` & `blackjax-nightly-0.9.6.post99/docs/examples/SparseLogisticRegression.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/TemperedSMC.md` & `blackjax-nightly-0.9.6.post99/docs/examples/TemperedSMC.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/change_of_variable_hmc.md` & `blackjax-nightly-0.9.6.post99/docs/examples/change_of_variable_hmc.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/data/google.csv` & `blackjax-nightly-0.9.6.post99/docs/examples/data/google.csv`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_custom_gradients.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_custom_gradients.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_other_frameworks.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_other_frameworks.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_sample_multiple_chains.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_sample_multiple_chains.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_use_aesara.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_use_aesara.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_use_numpyro.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_use_numpyro.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_use_oryx.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_use_oryx.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_use_pymc.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_use_pymc.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/examples/howto_use_tfp.md` & `blackjax-nightly-0.9.6.post99/docs/examples/howto_use_tfp.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/docs/index.md` & `blackjax-nightly-0.9.6.post99/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -77,25 +77,36 @@
 
 BlackJAX is written in pure Python but depends on XLA via JAX. By default, the
 version of JAX that will be installed along with BlackJAX will make your code
 run on CPU only. **If you want to use BlackJAX on GPU/TPU** we recommend you follow
 [these instructions](https://github.com/google/jax#installation) to install JAX
 with the relevant hardware acceleration support.
 
+```{toctree}
+---
+maxdepth: 1
+caption: PPL INTEGRATION
+hidden:
+---
+Aesara<examples/howto_use_aesara.md>
+Numpyro<examples/howto_use_numpyro.md>
+Oryx<examples/howto_use_oryx.md>
+PyMC<examples/howto_use_pymc.md>
+Tensorflow-Probability<examples/howto_use_tfp.md>
+```
 
 ```{toctree}
 ---
 maxdepth: 2
 caption: HOW TO
 hidden:
 ---
 Sample with multiple chains?<examples/howto_sample_multiple_chains.md>
 Use custom gradients?<examples/howto_custom_gradients.md>
 Use non-JAX log-prob functions?<examples/howto_other_frameworks.md>
-howto_use_ppl
 ```
 
 ```{toctree}
 ---
 maxdepth: 1
 caption: LEARN BY EXAMPLE
 hidden:
```

### Comparing `blackjax-nightly-0.9.6.post98/docs/mcmc.rst` & `blackjax-nightly-0.9.6.post99/docs/mcmc.rst`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/pyproject.toml` & `blackjax-nightly-0.9.6.post99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_adaptation.py` & `blackjax-nightly-0.9.6.post99/tests/test_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_benchmarks.py` & `blackjax-nightly-0.9.6.post99/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_compilation.py` & `blackjax-nightly-0.9.6.post99/tests/test_compilation.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_diagnostics.py` & `blackjax-nightly-0.9.6.post99/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_integrators.py` & `blackjax-nightly-0.9.6.post99/tests/test_integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_latent_gaussian.py` & `blackjax-nightly-0.9.6.post99/tests/test_latent_gaussian.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_mass_matrix.py` & `blackjax-nightly-0.9.6.post99/tests/test_mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_metrics.py` & `blackjax-nightly-0.9.6.post99/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_optimizers.py` & `blackjax-nightly-0.9.6.post99/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_pathfinder.py` & `blackjax-nightly-0.9.6.post99/tests/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_proposal.py` & `blackjax-nightly-0.9.6.post99/tests/test_proposal.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_resampling.py` & `blackjax-nightly-0.9.6.post99/tests/test_resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_sampling.py` & `blackjax-nightly-0.9.6.post99/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_smc.py` & `blackjax-nightly-0.9.6.post99/tests/test_smc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_smc_ess.py` & `blackjax-nightly-0.9.6.post99/tests/test_smc_ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_solver.py` & `blackjax-nightly-0.9.6.post99/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_step_size.py` & `blackjax-nightly-0.9.6.post99/tests/test_step_size.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_tempered_smc.py` & `blackjax-nightly-0.9.6.post99/tests/test_tempered_smc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_trajectory.py` & `blackjax-nightly-0.9.6.post99/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-0.9.6.post98/tests/test_uturn.py` & `blackjax-nightly-0.9.6.post99/tests/test_uturn.py`

 * *Files identical despite different names*


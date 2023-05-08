# Comparing `tmp/syne_tune-0.5.0.tar.gz` & `tmp/syne_tune-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syne_tune-0.5.0.tar", last modified: Thu Apr 20 13:27:06 2023, max compression
+gzip compressed data, was "syne_tune-0.6.0.tar", last modified: Mon May  8 09:47:34 2023, max compression
```

## Comparing `syne_tune-0.5.0.tar` & `syne_tune-0.6.0.tar`

### file list

```diff
@@ -1,290 +1,291 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-20 13:26:53.000000 syne_tune-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 13:26:53.000000 syne_tune-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 13:26:53.000000 syne_tune-0.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-04-20 13:27:06.302595 syne_tune-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-04-20 13:26:53.000000 syne_tune-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 13:27:06.302595 syne_tune-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-20 13:26:53.000000 syne_tune-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.282595 syne_tune-0.5.0/syne_tune/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/local_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/python_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/python_backend/python_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/python_backend/python_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/custom_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/simulator_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/trial_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/trial_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/tensorboard_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    43889 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/config_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/num_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36483 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_rush.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multi_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
--rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/random_seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/ray_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20877 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/duplicate_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    31946 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    42535 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    15446 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34001 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19578 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/remote_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/remote_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/remote_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/results_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/tuner_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/tuning_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/config_as_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/parse_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.282595 syne_tune-0.5.0/syne_tune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.953970 syne_tune-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-08 09:47:22.000000 syne_tune-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 09:47:22.000000 syne_tune-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 09:47:22.000000 syne_tune-0.6.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-05-08 09:47:34.953970 syne_tune-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-05-08 09:47:22.000000 syne_tune-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 09:47:34.953970 syne_tune-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-08 09:47:23.000000 syne_tune-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.929970 syne_tune-0.6.0/syne_tune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.929970 syne_tune-0.6.0/syne_tune/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/local_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/backend/python_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/python_backend/python_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/python_backend/python_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/custom_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/backend/simulator_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/trial_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/trial_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/tensorboard_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43889 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/config_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/experiments/experiment_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/experiments/results_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/num_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36483 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multi_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/random_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/ray_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21050 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15795 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42280 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34657 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/remote_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/remote_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/remote_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/results_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/tuner_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/tuning_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.953970 syne_tune-0.6.0/syne_tune/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/config_as_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/parse_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.929970 syne_tune-0.6.0/syne_tune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/top_level.txt
```

### Comparing `syne_tune-0.5.0/LICENSE` & `syne_tune-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/PKG-INFO` & `syne_tune-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne_tune
-Version: 0.5.0
+Version: 0.6.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `syne_tune-0.5.0/README.md` & `syne_tune-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/setup.py` & `syne_tune-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/__init__.py` & `syne_tune-0.6.0/syne_tune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/__init__.py` & `syne_tune-0.6.0/syne_tune/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/local_backend.py` & `syne_tune-0.6.0/syne_tune/backend/local_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 import logging
 import os
 import shutil
 import sys
-
+from operator import itemgetter
 import subprocess
 from datetime import datetime
 from pathlib import Path
 from typing import List, Optional, Tuple, Dict, Any
 
 from syne_tune.backend.trial_backend import TrialBackend, BUSY_STATUS
 from syne_tune.num_gpu import get_num_gpus
@@ -50,22 +50,26 @@
 
     :param entry_point: Path to Python main file to be tuned
     :param rotate_gpus: In case several GPUs are present, each trial is
         scheduled on a different GPU. A new trial is preferentially
         scheduled on a free GPU, and otherwise the GPU with least prior
         assignments is chosen. If ``False``, then all GPUs are used at the same
         time for all trials. Defaults to ``True``.
+    :param num_gpus_per_trial: Number of GPUs to be allocated to each trial.
+        Must be not larger than the total number of GPUs available.
+        Defaults to 1
     """
 
     def __init__(
         self,
         entry_point: str,
         delete_checkpoints: bool = False,
         pass_args_as_json: bool = False,
         rotate_gpus: bool = True,
+        num_gpus_per_trial: int = 1,
     ):
         super(LocalBackend, self).__init__(
             delete_checkpoints=delete_checkpoints, pass_args_as_json=pass_args_as_json
         )
 
         assert Path(
             entry_point
@@ -75,17 +79,19 @@
         self.trial_subprocess = dict()
 
         # GPU rotation
         # Note that the initialization is delayed until first used, so we can
         # be sure it happens on the instance running the training evaluations
         self.rotate_gpus = rotate_gpus
         self.num_gpus = None
+        # Maps ``trial_id`` to list of GPUs currently assigned to this trial
         self.trial_gpu = None
         self.gpu_times_assigned = None
-        # sets the path where to write files, can be overidden later by Tuner.
+        self.num_gpus_per_trial = num_gpus_per_trial
+        # sets the path where to write files, can be overridden later by Tuner.
         self.set_path(str(Path(experiment_path(tuner_name=random_string(length=10)))))
         # Trials which may currently be busy (status in ``BUSY_STATUS``). The
         # corresponding jobs are polled for status in ``busy_trial_ids``.
         self._busy_trial_id_candidates = set()
 
     def trial_path(self, trial_id: int) -> Path:
         """
@@ -120,46 +126,58 @@
         """
         if self.rotate_gpus and self.num_gpus is None:
             if num_gpus is None:
                 self.num_gpus = get_num_gpus()
             else:
                 self.num_gpus = num_gpus
             logger.info(f"Detected {self.num_gpus} GPUs")
+            if self.num_gpus_per_trial > self.num_gpus:
+                logger.warning(
+                    f"num_gpus_per_trial = {self.num_gpus_per_trial} is too "
+                    f"large, reducing to {self.num_gpus}"
+                )
+                self.num_gpus_per_trial = self.num_gpus
             if self.num_gpus > 1:
                 self.trial_gpu = dict()  # Maps running trials to GPUs
                 # To break ties among GPUs (free ones have precedence)
                 self.gpu_times_assigned = [0] * self.num_gpus
             else:
                 # Nothing to rotate over
                 self.rotate_gpus = False
 
-    def _gpu_for_new_trial(self) -> int:
+    def _gpus_for_new_trial(self) -> List[int]:
         """
-        Selects GPU for trial to be scheduled on. GPUs not assigned to other
-        running trials have precedence. Ties are resolved by selecting a GPU
-        with the least number of previous assignments.
-        The number of assignments is incremented for the GPU returned.
+        Selects ``num_gpus_per_trial`` GPUs for trial to be scheduled on. GPUs
+        not assigned to other running trials have precedence. Ties are resolved
+        by selecting GPUs with the least number of previous assignments.
+        The number of assignments is incremented for the GPUs returned.
         """
         assert self.rotate_gpus
-        free_gpus = set(range(self.num_gpus)).difference(self.trial_gpu.values())
-        if free_gpus:
-            eligible_gpus = free_gpus
-            logger.debug(f"Free GPUs: {free_gpus}")
+        assigned_gpus = list(gpu for gpus in self.trial_gpu.values() for gpu in gpus)
+        free_gpus = [x for x in range(self.num_gpus) if x not in assigned_gpus]
+        num_extra = self.num_gpus_per_trial - len(free_gpus)
+        if num_extra > 0:
+            candidate_gpus = assigned_gpus[:num_extra]
+            res_gpu = free_gpus  # Pick all free ones
         else:
-            eligible_gpus = range(self.num_gpus)
+            res_gpu = []
+            candidate_gpus = free_gpus
         # We select the GPU which has the least prior assignments. Selection
         # over all GPUs currently free. If all GPUs are currently assigned,
         # selection is over all GPUs. In this case, the assignment will go to
         # a GPU currently occupied (this happens if the number of GPUs is
         # smaller than the number of workers).
-        res_gpu, _ = min(
-            ((gpu, self.gpu_times_assigned[gpu]) for gpu in eligible_gpus),
-            key=lambda x: x[1],
-        )
-        self.gpu_times_assigned[res_gpu] += 1
+        num_extra = self.num_gpus_per_trial - len(res_gpu)
+        top_list = sorted(
+            ((gpu, self.gpu_times_assigned[gpu]) for gpu in candidate_gpus),
+            key=itemgetter(1),
+        )[:num_extra]
+        res_gpu = res_gpu + [gpu for gpu, _ in top_list]
+        for gpu in res_gpu:
+            self.gpu_times_assigned[gpu] += 1
         return res_gpu
 
     def _schedule(self, trial_id: int, config: Dict[str, Any]):
         self._prepare_for_schedule()
         trial_path = self.trial_path(trial_id)
         os.makedirs(trial_path, exist_ok=True)
         with open(trial_path / "std.out", "a") as stdout:
@@ -188,18 +206,20 @@
                 self.trial_subprocess[trial_id] = subprocess.Popen(
                     cmd.split(" "), stdout=stdout, stderr=stderr, env=env
                 )
         self._busy_trial_id_candidates.add(trial_id)  # Mark trial as busy
 
     def _allocate_gpu(self, trial_id: int, env: Dict[str, Any]):
         if self.rotate_gpus:
-            gpu = self._gpu_for_new_trial()
-            env["CUDA_VISIBLE_DEVICES"] = str(gpu)
-            self.trial_gpu[trial_id] = gpu
-            logger.debug(f"Assigned GPU {gpu} to trial_id {trial_id}")
+            gpus = self._gpus_for_new_trial()
+            env["CUDA_VISIBLE_DEVICES"] = ",".join(str(gpu) for gpu in gpus)
+            self.trial_gpu[trial_id] = gpus
+            part = f"GPU {gpus[0]}" if len(gpus) == 1 else f"GPUs {gpus}"
+            # logger.debug(f"Assigned {part} to trial_id {trial_id}")
+            logger.info(f"*** Assigned {part} to trial_id {trial_id}")  # DEBUG
 
     def _deallocate_gpu(self, trial_id: int):
         if self.rotate_gpus and trial_id in self.trial_gpu:
             del self.trial_gpu[trial_id]
 
     def _all_trial_results(self, trial_ids: List[int]) -> List[TrialResult]:
         res = []
```

### Comparing `syne_tune-0.5.0/syne_tune/backend/python_backend/__init__.py` & `syne_tune-0.6.0/syne_tune/backend/python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/python_backend/python_backend.py` & `syne_tune-0.6.0/syne_tune/backend/python_backend/python_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/python_backend/python_entrypoint.py` & `syne_tune-0.6.0/syne_tune/backend/python_backend/python_entrypoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/__init__.py` & `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/custom_framework.py` & `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/custom_framework.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv` & `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance_info.py` & `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance_info.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py` & `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 from syne_tune.backend.trial_status import TrialResult, Status
 from syne_tune.backend.sagemaker_backend.sagemaker_utils import (
     sagemaker_search,
     get_log,
     sagemaker_fit,
     add_syne_tune_dependency,
     map_identifier_limited_length,
-    s3_copy_files_recursively,
-    s3_delete_files_recursively,
+    s3_copy_objects_recursively,
+    s3_delete_objects_recursively,
     default_config,
     default_sagemaker_session,
     add_metric_definitions_to_sagemaker_estimator,
 )
 
 
 logger = logging.getLogger(__name__)
@@ -478,15 +478,15 @@
 
     def copy_checkpoint(self, src_trial_id: int, tgt_trial_id: int):
         s3_source_path = self._checkpoint_s3_uri_for_trial(src_trial_id)
         s3_target_path = self._checkpoint_s3_uri_for_trial(tgt_trial_id)
         logger.info(
             f"Copying checkpoint files from {s3_source_path} to " + s3_target_path
         )
-        result = s3_copy_files_recursively(s3_source_path, s3_target_path)
+        result = s3_copy_objects_recursively(s3_source_path, s3_target_path)
         num_action_calls = result["num_action_calls"]
         if num_action_calls == 0:
             logger.info(f"No checkpoint files found at {s3_source_path}")
         else:
             num_successful_action_calls = result["num_successful_action_calls"]
             assert num_successful_action_calls == num_action_calls, (
                 f"{num_successful_action_calls} files copied successfully, "
@@ -495,15 +495,15 @@
                 + result["first_error_message"]
             )
 
     def delete_checkpoint(self, trial_id: int):
         if trial_id in self._trial_ids_deleted_checkpoints:
             return
         s3_path = self._checkpoint_s3_uri_for_trial(trial_id)
-        result = s3_delete_files_recursively(s3_path)
+        result = s3_delete_objects_recursively(s3_path)
         self._trial_ids_deleted_checkpoints.add(trial_id)
         num_action_calls = result["num_action_calls"]
         if num_action_calls <= 0:
             return
         num_successful_action_calls = result["num_successful_action_calls"]
         if num_successful_action_calls == num_action_calls:
             logger.info(
```

### Comparing `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py` & `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 import os
 import re
 import subprocess
 import tarfile
 from ast import literal_eval
 from pathlib import Path
-from typing import List, Tuple, Dict, Optional, Any
+from typing import List, Tuple, Dict, Optional, Any, Callable
 
 import boto3
 from botocore.config import Config
 from botocore.exceptions import ClientError
 from sagemaker import Session
 from sagemaker.estimator import Framework, EstimatorBase
 
@@ -342,31 +342,37 @@
     else:
         assert 1 < rnd_digits < max_length
         postfix = random_string(rnd_digits)
         return name[: (max_length - rnd_digits)] + postfix
 
 
 def _s3_traverse_recursively(
-    s3_client, action, bucket: str, prefix: str
+    s3_client,
+    action: Callable[[str], Optional[str]],
+    bucket: str,
+    prefix: str,
+    valid_postfixes: Optional[List[str]] = None,
 ) -> Dict[str, Any]:
     """
     Traverses directory from root ``prefix``. The function ``action`` is applied
-    to all objects encountered, the signature is
-
-        ``action(s3_client, bucket, object_key)``
-
-    'action' returns None if successful, otherwise an error message.
-    We return a dict with 'num_action_calls', 'num_successful_action_calls',
-    'first_error_message' (the error message for the first failed ``action`` call
+    to all objects encountered, the signature is ``action(object_key)``.
+    ``action`` returns ``None`` if successful, otherwise an error message.
+    We return a dict with "num_action_calls", "num_successful_action_calls",
+    "first_error_message" (the error message for the first failed ``action`` call
     encountered).
 
+    If ``valid_postfixes`` is given, ``action`` is only applied to such
+    ``object_key`` for which ``object_key.endswith(postfix)`` for some
+    ``postfix in valid_postfixes``.
+
     :param s3_client: S3 client
     :param action: See above
     :param bucket: S3 bucket name
-    :param prefix: Prefix from where to traverse, must end with '/'
+    :param prefix: Prefix from where to traverse, must end with "/"
+    :param valid_postfixes: See above, optional
     :return: See above
     """
     more_objects = True
     continuation_kwargs = dict()
     list_objects_kwargs = dict(Bucket=bucket, Prefix=prefix, Delimiter="/")
     all_next_prefixes = []
     num_action_calls = 0
@@ -377,15 +383,20 @@
             **list_objects_kwargs, **continuation_kwargs
         )
         # Subdirectories
         for next_prefix in response.get("CommonPrefixes", []):
             all_next_prefixes.append(next_prefix["Prefix"])
         # Objects
         for source in response.get("Contents", []):
-            ret_msg = action(s3_client, bucket, source["Key"])
+            object_key = source["Key"]
+            if valid_postfixes is not None and not any(
+                object_key.endswith(postfix) for postfix in valid_postfixes
+            ):
+                continue  # Skip this key
+            ret_msg = action(object_key)
             num_action_calls += 1
             if ret_msg is None:
                 num_successful_action_calls += 1
             elif first_error_message is None:
                 first_error_message = ret_msg
         more_objects = "NextContinuationToken" in response
         if more_objects:
@@ -412,80 +423,138 @@
     bucket = parts[0]
     prefix = "/".join(parts[1:])
     if prefix[-1] != "/":
         prefix += "/"
     return bucket, prefix
 
 
-def s3_copy_files_recursively(
+def s3_copy_objects_recursively(
     s3_source_path: str, s3_target_path: str
 ) -> Dict[str, Any]:
     """
-    Recursively copies files from ``s3_source_path`` to ``s3_target_path``.
+    Recursively copies objects from ``s3_source_path`` to ``s3_target_path``.
 
     We return a dict with 'num_action_calls', 'num_successful_action_calls',
     'first_error_message' (the error message for the first failed ``action`` call
     encountered).
 
+    .. note::
+       This function should not be used to copy a large number of objects, as
+       it is rather slow (one API call for object)
+
     :param s3_source_path:
     :param s3_target_path:
     :return: See above
     """
     src_bucket, src_prefix = _split_bucket_prefix(s3_source_path)
     trg_bucket, trg_prefix = _split_bucket_prefix(s3_target_path)
+    s3_client = boto3.client("s3")
 
-    def copy_action(s3_client, bucket: str, object_key: str) -> Optional[str]:
+    def copy_action(object_key: str) -> Optional[str]:
         assert object_key.startswith(
             src_prefix
         ), f"object_key = {object_key} must start with {src_prefix}"
         target_key = trg_prefix + object_key[len(src_prefix) :]
-        copy_source = dict(Bucket=bucket, Key=object_key)
+        copy_source = dict(Bucket=src_bucket, Key=object_key)
         ret_msg = None
         try:
             s3_client.copy_object(
                 CopySource=copy_source, Bucket=trg_bucket, Key=target_key
             )
-            logger.debug(
-                f"Copied s3://{bucket}/{object_key}   to   s3://{trg_bucket}/{target_key}"
-            )
         except ClientError as ex:
             ret_msg = str(ex)
         return ret_msg
 
-    s3 = boto3.client("s3")
     return _s3_traverse_recursively(
-        s3_client=s3, action=copy_action, bucket=src_bucket, prefix=src_prefix
+        s3_client=s3_client, action=copy_action, bucket=src_bucket, prefix=src_prefix
     )
 
 
-def s3_delete_files_recursively(s3_path: str) -> Dict[str, Any]:
+def s3_delete_objects_recursively(s3_path: str) -> Dict[str, Any]:
     """
-    Recursively deletes files from ``s3_path``.
+    Recursively deletes objects from ``s3_path``.
 
     We return a dict with 'num_action_calls', 'num_successful_action_calls',
     'first_error_message' (the error message for the first failed ``action`` call
     encountered).
 
+    .. note::
+       This function should not be used to delete a large number of objects, as
+       it is rather slow (one API call for object)
+
     :param s3_path:
     :return: See above
     """
     bucket_name, prefix = _split_bucket_prefix(s3_path)
+    s3_client = boto3.client("s3")
+
+    def delete_action(object_key: str) -> Optional[str]:
+        ret_msg = None
+        try:
+            s3_client.delete_object(Bucket=bucket_name, Key=object_key)
+        except ClientError as ex:
+            ret_msg = str(ex)
+        return ret_msg
+
+    return _s3_traverse_recursively(
+        s3_client=s3_client, action=delete_action, bucket=bucket_name, prefix=prefix
+    )
 
-    def delete_action(s3_client, bucket: str, object_key: str) -> Optional[str]:
+
+def s3_download_files_recursively(
+    s3_source_path: str,
+    target_path: str,
+    valid_postfixes: Optional[List[str]] = None,
+) -> Dict[str, Any]:
+    """
+    Recursively downloads objects from ``s3_source_path`` and stores them locally
+    as files below ``target_path``
+
+    We return a dict with 'num_action_calls', 'num_successful_action_calls',
+    'first_error_message' (the error message for the first failed ``action`` call
+    encountered).
+
+    If ``valid_postfixes`` is given, only such objects are downloaded for which
+    ``object_key.endswith(postfix)`` for some ``postfix in valid_postfixes``.
+
+    .. note::
+       This function should not be used to download a large number of objects,
+       as it is rather slow (one API call for object). In this case, running
+       ``aws s3 sync`` can be much faster.
+
+    :param s3_source_path: See above
+    :param target_path: See above
+    :param valid_postfixes: See above, optional
+    :return: See above
+    """
+    src_bucket, src_prefix = _split_bucket_prefix(s3_source_path)
+    if target_path[-1] != "/":
+        target_path = target_path + "/"
+    s3_client = boto3.client("s3")
+
+    def download_action(object_key: str) -> Optional[str]:
+        assert object_key.startswith(
+            src_prefix
+        ), f"object_key = {object_key} must start with {src_prefix}"
+        target_file = target_path + object_key[len(src_prefix) :]
+        # Ensure that target directory exists
+        Path(target_file).parent.mkdir(exist_ok=True, parents=True)
         ret_msg = None
         try:
-            s3_client.delete_object(Bucket=bucket, Key=object_key)
-            logger.debug(f"Deleted s3://{bucket}/{object_key}")
+            s3_client.download_file(src_bucket, object_key, target_file)
         except ClientError as ex:
             ret_msg = str(ex)
         return ret_msg
 
-    s3 = boto3.client("s3")
     return _s3_traverse_recursively(
-        s3_client=s3, action=delete_action, bucket=bucket_name, prefix=prefix
+        s3_client=s3_client,
+        action=download_action,
+        bucket=src_bucket,
+        prefix=src_prefix,
+        valid_postfixes=valid_postfixes,
     )
 
 
 def backend_path_not_synced_to_s3() -> Path:
     """
     When an experiment with the local backend is run remotely (as SageMaker
     training job), we do not want checkpoints to be synced to S3, since this
```

### Comparing `syne_tune-0.5.0/syne_tune/backend/simulator_backend/__init__.py` & `syne_tune-0.6.0/syne_tune/backend/simulator_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/simulator_backend/events.py` & `syne_tune-0.6.0/syne_tune/backend/simulator_backend/events.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_backend.py` & `syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_callback.py` & `syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/simulator_backend/time_keeper.py` & `syne_tune-0.6.0/syne_tune/backend/simulator_backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/time_keeper.py` & `syne_tune-0.6.0/syne_tune/backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/trial_backend.py` & `syne_tune-0.6.0/syne_tune/backend/trial_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/backend/trial_status.py` & `syne_tune-0.6.0/syne_tune/backend/trial_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/__init__.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_offline.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_offline.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_surrogate.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_surrogate.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_tabular.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_tabular.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/utils.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/repository.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/repository.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/serialize.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/serialize.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/simulated_tabular_backend.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/simulated_tabular_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/blackbox_repository/utils.py` & `syne_tune-0.6.0/syne_tune/blackbox_repository/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/callbacks/__init__.py` & `syne_tune-0.6.0/syne_tune/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py` & `syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py` & `syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/callbacks/remove_checkpoints_callback.py` & `syne_tune-0.6.0/syne_tune/callbacks/remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/callbacks/tensorboard_callback.py` & `syne_tune-0.6.0/syne_tune/callbacks/tensorboard_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,19 +132,21 @@
         )
 
         self.iter += 1
 
     def _create_summary_writer(self):
         try:
             from tensorboardX import SummaryWriter
-        except ImportError:
-            logger.error(
-                "TensoboardX is not installed. You can install it via: pip install tensorboardX"
+        except ImportError as err:
+            print(
+                "TensorboardCallback requires tensorboardX to be installed:\n"
+                "   pip install tensorboardX\n\n" + str(err)
             )
             raise
+
         return SummaryWriter(self.output_path)
 
     def on_tuning_start(self, tuner):
         self.output_path = os.path.join(tuner.tuner_path, "tensorboard_output")
         self.writer = self._create_summary_writer()
         self.iter = 0
         self.start_time_stamp = perf_counter()
```

### Comparing `syne_tune-0.5.0/syne_tune/config_space.py` & `syne_tune-0.6.0/syne_tune/config_space.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/constants.py` & `syne_tune-0.6.0/syne_tune/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 
 ST_METADATA_FILENAME = "metadata.json"
 """Name for metadata file stored in ``Tuner``"""  # pylint: disable=W0105
 
 ST_TUNER_DILL_FILENAME = "tuner.dill"
 """Name for final tuner object file stored in ``Tuner``"""  # pylint: disable=W0105
 
+ST_DATETIME_FORMAT = "%Y-%m-%d-%H-%M-%S"
+"""Datetime format used in result path names"""  # pylint: disable=W0105
+
+
 # Limits
 
 MAX_METRICS_SUPPORTED_BY_SAGEMAKER = 40
 """Max number of metrics allowed for estimator"""  # pylint: disable=W0105
 
 TUNER_DEFAULT_SLEEP_TIME = 5.0
 """Default value for ``sleep_time``"""  # pylint: disable=W0105
```

### Comparing `syne_tune-0.5.0/syne_tune/experiments.py` & `syne_tune-0.6.0/syne_tune/experiments/experiment_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,35 @@
 from typing import List, Dict, Callable, Optional, Union, Any, Tuple
 
 import numpy as np
 import pandas as pd
 
 from syne_tune import Tuner
 from syne_tune.constants import (
-    ST_TUNER_TIME,
-    ST_TUNER_CREATION_TIMESTAMP,
     ST_METADATA_FILENAME,
     ST_RESULTS_DATAFRAME_FILENAME,
     ST_TUNER_DILL_FILENAME,
+    ST_TUNER_CREATION_TIMESTAMP,
+    ST_TUNER_TIME,
 )
 from syne_tune.optimizer.schedulers.multiobjective.utils import hypervolume_cumulative
-from syne_tune.try_import import try_import_aws_message
+from syne_tune.try_import import try_import_aws_message, try_import_visual_message
 from syne_tune.util import experiment_path, s3_experiment_path
 
 try:
     import boto3
     from botocore.exceptions import ClientError
 except ImportError:
     print(try_import_aws_message())
 
+try:
+    import matplotlib.pyplot as plt
+except ImportError:
+    print(try_import_visual_message())
+
 
 @dataclass
 class ExperimentResult:
     """
     Wraps results dataframe and provides retrieval services.
 
     :param name: Name of experiment
@@ -81,16 +86,14 @@
 
         :param reference_point: Reference point for hypervolume calculations.
             If None, the maximum values of each metric is used.
         :param figure_path: If specified, defines the path where the figure will be saved.
             If None, the figure is shown
         :param plt_kwargs: Arguments to :func:`matplotlib.pyplot.plot`
         """
-        import matplotlib.pyplot as plt
-
         if metrics_to_plot is None:
             metrics_to_plot = self.metric_names()
 
         assert (
             len(metrics_to_plot) > 1
         ), "Only one metric defined, cannot compute hypervolume"
 
@@ -127,16 +130,14 @@
 
         :param metric_to_plot: Indicates which metric to plot, can be the index or a name of the metric.
             default to 0 - first metric defined
         :param figure_path: If specified, defines the path where the figure will be saved.
             If None, the figure is shown
         :param plt_kwargs: Arguments to :func:`matplotlib.pyplot.plot`
         """
-        import matplotlib.pyplot as plt
-
         metric, metric_name, metric_mode = self._metric_name_mode(
             metric_to_plot, verbose=True
         )
 
         df = self.results
         if df is not None and len(df) > 0:
             df = df.sort_values(ST_TUNER_TIME)
```

### Comparing `syne_tune-0.5.0/syne_tune/num_gpu.py` & `syne_tune-0.6.0/syne_tune/num_gpu.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/baselines.py` & `syne_tune-0.6.0/syne_tune/optimizer/baselines.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/scheduler.py` & `syne_tune-0.6.0/syne_tune/optimizer/scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/fifo.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/fifo.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Optional, List, Dict, Any, Union
 import logging
 
+from syne_tune.optimizer.schedulers.random_seeds import RANDOM_SEED_UPPER_BOUND
 from syne_tune.optimizer.schedulers.searchers.searcher import BaseSearcher
 from syne_tune.optimizer.schedulers.searchers.searcher_factory import searcher_factory
 from syne_tune.optimizer.schedulers.searchers.utils.default_arguments import (
     check_and_merge_defaults,
     String,
     assert_no_invalid_options,
     Integer,
@@ -48,15 +49,15 @@
 
 _DEFAULT_OPTIONS = {
     "searcher": "random",
     "mode": "min",
 }
 
 _CONSTRAINTS = {
-    "random_seed": Integer(0, 2**32 - 1),
+    "random_seed": Integer(0, RANDOM_SEED_UPPER_BOUND),
     "max_resource_attr": String(),
     "max_t": Integer(1, None),
 }
 
 
 MetricModeType = Union[str, List[str]]
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_pasha.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_pasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_promotion.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_rush.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_stopping.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_stopping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/median_stopping_rule.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/median_stopping_rule.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multi_fidelity.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,15 @@
                     new_priority_rank = ranks[-1]
                     if new_priority_rank > 1 / self.rf:
                         action = SchedulerDecision.STOP
                 recorded[trial_id] = metrics
                 break
         return action
 
+    # TODO: Merge with plotting tools in ``experiments``
     def _plot(self, milestone, metric_recorded, priorities):
         """
         Plots the multiobjective candidates and the rank given by the multiobjective priority.
         """
         import numpy as np
         import matplotlib.pyplot as plt
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/utils.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/networks.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/networks.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/pbt.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/pbt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/random_seeds.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,16 +6,9 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-import numpy as np
-
-
-class RandomSeedGenerator:
-    def __init__(self, master_seed: int):
-        self._random_state = np.random.RandomState(master_seed)
-
-    def __call__(self) -> int:
-        return self._random_state.randint(0, 2**31 - 1)
+class SliceException(Exception):
+    pass
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/ray_scheduler.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/ray_scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/remove_checkpoints.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/remove_checkpoints.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/scheduler_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/scheduler_searcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Optional, Dict, Any
 import logging
-import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers import BaseSearcher
 from syne_tune.optimizer.scheduler import TrialSuggestion, TrialScheduler
-from syne_tune.optimizer.schedulers.random_seeds import RandomSeedGenerator
+from syne_tune.optimizer.schedulers.random_seeds import (
+    RandomSeedGenerator,
+    generate_random_seed,
+)
 from syne_tune.backend.trial_status import Trial
 
 logger = logging.getLogger(__name__)
 
 
 class TrialSchedulerWithSearcher(TrialScheduler):
     """
@@ -38,15 +40,15 @@
 
     def __init__(self, config_space: Dict[str, Any], **kwargs):
         super().__init__(config_space)
         self._searcher_initialized = False
         # Generator for random seeds
         random_seed = kwargs.get("random_seed")
         if random_seed is None:
-            random_seed = np.random.randint(0, 2**32)
+            random_seed = generate_random_seed()
         logger.info(f"Master random_seed = {random_seed}")
         self.random_seed_generator = RandomSeedGenerator(random_seed)
 
     @property
     def searcher(self) -> Optional[BaseSearcher]:
         raise NotImplementedError
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,39 +26,41 @@
 from syne_tune.optimizer.schedulers.searchers.random_grid_searcher import (  # noqa: F401
     RandomSearcher,
     GridSearcher,
 )
 from syne_tune.optimizer.schedulers.searchers.searcher_factory import (  # noqa: F401
     searcher_factory,
 )
+from syne_tune.optimizer.schedulers.searchers.model_based_searcher import (  # noqa: F401
+    ModelBasedSearcher,
+    BayesianOptimizationSearcher,
+)
 
 __all__ = [
     "BaseSearcher",
     "impute_points_to_evaluate",
     "StochasticSearcher",
     "StochasticAndFilterDuplicatesSearcher",
     "extract_random_seed",
     "RandomSearcher",
     "GridSearcher",
     "searcher_factory",
+    "ModelBasedSearcher",
+    "BayesianOptimizationSearcher",
 ]
 
 try:
-    from syne_tune.optimizer.schedulers.searchers.model_based_searcher import (  # noqa: F401
-        ModelBasedSearcher,
-    )
     from syne_tune.optimizer.schedulers.searchers.gp_fifo_searcher import (  # noqa: F401
         GPFIFOSearcher,
     )
     from syne_tune.optimizer.schedulers.searchers.gp_multifidelity_searcher import (  # noqa: F401
         GPMultiFidelitySearcher,
     )
 
     __all__.extend(
         [
-            "ModelBasedSearcher",
             "GPFIFOSearcher",
             "GPMultiFidelitySearcher",
         ]
     )
 except ImportError:
     logging.info(try_import_gpsearchers_message())
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Union, Dict, Optional, List
 from dataclasses import dataclass
 import numpy as np
 
 
-INTERNAL_METRIC_NAME = "active_metric"
+INTERNAL_METRIC_NAME = "target"
 
-INTERNAL_CONSTRAINT_NAME = "constraint_metric"
+INTERNAL_CONSTRAINT_NAME = "constraint"
 
-INTERNAL_COST_NAME = "cost_metric"
+INTERNAL_COST_NAME = "cost"
 
 
 def dictionarize_objective(x):
     return {INTERNAL_METRIC_NAME: x}
 
 
 MetricValues = Union[float, Dict[str, float]]
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     TrialEvaluations,
     PendingEvaluation,
     MetricValues,
     INTERNAL_METRIC_NAME,
 )
-from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
+from syne_tune.optimizer.schedulers.searchers.utils.common import (
+    Configuration,
+    ConfigurationFilter,
+)
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
     HyperparameterRanges,
 )
 
 
 class TuningJobState:
     """
@@ -298,7 +301,29 @@
         if self.hp_ranges != other.hp_ranges:
             return False
         if self.trials_evaluations != other.trials_evaluations:
             return False
         return self._map_configs_for_matching(
             self.config_for_trial
         ) == self._map_configs_for_matching(other.config_for_trial)
+
+    def all_configurations(
+        self, filter_observed_data: Optional[ConfigurationFilter] = None
+    ) -> List[Configuration]:
+        """
+        Returns list of configurations for all trials represented here, whether
+        observed, pending, or failed. If ``filter_observed_data`` is given, the
+        configurations for observed trials are filtered with this predicate.
+
+        :param filter_observed_data: See above, optional
+        :return: List of all configurations
+        """
+        _elist = [x.trial_id for x in self.pending_evaluations] + self.failed_trials
+        observed_trial_ids = [x.trial_id for x in self.trials_evaluations]
+        if filter_observed_data is not None:
+            observed_trial_ids = [
+                trial_id
+                for trial_id in observed_trial_ids
+                if filter_observed_data(self.config_for_trial[trial_id])
+            ]
+        _elist = set(_elist + observed_trial_ids)
+        return [self.config_for_trial[trial_id] for trial_id in _elist]
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py` & `syne_tune-0.6.0/syne_tune/utils/parse_bool.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,9 +6,16 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-class SliceException(Exception):
-    pass
+
+
+def parse_bool(val: str) -> bool:
+    val = val.upper()
+    if val == "TRUE":
+        return True
+    else:
+        assert val == "FALSE", f"val = '{val}' is not a boolean value"
+        return False
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.posterior_state import (
     PosteriorState,
     PosteriorStateWithSampleJoint,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.likelihood import (
     MarginalLikelihood,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.optimization_utils import (
     apply_lbfgs_with_multiple_starts,
     create_lbfgs_arguments,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -56,22 +55,21 @@
     def states(self) -> Optional[List[PosteriorState]]:
         """
         :return: Current posterior states (one per MCMC sample; just a single
             state if model parameters are optimized)
         """
         raise NotImplementedError
 
-    def fit(self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None):
+    def fit(self, data: Dict[str, Any]):
         """
         Adjust model parameters based on training data ``data``. Can be done via
         optimization or MCMC sampling. The posterior states are computed at the
         end as well.
 
         :param data: Training data
-        :param profiler: Used for profiling
         """
         raise NotImplementedError
 
     def recompute_states(self, data: Dict[str, Any]):
         """
         Recomputes posterior states for current model parameters.
 
@@ -210,27 +208,26 @@
     def states(self) -> Optional[List[PosteriorState]]:
         return self._states
 
     @property
     def likelihood(self) -> MarginalLikelihood:
         raise NotImplementedError
 
-    def fit(self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None):
+    def fit(self, data: Dict[str, Any]):
         """
         Fit the model parameters by optimizing the marginal likelihood,
         and set posterior states.
 
         We catch exceptions during the optimization restarts. If any restarts
         fail, log messages are written. If all restarts fail, the current
         parameters are not changed.
 
         :param data: Input data
-        :param profiler: Profiler, optional
         """
-        self.likelihood.on_fit_start(data, profiler)
+        self.likelihood.on_fit_start(data)
         if self.fit_reset_params:
             self.reset_params()
         n_starts = self.optimization_config.n_starts
         ret_infos = apply_lbfgs_with_multiple_starts(
             *create_lbfgs_arguments(
                 criterion=self.likelihood,
                 crit_args=[data],
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.posterior_state import (
     GaussProcPosteriorState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.slice import (
     SliceSampler,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 
 class GPRegressionMCMC(GaussianProcessModel):
     def __init__(
         self,
         build_kernel: Callable[[], KernelFunction],
         mcmc_config: MCMCConfig = DEFAULT_MCMC_CONFIG,
@@ -66,15 +65,15 @@
     def states(self) -> Optional[List[GaussProcPosteriorState]]:
         return self._states
 
     @property
     def number_samples(self) -> int:
         return self.mcmc_config.n_samples
 
-    def fit(self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None):
+    def fit(self, data: Dict[str, Any]):
         features, targets = self._check_features_targets(
             features=data["features"], targets=data["targets"]
         )
         assert (
             targets.shape[1] == 1
         ), "targets cannot be a matrix if parameters are to be fit"
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.mean import (
     MeanFunction,
     ScalarMeanFunction,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.target_transform import (
     ScalarTargetTransform,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 
 @dataclass
 class HyperTuneDistributionArguments:
     num_samples: int
     num_brackets: Optional[int] = None
 
@@ -221,16 +220,16 @@
 
     def hypertune_ensemble_distribution(self) -> Optional[Dict[int, float]]:
         if self._likelihood is not None:
             return self._likelihood.ensemble_distribution
         else:
             return None
 
-    def fit(self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None):
-        super().fit(data, profiler)
+    def fit(self, data: Dict[str, Any]):
+        super().fit(data)
         poster_state: IndependentGPPerResourcePosteriorState = self.states[0]
         ensemble_distribution = self.fit_distributions(
             poster_state=poster_state,
             data=data,
             resource_attr_range=self._resource_attr_range,
             random_state=self.random_state,
         )
@@ -312,16 +311,16 @@
 
     def hypertune_ensemble_distribution(self) -> Optional[Dict[int, float]]:
         if self._likelihood is not None:
             return self._likelihood.ensemble_distribution
         else:
             return None
 
-    def fit(self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None):
-        super().fit(data, profiler)
+    def fit(self, data: Dict[str, Any]):
+        super().fit(data)
         resource_attr_range = self._likelihood_kwargs["resource_attr_range"]
         poster_state = GaussProcPosteriorStateAndRungLevels(
             poster_state=self.states[0],
             rung_levels=self._rung_levels,
         )
         ensemble_distribution = self.fit_distributions(
             poster_state=poster_state,
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,14 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.posterior_state import (
     PosteriorState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.target_transform import (
     ScalarTargetTransform,
     IdentityTargetTransform,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import (
-    SimpleProfiler,
-)
 
 
 class IndependentGPPerResourceMarginalLikelihood(MarginalLikelihood):
     r"""
     Marginal likelihood for GP multi-fidelity model over :math:`f(x, r)`,
     where for each :math:`r`, :math:`f(x, r)` is represented by an independent
     GP. The different processes share the same kernel, but have their own mean
@@ -261,16 +258,14 @@
             for resource in self.noise_variance_internal.keys():
                 self._set_noise_variance(
                     resource, param_dict[f"noise_variance{resource}"]
                 )
         else:
             self._set_noise_variance(1, param_dict["noise_variance"])
 
-    def on_fit_start(
-        self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None
-    ):
+    def on_fit_start(self, data: Dict[str, Any]):
         GaussianProcessMarginalLikelihood.assert_data_entries(data)
         targets = data["targets"]
         assert (
             targets.shape[1] == 1
         ), "targets cannot be a matrix if parameters are to be fit"
         self.target_transform.on_fit_start(targets)
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import List, Dict, Optional, Tuple
+from typing import List, Dict, Tuple
 
 import numpy as np
 import scipy.linalg as spl
 import autograd.numpy as anp
 from autograd.scipy.special import logsumexp
 from autograd.scipy.linalg import solve_triangular
 from autograd.tracer import getval
@@ -37,15 +37,14 @@
     FantasizedPendingEvaluation,
     TrialEvaluations,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.config_ext import (
     ExtendedConfiguration,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 
 def _prepare_data_internal(
     state: TuningJobState,
     data_lst: List[Tuple[Configuration, List, str]],
     config_space_ext: ExtendedConfiguration,
     active_metric: str,
@@ -400,15 +399,14 @@
 
 def issm_likelihood_computations(
     precomputed: Dict,
     issm_params: Dict,
     r_min: int,
     r_max: int,
     skip_c_d: bool = False,
-    profiler: Optional[SimpleProfiler] = None,
 ) -> Dict:
     """
     Given ``precomputed`` from ``issm_likelihood_precomputations`` and ISSM
     parameters ``issm_params``, compute quantities required for inference and
     marginal likelihood computation, pertaining to the ISSM likelihood.
 
     The index for r is range(r_min, r_max + 1). Observations must be contiguous
@@ -445,16 +443,14 @@
     assert n == num_all_configs, f"alpha.size = {n} != {num_all_configs}"
     n = getval(betas.size)
     assert n == num_all_configs, f"beta.size = {n} != {num_all_configs}"
 
     if not skip_c_d:
         # We could probably refactor this to fit into the loop below, but it
         # seems subdominant
-        if profiler is not None:
-            profiler.start("issm_part1")
         c_lst = []
         d_lst = []
         for i, ydim in enumerate(precomputed["ydims"]):
             alpha = alphas[i]
             alpha_m1 = alpha - 1.0
             beta = betas[i]
             r_obs = r_min + ydim  # Observed in range(r_min, r_obs)
@@ -468,20 +464,16 @@
                 c_scal = alpha * anp.exp(logsumexp(lrvec))
                 d_scal = anp.square(gamma * alpha) * anp.exp(logsumexp(lrvec * 2.0))
                 c_lst.append(c_scal)
                 d_lst.append(d_scal)
             else:
                 c_lst.append(0.0)
                 d_lst.append(0.0)
-        if profiler is not None:
-            profiler.stop("issm_part1")
 
     # Loop over ydim
-    if profiler is not None:
-        profiler.start("issm_part2")
     deltay = precomputed["deltay"]
     logr = precomputed["logr"]
     off_dely = num_all_configs
     vvec = anp.ones(off_dely)
     wmat = deltay[:off_dely, :]  # [y_0]
     vtv = anp.ones(off_dely)
     wtv = wmat.copy()
@@ -530,16 +522,14 @@
     vtv_lst.append(vtv)
     wtv_lst.append(wtv)
     vtv_all = anp.concatenate(tuple(reversed(vtv_lst)), axis=0)
     wtv_all = anp.concatenate(tuple(reversed(wtv_lst)), axis=0)
     if compute_wtw:
         wtw_lst.append(wtw)
         wtw_all = anp.concatenate(tuple(reversed(wtw_lst)), axis=0)
-    if profiler is not None:
-        profiler.stop("issm_part2")
 
     # Compile results
     result = {"num_data": sum(precomputed["ydims"]), "vtv": vtv_all, "wtv": wtv_all}
     if compute_wtw:
         result["wtw"] = wtw_all
     if not skip_c_d:
         result["c"] = anp.array(c_lst)
@@ -889,15 +879,14 @@
 
 def issm_likelihood_slow_computations(
     targets: List[np.ndarray],
     issm_params: Dict,
     r_min: int,
     r_max: int,
     skip_c_d: bool = False,
-    profiler: Optional[SimpleProfiler] = None,
 ) -> Dict:
     """
     Naive implementation of ``issm_likelihood_computations``, which does not
     require precomputations, but is much slower. Here, results are computed
     one datapoint at a time, instead of en bulk.
 
     This code is used in unit testing, and called from ``sample_posterior_joint``.
@@ -922,16 +911,14 @@
     wtw_lst = []
     num_data = 0
     for i, ymat in enumerate(targets):
         alpha = alphas[i]
         alpha_m1 = alpha - 1.0
         beta = betas[i]
         ydim = ymat.shape[0]
-        if profiler is not None:
-            profiler.start("issm_part1")
         num_data += ydim
         r_obs = r_min + ydim  # Observed in range(r_min, r_obs)
         assert 0 < ydim <= num_res, f"len(y[{i}]) = {ydim}, num_res = {num_res}"
         if not skip_c_d:
             # c_i, d_i
             if ydim < num_res:
                 lrvec = (
@@ -942,17 +929,14 @@
                 d_scal = anp.square(gamma * alpha) * anp.exp(logsumexp(lrvec * 2.0))
                 c_lst.append(c_scal)
                 d_lst.append(d_scal)
             else:
                 c_lst.append(0.0)
                 d_lst.append(0.0)
         # Inner loop for v_i, w_i
-        if profiler is not None:
-            profiler.stop("issm_part1")
-            profiler.start("issm_part2")
         yprev = ymat[-1].reshape((1, -1))  # y_{j-1} (vector)
         vprev = 1.0  # v_{j-1} (scalar)
         wprev = yprev  # w_{j-1} (row vector)
         vtv = vprev * vprev  # scalar
         wtv = wprev * vprev  # row vector
         if compute_wtw:
             wtw = wprev * wprev  # shape (1, 1)
@@ -971,16 +955,14 @@
             vprev = vcurr
             wprev = wcurr
         vtv_lst.append(vtv)
         wtv_lst.append(wtv)
         if compute_wtw:
             assert wtw.shape == (1, 1)
             wtw_lst.append(wtw.item())
-        if profiler is not None:
-            profiler.stop("issm_part2")
     # Compile results
     result = {
         "num_data": num_data,
         "vtv": anp.array(vtv_lst),
         "wtv": anp.vstack(wtv_lst),
     }
     if compute_wtw:
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.kernel import (
     KernelFunction,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.mean import (
     ScalarMeanFunction,
     MeanFunction,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 
 LCModel = Union[ISSModelParameters, ExponentialDecayBaseKernelFunction]
 
 
 class GaussAdditiveMarginalLikelihood(MarginalLikelihood):
     """
@@ -119,29 +118,24 @@
                 "res_kernel": self.res_model,
             }
         self._components = [
             ("kernel_", self.kernel),
             ("mean_", self.mean),
             (tag, self.res_model),
         ]
-        self._profiler = None
         with self.name_scope():
             self.noise_variance_internal = register_parameter(
                 self.params, "noise_variance", self.encoding
             )
 
-    def set_profiler(self, profiler: Optional[SimpleProfiler]):
-        self._profiler = profiler
-
     def get_posterior_state(self, data: Dict[str, Any]) -> PosteriorState:
         return self._type(
             data,
             **self._posterstate_kwargs,
             noise_variance=self.get_noise_variance(),
-            profiler=self._profiler
         )
 
     def forward(self, data: Dict[str, Any]):
         assert not data["do_fantasizing"], (
             "data must not be for fantasizing. Call prepare_data with "
             + "do_fantasizing=False"
         )
@@ -180,17 +174,13 @@
             func.set_params(stripped_dict)
         self._set_noise_variance(param_dict["noise_variance"])
 
     def data_precomputations(self, data: Dict[str, Any], overwrite: bool = False):
         if overwrite or not self._type.has_precomputations(data):
             self._type.data_precomputations(data)
 
-    def on_fit_start(
-        self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None
-    ):
+    def on_fit_start(self, data: Dict[str, Any]):
         assert not data["do_fantasizing"], (
             "data must not be for fantasizing. Call prepare_data with "
             + "do_fantasizing=False"
         )
         self.data_precomputations(data)
-        if profiler is not None:
-            self.set_profiler(profiler)
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -448,44 +448,37 @@
         super().__init__(data, mean, kernel, noise_variance=noise_variance, **kwargs)
 
     @staticmethod
     def has_precomputations(data: Dict[str, Any]) -> bool:
         return all(k in data for k in ("ydims", "num_configs", "deltay", "logr"))
 
     def _compute_posterior_state(self, data: Dict[str, Any], noise_variance, **kwargs):
-        profiler = kwargs.get("profiler")
         # Compute posterior state
         issm_params = self.iss_model.get_issm_params(data["features"])
         if self.has_precomputations(data):
             issm_likelihood = issm_likelihood_computations(
                 precomputed=data,
                 issm_params=issm_params,
                 r_min=self.r_min,
                 r_max=self.r_max,
-                profiler=profiler,
             )
         else:
             issm_likelihood = issm_likelihood_slow_computations(
                 targets=data["targets"],
                 issm_params=issm_params,
                 r_min=self.r_min,
                 r_max=self.r_max,
-                profiler=profiler,
             )
-        if profiler is not None:
-            profiler.start("poster_comp")
         self.poster_state = posterior_computations(
             features=data["features"],
             mean=self.mean,
             kernel=self.kernel,
             issm_likelihood=issm_likelihood,
             noise_variance=noise_variance,
         )
-        if profiler is not None:
-            profiler.stop("poster_comp")
 
     def predict(self, test_features: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         resource_attr_range = (self.r_min, self.r_max)
         features, resources = decode_extended_features(
             test_features, resource_attr_range=resource_attr_range
         )
         issm_params = self.iss_model.get_issm_params(features)
@@ -606,42 +599,34 @@
         )
 
     @staticmethod
     def has_precomputations(data: Dict[str, Any]) -> bool:
         return all(k in data for k in ("ydims", "num_configs", "yflat"))
 
     def _compute_posterior_state(self, data: Dict[str, Any], noise_variance, **kwargs):
-        profiler = kwargs.get("profiler")
         # Compute posterior state
-        if profiler is not None:
-            profiler.start("likelihood")
         if self.has_precomputations(data):
             issm_likelihood = resource_kernel_likelihood_computations(
                 precomputed=data,
                 res_kernel=self.res_kernel,
                 noise_variance=noise_variance,
             )
         else:
             issm_likelihood = resource_kernel_likelihood_slow_computations(
                 targets=data["targets"],
                 res_kernel=self.res_kernel,
                 noise_variance=noise_variance,
             )
-        if profiler is not None:
-            profiler.stop("likelihood")
-            profiler.start("poster_comp")
         self.poster_state = posterior_computations(
             features=data["features"],
             mean=self.mean,
             kernel=self.kernel,
             issm_likelihood=issm_likelihood,
             noise_variance=noise_variance,
         )
-        if profiler is not None:
-            profiler.stop("poster_comp")
         # Add missing term to criterion value
         if "criterion" in self.poster_state:
             part3 = logdet_cholfact_cov_resource(issm_likelihood)
             self.poster_state["criterion"] += part3
         # Extra terms required in ``sample_curves``
         self.poster_state["lfact_all"] = issm_likelihood["lfact_all"]
         self.poster_state["means_all"] = issm_likelihood["means_all"]
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,14 @@
     PosteriorState,
     GaussProcPosteriorState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.target_transform import (
     ScalarTargetTransform,
     IdentityTargetTransform,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import (
-    SimpleProfiler,
-)
 
 
 class MarginalLikelihood(Block):
     """
     Interface for marginal likelihood of Gaussian-linear model.
     """
 
@@ -107,22 +104,19 @@
         included in ``data``, unless ``overwrite`` is True.
 
         :param data:
         :param overwrite:
         """
         pass
 
-    def on_fit_start(
-        self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None
-    ):
+    def on_fit_start(self, data: Dict[str, Any]):
         """
         Called at the beginning of ``fit``.
 
         :param data: Argument passed to ``fit``
-        :param profiler: Argument passed to ``fit``
 
         """
         raise NotImplementedError
 
 
 class GaussianProcessMarginalLikelihood(MarginalLikelihood):
     """
@@ -242,17 +236,15 @@
             len_pref = len(pref)
             stripped_dict = {
                 k[len_pref:]: v for k, v in param_dict.items() if k.startswith(pref)
             }
             func.set_params(stripped_dict)
         self._set_noise_variance(param_dict["noise_variance"])
 
-    def on_fit_start(
-        self, data: Dict[str, Any], profiler: Optional[SimpleProfiler] = None
-    ):
+    def on_fit_start(self, data: Dict[str, Any]):
         self.assert_data_entries(data)
         targets = data["targets"]
         assert (
             targets.shape[1] == 1
         ), "targets cannot be a matrix if parameters are to be fit"
         self.target_transform.on_fit_start(targets)
         targets = self.target_transform(targets)
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.gp_model import (
     GaussProcModelFactory,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     INTERNAL_METRIC_NAME,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import ConfigurationFilter
 
 logger = logging.getLogger(__name__)
 
@@ -50,24 +49,22 @@
     """
 
     def __init__(
         self,
         gpmodel: GPRegressionMCMC,
         active_metric: str = INTERNAL_METRIC_NAME,
         normalize_targets: bool = True,
-        profiler: Optional[SimpleProfiler] = None,
         debug_log: Optional[DebugLogPrinter] = None,
         filter_observed_data: Optional[ConfigurationFilter] = None,
         hp_ranges_for_prediction: Optional[HyperparameterRanges] = None,
     ):
         super().__init__(
             gpmodel=gpmodel,
             active_metric=active_metric,
             normalize_targets=normalize_targets,
-            profiler=profiler,
             debug_log=debug_log,
             filter_observed_data=filter_observed_data,
             hp_ranges_for_prediction=hp_ranges_for_prediction,
         )
 
     def get_params(self):
         return dict()  # Model has no parameters to be fit
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     SurrogateModel,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 logger = logging.getLogger(__name__)
 
 
 GPModel = Union[
     GaussianProcessRegression,
     GPRegressionMCMC,
@@ -247,40 +246,34 @@
     """
 
     def __init__(
         self,
         gpmodel: GPModel,
         active_metric: str,
         normalize_targets: bool = True,
-        profiler: Optional[SimpleProfiler] = None,
         debug_log: Optional[DebugLogPrinter] = None,
         filter_observed_data: Optional[ConfigurationFilter] = None,
         no_fantasizing: bool = False,
         hp_ranges_for_prediction: Optional[HyperparameterRanges] = None,
     ):
         self._gpmodel = gpmodel
         self.active_metric = active_metric
         self.normalize_targets = normalize_targets
         self._debug_log = debug_log
-        self._profiler = profiler
         self._filter_observed_data = filter_observed_data
         self._no_fantasizing = no_fantasizing
         self._hp_ranges_for_prediction = hp_ranges_for_prediction
         self._mean = None
         self._std = None
 
     @property
     def debug_log(self) -> Optional[DebugLogPrinter]:
         return self._debug_log
 
     @property
-    def profiler(self) -> Optional[SimpleProfiler]:
-        return self._profiler
-
-    @property
     def gpmodel(self) -> GPModel:
         return self._gpmodel
 
     def model(self, state: TuningJobState, fit_params: bool) -> SurrogateModel:
         """
         Parameters of ``self._gpmodel`` are optimized iff ``fit_params``. This
         requires ``state`` to contain labeled examples.
@@ -299,26 +292,20 @@
         if state.pending_evaluations:
             no_pending_state = TuningJobState(
                 hp_ranges=state.hp_ranges,
                 config_for_trial=state.config_for_trial,
                 trials_evaluations=state.trials_evaluations,
                 failed_trials=state.failed_trials,
             )
-        self._posterior_for_state(
-            no_pending_state, fit_params=fit_params, profiler=self._profiler
-        )
+        self._posterior_for_state(no_pending_state, fit_params=fit_params)
         if state.pending_evaluations and not self._no_fantasizing:
             # Sample fantasy values for pending evaluations
             state_with_fantasies = self._draw_fantasy_values(state)
             # Compute posterior for state with pending evals
-            # Note: profiler is not passed here, this would overwrite the
-            # results from the first call
-            self._posterior_for_state(
-                state_with_fantasies, fit_params=False, profiler=None
-            )
+            self._posterior_for_state(state_with_fantasies, fit_params=False)
             fantasy_samples = state_with_fantasies.pending_evaluations
         else:
             fantasy_samples = []
         return GaussProcSurrogateModel(
             state=state,
             active_metric=self.active_metric,
             gpmodel=self._gpmodel,
@@ -332,15 +319,14 @@
     def _get_num_fantasy_samples(self) -> int:
         raise NotImplementedError()
 
     def _posterior_for_state(
         self,
         state: TuningJobState,
         fit_params: bool,
-        profiler: Optional[SimpleProfiler] = None,
     ):
         """
         Computes posterior for state.
         If ``fit_params`` and ``state.pending_evaluations`` is empty, we first
         optimize the model parameters.
         If ``state.pending_evaluations`` are given, these must be of type
         :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common.FantasizedPendingEvaluations`,
@@ -367,15 +353,15 @@
         if not fit_params:
             if self._debug_log is not None:
                 logger.info("Recomputing posterior state")
             self._gpmodel.recompute_states(data)
         else:
             if self._debug_log is not None:
                 logger.info(f"Fitting surrogate model for {self.active_metric}")
-            self._gpmodel.fit(data, profiler=profiler)
+            self._gpmodel.fit(data)
         if self._debug_log is not None:
             self._debug_log.set_model_params(self.get_params())
             if not state.pending_evaluations:
                 deb_msg = "[GaussProcModelFactory._posterior_for_state]\n"
                 deb_msg += "- self.mean = {}\n".format(self._mean)
                 deb_msg += "- self.std = {}".format(self._std)
                 logger.info(deb_msg)
@@ -471,26 +457,24 @@
 
     def __init__(
         self,
         gpmodel: GPModel,
         num_fantasy_samples: int,
         active_metric: str = INTERNAL_METRIC_NAME,
         normalize_targets: bool = True,
-        profiler: Optional[SimpleProfiler] = None,
         debug_log: Optional[DebugLogPrinter] = None,
         filter_observed_data: Optional[ConfigurationFilter] = None,
         no_fantasizing: bool = False,
         hp_ranges_for_prediction: Optional[HyperparameterRanges] = None,
     ):
         assert num_fantasy_samples > 0
         super().__init__(
             gpmodel=gpmodel,
             active_metric=active_metric,
             normalize_targets=normalize_targets,
-            profiler=profiler,
             debug_log=debug_log,
             filter_observed_data=filter_observed_data,
             no_fantasizing=no_fantasizing,
             hp_ranges_for_prediction=hp_ranges_for_prediction,
         )
         self.num_fantasy_samples = num_fantasy_samples
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     FantasizedPendingEvaluation,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import ConfigurationFilter
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 logger = logging.getLogger(__name__)
 
 
 class GaussProcAdditiveSurrogateModel(BaseSurrogateModel):
     """
     Gaussian Process additive surrogate model, where model parameters are
@@ -158,15 +157,14 @@
     def __init__(
         self,
         gpmodel: GaussianProcessLearningCurveModel,
         num_fantasy_samples: int,
         active_metric: str,
         config_space_ext: ExtendedConfiguration,
         normalize_targets: bool = False,
-        profiler: Optional[SimpleProfiler] = None,
         debug_log: Optional[DebugLogPrinter] = None,
         filter_observed_data: Optional[ConfigurationFilter] = None,
     ):
         self._gpmodel = gpmodel
         self.active_metric = active_metric
         r_min, r_max = config_space_ext.resource_attr_range
         assert (
@@ -174,26 +172,21 @@
         ), f"r_min = {r_min}, r_max = {r_max}: Need 0 < r_min < r_max"
         assert (
             num_fantasy_samples >= 0
         ), f"num_fantasy_samples = {num_fantasy_samples}, must be non-negative int"
         self.num_fantasy_samples = num_fantasy_samples
         self._config_space_ext = config_space_ext
         self._debug_log = debug_log
-        self._profiler = profiler
         self._filter_observed_data = filter_observed_data
         self.normalize_targets = normalize_targets
 
     @property
     def debug_log(self) -> Optional[DebugLogPrinter]:
         return self._debug_log
 
-    @property
-    def profiler(self) -> Optional[SimpleProfiler]:
-        return self._profiler
-
     def get_params(self):
         return self._gpmodel.get_params()
 
     def set_params(self, param_dict):
         self._gpmodel.set_params(param_dict)
 
     def model(self, state: TuningJobState, fit_params: bool) -> SurrogateModel:
@@ -211,15 +204,15 @@
             self._config_space_ext,
             self.active_metric,
             normalize_targets=self.normalize_targets,
             do_fantasizing=False,
         )
         if fit_params:
             logger.info(f"Fitting surrogate model for {self.active_metric}")
-            self._gpmodel.fit(data, profiler=self._profiler)
+            self._gpmodel.fit(data)
         elif not do_fantasizing:
             # Only if part below is skipped
             logger.info("Recomputing posterior state")
             self._gpmodel.recompute_states(data)
         if self._debug_log is not None:
             self._debug_log.set_model_params(self.get_params())
         if self.normalize_targets:
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,35 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-import numpy as np
 from typing import Dict, Optional, Set, List, Tuple
 import logging
-from scipy.stats import norm
 import itertools
 
+import numpy as np
+from scipy.stats import norm
+from scipy.special import erfc
+
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.meanstd_acqfunc import (
     MeanStdAcquisitionFunction,
     HeadWithGradient,
     SamplePredictionsPerOutput,
     CurrentBestProvider,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
     BaseSurrogateModel,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     SurrogateOutputModel,
     SurrogateModel,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.density import (
-    get_quantiles,
-)
 
 logger = logging.getLogger(__name__)
 
 
 MIN_COST = 1e-12  # For numerical stability when dividing EI / cost
 
 MIN_STD_CONSTRAINT = (
@@ -515,7 +514,29 @@
             # Remove all infeasible candidates (i.e., where means_constraint
             # is >= 0)
             means_active[means_constraint >= 0] = np.nan
             # Compute the current *feasible* best (separately for every fantasy)
             min_across_observations = np.nanmin(means_active, axis=0)
             current_best_list.append(min_across_observations)
         return ConstraintCurrentBestProvider(current_best_list, num_samples_active)
+
+
+def get_quantiles(acquisition_par, fmin, m, s):
+    """
+    Quantiles of the Gaussian distribution, useful to determine the acquisition
+    function values.
+
+    :param acquisition_par: parameter of the acquisition function
+    :param fmin: current minimum.
+    :param m: vector of means.
+    :param s: vector of standard deviations.
+    """
+    if isinstance(s, np.ndarray):
+        s[s < 1e-10] = 1e-10
+    elif s < 1e-10:
+        s = 1e-10
+    u = (fmin - m - acquisition_par) / s
+
+    phi = np.exp(-0.5 * u**2) / np.sqrt(2 * np.pi)
+    # vectorized version of erfc to not depend on scipy
+    Phi = 0.5 * erfc(-u / np.sqrt(2))
+    return phi, Phi, u
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     PendingEvaluation,
     TrialEvaluations,
     dictionarize_objective,
     INTERNAL_METRIC_NAME,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 logger = logging.getLogger(__name__)
 
 
 def _assert_same_keys(dict1, dict2):
     assert set(dict1.keys()) == set(
         dict2.keys()
@@ -86,18 +85,14 @@
         """
         raise NotImplementedError()
 
     @property
     def debug_log(self) -> Optional[DebugLogPrinter]:
         return None
 
-    @property
-    def profiler(self) -> Optional[SimpleProfiler]:
-        return None
-
     def configure_scheduler(self, scheduler):
         """
         Called by :meth:`configure_scheduler` of searchers which make use of a
         class:``TransformerModelFactory``. Allows the factory to depend on
         parameters of the scheduler.
 
         :param scheduler: Scheduler object
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,29 @@
     Tuple,
     Type,
     Optional,
     Set,
     Dict,
     Union,
     Any,
+    Iterator,
 )
 import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     INTERNAL_METRIC_NAME,
 )
+from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
+    TuningJobState,
+)
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
     HyperparameterRanges,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
-    TuningJobState,
-)
 
 
 def assign_active_metric(model, active_metric):
     """Checks that active_metric is provided when model consists of multiple output models.
     Otherwise, just sets active_metric to the only model output name available.
     """
     model_output_names = sorted(model.keys())
@@ -310,7 +312,29 @@
         """Run local optimization, starting from ``candidate``
 
         :param candidate: Starting point
         :param model: Overrides ``self.model``
         :return: Configuration found by local optimization
         """
         raise NotImplementedError
+
+
+class CandidateGenerator:
+    """
+    Class to generate candidates from which to start the local minimization,
+    typically random candidate or some form of more uniformly spaced variation,
+    such as latin hypercube or Sobol sequence.
+    """
+
+    def generate_candidates(self) -> Iterator[Configuration]:
+        raise NotImplementedError
+
+    def generate_candidates_en_bulk(
+        self, num_cands: int, exclusion_list: Optional[ExclusionList] = None
+    ) -> List[Configuration]:
+        """
+        :param num_cands: Number of candidates to generate
+        :param exclusion_list: If given, these candidates must not be returned
+        :return: List of ``num_cands`` candidates. If ``exclusion_list`` is given,
+            the number of candidates returned can be ``< num_cands``
+        """
+        raise NotImplementedError
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,30 +24,25 @@
     ModelStateTransformer,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     NextCandidatesAlgorithm,
     ScoringFunction,
     LocalOptimizer,
     SurrogateModel,
+    CandidateGenerator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm_components import (
     LBFGSOptimizeAcquisition,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
     generate_unique_candidates,
-    ExclusionList,
-    CandidateGenerator,
+    DuplicateDetector,
 )
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.duplicate_detector import (
-    DuplicateDetector,
-)
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class BayesianOptimizationAlgorithm(NextCandidatesAlgorithm):
     """
@@ -89,15 +84,14 @@
         ``num_requested_candidates > 1`` and ``greedy_batch_selection == True``. In
         this case, ``num_initial_candidates_for_batch`` overrides
         ``num_initial_candidates`` when selecting all but the first candidate for
         the batch. Typically, ``num_initial_candidates`` is larger than
         ``num_initial_candidates_for_batch`` in this case, which speeds up
         selecting large batches, but still select the first candidate
         thoroughly
-    :param profiler: If given, this is used for profiling parts in the code
     :param sample_unique_candidates: If ``True``, we check that initial candidates
         sampled at random are unique and disjoint from the exclusion list.
         This can be expensive. Defaults to ``False``
     :param debug_log: If a
         :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log.DebugLogPrinter`
         object is passed here, it is used to write log messages
     """
@@ -108,15 +102,14 @@
     local_optimizer: LocalOptimizer
     pending_candidate_state_transformer: Optional[ModelStateTransformer]
     exclusion_candidates: ExclusionList
     num_requested_candidates: int
     greedy_batch_selection: bool
     duplicate_detector: DuplicateDetector
     num_initial_candidates_for_batch: Optional[int] = None
-    profiler: Optional[SimpleProfiler] = None
     sample_unique_candidates: bool = False
     debug_log: Optional[DebugLogPrinter] = None
 
     # Note: For greedy batch selection (num_outer_iterations > 1), the
     # underlying SurrrogateModel changes with each new pending candidate. The
     # model changes are managed by pending_candidate_state_transformer. The
     # model has to be passed to both initial_candidates_scorer and
@@ -219,18 +212,14 @@
             num_initial_candidates = self.num_initial_candidates
         # generate a random candidates among which to pick the ones to be
         # locally optimized
         logger.info(
             f"BayesOpt Algorithm: Generating {num_initial_candidates} "
             "initial candidates."
         )
-        if self.profiler is not None:
-            self.profiler.push_prefix("nextcand")
-            self.profiler.start("all")
-            self.profiler.start("genrandom")
         if self.sample_unique_candidates:
             # This can be expensive, depending on what type Candidate is
             initial_candidates = generate_unique_candidates(
                 self.initial_candidates_generator,
                 num_initial_candidates,
                 self.exclusion_candidates,
             )
@@ -238,17 +227,14 @@
             # Will not return candidates in ``exclusion_candidates``, but there
             # can be duplicates
             initial_candidates = (
                 self.initial_candidates_generator.generate_candidates_en_bulk(
                     num_initial_candidates, exclusion_list=self.exclusion_candidates
                 )
             )
-        if self.profiler is not None:
-            self.profiler.stop("genrandom")
-            self.profiler.start("scoring")
         logger.info("BayesOpt Algorithm: Scoring (and reordering) candidates.")
         if self.debug_log is not None:
             candidates_and_scores = _order_candidates(
                 initial_candidates,
                 self.initial_candidates_scorer,
                 model=model,
                 with_scores=True,
@@ -257,17 +243,14 @@
             config = initial_candidates[0]
             top_scores = np.array([x for x, _ in candidates_and_scores[:5]])
             self.debug_log.set_init_config(config, top_scores)
         else:
             initial_candidates = _order_candidates(
                 initial_candidates, self.initial_candidates_scorer, model=model
             )
-        if self.profiler is not None:
-            self.profiler.stop("scoring")
-            self.profiler.start("localsearch")
         candidates_with_optimization = _lazily_locally_optimize(
             initial_candidates,
             self.local_optimizer,
             hp_ranges=self.exclusion_candidates.hp_ranges,
             model=model,
         )
         logger.info("BayesOpt Algorithm: Selecting final set of candidates.")
@@ -284,18 +267,14 @@
             )
         candidates = _pick_from_locally_optimized(
             candidates_with_optimization,
             self.exclusion_candidates,
             num_candidates,
             self.duplicate_detector,
         )
-        if self.profiler is not None:
-            self.profiler.stop("localsearch")
-            self.profiler.stop("all")
-            self.profiler.pop_prefix()  # nextcand
         return candidates
 
 
 def _order_candidates(
     candidates: List[Configuration],
     scoring_function: ScoringFunction,
     model: Optional[SurrogateModel],
@@ -320,15 +299,15 @@
 ) -> Iterator[Tuple[Configuration, Configuration]]:
     """
     Due to local deduplication we do not know in advance how many candidates
     we have to locally optimize, hence this helper to create a lazy generator
     of locally optimized candidates.
     Note that ``candidates`` may contain duplicates, but such are skipped here.
     """
-    considered_already = ExclusionList.empty_list(hp_ranges)
+    considered_already = ExclusionList(hp_ranges)
     for cand in candidates:
         if not considered_already.contains(cand):
             considered_already.add(cand)
             yield cand, local_optimizer.optimize(cand, model=model)
 
 
 # Note: If ``duplicate_detector`` is at least :class:`DuplicateDetectorIdentical`,
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,136 +6,120 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Iterable, List, Optional
-import numpy as np
-from scipy.optimize import fmin_l_bfgs_b
+from typing import Dict, Optional, List, Any, Tuple
 import logging
-from numpy.random import RandomState
+import numpy as np
 
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateModel,
-    ScoringFunction,
-    LocalOptimizer,
-    SurrogateOutputModel,
-    AcquisitionClassAndArgs,
-    unwrap_acquisition_class_and_kwargs,
-)
-from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
-from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
-    HyperparameterRanges,
+from syne_tune.optimizer.schedulers.searchers.kde.kde_searcher import (
+    KernelDensityEstimator,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class IndependentThompsonSampling(ScoringFunction):
+class MultiFidelityKernelDensityEstimator(KernelDensityEstimator):
     """
-    Note: This is *not* Thompson sampling, but rather a variant called
-    "independent Thompson sampling", where means and variances are drawn
-    from the marginal rather than the joint distribution. This is cheap,
-    but incorrect. In fact, the larger the number of candidates, the more
-    likely the winning configuration is arising from pure chance.
-
-    :param model: Surrogate model for statistics of predictive distribution
-    :param random_state: PRN generator
-    """
-
-    def __init__(
-        self, model: SurrogateModel, random_state: Optional[RandomState] = None
-    ):
-        self.model = model
-        if random_state is None:
-            random_state = RandomState(31415629)
-        self.random_state = random_state
+    Adapts :class:`KernelDensityEstimator` to the multi-fidelity setting as proposed
+    by Falkner et al such that we can use it with Hyperband. Following Falkner
+    et al, we fit the KDE only on the highest resource level where we have at
+    least num_min_data_points. Code is based on the implementation by Falkner
+    et al: https://github.com/automl/HpBandSter/tree/master/hpbandster
+
+        | BOHB: Robust and Efficient Hyperparameter Optimization at Scale
+        | S. Falkner and A. Klein and F. Hutter
+        | Proceedings of the 35th International Conference on Machine Learning
 
-    def score(
-        self,
-        candidates: Iterable[Configuration],
-        model: Optional[SurrogateModel] = None,
-    ) -> List[float]:
-        if model is None:
-            model = self.model
-        predictions_list = model.predict_candidates(candidates)
-        scores = []
-        # If the model supports fantasizing, posterior_means is a matrix. In
-        # that case, samples are drawn for every column, then averaged (why
-        # we need np.mean)
-        for predictions in predictions_list:
-            posterior_means = predictions["mean"]
-            posterior_stds = predictions["std"]
-            new_score = [
-                np.mean(self.random_state.normal(m, s))
-                for m, s in zip(posterior_means, posterior_stds)
-            ]
-            scores.append(new_score)
-        return list(np.mean(np.array(scores), axis=0))
+    Additional arguments on top of parent class
+    :class:`~syne_tune.optimizer.schedulers.searchers.kde.KernelDensityEstimator`:
 
+    :param resource_attr: Name of resource attribute. Defaults to
+        ``scheduler.resource_attr`` in :meth:`configure_scheduler`
+    """
 
-class LBFGSOptimizeAcquisition(LocalOptimizer):
     def __init__(
         self,
-        hp_ranges: HyperparameterRanges,
-        model: SurrogateOutputModel,
-        acquisition_class: AcquisitionClassAndArgs,
-        active_metric: str = None,
+        config_space: Dict[str, Any],
+        metric: str,
+        points_to_evaluate: Optional[List[dict]] = None,
+        allow_duplicates: Optional[bool] = None,
+        mode: Optional[str] = None,
+        num_min_data_points: Optional[int] = None,
+        top_n_percent: Optional[int] = None,
+        min_bandwidth: Optional[float] = None,
+        num_candidates: Optional[int] = None,
+        bandwidth_factor: Optional[int] = None,
+        random_fraction: Optional[float] = None,
+        resource_attr: Optional[str] = None,
+        **kwargs
     ):
-        super().__init__(hp_ranges, model, acquisition_class, active_metric)
-        # Number criterion evaluations in last recent optimize call
-        self.num_evaluations = None
-
-    def optimize(
-        self, candidate: Configuration, model: Optional[SurrogateOutputModel] = None
-    ) -> Configuration:
-        # Before local minimization, the model for this state_id should have been fitted.
-        if model is None:
-            model = self.model
-        acquisition_class, acquisition_kwargs = unwrap_acquisition_class_and_kwargs(
-            self.acquisition_class
+        if min_bandwidth is None:
+            min_bandwidth = 0.1
+        super().__init__(
+            config_space,
+            metric=metric,
+            points_to_evaluate=points_to_evaluate,
+            allow_duplicates=allow_duplicates,
+            mode=mode,
+            num_min_data_points=num_min_data_points,
+            top_n_percent=top_n_percent,
+            min_bandwidth=min_bandwidth,
+            num_candidates=num_candidates,
+            bandwidth_factor=bandwidth_factor,
+            random_fraction=random_fraction,
+            **kwargs
         )
-        acquisition_function = acquisition_class(
-            model, self.active_metric, **acquisition_kwargs
+        self.resource_attr = resource_attr
+        self.resource_levels = []
+
+    def configure_scheduler(self, scheduler):
+        from syne_tune.optimizer.schedulers.multi_fidelity import (
+            MultiFidelitySchedulerMixin,
         )
 
-        x0 = self.hp_ranges.to_ndarray(candidate)
-        bounds = self.hp_ranges.get_ndarray_bounds()
-        n_evaluations = [0]  # wrapped in list to allow access from function
-
-        # unwrap 2d arrays
-        def f_df(x):
-            n_evaluations[0] += 1
-            return acquisition_function.compute_acq_with_gradient(x)
-
-        res = fmin_l_bfgs_b(f_df, x0=x0, bounds=bounds, maxiter=1000)
-        self.num_evaluations = n_evaluations[0]
-        if res[2]["task"] == b"ABNORMAL_TERMINATION_IN_LNSRCH":
-            # this condition was copied from the old GPyOpt code
-            logger.warning(
-                f"ABNORMAL_TERMINATION_IN_LNSRCH in lbfgs after {n_evaluations[0]} evaluations, "
-                "returning original candidate"
-            )
-            return candidate  # returning original candidate
+        super().configure_scheduler(scheduler)
+        assert isinstance(
+            scheduler, MultiFidelitySchedulerMixin
+        ), "This searcher requires MultiFidelitySchedulerMixin scheduler"
+        self.resource_attr = scheduler.resource_attr
+
+    def _highest_resource_model_can_fit(self, num_features: int) -> Optional[int]:
+        unique_resource_levels, counts = np.unique(
+            self.resource_levels, return_counts=True
+        )
+        for resource, count in reversed(list(zip(unique_resource_levels, counts))):
+            if self._check_data_shape_and_good_size((count, num_features)) is not None:
+                return resource
+        return None
+
+    def _train_kde(
+        self, train_data: np.ndarray, train_targets: np.ndarray
+    ) -> Optional[Tuple[Any, Any]]:
+        """
+        Find the highest resource level so that the data only at that level is
+        large enough to train KDE models both on the good part and the rest.
+        If no such resource level exists, we return ``None``.
+
+        :param train_data: Training input features
+        :param train_targets: Training targets
+        :return: Tuple of good model, bad model; or ``None``
+        """
+        train_data = train_data.reshape((train_targets.size, -1))
+        num_features = train_data.shape[1]
+        resource = self._highest_resource_model_can_fit(num_features)
+        if resource is None:
+            return None
         else:
-            # Clip to avoid situation where result is small epsilon out of bounds
-            a_min, a_max = zip(*bounds)
-            optimized_x = np.clip(res[0], a_min, a_max)
-            # Make sure the above clipping does really just fix numerical
-            # rounding issues in L-BFGS if any bigger change was made there is
-            # a bug and we want to throw an exception
-            assert np.linalg.norm(res[0] - optimized_x) < 1e-6, (
-                res[0],
-                optimized_x,
-                bounds,
-            )
-            result = self.hp_ranges.from_ndarray(optimized_x.flatten())
-            return result
-
-
-class NoOptimization(LocalOptimizer):
-    def optimize(
-        self, candidate: Configuration, model: Optional[SurrogateModel] = None
-    ) -> Configuration:
-        return candidate
+            # Models can be fit
+            indices = np.where(self.resource_levels == resource)
+            sub_data = train_data[indices]
+            sub_targets = train_targets[indices]
+            return super()._train_kde(sub_data, sub_targets)
+
+    def _update(self, trial_id: str, config: Dict, result: Dict):
+        super()._update(trial_id=trial_id, config=config, result=result)
+        resource_level = int(result[self.resource_attr])
+        self.resource_levels.append(resource_level)
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/common.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,148 +6,149 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Iterator, List, Union, Optional, Dict, Any
+from typing import Iterable, List, Optional, Iterator
 import numpy as np
+from scipy.optimize import fmin_l_bfgs_b
 import logging
+from numpy.random import RandomState
 
-from syne_tune.optimizer.schedulers.searchers.utils.common import (
-    Configuration,
-    ConfigurationFilter,
+from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
+    SurrogateModel,
+    ScoringFunction,
+    LocalOptimizer,
+    SurrogateOutputModel,
+    AcquisitionClassAndArgs,
+    unwrap_acquisition_class_and_kwargs,
+    CandidateGenerator,
 )
+from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
     HyperparameterRanges,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
-    TuningJobState,
-)
-from syne_tune.config_space import config_space_size
 
 logger = logging.getLogger(__name__)
 
 
-MAX_RETRIES_CANDIDATES_EN_BULK = 20
-
-
-class ExclusionList:
+class IndependentThompsonSampling(ScoringFunction):
     """
-    Maintains exclusion list of configs, to avoid choosing configs several
-    times. In fact, ``self.excl_set`` maintains a set of match strings.
+    Note: This is *not* Thompson sampling, but rather a variant called
+    "independent Thompson sampling", where means and variances are drawn
+    from the marginal rather than the joint distribution. This is cheap,
+    but incorrect. In fact, the larger the number of candidates, the more
+    likely the winning configuration is arising from pure chance.
 
-    The exclusion list contains non-extended configs, but it can be fed with
-    and queried with extended configs. In that case, the resource attribute
-    is removed from the config.
-
-    :param state: Either tuning job state, or a ``dict`` containing the members
-        to be used (copy constructor)
-    :param filter_observed_data: Filter on observed data, optional
+    :param model: Surrogate model for statistics of predictive distribution
+    :param random_state: PRN generator
     """
 
     def __init__(
+        self, model: SurrogateModel, random_state: Optional[RandomState] = None
+    ):
+        self.model = model
+        if random_state is None:
+            random_state = RandomState(31415629)
+        self.random_state = random_state
+
+    def score(
+        self,
+        candidates: Iterable[Configuration],
+        model: Optional[SurrogateModel] = None,
+    ) -> List[float]:
+        if model is None:
+            model = self.model
+        predictions_list = model.predict_candidates(candidates)
+        scores = []
+        # If the model supports fantasizing, posterior_means is a matrix. In
+        # that case, samples are drawn for every column, then averaged (why
+        # we need np.mean)
+        for predictions in predictions_list:
+            posterior_means = predictions["mean"]
+            posterior_stds = predictions["std"]
+            new_score = [
+                np.mean(self.random_state.normal(m, s))
+                for m, s in zip(posterior_means, posterior_stds)
+            ]
+            scores.append(new_score)
+        return list(np.mean(np.array(scores), axis=0))
+
+
+class LBFGSOptimizeAcquisition(LocalOptimizer):
+    def __init__(
         self,
-        state: Union[TuningJobState, dict],
-        filter_observed_data: Optional[ConfigurationFilter] = None,
+        hp_ranges: HyperparameterRanges,
+        model: SurrogateOutputModel,
+        acquisition_class: AcquisitionClassAndArgs,
+        active_metric: str = None,
     ):
-        is_new = isinstance(state, TuningJobState)
-        if is_new:
-            self.hp_ranges = state.hp_ranges
-            keys = self.hp_ranges.internal_keys
-            # Remove resource attribute from ``self.keys`` if present
-            resource_attr = self.hp_ranges.name_last_pos
-            if resource_attr is None:
-                self.keys = keys
-            else:
-                pos = keys.index(resource_attr)
-                self.keys = keys[:pos] + keys[(pos + 1) :]
-            _elist = [
-                x.trial_id for x in state.pending_evaluations
-            ] + state.failed_trials
-            observed_trial_ids = [x.trial_id for x in state.trials_evaluations]
-            if filter_observed_data is not None:
-                observed_trial_ids = [
-                    trial_id
-                    for trial_id in observed_trial_ids
-                    if filter_observed_data(state.config_for_trial[trial_id])
-                ]
-            _elist = set(_elist + observed_trial_ids)
-            self.excl_set = set(
-                self._to_matchstr(state.config_for_trial[trial_id])
-                for trial_id in _elist
+        super().__init__(hp_ranges, model, acquisition_class, active_metric)
+        # Number criterion evaluations in last recent optimize call
+        self.num_evaluations = None
+
+    def optimize(
+        self, candidate: Configuration, model: Optional[SurrogateOutputModel] = None
+    ) -> Configuration:
+        # Before local minimization, the model for this state_id should have been fitted.
+        if model is None:
+            model = self.model
+        acquisition_class, acquisition_kwargs = unwrap_acquisition_class_and_kwargs(
+            self.acquisition_class
+        )
+        acquisition_function = acquisition_class(
+            model, self.active_metric, **acquisition_kwargs
+        )
+
+        x0 = self.hp_ranges.to_ndarray(candidate)
+        bounds = self.hp_ranges.get_ndarray_bounds()
+        n_evaluations = [0]  # wrapped in list to allow access from function
+
+        # unwrap 2d arrays
+        def f_df(x):
+            n_evaluations[0] += 1
+            return acquisition_function.compute_acq_with_gradient(x)
+
+        res = fmin_l_bfgs_b(f_df, x0=x0, bounds=bounds, maxiter=1000)
+        self.num_evaluations = n_evaluations[0]
+        if res[2]["task"] == b"ABNORMAL_TERMINATION_IN_LNSRCH":
+            # this condition was copied from the old GPyOpt code
+            logger.warning(
+                f"ABNORMAL_TERMINATION_IN_LNSRCH in lbfgs after {n_evaluations[0]} evaluations, "
+                "returning original candidate"
             )
+            return candidate  # returning original candidate
         else:
-            self.hp_ranges = state["hp_ranges"]
-            self.excl_set = state["excl_set"]
-            self.keys = state["keys"]
-        self.configspace_size = config_space_size(self.hp_ranges.config_space)
-
-    def _to_matchstr(self, config) -> str:
-        return self.hp_ranges.config_to_match_string(config, keys=self.keys)
-
-    def contains(self, config: Configuration) -> bool:
-        return self._to_matchstr(config) in self.excl_set
-
-    def add(self, config: Configuration):
-        self.excl_set.add(self._to_matchstr(config))
-
-    def copy(self) -> "ExclusionList":
-        return ExclusionList(
-            {
-                "hp_ranges": self.hp_ranges,
-                "excl_set": set(self.excl_set),
-                "keys": self.keys,
-            }
-        )
+            # Clip to avoid situation where result is small epsilon out of bounds
+            a_min, a_max = zip(*bounds)
+            optimized_x = np.clip(res[0], a_min, a_max)
+            # Make sure the above clipping does really just fix numerical
+            # rounding issues in L-BFGS if any bigger change was made there is
+            # a bug and we want to throw an exception
+            assert np.linalg.norm(res[0] - optimized_x) < 1e-6, (
+                res[0],
+                optimized_x,
+                bounds,
+            )
+            result = self.hp_ranges.from_ndarray(optimized_x.flatten())
+            return result
 
-    @staticmethod
-    def empty_list(hp_ranges: HyperparameterRanges) -> "ExclusionList":
-        return ExclusionList(TuningJobState.empty_state(hp_ranges))
-
-    def __len__(self) -> int:
-        return len(self.excl_set)
-
-    def config_space_exhausted(self) -> bool:
-        return (self.configspace_size is not None) and len(
-            self.excl_set
-        ) >= self.configspace_size
-
-    def get_state(self) -> Dict[str, Any]:
-        return {
-            "excl_set": list(self.excl_set),
-            "keys": self.keys,
-        }
-
-    def clone_from_state(self, state: Dict[str, Any]):
-        self.keys = state["keys"]
-        self.excl_set = set(state["excl_set"])
 
+class NoOptimization(LocalOptimizer):
+    def optimize(
+        self, candidate: Configuration, model: Optional[SurrogateModel] = None
+    ) -> Configuration:
+        return candidate
 
-class CandidateGenerator:
-    """
-    Class to generate candidates from which to start the local minimization,
-    typically random candidate or some form of more uniformly spaced variation,
-    such as latin hypercube or Sobol sequence.
-    """
 
-    def generate_candidates(self) -> Iterator[Configuration]:
-        raise NotImplementedError
-
-    def generate_candidates_en_bulk(
-        self, num_cands: int, exclusion_list: Optional[ExclusionList] = None
-    ) -> List[Configuration]:
-        """
-        :param num_cands: Number of candidates to generate
-        :param exclusion_list: If given, these candidates must not be returned
-        :return: List of ``num_cands`` candidates. If ``exclusion_list`` is given,
-            the number of candidates returned can be ``< num_cands``
-        """
-        raise NotImplementedError
+MAX_RETRIES_CANDIDATES_EN_BULK = 20
+MAX_RETRIES_ON_DUPLICATES = 10000
 
 
 class RandomStatefulCandidateGenerator(CandidateGenerator):
     """
     This generator maintains a random state, so if :meth:`generate_candidates`
     is called several times, different sequences are returned.
 
@@ -198,17 +199,14 @@
                     f"Could only sample {num_done} candidates where "
                     f"{num_cands} were requested. len(exclusion_list) = "
                     f"{len(exclusion_list)}"
                 )
             return configs
 
 
-MAX_RETRIES_ON_DUPLICATES = 10000
-
-
 def generate_unique_candidates(
     candidates_generator: CandidateGenerator,
     num_candidates: int,
     exclusion_candidates: ExclusionList,
 ) -> List[Configuration]:
     exclusion_candidates = exclusion_candidates.copy()  # Copy
     result = []
@@ -319,7 +317,28 @@
                     config = self.base_set[pos]
                     if not exclusion_list.contains(config):
                         configs.append(config)
                         new_pos.append(pos)
                         len_configs += 1
                 self.pos_returned.update(new_pos)
         return self._extend_configs(configs)
+
+
+class DuplicateDetector:
+    def contains(
+        self, existing_candidates: ExclusionList, new_candidate: Configuration
+    ) -> bool:
+        raise NotImplementedError
+
+
+class DuplicateDetectorNoDetection(DuplicateDetector):
+    def contains(
+        self, existing_candidates: ExclusionList, new_candidate: Configuration
+    ) -> bool:
+        return False  # no duplicate detection at all
+
+
+class DuplicateDetectorIdentical(DuplicateDetector):
+    def contains(
+        self, existing_candidates: ExclusionList, new_candidate: Configuration
+    ) -> bool:
+        return existing_candidates.contains(new_candidate)
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,18 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.kernel import (
     Matern52,
     KernelFunction,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.warping import (
     kernel_with_warping,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
-    ExclusionList,
+from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     CandidateGenerator,
 )
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 
 
 def build_kernel(state: TuningJobState, do_warping: bool = False) -> KernelFunction:
     hp_ranges = state.hp_ranges
     dims = hp_ranges.ndarray_size
     kernel = Matern52(dims, ARD=True)
     if do_warping:
@@ -160,24 +160,15 @@
 ) -> ExclusionList:
     """
     Creates exclusion list from set of tuples.
 
     """
     if not is_dict:
         candidates_tpl = tuples_to_configs(candidates_tpl, hp_ranges)
-    config_for_trial = {
-        str(trial_id): config for trial_id, config in enumerate(candidates_tpl)
-    }
-    state = TuningJobState(
-        hp_ranges=hp_ranges,
-        config_for_trial=config_for_trial,
-        trials_evaluations=[],
-        failed_trials=[str(x) for x in range(len(candidates_tpl))],
-    )
-    return ExclusionList(state)
+    return ExclusionList(hp_ranges=hp_ranges, configurations=candidates_tpl)
 
 
 TupleOrDict = Union[tuple, dict]
 
 
 def create_tuning_job_state(
     hp_ranges: HyperparameterRanges,
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/de.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/de.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import logging
 import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers import (
     BaseSearcher,
     GPMultiFidelitySearcher,
 )
-from syne_tune.optimizer.schedulers.searchers.gp_fifo_searcher import (
+from syne_tune.optimizer.schedulers.searchers.model_based_searcher import (
     create_initial_candidates_scorer,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
-    ExclusionList,
-)
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils.common import (
     Configuration,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
+from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     CandidateGenerator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
     BaseSurrogateModel,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
     TuningJobState,
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,347 +6,530 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-import numpy as np
-from typing import Optional, List, Dict, Any
+import time
+from typing import Optional, Type, Dict, Any, List
 import logging
+import numpy as np
 import copy
 
-from syne_tune.optimizer.schedulers.searchers import ModelBasedSearcher
-from syne_tune.optimizer.schedulers.searchers.gp_searcher_factory import (
-    gp_fifo_searcher_factory,
-    gp_fifo_searcher_defaults,
-)
-from syne_tune.optimizer.schedulers.searchers.gp_searcher_utils import (
-    decode_state,
-)
-from syne_tune.optimizer.schedulers.searchers.utils.default_arguments import (
-    check_and_merge_defaults,
+from syne_tune.optimizer.schedulers.searchers import (
+    StochasticSearcher,
+    RandomSearcher,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     INTERNAL_METRIC_NAME,
+    MetricValues,
+    INTERNAL_COST_NAME,
+    TrialEvaluations,
+    dictionarize_objective,
 )
-from syne_tune.optimizer.schedulers.searchers.utils.common import (
-    Configuration,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
-    ModelStateTransformer,
+from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
+    TuningJobState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_skipopt import (
+    SkipOptimizationPredicate,
     AlwaysSkipPredicate,
 )
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
+    TransformerOutputModelFactory,
+    ModelStateTransformer,
+    StateForModelConverter,
+)
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
+    AcquisitionClassAndArgs,
+    LocalOptimizer,
     ScoringFunction,
     SurrogateOutputModel,
-    AcquisitionClassAndArgs,
     unwrap_acquisition_class_and_kwargs,
+    CandidateGenerator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm import (
     BayesianOptimizationAlgorithm,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm_components import (
-    IndependentThompsonSampling,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
+    NoOptimization,
     RandomStatefulCandidateGenerator,
     RandomFromSetCandidateGenerator,
-    CandidateGenerator,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.duplicate_detector import (
     DuplicateDetectorIdentical,
 )
+from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm_components import (
+    IndependentThompsonSampling,
+)
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import (
+    ExclusionList,
+    ExclusionListFromState,
+)
+from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults import (
+    DEFAULT_NUM_INITIAL_CANDIDATES,
+    DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
+    DEFAULT_LOCAL_OPTIMIZER_CLASS,
+)
+from syne_tune.optimizer.schedulers.searchers.gp_searcher_utils import (
+    DEFAULT_INITIAL_SCORING,
+    SUPPORTED_INITIAL_SCORING,
+    MapReward,
+    encode_state,
+)
+from syne_tune.optimizer.schedulers.searchers.utils import HyperparameterRanges
+from syne_tune.optimizer.schedulers.searchers.utils.common import (
+    ConfigurationFilter,
+    Configuration,
+)
 
 logger = logging.getLogger(__name__)
 
 
+GET_CONFIG_RANDOM_RETRIES = 50
+
+
+def check_initial_candidates_scorer(initial_scoring: Optional[str]) -> str:
+    if initial_scoring is None:
+        return DEFAULT_INITIAL_SCORING
+    else:
+        assert (
+            initial_scoring in SUPPORTED_INITIAL_SCORING
+        ), "initial_scoring = '{}' is not supported".format(initial_scoring)
+        return initial_scoring
+
+
+class ModelBasedSearcher(StochasticSearcher):
+    """Common code for surrogate model based searchers
+
+    If ``num_initial_random_choices > 0``, initial configurations are drawn using
+    an internal :class:`~syne_tune.optimizer.schedulers.searchers.RandomSearcher`
+    object, which is created in :meth:`_assign_random_searcher`. This internal
+    random searcher shares :attr:`random_state` with the searcher here. This ensures
+    that if ``ModelBasedSearcher`` and ``RandomSearcher`` objects are created with
+    the same ``random_seed`` and ``points_to_evaluate`` argument, initial
+    configurations are identical until :meth:`_get_config_modelbased` kicks in.
+
+    Note that this works because :attr:`random_state` is only used in the internal
+    random searcher until meth:`_get_config_modelbased` is first called.
+    """
+
+    def _create_internal(
+        self,
+        hp_ranges: HyperparameterRanges,
+        model_factory: TransformerOutputModelFactory,
+        acquisition_class: AcquisitionClassAndArgs,
+        map_reward: Optional[MapReward] = None,
+        init_state: TuningJobState = None,
+        local_minimizer_class: Type[LocalOptimizer] = None,
+        skip_optimization: SkipOptimizationPredicate = None,
+        num_initial_candidates: int = DEFAULT_NUM_INITIAL_CANDIDATES,
+        num_initial_random_choices: int = DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
+        initial_scoring: Optional[str] = None,
+        skip_local_optimization: bool = False,
+        cost_attr: Optional[str] = None,
+        resource_attr: Optional[str] = None,
+        filter_observed_data: Optional[ConfigurationFilter] = None,
+        state_converter: Optional[StateForModelConverter] = None,
+        allow_duplicates: bool = False,
+        restrict_configurations: List[Dict[str, Any]] = None,
+    ):
+        self.hp_ranges = hp_ranges
+        self.num_initial_candidates = num_initial_candidates
+        self.num_initial_random_choices = num_initial_random_choices
+        self.map_reward = map_reward
+        if restrict_configurations is not None:
+            restrict_configurations = self._filter_points_to_evaluate(
+                restrict_configurations, hp_ranges, allow_duplicates
+            )
+            if not skip_local_optimization:
+                logger.warning(
+                    "If restrict_configurations is given, need to have skip_local_optimization == True"
+                )
+                skip_local_optimization = True
+        self._restrict_configurations = restrict_configurations
+        if skip_local_optimization:
+            self.local_minimizer_class = NoOptimization
+        else:
+            self.local_minimizer_class = (
+                DEFAULT_LOCAL_OPTIMIZER_CLASS
+                if local_minimizer_class is None
+                else local_minimizer_class
+            )
+        self.acquisition_class = acquisition_class
+        if isinstance(model_factory, dict):
+            model_factory_main = model_factory[INTERNAL_METRIC_NAME]
+        else:
+            model_factory_main = model_factory
+        self._debug_log = model_factory_main.debug_log
+        self.initial_scoring = check_initial_candidates_scorer(initial_scoring)
+        self.skip_local_optimization = skip_local_optimization
+        # Create state transformer
+        # Initial state is empty (note that the state is mutable).
+        # If there is a state converter, it uses the same random state as the searcher
+        # here
+        if state_converter is not None:
+            state_converter.set_random_state(self.random_state)
+        if init_state is None:
+            init_state = TuningJobState.empty_state(self._hp_ranges_in_state())
+        self.state_transformer = ModelStateTransformer(
+            model_factory=model_factory,
+            init_state=init_state,
+            skip_optimization=skip_optimization,
+            state_converter=state_converter,
+        )
+        self._cost_attr = cost_attr
+        self._resource_attr = resource_attr
+        self._filter_observed_data = filter_observed_data
+        self._allow_duplicates = allow_duplicates
+        self._random_searcher = None
+        # Tracks the cumulative time spent in ``get_config`` calls
+        self.cumulative_get_config_time = 0
+        if self._debug_log is not None:
+            msg_parts = [
+                "[ModelBasedSearcher._create_internal]",
+                f"- acquisition_class = {acquisition_class}",
+                f"- local_minimizer_class = {self.local_minimizer_class}",
+                f"- num_initial_candidates = {num_initial_candidates}",
+                f"- num_initial_random_choices = {num_initial_random_choices}",
+                f"- initial_scoring = {initial_scoring}",
+                f"- allow_duplicates = {self._allow_duplicates}",
+            ]
+            logger.info("\n".join(msg_parts))
+
+    def _copy_kwargs_to_kwargs_int(
+        self, kwargs_int: Dict[str, Any], kwargs: Dict[str, Any]
+    ):
+        """Copies extra arguments not dealt with by ``gp_fifo_searcher_factory``
+
+        :param kwargs_int: Output of factory, to be passed to ``searcher_factory``
+        :param kwargs: Input arguments
+        """
+        # Extra arguments not parsed in factory
+        for k in (
+            "init_state",
+            "local_minimizer_class",
+            "cost_attr",
+            "resource_attr",
+            "restrict_configurations",
+        ):
+            kwargs_int[k] = kwargs.get(k)
+
+    def _hp_ranges_in_state(self):
+        """
+        :return: ``HyperparameterRanges`` to be used in ``self.state_transformer.state``
+        """
+        return self.hp_ranges
+
+    def _hp_ranges_for_prediction(self):
+        """
+        :return: ``HyperparameterRanges`` to be used in predictions and acquisition
+            functions
+        """
+        return self._hp_ranges_in_state()
+
+    def _metric_val_update(
+        self, crit_val: float, result: Dict[str, Any]
+    ) -> MetricValues:
+        return crit_val
+
+    def on_trial_result(
+        self,
+        trial_id: str,
+        config: Dict[str, Any],
+        result: Dict[str, Any],
+        update: bool,
+    ):
+        # If both ``cost_attr`` and ``resource_attr`` are given, cost data (if
+        # given) is written out from every ``result``, independent of ``update``
+        cattr = self._cost_attr
+        rattr = self._resource_attr
+        if (
+            cattr is not None
+            and rattr is not None
+            and cattr in result
+            and rattr in result
+        ):
+            cost_val = float(result[cattr])
+            resource = str(result[rattr])
+            metrics = {INTERNAL_COST_NAME: {resource: cost_val}}
+            self.state_transformer.label_trial(
+                TrialEvaluations(trial_id=trial_id, metrics=metrics), config=config
+            )
+        if update:
+            self._update(trial_id, config, result)
+
+    def _trial_id_string(self, trial_id: str, result: Dict[str, Any]):
+        """
+        For multi-fidelity, we also want to output the resource level
+        """
+        return trial_id
+
+    def _update(self, trial_id: str, config: Dict[str, Any], result: Dict[str, Any]):
+        metric_val = result[self._metric]
+        # Transform to criterion to be minimized
+        if self.map_reward is not None:
+            crit_val = self.map_reward(metric_val)
+        else:
+            crit_val = metric_val
+        metrics = dictionarize_objective(self._metric_val_update(crit_val, result))
+        # Cost value only dealt with here if ``resource_attr`` not given
+        attr = self._cost_attr
+        cost_val = None
+        if attr is not None and attr in result:
+            cost_val = float(result[attr])
+            if self._resource_attr is None:
+                metrics[INTERNAL_COST_NAME] = cost_val
+        self.state_transformer.label_trial(
+            TrialEvaluations(trial_id=trial_id, metrics=metrics), config=config
+        )
+        if self.debug_log is not None:
+            _trial_id = self._trial_id_string(trial_id, result)
+            msg = f"Update for trial_id {_trial_id}: metric = {metric_val:.3f}"
+            if self.map_reward is not None:
+                msg += f", crit_val = {crit_val:.3f}"
+            if cost_val is not None:
+                msg += f", cost_val = {cost_val:.2f}"
+            logger.info(msg)
+
+    def _get_config_modelbased(
+        self, exclusion_candidates: ExclusionList, **kwargs
+    ) -> Optional[Configuration]:
+        """
+        Implements ``get_config`` part if the surrogate model is used, instead
+        of initial choices from ``points_to_evaluate`` or initial random
+        choices.
+
+        :param exclusion_candidates: Configs to be avoided
+        :param kwargs: Extra arguments
+        :return: Suggested configuration, or None if configuration space is
+            exhausted
+        """
+        raise NotImplementedError
+
+    def _get_exclusion_candidates(self, skip_observed: bool = False) -> ExclusionList:
+        def skip_all(config: Configuration) -> bool:
+            return False
+
+        return ExclusionListFromState(
+            self.state_transformer.state,
+            filter_observed_data=skip_all
+            if skip_observed
+            else self._filter_observed_data,
+        )
+
+    def _should_pick_random_config(self, exclusion_candidates: ExclusionList) -> bool:
+        """
+        :param exclusion_candidates: Configs to be avoided
+        :return: Should config be drawn at random in ``get_config``
+        """
+        if len(exclusion_candidates) < self.num_initial_random_choices:
+            return True
+        # Determine whether there is any observed data after filtering
+        state = self.state_transformer.state
+        if not state.trials_evaluations:
+            return True
+        if self._filter_observed_data is None:
+            return False
+        for ev in state.trials_evaluations:
+            config = state.config_for_trial[ev.trial_id]
+            if self._filter_observed_data(config):
+                return False
+        return True
+
+    def _get_config_not_modelbased(
+        self, exclusion_candidates: ExclusionList
+    ) -> (Optional[Configuration], bool):
+        """
+        Does job of ``get_config``, as long as the decision does not involve
+        model-based search. If False is returned, model-based search must be
+        called.
+
+        :param exclusion_candidates: Configs to be avoided
+        :return: ``(config, use_get_config_modelbased)``
+        """
+        self._assign_random_searcher()
+        config = self._next_initial_config()  # Ask for initial config
+        if config is None:
+            pick_random = self._should_pick_random_config(exclusion_candidates)
+        else:
+            pick_random = True  # Initial configs count as random here
+        if pick_random and config is None:
+            for _ in range(GET_CONFIG_RANDOM_RETRIES):
+                _config = self._random_searcher.get_config()
+                if _config is None:
+                    # If ``RandomSearcher`` returns no config at all, the
+                    # search space is exhausted
+                    break
+                if not exclusion_candidates.contains(_config):
+                    config = _config
+                    break
+            # ``_random_searcher`` modified ``restrict_configurations``
+            if self._restrict_configurations is not None:
+                self._restrict_configurations = (
+                    self._random_searcher._restrict_configurations.copy()
+                )
+        return config, pick_random
+
+    def get_config(self, **kwargs) -> Optional[Dict[str, Any]]:
+        """
+        Runs Bayesian optimization in order to suggest the next config to evaluate.
+
+        :return: Next config to evaluate at
+        """
+        start_time = time.time()
+        state = self.state_transformer.state
+        # Initial configs come from ``points_to_evaluate`` or are drawn at random
+        # We use ``exclusion_candidates`` even if ``allow_duplicates == True``, in order
+        # to count how many unique configs have been suggested
+        exclusion_candidates = self._get_exclusion_candidates()
+        config, pick_random = self._get_config_not_modelbased(exclusion_candidates)
+        if self.debug_log is not None:
+            trial_id = kwargs.get("trial_id")
+            self.debug_log.start_get_config(
+                "random" if pick_random else "BO", trial_id=trial_id
+            )
+        if not pick_random:
+            # Model-based decision
+            if self._allow_duplicates or (
+                not exclusion_candidates.config_space_exhausted()
+            ):
+                # Even if ``allow_duplicates == True``, we exclude configs which are
+                # pending or failed
+                if self._allow_duplicates:
+                    excl_cands = self._get_exclusion_candidates(skip_observed=True)
+                else:
+                    excl_cands = exclusion_candidates
+                config = self._get_config_modelbased(
+                    exclusion_candidates=excl_cands, **kwargs
+                )
+
+        if config is not None:
+            if self.debug_log is not None:
+                self.debug_log.set_final_config(config)
+                # All get_config debug log info is only written here
+                self.debug_log.write_block()
+        else:
+            msg = (
+                "Failed to sample a configuration not already chosen "
+                + f"before. Exclusion list has size {len(exclusion_candidates)}."
+            )
+            cs_size = exclusion_candidates.configspace_size
+            if cs_size is not None:
+                msg += f" Configuration space has size {cs_size}."
+            logger.warning(msg)
+        self.cumulative_get_config_time += time.time() - start_time
+
+        return config
+
+    def dataset_size(self):
+        return self.state_transformer.state.num_observed_cases()
+
+    def model_parameters(self):
+        return self.state_transformer.get_params()
+
+    def set_params(self, param_dict):
+        self.state_transformer.set_params(param_dict)
+
+    def get_state(self) -> Dict[str, Any]:
+        """
+        The mutable state consists of the GP model parameters, the
+        ``TuningJobState``, and the ``skip_optimization`` predicate (which can have a
+        mutable state).
+        We assume that ``skip_optimization`` can be pickled.
+
+        Note that we do not have to store the state of :attr:`_random_searcher`,
+        since this internal searcher shares its ``random_state`` with the searcher
+        here.
+        """
+        state = dict(
+            super().get_state(),
+            model_params=self.model_parameters(),
+            state=encode_state(self.state_transformer.state),
+            skip_optimization=self.state_transformer.skip_optimization,
+        )
+        if self._restrict_configurations is not None:
+            state["restrict_configurations"] = self._restrict_configurations
+        return state
+
+    def _restore_from_state(self, state: Dict[str, Any]):
+        super()._restore_from_state(state)
+        self.state_transformer.set_params(state["model_params"])
+        self._restrict_configurations = state.get("restrict_configurations")
+        # The internal random searcher is generated once needed, and it shares its
+        # ``random_state`` with this searcher here
+        self._random_searcher = None
+
+    @property
+    def debug_log(self):
+        return self._debug_log
+
+    def _assign_random_searcher(self):
+        """
+        Assigns :attr:`_random_searcher` if not already done. This internal searcher
+        is sharing :attr:`random_state` with the searcher here, see header comments.
+        """
+        if self._random_searcher is None:
+            # Used for initial random configs (if any)
+            # We do not have to deal with ``points_to_evaluate``
+            self._random_searcher = RandomSearcher(
+                self.hp_ranges.config_space_for_sampling,
+                metric=self._metric,
+                points_to_evaluate=[],
+                random_seed=0,
+                debug_log=False,
+                allow_duplicates=self._allow_duplicates,
+                restrict_configurations=self._restrict_configurations,
+            )
+            self._random_searcher.set_random_state(self.random_state)
+
+
 def create_initial_candidates_scorer(
     initial_scoring: str,
     model: SurrogateOutputModel,
     acquisition_class: AcquisitionClassAndArgs,
     random_state: np.random.RandomState,
-    active_output: str = INTERNAL_METRIC_NAME,
+    active_metric: str = INTERNAL_METRIC_NAME,
 ) -> ScoringFunction:
     if initial_scoring == "thompson_indep":
         if isinstance(model, dict):
-            assert active_output in model
-            model = model[active_output]
+            assert active_metric in model
+            model = model[active_metric]
         return IndependentThompsonSampling(model, random_state=random_state)
     else:
         acquisition_class, acquisition_kwargs = unwrap_acquisition_class_and_kwargs(
             acquisition_class
         )
         return acquisition_class(
-            model, active_metric=active_output, **acquisition_kwargs
+            model, active_metric=active_metric, **acquisition_kwargs
         )
 
 
-class GPFIFOSearcher(ModelBasedSearcher):
-    """Gaussian process Bayesian optimization for FIFO scheduler
+class BayesianOptimizationSearcher(ModelBasedSearcher):
+    """Common Code for searchers using Bayesian optimization
 
-    This searcher must be used with
-    :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`. It provides
-    Bayesian optimization, based on a Gaussian process surrogate model.
-
-    It is *not* recommended creating :class:`GPFIFOSearcher` searcher objects
-    directly, but rather to create
-    :class:`~syne_tune.optimizer.schedulers.FIFOScheduler` objects with
-    ``searcher="bayesopt"``, and passing arguments here in ``search_options``.
-    This will use the appropriate functions from
-    :mod:``syne_tune.optimizer.schedulers.searchers.gp_searcher_factory`` to
-    create components in a consistent way.
-
-    Note: If metric values are to be maximized (``mode-"max"`` in scheduler),
-    the searcher uses ``map_reward`` to map metric values to internal
-    criterion values, and *minimizes* the latter. The default choice is
-    to multiply values by -1.
-
-    Pending configurations (for which evaluation tasks are currently running)
-    are dealt with by fantasizing (i.e., target values are drawn from the
-    current posterior, and acquisition functions are averaged over this
-    sample, see ``num_fantasy_samples``).
-
-    The GP surrogate model uses a Matern 5/2 covariance function with automatic
-    relevance determination (ARD) of input attributes, and a constant mean
-    function. The acquisition function is expected improvement (EI). All
-    hyperparameters of the surrogate model are estimated by empirical Bayes
-    (maximizing the marginal likelihood). In general, this hyperparameter
-    fitting is the most expensive part of a :meth:`get_config` call.
+    We implement Bayesian optimization, based on a model factory which
+    parameterizes the state transformer. This implementation works with
+    any type of surrogate model and acquisition function, which are
+    compatible with each other.
 
     The following happens in :meth:`get_config`:
 
     * For the first ``num_init_random`` calls, a config is drawn at random
       (after ``points_to_evaluate``, which are included in the ``num_init_random``
       initial ones). Afterwards, Bayesian optimization is used, unless there
-      are no finished evaluations yet (a surrogate model cannot be fix on no
-      data).
+      are no finished evaluations yet (a surrogate model cannot be used with no
+      data at all)
     * For BO, model hyperparameter are refit first. This step can be skipped
       (see ``opt_skip_*`` parameters).
-    * Next, ``num_init_candidates`` configs are sampled at random (as in random
-      search), and ranked by a scoring function (``initial_scoring``).
-    * BFGS local optimization is then run starting from the top scoring config,
-      where EI is minimized (this is skipped if
-      ``skip_local_optimization == True``).
-
-    Note that the full logic of construction based on arguments is given in
-    :mod:``syne_tune.optimizer.schedulers.searchers.gp_searcher_factory``. In
-    particular, see
-    :func:`~syne_tune.optimizer.schedulers.searchers.gp_searcher_factory.gp_fifo_searcher_defaults`
-    for default values.
-
-    Additional arguments on top of parent class
-    :class:`~syne_tune.optimizer.schedulers.searchers.StochasticSearcher`:
-
-    :param clone_from_state: Internal argument, do not use
-    :type clone_from_state: bool
-    :param resource_attr: Name of resource attribute in reports. This is
-        optional here, but required for multi-fidelity searchers.
-        If ``resource_attr`` and ``cost_attr`` are given, cost values are read from
-        each report and stored in the state. This allows cost models to be fit
-        on more data.
-    :type resource_attr: str, optional
-    :param cost_attr: Name of cost attribute in data obtained from reporter
-        (e.g., elapsed training time). Needed only by cost-aware searchers.
-        Depending on whether ``resource_attr`` is given, cost values are read
-        from each report or only at the end.
-    :type cost_attr: str, optional
-    :param num_init_random: Number of initial :meth:`get_config` calls for which
-        randomly sampled configs are returned. Afterwards, the model-based
-        searcher is used. Defaults to
-        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults.DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS`
-    :type num_init_random: int, optional
-    :param num_init_candidates: Number of initial candidates sampled at
-        random in order to seed the model-based search in ``get_config``.
-        Defaults to :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults.DEFAULT_NUM_INITIAL_CANDIDATES`
-    :type num_init_candidates: int, optional
-    :param num_fantasy_samples: Number of samples drawn for fantasizing
-        (latent target values for pending evaluations), defaults to 20
-    :type num_fantasy_samples: int, optional
-    :param no_fantasizing: If True, fantasizing is not done and pending
-        evaluations are ignored. This may lead to loss of diversity in
-        decisions. Defaults to ``False``
-    :type no_fantasizing: bool, optional
-    :param input_warping: If ``True``, we use a warping transform, so the kernel
-        function becomes :math:`k(w(x), w(x'))`, where :math:`w(x)` is a warping
-        transform parameterized by two non-negative numbers per component, which
-        are learned as hyperparameters. See also
-        :class:`~syne_tune.optimizer.schedulers.searcher.bayesopt.gpautograd.warping.Warping`.
-        Coordinates which belong to categorical hyperparameters, are not warped.
-        Defaults to ``False``.
-    :type input_warping: bool, optional
-    :param boxcox_transform: If ``True``, target values are transformed before
-        being fitted with a Gaussian marginal likelihood. This is using the Box-Cox
-        transform with a parameter :math:`\lambda`, which is learned alongside
-        other parameters of the surrogate model. The transform is :math:`\log y`
-        for :math:`\lambda = 0`, and :math:`y - 1` for :math:`\lambda = 1`. This
-        option requires the targets to be positive. Defaults to ``False``.
-    :type boxcox_transform: bool, optional
-    :param initial_scoring: Scoring function to rank initial candidates
-        (local optimization of EI is started from top scorer):
-
-        * "thompson_indep": Independent Thompson sampling; randomized score,
-          which can increase exploration
-        * "acq_func": score is the same (EI) acquisition function which is
-          used for local optimization afterwards
-
-        Defaults to
-        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults.DEFAULT_INITIAL_SCORING`
-    :type initial_scoring: str, optional
-    :param skip_local_optimization: If ``True``, the local gradient-based
-        optimization of the acquisition function is skipped, and the
-        top-ranked initial candidate (after initial scoring) is returned
-        instead. In this case, ``initial_scoring="acq_func"`` makes most
-        sense, otherwise the acquisition function will not be used.
-        Defaults to False
-    :type skip_local_optimization: bool, optional
-    :param opt_nstarts: Parameter for surrogate model fitting. Number of
-        random restarts. Defaults to 2
-    :type opt_nstarts: int, optional
-    :param opt_maxiter: Parameter for surrogate model fitting. Maximum
-        number of iterations per restart. Defaults to 50
-    :type opt_maxiter: int, optional
-    :param opt_warmstart: Parameter for surrogate model fitting. If ``True``,
-        each fitting is started from the previous optimum. Not recommended
-        in general. Defaults to ``False``
-    :type opt_warmstart: bool, optional
-    :param opt_verbose: Parameter for surrogate model fitting. If ``True``,
-        lots of output. Defaults to ``False``
-    :type opt_verbose: bool, optional
-    :param max_size_data_for_model: If this is set, we limit the number of
-        observations the surrogate model is fitted on this value. If there are
-        more observations, they are down sampled, see
-        :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state.SubsampleSingleFidelityStateConverter`
-        for details. This down sampling is repeated every time the model is
-        fit. The ``opt_skip_*`` predicates are evaluated before the state is
-        downsampled. Pass ``None`` not to apply such a threshold. The default is
-        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults.DEFAULT_MAX_SIZE_DATA_FOR_MODEL`.
-    :type max_size_data_for_model: int, optional
-    :param max_size_top_fraction: Only used if ``max_size_data_for_model`` is
-        set. This fraction of the down sampled set is filled with the top entries
-        in the full set, the remaining ones are sampled at random from the full
-        set, see
-        :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state.SubsampleSingleFidelityStateConverter`
-        for details. Defaults to 0.25.
-    :type max_size_top_fraction: float, optional
-    :param opt_skip_init_length: Parameter for surrogate model fitting,
-        skip predicate. Fitting is never skipped as long as number of
-        observations below this threshold. Defaults to 150
-    :type opt_skip_init_length: int, optional
-    :param opt_skip_period: Parameter for surrogate model fitting, skip
-        predicate. If ``>1``, and number of observations above
-        ``opt_skip_init_length``, fitting is done only K-th call, and skipped
-        otherwise. Defaults to 1 (no skipping)
-    :type opt_skip_period: int, optional
-    :param allow_duplicates: If ``True``, :meth:`get_config` may return the same
-        configuration more than once. Defaults to ``False``
-    :type allow_duplicates: bool, optional
-    :param restrict_configurations: If given, the searcher only suggests
-        configurations from this list. This needs
-        ``skip_local_optimization == True``. If ``allow_duplicates == False``,
-         entries are popped off this list once suggested.
-    :type restrict_configurations: List[dict], optional
-    :param map_reward: In the scheduler, the metric may be minimized or
-        maximized, but internally, Bayesian optimization is minimizing
-        the criterion. ``map_reward`` converts from metric to internal
-        criterion:
-
-        * "minus_x": ``criterion = -metric``
-        * "<a>_minus_x": ``criterion = <a> - metric``. For example "1_minus_x"
-          maps accuracy to zero-one error
-
-        From a technical standpoint, it does not matter what is chosen here,
-        because criterion is only used internally. Also note that criterion
-        data is always normalized to mean 0, variance 1 before fitted with a
-        Gaussian process. Defaults to "1_minus_x"
-    :type map_reward: str or :class:`MapReward`, optional
-    :param transfer_learning_task_attr: Used to support transfer HPO, where
-        the state contains observed data from several tasks, one of which
-        is the active one. To this end, ``config_space`` must contain a
-        categorical parameter of name ``transfer_learning_task_attr``, whose
-        range are all task IDs. Also, ``transfer_learning_active_task`` must
-        denote the active task, and ``transfer_learning_active_config_space``
-        is used as ``active_config_space`` argument in
-        :class:`~syne_tune.optimizer.schedulers.searchers.utils.HyperparameterRanges`.
-        This allows us to use a narrower search space for the active task than
-        for the union of all tasks (``config_space`` must be that), which is
-        needed if some configurations of non-active tasks lie outside of the
-        ranges in ``active_config_space``. One of the implications is that
-        :meth:`filter_observed_data` is selecting configs of the active task,
-        so that incumbents or exclusion lists are restricted to data from the
-        active task.
-    :type transfer_learning_task_attr: str, optional
-    :param transfer_learning_active_task: See ``transfer_learning_task_attr``.
-    :type transfer_learning_active_task: str, optional
-    :param transfer_learning_active_config_space:
-        See ``transfer_learning_task_attr``. If not given, ``config_space`` is the
-        search space for the active task as well. This active config space need
-        not contain the ``transfer_learning_task_attr`` parameter. In fact, this
-        parameter is set to a categorical with ``transfer_learning_active_task``
-        as single value, so that new configs are chosen for the active task
-        only.
-    :type transfer_learning_active_config_space: Dict[str, Any], optional
-    :param transfer_learning_model: See ``transfer_learning_task_attr``.
-        Specifies the surrogate model to be used for transfer learning:
-
-        * "matern52_product": Kernel is product of Matern 5/2 (not ARD) on
-          ``transfer_learning_task_attr`` and Matern 5/2 (ARD) on the rest.
-          Assumes that data from same task are more closely related than
-          data from different tasks
-        * "matern52_same": Kernel is Matern 5/2 (ARD) on the rest of the
-          variables, ``transfer_learning_task_attr`` is ignored. Assumes
-          that data from all tasks can be merged together
-
-        Defaults to "matern52_product"
-    :type transfer_learning_model: str, optional
+    * Next, the BO decision is made based on
+      :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm.BayesianOptimizationAlgorithm`.
+      This involves sampling `num_init_candidates`` configs are sampled at
+      random, ranking them with a scoring function (``initial_scoring``), and
+      finally runing local optimization starting from the top scoring config.
     """
 
-    def __init__(
-        self,
-        config_space: Dict[str, Any],
-        metric: str,
-        points_to_evaluate: Optional[List[Dict[str, Any]]] = None,
-        clone_from_state: bool = False,
-        **kwargs,
-    ):
-        super().__init__(
-            config_space,
-            metric=metric,
-            points_to_evaluate=points_to_evaluate,
-            random_seed_generator=kwargs.get("random_seed_generator"),
-            random_seed=kwargs.get("random_seed"),
-        )
-        if not clone_from_state:
-            kwargs["config_space"] = config_space
-            kwargs["metric"] = metric
-            kwargs_int = self._create_kwargs_int(kwargs)
-        else:
-            # Internal constructor, bypassing the factory
-            # Note: Members which are part of the mutable state, will be
-            # overwritten in ``_restore_from_state``
-            kwargs_int = kwargs.copy()
-        self._call_create_internal(kwargs_int)
-
-    def _create_kwargs_int(self, kwargs):
-        _kwargs = check_and_merge_defaults(
-            kwargs, *gp_fifo_searcher_defaults(kwargs), dict_name="search_options"
-        )
-        kwargs_int = gp_fifo_searcher_factory(**_kwargs)
-        # Extra arguments not parsed in factory
-        self._copy_kwargs_to_kwargs_int(kwargs_int, kwargs)
-        return kwargs_int
-
-    def _call_create_internal(self, kwargs_int):
-        """
-        Part of constructor which can be different in subclasses
-        """
-        self._create_internal(**kwargs_int)
-
     def configure_scheduler(self, scheduler):
         from syne_tune.optimizer.schedulers.scheduler_searcher import (
             TrialSchedulerWithSearcher,
         )
 
         assert isinstance(
             scheduler, TrialSchedulerWithSearcher
@@ -363,23 +546,20 @@
 
     def register_pending(
         self, trial_id: str, config: Optional[Dict[str, Any]] = None, milestone=None
     ):
         """
         Registers trial as pending. This means the corresponding evaluation
         task is running. Once it finishes, update is called for this trial.
-
         """
-        # It is OK for the candidate already to be registered as pending, in
-        # which case we do nothing
         state = self.state_transformer.state
         if not state.is_pending(trial_id):
             assert not state.is_labeled(trial_id), (
                 f"Trial trial_id = {trial_id} is already labeled, so cannot "
-                + "be pending"
+                "be pending"
             )
             self.state_transformer.append_trial(trial_id, config=config)
 
     def _fix_resource_attribute(self, **kwargs):
         pass
 
     def _postprocess_config(self, config: Dict[str, Any]) -> Dict[str, Any]:
@@ -435,22 +615,16 @@
             ]
 
     def _get_config_modelbased(
         self, exclusion_candidates, **kwargs
     ) -> Optional[Configuration]:
         # Obtain current :class:`SurrogateModel` from state transformer. Based on
         # this, the BO algorithm components can be constructed
-        if self.do_profile:
-            self.profiler.push_prefix("getconfig")
-            self.profiler.start("all")
-            self.profiler.start("gpmodel")
         # Note: Asking for the model triggers the posterior computation
         model = self.state_transformer.model()
-        if self.do_profile:
-            self.profiler.stop("gpmodel")
         # Select and fix target resource attribute (relevant in subclasses)
         self._fix_resource_attribute(**kwargs)
         # Create BO algorithm
         random_generator = self._create_random_generator()
         initial_candidates_scorer = create_initial_candidates_scorer(
             initial_scoring=self.initial_scoring,
             model=model,
@@ -469,30 +643,26 @@
             num_initial_candidates=self.num_initial_candidates,
             local_optimizer=local_optimizer,
             pending_candidate_state_transformer=None,
             exclusion_candidates=exclusion_candidates,
             num_requested_candidates=1,
             greedy_batch_selection=False,
             duplicate_detector=DuplicateDetectorIdentical(),
-            profiler=self.profiler,
             sample_unique_candidates=False,
             debug_log=self.debug_log,
         )
         # Next candidate decision
         _config = bo_algorithm.next_candidates()
         if len(_config) > 0:
             config = self._postprocess_config(_config[0])
             if self._restrict_configurations is not None:
                 # Remove ``config`` from ``_restrict_configurations``
                 self._update_restrict_configurations([config], random_generator)
         else:
             config = None
-        if self.do_profile:
-            self.profiler.stop("all")
-            self.profiler.pop_prefix()  # getconfig
         return config
 
     def get_batch_configs(
         self,
         batch_size: int,
         num_init_candidates_for_batch: Optional[int] = None,
         **kwargs,
@@ -633,24 +803,7 @@
             skip_local_optimization=self.skip_local_optimization,
             cost_attr=self._cost_attr,
             resource_attr=self._resource_attr,
             filter_observed_data=self._filter_observed_data,
             allow_duplicates=self._allow_duplicates,
             restrict_configurations=self._restrict_configurations,
         )
-
-    def clone_from_state(self, state):
-        # Create clone with mutable state taken from 'state'
-        init_state = decode_state(state["state"], self._hp_ranges_in_state())
-        skip_optimization = state["skip_optimization"]
-        model_factory = self.state_transformer.model_factory
-        # Call internal constructor
-        new_searcher = GPFIFOSearcher(
-            **self._new_searcher_kwargs_for_clone(),
-            model_factory=model_factory,
-            init_state=init_state,
-            skip_optimization=skip_optimization,
-        )
-        new_searcher._restore_from_state(state)
-        # Invalidate self (must not be used afterwards)
-        self.state_transformer = None
-        return new_searcher
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,28 +107,29 @@
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state_single_fidelity import (
     SubsampleSingleFidelityStateConverter,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
     StateForModelConverter,
 )
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 from syne_tune.optimizer.schedulers.searchers.utils.default_arguments import (
     Integer,
     Categorical,
     Boolean,
     Float,
     IntegerOrNone,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.warmstarting import (
     create_hp_ranges_for_warmstarting,
     create_filter_observed_data_for_warmstarting,
     create_base_gp_kernel_for_warmstarting,
 )
 from syne_tune.optimizer.schedulers.searchers import extract_random_seed
+from syne_tune.optimizer.schedulers.random_seeds import RANDOM_SEED_UPPER_BOUND
+
 
 __all__ = [
     "gp_fifo_searcher_factory",
     "gp_multifidelity_searcher_factory",
     "constrained_gp_fifo_searcher_factory",
     "cost_aware_coarse_gp_fifo_searcher_factory",
     "cost_aware_fine_gp_fifo_searcher_factory",
@@ -186,18 +187,14 @@
     mean = ScalarMeanFunction()
     optimization_config = OptimizationConfig(
         lbfgs_tol=DEFAULT_OPTIMIZATION_CONFIG.lbfgs_tol,
         lbfgs_maxiter=kwargs["opt_maxiter"],
         verbose=kwargs["opt_verbose"],
         n_starts=kwargs["opt_nstarts"],
     )
-    if kwargs.get("profiler", False):
-        profiler = SimpleProfiler()
-    else:
-        profiler = None
     if kwargs.get("debug_log", False):
         debug_log = DebugLogPrinter()
     else:
         debug_log = None
     if kwargs.get("boxcox_transform", False):
         target_transform = BoxCoxTargetTransform()
     else:
@@ -205,15 +202,14 @@
     filter_observed_data = create_filter_observed_data_for_warmstarting(**kwargs)
     return {
         "opt_warmstart": opt_warmstart,
         "kernel": kernel,
         "mean": mean,
         "target_transform": target_transform,
         "optimization_config": optimization_config,
-        "profiler": profiler,
         "debug_log": debug_log,
         "filter_observed_data": filter_observed_data,
     }
 
 
 def _create_gp_model_factory(
     gpmodel,
@@ -224,15 +220,14 @@
 ):
     filter_observed_data = result["filter_observed_data"]
     model_factory = GaussProcEmpiricalBayesModelFactory(
         active_metric=active_metric,
         gpmodel=gpmodel,
         num_fantasy_samples=kwargs["num_fantasy_samples"],
         normalize_targets=kwargs.get("normalize_targets", True),
-        profiler=result["profiler"],
         debug_log=result["debug_log"],
         filter_observed_data=filter_observed_data,
         no_fantasizing=kwargs.get("no_fantasizing", False),
         hp_ranges_for_prediction=hp_ranges_for_prediction,
     )
     return {
         "model_factory": model_factory,
@@ -367,15 +362,14 @@
     no_fantasizing = kwargs.get("no_fantasizing", False)
     num_fantasy_samples = 0 if no_fantasizing else kwargs["num_fantasy_samples"]
     model_factory = GaussProcAdditiveModelFactory(
         gpmodel=gpmodel,
         num_fantasy_samples=num_fantasy_samples,
         active_metric=active_metric,
         config_space_ext=config_space_ext,
-        profiler=result["profiler"],
         debug_log=result["debug_log"],
         filter_observed_data=filter_observed_data,
         normalize_targets=kwargs.get("normalize_targets", True),
     )
     return {
         "model_factory": model_factory,
         "filter_observed_data": filter_observed_data,
@@ -886,15 +880,14 @@
     is_restrict_configs: bool = False,
 ) -> (Set[str], dict, dict):
     mandatory = set()
 
     default_options = {
         "opt_skip_init_length": 150,
         "opt_skip_period": 1,
-        "profiler": False,
         "opt_maxiter": 50,
         "opt_nstarts": 2,
         "opt_warmstart": False,
         "opt_verbose": False,
         "opt_debug_writer": False,
         "num_fantasy_samples": 20,
         "scheduler": "fifo",
@@ -935,18 +928,17 @@
     ):
         default_options["max_size_data_for_model"] = DEFAULT_MAX_SIZE_DATA_FOR_MODEL
     if is_multi_output:
         default_options["initial_scoring"] = "acq_func"
         default_options["exponent_cost"] = 1.0
 
     constraints = {
-        "random_seed": Integer(0, 2**32 - 1),
+        "random_seed": Integer(0, RANDOM_SEED_UPPER_BOUND),
         "opt_skip_init_length": Integer(0, None),
         "opt_skip_period": Integer(1, None),
-        "profiler": Boolean(),
         "opt_maxiter": Integer(1, None),
         "opt_nstarts": Integer(1, None),
         "opt_warmstart": Boolean(),
         "opt_verbose": Boolean(),
         "opt_debug_writer": Boolean(),
         "num_fantasy_samples": Integer(1, None),
         "num_init_random": Integer(0, None),
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,484 +6,436 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-import time
-from typing import Optional, Type, Dict, Any, List
+from typing import Optional, List, Set, Dict, Any, Tuple
 import logging
+import numpy as np
 
-from syne_tune.optimizer.schedulers.searchers import (
-    StochasticSearcher,
-    RandomSearcher,
+from syne_tune.callbacks.remove_checkpoints_callback import (
+    DefaultRemoveCheckpointsSchedulerMixin,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
-    INTERNAL_METRIC_NAME,
-    MetricValues,
-    INTERNAL_COST_NAME,
-    TrialEvaluations,
-    dictionarize_objective,
+from syne_tune.optimizer.schedulers.random_seeds import RANDOM_SEED_UPPER_BOUND
+from syne_tune.optimizer.schedulers.synchronous.hyperband_bracket_manager import (
+    SynchronousHyperbandBracketManager,
+)
+from syne_tune.optimizer.schedulers.synchronous.hyperband_bracket import SlotInRung
+from syne_tune.optimizer.schedulers.synchronous.hyperband_rung_system import (
+    RungSystemsPerBracket,
+)
+from syne_tune.optimizer.scheduler import TrialSuggestion, SchedulerDecision
+from syne_tune.optimizer.schedulers.scheduler_searcher import TrialSchedulerWithSearcher
+from syne_tune.optimizer.schedulers.multi_fidelity import MultiFidelitySchedulerMixin
+from syne_tune.backend.trial_status import Trial
+from syne_tune.config_space import cast_config_values
+from syne_tune.optimizer.schedulers.searchers.utils.default_arguments import (
+    check_and_merge_defaults,
+    Categorical,
+    String,
+    assert_no_invalid_options,
+    Integer,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
-    TuningJobState,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_skipopt import (
-    SkipOptimizationPredicate,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
-    TransformerOutputModelFactory,
-    ModelStateTransformer,
-    StateForModelConverter,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    AcquisitionClassAndArgs,
-    LocalOptimizer,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm_components import (
-    NoOptimization,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
-    ExclusionList,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults import (
-    DEFAULT_NUM_INITIAL_CANDIDATES,
-    DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
-    DEFAULT_LOCAL_OPTIMIZER_CLASS,
-)
-from syne_tune.optimizer.schedulers.searchers.gp_searcher_utils import (
-    DEFAULT_INITIAL_SCORING,
-    SUPPORTED_INITIAL_SCORING,
-    MapReward,
-    encode_state,
-)
-from syne_tune.optimizer.schedulers.searchers.utils import HyperparameterRanges
-from syne_tune.optimizer.schedulers.searchers.utils.common import (
-    ConfigurationFilter,
-    Configuration,
-)
-from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
+from syne_tune.optimizer.schedulers.searchers.searcher import BaseSearcher
+from syne_tune.optimizer.schedulers.searchers.searcher_factory import searcher_factory
 
 logger = logging.getLogger(__name__)
 
 
-GET_CONFIG_RANDOM_RETRIES = 50
-
-
-def check_initial_candidates_scorer(initial_scoring: Optional[str]) -> str:
-    if initial_scoring is None:
-        return DEFAULT_INITIAL_SCORING
-    else:
-        assert (
-            initial_scoring in SUPPORTED_INITIAL_SCORING
-        ), "initial_scoring = '{}' is not supported".format(initial_scoring)
-        return initial_scoring
-
-
-class ModelBasedSearcher(StochasticSearcher):
-    """Common code for surrogate model based searchers
-
-    If ``num_initial_random_choices > 0``, initial configurations are drawn using
-    an internal :class:`~syne_tune.optimizer.schedulers.searchers.RandomSearcher`
-    object, which is created in :meth:`_assign_random_searcher`. This internal
-    random searcher shares :attr:`random_state` with the searcher here. This ensures
-    that if ``ModelBasedSearcher`` and ``RandomSearcher`` objects are created with
-    the same ``random_seed`` and ``points_to_evaluate`` argument, initial
-    configurations are identical until :meth:`_get_config_modelbased` kicks in.
-
-    Note that this works because :attr:`random_state` is only used in the internal
-    random searcher until meth:`_get_config_modelbased` is first called.
+_ARGUMENT_KEYS = {
+    "searcher",
+    "search_options",
+    "metric",
+    "mode",
+    "points_to_evaluate",
+    "random_seed",
+    "max_resource_attr",
+    "max_resource_level",
+    "resource_attr",
+    "searcher_data",
+}
+
+_DEFAULT_OPTIONS = {
+    "searcher": "random",
+    "mode": "min",
+    "resource_attr": "epoch",
+    "searcher_data": "rungs",
+}
+
+_CONSTRAINTS = {
+    "metric": String(),
+    "mode": Categorical(choices=("min", "max")),
+    "random_seed": Integer(0, RANDOM_SEED_UPPER_BOUND),
+    "max_resource_attr": String(),
+    "max_resource_level": Integer(1, None),
+    "resource_attr": String(),
+    "searcher_data": Categorical(("rungs", "all")),
+}
+
+
+class SynchronousHyperbandCommon(
+    TrialSchedulerWithSearcher, MultiFidelitySchedulerMixin
+):
+    """
+    Common code for :meth:`_create_internal` in
+    :class:`~syne_tune.optimizer.schedulers.synchronous.SynchronousHyperbandScheduler`
+    and
+    :class:`~syne_tune.optimizer.schedulers.synchronous.DifferentialEvolutionHyperbandScheduler`
     """
 
-    def _create_internal(
-        self,
-        hp_ranges: HyperparameterRanges,
-        model_factory: TransformerOutputModelFactory,
-        acquisition_class: AcquisitionClassAndArgs,
-        map_reward: Optional[MapReward] = None,
-        init_state: TuningJobState = None,
-        local_minimizer_class: Type[LocalOptimizer] = None,
-        skip_optimization: SkipOptimizationPredicate = None,
-        num_initial_candidates: int = DEFAULT_NUM_INITIAL_CANDIDATES,
-        num_initial_random_choices: int = DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
-        initial_scoring: Optional[str] = None,
-        skip_local_optimization: bool = False,
-        cost_attr: Optional[str] = None,
-        resource_attr: Optional[str] = None,
-        filter_observed_data: Optional[ConfigurationFilter] = None,
-        state_converter: Optional[StateForModelConverter] = None,
-        allow_duplicates: bool = False,
-        restrict_configurations: List[Dict[str, Any]] = None,
-    ):
-        self.hp_ranges = hp_ranges
-        self.num_initial_candidates = num_initial_candidates
-        self.num_initial_random_choices = num_initial_random_choices
-        self.map_reward = map_reward
-        if restrict_configurations is not None:
-            restrict_configurations = self._filter_points_to_evaluate(
-                restrict_configurations, hp_ranges, allow_duplicates
+    def _create_internal_common(
+        self, skip_searchers: Optional[Set[str]] = None, **kwargs
+    ) -> Dict[str, Any]:
+        self.metric = kwargs.get("metric")
+        assert self.metric is not None, (
+            "Argument 'metric' is mandatory. Pass the name of the metric "
+            + "reported by your training script, which you'd like to "
+            + "optimize, and use 'mode' to specify whether it should "
+            + "be minimized or maximized"
+        )
+        self.mode = kwargs["mode"]
+        self.max_resource_attr = kwargs.get("max_resource_attr")
+        self._resource_attr = kwargs["resource_attr"]
+        if self.max_resource_attr is None:
+            logger.warning(
+                "You do not specify max_resource_attr, but use max_resource_level "
+                "instead. This is not recommended best practice and may lead to a "
+                "loss of efficiency. Consider using max_resource_attr instead.\n"
+                "See https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/mf_setup.html#the-launcher-script "
+                "for details."
             )
-            if not skip_local_optimization:
-                logger.warning(
-                    "If restrict_configurations is given, need to have skip_local_optimization == True"
-                )
-                skip_local_optimization = True
-        self._restrict_configurations = restrict_configurations
-        if skip_local_optimization:
-            self.local_minimizer_class = NoOptimization
+        self._max_resource_level = self._infer_max_resource_level(
+            max_resource_level=kwargs.get("max_resource_level"),
+            max_resource_attr=self.max_resource_attr,
+        )
+        assert self._max_resource_level is not None, (
+            "Maximum resource level has to be specified, please provide "
+            "max_resource_attr or max_resource_level argument."
+        )
+        self._searcher_data = kwargs["searcher_data"]
+        # Generate searcher
+        searcher = kwargs["searcher"]
+        assert isinstance(
+            searcher, str
+        ), f"searcher must be of type string, but has type {type(searcher)}"
+        search_options = kwargs.get("search_options")
+        if search_options is None:
+            search_options = dict()
         else:
-            self.local_minimizer_class = (
-                DEFAULT_LOCAL_OPTIMIZER_CLASS
-                if local_minimizer_class is None
-                else local_minimizer_class
+            search_options = search_options.copy()
+        if skip_searchers is None or searcher not in skip_searchers:
+            search_options.update(
+                {
+                    "config_space": self.config_space.copy(),
+                    "metric": self.metric,
+                    "points_to_evaluate": kwargs.get("points_to_evaluate"),
+                    "mode": kwargs["mode"],
+                    "random_seed_generator": self.random_seed_generator,
+                    "resource_attr": self._resource_attr,
+                    "scheduler": "hyperband_synchronous",
+                }
             )
-        self.acquisition_class = acquisition_class
-        if isinstance(model_factory, dict):
-            model_factory_main = model_factory[INTERNAL_METRIC_NAME]
+            if searcher == "bayesopt":
+                search_options["max_epochs"] = self._max_resource_level
+            self._searcher: BaseSearcher = searcher_factory(searcher, **search_options)
         else:
-            model_factory_main = model_factory
-        self._debug_log = model_factory_main.debug_log
-        self.initial_scoring = check_initial_candidates_scorer(initial_scoring)
-        self.skip_local_optimization = skip_local_optimization
-        # Create state transformer
-        # Initial state is empty (note that the state is mutable).
-        # If there is a state converter, it uses the same random state as the searcher
-        # here
-        if state_converter is not None:
-            state_converter.set_random_state(self.random_state)
-        if init_state is None:
-            init_state = TuningJobState.empty_state(self._hp_ranges_in_state())
-        self.state_transformer = ModelStateTransformer(
-            model_factory=model_factory,
-            init_state=init_state,
-            skip_optimization=skip_optimization,
-            state_converter=state_converter,
-        )
-        self.set_profiler(model_factory_main.profiler)
-        self._cost_attr = cost_attr
-        self._resource_attr = resource_attr
-        self._filter_observed_data = filter_observed_data
-        self._allow_duplicates = allow_duplicates
-        self._random_searcher = None
-        # Tracks the cumulative time spent in ``get_config`` calls
-        self.cumulative_get_config_time = 0
-        if self._debug_log is not None:
-            msg_parts = [
-                "[ModelBasedSearcher._create_internal]",
-                f"- acquisition_class = {acquisition_class}",
-                f"- local_minimizer_class = {self.local_minimizer_class}",
-                f"- num_initial_candidates = {num_initial_candidates}",
-                f"- num_initial_random_choices = {num_initial_random_choices}",
-                f"- initial_scoring = {initial_scoring}",
-                f"- allow_duplicates = {self._allow_duplicates}",
-            ]
-            logger.info("\n".join(msg_parts))
+            self._searcher = None
+        return search_options
 
-    def _copy_kwargs_to_kwargs_int(
-        self, kwargs_int: Dict[str, Any], kwargs: Dict[str, Any]
-    ):
-        """Copies extra arguments not dealt with by ``gp_fifo_searcher_factory``
+    @property
+    def searcher(self) -> Optional[BaseSearcher]:
+        return self._searcher
 
-        :param kwargs_int: Output of factory, to be passed to ``searcher_factory``
-        :param kwargs: Input arguments
-        """
-        # Extra arguments not parsed in factory
-        for k in (
-            "init_state",
-            "local_minimizer_class",
-            "cost_attr",
-            "resource_attr",
-            "restrict_configurations",
-        ):
-            kwargs_int[k] = kwargs.get(k)
+    @property
+    def resource_attr(self) -> str:
+        return self._resource_attr
 
-    def _hp_ranges_in_state(self):
-        """
-        :return: ``HyperparameterRanges`` to be used in ``self.state_transformer.state``
-        """
-        return self.hp_ranges
+    @property
+    def max_resource_level(self) -> int:
+        return self._max_resource_level
 
-    def _hp_ranges_for_prediction(self):
-        """
-        :return: ``HyperparameterRanges`` to be used in predictions and acquisition
-            functions
-        """
-        return self._hp_ranges_in_state()
+    @property
+    def searcher_data(self) -> str:
+        return self._searcher_data
 
-    def _metric_val_update(
-        self, crit_val: float, result: Dict[str, Any]
-    ) -> MetricValues:
-        return crit_val
 
-    def on_trial_result(
+class SynchronousHyperbandScheduler(
+    SynchronousHyperbandCommon, DefaultRemoveCheckpointsSchedulerMixin
+):
+    """
+    Synchronous Hyperband. Compared to
+    :class:`~syne_tune.optimizer.schedulers.HyperbandScheduler`, this is also
+    scheduling jobs asynchronously, but decision-making is synchronized,
+    in that trials are only promoted to the next milestone once the rung they
+    are currently paused at, is completely occupied.
+
+    Our implementation never delays scheduling of a job. If the currently
+    active bracket does not accept jobs, we assign the job to a later bracket.
+    This means that at any point in time, several brackets can be active, but
+    jobs are preferentially assigned to the first one (the "primary" active
+    bracket).
+
+    :param config_space: Configuration space for trial evaluation function
+    :param bracket_rungs: Determines rung level systems for each bracket, see
+        :class:`~syne_tune.optimizer.schedulers.synchronous.hyperband_bracket_manager.SynchronousHyperbandBracketManager`
+    :param metric: Name of metric to optimize, key in result's obtained via
+        :meth:`on_trial_result`
+    :type metric: str
+    :param searcher: Searcher for ``get_config`` decisions. Passed to
+        :func:`~syne_tune.optimizer.schedulers.searchers.searcher_factory` along
+        with ``search_options`` and extra information. Supported values:
+        :const:`~syne_tune.optimizer.schedulers.searchers.searcher_factory.SUPPORTED_SEARCHERS_HYPERBAND`.
+        Defaults to "random" (i.e., random search)
+    :type searcher: str, optional
+    :param search_options: Passed to
+        :func:`~syne_tune.optimizer.schedulers.searchers.searcher_factory`.
+    :type search_options: Dict[str, Any], optional
+    :param mode: Mode to use for the metric given, can be "min" (default) or
+        "max"
+    :type mode: str, optional
+    :param points_to_evaluate: List of configurations to be evaluated
+        initially (in that order). Each config in the list can be partially
+        specified, or even be an empty dict. For each hyperparameter not
+        specified, the default value is determined using a midpoint heuristic.
+        If None (default), this is mapped to ``[dict()]``, a single default config
+        determined by the midpoint heuristic. If ``[]`` (empty list), no initial
+        configurations are specified.
+    :type points_to_evaluate: ``List[dict]``, optional
+    :param random_seed: Master random seed. Generators used in the scheduler
+        or searcher are seeded using
+        :class:`~syne_tune.optimizer.schedulers.random_seeds.RandomSeedGenerator`.
+        If not given, the master random seed is drawn at random here.
+    :type random_seed: int, optional
+    :param max_resource_attr: Key name in config for fixed attribute
+        containing the maximum resource. If given, trials need not be
+        stopped, which can run more efficiently.
+    :type max_resource_attr: str, optional
+    :param max_resource_level: Largest rung level, corresponds to ``max_t`` in
+        :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`. Must be positive
+        int larger than ``grace_period``. If this is not given, it is inferred
+        like in :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`. In
+        particular, it is not needed if ``max_resource_attr`` is given.
+    :type max_resource_level: int, optional
+    :param resource_attr: Name of resource attribute in results obtained via
+        ``:meth:`on_trial_result`. The type of resource must be int. Default to
+        "epoch"
+    :type resource_attr: str, optional
+    :param searcher_data: Relevant only if a model-based searcher is used.
+        Example: For NN tuning and ``resource_attr == "epoch"``, we receive a
+        result for each epoch, but not all epoch values are also rung levels.
+        searcher_data determines which of these results are passed to the
+        searcher. As a rule, the more data the searcher receives, the better
+        its fit, but also the more expensive get_config may become. Choices:
+
+        * "rungs" (default): Only results at rung levels. Cheapest
+        * "all": All results. Most expensive
+
+        Note: For a Gaussian additive learning curve surrogate model, this
+        has to be set to "all".
+    :type searcher_data: str, optional
+    """
+
+    def __init__(
         self,
-        trial_id: str,
-        config: Dict[str, Any],
-        result: Dict[str, Any],
-        update: bool,
+        config_space: Dict[str, Any],
+        bracket_rungs: RungSystemsPerBracket,
+        **kwargs,
     ):
-        # If both ``cost_attr`` and ``resource_attr`` are given, cost data (if
-        # given) is written out from every ``result``, independent of ``update``
-        cattr = self._cost_attr
-        rattr = self._resource_attr
-        if (
-            cattr is not None
-            and rattr is not None
-            and cattr in result
-            and rattr in result
-        ):
-            cost_val = float(result[cattr])
-            resource = str(result[rattr])
-            metrics = {INTERNAL_COST_NAME: {resource: cost_val}}
-            self.state_transformer.label_trial(
-                TrialEvaluations(trial_id=trial_id, metrics=metrics), config=config
-            )
-        if update:
-            self._update(trial_id, config, result)
+        super().__init__(config_space, **kwargs)
+        self._create_internal(bracket_rungs, **kwargs)
 
-    def _trial_id_string(self, trial_id: str, result: Dict[str, Any]):
-        """
-        For multi-fidelity, we also want to output the resource level
-        """
-        return trial_id
-
-    def _update(self, trial_id: str, config: Dict[str, Any], result: Dict[str, Any]):
-        metric_val = result[self._metric]
-        # Transform to criterion to be minimized
-        if self.map_reward is not None:
-            crit_val = self.map_reward(metric_val)
-        else:
-            crit_val = metric_val
-        metrics = dictionarize_objective(self._metric_val_update(crit_val, result))
-        # Cost value only dealt with here if ``resource_attr`` not given
-        attr = self._cost_attr
-        cost_val = None
-        if attr is not None and attr in result:
-            cost_val = float(result[attr])
-            if self._resource_attr is None:
-                metrics[INTERNAL_COST_NAME] = cost_val
-        self.state_transformer.label_trial(
-            TrialEvaluations(trial_id=trial_id, metrics=metrics), config=config
+    def _create_internal(self, bracket_rungs: RungSystemsPerBracket, **kwargs):
+        # Check values and impute default values
+        assert_no_invalid_options(
+            kwargs, _ARGUMENT_KEYS, name="SynchronousHyperbandScheduler"
         )
-        if self.debug_log is not None:
-            _trial_id = self._trial_id_string(trial_id, result)
-            msg = f"Update for trial_id {_trial_id}: metric = {metric_val:.3f}"
-            if self.map_reward is not None:
-                msg += f", crit_val = {crit_val:.3f}"
-            if cost_val is not None:
-                msg += f", cost_val = {cost_val:.2f}"
-            logger.info(msg)
-
-    def _get_config_modelbased(
-        self, exclusion_candidates: ExclusionList, **kwargs
-    ) -> Optional[Configuration]:
-        """
-        Implements ``get_config`` part if the surrogate model is used, instead
-        of initial choices from ``points_to_evaluate`` or initial random
-        choices.
-
-        :param exclusion_candidates: Configs to be avoided
-        :param kwargs: Extra arguments
-        :return: Suggested configuration, or None if configuration space is
-            exhausted
-        """
-        raise NotImplementedError
-
-    def _get_exclusion_candidates(self, skip_observed: bool = False) -> ExclusionList:
-        def skip_all(config: Configuration) -> bool:
-            return False
-
-        return ExclusionList(
-            self.state_transformer.state,
-            filter_observed_data=skip_all
-            if skip_observed
-            else self._filter_observed_data,
+        kwargs = check_and_merge_defaults(
+            kwargs, set(), _DEFAULT_OPTIONS, _CONSTRAINTS, dict_name="scheduler_options"
+        )
+        self._create_internal_common(**kwargs)
+        # Bracket manager
+        self.bracket_manager = SynchronousHyperbandBracketManager(
+            bracket_rungs,
+            mode=self.mode,
         )
+        # Maps trial_id to tuples (bracket_id, slot_in_rung), as returned
+        # by ``bracket_manager.next_job``, and required by
+        # ``bracket_manager.on_result``. Entries are removed once passed to
+        # ``on_result``. Note that a trial_id can be associated with different
+        # job descriptions in its lifetime
+        self._trial_to_pending_slot = dict()
+        # Maps trial_id (active) to config
+        self._trial_to_config = dict()
+        self._rung_levels = [level for _, level in bracket_rungs[0]]
+        self._trials_checkpoints_can_be_removed = []
 
-    def _should_pick_random_config(self, exclusion_candidates: ExclusionList) -> bool:
-        """
-        :param exclusion_candidates: Configs to be avoided
-        :return: Should config be drawn at random in ``get_config``
-        """
-        if len(exclusion_candidates) < self.num_initial_random_choices:
-            return True
-        # Determine whether there is any observed data after filtering
-        state = self.state_transformer.state
-        if not state.trials_evaluations:
-            return True
-        if self._filter_observed_data is None:
-            return False
-        for ev in state.trials_evaluations:
-            config = state.config_for_trial[ev.trial_id]
-            if self._filter_observed_data(config):
-                return False
-        return True
-
-    def _get_config_not_modelbased(
-        self, exclusion_candidates: ExclusionList
-    ) -> (Optional[Configuration], bool):
-        """
-        Does job of ``get_config``, as long as the decision does not involve
-        model-based search. If False is returned, model-based search must be
-        called.
+    @property
+    def rung_levels(self) -> List[int]:
+        return self._rung_levels
 
-        :param exclusion_candidates: Configs to be avoided
-        :return: ``(config, use_get_config_modelbased)``
-        """
-        self._assign_random_searcher()
-        config = self._next_initial_config()  # Ask for initial config
-        if config is None:
-            pick_random = self._should_pick_random_config(exclusion_candidates)
+    @property
+    def num_brackets(self) -> int:
+        return len(self.bracket_manager.bracket_rungs)
+
+    def _suggest(self, trial_id: int) -> Optional[TrialSuggestion]:
+        do_debug_log = self.searcher.debug_log is not None
+        if do_debug_log and trial_id == 0:
+            # This is printed at the start of the experiment. Cannot do this
+            # at construction, because with ``RemoteLauncher`` this does not end
+            # up in the right log
+            parts = ["Rung systems for each bracket:"] + [
+                f"Bracket {bracket}: {rungs}"
+                for bracket, rungs in enumerate(self.bracket_manager.bracket_rungs)
+            ]
+            logger.info("\n".join(parts))
+        # Ask bracket manager for job
+        bracket_id, slot_in_rung = self.bracket_manager.next_job()
+        suggestion = None
+        if slot_in_rung.trial_id is not None:
+            # Paused trial to be resumed (``trial_id`` passed in is ignored)
+            trial_id = slot_in_rung.trial_id
+            _config = self._trial_to_config[trial_id]
+            if self.max_resource_attr is not None:
+                config = dict(_config, **{self.max_resource_attr: slot_in_rung.level})
+            else:
+                config = _config
+            suggestion = TrialSuggestion.resume_suggestion(
+                trial_id=trial_id, config=config
+            )
+            if do_debug_log:
+                logger.info(f"trial_id {trial_id} promoted to {slot_in_rung.level}")
         else:
-            pick_random = True  # Initial configs count as random here
-        if pick_random and config is None:
-            if self.do_profile:
-                self.profiler.start("random")
-            for _ in range(GET_CONFIG_RANDOM_RETRIES):
-                _config = self._random_searcher.get_config()
-                if _config is None:
-                    # If ``RandomSearcher`` returns no config at all, the
-                    # search space is exhausted
-                    break
-                if not exclusion_candidates.contains(_config):
-                    config = _config
-                    break
-            if self.do_profile:
-                self.profiler.stop("random")
-            # ``_random_searcher`` modified ``restrict_configurations``
-            if self._restrict_configurations is not None:
-                self._restrict_configurations = (
-                    self._random_searcher._restrict_configurations.copy()
+            # New trial to be started (id is ``trial_id`` passed in)
+            config = self.searcher.get_config(trial_id=str(trial_id))
+            if config is not None:
+                config = cast_config_values(config, self.config_space)
+                self.searcher.register_pending(
+                    trial_id=str(trial_id), config=config, milestone=slot_in_rung.level
                 )
-        return config, pick_random
+                if self.max_resource_attr is not None:
+                    config[self.max_resource_attr] = slot_in_rung.level
+                self._trial_to_config[trial_id] = config
+                suggestion = TrialSuggestion.start_suggestion(config=config)
+                # Assign trial id to job descriptor
+                slot_in_rung.trial_id = trial_id
+                if do_debug_log:
+                    logger.info(
+                        f"trial_id {trial_id} starts (milestone = "
+                        f"{slot_in_rung.level})"
+                    )
+        if suggestion is not None:
+            assert trial_id not in self._trial_to_pending_slot, (
+                f"Trial for trial_id = {trial_id} is already registered as "
+                + "pending, cannot resume or start it"
+            )
+            self._trial_to_pending_slot[trial_id] = (bracket_id, slot_in_rung)
+        else:
+            # Searcher failed to return a config for a new trial_id. We report
+            # the corresponding job as failed, so that in case the experiment
+            # is continued, the bracket is not blocked with a slot which remains
+            # pending forever
+            logger.warning(
+                "Searcher failed to suggest a configuration for new trial "
+                f"{trial_id}. The corresponding rung slot is marked as failed."
+            )
+            self._report_as_failed(bracket_id, slot_in_rung)
+        return suggestion
 
-    def get_config(self, **kwargs) -> Optional[Dict[str, Any]]:
-        """
-        Runs Bayesian optimization in order to suggest the next config to evaluate.
+    def _on_result(self, result: Tuple[int, SlotInRung]):
+        trials_not_promoted = self.bracket_manager.on_result(result)
+        if trials_not_promoted is not None:
+            self._trials_checkpoints_can_be_removed.extend(trials_not_promoted)
+
+    def _report_as_failed(self, bracket_id: int, slot_in_rung: SlotInRung):
+        result_failed = SlotInRung(
+            rung_index=slot_in_rung.rung_index,
+            level=slot_in_rung.level,
+            slot_index=slot_in_rung.slot_index,
+            trial_id=slot_in_rung.trial_id,
+            metric_val=np.NAN,
+        )
+        self._on_result((bracket_id, result_failed))
 
-        :return: Next config to evaluate at
-        """
-        start_time = time.time()
-        state = self.state_transformer.state
-        if self.do_profile:
-            # Start new profiler block
-            skip_optimization = self.state_transformer.skip_optimization
-            if isinstance(skip_optimization, dict):
-                skip_optimization = skip_optimization[INTERNAL_METRIC_NAME]
-            meta = {
-                "fit_hyperparams": not skip_optimization(state),
-                "num_observed": state.num_observed_cases(),
-                "num_pending": len(state.pending_evaluations),
-            }
-            self.profiler.begin_block(meta)
-            self.profiler.start("all")
-        # Initial configs come from ``points_to_evaluate`` or are drawn at random
-        # We use ``exclusion_candidates`` even if ``allow_duplicates == True``, in order
-        # to count how many unique configs have been suggested
-        exclusion_candidates = self._get_exclusion_candidates()
-        config, pick_random = self._get_config_not_modelbased(exclusion_candidates)
-        if self.debug_log is not None:
-            trial_id = kwargs.get("trial_id")
-            self.debug_log.start_get_config(
-                "random" if pick_random else "BO", trial_id=trial_id
+    def on_trial_result(self, trial: Trial, result: Dict[str, Any]) -> str:
+        trial_id = trial.trial_id
+        if trial_id in self._trial_to_pending_slot:
+            bracket_id, slot_in_rung = self._trial_to_pending_slot[trial_id]
+            assert slot_in_rung.trial_id == trial_id  # Sanity check
+            assert self.metric in result, (
+                f"Result for trial_id {trial_id} does not contain "
+                + f"'{self.metric}' field"
+            )
+            metric_val = float(result[self.metric])
+            assert self._resource_attr in result, (
+                f"Result for trial_id {trial_id} does not contain "
+                + f"'{self._resource_attr}' field"
             )
-        if not pick_random:
-            # Model-based decision
-            if self._allow_duplicates or (
-                not exclusion_candidates.config_space_exhausted()
-            ):
-                # Even if ``allow_duplicates == True``, we exclude configs which are
-                # pending or failed
-                if self._allow_duplicates:
-                    excl_cands = self._get_exclusion_candidates(skip_observed=True)
-                else:
-                    excl_cands = exclusion_candidates
-                config = self._get_config_modelbased(
-                    exclusion_candidates=excl_cands, **kwargs
+            resource = int(result[self._resource_attr])
+            milestone = slot_in_rung.level
+            trial_decision = SchedulerDecision.CONTINUE
+            if resource >= milestone:
+                assert resource == milestone, (
+                    f"Trial trial_id {trial_id}: Obtained result for "
+                    + f"resource = {resource}, but not for {milestone}. "
+                    + "Training script must not skip rung levels!"
+                )
+                # Reached rung level: Pass result to bracket manager
+                slot_in_rung.metric_val = metric_val
+                self._on_result((bracket_id, slot_in_rung))
+                # Remove it from pending slots
+                del self._trial_to_pending_slot[trial_id]
+                # Trial should be paused
+                trial_decision = SchedulerDecision.PAUSE
+            prev_level = self.bracket_manager.level_to_prev_level(bracket_id, milestone)
+            if resource > prev_level:
+                # If the training script does not implement checkpointing, each
+                # trial starts from scratch. In this case, the condition
+                # ``resource > prev_level`` ensures that the searcher does not
+                # receive multiple reports for the same resource
+                update = self.searcher_data == "all" or resource == milestone
+                self.searcher.on_trial_result(
+                    trial_id=str(trial_id),
+                    config=self._trial_to_config[trial_id],
+                    result=result,
+                    update=update,
                 )
-
-        if config is not None:
-            if self.debug_log is not None:
-                self.debug_log.set_final_config(config)
-                # All get_config debug log info is only written here
-                self.debug_log.write_block()
         else:
-            msg = (
-                "Failed to sample a configuration not already chosen "
-                + f"before. Exclusion list has size {len(exclusion_candidates)}."
+            trial_decision = SchedulerDecision.STOP
+            logger.warning(
+                f"Received result for trial_id {trial_id}, which is not "
+                f"pending. This result is not used:\n{result}"
             )
-            cs_size = exclusion_candidates.configspace_size
-            if cs_size is not None:
-                msg += f" Configuration space has size {cs_size}."
-            logger.warning(msg)
-        if self.do_profile:
-            self.profiler.stop("all")
-            self.profiler.clear()
-        self.cumulative_get_config_time += time.time() - start_time
-
-        return config
-
-    def dataset_size(self):
-        return self.state_transformer.state.num_observed_cases()
 
-    def model_parameters(self):
-        return self.state_transformer.get_params()
+        return trial_decision
 
-    def set_params(self, param_dict):
-        self.state_transformer.set_params(param_dict)
-
-    def get_state(self) -> Dict[str, Any]:
-        """
-        The mutable state consists of the GP model parameters, the
-        ``TuningJobState``, and the ``skip_optimization`` predicate (which can have a
-        mutable state).
-        We assume that ``skip_optimization`` can be pickled.
-
-        Note that we do not have to store the state of :attr:`_random_searcher`,
-        since this internal searcher shares its ``random_state`` with the searcher
-        here.
+    def on_trial_error(self, trial: Trial):
         """
-        state = dict(
-            super().get_state(),
-            model_params=self.model_parameters(),
-            state=encode_state(self.state_transformer.state),
-            skip_optimization=self.state_transformer.skip_optimization,
-        )
-        if self._restrict_configurations is not None:
-            state["restrict_configurations"] = self._restrict_configurations
-        return state
-
-    def _restore_from_state(self, state: Dict[str, Any]):
-        super()._restore_from_state(state)
-        self.state_transformer.set_params(state["model_params"])
-        self._restrict_configurations = state.get("restrict_configurations")
-        # The internal random searcher is generated once needed, and it shares its
-        # ``random_state`` with this searcher here
-        self._random_searcher = None
-
-    def set_profiler(self, profiler: Optional[SimpleProfiler]):
-        self.profiler = profiler
-        self.do_profile = profiler is not None
+        Given the ``trial`` is currently pending, we send a result at its
+        milestone for metric value NaN. Such trials are ranked after all others
+        and will most likely not be promoted.
+
+        """
+        super().on_trial_error(trial)
+        trial_id = trial.trial_id
+        if trial_id in self._trial_to_pending_slot:
+            bracket_id, slot_in_rung = self._trial_to_pending_slot[trial_id]
+            self._report_as_failed(bracket_id, slot_in_rung)
+            # A failed trial is not pending anymore
+            del self._trial_to_pending_slot[trial_id]
+        else:
+            logger.warning(
+                f"Trial trial_id {trial_id} not registered at pending: "
+                "on_trial_error call is ignored"
+            )
 
-    @property
-    def debug_log(self):
-        return self._debug_log
+    def metric_names(self) -> List[str]:
+        return [self.metric]
 
-    def _assign_random_searcher(self):
-        """
-        Assigns :attr:`_random_searcher` if not already done. This internal searcher
-        is sharing :attr:`random_state` with the searcher here, see header comments.
-        """
-        if self._random_searcher is None:
-            # Used for initial random configs (if any)
-            # We do not have to deal with ``points_to_evaluate``
-            self._random_searcher = RandomSearcher(
-                self.hp_ranges.config_space_for_sampling,
-                metric=self._metric,
-                points_to_evaluate=[],
-                random_seed=0,
-                debug_log=False,
-                allow_duplicates=self._allow_duplicates,
-                restrict_configurations=self._restrict_configurations,
-            )
-            self._random_searcher.set_random_state(self.random_state)
+    def metric_mode(self) -> str:
+        return self.mode
+
+    def trials_checkpoints_can_be_removed(self) -> List[int]:
+        result = self._trials_checkpoints_can_be_removed
+        self._trials_checkpoints_can_be_removed = []
+        return result
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,15 @@
     Domain,
     config_space_size,
 )
 from syne_tune.optimizer.schedulers.searchers import (
     StochasticSearcher,
     StochasticAndFilterDuplicatesSearcher,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
-    ExclusionList,
-)
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
 from syne_tune.optimizer.schedulers.searchers.utils import make_hyperparameter_ranges
 
 logger = logging.getLogger(__name__)
 
@@ -199,15 +197,15 @@
 
         if not isinstance(shuffle_config, bool):
             shuffle_config = True
         self._shuffle_config = shuffle_config
         self._generate_all_candidates_on_grid()
         self._next_index = 0
         self._allow_duplicates = allow_duplicates
-        self._all_initial_configs = ExclusionList.empty_list(self._hp_ranges)
+        self._all_initial_configs = ExclusionList(self._hp_ranges)
 
     def _validate_config_space(
         self, config_space: Dict[str, Any], num_samples: Optional[Dict[str, int]]
     ):
         """
         Validates ``config_space`` from two aspects: first, that all
         hyperparameters are of acceptable types (i.e. float, integer,
@@ -338,15 +336,15 @@
             if self._all_initial_configs.contains(candidate):
                 candidate = None
             if self._allow_duplicates and self._next_index == num_combinations:
                 # Another round through the grid. It is important to reset
                 # ``_all_initial_configs`` to empty, so the initial configs can be
                 # suggested again in the second round
                 self._next_index = 0
-                self._all_initial_configs = ExclusionList.empty_list(self._hp_ranges)
+                self._all_initial_configs = ExclusionList(self._hp_ranges)
         return candidate
 
     def get_state(self) -> Dict[str, Any]:
         state = dict(
             super().get_state(),
             next_index=self._next_index,
             all_initial_configs=self._all_initial_configs.get_state(),
@@ -362,12 +360,12 @@
         )
         new_searcher._restore_from_state(state)
         return new_searcher
 
     def _restore_from_state(self, state: Dict[str, Any]):
         super()._restore_from_state(state)
         self._next_index = state["next_index"]
-        self._all_initial_configs = ExclusionList.empty_list(self._hp_ranges)
+        self._all_initial_configs = ExclusionList(self._hp_ranges)
         self._all_initial_configs.clone_from_state(state["all_initial_configs"])
 
     def _update(self, trial_id: str, config: Dict[str, Any], result: Dict[str, Any]):
         pass
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Optional, Dict, Any, List
 import logging
 import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers import BaseSearcher
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
-    ExclusionList,
-)
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils import (
     HyperparameterRanges,
     make_hyperparameter_ranges,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -221,15 +219,15 @@
         )
         self._hp_ranges = make_hyperparameter_ranges(config_space)
         if allow_duplicates is None:
             allow_duplicates = False
         self._allow_duplicates = allow_duplicates
         # Used to avoid returning the same config more than once. If
         # ``allow_duplicates == True``, this is used to block failed trials
-        self._excl_list = ExclusionList.empty_list(self._hp_ranges)
+        self._excl_list = ExclusionList(self._hp_ranges)
         # Maps ``trial_id`` to configuration. This is used to blacklist
         # configurations whose trial has failed (only if
         # `allow_duplicates == True``)
         self._config_for_trial_id = dict() if allow_duplicates else None
         # Assign ``_restrict_configurations`` and filter ``_points_to_evaluate``
         # accordingly
         if restrict_configurations is None:
@@ -349,15 +347,15 @@
             state["config_for_trial_id"] = self._config_for_trial_id
         if self._restrict_configurations is not None:
             state["restrict_configurations"] = self._restrict_configurations
         return state
 
     def _restore_from_state(self, state: Dict[str, Any]):
         super()._restore_from_state(state)
-        self._excl_list = ExclusionList.empty_list(self._hp_ranges)
+        self._excl_list = ExclusionList(self._hp_ranges)
         self._excl_list.clone_from_state(state["excl_list"])
         if self._allow_duplicates:
             self._config_for_trial_id = state["config_for_trial_id"]
         k = "restrict_configurations"
         if k in state:
             self._restrict_configurations = state[k]
         else:
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/common.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Optional, List, Tuple, Dict, Any
 import logging
 import numpy as np
 from dataclasses import dataclass
 
+from syne_tune.optimizer.schedulers.random_seeds import RANDOM_SEED_UPPER_BOUND
 from syne_tune.optimizer.schedulers.synchronous.dehb_bracket_manager import (
     DifferentialEvolutionHyperbandBracketManager,
 )
 from syne_tune.optimizer.schedulers.synchronous.hyperband_bracket import (
     SlotInRung,
 )
 from syne_tune.optimizer.schedulers.synchronous.hyperband import (
@@ -38,17 +39,15 @@
 )
 from syne_tune.optimizer.schedulers.searchers.searcher import (
     impute_points_to_evaluate,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges_factory import (
     make_hyperparameter_ranges,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
-    ExclusionList,
-)
+from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -77,15 +76,15 @@
     "support_pause_resume": True,
     "searcher_data": "rungs",
 }
 
 _CONSTRAINTS = {
     "metric": String(),
     "mode": Categorical(choices=("min", "max")),
-    "random_seed": Integer(0, 2**32 - 1),
+    "random_seed": Integer(0, RANDOM_SEED_UPPER_BOUND),
     "max_resource_attr": String(),
     "max_resource_level": Integer(1, None),
     "resource_attr": String(),
     "mutation_factor": Float(lower=0, upper=1),
     "crossover_probability": Float(lower=0, upper=1),
     "support_pause_resume": Boolean(),
     "searcher_data": Categorical(("rungs", "all")),
@@ -281,15 +280,15 @@
         self.bracket_manager = DifferentialEvolutionHyperbandBracketManager(
             rungs_first_bracket=rungs_first_bracket,
             mode=self.mode,
             num_brackets_per_iteration=num_brackets_per_iteration,
         )
         # Needed to convert encoded configs to configs
         self._hp_ranges = make_hyperparameter_ranges(self.config_space)
-        self._excl_list = ExclusionList.empty_list(self._hp_ranges)
+        self._excl_list = ExclusionList(self._hp_ranges)
         # PRNG for mutation and crossover random draws
         self.random_state = np.random.RandomState(self.random_seed_generator())
         # How often is selection skipped because target still pending?
         self.num_selection_skipped = 0
         # Maps ``trial_id`` to ``ext_slot``, as returned by ``bracket_manager.next_job``,
         # and required by ``bracket_manager.on_result``. Entries are removed once
         # passed to ``on_result``. Here, ``ext_slot`` is of type ``ExtendedSlotInRung``.
```

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/__init__.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/successive_halving.py` & `syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/successive_halving.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/remote/__init__.py` & `syne_tune-0.6.0/syne_tune/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/remote/estimators.py` & `syne_tune-0.6.0/syne_tune/remote/estimators.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/remote/remote_launcher.py` & `syne_tune-0.6.0/syne_tune/remote/remote_launcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/remote/remote_main.py` & `syne_tune-0.6.0/syne_tune/remote/remote_main.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/remote/remote_metrics_callback.py` & `syne_tune-0.6.0/syne_tune/remote/remote_metrics_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/report.py` & `syne_tune-0.6.0/syne_tune/report.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/results_callback.py` & `syne_tune-0.6.0/syne_tune/results_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/stopping_criterion.py` & `syne_tune-0.6.0/syne_tune/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/try_import.py` & `syne_tune-0.6.0/syne_tune/try_import.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 
 def try_import_kde_message() -> str:
     return _try_import_message("KDE searchers are not imported", tag="kde")
 
 
 def try_import_bore_message() -> str:
-    return _try_import_message("BORE searchers are not imported", tag="bore")
+    return _try_import_message(
+        "BORE searchers are not imported (not contained in extra)", tag="bore"
+    )
 
 
 def try_import_raytune_message() -> str:
     return _try_import_message(
         "Ray Tune schedulers and searchers are not imported", tag="raytune"
     )
 
@@ -40,15 +42,18 @@
 
 
 def try_import_aws_message() -> str:
     return _try_import_message("AWS dependencies are not imported", tag="aws")
 
 
 def try_import_botorch_message() -> str:
-    return _try_import_message("BoTorch dependencies are not imported", tag="botorch")
+    return _try_import_message(
+        "BoTorch dependencies are not imported (needs Python 3.8 or later)",
+        tag="botorch",
+    )
 
 
 def try_import_blackbox_repository_message() -> str:
     return _try_import_message(
         "Dependencies of blackbox repository are not imported",
         tag="blackbox-repository",
     )
@@ -57,23 +62,29 @@
 def try_import_yahpo_message() -> str:
     return _try_import_message(
         "Dependencies of YAHPO are not imported",
         tag="yahpo",
     )
 
 
-def try_import_backends_message() -> str:
+def try_import_moo_message() -> str:
     return _try_import_message(
-        "LocalBackend / PythonBackend are not imported", tag=None
+        "Multi Objective Optimization dependencies are not imported", tag="moo"
     )
 
 
-def try_import_moo_message() -> str:
+def try_import_visual_message() -> str:
     return _try_import_message(
-        "Multi Objective Optimization dependencies are not imported", tag="moo"
+        "Dependencies for visualization are not imported", tag="visual"
+    )
+
+
+def try_import_backends_message() -> str:
+    return _try_import_message(
+        "LocalBackend / PythonBackend are not imported", tag=None
     )
 
 
 def _try_import_message(message_text: str, tag: Optional[str]) -> str:
     if tag is None:
         insert = ""
     else:
```

### Comparing `syne_tune-0.5.0/syne_tune/tuner.py` & `syne_tune-0.6.0/syne_tune/tuner.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/tuner_callback.py` & `syne_tune-0.6.0/syne_tune/tuner_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/tuning_status.py` & `syne_tune-0.6.0/syne_tune/tuning_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/util.py` & `syne_tune-0.6.0/syne_tune/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 from pathlib import Path
 from typing import Optional, List, Union, Dict, Any, Iterable
 from time import perf_counter
 from contextlib import contextmanager
 
 import numpy as np
 
-from syne_tune.constants import SYNE_TUNE_DEFAULT_FOLDER, SYNE_TUNE_ENV_FOLDER
+from syne_tune.constants import (
+    SYNE_TUNE_DEFAULT_FOLDER,
+    SYNE_TUNE_ENV_FOLDER,
+    ST_DATETIME_FORMAT,
+)
 from syne_tune.try_import import try_import_aws_message
 
 try:
     import sagemaker
 except ImportError:
     print(try_import_aws_message())
 
@@ -139,17 +143,16 @@
         check_valid_sagemaker_name(default)
         base = default
     else:
         check_valid_sagemaker_name(base)
 
     moment = time.time()
     moment_ms = repr(moment).split(".")[1][:3]
-    timestamp = time.strftime(
-        "%Y-%m-%d-%H-%M-%S-{}".format(moment_ms), time.gmtime(moment)
-    )
+    format = ST_DATETIME_FORMAT + f"-{moment_ms}"
+    timestamp = time.strftime(format, time.gmtime(moment))
     trimmed_base = base[: max_length - len(timestamp) - 1]
     return "{}-{}".format(trimmed_base, timestamp)
 
 
 def random_string(length: int) -> str:
     pool = string.ascii_letters + string.digits
     return "".join(random.choice(pool) for _ in range(length))
```

### Comparing `syne_tune-0.5.0/syne_tune/utils/__init__.py` & `syne_tune-0.6.0/syne_tune/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/utils/checkpoint.py` & `syne_tune-0.6.0/syne_tune/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune/utils/config_as_json.py` & `syne_tune-0.6.0/syne_tune/utils/config_as_json.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.5.0/syne_tune.egg-info/PKG-INFO` & `syne_tune-0.6.0/syne_tune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne-tune
-Version: 0.5.0
+Version: 0.6.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `syne_tune-0.5.0/syne_tune.egg-info/SOURCES.txt` & `syne_tune-0.6.0/syne_tune.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 NOTICE
 README.md
 setup.cfg
 setup.py
 syne_tune/__init__.py
 syne_tune/config_space.py
 syne_tune/constants.py
-syne_tune/experiments.py
 syne_tune/num_gpu.py
 syne_tune/report.py
 syne_tune/results_callback.py
 syne_tune/stopping_criterion.py
 syne_tune/try_import.py
 syne_tune/tuner.py
 syne_tune/tuner_callback.py
@@ -65,14 +64,17 @@
 syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
 syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
 syne_tune/callbacks/__init__.py
 syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
 syne_tune/callbacks/hyperband_remove_checkpoints_score.py
 syne_tune/callbacks/remove_checkpoints_callback.py
 syne_tune/callbacks/tensorboard_callback.py
+syne_tune/experiments/__init__.py
+syne_tune/experiments/experiment_result.py
+syne_tune/experiments/results_utils.py
 syne_tune/optimizer/__init__.py
 syne_tune/optimizer/baselines.py
 syne_tune/optimizer/scheduler.py
 syne_tune/optimizer/schedulers/__init__.py
 syne_tune/optimizer/schedulers/fifo.py
 syne_tune/optimizer/schedulers/hyperband.py
 syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
@@ -175,21 +177,18 @@
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
-syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/common.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
-syne_tune/optimizer/schedulers/searchers/bayesopt/utils/density.py
-syne_tune/optimizer/schedulers/searchers/bayesopt/utils/duplicate_detector.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
 syne_tune/optimizer/schedulers/searchers/bore/__init__.py
 syne_tune/optimizer/schedulers/searchers/bore/bore.py
 syne_tune/optimizer/schedulers/searchers/bore/de.py
 syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
 syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
 syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
@@ -208,14 +207,15 @@
 syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
 syne_tune/optimizer/schedulers/searchers/kde/__init__.py
 syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
 syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
 syne_tune/optimizer/schedulers/searchers/utils/__init__.py
 syne_tune/optimizer/schedulers/searchers/utils/common.py
 syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
+syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
 syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
 syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
 syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
 syne_tune/optimizer/schedulers/searchers/utils/scaling.py
 syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
 syne_tune/optimizer/schedulers/synchronous/__init__.py
 syne_tune/optimizer/schedulers/synchronous/dehb.py
```


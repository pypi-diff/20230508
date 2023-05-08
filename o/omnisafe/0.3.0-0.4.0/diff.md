# Comparing `tmp/omnisafe-0.3.0.tar.gz` & `tmp/omnisafe-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnisafe-0.3.0.tar", last modified: Sat Apr  1 01:00:08 2023, max compression
+gzip compressed data, was "omnisafe-0.4.0.tar", last modified: Mon May  8 20:07:23 2023, max compression
```

## Comparing `omnisafe-0.3.0.tar` & `omnisafe-0.4.0.tar`

### file list

```diff
@@ -1,148 +1,209 @@
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/
--rw-r--r--   0 borong    (1000) borong    (1000)    11375 2023-03-28 07:12:07.000000 omnisafe-0.3.0/LICENSE
--rw-r--r--   0 borong    (1000) borong    (1000)       43 2023-04-01 00:44:06.000000 omnisafe-0.3.0/MANIFEST.in
--rw-r--r--   0 borong    (1000) borong    (1000)    17442 2023-04-01 01:00:08.449923 omnisafe-0.3.0/PKG-INFO
--rw-r--r--   0 borong    (1000) borong    (1000)    16163 2023-04-01 00:44:06.000000 omnisafe-0.3.0/README.md
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.429923 omnisafe-0.3.0/omnisafe/
--rw-r--r--   0 borong    (1000) borong    (1000)     1107 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/__init__.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/adapter/
--rw-r--r--   0 borong    (1000) borong    (1000)     1051 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/adapter/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     1935 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/adapter/early_terminated_adapter.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6070 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/adapter/offpolicy_adapter.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6497 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/adapter/online_adapter.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6697 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/adapter/onpolicy_adapter.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5057 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/adapter/saute_adapter.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2509 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/adapter/simmer_adapter.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/
--rw-r--r--   0 borong    (1000) borong    (1000)     1969 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     9072 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/algo_wrapper.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2392 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/base_algo.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/off_policy/
--rw-r--r--   0 borong    (1000) borong    (1000)      915 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/off_policy/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)    13923 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/off_policy/ddpg.py
--rw-r--r--   0 borong    (1000) borong    (1000)     8645 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/off_policy/sac.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6300 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/off_policy/td3.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/on_policy/
--rw-r--r--   0 borong    (1000) borong    (1000)     1871 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/__init__.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/
--rw-r--r--   0 borong    (1000) borong    (1000)     1069 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     9274 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/natural_pg.py
--rw-r--r--   0 borong    (1000) borong    (1000)    22375 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/policy_gradient.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2928 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/ppo.py
--rw-r--r--   0 borong    (1000) borong    (1000)     8764 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/trpo.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/on_policy/first_order/
--rw-r--r--   0 borong    (1000) borong    (1000)      887 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/first_order/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     9008 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/first_order/cup.py
--rw-r--r--   0 borong    (1000) borong    (1000)     8370 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/first_order/focops.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/
--rw-r--r--   0 borong    (1000) borong    (1000)     1148 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2644 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/crpo.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2819 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py
--rw-r--r--   0 borong    (1000) borong    (1000)     3727 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2957 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py
--rw-r--r--   0 borong    (1000) borong    (1000)     3641 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/on_policy/penalty_function/
--rw-r--r--   0 borong    (1000) borong    (1000)      891 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/penalty_function/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2616 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/penalty_function/ipo.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5161 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/penalty_function/p3o.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/algorithms/on_policy/second_order/
--rw-r--r--   0 borong    (1000) borong    (1000)      884 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/second_order/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)    16168 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/second_order/cpo.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6022 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/on_policy/second_order/pcpo.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2219 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/algorithms/registry.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/common/
--rw-r--r--   0 borong    (1000) borong    (1000)      923 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/common/__init__.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/common/buffer/
--rw-r--r--   0 borong    (1000) borong    (1000)     1199 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/common/buffer/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4686 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/buffer/base.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4045 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/buffer/offpolicy_buffer.py
--rw-r--r--   0 borong    (1000) borong    (1000)    17971 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/buffer/onpolicy_buffer.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4978 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/buffer/vector_offpolicy_buffer.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5721 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/buffer/vector_onpolicy_buffer.py
--rw-r--r--   0 borong    (1000) borong    (1000)    24155 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/experiment_grid.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4228 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/lagrange.py
--rw-r--r--   0 borong    (1000) borong    (1000)    14215 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/logger.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5163 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/normalizer.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5032 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/pid_lagrange.py
--rw-r--r--   0 borong    (1000) borong    (1000)    14627 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/common/statistics_tools.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.429923 omnisafe-0.3.0/omnisafe/configs/
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.439923 omnisafe-0.3.0/omnisafe/configs/off-policy/
--rw-r--r--   0 borong    (1000) borong    (1000)     3409 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/off-policy/DDPG.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3559 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/off-policy/SAC.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3575 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/off-policy/TD3.yaml
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/omnisafe/configs/on-policy/
--rw-r--r--   0 borong    (1000) borong    (1000)     4219 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/CPO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3911 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/CUP.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     4081 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/FOCOPS.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3981 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/IPO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     4632 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/NaturalPG.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3608 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/OnCRPO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3607 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/P3O.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     4219 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/PCPO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3804 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/PDO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3514 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/PPO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3834 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/PPOLag.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     3483 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/PolicyGradient.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     4265 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/RCPO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     4602 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/TRPO.yaml
--rw-r--r--   0 borong    (1000) borong    (1000)     4513 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/configs/on-policy/TRPOLag.yaml
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/omnisafe/envs/
--rw-r--r--   0 borong    (1000) borong    (1000)      858 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/envs/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)    13003 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/envs/core.py
--rw-r--r--   0 borong    (1000) borong    (1000)     7057 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/envs/safety_gymnasium_env.py
--rw-r--r--   0 borong    (1000) borong    (1000)    19101 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/envs/wrapper.py
--rw-r--r--   0 borong    (1000) borong    (1000)    12381 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/evaluator.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/omnisafe/models/
--rw-r--r--   0 borong    (1000) borong    (1000)     1507 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/models/__init__.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/omnisafe/models/actor/
--rw-r--r--   0 borong    (1000) borong    (1000)     1088 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/models/actor/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4050 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor/actor_builder.py
--rw-r--r--   0 borong    (1000) borong    (1000)     1415 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor/gaussian_actor.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5011 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor/gaussian_learning_actor.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6029 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor/gaussian_sac_actor.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4244 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor/mlp_actor.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/omnisafe/models/actor_critic/
--rw-r--r--   0 borong    (1000) borong    (1000)     1035 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor_critic/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6367 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor_critic/actor_critic.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6168 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor_critic/actor_q_critic.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5031 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor_critic/constraint_actor_critic.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4453 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/actor_critic/constraint_actor_q_critic.py
--rw-r--r--   0 borong    (1000) borong    (1000)     8799 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/base.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/omnisafe/models/critic/
--rw-r--r--   0 borong    (1000) borong    (1000)      935 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/models/critic/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4105 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/critic/critic_builder.py
--rw-r--r--   0 borong    (1000) borong    (1000)     5332 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/critic/q_critic.py
--rw-r--r--   0 borong    (1000) borong    (1000)     3008 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/models/critic/v_critic.py
--rw-r--r--   0 borong    (1000) borong    (1000)     1557 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/typing.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/omnisafe/utils/
--rw-r--r--   0 borong    (1000) borong    (1000)      685 2023-03-28 07:12:07.000000 omnisafe-0.3.0/omnisafe/utils/__init__.py
--rw-r--r--   0 borong    (1000) borong    (1000)    16095 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/command_app.py
--rw-r--r--   0 borong    (1000) borong    (1000)    14113 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/config.py
--rw-r--r--   0 borong    (1000) borong    (1000)    10654 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/distributed.py
--rw-r--r--   0 borong    (1000) borong    (1000)     1651 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/exp_grid_tools.py
--rw-r--r--   0 borong    (1000) borong    (1000)     9641 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/math.py
--rw-r--r--   0 borong    (1000) borong    (1000)     4724 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/model.py
--rw-r--r--   0 borong    (1000) borong    (1000)    13526 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/plotter.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2683 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/schedule.py
--rw-r--r--   0 borong    (1000) borong    (1000)     9150 2023-04-01 00:44:06.000000 omnisafe-0.3.0/omnisafe/utils/tools.py
--rw-r--r--   0 borong    (1000) borong    (1000)     1812 2023-04-01 00:59:53.000000 omnisafe-0.3.0/omnisafe/version.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.429923 omnisafe-0.3.0/omnisafe.egg-info/
--rw-r--r--   0 borong    (1000) borong    (1000)    17442 2023-04-01 01:00:08.000000 omnisafe-0.3.0/omnisafe.egg-info/PKG-INFO
--rw-r--r--   0 borong    (1000) borong    (1000)     4376 2023-04-01 01:00:08.000000 omnisafe-0.3.0/omnisafe.egg-info/SOURCES.txt
--rw-r--r--   0 borong    (1000) borong    (1000)        1 2023-04-01 01:00:08.000000 omnisafe-0.3.0/omnisafe.egg-info/dependency_links.txt
--rw-r--r--   0 borong    (1000) borong    (1000)       60 2023-04-01 01:00:08.000000 omnisafe-0.3.0/omnisafe.egg-info/entry_points.txt
--rw-r--r--   0 borong    (1000) borong    (1000)      465 2023-04-01 01:00:08.000000 omnisafe-0.3.0/omnisafe.egg-info/requires.txt
--rw-r--r--   0 borong    (1000) borong    (1000)        9 2023-04-01 01:00:08.000000 omnisafe-0.3.0/omnisafe.egg-info/top_level.txt
--rw-r--r--   0 borong    (1000) borong    (1000)     5657 2023-04-01 00:44:06.000000 omnisafe-0.3.0/pyproject.toml
--rw-r--r--   0 borong    (1000) borong    (1000)       38 2023-04-01 01:00:08.449923 omnisafe-0.3.0/setup.cfg
--rwxr-xr-x   0 borong    (1000) borong    (1000)     1533 2023-04-01 00:44:06.000000 omnisafe-0.3.0/setup.py
-drwxr-xr-x   0 borong    (1000) borong    (1000)        0 2023-04-01 01:00:08.449923 omnisafe-0.3.0/tests/
--rw-r--r--   0 borong    (1000) borong    (1000)    15876 2023-04-01 00:44:06.000000 omnisafe-0.3.0/tests/test_buffer.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2796 2023-04-01 00:44:06.000000 omnisafe-0.3.0/tests/test_cli.py
--rw-r--r--   0 borong    (1000) borong    (1000)     2006 2023-03-28 07:12:07.000000 omnisafe-0.3.0/tests/test_env.py
--rw-r--r--   0 borong    (1000) borong    (1000)     3184 2023-04-01 00:44:06.000000 omnisafe-0.3.0/tests/test_experiment_grid.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6790 2023-04-01 00:44:06.000000 omnisafe-0.3.0/tests/test_model.py
--rw-r--r--   0 borong    (1000) borong    (1000)     1564 2023-03-28 07:12:07.000000 omnisafe-0.3.0/tests/test_normalizer.py
--rw-r--r--   0 borong    (1000) borong    (1000)     9812 2023-04-01 00:44:06.000000 omnisafe-0.3.0/tests/test_policy.py
--rw-r--r--   0 borong    (1000) borong    (1000)     1478 2023-04-01 00:44:06.000000 omnisafe-0.3.0/tests/test_statistics_tools.py
--rw-r--r--   0 borong    (1000) borong    (1000)     6106 2023-04-01 00:44:06.000000 omnisafe-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.118508 omnisafe-0.4.0/
+-rw-r--r--   0 jiaming    (501) staff       (20)    11375 2023-05-08 19:46:32.000000 omnisafe-0.4.0/LICENSE
+-rw-r--r--   0 jiaming    (501) staff       (20)       43 2023-05-08 19:46:32.000000 omnisafe-0.4.0/MANIFEST.in
+-rw-r--r--   0 jiaming    (501) staff       (20)    17209 2023-05-08 20:07:23.118334 omnisafe-0.4.0/PKG-INFO
+-rw-r--r--   0 jiaming    (501) staff       (20)    16005 2023-05-08 19:53:25.000000 omnisafe-0.4.0/README.md
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.094657 omnisafe-0.4.0/omnisafe/
+-rw-r--r--   0 jiaming    (501) staff       (20)      997 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.096581 omnisafe-0.4.0/omnisafe/adapter/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1117 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/adapter/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3332 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/early_terminated_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    13974 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/adapter/modelbased_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7703 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/offpolicy_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8063 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/online_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6745 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/onpolicy_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     9663 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/saute_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4872 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/simmer_adapter.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.097152 omnisafe-0.4.0/omnisafe/algorithms/
+-rw-r--r--   0 jiaming    (501) staff       (20)     2054 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    10644 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/algo_wrapper.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2583 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/base_algo.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.098139 omnisafe-0.4.0/omnisafe/algorithms/model_based/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1166 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.098745 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/
+-rw-r--r--   0 jiaming    (501) staff       (20)      892 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    30036 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/ensemble.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    16182 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/loop.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    19238 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/pets.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5077 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/cap_pets.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3640 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/cce_pets.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.099717 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1252 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    13125 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/arc.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7088 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cap.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6127 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cce.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    11664 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cem.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4926 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/rce.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    10530 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/safe_arc.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3567 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/rce_pets.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4071 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/safeloop.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.100648 omnisafe-0.4.0/omnisafe/algorithms/off_policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1107 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    22970 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/ddpg.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3989 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/ddpg_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8556 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/sac.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4068 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/sac_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5071 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/td3.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3908 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/td3_lag.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.100782 omnisafe-0.4.0/omnisafe/algorithms/on_policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1848 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.101702 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1069 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     9606 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/natural_pg.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    25220 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/policy_gradient.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3188 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/ppo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8719 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/trpo.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.102153 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1018 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2467 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2373 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.102588 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/
+-rw-r--r--   0 jiaming    (501) staff       (20)      887 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     9137 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/cup.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8843 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/focops.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.103370 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1148 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3068 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/crpo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3936 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4057 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4076 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3973 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.103769 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/
+-rw-r--r--   0 jiaming    (501) staff       (20)      891 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2891 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/ipo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5136 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/p3o.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.104158 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/
+-rw-r--r--   0 jiaming    (501) staff       (20)      907 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4115 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3963 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.104537 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/
+-rw-r--r--   0 jiaming    (501) staff       (20)      918 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2927 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/ppo_saute.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2939 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/trpo_saute.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.104951 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/
+-rw-r--r--   0 jiaming    (501) staff       (20)      884 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    19058 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/cpo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5867 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/pcpo.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.105341 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/
+-rw-r--r--   0 jiaming    (501) staff       (20)      947 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3216 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3228 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2225 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/registry.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.106576 omnisafe-0.4.0/omnisafe/common/
+-rw-r--r--   0 jiaming    (501) staff       (20)      923 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.107466 omnisafe-0.4.0/omnisafe/common/buffer/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1199 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5226 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/base.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4184 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/common/buffer/offpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    18538 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/onpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4919 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/vector_offpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5997 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/vector_onpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    26453 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/common/experiment_grid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5272 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/lagrange.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    14926 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/logger.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5822 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/normalizer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5170 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/pid_lagrange.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7026 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/simmer_agent.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    16410 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/common/statistics_tools.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.092099 omnisafe-0.4.0/omnisafe/configs/
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.108328 omnisafe-0.4.0/omnisafe/configs/model-based/
+-rw-r--r--   0 jiaming    (501) staff       (20)     5127 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/CAPPETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4822 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/CCEPETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6646 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/LOOP.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4656 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/PETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4825 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/RCEPETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6757 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/SafeLOOP.yaml
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.109164 omnisafe-0.4.0/omnisafe/configs/off-policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     3237 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/DDPG.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3557 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/DDPGLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3438 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/SAC.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3757 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/SACLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3333 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/TD3.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3653 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/TD3Lag.yaml
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.112169 omnisafe-0.4.0/omnisafe/configs/on-policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     4219 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/CPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4347 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/CPPOPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3916 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/CUP.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4086 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/FOCOPS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3984 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/IPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3759 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/NaturalPG.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3611 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/OnCRPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3610 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/P3O.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4219 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PCPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3807 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PDO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3519 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3826 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3839 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3763 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOSaute.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4064 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOSimmerPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3488 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PolicyGradient.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4265 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/RCPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4602 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3789 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4515 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4587 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3969 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOSaute.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4271 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.112973 omnisafe-0.4.0/omnisafe/envs/
+-rw-r--r--   0 jiaming    (501) staff       (20)      985 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    12363 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/envs/core.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6122 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/mujoco_env.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7596 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/envs/safety_gymnasium_env.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    22219 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/safety_gymnasium_modelbased.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    21885 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/wrapper.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    20370 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/evaluator.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.113279 omnisafe-0.4.0/omnisafe/models/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1507 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.114057 omnisafe-0.4.0/omnisafe/models/actor/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1088 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4165 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/actor_builder.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1412 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/gaussian_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5276 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/gaussian_learning_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6513 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/gaussian_sac_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4490 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/mlp_actor.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.114733 omnisafe-0.4.0/omnisafe/models/actor_critic/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1035 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7170 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/actor_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6979 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/actor_q_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5182 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/constraint_actor_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4427 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/constraint_actor_q_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8344 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/base.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.115290 omnisafe-0.4.0/omnisafe/models/critic/
+-rw-r--r--   0 jiaming    (501) staff       (20)      935 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4449 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/critic_builder.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5432 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/q_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3204 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/v_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1686 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/typing.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.116719 omnisafe-0.4.0/omnisafe/utils/
+-rw-r--r--   0 jiaming    (501) staff       (20)      723 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    16911 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/utils/command_app.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    15464 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/config.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    11428 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/distributed.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3249 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/utils/exp_grid_tools.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7309 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/math.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4027 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/model.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    16365 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/plotter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3833 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/schedule.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    12015 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/tools.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1831 2023-05-08 20:07:12.000000 omnisafe-0.4.0/omnisafe/version.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.095523 omnisafe-0.4.0/omnisafe.egg-info/
+-rw-r--r--   0 jiaming    (501) staff       (20)    17209 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/PKG-INFO
+-rw-r--r--   0 jiaming    (501) staff       (20)     6816 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)        1 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)       60 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/entry_points.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)      379 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/requires.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)        9 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/top_level.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)     5318 2023-05-08 19:46:32.000000 omnisafe-0.4.0/pyproject.toml
+-rw-r--r--   0 jiaming    (501) staff       (20)       38 2023-05-08 20:07:23.118550 omnisafe-0.4.0/setup.cfg
+-rw-r--r--   0 jiaming    (501) staff       (20)      988 2023-05-08 19:46:32.000000 omnisafe-0.4.0/setup.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.118090 omnisafe-0.4.0/tests/
+-rw-r--r--   0 jiaming    (501) staff       (20)    15876 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2799 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_cli.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4480 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_env.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3325 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_experiment_grid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7114 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_model.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1564 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_normalizer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    19763 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_policy.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1045 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_registry.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1478 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_statistics_tools.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6008 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_utils.py
```

### Comparing `omnisafe-0.3.0/LICENSE` & `omnisafe-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/PKG-INFO` & `omnisafe-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,48 @@
-Metadata-Version: 2.1
-Name: omnisafe
-Version: 0.3.0
-Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
-Home-page: https://github.com/PKU-MARL/omnisafe
-Author: OmniSafe Contributors
-Author-email: jiamg.ji@gmail.com
-License: Apache License, Version 2.0
-Project-URL: Homepage, https://github.com/PKU-MARL/omnisafe
-Project-URL: Repository, https://github.com/PKU-MARL/omnisafe
-Project-URL: Documentation, https://omnisafe.readthedocs.io
-Project-URL: Bug Report, https://github.com/PKU-MARL/omnisafe/issues
-Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: lint
-Provides-Extra: test
-License-File: LICENSE
-
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
-  <img src="https://github.com/PKU-MARL/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
+  <img src="https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
 
 <div align="center">
 
-  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/PKU-MARL)
+  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/OmniSafeAI)
   [![PyPI](https://img.shields.io/pypi/v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe)
+  [![tests](https://img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/HEAD/tests)
   [![Documentation Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io)
   [![Downloads](https://static.pepy.tech/personalized-badge/omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/omnisafe)
-  [![GitHub Repo Stars](https://img.shields.io/github/stars/PKU-MARL/omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-MARL/OmniSafe/stargazers)
+  [![GitHub Repo Stars](https://img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)](https://github.com/OmniSafeAI/OmniSafe/stargazers)
   [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-  [![License](https://img.shields.io/github/license/PKU-MARL/OmniSafe?label=license)](#license)
-  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-MARL/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-MARL/omnisafe)
+  [![License](https://img.shields.io/github/license/OmniSafeAI/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/OmniSafeAI/omnisafe)
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/omnisafe/)
 
 </div>
 
 <p align="center">
   <a href="https://omnisafe.readthedocs.io">Documentation</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#installation">Installation</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#getting-started">Getting Started</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#license">License</a>
+  <a href="https://github.com/OmniSafeAI/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#installation">Installation</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#getting-started">Getting Started</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#license">License</a>
 </p>
 
 --------------------------------------------------------------------------------
 
 **This library is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open a GitHub issue or reach out. We'd love to hear about how you're using the library.**
 
-OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms. The field of RL has great potential to benefit society, but safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior. Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
-
-OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment. Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms. By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
+OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms.
+The field of RL has great potential to benefit the society, and safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior.
+Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
+
+OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment.
+Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms.
+By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
 
 --------------------------------------------------------------------------------
 
 ### Table of Contents  <!-- omit in toc --> <!-- markdownlint-disable heading-increment -->
 
 - [Implemented Algorithms](#implemented-algorithms)
   - [Latest SafeRL Papers](#latest-saferl-papers)
@@ -78,19 +55,16 @@
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
   - [Examples](#examples)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
-    - [Important Hints](#important-hints)
-  - [1. Run Agent from preset yaml file](#1-run-agent-from-preset-yaml-file)
-  - [2. Run agent with custom cfg](#2-run-agent-with-custom-cfg)
-  - [3. Run Agent from custom terminal config](#3-run-agent-from-custom-terminal-config)
-  - [4. Evaluate Saved Policy](#4-evaluate-saved-policy)
+  - [Important Hints](#important-hints)
+  - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
 ## Implemented Algorithms
@@ -136,14 +110,16 @@
 #### Model-Based Safe
 
 - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789)
 - [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
 - [X] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
 - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - [ ] **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
+- [X] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
+- [X] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
 
 #### Offline Safe
 
 - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
 - [X] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
 - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003)
 - [ ] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
@@ -160,59 +136,60 @@
 
 ## Installation
 
 ### Prerequisites
 
 OmniSafe requires Python 3.8+ and PyTorch 1.10+.
 
+> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
+
 #### Install from source
 
 ```bash
 # Clone the repo
-git clone https://github.com/PKU-MARL/omnisafe
+git clone https://github.com/OmniSafeAI/omnisafe
 cd omnisafe
 
 # Create a conda environment
-conda create -n omnisafe python=3.8
+conda env create --file conda-recipe.yaml
 conda activate omnisafe
 
 # Install omnisafe
 pip install -e .
 ```
 
 #### Install from PyPI
+
 OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+
 ```bash
 pip install omnisafe
 ```
 
-
 ### Examples
 
 ```bash
 cd examples
 python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
 ```
 
-
 **algo:**
 | Type              | Name                                                             |
 | ----------------- | ---------------------------------------------------------------- |
 | `Base-On-Policy`  | `PolicyGradient, PPO`<br> `NaturalPG, TRPO`                      |
 | `Base-Off-Policy` | `DDPG, TD3, SAC`                                                 |
 | `Naive Lagrange`  | `RCPO, PPOLag, TRPOLag`<br> `DDPGLag, TD3Lag, SACLag`            |
 | `PID Lagrange`    | `CPPOPid, TRPOPid`                                               |
 | `First Order`     | `FOCOPS, CUP`                                                    |
 | `Second Order`    | `SDDPG, CPO, PCPO`                                               |
 | `Saute RL`        | `PPOSaute, PPOLagSaute`                                          |
 | `Simmer RL`       | `PPOSimmerQ, PPOSimmerPid` <br> `PPOLagSimmerQ, PPOLagSimmerPid` |
 | `EarlyTerminated` | `PPOEarlyTerminated` <br> `PPOLagEarlyTerminated`                |
 | `Model-Based`     | `CAP, MBPPOLag, SafeLOOP`                                        |
 
-
 **env-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/), here a list of envs that safety-gymnasium supports.
 
 <table border="1">
 <thead>
   <tr>
     <th>Category</th>
     <th>Task</th>
@@ -236,29 +213,28 @@
   <tr>
     <td>Circle[012]</td>
   </tr>
   <tr>
     <td>Safe Velocity</td>
     <td>Velocity</td>
     <td>HalfCheetah, Hopper, Swimmer, Walker2d, Ant, Humanoid</td>
-    <td>SafetyHumanoidVelocity-v4</td>
+    <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
 More information about environments, please refer to [Safety Gymnasium](https://www.safety-gymnasium.com/)
 
 **parallel:** `Number of parallels`
 
-
 #### Try with CLI
 
 **A video example**
 
-![Segmentfault](https://github.com/PKU-MARL/omnisafe/blob/main/images/CLI_example.svg)
+![Segmentfault](https://github.com/OmniSafeAI/omnisafe/blob/main/images/CLI_example.svg)
 
 ```bash
 pip install omnisafe
 
 omnisafe --help # Ask for help
 
 omnisafe benchmark --help # The benchmark also can be replaced with 'eval', 'train', 'train-config'
@@ -267,94 +243,47 @@
 omnisafe benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml
 
 # Quick evaluating and rendering your trained policy, just specify: 1.path of algorithm which you trained
 omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
 
 # Quick training some algorithms to validate your thoughts
 # Note: use `key1:key2`, your can select key of hyperparameters which are recursively contained, and use `--custom-cfgs`, you can add custom cfgs via CLI
-omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:update_cycle --custom-cfgs 1024
+omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024
 
 # Quick training some algorithms via a saved config file, the format is as same as default format
 omnisafe train-config ./saved_source/train_config.yaml
 ```
 
-
 --------------------------------------------------------------------------------
 
 ## Getting Started
-#### Important Hints
-- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
-### 1. Run Agent from preset yaml file
 
-```python
-import omnisafe
+### Important Hints
 
-env_id = 'SafetyPointGoal1-v0'
-agent = omnisafe.Agent('PPOLag', env_id)
-agent.learn()
-```
-
-### 2. Run agent with custom cfg
-```python
-import omnisafe
-
-env_id = 'SafetyPointGoal1-v0'
-custom_cfgs = {
-    'train_cfgs': {
-        'total_steps': 1024000,
-        'vector_env_nums': 1,
-        'parallel': 1,
-    },
-    'algo_cfgs': {
-        'update_cycle': 2048,
-        'update_iters': 1,
-    },
-    'logger_cfgs': {
-        'use_wandb': False,
-    },
-}
-agent = omnisafe.Agent('PPOLag', env_id, custom_cfgs=custom_cfgs)
-agent.learn()
-```
-
-### 3. Run Agent from custom terminal config
-
-You can also run agent from a custom terminal config. You can set any config in a corresponding yaml file.
-
-For example, you can run `PPOLag` agent on `SafetyPointGoal1-v0` environment with `total_steps=1024000`, `vector_env_nums=1` and `parallel=1` by:
-
-```bash
-cd examples
-python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
-```
-
-### 4. Evaluate Saved Policy
-
-```python
-import os
+- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
 
-import omnisafe
+### Quickstart: Colab on the Cloud
 
+Explore OmniSafe easily and quickly through a series of colab notebooks:
 
-# Just fill your experiment's log directory in here.
-# Such as: ~/omnisafe/runs/SafetyPointGoal1-v0/CPO/seed-000-2022-12-25_14-45-05
-LOG_DIR = ''
+- [Getting Started](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand on it.
+- [CLI Command](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
 
-evaluator = omnisafe.Evaluator()
-for item in os.scandir(os.path.join(LOG_DIR, 'torch_save')):
-    if item.is_file() and item.name.split('.')[-1] == 'pt':
-        evaluator.load_saved_model(save_dir=LOG_DIR, model_name=item.name)
-        evaluator.render(num_episode=10, camera_name='track', width=256, height=256)
-```
+We take great pleasure in collaborating with our users to create tutorials in various languages.
+Please refer to our list of currently supported languages.
+If you are interested in translating the tutorial into a new language or improving an existing version, kindly submit a PR to us.
 
 --------------------------------------------------------------------------------
 
 ## Changelog
-See [CHANGELOG.md](https://github.com/PKU-MARL/omnisafe/blob/main/CHANGELOG.md).
+
+See [CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
 
 ## The OmniSafe Team
 
-OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/PKU-MARL/people/PKU-YYang). Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-MARL/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
+OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-YYang).
+Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
+If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
 
 OmniSafe is released under Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,154 +1,146 @@
-Metadata-Version: 2.1 Name: omnisafe Version: 0.3.0 Summary: A comprehensive
-and reliable benchmark for safe reinforcement learning. Home-page: https://
-github.com/PKU-MARL/omnisafe Author: OmniSafe Contributors Author-email:
-jiamg.ji@gmail.com License: Apache License, Version 2.0 Project-URL: Homepage,
-https://github.com/PKU-MARL/omnisafe Project-URL: Repository, https://
-github.com/PKU-MARL/omnisafe Project-URL: Documentation, https://
-omnisafe.readthedocs.io Project-URL: Bug Report, https://github.com/PKU-MARL/
-omnisafe/issues Keywords: Safe Reinforcement Learning,Reinforcement
-Learning,PyTorch Classifier: Development Status :: 4 - Beta Classifier: License
-:: OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: lint Provides-Extra: test License-
-File: LICENSE
-        [https://github.com/PKU-MARL/omnisafe/raw/HEAD/images/logo.png]
+
+       [https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png]
 [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)]
-     (https://github.com/PKU-MARL) [![PyPI](https://img.shields.io/pypi/v/
-   omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![Documentation
-Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://
- omnisafe.readthedocs.io) [![Downloads](https://static.pepy.tech/personalized-
-                                    badge/
+    (https://github.com/OmniSafeAI) [![PyPI](https://img.shields.io/pypi/v/
+  omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
+      img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/
+test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/
+   HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
+  omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io) [![Downloads]
+                 (https://static.pepy.tech/personalized-badge/
  omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)]
       (https://pepy.tech/project/omnisafe) [![GitHub Repo Stars](https://
- img.shields.io/github/stars/PKU-MARL/omnisafe?color=brightgreen&logo=github)]
-   (https://github.com/PKU-MARL/OmniSafe/stargazers) [![codestyle](https://
+img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)]
+  (https://github.com/OmniSafeAI/OmniSafe/stargazers) [![codestyle](https://
  img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-      black) [![License](https://img.shields.io/github/license/PKU-MARL/
+     black) [![License](https://img.shields.io/github/license/OmniSafeAI/
 OmniSafe?label=license)](#license) [![CodeCov](https://img.shields.io/codecov/
- c/github/PKU-MARL/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-
-                                MARL/omnisafe)
+  c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/
+   OmniSafeAI/omnisafe) [![Open In Colab](https://colab.research.google.com/
+ assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/
+                                  omnisafe/)
    Documentation | Implemented_Algorithms | Installation | Getting_Started |
                                     License
 -------------------------------------------------------------------------------
 - **This library is currently under heavy development - if you have suggestions
 on the API or use-cases you'd like to be covered, please open a GitHub issue or
 reach out. We'd love to hear about how you're using the library.** OmniSafe is
 an infrastructural framework designed to accelerate safe reinforcement learning
 (RL) research by providing a comprehensive and reliable benchmark for safe RL
-algorithms. The field of RL has great potential to benefit society, but safety
-concerns are a significant issue, and RL algorithms have raised concerns about
-unintended harm or unsafe behavior. Safe RL intends to develop algorithms that
-minimize the risk of unintended harm or unsafe behavior, but there is currently
-a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe addresses
-these issues by providing more than 40 experimentally validated algorithms and
-a sound and efficient simulation environment. Researchers can use OmniSafe to
-conduct experiments and verify their ideas, ensuring consistency and enabling
-more efficient development of safe RL algorithms. By using OmniSafe as a
-benchmark, researchers can evaluate the performance of their own safe RL
-algorithms and contribute to the advancement of safe RL research. -------------
-------------------------------------------------------------------- ### Table
-of Contents   - [Implemented Algorithms](#implemented-algorithms) - [Latest
-SafeRL Papers](#latest-saferl-papers) - [List of Algorithms](#list-of-
-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-Policy Safe](#off-
-policy-safe) - [Model-Based Safe](#model-based-safe) - [Offline Safe](#offline-
-safe) - [Others](#others) - [Installation](#installation) - [Prerequisites]
-(#prerequisites) - [Install from source](#install-from-source) - [Install from
-PyPI](#install-from-pypi) - [Examples](#examples) - [Try with CLI](#try-with-
-cli) - [Getting Started](#getting-started) - [Important Hints](#important-
-hints) - [1. Run Agent from preset yaml file](#1-run-agent-from-preset-yaml-
-file) - [2. Run agent with custom cfg](#2-run-agent-with-custom-cfg) - [3. Run
-Agent from custom terminal config](#3-run-agent-from-custom-terminal-config) -
-[4. Evaluate Saved Policy](#4-evaluate-saved-policy) - [Changelog](#changelog)
-- [The OmniSafe Team](#the-omnisafe-team) - [License](#license) ---------------
------------------------------------------------------------------ ##
-Implemented Algorithms The supported interface algorithms currently include:
-### Latest SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy
-Optimization for Safe Reinforcement Learning (APPO) - **[NeurIPS 2022]**
-[Constrained Update Projection Approach to Safe Policy Optimization (CUP)]
-(https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]** [Effects of Safety
-State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/
-2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning
-via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/
-abs/2210.07573) - **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
-Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- **[ICML 2022]** [Constrained Variational Policy Optimization for Safe
-Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) - **[IJCAI
-2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement
-Learning](https://arxiv.org/abs/2205.11814) - **[ICLR 2022]** [Constrained
-Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) ###
-List of Algorithms #### On-Policy Safe - [X] [The Lagrange version of PPO (PPO-
-Lag)](https://cdn.openai.com/safexp-short.pdf) - [X] [The Lagrange version of
-TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]**
-[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
-achiam17a) - [X] **[ICLR 2019]** [Reward Constrained Policy Optimization
-(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [X] **[ICML 2020]**
-[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
-Lag)](https://arxiv.org/abs/2007.03964) - [X] **[NeurIPS 2020]** [First Order
-Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
-2002.06506) - [X] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
-under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [X] **[ICLR
-2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
-openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML 2021]** [CRPO: A New Approach
-for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
-abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
-for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf)
-#### Off-Policy Safe - [X] The Lagrange version of TD3 (TD3-Lag) - [X] The
-Lagrange version of DDPG (DDPG-Lag) - [X] The Lagrange version of SAC (SAC-Lag)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous
-Control (SDDPG)](https://arxiv.org/abs/1901.10031) - [X] **[ICML 2019]**
-[Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG-
-modular)](https://arxiv.org/abs/1901.10031) - [ ] **[ICML 2022]** [Constrained
+algorithms. The field of RL has great potential to benefit the society, and
+safety concerns are a significant issue, and RL algorithms have raised concerns
+about unintended harm or unsafe behavior. Safe RL intends to develop algorithms
+that minimize the risk of unintended harm or unsafe behavior, but there is
+currently a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe
+addresses these issues by providing more than 40 experimentally validated
+algorithms and a sound and efficient simulation environment. Researchers can
+use OmniSafe to conduct experiments and verify their ideas, ensuring
+consistency and enabling more efficient development of safe RL algorithms. By
+using OmniSafe as a benchmark, researchers can evaluate the performance of
+their own safe RL algorithms and contribute to the advancement of safe RL
+research. ---------------------------------------------------------------------
+----------- ### Table of Contents   - [Implemented Algorithms](#implemented-
+algorithms) - [Latest SafeRL Papers](#latest-saferl-papers) - [List of
+Algorithms](#list-of-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-
+Policy Safe](#off-policy-safe) - [Model-Based Safe](#model-based-safe) -
+[Offline Safe](#offline-safe) - [Others](#others) - [Installation]
+(#installation) - [Prerequisites](#prerequisites) - [Install from source]
+(#install-from-source) - [Install from PyPI](#install-from-pypi) - [Examples]
+(#examples) - [Try with CLI](#try-with-cli) - [Getting Started](#getting-
+started) - [Important Hints](#important-hints) - [Quickstart: Colab on the
+Cloud](#quickstart-colab-on-the-cloud) - [Changelog](#changelog) - [The
+OmniSafe Team](#the-omnisafe-team) - [License](#license) ----------------------
+---------------------------------------------------------- ## Implemented
+Algorithms The supported interface algorithms currently include: ### Latest
+SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe
+Reinforcement Learning (APPO) - **[NeurIPS 2022]** [Constrained Update
+Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/
+2209.07089) - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
+Exploration (Simmer)](https://arxiv.org/abs/2206.02675) - **[NeurIPS 2022]**
+[Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy
+Optimization Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]**
+[SautÃ© RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
+(SauteRL)](https://arxiv.org/abs/2202.06558) - **[ICML 2022]** [Constrained
 Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https:/
-/arxiv.org/abs/2201.11927) #### Model-Based Safe - [ ] **[NeurIPS 2021]** [Safe
-Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
-abs/2202.07789) - [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
-Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]**
-[Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
-(CAP)](https://arxiv.org/abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based
-Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
-Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
-Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) #### Offline Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)]
-(https://arxiv.org/abs/1812.02900) - [X] [The Constrained version of CRR (C-
-CRR)](https://proceedings.neurips.cc/paper/2020/hash/
-588cb956d6bbe67078f29f8de420a13d-Abstract.html) - [ ] **[AAAI 2022]**
-[Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ]
-(https://arxiv.org/abs/2107.09003) - [ ] **[ICLR 2022 (Spotlight)]**
-[COptiDICE: Offline Constrained Reinforcement Learning via Stationary
-Distribution Correction Estimation](https://arxiv.org/abs/
-2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
+/arxiv.org/abs/2201.11927) - **[IJCAI 2022]** [Penalized Proximal Policy
+Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
+- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models
+(LA-MBDA)](https://arxiv.org/abs/2201.09802) - **[AAAI 2022]** [Conservative
+and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https:/
+/arxiv.org/abs/2112.07701) ### List of Algorithms #### On-Policy Safe - [X]
+[The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
+short.pdf) - [X] [The Lagrange version of TRPO (TRPO-Lag)](https://
+cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]** [Constrained Policy
+Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [X] **[ICLR
+2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
+forum?id=SkfrvsA9FX) - [X] **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
+(FOCOPS)](https://arxiv.org/abs/2002.06506) - [X] **[AAAI 2020]** [IPO:
+Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
+abs/1910.09615) - [X] **[ICLR 2020]** [Projection-Based Constrained Policy
+Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML
+2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
+Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
+Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
+arxiv.org/pdf/2205.11814.pdf) #### Off-Policy Safe - [X] The Lagrange version
+of TD3 (TD3-Lag) - [X] The Lagrange version of DDPG (DDPG-Lag) - [X] The
+Lagrange version of SAC (SAC-Lag) - [X] **[ICML 2019]** [Lyapunov-based Safe
+Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/
+1901.10031) - [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for
+Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031) - [ ] **
+[ICML 2022]** [Constrained Variational Policy Optimization for Safe
+Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) #### Model-
+Based Safe - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining
+the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [X] **[CoRL 2021
+(Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://
+arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]** [Conservative and Adaptive
+Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/
+abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement
+Learning via a Constrained Proximal Policy Optimization Algorithm](https://
+arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained Policy
+Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
+2201.09802) - [X] **[ICML 2022 Workshop]** [Constrained Model-based
+Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
+arxiv.org/abs/2010.07968) - [X] **[NeurIPS 2018]** [Constrained Cross-Entropy
+Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
+paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) #### Offline
+Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/
+1812.02900) - [X] [The Constrained version of CRR (C-CRR)](https://
+proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-
+Abstract.html) - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe
+Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003) - [ ] **
+[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement
+Learning via Stationary Distribution Correction Estimation](https://arxiv.org/
+abs/2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
 Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) ####
 Others - [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)]
 (https://arxiv.org/abs/1801.08757) - [ ] **[RA-L 2021]** [Recovery RL: Safe
 Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/
 2010.15920) - [X] **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
 Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
 - [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
 Exploration](https://arxiv.org/abs/2206.02675) --------------------------------
 ------------------------------------------------ ## Installation ###
-Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. #### Install
-from source ```bash # Clone the repo git clone https://github.com/PKU-MARL/
-omnisafe cd omnisafe # Create a conda environment conda create -n omnisafe
-python=3.8 conda activate omnisafe # Install omnisafe pip install -e . ``` ####
-Install from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
-omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
-(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
-omnisafe ``` ### Examples ```bash cd examples python train_policy.py --algo
-PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device
-cpu --vector-env-nums 1 --torch-threads 1 ``` **algo:** | Type | Name | | -----
------------- | ---------------------------------------------------------------
-- | | `Base-On-Policy` | `PolicyGradient, PPO`
+Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
+test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
+versions of macOS. We will accept PRs related to Windows, but do not officially
+support it. #### Install from source ```bash # Clone the repo git clone https:/
+/github.com/OmniSafeAI/omnisafe cd omnisafe # Create a conda environment conda
+env create --file conda-recipe.yaml conda activate omnisafe # Install omnisafe
+pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [![PyPI]
+(https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
+pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
+omnisafe?label=status). ```bash pip install omnisafe ``` ### Examples ```bash
+cd examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 -
+-parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
+threads 1 ``` **algo:** | Type | Name | | ----------------- | -----------------
+----------------------------------------------- | | `Base-On-Policy` |
+`PolicyGradient, PPO`
 `NaturalPG, TRPO` | | `Base-Off-Policy` | `DDPG, TD3, SAC` | | `Naive Lagrange`
 | `RCPO, PPOLag, TRPOLag`
 `DDPGLag, TD3Lag, SACLag` | | `PID Lagrange` | `CPPOPid, TRPOPid` | | `First
 Order` | `FOCOPS, CUP` | | `Second Order` | `SDDPG, CPO, PCPO` | | `Saute RL` |
 `PPOSaute, PPOLagSaute` | | `Simmer RL` | `PPOSimmerQ, PPOSimmerPid`
 `PPOLagSimmerQ, PPOLagSimmerPid` | | `EarlyTerminated` | `PPOEarlyTerminated`
 `PPOLagEarlyTerminated` | | `Model-Based` | `CAP, MBPPOLag, SafeLOOP` | **env-
@@ -157,63 +149,54 @@
  ____________________________________________________________________________
 |Category_______|Task_______|Agent___________________|Example________________|
 |               |Goal[012]__|                        |                       |
 |Safe Navigation|Button[012]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |Push[012]__|                        |                       |
 |_______________|Circle[012]|________________________|_______________________|
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
-|Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v4                     |
+|Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_______________|___________|Humanoid________________|_______________________|
 More information about environments, please refer to [Safety Gymnasium](https:/
 /www.safety-gymnasium.com/) **parallel:** `Number of parallels` #### Try with
-CLI **A video example** ![Segmentfault](https://github.com/PKU-MARL/omnisafe/
+CLI **A video example** ![Segmentfault](https://github.com/OmniSafeAI/omnisafe/
 blob/main/images/CLI_example.svg) ```bash pip install omnisafe omnisafe --help
 # Ask for help omnisafe benchmark --help # The benchmark also can be replaced
 with 'eval', 'train', 'train-config' # Quick benchmarking for your research,
 just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path
 of the config file(refer to omnisafe/examples/benchmarks for format) omnisafe
 benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml # Quick
 evaluating and rendering your trained policy, just specify: 1.path of algorithm
 which you trained omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-
 episode 1 # Quick training some algorithms to validate your thoughts # Note:
 use `key1:key2`, your can select key of hyperparameters which are recursively
 contained, and use `--custom-cfgs`, you can add custom cfgs via CLI omnisafe
 train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs
-algo_cfgs:update_cycle --custom-cfgs 1024 # Quick training some algorithms via
-a saved config file, the format is as same as default format omnisafe train-
-config ./saved_source/train_config.yaml ``` -----------------------------------
---------------------------------------------- ## Getting Started #### Important
-Hints - `train_cfgs:torch_threads` is especially important for training speed,
-and is varying with users' machine, this value shouldn't be too small or too
-large. ### 1. Run Agent from preset yaml file ```python import omnisafe env_id
-= 'SafetyPointGoal1-v0' agent = omnisafe.Agent('PPOLag', env_id) agent.learn()
-``` ### 2. Run agent with custom cfg ```python import omnisafe env_id =
-'SafetyPointGoal1-v0' custom_cfgs = { 'train_cfgs': { 'total_steps': 1024000,
-'vector_env_nums': 1, 'parallel': 1, }, 'algo_cfgs': { 'update_cycle': 2048,
-'update_iters': 1, }, 'logger_cfgs': { 'use_wandb': False, }, } agent =
-omnisafe.Agent('PPOLag', env_id, custom_cfgs=custom_cfgs) agent.learn() ``` ###
-3. Run Agent from custom terminal config You can also run agent from a custom
-terminal config. You can set any config in a corresponding yaml file. For
-example, you can run `PPOLag` agent on `SafetyPointGoal1-v0` environment with
-`total_steps=1024000`, `vector_env_nums=1` and `parallel=1` by: ```bash cd
-examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --
-parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
-threads 1 ``` ### 4. Evaluate Saved Policy ```python import os import omnisafe
-# Just fill your experiment's log directory in here. # Such as: ~/omnisafe/
-runs/SafetyPointGoal1-v0/CPO/seed-000-2022-12-25_14-45-05 LOG_DIR = ''
-evaluator = omnisafe.Evaluator() for item in os.scandir(os.path.join(LOG_DIR,
-'torch_save')): if item.is_file() and item.name.split('.')[-1] == 'pt':
-evaluator.load_saved_model(save_dir=LOG_DIR, model_name=item.name)
-evaluator.render(num_episode=10, camera_name='track', width=256, height=256)
-``` ---------------------------------------------------------------------------
------ ## Changelog See [CHANGELOG.md](https://github.com/PKU-MARL/omnisafe/
-blob/main/CHANGELOG.md). ## The OmniSafe Team OmniSafe is mainly developed by
-the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/
-orgs/PKU-MARL/people/PKU-YYang). Our SafeRL research team members include
-[Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/
-Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://
-github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai
-Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-
-2077). If you have any questions in the process of using omnisafe, don't
-hesitate to ask your questions on [the GitHub issue page](https://github.com/
-PKU-MARL/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
-## License OmniSafe is released under Apache License 2.0.
+algo_cfgs:steps_per_epoch --custom-cfgs 1024 # Quick training some algorithms
+via a saved config file, the format is as same as default format omnisafe
+train-config ./saved_source/train_config.yaml ``` -----------------------------
+--------------------------------------------------- ## Getting Started ###
+Important Hints - `train_cfgs:torch_threads` is especially important for
+training speed, and is varying with users' machine, this value shouldn't be too
+small or too large. ### Quickstart: Colab on the Cloud Explore OmniSafe easily
+and quickly through a series of colab notebooks: - [Getting Started](https://
+colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that
+users can quickly hand on it. - [CLI Command](https://
+colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
+take great pleasure in collaborating with our users to create tutorials in
+various languages. Please refer to our list of currently supported languages.
+If you are interested in translating the tutorial into a new language or
+improving an existing version, kindly submit a PR to us. ----------------------
+---------------------------------------------------------- ## Changelog See
+[CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
+## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research team
+directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-
+YYang). Our SafeRL research team members include [Borong Zhang](https://
+github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https:/
+/github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang
+Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/
+XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any
+questions in the process of using omnisafe, don't hesitate to ask your
+questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/
+issues/new/choose), we will reply to you in 2-3 working days. ## License
+OmniSafe is released under Apache License 2.0.
```

### Comparing `omnisafe-0.3.0/README.md` & `omnisafe-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,75 @@
+Metadata-Version: 2.1
+Name: omnisafe
+Version: 0.4.0
+Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
+Author: OmniSafe Contributors
+License: Apache License, Version 2.0
+Project-URL: Homepage, https://github.com/OmniSafeAI/omnisafe
+Project-URL: Repository, https://github.com/OmniSafeAI/omnisafe
+Project-URL: Documentation, https://omnisafe.readthedocs.io
+Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
+Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
+License-File: LICENSE
+
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
-  <img src="https://github.com/PKU-MARL/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
+  <img src="https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
 
 <div align="center">
 
-  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/PKU-MARL)
+  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/OmniSafeAI)
   [![PyPI](https://img.shields.io/pypi/v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe)
+  [![tests](https://img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/HEAD/tests)
   [![Documentation Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io)
   [![Downloads](https://static.pepy.tech/personalized-badge/omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/omnisafe)
-  [![GitHub Repo Stars](https://img.shields.io/github/stars/PKU-MARL/omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-MARL/OmniSafe/stargazers)
+  [![GitHub Repo Stars](https://img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)](https://github.com/OmniSafeAI/OmniSafe/stargazers)
   [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-  [![License](https://img.shields.io/github/license/PKU-MARL/OmniSafe?label=license)](#license)
-  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-MARL/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-MARL/omnisafe)
+  [![License](https://img.shields.io/github/license/OmniSafeAI/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/OmniSafeAI/omnisafe)
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/omnisafe/)
 
 </div>
 
 <p align="center">
   <a href="https://omnisafe.readthedocs.io">Documentation</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#installation">Installation</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#getting-started">Getting Started</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#license">License</a>
+  <a href="https://github.com/OmniSafeAI/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#installation">Installation</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#getting-started">Getting Started</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#license">License</a>
 </p>
 
 --------------------------------------------------------------------------------
 
 **This library is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open a GitHub issue or reach out. We'd love to hear about how you're using the library.**
 
-OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms. The field of RL has great potential to benefit society, but safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior. Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
-
-OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment. Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms. By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
+OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms.
+The field of RL has great potential to benefit the society, and safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior.
+Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
+
+OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment.
+Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms.
+By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
 
 --------------------------------------------------------------------------------
 
 ### Table of Contents  <!-- omit in toc --> <!-- markdownlint-disable heading-increment -->
 
 - [Implemented Algorithms](#implemented-algorithms)
   - [Latest SafeRL Papers](#latest-saferl-papers)
@@ -49,19 +82,16 @@
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
   - [Examples](#examples)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
-    - [Important Hints](#important-hints)
-  - [1. Run Agent from preset yaml file](#1-run-agent-from-preset-yaml-file)
-  - [2. Run agent with custom cfg](#2-run-agent-with-custom-cfg)
-  - [3. Run Agent from custom terminal config](#3-run-agent-from-custom-terminal-config)
-  - [4. Evaluate Saved Policy](#4-evaluate-saved-policy)
+  - [Important Hints](#important-hints)
+  - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
 ## Implemented Algorithms
@@ -107,14 +137,16 @@
 #### Model-Based Safe
 
 - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789)
 - [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
 - [X] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
 - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - [ ] **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
+- [X] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
+- [X] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
 
 #### Offline Safe
 
 - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
 - [X] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
 - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003)
 - [ ] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
@@ -131,59 +163,60 @@
 
 ## Installation
 
 ### Prerequisites
 
 OmniSafe requires Python 3.8+ and PyTorch 1.10+.
 
+> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
+
 #### Install from source
 
 ```bash
 # Clone the repo
-git clone https://github.com/PKU-MARL/omnisafe
+git clone https://github.com/OmniSafeAI/omnisafe
 cd omnisafe
 
 # Create a conda environment
-conda create -n omnisafe python=3.8
+conda env create --file conda-recipe.yaml
 conda activate omnisafe
 
 # Install omnisafe
 pip install -e .
 ```
 
 #### Install from PyPI
+
 OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+
 ```bash
 pip install omnisafe
 ```
 
-
 ### Examples
 
 ```bash
 cd examples
 python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
 ```
 
-
 **algo:**
 | Type              | Name                                                             |
 | ----------------- | ---------------------------------------------------------------- |
 | `Base-On-Policy`  | `PolicyGradient, PPO`<br> `NaturalPG, TRPO`                      |
 | `Base-Off-Policy` | `DDPG, TD3, SAC`                                                 |
 | `Naive Lagrange`  | `RCPO, PPOLag, TRPOLag`<br> `DDPGLag, TD3Lag, SACLag`            |
 | `PID Lagrange`    | `CPPOPid, TRPOPid`                                               |
 | `First Order`     | `FOCOPS, CUP`                                                    |
 | `Second Order`    | `SDDPG, CPO, PCPO`                                               |
 | `Saute RL`        | `PPOSaute, PPOLagSaute`                                          |
 | `Simmer RL`       | `PPOSimmerQ, PPOSimmerPid` <br> `PPOLagSimmerQ, PPOLagSimmerPid` |
 | `EarlyTerminated` | `PPOEarlyTerminated` <br> `PPOLagEarlyTerminated`                |
 | `Model-Based`     | `CAP, MBPPOLag, SafeLOOP`                                        |
 
-
 **env-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/), here a list of envs that safety-gymnasium supports.
 
 <table border="1">
 <thead>
   <tr>
     <th>Category</th>
     <th>Task</th>
@@ -207,29 +240,28 @@
   <tr>
     <td>Circle[012]</td>
   </tr>
   <tr>
     <td>Safe Velocity</td>
     <td>Velocity</td>
     <td>HalfCheetah, Hopper, Swimmer, Walker2d, Ant, Humanoid</td>
-    <td>SafetyHumanoidVelocity-v4</td>
+    <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
 More information about environments, please refer to [Safety Gymnasium](https://www.safety-gymnasium.com/)
 
 **parallel:** `Number of parallels`
 
-
 #### Try with CLI
 
 **A video example**
 
-![Segmentfault](https://github.com/PKU-MARL/omnisafe/blob/main/images/CLI_example.svg)
+![Segmentfault](https://github.com/OmniSafeAI/omnisafe/blob/main/images/CLI_example.svg)
 
 ```bash
 pip install omnisafe
 
 omnisafe --help # Ask for help
 
 omnisafe benchmark --help # The benchmark also can be replaced with 'eval', 'train', 'train-config'
@@ -238,94 +270,47 @@
 omnisafe benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml
 
 # Quick evaluating and rendering your trained policy, just specify: 1.path of algorithm which you trained
 omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
 
 # Quick training some algorithms to validate your thoughts
 # Note: use `key1:key2`, your can select key of hyperparameters which are recursively contained, and use `--custom-cfgs`, you can add custom cfgs via CLI
-omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:update_cycle --custom-cfgs 1024
+omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024
 
 # Quick training some algorithms via a saved config file, the format is as same as default format
 omnisafe train-config ./saved_source/train_config.yaml
 ```
 
-
 --------------------------------------------------------------------------------
 
 ## Getting Started
-#### Important Hints
-- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
-### 1. Run Agent from preset yaml file
 
-```python
-import omnisafe
+### Important Hints
 
-env_id = 'SafetyPointGoal1-v0'
-agent = omnisafe.Agent('PPOLag', env_id)
-agent.learn()
-```
-
-### 2. Run agent with custom cfg
-```python
-import omnisafe
-
-env_id = 'SafetyPointGoal1-v0'
-custom_cfgs = {
-    'train_cfgs': {
-        'total_steps': 1024000,
-        'vector_env_nums': 1,
-        'parallel': 1,
-    },
-    'algo_cfgs': {
-        'update_cycle': 2048,
-        'update_iters': 1,
-    },
-    'logger_cfgs': {
-        'use_wandb': False,
-    },
-}
-agent = omnisafe.Agent('PPOLag', env_id, custom_cfgs=custom_cfgs)
-agent.learn()
-```
-
-### 3. Run Agent from custom terminal config
-
-You can also run agent from a custom terminal config. You can set any config in a corresponding yaml file.
-
-For example, you can run `PPOLag` agent on `SafetyPointGoal1-v0` environment with `total_steps=1024000`, `vector_env_nums=1` and `parallel=1` by:
-
-```bash
-cd examples
-python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
-```
-
-### 4. Evaluate Saved Policy
-
-```python
-import os
+- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
 
-import omnisafe
+### Quickstart: Colab on the Cloud
 
+Explore OmniSafe easily and quickly through a series of colab notebooks:
 
-# Just fill your experiment's log directory in here.
-# Such as: ~/omnisafe/runs/SafetyPointGoal1-v0/CPO/seed-000-2022-12-25_14-45-05
-LOG_DIR = ''
+- [Getting Started](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand on it.
+- [CLI Command](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
 
-evaluator = omnisafe.Evaluator()
-for item in os.scandir(os.path.join(LOG_DIR, 'torch_save')):
-    if item.is_file() and item.name.split('.')[-1] == 'pt':
-        evaluator.load_saved_model(save_dir=LOG_DIR, model_name=item.name)
-        evaluator.render(num_episode=10, camera_name='track', width=256, height=256)
-```
+We take great pleasure in collaborating with our users to create tutorials in various languages.
+Please refer to our list of currently supported languages.
+If you are interested in translating the tutorial into a new language or improving an existing version, kindly submit a PR to us.
 
 --------------------------------------------------------------------------------
 
 ## Changelog
-See [CHANGELOG.md](https://github.com/PKU-MARL/omnisafe/blob/main/CHANGELOG.md).
+
+See [CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
 
 ## The OmniSafe Team
 
-OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/PKU-MARL/people/PKU-YYang). Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-MARL/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
+OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-YYang).
+Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
+If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
 
 OmniSafe is released under Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,137 +1,161 @@
-
-        [https://github.com/PKU-MARL/omnisafe/raw/HEAD/images/logo.png]
+Metadata-Version: 2.1 Name: omnisafe Version: 0.4.0 Summary: A comprehensive
+and reliable benchmark for safe reinforcement learning. Author: OmniSafe
+Contributors License: Apache License, Version 2.0 Project-URL: Homepage, https:
+//github.com/OmniSafeAI/omnisafe Project-URL: Repository, https://github.com/
+OmniSafeAI/omnisafe Project-URL: Documentation, https://omnisafe.readthedocs.io
+Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
+Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
+Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
+Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: lint Provides-Extra: test License-File: LICENSE
+       [https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png]
 [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)]
-     (https://github.com/PKU-MARL) [![PyPI](https://img.shields.io/pypi/v/
-   omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![Documentation
-Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://
- omnisafe.readthedocs.io) [![Downloads](https://static.pepy.tech/personalized-
-                                    badge/
+    (https://github.com/OmniSafeAI) [![PyPI](https://img.shields.io/pypi/v/
+  omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
+      img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/
+test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/
+   HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
+  omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io) [![Downloads]
+                 (https://static.pepy.tech/personalized-badge/
  omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)]
       (https://pepy.tech/project/omnisafe) [![GitHub Repo Stars](https://
- img.shields.io/github/stars/PKU-MARL/omnisafe?color=brightgreen&logo=github)]
-   (https://github.com/PKU-MARL/OmniSafe/stargazers) [![codestyle](https://
+img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)]
+  (https://github.com/OmniSafeAI/OmniSafe/stargazers) [![codestyle](https://
  img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-      black) [![License](https://img.shields.io/github/license/PKU-MARL/
+     black) [![License](https://img.shields.io/github/license/OmniSafeAI/
 OmniSafe?label=license)](#license) [![CodeCov](https://img.shields.io/codecov/
- c/github/PKU-MARL/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-
-                                MARL/omnisafe)
+  c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/
+   OmniSafeAI/omnisafe) [![Open In Colab](https://colab.research.google.com/
+ assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/
+                                  omnisafe/)
    Documentation | Implemented_Algorithms | Installation | Getting_Started |
                                     License
 -------------------------------------------------------------------------------
 - **This library is currently under heavy development - if you have suggestions
 on the API or use-cases you'd like to be covered, please open a GitHub issue or
 reach out. We'd love to hear about how you're using the library.** OmniSafe is
 an infrastructural framework designed to accelerate safe reinforcement learning
 (RL) research by providing a comprehensive and reliable benchmark for safe RL
-algorithms. The field of RL has great potential to benefit society, but safety
-concerns are a significant issue, and RL algorithms have raised concerns about
-unintended harm or unsafe behavior. Safe RL intends to develop algorithms that
-minimize the risk of unintended harm or unsafe behavior, but there is currently
-a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe addresses
-these issues by providing more than 40 experimentally validated algorithms and
-a sound and efficient simulation environment. Researchers can use OmniSafe to
-conduct experiments and verify their ideas, ensuring consistency and enabling
-more efficient development of safe RL algorithms. By using OmniSafe as a
-benchmark, researchers can evaluate the performance of their own safe RL
-algorithms and contribute to the advancement of safe RL research. -------------
-------------------------------------------------------------------- ### Table
-of Contents   - [Implemented Algorithms](#implemented-algorithms) - [Latest
-SafeRL Papers](#latest-saferl-papers) - [List of Algorithms](#list-of-
-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-Policy Safe](#off-
-policy-safe) - [Model-Based Safe](#model-based-safe) - [Offline Safe](#offline-
-safe) - [Others](#others) - [Installation](#installation) - [Prerequisites]
-(#prerequisites) - [Install from source](#install-from-source) - [Install from
-PyPI](#install-from-pypi) - [Examples](#examples) - [Try with CLI](#try-with-
-cli) - [Getting Started](#getting-started) - [Important Hints](#important-
-hints) - [1. Run Agent from preset yaml file](#1-run-agent-from-preset-yaml-
-file) - [2. Run agent with custom cfg](#2-run-agent-with-custom-cfg) - [3. Run
-Agent from custom terminal config](#3-run-agent-from-custom-terminal-config) -
-[4. Evaluate Saved Policy](#4-evaluate-saved-policy) - [Changelog](#changelog)
-- [The OmniSafe Team](#the-omnisafe-team) - [License](#license) ---------------
------------------------------------------------------------------ ##
-Implemented Algorithms The supported interface algorithms currently include:
-### Latest SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy
-Optimization for Safe Reinforcement Learning (APPO) - **[NeurIPS 2022]**
-[Constrained Update Projection Approach to Safe Policy Optimization (CUP)]
-(https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]** [Effects of Safety
-State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/
-2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning
-via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/
-abs/2210.07573) - **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
-Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- **[ICML 2022]** [Constrained Variational Policy Optimization for Safe
-Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) - **[IJCAI
-2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement
-Learning](https://arxiv.org/abs/2205.11814) - **[ICLR 2022]** [Constrained
-Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) ###
-List of Algorithms #### On-Policy Safe - [X] [The Lagrange version of PPO (PPO-
-Lag)](https://cdn.openai.com/safexp-short.pdf) - [X] [The Lagrange version of
-TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]**
-[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
-achiam17a) - [X] **[ICLR 2019]** [Reward Constrained Policy Optimization
-(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [X] **[ICML 2020]**
-[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
-Lag)](https://arxiv.org/abs/2007.03964) - [X] **[NeurIPS 2020]** [First Order
-Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
-2002.06506) - [X] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
-under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [X] **[ICLR
-2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
-openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML 2021]** [CRPO: A New Approach
-for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
-abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
-for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf)
-#### Off-Policy Safe - [X] The Lagrange version of TD3 (TD3-Lag) - [X] The
-Lagrange version of DDPG (DDPG-Lag) - [X] The Lagrange version of SAC (SAC-Lag)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous
-Control (SDDPG)](https://arxiv.org/abs/1901.10031) - [X] **[ICML 2019]**
-[Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG-
-modular)](https://arxiv.org/abs/1901.10031) - [ ] **[ICML 2022]** [Constrained
+algorithms. The field of RL has great potential to benefit the society, and
+safety concerns are a significant issue, and RL algorithms have raised concerns
+about unintended harm or unsafe behavior. Safe RL intends to develop algorithms
+that minimize the risk of unintended harm or unsafe behavior, but there is
+currently a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe
+addresses these issues by providing more than 40 experimentally validated
+algorithms and a sound and efficient simulation environment. Researchers can
+use OmniSafe to conduct experiments and verify their ideas, ensuring
+consistency and enabling more efficient development of safe RL algorithms. By
+using OmniSafe as a benchmark, researchers can evaluate the performance of
+their own safe RL algorithms and contribute to the advancement of safe RL
+research. ---------------------------------------------------------------------
+----------- ### Table of Contents   - [Implemented Algorithms](#implemented-
+algorithms) - [Latest SafeRL Papers](#latest-saferl-papers) - [List of
+Algorithms](#list-of-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-
+Policy Safe](#off-policy-safe) - [Model-Based Safe](#model-based-safe) -
+[Offline Safe](#offline-safe) - [Others](#others) - [Installation]
+(#installation) - [Prerequisites](#prerequisites) - [Install from source]
+(#install-from-source) - [Install from PyPI](#install-from-pypi) - [Examples]
+(#examples) - [Try with CLI](#try-with-cli) - [Getting Started](#getting-
+started) - [Important Hints](#important-hints) - [Quickstart: Colab on the
+Cloud](#quickstart-colab-on-the-cloud) - [Changelog](#changelog) - [The
+OmniSafe Team](#the-omnisafe-team) - [License](#license) ----------------------
+---------------------------------------------------------- ## Implemented
+Algorithms The supported interface algorithms currently include: ### Latest
+SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe
+Reinforcement Learning (APPO) - **[NeurIPS 2022]** [Constrained Update
+Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/
+2209.07089) - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
+Exploration (Simmer)](https://arxiv.org/abs/2206.02675) - **[NeurIPS 2022]**
+[Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy
+Optimization Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]**
+[SautÃ© RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
+(SauteRL)](https://arxiv.org/abs/2202.06558) - **[ICML 2022]** [Constrained
 Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https:/
-/arxiv.org/abs/2201.11927) #### Model-Based Safe - [ ] **[NeurIPS 2021]** [Safe
-Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
-abs/2202.07789) - [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
-Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]**
-[Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
-(CAP)](https://arxiv.org/abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based
-Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
-Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
-Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) #### Offline Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)]
-(https://arxiv.org/abs/1812.02900) - [X] [The Constrained version of CRR (C-
-CRR)](https://proceedings.neurips.cc/paper/2020/hash/
-588cb956d6bbe67078f29f8de420a13d-Abstract.html) - [ ] **[AAAI 2022]**
-[Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ]
-(https://arxiv.org/abs/2107.09003) - [ ] **[ICLR 2022 (Spotlight)]**
-[COptiDICE: Offline Constrained Reinforcement Learning via Stationary
-Distribution Correction Estimation](https://arxiv.org/abs/
-2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
+/arxiv.org/abs/2201.11927) - **[IJCAI 2022]** [Penalized Proximal Policy
+Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
+- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models
+(LA-MBDA)](https://arxiv.org/abs/2201.09802) - **[AAAI 2022]** [Conservative
+and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https:/
+/arxiv.org/abs/2112.07701) ### List of Algorithms #### On-Policy Safe - [X]
+[The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
+short.pdf) - [X] [The Lagrange version of TRPO (TRPO-Lag)](https://
+cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]** [Constrained Policy
+Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [X] **[ICLR
+2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
+forum?id=SkfrvsA9FX) - [X] **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
+(FOCOPS)](https://arxiv.org/abs/2002.06506) - [X] **[AAAI 2020]** [IPO:
+Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
+abs/1910.09615) - [X] **[ICLR 2020]** [Projection-Based Constrained Policy
+Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML
+2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
+Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
+Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
+arxiv.org/pdf/2205.11814.pdf) #### Off-Policy Safe - [X] The Lagrange version
+of TD3 (TD3-Lag) - [X] The Lagrange version of DDPG (DDPG-Lag) - [X] The
+Lagrange version of SAC (SAC-Lag) - [X] **[ICML 2019]** [Lyapunov-based Safe
+Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/
+1901.10031) - [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for
+Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031) - [ ] **
+[ICML 2022]** [Constrained Variational Policy Optimization for Safe
+Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) #### Model-
+Based Safe - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining
+the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [X] **[CoRL 2021
+(Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://
+arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]** [Conservative and Adaptive
+Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/
+abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement
+Learning via a Constrained Proximal Policy Optimization Algorithm](https://
+arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained Policy
+Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
+2201.09802) - [X] **[ICML 2022 Workshop]** [Constrained Model-based
+Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
+arxiv.org/abs/2010.07968) - [X] **[NeurIPS 2018]** [Constrained Cross-Entropy
+Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
+paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) #### Offline
+Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/
+1812.02900) - [X] [The Constrained version of CRR (C-CRR)](https://
+proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-
+Abstract.html) - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe
+Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003) - [ ] **
+[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement
+Learning via Stationary Distribution Correction Estimation](https://arxiv.org/
+abs/2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
 Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) ####
 Others - [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)]
 (https://arxiv.org/abs/1801.08757) - [ ] **[RA-L 2021]** [Recovery RL: Safe
 Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/
 2010.15920) - [X] **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
 Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
 - [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
 Exploration](https://arxiv.org/abs/2206.02675) --------------------------------
 ------------------------------------------------ ## Installation ###
-Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. #### Install
-from source ```bash # Clone the repo git clone https://github.com/PKU-MARL/
-omnisafe cd omnisafe # Create a conda environment conda create -n omnisafe
-python=3.8 conda activate omnisafe # Install omnisafe pip install -e . ``` ####
-Install from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
-omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
-(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
-omnisafe ``` ### Examples ```bash cd examples python train_policy.py --algo
-PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device
-cpu --vector-env-nums 1 --torch-threads 1 ``` **algo:** | Type | Name | | -----
------------- | ---------------------------------------------------------------
-- | | `Base-On-Policy` | `PolicyGradient, PPO`
+Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
+test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
+versions of macOS. We will accept PRs related to Windows, but do not officially
+support it. #### Install from source ```bash # Clone the repo git clone https:/
+/github.com/OmniSafeAI/omnisafe cd omnisafe # Create a conda environment conda
+env create --file conda-recipe.yaml conda activate omnisafe # Install omnisafe
+pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [![PyPI]
+(https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
+pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
+omnisafe?label=status). ```bash pip install omnisafe ``` ### Examples ```bash
+cd examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 -
+-parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
+threads 1 ``` **algo:** | Type | Name | | ----------------- | -----------------
+----------------------------------------------- | | `Base-On-Policy` |
+`PolicyGradient, PPO`
 `NaturalPG, TRPO` | | `Base-Off-Policy` | `DDPG, TD3, SAC` | | `Naive Lagrange`
 | `RCPO, PPOLag, TRPOLag`
 `DDPGLag, TD3Lag, SACLag` | | `PID Lagrange` | `CPPOPid, TRPOPid` | | `First
 Order` | `FOCOPS, CUP` | | `Second Order` | `SDDPG, CPO, PCPO` | | `Saute RL` |
 `PPOSaute, PPOLagSaute` | | `Simmer RL` | `PPOSimmerQ, PPOSimmerPid`
 `PPOLagSimmerQ, PPOLagSimmerPid` | | `EarlyTerminated` | `PPOEarlyTerminated`
 `PPOLagEarlyTerminated` | | `Model-Based` | `CAP, MBPPOLag, SafeLOOP` | **env-
@@ -140,63 +164,54 @@
  ____________________________________________________________________________
 |Category_______|Task_______|Agent___________________|Example________________|
 |               |Goal[012]__|                        |                       |
 |Safe Navigation|Button[012]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |Push[012]__|                        |                       |
 |_______________|Circle[012]|________________________|_______________________|
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
-|Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v4                     |
+|Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_______________|___________|Humanoid________________|_______________________|
 More information about environments, please refer to [Safety Gymnasium](https:/
 /www.safety-gymnasium.com/) **parallel:** `Number of parallels` #### Try with
-CLI **A video example** ![Segmentfault](https://github.com/PKU-MARL/omnisafe/
+CLI **A video example** ![Segmentfault](https://github.com/OmniSafeAI/omnisafe/
 blob/main/images/CLI_example.svg) ```bash pip install omnisafe omnisafe --help
 # Ask for help omnisafe benchmark --help # The benchmark also can be replaced
 with 'eval', 'train', 'train-config' # Quick benchmarking for your research,
 just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path
 of the config file(refer to omnisafe/examples/benchmarks for format) omnisafe
 benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml # Quick
 evaluating and rendering your trained policy, just specify: 1.path of algorithm
 which you trained omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-
 episode 1 # Quick training some algorithms to validate your thoughts # Note:
 use `key1:key2`, your can select key of hyperparameters which are recursively
 contained, and use `--custom-cfgs`, you can add custom cfgs via CLI omnisafe
 train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs
-algo_cfgs:update_cycle --custom-cfgs 1024 # Quick training some algorithms via
-a saved config file, the format is as same as default format omnisafe train-
-config ./saved_source/train_config.yaml ``` -----------------------------------
---------------------------------------------- ## Getting Started #### Important
-Hints - `train_cfgs:torch_threads` is especially important for training speed,
-and is varying with users' machine, this value shouldn't be too small or too
-large. ### 1. Run Agent from preset yaml file ```python import omnisafe env_id
-= 'SafetyPointGoal1-v0' agent = omnisafe.Agent('PPOLag', env_id) agent.learn()
-``` ### 2. Run agent with custom cfg ```python import omnisafe env_id =
-'SafetyPointGoal1-v0' custom_cfgs = { 'train_cfgs': { 'total_steps': 1024000,
-'vector_env_nums': 1, 'parallel': 1, }, 'algo_cfgs': { 'update_cycle': 2048,
-'update_iters': 1, }, 'logger_cfgs': { 'use_wandb': False, }, } agent =
-omnisafe.Agent('PPOLag', env_id, custom_cfgs=custom_cfgs) agent.learn() ``` ###
-3. Run Agent from custom terminal config You can also run agent from a custom
-terminal config. You can set any config in a corresponding yaml file. For
-example, you can run `PPOLag` agent on `SafetyPointGoal1-v0` environment with
-`total_steps=1024000`, `vector_env_nums=1` and `parallel=1` by: ```bash cd
-examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --
-parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
-threads 1 ``` ### 4. Evaluate Saved Policy ```python import os import omnisafe
-# Just fill your experiment's log directory in here. # Such as: ~/omnisafe/
-runs/SafetyPointGoal1-v0/CPO/seed-000-2022-12-25_14-45-05 LOG_DIR = ''
-evaluator = omnisafe.Evaluator() for item in os.scandir(os.path.join(LOG_DIR,
-'torch_save')): if item.is_file() and item.name.split('.')[-1] == 'pt':
-evaluator.load_saved_model(save_dir=LOG_DIR, model_name=item.name)
-evaluator.render(num_episode=10, camera_name='track', width=256, height=256)
-``` ---------------------------------------------------------------------------
------ ## Changelog See [CHANGELOG.md](https://github.com/PKU-MARL/omnisafe/
-blob/main/CHANGELOG.md). ## The OmniSafe Team OmniSafe is mainly developed by
-the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/
-orgs/PKU-MARL/people/PKU-YYang). Our SafeRL research team members include
-[Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/
-Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://
-github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai
-Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-
-2077). If you have any questions in the process of using omnisafe, don't
-hesitate to ask your questions on [the GitHub issue page](https://github.com/
-PKU-MARL/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
-## License OmniSafe is released under Apache License 2.0.
+algo_cfgs:steps_per_epoch --custom-cfgs 1024 # Quick training some algorithms
+via a saved config file, the format is as same as default format omnisafe
+train-config ./saved_source/train_config.yaml ``` -----------------------------
+--------------------------------------------------- ## Getting Started ###
+Important Hints - `train_cfgs:torch_threads` is especially important for
+training speed, and is varying with users' machine, this value shouldn't be too
+small or too large. ### Quickstart: Colab on the Cloud Explore OmniSafe easily
+and quickly through a series of colab notebooks: - [Getting Started](https://
+colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that
+users can quickly hand on it. - [CLI Command](https://
+colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
+take great pleasure in collaborating with our users to create tutorials in
+various languages. Please refer to our list of currently supported languages.
+If you are interested in translating the tutorial into a new language or
+improving an existing version, kindly submit a PR to us. ----------------------
+---------------------------------------------------------- ## Changelog See
+[CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
+## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research team
+directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-
+YYang). Our SafeRL research team members include [Borong Zhang](https://
+github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https:/
+/github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang
+Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/
+XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any
+questions in the process of using omnisafe, don't hesitate to ask your
+questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/
+issues/new/choose), we will reply to you in 2-3 working days. ## License
+OmniSafe is released under Apache License 2.0.
```

### Comparing `omnisafe-0.3.0/omnisafe/__init__.py` & `omnisafe-0.4.0/omnisafe/models/critic/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""OmniSafe: A comprehensive and reliable benchmark for safe reinforcement learning."""
+"""The abstract interfaces of Critic networks for the Actor-Critic algorithm."""
 
-from omnisafe import algorithms
-from omnisafe.algorithms import ALGORITHMS
-from omnisafe.algorithms.algo_wrapper import AlgoWrapper as Agent
-from omnisafe.evaluator import Evaluator
-
-# from omnisafe.algorithms.env_wrapper import EnvWrapper as Env
-from omnisafe.version import __version__
-
-
-# from omnisafe.evaluator import Evaluator
+from omnisafe.models.critic.critic_builder import CriticBuilder
+from omnisafe.models.critic.q_critic import QCritic
+from omnisafe.models.critic.v_critic import VCritic
```

### Comparing `omnisafe-0.3.0/omnisafe/adapter/__init__.py` & `omnisafe-0.4.0/omnisafe/adapter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Adapter for the environment and the algorithm."""
 
 from omnisafe.adapter.early_terminated_adapter import EarlyTerminatedAdapter
+from omnisafe.adapter.modelbased_adapter import ModelBasedAdapter
 from omnisafe.adapter.offpolicy_adapter import OffPolicyAdapter
 from omnisafe.adapter.online_adapter import OnlineAdapter
 from omnisafe.adapter.onpolicy_adapter import OnPolicyAdapter
 from omnisafe.adapter.saute_adapter import SauteAdapter
```

### Comparing `omnisafe-0.3.0/omnisafe/adapter/offpolicy_adapter.py` & `omnisafe-0.4.0/omnisafe/adapter/onpolicy_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,165 +8,174 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""OffPolicy Adapter for OmniSafe."""
+"""OnPolicy Adapter for OmniSafe."""
 
 from __future__ import annotations
 
+from typing import Any
+
 import torch
+from rich.progress import track
 
 from omnisafe.adapter.online_adapter import OnlineAdapter
-from omnisafe.common.buffer import VectorOffPolicyBuffer
+from omnisafe.common.buffer import VectorOnPolicyBuffer
 from omnisafe.common.logger import Logger
-from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
+from omnisafe.models.actor_critic.constraint_actor_critic import ConstraintActorCritic
 from omnisafe.utils.config import Config
 
 
-class OffPolicyAdapter(OnlineAdapter):
-    """OffPolicy Adapter for OmniSafe.
-
-    :class:`OffPolicyAdapter` is used to adapt the environment to the off-policy training.
-
-    .. note::
+class OnPolicyAdapter(OnlineAdapter):
+    """OnPolicy Adapter for OmniSafe.
 
-        Off-policy training need to update the policy before finish the episode,
-        so the :class:`OffPolicyAdapter` will store the current observation in ``_current_obs``.
-        After update the policy, the agent will *remember* the current observation and
-        use it to interact with the environment.
+    :class:`OnPolicyAdapter` is used to adapt the environment to the on-policy training.
 
     Args:
         env_id (str): The environment id.
         num_envs (int): The number of environments.
         seed (int): The random seed.
         cfgs (Config): The configuration.
-
-    Attributes:
-        _env_id (str): The environment id.
-        _env (CMDP): The environment.
-        _cfgs (Config): The configuration.
-        _device (torch.device): The device.
-        _ep_ret (torch.Tensor): The episode return.
-        _ep_cost (torch.Tensor): The episode cost.
-        _ep_len (torch.Tensor): The episode length.
-        _current_obs (torch.Tensor): The current observation.
-        _max_ep_len (int): The maximum episode length.
     """
 
+    _ep_ret: torch.Tensor
+    _ep_cost: torch.Tensor
+    _ep_len: torch.Tensor
+
     def __init__(  # pylint: disable=too-many-arguments
         self,
         env_id: str,
         num_envs: int,
         seed: int,
         cfgs: Config,
     ) -> None:
+        """Initialize an instance of :class:`OnPolicyAdapter`."""
         super().__init__(env_id, num_envs, seed, cfgs)
-
-        self._ep_ret: torch.Tensor
-        self._ep_cost: torch.Tensor
-        self._ep_len: torch.Tensor
-        self._current_obs, _ = self.reset()
-        self._max_ep_len = 1000
-        self._device = cfgs.train_cfgs.device
         self._reset_log()
 
-    def roll_out(  # pylint: disable=too-many-locals
+    def rollout(  # pylint: disable=too-many-locals
         self,
-        roll_out_step: int,
-        agent: ConstraintActorQCritic,
-        buffer: VectorOffPolicyBuffer,
+        steps_per_epoch: int,
+        agent: ConstraintActorCritic,
+        buffer: VectorOnPolicyBuffer,
         logger: Logger,
-        use_rand_action: bool,
     ) -> None:
-        """Roll out the environment and store the data in the buffer.
+        """Rollout the environment and store the data in the buffer.
 
         .. warning::
-
             As OmniSafe uses :class:`AutoReset` wrapper, the environment will be reset automatically,
             so the final observation will be stored in ``info['final_observation']``.
 
         Args:
             steps_per_epoch (int): Number of steps per epoch.
-            agent (ConstraintActorCritic): Agent.
-            buf (VectorOnPolicyBuffer): Buffer.
-            logger (Logger): Logger.
+            agent (ConstraintActorCritic): Constraint actor-critic, including actor , reward critic
+                and cost critic.
+            buffer (VectorOnPolicyBuffer): Vector on-policy buffer.
+            logger (Logger): Logger, to log ``EpRet``, ``EpCost``, ``EpLen``.
         """
-        for _ in range(roll_out_step):
-            if use_rand_action:
-                act = torch.as_tensor(self._env.sample_action(), dtype=torch.float32).to(
-                    self._device,
-                )
-            else:
-                act = agent.step(self._current_obs, deterministic=False)
+        self._reset_log()
 
+        obs, _ = self.reset()
+        for step in track(
+            range(steps_per_epoch),
+            description=f'Processing rollout for epoch: {logger.current_epoch}...',
+        ):
+            act, value_r, value_c, logp = agent.step(obs)
             next_obs, reward, cost, terminated, truncated, info = self.step(act)
 
             self._log_value(reward=reward, cost=cost, info=info)
 
+            if self._cfgs.algo_cfgs.use_cost:
+                logger.store({'Value/cost': value_c})
+            logger.store({'Value/reward': value_r})
+
             buffer.store(
-                obs=self._current_obs,
+                obs=obs,
                 act=act,
                 reward=reward,
                 cost=cost,
-                done=terminated,
-                next_obs=next_obs,
+                value_r=value_r,
+                value_c=value_c,
+                logp=logp,
             )
 
-            self._current_obs = next_obs
-            for idx, done in enumerate(torch.logical_or(terminated, truncated)):
-                if done or self._ep_len[idx] >= self._max_ep_len:
-                    # self.reset()
-                    self._log_metrics(logger, idx)
-                    self._reset_log(idx)
+            obs = next_obs
+            epoch_end = step >= steps_per_epoch - 1
+            for idx, (done, time_out) in enumerate(zip(terminated, truncated)):
+                if epoch_end or done or time_out:
+                    last_value_r = torch.zeros(1)
+                    last_value_c = torch.zeros(1)
+                    if not done:
+                        if epoch_end:
+                            logger.log(
+                                f'Warning: trajectory cut off when rollout by epoch at {self._ep_len[idx]} steps.',
+                            )
+                            _, last_value_r, last_value_c, _ = agent.step(obs[idx])
+                        if time_out:
+                            _, last_value_r, last_value_c, _ = agent.step(
+                                info['final_observation'][idx],
+                            )
+                        last_value_r = last_value_r.unsqueeze(0)
+                        last_value_c = last_value_c.unsqueeze(0)
+
+                    if done or time_out:
+                        self._log_metrics(logger, idx)
+                        self._reset_log(idx)
+
+                        self._ep_ret[idx] = 0.0
+                        self._ep_cost[idx] = 0.0
+                        self._ep_len[idx] = 0.0
+
+                    buffer.finish_path(last_value_r, last_value_c, idx)
 
     def _log_value(
         self,
         reward: torch.Tensor,
         cost: torch.Tensor,
-        info: dict,
-        **kwargs,  # pylint: disable=unused-argument
+        info: dict[str, Any],
     ) -> None:
         """Log value.
 
         .. note::
             OmniSafe uses :class:`RewardNormalizer` wrapper, so the original reward and cost will
             be stored in ``info['original_reward']`` and ``info['original_cost']``.
 
         Args:
-            reward (torch.Tensor): The reward.
-            cost (torch.Tensor): The cost.
-            **kwargs: Other arguments.
+            reward (torch.Tensor): The immediate step reward.
+            cost (torch.Tensor): The immediate step cost.
+            info (dict[str, Any]): Some information logged by the environment.
         """
         self._ep_ret += info.get('original_reward', reward).cpu()
         self._ep_cost += info.get('original_cost', cost).cpu()
         self._ep_len += 1
 
     def _log_metrics(self, logger: Logger, idx: int) -> None:
-        """Log metrics.
+        """Log metrics, including ``EpRet``, ``EpCost``, ``EpLen``.
 
         Args:
-            logger (Logger): Logger.
+            logger (Logger): Logger, to log ``EpRet``, ``EpCost``, ``EpLen``.
             idx (int): The index of the environment.
         """
         logger.store(
-            **{
+            {
                 'Metrics/EpRet': self._ep_ret[idx],
                 'Metrics/EpCost': self._ep_cost[idx],
                 'Metrics/EpLen': self._ep_len[idx],
             },
         )
 
     def _reset_log(self, idx: int | None = None) -> None:
-        """Reset log.
+        """Reset the episode return, episode cost and episode length.
 
         Args:
-            idx (int | None): The index of the environment.
+            idx (int or None, optional): The index of the environment. Defaults to None
+                (single environment).
         """
         if idx is None:
             self._ep_ret = torch.zeros(self._env.num_envs)
             self._ep_cost = torch.zeros(self._env.num_envs)
             self._ep_len = torch.zeros(self._env.num_envs)
         else:
             self._ep_ret[idx] = 0.0
```

### Comparing `omnisafe-0.3.0/omnisafe/adapter/online_adapter.py` & `omnisafe-0.4.0/omnisafe/envs/mujoco_env.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,182 +8,167 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Online Adapter for OmniSafe."""
-
+"""Environments in the Safety Gymnasium."""
 from __future__ import annotations
 
+from typing import Any
+
+import gymnasium
+import numpy as np
 import torch
 
-from omnisafe.envs.core import make, support_envs
-from omnisafe.envs.wrapper import (
-    ActionScale,
-    AutoReset,
-    CostNormalize,
-    ObsNormalize,
-    RewardNormalize,
-    TimeLimit,
-    Unsqueeze,
-)
-from omnisafe.typing import OmnisafeSpace
-from omnisafe.utils.config import Config
-
-
-class OnlineAdapter:
-    """Online Adapter for OmniSafe.
-
-    Online Adapter is used to adapt the environment to the online training.
-
-    Args:
-        env_id (str): The environment id.
-        num_envs (int): The number of environments.
-        seed (int): The random seed.
-        cfgs (Config): The configuration.
+from omnisafe.envs.core import CMDP, env_register
+from omnisafe.typing import Box
 
-    Attributes:
-        _env_id (str): The environment id.
-        _env (CMDP): The environment.
-        _cfgs (Config): The configuration.
-        _device (torch.device): The device.
 
+@env_register
+class MujocoEnv(CMDP):
+    """Gymnasium Mujoco environment.
+
+    Attributes:
+        _support_envs (list[str]): List of supported environments.
+        need_auto_reset_wrapper (bool): Whether to use auto reset wrapper.
+        need_time_limit_wrapper (bool): Whether to use time limit wrapper.
     """
 
-    def __init__(  # pylint: disable=too-many-arguments
+    _support_envs = [
+        'Ant-v4',
+        'Hopper-v4',
+        'Walker2d-v4',
+        'Humanoid-v4',
+        'Swimmer-v4',
+        'HalfCheetah-v4',
+    ]
+    need_auto_reset_wrapper = False
+
+    need_time_limit_wrapper = False
+    need_action_repeat_wrapper = True
+
+    def __init__(
         self,
         env_id: str,
-        num_envs: int,
-        seed: int,
-        cfgs: Config,
+        num_envs: int = 1,
+        device: str = 'cpu',
+        **kwargs: Any,
     ) -> None:
-        """Initialize the online adapter.
+        """Initialize the environment.
 
         Args:
-            env_id (str): The environment id.
-            num_envs (int): The number of environments.
-            seed (int): The random seed.
-            cfgs (Config): The configuration.
-
+            env_id (str): Environment id.
+            num_envs (int, optional): Number of environments. Defaults to 1.
+            device (torch.device, optional): Device to store the data. Defaults to 'cpu'.
+            **kwargs: Other arguments.
         """
-        assert env_id in support_envs(), f'Env {env_id} is not supported.'
-
+        super().__init__(env_id)
         self._env_id = env_id
-        self._env = make(env_id, num_envs=num_envs, device=cfgs.train_cfgs.device)
-        self._cfgs = cfgs
-        self._device = cfgs.train_cfgs.device
-        self._wrapper(
-            obs_normalize=cfgs.algo_cfgs.obs_normalize,
-            reward_normalize=cfgs.algo_cfgs.reward_normalize,
-            cost_normalize=cfgs.algo_cfgs.cost_normalize,
-        )
-        self._env.set_seed(seed)
-
-    def _wrapper(
-        self,
-        obs_normalize: bool = True,
-        reward_normalize: bool = True,
-        cost_normalize: bool = True,
-    ):
-        """Wrapper the environment.
-
-        .. hint::
-
-            OmniSafe supports the following wrappers:
-
-            .. list-table::
-
-                *   -   Wrapper
-                    -   Description
-                *   -   TimeLimit
-                    -   Limit the time steps of the environment.
-                *   -   AutoReset
-                    -   Reset the environment when the episode is done.
-                *   -   ObsNormalize
-                    -   Normalize the observation.
-                *   -   RewardNormalize
-                    -   Normalize the reward.
-                *   -   CostNormalize
-                    -   Normalize the cost.
-                *   -   ActionScale
-                    -   Scale the action.
-                *   -   Unsqueeze
-                    -   Unsqueeze the step result for single environment case.
-
-        Args:
-            obs_normalize (bool): Whether to normalize the observation.
-            reward_normalize (bool): Whether to normalize the reward.
-            cost_normalize (bool): Whether to normalize the cost.
-
-        """
-        if self._env.need_time_limit_wrapper:
-            self._env = TimeLimit(self._env, device=self._device, time_limit=1000)
-        if self._env.need_auto_reset_wrapper:
-            self._env = AutoReset(self._env, device=self._device)
-        if obs_normalize:
-            self._env = ObsNormalize(self._env, device=self._device)
-        if reward_normalize:
-            self._env = RewardNormalize(self._env, device=self._device)
-        if cost_normalize:
-            self._env = CostNormalize(self._env, device=self._device)
-        self._env = ActionScale(self._env, device=self._device, low=-1.0, high=1.0)
-        if self._env.num_envs == 1:
-            self._env = Unsqueeze(self._env, device=self._device)
-
-    @property
-    def action_space(self) -> OmnisafeSpace:
-        """The action space of the environment.
-
-        Returns:
-            OmnisafeSpace: the action space.
-        """
-        return self._env.action_space
-
-    @property
-    def observation_space(self) -> OmnisafeSpace:
-        """The observation space of the environment.
+        if num_envs == 1:
+            # set healthy_reward=0.0 for removing the safety constraint in reward
+            self._env = gymnasium.make(id=env_id, autoreset=False, **kwargs)
+            assert isinstance(self._env.action_space, Box), 'Only support Box action space.'
+            assert isinstance(
+                self._env.observation_space,
+                Box,
+            ), 'Only support Box observation space.'
+            self._action_space = self._env.action_space
+            self._observation_space = self._env.observation_space
+        else:
+            raise NotImplementedError('Only support num_envs=1 now.')
+        self._device = torch.device(device)
 
-        Returns:
-            OmnisafeSpace: the observation space.
-        """
-        return self._env.observation_space
+        self._num_envs = num_envs
+        self._metadata = self._env.metadata
 
     def step(
         self,
         action: torch.Tensor,
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
-        """Run one timestep of the environment's dynamics using the agent actions.
+        """Step the environment.
+
+        .. note::
+
+            OmniSafe use auto reset wrapper to reset the environment when the episode is
+            terminated. So the ``obs`` will be the first observation of the next episode.
+            And the true ``final_observation`` in ``info`` will be stored in the ``final_observation`` key of ``info``.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): Action to take.
 
         Returns:
             observation (torch.Tensor): agent's observation of the current environment.
             reward (torch.Tensor): amount of reward returned after previous action.
             cost (torch.Tensor): amount of cost returned after previous action.
             terminated (torch.Tensor): whether the episode has ended.
             truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
             info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
         """
-        return self._env.step(action)
+        obs, reward, terminated, truncated, info = self._env.step(
+            action.detach().cpu().numpy(),
+        )
+        obs, reward, terminated, truncated = (
+            torch.as_tensor(x, dtype=torch.float32, device=self._device)
+            for x in (obs, reward, terminated, truncated)
+        )
+        cost = terminated.float()
+        if 'final_observation' in info:
+            info['final_observation'] = np.array(
+                [
+                    array if array is not None else np.zeros(obs.shape[-1])
+                    for array in info['final_observation']
+                ],
+            )
+            info['final_observation'] = torch.as_tensor(
+                info['final_observation'],
+                dtype=torch.float32,
+                device=self._device,
+            )
+
+        return obs, reward, cost, terminated, truncated, info
 
-    def reset(self) -> tuple[torch.Tensor, dict]:
-        """Resets the environment and returns an initial observation.
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
+        """Reset the environment.
 
         Args:
-            seed (Optional[int]): seed for the environment.
+            seed (int, optional): Seed to reset the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): the initial observation of the space.
+            observation (torch.Tensor): agent's observation of the current environment.
             info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
         """
-        return self._env.reset()
+        obs, info = self._env.reset(seed=seed)
+        return torch.as_tensor(obs, dtype=torch.float32, device=self._device), info
+
+    def set_seed(self, seed: int) -> None:
+        """Set the seed for the environment.
+
+        Args:
+            seed (int): Seed to set.
+        """
+        self.reset(seed=seed)
 
-    def save(self) -> dict[str, torch.nn.Module]:
-        """Save the environment.
+    def sample_action(self) -> torch.Tensor:
+        """Sample a random action.
 
         Returns:
-            Dict[str, torch.nn.Module]: the saved environment.
+            torch.Tensor: A random action.
         """
-        return self._env.save()
+        return torch.as_tensor(
+            self._env.action_space.sample(),
+            dtype=torch.float32,
+            device=self._device,
+        )
+
+    def render(self) -> Any:
+        """Render the environment.
+
+        Returns:
+            Any: Rendered environment.
+        """
+        return self._env.render()
+
+    def close(self) -> None:
+        """Close the environment."""
+        self._env.close()
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,47 +13,54 @@
 # limitations under the License.
 # ==============================================================================
 """Safe Reinforcement Learning algorithms."""
 
 import itertools
 from types import MappingProxyType
 
-from omnisafe.algorithms import off_policy, on_policy
+from omnisafe.algorithms import model_based, off_policy, on_policy
 from omnisafe.algorithms.base_algo import BaseAlgo
-from omnisafe.algorithms.off_policy import DDPG, SAC, TD3
+
+# Off-Policy Safe
+from omnisafe.algorithms.off_policy import DDPG, SAC, TD3, DDPGLag, SACLag, TD3Lag
 
 # On-Policy Safe
 from omnisafe.algorithms.on_policy import (
     CPO,
+    CPPOPID,
     CUP,
     FOCOPS,
     PCPO,
     PDO,
     PPO,
     RCPO,
     TRPO,
+    TRPOPID,
     NaturalPG,
     OnCRPO,
     PolicyGradient,
+    PPOEarlyTerminated,
     PPOLag,
+    PPOSaute,
+    PPOSimmerPID,
+    TRPOEarlyTerminated,
     TRPOLag,
+    TRPOSaute,
+    TRPOSimmerPID,
 )
 
 
 # Model-based Safe
 # from omnisafe.algorithms.model_based import CAP, MBPPOLag, SafeLOOP
 
-# Off-Policy Safe
-# from omnisafe.algorithms.off_policy import DDPG, SAC, SDDPG, TD3, DDPGLag, SACLag, TD3Lag
-
 
 ALGORITHMS = {
     'on-policy': tuple(on_policy.__all__),
     'off-policy': tuple(off_policy.__all__),
-    # 'model-based': tuple(model_based.__all__),
+    'model-based': tuple(model_based.__all__),
 }
 
 ALGORITHM2TYPE = {
     algo: algo_type for algo_type, algorithms in ALGORITHMS.items() for algo in algorithms
 }
 
 __all__ = ALGORITHMS['all'] = tuple(itertools.chain.from_iterable(ALGORITHMS.values()))
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/algo_wrapper.py` & `omnisafe-0.4.0/omnisafe/algorithms/algo_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,68 +12,93 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the AlgoWrapper Class."""
 
 from __future__ import annotations
 
-import difflib
 import os
 import sys
 from typing import Any
 
-import psutil
 import torch
 
 from omnisafe.algorithms import ALGORITHM2TYPE, ALGORITHMS, registry
 from omnisafe.algorithms.base_algo import BaseAlgo
 from omnisafe.envs import support_envs
 from omnisafe.evaluator import Evaluator
 from omnisafe.utils import distributed
-from omnisafe.utils.config import check_all_configs, get_default_kwargs_yaml
+from omnisafe.utils.config import Config, check_all_configs, get_default_kwargs_yaml
 from omnisafe.utils.plotter import Plotter
 from omnisafe.utils.tools import recursive_check_config
 
 
 class AlgoWrapper:
-    """Algo Wrapper for algo."""
+    """Algo Wrapper for algorithms.
+
+    Args:
+        algo (str): The algorithm name.
+        env_id (str): The environment id.
+        train_terminal_cfgs (dict[str, Any], optional): The configurations for training termination.
+            Defaults to None.
+        custom_cfgs (dict[str, Any], optional): The custom configurations. Defaults to None.
+
+    Attributes:
+        algo (str): The algorithm name.
+        env_id (str): The environment id.
+        train_terminal_cfgs (dict[str, Any]): The configurations for training termination.
+        custom_cfgs (dict[str, Any]): The custom configurations.
+        cfgs (Config): The configurations for the algorithm.
+        algo_type (str): The algorithm type.
+    """
+
+    algo_type: str
 
     def __init__(
         self,
         algo: str,
         env_id: str,
         train_terminal_cfgs: dict[str, Any] | None = None,
         custom_cfgs: dict[str, Any] | None = None,
     ) -> None:
-        self.algo = algo
-        self.env_id = env_id
+        """Initialize an instance of :class:`AlgoWrapper`."""
+        self.algo: str = algo
+        self.env_id: str = env_id
         # algo_type will set in _init_checks()
-        self.algo_type: str
-        self.agent: BaseAlgo
-
-        self.train_terminal_cfgs = train_terminal_cfgs
-        self.custom_cfgs = custom_cfgs
-        self._evaluator: Evaluator = None
-        self._plotter: Plotter = None
-        self.cfgs = self._init_config()
+        self.train_terminal_cfgs: dict[str, Any] | None = train_terminal_cfgs
+        self.custom_cfgs: dict[str, Any] | None = custom_cfgs
+        self._evaluator: Evaluator | None = None
+        self._plotter: Plotter | None = None
+        self.cfgs: Config = self._init_config()
         self._init_checks()
+        self._init_algo()
 
-    def _init_config(self):
-        """Init config."""
-        assert self.algo in ALGORITHMS['all'], (
-            f"{self.algo} doesn't exist. "
-            f"Did you mean {difflib.get_close_matches(self.algo, ALGORITHMS['all'], n=1)[0]}?"
-        )
+    def _init_config(self) -> Config:
+        """Initialize config.
+
+        Initialize the configurations for the algorithm, following the order of default
+        configurations, custom configurations, and terminal configurations.
+
+        Returns:
+            The configurations for the algorithm.
+
+        Raises:
+            AssertionError: If the algorithm name is not in the supported algorithms.
+        """
+        assert (
+            self.algo in ALGORITHMS['all']
+        ), f"{self.algo} doesn't exist. Please choose from {ALGORITHMS['all']}."
         self.algo_type = ALGORITHM2TYPE.get(self.algo, '')
-        if self.algo_type is None or self.algo_type == '':
-            raise ValueError(f'{self.algo} is not supported!')
-        if self.algo_type in {'off-policy', 'model-based'} and self.train_terminal_cfgs is not None:
+        if self.algo_type in ['model-based'] and self.train_terminal_cfgs is not None:
             assert (
                 self.train_terminal_cfgs['parallel'] == 1
-            ), 'off-policy or model-based only support parallel==1!'
+            ), 'model-based only support parallel==1!'
+            assert (
+                self.train_terminal_cfgs['vector_env_nums'] == 1
+            ), 'model-based only support vector_env_nums==1!'
         cfgs = get_default_kwargs_yaml(self.algo, self.env_id, self.algo_type)
 
         # update the cfgs from custom configurations
         if self.custom_cfgs:
             # avoid repeatedly record the env_id and algo
             if 'env_id' in self.custom_cfgs:
                 self.custom_cfgs.pop('env_id')
@@ -95,77 +120,78 @@
             # validate the keys of train_terminal_cfgs configuration
             recursive_check_config(self.train_terminal_cfgs, cfgs.train_cfgs)
             # update the cfgs.train_cfgs from train_terminal configurations
             cfgs.train_cfgs.recurisve_update(self.train_terminal_cfgs)
             # save configurations specified in current experiment
             cfgs.recurisve_update({'exp_increment_cfgs': {'train_cfgs': self.train_terminal_cfgs}})
 
-        # the exp_name format is PPO-{SafetyPointGoal1-v0}-
+        # the exp_name format is PPO-{SafetyPointGoal1-v0}
         exp_name = f'{self.algo}-{{{self.env_id}}}'
         cfgs.recurisve_update({'exp_name': exp_name, 'env_id': self.env_id, 'algo': self.algo})
         cfgs.train_cfgs.recurisve_update(
-            {'epochs': cfgs.train_cfgs.total_steps // cfgs.algo_cfgs.update_cycle},
+            {'epochs': cfgs.train_cfgs.total_steps // cfgs.algo_cfgs.steps_per_epoch},
         )
         return cfgs
 
-    def _init_checks(self):
-        """Init checks."""
+    def _init_checks(self) -> None:
+        """Initial checks."""
         assert isinstance(self.algo, str), 'algo must be a string!'
         assert isinstance(self.cfgs.train_cfgs.parallel, int), 'parallel must be an integer!'
         assert self.cfgs.train_cfgs.parallel > 0, 'parallel must be greater than 0!'
         assert (
-            isinstance(self.custom_cfgs, dict) or self.custom_cfgs is None
-        ), 'custom_cfgs must be a dict!'
-        assert self.env_id in support_envs(), (
-            f"{self.env_id} doesn't exist. "
-            f'Did you mean {difflib.get_close_matches(self.env_id, support_envs(), n=1)[0]}?'
-        )
-
-    def learn(self):
-        """Agent Learning."""
-        # Use number of physical cores as default.
-        # If also hardware threading CPUs should be used
-        # enable this by the use_number_of_threads=True
-        physical_cores = psutil.cpu_count(logical=False)
-        use_number_of_threads = bool(self.cfgs.train_cfgs.parallel > physical_cores)
+            self.env_id in support_envs()
+        ), f"{self.env_id} doesn't exist. Please choose from {support_envs()}."
 
+    def _init_algo(self) -> None:
+        """Initialize the algorithm."""
         check_all_configs(self.cfgs, self.algo_type)
         device = self.cfgs.train_cfgs.device
         if device == 'cpu':
             torch.set_num_threads(self.cfgs.train_cfgs.torch_threads)
         else:
             torch.set_num_threads(1)
             torch.cuda.set_device(self.cfgs.train_cfgs.device)
         if distributed.fork(
             self.cfgs.train_cfgs.parallel,
-            use_number_of_threads=use_number_of_threads,
             device=self.cfgs.train_cfgs.device,
         ):
-            # Re-launches the current script with workers linked by MPI
+            # re-launches the current script with workers linked by MPI
             sys.exit()
-        self.agent = registry.get(self.algo)(
+        self.agent: BaseAlgo = registry.get(self.algo)(
             env_id=self.env_id,
             cfgs=self.cfgs,
         )
+
+    def learn(self) -> tuple[float, float, int]:
+        """Agent learning.
+
+        Returns:
+            ep_ret: The episode return of the final episode.
+            ep_cost: The episode cost of the final episode.
+            ep_len: The episode length of the final episode.
+        """
         ep_ret, ep_cost, ep_len = self.agent.learn()
 
         self._init_statistical_tools()
 
-        return ep_ret, ep_len, ep_cost
+        return ep_ret, ep_cost, ep_len
 
-    def _init_statistical_tools(self):
-        """Init statistical tools."""
+    def _init_statistical_tools(self) -> None:
+        """Initialize statistical tools."""
         self._evaluator = Evaluator()
         self._plotter = Plotter()
 
-    def plot(self, smooth=1):
+    def plot(self, smooth: int = 1) -> None:
         """Plot the training curve.
 
         Args:
-            smooth (int): window size, for smoothing the curve.
+            smooth (int, optional): window size, for smoothing the curve. Defaults to 1.
+
+        Raises:
+            AssertionError: If the :meth:`learn` method has not been called.
         """
         assert self._plotter is not None, 'Please run learn() first!'
         self._plotter.make_plots(
             [self.agent.logger.log_dir],
             None,
             'Steps',
             'Rewards',
@@ -174,51 +200,62 @@
             smooth,
             None,
             None,
             'mean',
             self.agent.logger.log_dir,
         )
 
-    def evaluate(self, num_episodes: int = 10, cost_criteria: float = 1.0):
+    def evaluate(self, num_episodes: int = 10, cost_criteria: float = 1.0) -> None:
         """Agent Evaluation.
 
         Args:
-            num_episodes (int): number of episodes to evaluate.
-            cost_criteria (float): the cost criteria to evaluate.
+            num_episodes (int, optional): number of episodes to evaluate. Defaults to 10.
+            cost_criteria (float, optional): the cost criteria to evaluate. Defaults to 1.0.
+
+        Raises:
+            AssertionError: If the :meth:`learn` method has not been called.
         """
         assert self._evaluator is not None, 'Please run learn() first!'
-        for item in os.scandir(os.path.join(self.agent.logger.log_dir, 'torch_save')):
+        scan_dir = os.scandir(os.path.join(self.agent.logger.log_dir, 'torch_save'))
+        for item in scan_dir:
             if item.is_file() and item.name.split('.')[-1] == 'pt':
                 self._evaluator.load_saved(save_dir=self.agent.logger.log_dir, model_name=item.name)
                 self._evaluator.evaluate(num_episodes=num_episodes, cost_criteria=cost_criteria)
+        scan_dir.close()
 
     # pylint: disable-next=too-many-arguments
     def render(
         self,
         num_episodes: int = 10,
         render_mode: str = 'rgb_array',
         camera_name: str = 'track',
         width: int = 256,
         height: int = 256,
-    ):
+    ) -> None:
         """Evaluate and render some episodes.
 
         Args:
-            num_episodes (int): number of episodes to render.
-            render_mode (str): render mode, can be 'rgb_array', 'depth_array' or 'human'.
-            camera_name (str): camera name, specify the camera which you use to capture
-                images.
-            width (int): width of the rendered image.
-            height (int): height of the rendered image.
+            num_episodes (int, optional): The number of episodes to render. Defaults to 10.
+            render_mode (str, optional): The render mode, can be 'rgb_array', 'depth_array' or
+                'human'. Defaults to 'rgb_array'.
+            camera_name (str, optional): the camera name, specify the camera which you use to
+                capture images. Defaults to 'track'.
+            width (int, optional): The width of the rendered image. Defaults to 256.
+            height (int, optional): The height of the rendered image. Defaults to 256.
+
+        Raises:
+            AssertionError: If the :meth:`learn` method has not been called.
         """
         assert self._evaluator is not None, 'Please run learn() first!'
-        for item in os.scandir(os.path.join(self.agent.logger.log_dir, 'torch_save')):
+        scan_dir = os.scandir(os.path.join(self.agent.logger.log_dir, 'torch_save'))
+        for item in scan_dir:
             if item.is_file() and item.name.split('.')[-1] == 'pt':
                 self._evaluator.load_saved(
                     save_dir=self.agent.logger.log_dir,
                     model_name=item.name,
                     render_mode=render_mode,
                     camera_name=camera_name,
                     width=width,
                     height=height,
                 )
                 self._evaluator.render(num_episodes=num_episodes)
+        scan_dir.close()
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/base_algo.py` & `omnisafe-0.4.0/omnisafe/algorithms/base_algo.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,49 +16,53 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 import torch
 
+from omnisafe.common.logger import Logger
 from omnisafe.utils import distributed
 from omnisafe.utils.config import Config
-from omnisafe.utils.tools import seed_all
+from omnisafe.utils.tools import get_device, seed_all
 
 
 class BaseAlgo(ABC):  # pylint: disable=too-few-public-methods
     """Base class for all algorithms."""
 
+    _logger: Logger
+
     def __init__(self, env_id: str, cfgs: Config) -> None:
-        self._env_id = env_id
-        self._cfgs = cfgs
+        """Initialize an instance of :class:`BaseAlgo`."""
+        self._env_id: str = env_id
+        self._cfgs: Config = cfgs
 
         assert hasattr(cfgs, 'seed'), 'Please specify the seed in the config file.'
-        self._seed = int(cfgs.seed) + distributed.get_rank() * 1000
+        self._seed: int = int(cfgs.seed) + distributed.get_rank() * 1000
         seed_all(self._seed)
 
         assert hasattr(cfgs.train_cfgs, 'device'), 'Please specify the device in the config file.'
-        self._device = torch.device(self._cfgs.train_cfgs.device)
+        self._device: torch.device = get_device(self._cfgs.train_cfgs.device)
 
         distributed.setup_distributed()
 
         self._init_env()
         self._init_model()
 
         self._init()
 
         self._init_log()
 
     @property
-    def logger(self):
+    def logger(self) -> Logger:
         """Get the logger."""
         return self._logger  # pylint: disable=no-member
 
     @property
-    def cost_limit(self):
+    def cost_limit(self) -> float | None:
         """Get the cost limit."""
         return getattr(self._cfgs.algo_cfgs, '_cost_limit', None)
 
     @abstractmethod
     def _init(self) -> None:
         """Initialize the algorithm."""
 
@@ -71,9 +75,9 @@
         """Initialize the model."""
 
     @abstractmethod
     def _init_log(self) -> None:
         """Initialize the logger."""
 
     @abstractmethod
-    def learn(self) -> tuple[int | float, ...]:
+    def learn(self) -> tuple[float, float, int]:
         """Learn the policy."""
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/off_policy/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/off_policy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Off-policy algorithms."""
 
 from omnisafe.algorithms.off_policy.ddpg import DDPG
+from omnisafe.algorithms.off_policy.ddpg_lag import DDPGLag
 from omnisafe.algorithms.off_policy.sac import SAC
+from omnisafe.algorithms.off_policy.sac_lag import SACLag
 from omnisafe.algorithms.off_policy.td3 import TD3
+from omnisafe.algorithms.off_policy.td3_lag import TD3Lag
 
 
-__all__ = [
-    'DDPG',
-    'TD3',
-    'SAC',
-]
+__all__ = ['DDPG', 'TD3', 'SAC', 'DDPGLag', 'TD3Lag', 'SACLag']
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/off_policy/ddpg.py` & `omnisafe-0.4.0/omnisafe/algorithms/model_based/base/loop.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,339 +8,417 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of the Deep Deterministic Policy Gradient algorithm."""
+"""Implementation of the Learning Off-Policy with Online Planning algorithm."""
 
 from __future__ import annotations
 
-import time
 from typing import Any
 
 import torch
-from torch import nn
+from gymnasium.spaces import Box
+from torch import nn, optim
+from torch.nn.utils.clip_grad import clip_grad_norm_
 
-from omnisafe.adapter import OffPolicyAdapter
+from omnisafe.adapter import ModelBasedAdapter
 from omnisafe.algorithms import registry
-from omnisafe.algorithms.base_algo import BaseAlgo
-from omnisafe.common.buffer import VectorOffPolicyBuffer
-from omnisafe.common.logger import Logger
+from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
+from omnisafe.algorithms.model_based.base.pets import PETS
+from omnisafe.algorithms.model_based.planner.arc import ARCPlanner
+from omnisafe.common.buffer import OffPolicyBuffer
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
-from omnisafe.utils import distributed
 
 
 @registry.register
-# pylint: disable-next=too-many-instance-attributes,too-few-public-methods
-class DDPG(BaseAlgo):
-    """The Deep Deterministic Policy Gradient (DDPG) algorithm.
+# pylint: disable-next=too-many-instance-attributes, too-few-public-methods
+class LOOP(PETS):
+    """The Learning Off-Policy with Online Planning (LOOP) algorithm.
 
     References:
-
-        - Title: Continuous control with deep reinforcement learning
-        - Authors: Timothy P. Lillicrap, Jonathan J. Hunt, Alexander Pritzel, Nicolas Heess,
-        Tom Erez, Yuval Tassa, David Silver, Daan Wierstra.
-        - URL: `DDPG <https://arxiv.org/abs/1509.02971>`_
+        - Title: Learning Off-Policy with Online Planning
+        - Authors: Harshit Sikchi, Wenxuan Zhou, David Held.
+        - URL: `LOOP <https://arxiv.org/abs/2008.10066>`_
     """
 
-    def _init_env(self) -> None:
-        self._env = OffPolicyAdapter(
-            self._env_id,
-            self._cfgs.train_cfgs.vector_env_nums,
-            self._seed,
-            self._cfgs,
-        )
-        assert (self._cfgs.algo_cfgs.update_cycle) % (
-            distributed.world_size() * self._cfgs.train_cfgs.vector_env_nums
-        ) == 0, 'The number of steps per epoch is not divisible by the number of environments.'
-
-        assert (
-            int(self._cfgs.train_cfgs.total_steps) % self._cfgs.algo_cfgs.update_cycle == 0
-        ), 'The total number of steps is not divisible by the number of steps per epoch.'
-        self._epochs = int(self._cfgs.train_cfgs.total_steps // self._cfgs.algo_cfgs.update_cycle)
-        self._epoch = 0
-        self._update_cycle = self._cfgs.algo_cfgs.update_cycle // (
-            distributed.world_size() * self._cfgs.train_cfgs.vector_env_nums
-        )
-        self._steps_per_sample = self._cfgs.algo_cfgs.steps_per_sample
-        assert (
-            self._update_cycle % self._steps_per_sample == 0
-        ), 'The number of steps per epoch is not divisible by the number of steps per sample.'
-        self._samples_per_epoch = self._update_cycle // self._steps_per_sample
-
     def _init_model(self) -> None:
-        self._cfgs.model_cfgs.critic['num_critics'] = 1
+        """Initialize the dynamics model and the planner."""
+        self._dynamics_state_space = (
+            self._env.coordinate_observation_space
+            if self._env.coordinate_observation_space is not None
+            else self._env.observation_space
+        )
+        assert self._env.action_space is not None and isinstance(
+            self._env.action_space.shape,
+            tuple,
+        )
+        if isinstance(self._env.action_space, Box):
+            self._action_space = self._env.action_space
+        else:
+            raise NotImplementedError
         self._actor_critic = ConstraintActorQCritic(
-            obs_space=self._env.observation_space,
+            obs_space=self._dynamics_state_space,
             act_space=self._env.action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._epochs,
         ).to(self._device)
-
-        if distributed.world_size() > 1:
-            distributed.sync_params(self._actor_critic)
+        self._use_actor_critic = True
+        self._update_count = 0
+        self._dynamics = EnsembleDynamicsModel(
+            model_cfgs=self._cfgs.dynamics_cfgs,
+            device=self._device,
+            state_shape=self._dynamics_state_space.shape,
+            action_shape=self._env.action_space.shape,
+            actor_critic=self._actor_critic,
+            rew_func=None,
+            cost_func=None,
+            terminal_func=None,
+        )
+        self._update_dynamics_cycle = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
+        self._planner = ARCPlanner(
+            dynamics=self._dynamics,
+            planner_cfgs=self._cfgs.planner_cfgs,
+            gamma=float(self._cfgs.algo_cfgs.gamma),
+            cost_gamma=float(self._cfgs.algo_cfgs.cost_gamma),
+            dynamics_state_shape=self._dynamics_state_space.shape,
+            action_shape=self._action_space.shape,
+            action_max=1.0,
+            action_min=-1.0,
+            device=self._device,
+            actor_critic=self._actor_critic,
+        )
 
     def _init(self) -> None:
-        self._buf = VectorOffPolicyBuffer(
-            obs_space=self._env.observation_space,
+        super()._init()
+        self._log_alpha: torch.Tensor
+        self._alpha_optimizer: optim.Optimizer
+        self._target_entropy: float
+
+        self._alpha = self._cfgs.algo_cfgs.alpha
+        self._alpha_gamma = self._cfgs.algo_cfgs.alpha_gamma
+        self._policy_buf = OffPolicyBuffer(
+            obs_space=self._dynamics_state_space,
             act_space=self._env.action_space,
-            size=self._cfgs.algo_cfgs.size,
-            batch_size=self._cfgs.algo_cfgs.batch_size,
-            num_envs=self._cfgs.train_cfgs.vector_env_nums,
+            size=self._cfgs.train_cfgs.total_steps,
+            batch_size=self._cfgs.algo_cfgs.policy_batch_size,
             device=self._device,
         )
 
-    def _init_log(self) -> None:
-        self._logger = Logger(
-            output_dir=self._cfgs.logger_cfgs.log_dir,
-            exp_name=self._cfgs.exp_name,
-            seed=self._cfgs.seed,
-            use_tensorboard=self._cfgs.logger_cfgs.use_tensorboard,
-            use_wandb=self._cfgs.logger_cfgs.use_wandb,
-            config=self._cfgs,
-        )
-
-        what_to_save: dict[str, Any] = {}
-        what_to_save['pi'] = self._actor_critic.actor
-        if self._cfgs.algo_cfgs.obs_normalize:
-            obs_normalizer = self._env.save()['obs_normalizer']
-            what_to_save['obs_normalizer'] = obs_normalizer
-
-        self._logger.setup_torch_saver(what_to_save)
-        self._logger.torch_save()
-
-        self._logger.register_key('Metrics/EpRet', window_length=50)
-        self._logger.register_key('Metrics/EpCost', window_length=50)
-        self._logger.register_key('Metrics/EpLen', window_length=50)
-
-        self._logger.register_key('Train/Epoch')
-        self._logger.register_key('Train/LR')
-
-        self._logger.register_key('TotalEnvSteps')
+    def _alpha_discount(self) -> None:
+        """Alpha discount."""
+        self._alpha *= self._alpha_gamma
 
+    def _init_log(self) -> None:
+        """Initialize logger."""
+        super()._init_log()
+        self._logger.register_key('Value/alpha')
         # log information about actor
         self._logger.register_key('Loss/Loss_pi', delta=True)
 
         # log information about critic
         self._logger.register_key('Loss/Loss_reward_critic', delta=True)
         self._logger.register_key('Value/reward_critic')
 
         if self._cfgs.algo_cfgs.use_cost:
             # log information about cost critic
             self._logger.register_key('Loss/Loss_cost_critic', delta=True)
             self._logger.register_key('Value/cost_critic')
 
-        self._logger.register_key('Time/Total')
-        self._logger.register_key('Time/Rollout')
-        self._logger.register_key('Time/Update')
-        self._logger.register_key('Time/Epoch')
-        self._logger.register_key('Time/FPS')
-
-    def _update_epoch(self) -> None:
-        """Update something per epoch"""
-        self._actor_critic.actor_scheduler.step()
-
-    def learn(self) -> tuple[int | float, ...]:
-        """This is main function for algorithm update, divided into the following steps:
-
-        - :meth:`rollout`: collect interactive data from environment.
-        - :meth:`update`: perform actor/critic updates.
-        - :meth:`log`: epoch/update information for visualization and terminal log print.
+    def _save_model(self) -> None:
+        """Save the model."""
+        what_to_save: dict[str, Any] = {}
+        # set up model saving
+        what_to_save = {
+            'dynamics': self._dynamics.ensemble_model,
+            'actor_critic': self._actor_critic,
+        }
+        if self._cfgs.algo_cfgs.obs_normalize:
+            obs_normalizer = self._env.save()['obs_normalizer']
+            what_to_save['obs_normalizer'] = obs_normalizer
+        self._logger.setup_torch_saver(what_to_save)
+        self._logger.torch_save()
+
+    def _select_action(  # pylint: disable=unused-argument
+        self,
+        current_step: int,
+        state: torch.Tensor,
+        env: ModelBasedAdapter,
+    ) -> tuple[torch.Tensor, dict]:
+        """Select action.
+
+        Args:
+            current_step (int): current step
+            state (torch.Tensor): current state
+            env (ModelBasedAdapter): environment
+
+        Returns:
+            action (torch.Tensor): action
+            action_info (dict): action information
         """
-        self._logger.log('INFO: Start training')
-        start_time = time.time()
-        for epoch in range(self._epochs):
-            roll_out_time = 0.0
-            update_time = 0.0
-            epoch_time = time.time()
-
-            for sample_step in range(
-                epoch * self._samples_per_epoch,
-                (epoch + 1) * self._samples_per_epoch,
-            ):
-                step = sample_step * self._steps_per_sample * self._cfgs.train_cfgs.vector_env_nums
-
-                roll_out_start = time.time()
-                # set noise for exploration
-                if self._cfgs.algo_cfgs.use_exploration_noise:
-                    self._actor_critic.actor.noise = self._cfgs.algo_cfgs.exploration_noise
-
-                # collect data from environment
-                self._env.roll_out(
-                    roll_out_step=self._steps_per_sample,
-                    agent=self._actor_critic,
-                    buffer=self._buf,
-                    logger=self._logger,
-                    use_rand_action=(step <= self._cfgs.algo_cfgs.start_learning_steps),
-                )
-                roll_out_time += time.time() - roll_out_start
+        if current_step < self._cfgs.algo_cfgs.start_learning_steps:
+            action = torch.tensor(self._env.action_space.sample()).to(self._device).unsqueeze(0)
+        else:
+            action, info = self._planner.output_action(state)
+            self._logger.store(**info)
+
+        assert action.shape == torch.Size(
+            [1, *self._action_space.shape],
+        ), 'action shape should be [batch_size, action_dim]'
+        info = {}
+        return action, info
 
-                # update parameters
-                update_start = time.time()
-                if step > self._cfgs.algo_cfgs.start_learning_steps:
-                    self._update()
-                # if we haven't updated the network, log 0 for the loss
-                else:
-                    self._log_when_not_update()
-                update_time += time.time() - update_start
-
-            self._logger.store(**{'Time/Update': update_time})
-            self._logger.store(**{'Time/Rollout': roll_out_time})
-
-            if step > self._cfgs.algo_cfgs.start_learning_steps:
-                # update something per epoch
-                # e.g. update lagrange multiplier
-                self._update_epoch()
-
-            self._logger.store(
-                **{
-                    'TotalEnvSteps': step,
-                    'Time/FPS': self._cfgs.algo_cfgs.update_cycle / (time.time() - epoch_time),
-                    'Time/Total': (time.time() - start_time),
-                    'Time/Epoch': (time.time() - epoch_time),
-                    'Train/Epoch': epoch,
-                    'Train/LR': self._actor_critic.actor_scheduler.get_last_lr()[0],
-                },
-            )
+    def _update_policy(self, current_step: int) -> None:
+        """Update policy.
 
-            self._logger.dump_tabular()
+        Args:
+            current_step (int): current step
+        """
+        if current_step >= self._cfgs.algo_cfgs.start_learning_steps:
+            for _step in range(self._cfgs.algo_cfgs.update_policy_iters):
+                self._update_count += 1
+
+                data = self._policy_buf.sample_batch()
+                obs, act, reward, cost, done, next_obs = (
+                    data['obs'],
+                    data['act'],
+                    data['reward'],
+                    data['cost'],
+                    data['done'],
+                    data['next_obs'],
+                )
 
-            # save model to disk
-            if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0:
-                self._logger.torch_save()
-
-        ep_ret = self._logger.get_stats('Metrics/EpRet')[0]
-        ep_cost = self._logger.get_stats('Metrics/EpCost')[0]
-        ep_len = self._logger.get_stats('Metrics/EpLen')[0]
-        self._logger.close()
-
-        return ep_ret, ep_cost, ep_len
-
-    def _update(self) -> None:
-        for step in range(self._steps_per_sample // self._cfgs.algo_cfgs.update_iters):
-            data = self._buf.sample_batch()
-            obs, act, reward, cost, done, next_obs = (
-                data['obs'],
-                data['act'],
-                data['reward'],
-                data['cost'],
-                data['done'],
-                data['next_obs'],
-            )
+                self._update_reward_critic(obs, act, reward, done, next_obs)
+                if self._cfgs.algo_cfgs.use_cost:
+                    self._update_cost_critic(obs, act, cost, done, next_obs)
+
+                if self._update_count % self._cfgs.algo_cfgs.policy_delay == 0:
+                    # freeze Q-network so you don't waste computational effort
+                    # computing gradients for it during the policy learning step
+                    for param in self._actor_critic.reward_critic.parameters():
+                        param.requires_grad = False
+                    if self._cfgs.algo_cfgs.use_cost:
+                        for param in self._actor_critic.cost_critic.parameters():
+                            param.requires_grad = False
+
+                    self._update_actor(obs)
+
+                    # unfreeze Q-network so you can optimize it at next DDPG step.
+                    for param in self._actor_critic.reward_critic.parameters():
+                        param.requires_grad = True
+                    if self._cfgs.algo_cfgs.use_cost:
+                        for param in self._actor_critic.cost_critic.parameters():
+                            param.requires_grad = True
 
-            self._update_rewrad_critic(obs, act, reward, done, next_obs)
-            if self._cfgs.algo_cfgs.use_cost:
-                self._update_cost_critic(obs, act, cost, done, next_obs)
+                    self._actor_critic.polyak_update(self._cfgs.algo_cfgs.polyak)
 
-            if step % self._cfgs.algo_cfgs.policy_delay == 0:
-                self._update_actor(obs)
+                if self._cfgs.algo_cfgs.alpha_discount:
+                    self._alpha_discount()
 
-            self._actor_critic.polyak_update(self._cfgs.algo_cfgs.polyak)
+    def _store_real_data(  # pylint: disable=too-many-arguments,unused-argument
+        self,
+        current_step: int,
+        ep_len: int,
+        state: torch.Tensor,
+        action: torch.Tensor,
+        reward: torch.Tensor,
+        cost: torch.Tensor,
+        terminated: torch.Tensor,
+        truncated: torch.Tensor,
+        next_state: torch.Tensor,
+        info: dict,
+        action_info: dict,
+    ) -> None:  # pylint: disable=too-many-arguments
+        """Store real data in buffer.
+
+        Args:
+            current_step (int): current step
+            ep_len (int): episode length
+            state (torch.Tensor): current state
+            action (torch.Tensor): action
+            reward (torch.Tensor): reward
+            cost (torch.Tensor): cost
+            terminated (torch.Tensor): terminated
+            truncated (torch.Tensor): truncated
+            next_state (torch.Tensor): next state
+            info (dict): information
+            action_info (dict): action information
+        """
+        done = terminated or truncated
+        goal_met = False if 'goal_met' not in info.keys() else info['goal_met']
+        if not done and not goal_met:
+            # when goal_met == true:
+            # current goal position is not related to the last goal position,
+            # this huge transition will confuse the dynamics model.
+            self._dynamics_buf.store(
+                obs=state,
+                act=action,
+                reward=reward,
+                cost=cost,
+                next_obs=next_state,
+                done=done,
+            )
+        if (done and self._cfgs.algo_cfgs.policy_store_done) or (not done and not goal_met):
+            self._policy_buf.store(
+                obs=state,
+                act=action,
+                reward=reward,
+                cost=cost,
+                next_obs=next_state,
+                done=done,
+            )
 
-    def _update_rewrad_critic(
+    def _update_reward_critic(
         self,
         obs: torch.Tensor,
         action: torch.Tensor,
         reward: torch.Tensor,
         done: torch.Tensor,
         next_obs: torch.Tensor,
     ) -> None:
+        """Update reward critic using Soft Actor-Critic.
+
+        Args:
+            obs (torch.Tensor): observation
+            action (torch.Tensor): action
+            reward (torch.Tensor): reward
+            done (torch.Tensor): done
+            next_obs (torch.Tensor): next observation
+        """
+        self._actor_critic.reward_critic_optimizer.zero_grad()
+
         with torch.no_grad():
-            next_action = self._actor_critic.actor.predict(next_obs, deterministic=True)
-            next_q_value_r = self._actor_critic.target_reward_critic(next_obs, next_action)[0]
+            next_action = self._actor_critic.actor.predict(next_obs, deterministic=False)
+            next_logp = self._actor_critic.actor.log_prob(next_action)
+            next_q1_value_r, next_q2_value_r = self._actor_critic.target_reward_critic(
+                next_obs,
+                next_action,
+            )
+            next_q_value_r = torch.min(next_q1_value_r, next_q2_value_r) - next_logp * self._alpha
             target_q_value_r = reward + self._cfgs.algo_cfgs.gamma * (1 - done) * next_q_value_r
-        q_value_r = self._actor_critic.reward_critic(obs, action)[0]
-        loss = nn.functional.mse_loss(q_value_r, target_q_value_r)
 
+        q1_value_r, q2_value_r = self._actor_critic.reward_critic(obs, action)
+        loss = nn.functional.mse_loss(q1_value_r, target_q_value_r) + nn.functional.mse_loss(
+            q2_value_r,
+            target_q_value_r,
+        )
         if self._cfgs.algo_cfgs.use_critic_norm:
             for param in self._actor_critic.reward_critic.parameters():
                 loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coeff
-        self._logger.store(
-            **{
-                'Loss/Loss_reward_critic': loss.mean().item(),
-                'Value/reward_critic': q_value_r.mean().item(),
-            },
-        )
-        self._actor_critic.reward_critic_optimizer.zero_grad()
         loss.backward()
 
-        if self._cfgs.algo_cfgs.max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+        if self._cfgs.algo_cfgs.use_grad_norm:
+            clip_grad_norm_(
                 self._actor_critic.reward_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
-        distributed.avg_grads(self._actor_critic.reward_critic)
         self._actor_critic.reward_critic_optimizer.step()
+        self._logger.store(
+            **{
+                'Loss/Loss_reward_critic': loss.mean().item(),
+                'Value/reward_critic': q1_value_r.mean().item(),
+            },
+        )
 
     def _update_cost_critic(
         self,
         obs: torch.Tensor,
         action: torch.Tensor,
         cost: torch.Tensor,
         done: torch.Tensor,
         next_obs: torch.Tensor,
     ) -> None:
+        """Update cost critic using TD3 algorithm.
+
+        Args:
+            obs (torch.Tensor): current observation
+            action (torch.Tensor): current action
+            cost (torch.Tensor): current cost
+            done (torch.Tensor): current done signal
+            next_obs (torch.Tensor): next observation
+        """
         with torch.no_grad():
             next_action = self._actor_critic.actor.predict(next_obs, deterministic=True)
             next_q_value_c = self._actor_critic.target_cost_critic(next_obs, next_action)[0]
             target_q_value_c = cost + self._cfgs.algo_cfgs.gamma * (1 - done) * next_q_value_c
         q_value_c = self._actor_critic.cost_critic(obs, action)[0]
         loss = nn.functional.mse_loss(q_value_c, target_q_value_c)
 
         if self._cfgs.algo_cfgs.use_critic_norm:
             for param in self._actor_critic.cost_critic.parameters():
                 loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coeff
 
         self._actor_critic.cost_critic_optimizer.zero_grad()
         loss.backward()
 
-        if self._cfgs.algo_cfgs.max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+        if self._cfgs.algo_cfgs.use_grad_norm:
+            clip_grad_norm_(
                 self._actor_critic.cost_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
-        distributed.avg_grads(self._actor_critic.cost_critic)
         self._actor_critic.cost_critic_optimizer.step()
 
         self._logger.store(
             **{
                 'Loss/Loss_cost_critic': loss.mean().item(),
                 'Value/cost_critic': q_value_c.mean().item(),
             },
         )
 
-    def _update_actor(  # pylint: disable=too-many-arguments
+    def _update_actor(
         self,
         obs: torch.Tensor,
     ) -> None:
-        loss = self._loss_pi(obs)
+        """Update actor using Soft Actor-Critic algorithm.
+
+        Args:
+            obs (torch.Tensor): observation
+        """
         self._actor_critic.actor_optimizer.zero_grad()
+        loss = self._loss_pi(obs)
         loss.backward()
-        if self._cfgs.algo_cfgs.max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+        if self._cfgs.algo_cfgs.use_grad_norm:
+            clip_grad_norm_(
                 self._actor_critic.actor.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
         self._actor_critic.actor_optimizer.step()
         self._logger.store(
             **{
                 'Loss/Loss_pi': loss.mean().item(),
             },
         )
 
+        self._logger.store(
+            **{
+                'Value/alpha': self._alpha,
+            },
+        )
+
     def _loss_pi(
         self,
         obs: torch.Tensor,
     ) -> torch.Tensor:
-        action = self._actor_critic.actor.predict(obs, deterministic=True)
-        return -self._actor_critic.reward_critic(obs, action)[0].mean()
+        """Compute loss for actor using Soft Actor-Critic algorithm.
+
+        Args:
+            obs (torch.Tensor): observation
+        """
+        action = self._actor_critic.actor.predict(
+            obs,
+            deterministic=self._cfgs.algo_cfgs.loss_pi_deterministic,
+        )
+        log_prob = self._actor_critic.actor.log_prob(action)
+        q1_value_r, q2_value_r = self._actor_critic.reward_critic(obs, action)
+        return (self._alpha * log_prob - torch.min(q1_value_r, q2_value_r)).mean()
 
     def _log_when_not_update(self) -> None:
+        """Log when not update."""
         self._logger.store(
             **{
                 'Loss/Loss_reward_critic': 0.0,
                 'Loss/Loss_pi': 0.0,
                 'Value/reward_critic': 0.0,
             },
         )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/off_policy/sac.py` & `omnisafe-0.4.0/omnisafe/algorithms/off_policy/sac.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,59 +10,81 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the Soft Actor-Critic algorithm."""
 
-
 import torch
 from torch import nn, optim
+from torch.nn.utils.clip_grad import clip_grad_norm_
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.off_policy.ddpg import DDPG
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
 from omnisafe.utils import distributed
-from omnisafe.utils.config import Config
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes,too-few-public-methods
 class SAC(DDPG):
     """The Soft Actor-Critic (SAC) algorithm.
 
     References:
         - Title: Soft Actor-Critic: Off-Policy Maximum Entropy Deep Reinforcement Learning with a Stochastic Actor
         - Authors: Tuomas Haarnoja, Aurick Zhou, Pieter Abbeel, Sergey Levine.
         - URL: `SAC <https://arxiv.org/abs/1801.01290>`_
     """
 
-    def __init__(self, env_id: str, cfgs: Config) -> None:
-        super().__init__(env_id, cfgs)
-        self._log_alpha: torch.Tensor
-        self._alpha_optimizer: optim.Optimizer
-        self._target_entropy: float
+    _log_alpha: torch.Tensor
+    _alpha_optimizer: optim.Optimizer
+    _target_entropy: float
 
     def _init_model(self) -> None:
+        """Initialize the model.
+
+        OmniSafe uses :class:`omnisafe.models.actor_critic.constraint_actor_q_critic.ConstraintActorQCritic`
+        as the default model.
+
+        User can customize the model by inheriting this method.
+
+        .. note::
+            The ``num_critics`` in ``critic`` configuration must be 2.
+
+        Examples:
+            >>> def _init_model(self) -> None:
+            ...     self._actor_critic = CustomActorQCritic()
+        """
         self._cfgs.model_cfgs.critic['num_critics'] = 2
         self._actor_critic = ConstraintActorQCritic(
             obs_space=self._env.observation_space,
             act_space=self._env.action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._epochs,
         ).to(self._device)
 
-        if distributed.world_size() > 1:
-            distributed.sync_params(self._actor_critic)
-
     def _init(self) -> None:
+        """The initialization of the algorithm.
+
+        User can define the initialization of the algorithm by inheriting this method.
+
+        Examples:
+            >>> def _init(self) -> None:
+            ...     super()._init()
+            ...     self._buffer = CustomBuffer()
+            ...     self._model = CustomModel()
+
+        In SAC, we need to initialize the ``log_alpha`` and ``alpha_optimizer``.
+        """
         super()._init()
         if self._cfgs.algo_cfgs.auto_alpha:
             self._target_entropy = -torch.prod(torch.Tensor(self._env.action_space.shape)).item()
             self._log_alpha = torch.zeros(1, requires_grad=True, device=self._device)
+
+            assert self._cfgs.model_cfgs.critic.lr is not None
             self._alpha_optimizer = optim.Adam(
                 [self._log_alpha],
                 lr=self._cfgs.model_cfgs.critic.lr,
             )
         else:
             self._log_alpha = torch.log(
                 torch.tensor(self._cfgs.algo_cfgs.alpha, device=self._device),
@@ -72,24 +94,40 @@
         super()._init_log()
         self._logger.register_key('Value/alpha')
         if self._cfgs.algo_cfgs.auto_alpha:
             self._logger.register_key('Loss/alpha_loss')
 
     @property
     def _alpha(self) -> float:
+        """The value of alpha."""
         return self._log_alpha.exp().item()
 
-    def _update_rewrad_critic(
+    def _update_reward_critic(
         self,
         obs: torch.Tensor,
         action: torch.Tensor,
         reward: torch.Tensor,
         done: torch.Tensor,
         next_obs: torch.Tensor,
     ) -> None:
+        """Update reward critic.
+
+        - Sample the target action by target actor.
+        - Get the target Q value by target critic.
+        - Use the minimum target Q value to update reward critic.
+        - Add the entropy loss to reward critic.
+        - Log useful information.
+
+        Args:
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            action (torch.Tensor): The ``action`` sampled from buffer.
+            reward (torch.Tensor): The ``reward`` sampled from buffer.
+            done (torch.Tensor): The ``terminated`` sampled from buffer.
+            next_obs (torch.Tensor): The ``next observation`` sampled from buffer.
+        """
         with torch.no_grad():
             next_action = self._actor_critic.actor.predict(next_obs, deterministic=False)
             next_logp = self._actor_critic.actor.log_prob(next_action)
             next_q1_value_r, next_q2_value_r = self._actor_critic.target_reward_critic(
                 next_obs,
                 next_action,
             )
@@ -106,127 +144,91 @@
             for param in self._actor_critic.reward_critic.parameters():
                 loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coeff
 
         self._actor_critic.reward_critic_optimizer.zero_grad()
         loss.backward()
 
         if self._cfgs.algo_cfgs.max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+            clip_grad_norm_(
                 self._actor_critic.reward_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
         distributed.avg_grads(self._actor_critic.reward_critic)
         self._actor_critic.reward_critic_optimizer.step()
         self._logger.store(
-            **{
+            {
                 'Loss/Loss_reward_critic': loss.mean().item(),
                 'Value/reward_critic': q1_value_r.mean().item(),
             },
         )
 
     def _update_actor(
         self,
         obs: torch.Tensor,
     ) -> None:
+        """Update actor and alpha if ``auto_alpha`` is True.
+
+        Args:
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+        """
         super()._update_actor(obs)
 
         if self._cfgs.algo_cfgs.auto_alpha:
             with torch.no_grad():
                 action = self._actor_critic.actor.predict(obs, deterministic=False)
                 log_prob = self._actor_critic.actor.log_prob(action)
             alpha_loss = -self._log_alpha * (log_prob + self._target_entropy).mean()
 
             self._alpha_optimizer.zero_grad()
             alpha_loss.backward()
             self._alpha_optimizer.step()
             self._logger.store(
-                **{
+                {
                     'Loss/alpha_loss': alpha_loss.mean().item(),
                 },
             )
         self._logger.store(
-            **{
+            {
                 'Value/alpha': self._alpha,
             },
         )
 
-    def _update_cost_critic(
+    def _loss_pi(
         self,
         obs: torch.Tensor,
-        action: torch.Tensor,
-        cost: torch.Tensor,
-        done: torch.Tensor,
-        next_obs: torch.Tensor,
-    ) -> None:
-        """
-        Update cost critic using TD3 algorithm.
-
-        Args:
-            obs (torch.Tensor): current observation
-            act (torch.Tensor): current action
-            cost (torch.Tensor): current cost
-            done (torch.Tensor): current done signal
-            next_obs (torch.Tensor): next observation
+    ) -> torch.Tensor:
+        r"""Computing ``pi/actor`` loss.
 
-        Returns:
-            None
-        """
-        with torch.no_grad():
-            # set the update noise and noise clip.
-            next_action = self._actor_critic.actor.predict(next_obs, deterministic=False)
-            next_logp = self._actor_critic.actor.log_prob(next_action)
-            next_q1_value_c, next_q2_value_c = self._actor_critic.target_cost_critic(
-                next_obs,
-                next_action,
-            )
-            next_q_value_c = torch.max(next_q1_value_c, next_q2_value_c) - next_logp * self._alpha
-            target_q_value_c = cost + self._cfgs.algo_cfgs.gamma * (1 - done) * next_q_value_c
+        The loss function in SAC is defined as:
 
-        q1_value_c, q2_value_c = self._actor_critic.cost_critic(obs, action)
-        loss = nn.functional.mse_loss(q1_value_c, target_q_value_c) + nn.functional.mse_loss(
-            q2_value_c,
-            target_q_value_c,
-        )
+        .. math::
 
-        if self._cfgs.algo_cfgs.use_critic_norm:
-            for param in self._actor_critic.cost_critic.parameters():
-                loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coeff
+            L = -Q^V (s, \pi (s)) + \alpha \log \pi (s)
 
-        self._actor_critic.cost_critic_optimizer.zero_grad()
-        loss.backward()
+        where :math:`Q^V` is the min value of two reward critic networks, and :math:`\pi` is the
+        policy network, and :math:`\alpha` is the temperature parameter.
 
-        if self._cfgs.algo_cfgs.max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
-                self._actor_critic.cost_critic.parameters(),
-                self._cfgs.algo_cfgs.max_grad_norm,
-            )
-        distributed.avg_grads(self._actor_critic.cost_critic)
-        self._actor_critic.cost_critic_optimizer.step()
-        self._logger.store(
-            **{
-                'Loss/Loss_cost_critic': loss.mean().item(),
-                'Value/cost_critic': q1_value_c.mean().item(),
-            },
-        )
+        Args:
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
 
-    def _loss_pi(
-        self,
-        obs: torch.Tensor,
-    ) -> torch.Tensor:
+        Returns:
+            The loss of pi/actor.
+        """
         action = self._actor_critic.actor.predict(obs, deterministic=False)
         log_prob = self._actor_critic.actor.log_prob(action)
         q1_value_r, q2_value_r = self._actor_critic.reward_critic(obs, action)
         return (self._alpha * log_prob - torch.min(q1_value_r, q2_value_r)).mean()
 
     def _log_when_not_update(self) -> None:
+        """Log default value when not update."""
         super()._log_when_not_update()
         self._logger.store(
-            **{
+            {
                 'Value/alpha': self._alpha,
             },
         )
         if self._cfgs.algo_cfgs.auto_alpha:
             self._logger.store(
-                **{
+                {
                     'Loss/alpha_loss': 0.0,
                 },
             )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/off_policy/td3.py` & `omnisafe-0.4.0/omnisafe/algorithms/off_policy/td3.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the Twin Delayed DDPG algorithm."""
 
 import torch
 from torch import nn
+from torch.nn.utils.clip_grad import clip_grad_norm_
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.off_policy.ddpg import DDPG
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
 from omnisafe.utils import distributed
 
 
@@ -31,50 +32,71 @@
     References:
         - Title: Addressing Function Approximation Error in Actor-Critic Methods
         - Authors: Scott Fujimoto, Herke van Hoof, David Meger.
         - URL: `TD3 <https://arxiv.org/abs/1802.09477>`_
     """
 
     def _init_model(self) -> None:
+        """Initialize the model.
+
+        OmniSafe uses :class:`omnisafe.models.actor_critic.constraint_actor_q_critic.ConstraintActorQCritic`
+        as the default model.
+
+        User can customize the model by inheriting this method.
+
+        .. note::
+            The ``num_critics`` in ``critic`` configuration must be 2.
+
+        Examples:
+            >>> def _init_model(self) -> None:
+            ...     self._actor_critic = CustomActorQCritic()
+        """
         self._cfgs.model_cfgs.critic['num_critics'] = 2
         self._actor_critic = ConstraintActorQCritic(
             obs_space=self._env.observation_space,
             act_space=self._env.action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._epochs,
         ).to(self._device)
 
-        if distributed.world_size() > 1:
-            distributed.sync_params(self._actor_critic)
-
-    def _update_rewrad_critic(
+    def _update_reward_critic(
         self,
         obs: torch.Tensor,
         action: torch.Tensor,
         reward: torch.Tensor,
         done: torch.Tensor,
         next_obs: torch.Tensor,
     ) -> None:
-        """
-        Update reward critic using TD3 algorithm.
+        """Update reward critic.
 
-        Args:
-            obs (torch.Tensor): current observation
-            act (torch.Tensor): current action
-            reward (torch.Tensor): current reward
-            done (torch.Tensor): current done signal
-            next_obs (torch.Tensor): next observation
+        - Get the target action by target actor.
+        - Add noise to target action.
+        - Clip the noise.
+
+        - Get the target Q value by target critic.
+        - Use the minimum target Q value to update reward critic.
+        - Log useful information.
 
-        Returns:
-            None
+        Args:
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            action (torch.Tensor): The ``action`` sampled from buffer.
+            reward (torch.Tensor): The ``reward`` sampled from buffer.
+            done (torch.Tensor): The ``terminated`` sampled from buffer.
+            next_obs (torch.Tensor): The ``next observation`` sampled from buffer.
         """
         with torch.no_grad():
             # set the update noise and noise clip.
-            self._actor_critic.target_actor.noise = self._cfgs.algo_cfgs.policy_noise
-            next_action = self._actor_critic.target_actor.predict(next_obs, deterministic=False)
+            next_action = self._actor_critic.target_actor.predict(next_obs, deterministic=True)
+            policy_noise = self._cfgs.algo_cfgs.policy_noise
+            policy_noise_clip = self._cfgs.algo_cfgs.policy_noise_clip
+            noise = (torch.randn_like(next_action) * policy_noise).clamp(
+                -policy_noise_clip,
+                policy_noise_clip,
+            )
+            next_action = (next_action + noise).clamp(-1.0, 1.0)
             next_q1_value_r, next_q2_value_r = self._actor_critic.target_reward_critic(
                 next_obs,
                 next_action,
             )
             next_q_value_r = torch.min(next_q1_value_r, next_q2_value_r)
             target_q_value_r = reward + self._cfgs.algo_cfgs.gamma * (1 - done) * next_q_value_r
 
@@ -88,78 +110,19 @@
             for param in self._actor_critic.reward_critic.parameters():
                 loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coeff
 
         self._actor_critic.reward_critic_optimizer.zero_grad()
         loss.backward()
 
         if self._cfgs.algo_cfgs.max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+            clip_grad_norm_(
                 self._actor_critic.reward_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
         distributed.avg_grads(self._actor_critic.reward_critic)
         self._actor_critic.reward_critic_optimizer.step()
         self._logger.store(
-            **{
+            {
                 'Loss/Loss_reward_critic': loss.mean().item(),
                 'Value/reward_critic': q1_value_r.mean().item(),
             },
         )
-
-    def _update_cost_critic(
-        self,
-        obs: torch.Tensor,
-        action: torch.Tensor,
-        cost: torch.Tensor,
-        done: torch.Tensor,
-        next_obs: torch.Tensor,
-    ) -> None:
-        """
-        Update cost critic using TD3 algorithm.
-
-        Args:
-            obs (torch.Tensor): current observation
-            act (torch.Tensor): current action
-            cost (torch.Tensor): current cost
-            done (torch.Tensor): current done signal
-            next_obs (torch.Tensor): next observation
-
-        Returns:
-            None
-        """
-        with torch.no_grad():
-            # Set the update noise and noise clip.
-            self._actor_critic.target_actor.noise = self._cfgs.algo_cfgs.policy_noise
-            next_action = self._actor_critic.target_actor.predict(next_obs, deterministic=False)
-            next_q1_value_c, next_q2_value_c = self._actor_critic.target_cost_critic(
-                next_obs,
-                next_action,
-            )
-            next_q_value_c = torch.max(next_q1_value_c, next_q2_value_c)
-            target_q_value_c = cost + self._cfgs.algo_cfgs.gamma * (1 - done) * next_q_value_c
-
-        q1_value_c, q2_value_c = self._actor_critic.cost_critic(obs, action)
-        loss = nn.functional.mse_loss(q1_value_c, target_q_value_c) + nn.functional.mse_loss(
-            q2_value_c,
-            target_q_value_c,
-        )
-
-        if self._cfgs.algo_cfgs.use_critic_norm:
-            for param in self._actor_critic.cost_critic.parameters():
-                loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coeff
-
-        self._actor_critic.cost_critic_optimizer.zero_grad()
-        loss.backward()
-
-        if self._cfgs.algo_cfgs.max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
-                self._actor_critic.cost_critic.parameters(),
-                self._cfgs.algo_cfgs.max_grad_norm,
-            )
-        distributed.avg_grads(self._actor_critic.cost_critic)
-        self._actor_critic.cost_critic_optimizer.step()
-        self._logger.store(
-            **{
-                'Loss/Loss_cost_critic': loss.mean().item(),
-                'Value/cost_critic': q1_value_c.mean().item(),
-            },
-        )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,45 +12,38 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """On-policy algorithms."""
 
 from omnisafe.algorithms.on_policy import (
     base,
+    early_terminated,
     first_order,
     naive_lagrange,
     penalty_function,
+    pid_lagrange,
+    saute,
     second_order,
+    simmer,
 )
 from omnisafe.algorithms.on_policy.base import PPO, TRPO, NaturalPG, PolicyGradient
-
-# from omnisafe.algorithms.on_policy.early_terminated import PPOEarlyTerminated, PPOLagEarlyTerminated
+from omnisafe.algorithms.on_policy.early_terminated import PPOEarlyTerminated, TRPOEarlyTerminated
 from omnisafe.algorithms.on_policy.first_order import CUP, FOCOPS
 from omnisafe.algorithms.on_policy.naive_lagrange import PDO, RCPO, OnCRPO, PPOLag, TRPOLag
 from omnisafe.algorithms.on_policy.penalty_function import IPO, P3O
-
-# from omnisafe.algorithms.on_policy.saute import PPOLagSaute, PPOSaute
+from omnisafe.algorithms.on_policy.pid_lagrange import CPPOPID, TRPOPID
+from omnisafe.algorithms.on_policy.saute import PPOSaute, TRPOSaute
 from omnisafe.algorithms.on_policy.second_order import CPO, PCPO
-
-
-# from omnisafe.algorithms.on_policy.pid_lagrange import CPPOPid, TRPOPid
-
-
-# from omnisafe.algorithms.on_policy.simmer import (
-#     PPOLagSimmerPid,
-#     PPOLagSimmerQ,
-#     PPOSimmerPid,
-#     PPOSimmerQ,
-# )
+from omnisafe.algorithms.on_policy.simmer import PPOSimmerPID, TRPOSimmerPID
 
 
 __all__ = [
     *base.__all__,
-    # *early_terminated.__all__,
+    *early_terminated.__all__,
     *first_order.__all__,
     *naive_lagrange.__all__,
     *penalty_function.__all__,
-    # *pid_lagrange.__all__,
-    # *saute.__all__,
+    *pid_lagrange.__all__,
+    *saute.__all__,
     *second_order.__all__,
-    # *simmer.__all__,
+    *simmer.__all__,
 ]
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/natural_pg.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/natural_pg.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,221 +16,215 @@
 
 import torch
 from torch.utils.data import DataLoader, TensorDataset
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.on_policy.base.policy_gradient import PolicyGradient
 from omnisafe.utils import distributed
-from omnisafe.utils.config import Config
 from omnisafe.utils.math import conjugate_gradients
 from omnisafe.utils.tools import (
     get_flat_gradients_from,
     get_flat_params_from,
     set_param_values_to_model,
 )
 
 
 @registry.register
 class NaturalPG(PolicyGradient):
     """The Natural Policy Gradient algorithm.
 
     The Natural Policy Gradient algorithm is a policy gradient algorithm that uses the
-    `Fisher information matrix <https://en.wikipedia.org/wiki/Fisher_information>`_ to
-    approximate the Hessian matrix. The Fisher information matrix is the second-order derivative of the KL-divergence.
+    `Fisher information matrix <https://en.wikipedia.org/wiki/Fisher_information>`_ to approximate
+    the Hessian matrix. The Fisher information matrix is the second-order derivative of the KL-divergence.
 
     References:
         - Title: A Natural Policy Gradient
         - Author: Sham Kakade.
         - URL: `Natural PG <https://proceedings.neurips.cc/paper/2001/file/4b86abe48d358ecf194c56c69108433e-Paper.pdf>`_
     """
 
-    def __init__(self, env_id: str, cfgs: Config) -> None:
-        super().__init__(env_id, cfgs)
-
-        self._fvp_obs: torch.Tensor
+    _fvp_obs: torch.Tensor
 
     def _init_log(self) -> None:
         r"""Log the Natural Policy Gradient specific information.
 
-        .. list-table::
-
-            *   -   Things to log
-                -   Description
-            *   -   ``Misc/AcceptanceStep``
-                -   The acceptance step size.
-            *   -   ``Misc/Alpha``
-                -   :math:`\frac{\delta_{KL}}{xHx}` in original paper.
-                    where :math:`x` is the step direction, :math:`H` is the Hessian matrix,
-                    and :math:`\delta_{KL}` is the target KL divergence.
-            *   -   ``Misc/FinalStepNorm``
-                -   The final step norm.
-            *   -   ``Misc/gradient_norm``
-                -   The gradient norm.
-            *   -   ``Misc/xHx``
-                -   :math:`xHx` in original paper.
-            *   -   ``Misc/H_inv_g``
-                -   :math:`H^{-1}g` in original paper.
-
-        Args:
-            epoch (int): current epoch.
+        +---------------------+--------------------------------------------------------+
+        | Things to log       | Description                                            |
+        +=====================+========================================================+
+        | Misc/AcceptanceStep | The acceptance step size.                              |
+        +---------------------+--------------------------------------------------------+
+        | Misc/Alpha          | :math:`\frac{\delta_{KL}}{xHx}` in the original paper. |
+        +---------------------+--------------------------------------------------------+
+        | Misc/FinalStepNorm  | The final step norm.                                   |
+        +---------------------+--------------------------------------------------------+
+        | Misc/gradient_norm  | The gradient norm.                                     |
+        +---------------------+--------------------------------------------------------+
+        | Misc/xHx            | :math:`x H x` in the original paper.                   |
+        +---------------------+--------------------------------------------------------+
+        | Misc/H_inv_g        | :math:`H^{-1} g` in the original paper.                |
+        +---------------------+--------------------------------------------------------+
         """
         super()._init_log()
 
         self._logger.register_key('Misc/Alpha')
         self._logger.register_key('Misc/FinalStepNorm')
         self._logger.register_key('Misc/gradient_norm')
         self._logger.register_key('Misc/xHx')
         self._logger.register_key('Misc/H_inv_g')
 
     def _fvp(self, params: torch.Tensor) -> torch.Tensor:
-        """Build the `Hessian-vector product <https://en.wikipedia.org/wiki/Hessian_matrix>`_
-        based on an approximation of the KL-divergence.
+        """Build the Hessian-vector product.
+
+        Build the `Hessian-vector product <https://en.wikipedia.org/wiki/Hessian_matrix>`_ , which
+        is the second-order derivative of the KL-divergence.
 
-        The Hessian-vector product is approximated by the Fisher information matrix,
-        which is the second-order derivative of the KL-divergence.
+        The Hessian-vector product is approximated by the Fisher information matrix, which is the
+        second-order derivative of the KL-divergence.
 
-        For details see John Schulman's PhD thesis (pp. 40) http://joschu.net/docs/thesis.pdf
+        For details see John Schulman's PhD thesis (pp. 40) http://joschu.net/docs/thesis.pdf .
 
         Args:
             params (torch.Tensor): The parameters of the actor network.
+
+        Returns:
+            The Fisher vector product.
         """
         self._actor_critic.actor.zero_grad()
         q_dist = self._actor_critic.actor(self._fvp_obs)
         with torch.no_grad():
             p_dist = self._actor_critic.actor(self._fvp_obs)
         kl = torch.distributions.kl.kl_divergence(p_dist, q_dist).mean()
 
-        grads = torch.autograd.grad(kl, self._actor_critic.actor.parameters(), create_graph=True)  # type: ignore
+        grads = torch.autograd.grad(
+            kl,
+            tuple(self._actor_critic.actor.parameters()),
+            create_graph=True,
+        )
         flat_grad_kl = torch.cat([grad.view(-1) for grad in grads])
 
         kl_p = (flat_grad_kl * params).sum()
-        grads = torch.autograd.grad(kl_p, self._actor_critic.actor.parameters(), retain_graph=False)  # type: ignore
+        grads = torch.autograd.grad(
+            kl_p,
+            tuple(self._actor_critic.actor.parameters()),
+            retain_graph=False,
+        )
 
         flat_grad_grad_kl = torch.cat([grad.contiguous().view(-1) for grad in grads])
         distributed.avg_tensor(flat_grad_grad_kl)
 
         self._logger.store(
-            **{
+            {
                 'Train/KL': kl.item(),
             },
         )
         return flat_grad_grad_kl + params * self._cfgs.algo_cfgs.cg_damping
 
     def _update_actor(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_r: torch.Tensor,
         adv_c: torch.Tensor,
     ) -> None:
-        """Update policy network.
+        r"""Update policy network.
 
         Natural Policy Gradient (NPG) update policy network using the conjugate gradient algorithm,
         following the steps:
 
         - Calculate the gradient of the policy network,
         - Use the conjugate gradient algorithm to calculate the step direction.
         - Update the policy network by taking a step in the step direction.
 
         Args:
             obs (torch.Tensor): The observation tensor.
             act (torch.Tensor): The action tensor.
-            log_p (torch.Tensor): The log probability of the action.
-            adv (torch.Tensor): The advantage tensor.
-            cost_adv (torch.Tensor): The cost advantage tensor.
+            logp (torch.Tensor): The log probability of the action.
+            adv_r (torch.Tensor): The reward advantage tensor.
+            adv_c (torch.Tensor): The cost advantage tensor.
+
+        Raises:
+            AssertionError: If :math:`x` is not finite.
+            AssertionError: If :math:`x H x` is not positive.
+            AssertionError: If :math:`\alpha` is not finite.
         """
         self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
         theta_old = get_flat_params_from(self._actor_critic.actor)
         self._actor_critic.actor.zero_grad()
         adv = self._compute_adv_surrogate(adv_r, adv_c)
-        loss, info = self._loss_pi(obs, act, logp, adv)
+        loss = self._loss_pi(obs, act, logp, adv)
 
         loss.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
-        grad = -get_flat_gradients_from(self._actor_critic.actor)
-        x = conjugate_gradients(self._fvp, grad, self._cfgs.algo_cfgs.cg_iters)
+        grads = -get_flat_gradients_from(self._actor_critic.actor)
+        x = conjugate_gradients(self._fvp, grads, self._cfgs.algo_cfgs.cg_iters)
         assert torch.isfinite(x).all(), 'x is not finite'
         xHx = torch.dot(x, self._fvp(x))
         assert xHx.item() >= 0, 'xHx is negative'
         alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
         step_direction = x * alpha
         assert torch.isfinite(step_direction).all(), 'step_direction is not finite'
 
         theta_new = theta_old + step_direction
         set_param_values_to_model(self._actor_critic.actor, theta_new)
 
         with torch.no_grad():
-            loss, info = self._loss_pi(obs, act, logp, adv)
+            loss = self._loss_pi(obs, act, logp, adv)
 
         self._logger.store(
-            **{
-                'Train/Entropy': info['entropy'],
-                'Train/PolicyRatio': info['ratio'],
-                'Train/PolicyStd': info['std'],
-                'Loss/Loss_pi': loss.mean().item(),
+            {
                 'Misc/Alpha': alpha.item(),
                 'Misc/FinalStepNorm': torch.norm(step_direction).mean().item(),
                 'Misc/xHx': xHx.item(),
-                'Misc/gradient_norm': torch.norm(grad).mean().item(),
+                'Misc/gradient_norm': torch.norm(grads).mean().item(),
                 'Misc/H_inv_g': x.norm().item(),
             },
         )
 
     def _update(self) -> None:
-        r"""Update actor, critic.
+        """Update actor, critic.
 
         .. hint::
-
-            Here are some differences between NPG and Policy Gradient (PG):
-            In PG, the actor network and the critic network are updated together.
-            When the KL divergence between the old policy,
-            and the new policy is larger than a threshold, the update is rejected together.
-
-            In NPG, the actor network and the critic network are updated separately.
-            When the KL divergence between the old policy,
-            and the new policy is larger than a threshold,
-            the update of the actor network is rejected,
-            but the update of the critic network is still accepted.
-
-        Args:
-            self (object): object of the class.
+            Here are some differences between NPG and Policy Gradient (PG): In PG, the actor network
+            and the critic network are updated together. When the KL divergence between the old
+            policy, and the new policy is larger than a threshold, the update is rejected together.
+
+            In NPG, the actor network and the critic network are updated separately. When the KL
+            divergence between the old policy, and the new policy is larger than a threshold, the
+            update of the actor network is rejected, but the update of the critic network is still
+            accepted.
         """
         data = self._buf.get()
         obs, act, logp, target_value_r, target_value_c, adv_r, adv_c = (
             data['obs'],
             data['act'],
             data['logp'],
             data['target_value_r'],
             data['target_value_c'],
             data['adv_r'],
             data['adv_c'],
         )
         self._update_actor(obs, act, logp, adv_r, adv_c)
 
         dataloader = DataLoader(
-            dataset=TensorDataset(obs, act, logp, target_value_r, target_value_c, adv_r, adv_c),
+            dataset=TensorDataset(obs, target_value_r, target_value_c),
             batch_size=self._cfgs.algo_cfgs.batch_size,
             shuffle=True,
         )
 
-        for _i in range(self._cfgs.algo_cfgs.update_iters):
+        for _ in range(self._cfgs.algo_cfgs.update_iters):
             for (
                 obs,
-                _act,
-                _logp,
                 target_value_r,
                 target_value_c,
-                _adv_r,
-                _adv_c,
             ) in dataloader:
                 self._update_reward_critic(obs, target_value_r)
                 if self._cfgs.algo_cfgs.use_cost:
                     self._update_cost_critic(obs, target_value_c)
 
         self._logger.store(
-            **{
-                'Train/StopIter': _i + 1,
+            {
+                'Train/StopIter': self._cfgs.algo_cfgs.update_iters,
                 'Value/Adv': adv_r.mean().item(),
             },
         )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/policy_gradient.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/policy_gradient.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import time
 from typing import Any
 
 import torch
 import torch.nn as nn
 from rich.progress import track
+from torch.nn.utils.clip_grad import clip_grad_norm_
 from torch.utils.data import DataLoader, TensorDataset
 
 from omnisafe.adapter import OnPolicyAdapter
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.base_algo import BaseAlgo
 from omnisafe.common.buffer import VectorOnPolicyBuffer
 from omnisafe.common.logger import Logger
@@ -43,50 +44,55 @@
         - Authors: Richard S. Sutton, David McAllester, Satinder Singh, Yishay Mansour.
         - URL: `PG <https://proceedings.neurips.cc/paper/1999/file64d828b85b0bed98e80ade0a5c43b0f-Paper.pdf>`_
     """
 
     def _init_env(self) -> None:
         """Initialize the environment.
 
-        Omnisafe use :class:`omnisafe.adapter.OnPolicyAdapter` to adapt the environment to the algorithm.
+        OmniSafe uses :class:`omnisafe.adapter.OnPolicyAdapter` to adapt the environment to the
+        algorithm.
 
-        User can customize the environment by inheriting this function.
+        User can customize the environment by inheriting this method.
 
-        Example:
+        Examples:
             >>> def _init_env(self) -> None:
-            >>>    self._env = CustomAdapter()
+            ...     self._env = CustomAdapter()
+
+        Raises:
+            AssertionError: If the number of steps per epoch is not divisible by the number of
+                environments.
         """
-        self._env = OnPolicyAdapter(
+        self._env: OnPolicyAdapter = OnPolicyAdapter(
             self._env_id,
             self._cfgs.train_cfgs.vector_env_nums,
             self._seed,
             self._cfgs,
         )
-        assert (self._cfgs.algo_cfgs.update_cycle) % (
+        assert (self._cfgs.algo_cfgs.steps_per_epoch) % (
             distributed.world_size() * self._cfgs.train_cfgs.vector_env_nums
         ) == 0, 'The number of steps per epoch is not divisible by the number of environments.'
-        self._steps_per_epoch = (
-            self._cfgs.algo_cfgs.update_cycle
+        self._steps_per_epoch: int = (
+            self._cfgs.algo_cfgs.steps_per_epoch
             // distributed.world_size()
             // self._cfgs.train_cfgs.vector_env_nums
         )
 
     def _init_model(self) -> None:
         """Initialize the model.
 
-        Omnisafe use :class:`omnisafe.models.actor_critic.constraint_actor_critic.
-        ConstraintActorCritic` as the default model.
+        OmniSafe uses :class:`omnisafe.models.actor_critic.constraint_actor_critic.ConstraintActorCritic`
+        as the default model.
 
-        User can customize the model by inheriting this function.
+        User can customize the model by inheriting this method.
 
-        Example:
+        Examples:
             >>> def _init_model(self) -> None:
-            >>>    self._actor_critic = CustomActorCritic()
+            ...     self._actor_critic = CustomActorCritic()
         """
-        self._actor_critic = ConstraintActorCritic(
+        self._actor_critic: ConstraintActorCritic = ConstraintActorCritic(
             obs_space=self._env.observation_space,
             act_space=self._env.action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._cfgs.train_cfgs.epochs,
         ).to(self._device)
 
         if distributed.world_size() > 1:
@@ -97,23 +103,23 @@
                 epochs=[0, self._cfgs.train_cfgs.epochs],
                 std=self._cfgs.model_cfgs.std_range,
             )
 
     def _init(self) -> None:
         """The initialization of the algorithm.
 
-        User can define the initialization of the algorithm by inheriting this function.
+        User can define the initialization of the algorithm by inheriting this method.
 
-        Example:
+        Examples:
             >>> def _init(self) -> None:
-            >>>    super()._init()
-            >>>    self._buffer = CustomBuffer()
-            >>>    self._model = CustomModel()
+            ...     super()._init()
+            ...     self._buffer = CustomBuffer()
+            ...     self._model = CustomModel()
         """
-        self._buf = VectorOnPolicyBuffer(
+        self._buf: VectorOnPolicyBuffer = VectorOnPolicyBuffer(
             obs_space=self._env.observation_space,
             act_space=self._env.action_space,
             size=self._steps_per_epoch,
             gamma=self._cfgs.algo_cfgs.gamma,
             lam=self._cfgs.algo_cfgs.lam,
             lam_c=self._cfgs.algo_cfgs.lam_c,
             advantage_estimator=self._cfgs.algo_cfgs.adv_estimation_method,
@@ -123,67 +129,51 @@
             num_envs=self._cfgs.train_cfgs.vector_env_nums,
             device=self._device,
         )
 
     def _init_log(self) -> None:
         """Log info about epoch.
 
-            .. list-table::
-
-                *   -   Things to log
-                    -   Description
-                *   -   Train/Epoch
-                    -   Current epoch.
-                *   -   Metrics/EpCost
-                    -   Average cost of the epoch.
-                *   -   Metrics/EpCost
-                    -   Average cost of the epoch.
-                *   -   Metrics/EpRet
-                    -   Average return of the epoch.
-                *   -   Metrics/EpLen
-                    -   Average length of the epoch.
-                *   -   Values/reward
-                    -   Average value in :meth:`roll_out()` (from critic network) of the epoch.
-                *   -   Values/cost
-                    -   Average cost in :meth:`roll_out()` (from critic network) of the epoch.
-                *   -   Values/Adv
-                    -   Average advantage in :meth:`roll_out()` of the epoch.
-                *   -   Loss/Loss_pi
-                    -   Loss of the policy network.
-                *   -   Loss/Delta_loss_pi
-                    -   Delta loss of the policy network.
-                *   -   Loss/Loss_reward_critic
-                    -   Loss of the value network.
-                *   -   Loss/Delta_loss_reward_critic
-                    -   Delta loss of the value network.
-                *   -   Loss/Loss_cost_critic
-                    -   Loss of the cost network.
-                *   -   Loss/Delta_loss_cost_critic
-                    -   Delta loss of the cost network.
-                *   -   Train/Entropy
-                    -   Entropy of the policy network.
-                *   -   Train/KL
-                    -   KL divergence of the policy network.
-                *   -   Train/StopIters
-                    -   Number of iterations of the policy network.
-                *   -   Train/PolicyRatio
-                    -   Ratio of the policy network.
-                *   -   Train/LR
-                    -   Learning rate of the policy network.
-                *   -   Misc/Seed
-                    -   Seed of the experiment.
-                *   -   Misc/TotalEnvSteps
-                    -   Total steps of the experiment.
-                *   -   Time
-                    -   Total time.
-                *   -   FPS
-                    -   Frames per second of the epoch.
-
-        Args:
-            epoch (int): current epoch.
+        +-----------------------+----------------------------------------------------------------------+
+        | Things to log         | Description                                                          |
+        +=======================+======================================================================+
+        | Train/Epoch           | Current epoch.                                                       |
+        +-----------------------+----------------------------------------------------------------------+
+        | Metrics/EpCost        | Average cost of the epoch.                                           |
+        +-----------------------+----------------------------------------------------------------------+
+        | Metrics/EpRet         | Average return of the epoch.                                         |
+        +-----------------------+----------------------------------------------------------------------+
+        | Metrics/EpLen         | Average length of the epoch.                                         |
+        +-----------------------+----------------------------------------------------------------------+
+        | Values/reward         | Average value in :meth:`rollout` (from critic network) of the epoch. |
+        +-----------------------+----------------------------------------------------------------------+
+        | Values/cost           | Average cost in :meth:`rollout` (from critic network) of the epoch.  |
+        +-----------------------+----------------------------------------------------------------------+
+        | Values/Adv            | Average reward advantage of the epoch.                               |
+        +-----------------------+----------------------------------------------------------------------+
+        | Loss/Loss_pi          | Loss of the policy network.                                          |
+        +-----------------------+----------------------------------------------------------------------+
+        | Loss/Loss_cost_critic | Loss of the cost critic network.                                     |
+        +-----------------------+----------------------------------------------------------------------+
+        | Train/Entropy         | Entropy of the policy network.                                       |
+        +-----------------------+----------------------------------------------------------------------+
+        | Train/StopIters       | Number of iterations of the policy network.                          |
+        +-----------------------+----------------------------------------------------------------------+
+        | Train/PolicyRatio     | Ratio of the policy network.                                         |
+        +-----------------------+----------------------------------------------------------------------+
+        | Train/LR              | Learning rate of the policy network.                                 |
+        +-----------------------+----------------------------------------------------------------------+
+        | Misc/Seed             | Seed of the experiment.                                              |
+        +-----------------------+----------------------------------------------------------------------+
+        | Misc/TotalEnvSteps    | Total steps of the experiment.                                       |
+        +-----------------------+----------------------------------------------------------------------+
+        | Time                  | Total time.                                                          |
+        +-----------------------+----------------------------------------------------------------------+
+        | FPS                   | Frames per second of the epoch.                                      |
+        +-----------------------+----------------------------------------------------------------------+
         """
         self._logger = Logger(
             output_dir=self._cfgs.logger_cfgs.log_dir,
             exp_name=self._cfgs.exp_name,
             seed=self._cfgs.seed,
             use_tensorboard=self._cfgs.logger_cfgs.use_tensorboard,
             use_wandb=self._cfgs.logger_cfgs.use_wandb,
@@ -202,15 +192,15 @@
         self._logger.register_key('Metrics/EpCost', window_length=50)
         self._logger.register_key('Metrics/EpLen', window_length=50)
 
         self._logger.register_key('Train/Epoch')
         self._logger.register_key('Train/Entropy')
         self._logger.register_key('Train/KL')
         self._logger.register_key('Train/StopIter')
-        self._logger.register_key('Train/PolicyRatio')
+        self._logger.register_key('Train/PolicyRatio', min_and_max=True)
         self._logger.register_key('Train/LR')
         if self._cfgs.model_cfgs.actor_type == 'gaussian_learning':
             self._logger.register_key('Train/PolicyStd')
 
         self._logger.register_key('TotalEnvSteps')
 
         # log information about actor
@@ -228,114 +218,115 @@
 
         self._logger.register_key('Time/Total')
         self._logger.register_key('Time/Rollout')
         self._logger.register_key('Time/Update')
         self._logger.register_key('Time/Epoch')
         self._logger.register_key('Time/FPS')
 
-    def learn(self) -> tuple[int | float, ...]:
-        r"""This is main function for algorithm update, divided into the following steps,
+    def learn(self) -> tuple[float, float, int]:
+        """This is main function for algorithm update.
+
+        It is divided into the following steps:
 
         - :meth:`rollout`: collect interactive data from environment.
         - :meth:`update`: perform actor/critic updates.
         - :meth:`log`: epoch/update information for visualization and terminal log print.
 
-        Args:
-            self (object): object of the class.
+        Returns:
+            ep_ret: average episode return in final epoch.
+            ep_cost: average episode cost in final epoch.
+            ep_len: average episode length in final epoch.
         """
         start_time = time.time()
         self._logger.log('INFO: Start training')
 
         for epoch in range(self._cfgs.train_cfgs.epochs):
             epoch_time = time.time()
 
-            roll_out_time = time.time()
-            self._env.roll_out(
+            rollout_time = time.time()
+            self._env.rollout(
                 steps_per_epoch=self._steps_per_epoch,
                 agent=self._actor_critic,
                 buffer=self._buf,
                 logger=self._logger,
             )
-            self._logger.store(**{'Time/Rollout': time.time() - roll_out_time})
+            self._logger.store({'Time/Rollout': time.time() - rollout_time})
 
             update_time = time.time()
             self._update()
-            self._logger.store(**{'Time/Update': time.time() - update_time})
+            self._logger.store({'Time/Update': time.time() - update_time})
 
             if self._cfgs.model_cfgs.exploration_noise_anneal:
                 self._actor_critic.annealing(epoch)
 
-            if self._cfgs.model_cfgs.actor.lr != 'None':
+            if self._cfgs.model_cfgs.actor.lr is not None:
                 self._actor_critic.actor_scheduler.step()
 
             self._logger.store(
-                **{
-                    'TotalEnvSteps': (epoch + 1) * self._cfgs.algo_cfgs.update_cycle,
-                    'Time/FPS': self._cfgs.algo_cfgs.update_cycle / (time.time() - epoch_time),
+                {
+                    'TotalEnvSteps': (epoch + 1) * self._cfgs.algo_cfgs.steps_per_epoch,
+                    'Time/FPS': self._cfgs.algo_cfgs.steps_per_epoch / (time.time() - epoch_time),
                     'Time/Total': (time.time() - start_time),
                     'Time/Epoch': (time.time() - epoch_time),
                     'Train/Epoch': epoch,
                     'Train/LR': 0.0
-                    if self._cfgs.model_cfgs.actor.lr == 'None'
+                    if self._cfgs.model_cfgs.actor.lr is None
                     else self._actor_critic.actor_scheduler.get_last_lr()[0],
                 },
             )
 
             self._logger.dump_tabular()
 
             # save model to disk
             if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0:
                 self._logger.torch_save()
 
         ep_ret = self._logger.get_stats('Metrics/EpRet')[0]
         ep_cost = self._logger.get_stats('Metrics/EpCost')[0]
-        ep_len = self._logger.get_stats('Metrics/EpLen')[0]
+        ep_len = int(self._logger.get_stats('Metrics/EpLen')[0])
         self._logger.close()
 
         return ep_ret, ep_cost, ep_len
 
     def _update(self) -> None:
-        r"""Update actor, critic, following next steps:
+        """Update actor, critic.
 
         -  Get the ``data`` from buffer
 
         .. hint::
 
-            .. list-table::
-
-                *   -   obs
-                    -   ``observaion`` stored in buffer.
-                *   -   act
-                    -   ``action`` stored in buffer.
-                *   -   target_value_r
-                    -   ``target value`` stored in buffer.
-                *   -   target_value_c
-                    -   ``target cost`` stored in buffer.
-                *   -   logp
-                    -   ``log probability`` stored in buffer.
-                *   -   adv
-                    -   ``estimated advantage`` (e.g. **GAE**) stored in buffer.
-                *   -   cost_adv
-                    -   ``estimated cost advantage`` (e.g. **GAE**) stored in buffer.
-
-        -  Update value net by :meth:`_update_reward_critic()`.
-        -  Update cost net by :meth:`_update_cost_critic()`.
-        -  Update policy net by :meth:`_update_actor()`.
+            +----------------+------------------------------------------------------------------+
+            | obs            | ``observation`` sampled from buffer.                             |
+            +================+==================================================================+
+            | act            | ``action`` sampled from buffer.                                  |
+            +----------------+------------------------------------------------------------------+
+            | target_value_r | ``target reward value`` sampled from buffer.                     |
+            +----------------+------------------------------------------------------------------+
+            | target_value_c | ``target cost value`` sampled from buffer.                       |
+            +----------------+------------------------------------------------------------------+
+            | logp           | ``log probability`` sampled from buffer.                         |
+            +----------------+------------------------------------------------------------------+
+            | adv_r          | ``estimated advantage`` (e.g. **GAE**) sampled from buffer.      |
+            +----------------+------------------------------------------------------------------+
+            | adv_c          | ``estimated cost advantage`` (e.g. **GAE**) sampled from buffer. |
+            +----------------+------------------------------------------------------------------+
+
+
+        -  Update value net by :meth:`_update_reward_critic`.
+        -  Update cost net by :meth:`_update_cost_critic`.
+        -  Update policy net by :meth:`_update_actor`.
 
         The basic process of each update is as follows:
 
         #. Get the data from buffer.
         #. Shuffle the data and split it into mini-batch data.
         #. Get the loss of network.
         #. Update the network by loss.
         #. Repeat steps 2, 3 until the number of mini-batch data is used up.
         #. Repeat steps 2, 3, 4 until the KL divergence violates the limit.
-
-        Args:
-            self (object): object of the class.
         """
         data = self._buf.get()
         obs, act, logp, target_value_r, target_value_c, adv_r, adv_c = (
             data['obs'],
             data['act'],
             data['logp'],
             data['target_value_r'],
@@ -349,14 +340,17 @@
 
         dataloader = DataLoader(
             dataset=TensorDataset(obs, act, logp, target_value_r, target_value_c, adv_r, adv_c),
             batch_size=self._cfgs.algo_cfgs.batch_size,
             shuffle=True,
         )
 
+        update_counts = 0
+        final_kl = torch.ones_like(old_distribution.loc)
+
         for i in track(range(self._cfgs.algo_cfgs.update_iters), description='Updating...'):
             for (
                 obs,
                 act,
                 logp,
                 target_value_r,
                 target_value_c,
@@ -374,195 +368,204 @@
                 torch.distributions.kl.kl_divergence(old_distribution, new_distribution)
                 .sum(-1, keepdim=True)
                 .mean()
                 .item()
             )
             kl = distributed.dist_avg(kl)
 
+            final_kl = kl
+            update_counts += 1
+
             if self._cfgs.algo_cfgs.kl_early_stop and kl > self._cfgs.algo_cfgs.target_kl:
                 self._logger.log(f'Early stopping at iter {i + 1} due to reaching max kl')
                 break
 
         self._logger.store(
-            **{
-                'Train/StopIter': i + 1,  # pylint: disable=undefined-loop-variable
+            {
+                'Train/StopIter': update_counts,  # pylint: disable=undefined-loop-variable
                 'Value/Adv': adv_r.mean().item(),
-                'Train/KL': kl,
+                'Train/KL': final_kl,
             },
         )
 
     def _update_reward_critic(self, obs: torch.Tensor, target_value_r: torch.Tensor) -> None:
         r"""Update value network under a double for loop.
 
         The loss function is ``MSE loss``, which is defined in ``torch.nn.MSELoss``.
         Specifically, the loss function is defined as:
 
         .. math::
+
             L = \frac{1}{N} \sum_{i=1}^N (\hat{V} - V)^2
 
         where :math:`\hat{V}` is the predicted cost and :math:`V` is the target cost.
 
         #. Compute the loss function.
         #. Add the ``critic norm`` to the loss function if ``use_critic_norm`` is ``True``.
         #. Clip the gradient if ``use_max_grad_norm`` is ``True``.
         #. Update the network by loss function.
 
         Args:
-            obs (torch.Tensor): ``observation`` stored in buffer.
-            target_value_r (torch.Tensor): ``target_value_r`` stored in buffer.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            target_value_r (torch.Tensor): The ``target_value_r`` sampled from buffer.
         """
         self._actor_critic.reward_critic_optimizer.zero_grad()
         loss = nn.functional.mse_loss(self._actor_critic.reward_critic(obs)[0], target_value_r)
 
         if self._cfgs.algo_cfgs.use_critic_norm:
             for param in self._actor_critic.reward_critic.parameters():
                 loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coef
 
         loss.backward()
 
         if self._cfgs.algo_cfgs.use_max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+            clip_grad_norm_(
                 self._actor_critic.reward_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
         distributed.avg_grads(self._actor_critic.reward_critic)
         self._actor_critic.reward_critic_optimizer.step()
 
-        self._logger.store(**{'Loss/Loss_reward_critic': loss.mean().item()})
+        self._logger.store({'Loss/Loss_reward_critic': loss.mean().item()})
 
     def _update_cost_critic(self, obs: torch.Tensor, target_value_c: torch.Tensor) -> None:
         r"""Update value network under a double for loop.
 
         The loss function is ``MSE loss``, which is defined in ``torch.nn.MSELoss``.
         Specifically, the loss function is defined as:
 
         .. math::
+
             L = \frac{1}{N} \sum_{i=1}^N (\hat{V} - V)^2
 
         where :math:`\hat{V}` is the predicted cost and :math:`V` is the target cost.
 
         #. Compute the loss function.
         #. Add the ``critic norm`` to the loss function if ``use_critic_norm`` is ``True``.
         #. Clip the gradient if ``use_max_grad_norm`` is ``True``.
         #. Update the network by loss function.
 
         Args:
-            obs (torch.Tensor): ``observation`` stored in buffer.
-            target_value_c (torch.Tensor): ``target_value_c`` stored in buffer.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            target_value_c (torch.Tensor): The ``target_value_c`` sampled from buffer.
         """
         self._actor_critic.cost_critic_optimizer.zero_grad()
         loss = nn.functional.mse_loss(self._actor_critic.cost_critic(obs)[0], target_value_c)
 
         if self._cfgs.algo_cfgs.use_critic_norm:
             for param in self._actor_critic.cost_critic.parameters():
                 loss += param.pow(2).sum() * self._cfgs.algo_cfgs.critic_norm_coef
 
         loss.backward()
 
         if self._cfgs.algo_cfgs.use_max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+            clip_grad_norm_(
                 self._actor_critic.cost_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
         distributed.avg_grads(self._actor_critic.cost_critic)
         self._actor_critic.cost_critic_optimizer.step()
 
-        self._logger.store(**{'Loss/Loss_cost_critic': loss.mean().item()})
+        self._logger.store({'Loss/Loss_cost_critic': loss.mean().item()})
 
     def _update_actor(  # pylint: disable=too-many-arguments
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_r: torch.Tensor,
         adv_c: torch.Tensor,
     ) -> None:
-        r"""Update policy network under a double for loop.
+        """Update policy network under a double for loop.
+
+        #. Compute the loss function.
+        #. Clip the gradient if ``use_max_grad_norm`` is ``True``.
+        #. Update the network by loss function.
 
-            #. Compute the loss function.
-            #. Clip the gradient if ``use_max_grad_norm`` is ``True``.
-            #. Update the network by loss function.
-
-            .. warning::
-
-                For some ``KL divergence`` based algorithms (e.g. TRPO, CPO, etc.),
-                the ``KL divergence`` between the old policy and the new policy is calculated.
-                And the ``KL divergence`` is used to determine whether the update is successful.
-                If the ``KL divergence`` is too large, the update will be terminated.
+        .. warning::
+            For some ``KL divergence`` based algorithms (e.g. TRPO, CPO, etc.),
+            the ``KL divergence`` between the old policy and the new policy is calculated.
+            And the ``KL divergence`` is used to determine whether the update is successful.
+            If the ``KL divergence`` is too large, the update will be terminated.
 
         Args:
-            obs (torch.Tensor): ``observation`` stored in buffer.
-            act (torch.Tensor): ``action`` stored in buffer.
-            log_p (torch.Tensor): ``log_p`` stored in buffer.
-            adv_r (torch.Tensor): ``advantage`` stored in buffer.
-            adv_c (torch.Tensor): ``cost_advantage`` stored in buffer.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            act (torch.Tensor): The ``action`` sampled from buffer.
+            logp (torch.Tensor): The ``log_p`` sampled from buffer.
+            adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
         """
         adv = self._compute_adv_surrogate(adv_r, adv_c)
-        loss, info = self._loss_pi(obs, act, logp, adv)
+        loss = self._loss_pi(obs, act, logp, adv)
         self._actor_critic.actor_optimizer.zero_grad()
         loss.backward()
         if self._cfgs.algo_cfgs.use_max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+            clip_grad_norm_(
                 self._actor_critic.actor.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
         distributed.avg_grads(self._actor_critic.actor)
         self._actor_critic.actor_optimizer.step()
-        self._logger.store(
-            **{
-                'Train/Entropy': info['entropy'],
-                'Train/PolicyRatio': info['ratio'],
-                'Train/PolicyStd': info['std'],
-                'Loss/Loss_pi': loss.mean().item(),
-            },
-        )
 
     def _compute_adv_surrogate(  # pylint: disable=unused-argument
         self,
         adv_r: torch.Tensor,
         adv_c: torch.Tensor,
     ) -> torch.Tensor:
         """Compute surrogate loss.
 
         Policy Gradient only use reward advantage.
 
         Args:
-            adv_r (torch.Tensor): reward advantage
-            adv_c (torch.Tensor): cost advantage
+            adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
+
+        Returns:
+            The ``reward_advantage`` used to update policy network.
         """
         return adv_r
 
     def _loss_pi(
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv: torch.Tensor,
-    ) -> tuple[torch.Tensor, dict[str, float]]:
+    ) -> torch.Tensor:
         r"""Computing pi/actor loss.
 
         In Policy Gradient, the loss is defined as:
 
         .. math::
 
-            L = -\mathbb{E}_{s_t \sim \rho_\theta} [
-                \sum_{t=0}^T ( \frac{\pi^{'}_\theta(a_t|s_t)}{\pi_\theta(a_t|s_t)} )
+            L = -\mathbb{E}_{s_t \sim \rho_{\theta}} [
+                \sum_{t=0}^T ( \frac{\pi^{'}_{\theta}(a_t|s_t)}{\pi_{\theta}(a_t|s_t)} )
                  A^{R}_{\pi_{\theta}}(s_t, a_t)
             ]
 
-        where :math:`\pi_\theta` is the policy network, :math:`\pi^{'}_\theta`
+        where :math:`\pi_{\theta}` is the policy network, :math:`\pi^{'}_{\theta}`
         is the new policy network, :math:`A^{R}_{\pi_{\theta}}(s_t, a_t)` is the advantage.
 
         Args:
-            obs (torch.Tensor): ``observation`` stored in buffer.
-            act (torch.Tensor): ``action`` stored in buffer.
-            logp (torch.Tensor): ``log probability`` of action stored in buffer.
-            adv (torch.Tensor): ``advantage`` stored in buffer.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            act (torch.Tensor): The ``action`` sampled from buffer.
+            logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
+            adv (torch.Tensor): The ``advantage`` sampled from buffer.
+
+        Returns:
+            The loss of pi/actor.
         """
         distribution = self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
         std = self._actor_critic.actor.std
         ratio = torch.exp(logp_ - logp)
         loss = -(ratio * adv).mean()
         entropy = distribution.entropy().mean().item()
-        info = {'entropy': entropy, 'ratio': ratio.mean().item(), 'std': std}
-        return loss, info
+        self._logger.store(
+            {
+                'Train/Entropy': entropy,
+                'Train/PolicyRatio': ratio,
+                'Train/PolicyStd': std,
+                'Loss/Loss_pi': loss.mean().item(),
+            },
+        )
+        return loss
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/ppo.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/ppo.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,41 +34,54 @@
 
     def _loss_pi(
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv: torch.Tensor,
-    ) -> tuple[torch.Tensor, dict[str, float]]:
+    ) -> torch.Tensor:
         r"""Computing pi/actor loss.
 
         In Proximal Policy Optimization, the loss is defined as:
 
         .. math::
-            L^{CLIP} = \mathbb{E}_{s_t \sim \rho_{\theta}}
-            \left[ \min(r_t  A^{R}_{\pi_{\theta}}(s_t, a_t) ,
-            \text{clip}(r_t, 1-\epsilon, 1+\epsilon)  A^{R}_{\pi_{\theta}}(s_t, a_t)  \right]
 
-        where :math:`r_t = \frac{\pi_\theta ^{'}(a_t|s_t)}{\pi_\theta(a_t|s_t)}`,
-        :math:`\epsilon` is the clip parameter, :math:`A^{R}_{\pi_{\theta}}(s_t, a_t)` is the advantage.
+            L^{CLIP} = \mathbb{E}_{s_t \sim \rho_{\theta}} \left[
+                \min ( r_t A^{R}_{\pi_{\theta}} (s_t, a_t) , \text{clip} (r_t, 1 - \epsilon, 1 + \epsilon)
+                A^{R}_{\pi_{\theta}} (s_t, a_t)
+            \right]
+
+        where :math:`r_t = \frac{\pi_{\theta}^{'} (a_t|s_t)}{\pi_{\theta} (a_t|s_t)}`,
+        :math:`\epsilon` is the clip parameter, and :math:`A^{R}_{\pi_{\theta}} (s_t, a_t)` is the
+        advantage.
 
         Args:
-            obs (torch.Tensor): ``observation`` stored in buffer.
-            act (torch.Tensor): ``action`` stored in buffer.
-            log_p (torch.Tensor): ``log probability`` of action stored in buffer.
-            adv (torch.Tensor): ``advantage`` stored in buffer.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            act (torch.Tensor): The ``action`` sampled from buffer.
+            logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
+            adv (torch.Tensor): The ``advantage`` sampled from buffer.
+
+        Returns:
+            The loss of pi/actor.
         """
         distribution = self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
         std = self._actor_critic.actor.std
         ratio = torch.exp(logp_ - logp)
         ratio_cliped = torch.clamp(
             ratio,
             1 - self._cfgs.algo_cfgs.clip,
             1 + self._cfgs.algo_cfgs.clip,
         )
         loss = -torch.min(ratio * adv, ratio_cliped * adv).mean()
         loss -= self._cfgs.algo_cfgs.entropy_coef * distribution.entropy().mean()
         # useful extra info
         entropy = distribution.entropy().mean().item()
-        info = {'entropy': entropy, 'ratio': ratio.mean().item(), 'std': std}
-        return loss, info
+        self._logger.store(
+            {
+                'Train/Entropy': entropy,
+                'Train/PolicyRatio': ratio,
+                'Train/PolicyStd': std,
+                'Loss/Loss_pi': loss.mean().item(),
+            },
+        )
+        return loss
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/base/trpo.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/trpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,66 +44,70 @@
         super()._init_log()
         self._logger.register_key('Misc/AcceptanceStep')
 
     # pylint: disable-next=too-many-arguments,too-many-locals,arguments-differ
     def _search_step_size(
         self,
         step_direction: torch.Tensor,
-        grad: torch.Tensor,
+        grads: torch.Tensor,
         p_dist: Distribution,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv: torch.Tensor,
         loss_before: float,
         total_steps: int = 15,
         decay: float = 0.8,
     ) -> tuple[torch.Tensor, int]:
         """TRPO performs `line-search <https://en.wikipedia.org/wiki/Line_search>`_ until constraint satisfaction.
 
         .. hint::
-
-            TRPO search around for a satisfied step of policy update to improve loss and reward performance.
-            The search is done by line-search, which is a way to find a step size that satisfies the constraint.
-            The constraint is the KL-divergence between the old policy and the new policy.
+            TRPO search around for a satisfied step of policy update to improve loss and reward performance. The search
+            is done by line-search, which is a way to find a step size that satisfies the constraint. The constraint is
+            the KL-divergence between the old policy and the new policy.
 
         Args:
             step_dir (torch.Tensor): The step direction.
             g_flat (torch.Tensor): The gradient of the policy.
             p_dist (torch.distributions.Distribution): The old policy distribution.
             obs (torch.Tensor): The observation.
             act (torch.Tensor): The action.
             logp (torch.Tensor): The log probability of the action.
             adv (torch.Tensor): The advantage.
-            cost_adv (torch.Tensor): The cost advantage.
+            adv_c (torch.Tensor): The cost advantage.
             loss_pi_before (float): The loss of the policy before the update.
             total_steps (int, optional): The total steps to search. Defaults to 15.
             decay (float, optional): The decay rate of the step size. Defaults to 0.8.
+
+        Returns:
+            The tuple of final update direction and acceptance step size.
         """
         # How far to go in a single update
         step_frac = 1.0
         # Get old parameterized policy expression
         theta_old = get_flat_params_from(self._actor_critic.actor)
         # Change expected objective function gradient = expected_imrpove best this moment
-        expected_improve = grad.dot(step_direction)
+        expected_improve = grads.dot(step_direction)
+
+        final_kl = 0.0
 
         # While not within_trust_region and not out of total_steps:
         for step in range(total_steps):
             # update theta params
             new_theta = theta_old + step_frac * step_direction
             # set new params as params of net
             set_param_values_to_model(self._actor_critic.actor, new_theta)
 
             with torch.no_grad():
-                loss, _ = self._loss_pi(obs, act, logp, adv)
+                loss = self._loss_pi(obs, act, logp, adv)
                 # compute KL distance between new and old policy
                 q_dist = self._actor_critic.actor(obs)
                 # KL-distance of old p-dist and new q-dist, applied in KLEarlyStopping
                 kl = torch.distributions.kl.kl_divergence(p_dist, q_dist).mean().item()
-                kl = distributed.dist_avg(kl)
+                kl = distributed.dist_avg(kl).mean().item()
             # real loss improve: old policy loss - new policy loss
             loss_improve = loss_before - loss.item()
             # average processes.... multi-processing style like: mpi_tools.mpi_avg(xxx)
             loss_improve = distributed.dist_avg(loss_improve)
             self._logger.log(f'Expected Improvement: {expected_improve} Actual: {loss_improve}')
             if not torch.isfinite(loss):
                 self._logger.log('WARNING: loss_pi not finite')
@@ -111,26 +115,27 @@
                 self._logger.log('INFO: did not improve improve <0')
             elif kl > self._cfgs.algo_cfgs.target_kl:
                 self._logger.log('INFO: violated KL constraint.')
             else:
                 # step only if surrogate is improved and when within trust reg.
                 acceptance_step = step + 1
                 self._logger.log(f'Accept step at i={acceptance_step}')
+                final_kl = kl
                 break
             step_frac *= decay
         else:
             self._logger.log('INFO: no suitable step found...')
             step_direction = torch.zeros_like(step_direction)
             acceptance_step = 0
 
         set_param_values_to_model(self._actor_critic.actor, theta_old)
 
         self._logger.store(
-            **{
-                'Train/KL': kl,
+            {
+                'Train/KL': final_kl,
             },
         )
 
         return step_frac * step_direction, acceptance_step
 
     def _update_actor(  # pylint: disable=too-many-arguments,too-many-locals
         self,
@@ -151,61 +156,57 @@
         - Search for a step size that satisfies the constraint.
         - Update the policy network.
 
         Args:
             obs (torch.Tensor): The observation tensor.
             act (torch.Tensor): The action tensor.
             logp (torch.Tensor): The log probability of the action.
-            adv_r (torch.Tensor): The advantage tensor.
+            adv_r (torch.Tensor): The reward advantage tensor.
             adv_c (torch.Tensor): The cost advantage tensor.
         """
         self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
         theta_old = get_flat_params_from(self._actor_critic.actor)
         self._actor_critic.actor.zero_grad()
         adv = self._compute_adv_surrogate(adv_r, adv_c)
-        loss, info = self._loss_pi(obs, act, logp, adv)
+        loss = self._loss_pi(obs, act, logp, adv)
         loss_before = distributed.dist_avg(loss).item()
         p_dist = self._actor_critic.actor(obs)
 
         loss.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
-        grad = -get_flat_gradients_from(self._actor_critic.actor)
-        x = conjugate_gradients(self._fvp, grad, self._cfgs.algo_cfgs.cg_iters)
+        grads = -get_flat_gradients_from(self._actor_critic.actor)
+        x = conjugate_gradients(self._fvp, grads, self._cfgs.algo_cfgs.cg_iters)
         assert torch.isfinite(x).all(), 'x is not finite'
         xHx = torch.dot(x, self._fvp(x))
         assert xHx.item() >= 0, 'xHx is negative'
         alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
         step_direction = x * alpha
         assert torch.isfinite(step_direction).all(), 'step_direction is not finite'
 
         step_direction, accept_step = self._search_step_size(
             step_direction=step_direction,
-            grad=grad,
+            grads=grads,
             p_dist=p_dist,
             obs=obs,
             act=act,
             logp=logp,
             adv=adv,
             loss_before=loss_before,
         )
 
         theta_new = theta_old + step_direction
         set_param_values_to_model(self._actor_critic.actor, theta_new)
 
         with torch.no_grad():
-            loss, info = self._loss_pi(obs, act, logp, adv)
+            loss = self._loss_pi(obs, act, logp, adv)
 
         self._logger.store(
-            **{
-                'Train/Entropy': info['entropy'],
-                'Train/PolicyRatio': info['ratio'],
-                'Train/PolicyStd': info['std'],
-                'Loss/Loss_pi': loss.mean().item(),
+            {
                 'Misc/Alpha': alpha.item(),
                 'Misc/FinalStepNorm': torch.norm(step_direction).mean().item(),
                 'Misc/xHx': xHx.item(),
-                'Misc/gradient_norm': torch.norm(grad).mean().item(),
+                'Misc/gradient_norm': torch.norm(grads).mean().item(),
                 'Misc/H_inv_g': x.norm().item(),
                 'Misc/AcceptanceStep': accept_step,
             },
         )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/first_order/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/first_order/cup.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/cup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,147 +13,141 @@
 # limitations under the License.
 # ==============================================================================
 """Implementation of the CUP algorithm."""
 
 import torch
 from rich.progress import track
 from torch.distributions import Normal
+from torch.nn.utils.clip_grad import clip_grad_norm_
 from torch.utils.data import DataLoader, TensorDataset
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.on_policy.base.ppo import PPO
 from omnisafe.common.lagrange import Lagrange
 from omnisafe.utils import distributed
-from omnisafe.utils.config import Config
 
 
 @registry.register
 class CUP(PPO):
     """The Constrained Update Projection (CUP) Approach to Safe Policy Optimization.
 
     References:
         - Title: Constrained Update Projection Approach to Safe Policy Optimization
         - Authors: Long Yang, Jiaming Ji, Juntao Dai, Linrui Zhang, Binbin Zhou, Pengfei Li,
-                    Yaodong Yang, Gang Pan.
+            Yaodong Yang, Gang Pan.
         - URL: `CUP <https://arxiv.org/abs/2209.07089>`_
     """
 
+    _p_dist: Normal
+
     def _init(self) -> None:
+        """The initialization of the algorithm.
+
+        Here we additionally initialize the Lagrange multiplier.
+        """
         super()._init()
-        self._lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
+        self._lagrange: Lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
 
     def _init_log(self) -> None:
-        r"""Log the CUP specific information.
-
-        .. list-table::
+        """Log the CUP specific information.
 
-            *   -   Things to log
-                -   Description
-            *   -   ``Metrics/LagrangeMultiplier``
-                -   The Lagrange multiplier.
-            *   -   ``Train/MaxRatio``
-                -   The maximum ratio between the current policy and the old policy.
-            *   -   ``Train/MinRatio``
-                -   The minimum ratio between the current policy and the old policy.
-            *   -   ``Loss/Loss_pi_c``
-                -   The loss of the cost performance.
-            *   -   ``Train/SecondStepStopIter``
-                -   The number of iterations to stop the second step.
-            *   -   ``Train/SecondStepEntropy``
-                -   The entropy of the current policy.
-            *   -   ``Train/SecondStepPolicyRatio``
-                -   The ratio between the current policy and the old policy.
+        +-----------------------------+----------------------------------------------------------+
+        | Things to log               | Description                                              |
+        +=============================+==========================================================+
+        | Metrics/LagrangeMultiplier  | The Lagrange multiplier.                                 |
+        +-----------------------------+----------------------------------------------------------+
+        | Loss/Loss_pi_c              | The loss of the cost performance.                        |
+        +-----------------------------+----------------------------------------------------------+
+        | Train/SecondStepStopIter    | The number of iterations to stop the second step.        |
+        +-----------------------------+----------------------------------------------------------+
+        | Train/SecondStepEntropy     | The entropy of the current policy.                       |
+        +-----------------------------+----------------------------------------------------------+
+        | Train/SecondStepPolicyRatio | The ratio between the current policy and the old policy. |
+        +-----------------------------+----------------------------------------------------------+
         """
         super()._init_log()
         self._logger.register_key('Metrics/LagrangeMultiplier')
-        self._logger.register_key('Train/MaxRatio')
-        self._logger.register_key('Train/MinRatio')
         self._logger.register_key('Loss/Loss_pi_c', delta=True)
         self._logger.register_key('Train/SecondStepStopIter')
         self._logger.register_key('Train/SecondStepEntropy')
-        self._logger.register_key('Train/SecondStepPolicyRatio')
+        self._logger.register_key('Train/SecondStepPolicyRatio', min_and_max=True)
 
-    def __init__(self, env_id: str, cfgs: Config) -> None:
-        super().__init__(env_id, cfgs)
-        self._p_dist: Normal
-        self._max_ratio: float = 0.0
-        self._min_ratio: float = 0.0
-
-    def _loss_pi_cost(self, obs, act, logp, adv_c):
+    def _loss_pi_cost(
+        self,
+        obs: torch.Tensor,
+        act: torch.Tensor,
+        logp: torch.Tensor,
+        adv_c: torch.Tensor,
+    ) -> torch.Tensor:
         r"""Compute the performance of cost on this moment.
 
-        Detailedly, we compute the KL divergence between the current policy and the old policy,
-        the entropy of the current policy, and the ratio between the current policy and the old
-        policy.
+        We compute the KL divergence between the current policy and the old policy, the entropy of
+        the current policy, and the ratio between the current policy and the old policy.
 
         The loss of the cost performance is defined as:
 
         .. math::
-            L = \underset{a \sim \pi_{\theta}}{\mathbb{E}}[\lambda \frac{1 - \gamma \nu}{1 - \gamma}
-            \frac{\pi_\theta^{'}(a|s)}{\pi_\theta(a|s)} A^{C}_{\pi_{\theta}}
-            + KL(\pi_\theta^{'}(a|s)||\pi_\theta(a|s))]
-
-        where :math:`\lambda` is the Lagrange multiplier,
-        :math:`\frac{1 - \gamma \nu}{1 - \gamma}` is the coefficient value,
-        :math:`\pi_\theta^{'}(a_t|s_t)` is the current policy,
-        :math:`\pi_\theta(a_t|s_t)` is the old policy,
-        :math:`A^{C}_{\pi_{\theta}}` is the cost advantage,
-        :math:`KL(\pi_\theta^{'}(a_t|s_t)||\pi_\theta(a_t|s_t))` is the KL divergence between the
-        current policy and the old policy.
+
+            L = \underset{a \sim \pi_{\theta}}{\mathbb{E}} [
+                \lambda \frac{1 - \gamma \nu}{1 - \gamma}
+                    \frac{\pi_{\theta}^{'} (a|s)}{\pi_{\theta} (a|s)} A^{C}_{\pi_{\theta}}
+                + KL (\pi_{\theta}^{'} (a|s) || \pi_{\theta} (a|s))
+            ]
+
+        where :math:`\lambda` is the Lagrange multiplier, :math:`\frac{1 - \gamma \nu}{1 - \gamma}`
+        is the coefficient value, :math:`\pi_{\theta}^{'} (a_t|s_t)` is the current policy,
+        :math:`\pi_{\theta} (a_t|s_t)` is the old policy, :math:`A^{C}_{\pi_{\theta}}` is the cost
+        advantage, :math:`KL (\pi_{\theta}^{'} (a_t|s_t) || \pi_{\theta} (a_t|s_t))` is the KL
+        divergence between the current policy and the old policy.
 
         Args:
-            obs (torch.Tensor): Observation.
-            act (torch.Tensor): Action.
-            log_p (torch.Tensor): Log probability.
-            cost_adv (torch.Tensor): Cost advantage.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            act (torch.Tensor): The ``action`` sampled from buffer.
+            logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
+
+        Returns:
+            The loss of the cost performance.
         """
         distribution = self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
-        std = self._actor_critic.actor.std
         ratio = torch.exp(logp_ - logp)
 
         kl = torch.distributions.kl_divergence(distribution, self._p_dist).sum(-1, keepdim=True)
 
         coef = (1 - self._cfgs.algo_cfgs.gamma * self._cfgs.algo_cfgs.lam) / (
             1 - self._cfgs.algo_cfgs.gamma
         )
         loss = (self._lagrange.lagrangian_multiplier * coef * ratio * adv_c + kl).mean()
 
-        # useful extra info
-        temp_max = torch.max(ratio).detach().mean().item()
-        temp_min = torch.min(ratio).detach().mean().item()
-        if temp_max > self._max_ratio:
-            self._max_ratio = temp_max
-        if temp_min < self._min_ratio:
-            self._min_ratio = temp_min
         entropy = distribution.entropy().mean().item()
-        info = {'entropy': entropy, 'ratio': ratio.mean().item(), 'std': std}
-
-        self._logger.store(**{'Loss/Loss_pi_c': loss.item()})
-
-        return loss, info
+        self._logger.store(
+            {
+                'Loss/Loss_pi_c': loss.item(),
+                'Train/SecondStepEntropy': entropy,
+                'Train/SecondStepPolicyRatio': ratio,
+            },
+        )
+        return loss
 
     def _update(self) -> None:
         r"""Update actor, critic, and Lagrange multiplier parameters.
 
         In CUP, the Lagrange multiplier is updated as the naive lagrange multiplier update:
 
         .. math::
-            \lambda_{k+1} = \lambda_k + \eta (J^{C}_{\pi_\theta} - C)
 
-        where :math:`\lambda_k` is the Lagrange multiplier at iteration :math:`k`,
-        :math:`\eta` is the Lagrange multiplier learning rate,
-        :math:`J^{C}_{\pi_{\theta}}` is the cost of the current policy,
-        and :math:`C` is the cost limit.
+            \lambda_{k+1} = \lambda_k + \eta (J^{C}_{\pi_{\theta}} - C)
 
-        Then in each iteration of the policy update, CUP calculates current policy's
-        distribution, which used to calculate the policy loss.
+        where :math:`\lambda_k` is the Lagrange multiplier at iteration :math:`k`, :math:`\eta` is
+        the Lagrange multiplier learning rate, :math:`J^{C}_{\pi_{\theta}}` is the cost of the
+        current policy, and :math:`C` is the cost limit.
 
-        Args:
-            self (object): object of the class.
+        Then in each iteration of the policy update, CUP calculates current policy's distribution,
+        which used to calculate the policy loss.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
         self._lagrange.update_lagrange_multiplier(Jc)
 
         super()._update()
@@ -173,22 +167,23 @@
 
         dataloader = DataLoader(
             dataset=TensorDataset(obs, act, logp, adv_c, old_mean, old_std),
             batch_size=self._cfgs.algo_cfgs.batch_size,
             shuffle=True,
         )
 
+        final_steps = self._cfgs.algo_cfgs.update_iters
         for i in track(range(self._cfgs.algo_cfgs.update_iters), description='Updating...'):
             for obs, act, logp, adv_c, old_mean, old_std in dataloader:
                 self._p_dist = Normal(old_mean, old_std)
-                loss_cost, info = self._loss_pi_cost(obs, act, logp, adv_c)
+                loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
                 self._actor_critic.actor_optimizer.zero_grad()
                 loss_cost.backward()
                 if self._cfgs.algo_cfgs.max_grad_norm is not None:
-                    torch.nn.utils.clip_grad_norm_(
+                    clip_grad_norm_(
                         self._actor_critic.actor.parameters(),
                         self._cfgs.algo_cfgs.max_grad_norm,
                     )
                 distributed.avg_grads(self._actor_critic.actor)
                 self._actor_critic.actor_optimizer.step()
 
             new_distribution = self._actor_critic.actor(original_obs)
@@ -198,20 +193,17 @@
                 .sum(-1, keepdim=True)
                 .mean()
                 .item()
             )
             kl = distributed.dist_avg(kl)
 
             if self._cfgs.algo_cfgs.kl_early_stop and kl > self._cfgs.algo_cfgs.target_kl:
+                final_steps = i + 1
                 self._logger.log(f'Early stopping at iter {i + 1} due to reaching max kl')
                 break
 
         self._logger.store(
-            **{
+            {
                 'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier.item(),
-                'Train/MaxRatio': self._max_ratio,
-                'Train/MinRatio': self._min_ratio,
-                'Train/SecondStepStopIter': i + 1,  # pylint: disable=undefined-loop-variable
-                'Train/SecondStepEntropy': info['entropy'],
-                'Train/SecondStepPolicyRatio': info['ratio'],
+                'Train/SecondStepStopIter': final_steps,  # pylint: disable=undefined-loop-variable
             },
         )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/first_order/focops.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/focops.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,136 +21,145 @@
 from torch.distributions import Normal
 from torch.utils.data import DataLoader, TensorDataset
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.on_policy.base.policy_gradient import PolicyGradient
 from omnisafe.common.lagrange import Lagrange
 from omnisafe.utils import distributed
-from omnisafe.utils.config import Config
 
 
 @registry.register
 class FOCOPS(PolicyGradient):
     """The First Order Constrained Optimization in Policy Space (FOCOPS) algorithm.
 
     References:
         - Title: First Order Constrained Optimization in Policy Space
         - Authors: Yiming Zhang, Quan Vuong, Keith W. Ross.
         - URL: `FOCOPS <https://arxiv.org/abs/2002.06506>`_
     """
 
+    _p_dist: Normal
+
     def _init(self) -> None:
         """Initialize the FOCOPS specific model.
 
         The FOCOPS algorithm uses a Lagrange multiplier to balance the cost and reward.
         """
         super()._init()
-        self._lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
+        self._lagrange: Lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
 
     def _init_log(self) -> None:
-        r"""Log the FOCOPS specific information.
-
-        .. list-table::
+        """Log the FOCOPS specific information.
 
-            *   -   Things to log
-                -   Description
-            *   -   ``Metrics/LagrangeMultiplier``
-                -   The Lagrange multiplier.
+        +----------------------------+--------------------------+
+        | Things to log              | Description              |
+        +============================+==========================+
+        | Metrics/LagrangeMultiplier | The Lagrange multiplier. |
+        +----------------------------+--------------------------+
         """
         super()._init_log()
         self._logger.register_key('Metrics/LagrangeMultiplier')
 
-    def __init__(self, env_id: str, cfgs: Config) -> None:
-        super().__init__(env_id, cfgs)
-        self._p_dist: Normal
-
     def _loss_pi(
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv: torch.Tensor,
-    ) -> tuple[torch.Tensor, dict[str, float]]:
+    ) -> torch.Tensor:
         r"""Compute pi/actor loss.
 
         In FOCOPS, the loss is defined as:
 
         .. math::
             :nowrap:
 
             \begin{eqnarray}
-            L = \nabla_\theta D_{K L}\left(\pi_\theta^{'} \| \pi_{\theta}\right)[s]
-            -\frac{1}{\eta} \underset{a \sim \pi_{\theta}}
-            {\mathbb{E}}\left[\frac{\nabla_\theta \pi_\theta(a \mid s)}
-            {\pi_{\theta}(a \mid s)}\left(A^{R}_{\pi_{\theta}}(s, a)
-            -\lambda A^C_{\pi_{\theta}}(s, a)\right)\right]
+                L = \nabla_{\theta} D_{K L} \left( \pi_{\theta}^{'} \| \pi_{\theta} \right)[s]
+                - \frac{1}{\eta} \underset{a \sim \pi_{\theta}}{\mathbb{E}} \left[
+                    \frac{\nabla_{\theta} \pi_{\theta} (a \mid s)}{\pi_{\theta}(a \mid s)}
+                    \left( A^{R}_{\pi_{\theta}} (s, a) - \lambda A^C_{\pi_{\theta}} (s, a) \right)
+                \right]
             \end{eqnarray}
 
         where :math:`\eta` is a hyperparameter, :math:`\lambda` is the Lagrange multiplier,
         :math:`A_{\pi_{\theta_k}}(s, a)` is the advantage function,
         :math:`A^C_{\pi_{\theta_k}}(s, a)` is the cost advantage function,
         :math:`\pi^*` is the optimal policy, and :math:`\pi_{\theta}` is the current policy.
 
         Args:
-            obs (torch.Tensor): ``observation`` stored in buffer.
-            act (torch.Tensor): ``action`` stored in buffer.
-            logp (torch.Tensor): ``log probability`` of action stored in buffer.
-            adv (torch.Tensor): ``advantage`` stored in buffer.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            act (torch.Tensor): The ``action`` sampled from buffer.
+            logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
+            adv (torch.Tensor): The ``advantage`` sampled from buffer.
+
+        Returns:
+            The loss of pi/actor.
         """
         distribution = self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
         std = self._actor_critic.actor.std
         ratio = torch.exp(logp_ - logp)
 
         kl = torch.distributions.kl_divergence(distribution, self._p_dist).sum(-1, keepdim=True)
         loss = (kl - (1 / self._cfgs.algo_cfgs.focops_lam) * ratio * adv) * (
             kl.detach() <= self._cfgs.algo_cfgs.focops_eta
         ).type(torch.float32)
         loss = loss.mean()
         loss -= self._cfgs.algo_cfgs.entropy_coef * distribution.entropy().mean()
 
         entropy = distribution.entropy().mean().item()
-        info = {'entropy': entropy, 'ratio': ratio.mean().item(), 'std': std}
-        return loss, info
+        self._logger.store(
+            {
+                'Train/Entropy': entropy,
+                'Train/PolicyRatio': ratio,
+                'Train/PolicyStd': std,
+                'Loss/Loss_pi': loss.mean().item(),
+            },
+        )
+        return loss
 
     def _compute_adv_surrogate(self, adv_r: torch.Tensor, adv_c: torch.Tensor) -> torch.Tensor:
         r"""Compute surrogate loss.
 
         FOCOPS uses the following surrogate loss:
 
         .. math::
-            L = \frac{1}{1 + \lambda} [A^{R}_{\pi_{\theta}}(s, a)
-            - \lambda A^C_{\pi_{\theta}}(s, a)]
+
+            L = \frac{1}{1 + \lambda} [
+                A^{R}_{\pi_{\theta}} (s, a)
+                - \lambda A^C_{\pi_{\theta}} (s, a)
+            ]
 
         Args:
-            adv (torch.Tensor): reward advantage
-            cost_adv (torch.Tensor): cost advantage
+            adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
+
+        Returns:
+            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
         """
         return (adv_r - self._lagrange.lagrangian_multiplier * adv_c) / (
             1 + self._lagrange.lagrangian_multiplier
         )
 
     def _update(self) -> None:
         r"""Update actor, critic, and Lagrange multiplier parameters.
 
         In FOCOPS, the Lagrange multiplier is updated as the naive lagrange multiplier update:
 
         .. math::
-            \lambda_{k+1} = \lambda_k + \eta (J^{C}_{\pi_\theta} - C)
 
-        where :math:`\lambda_k` is the Lagrange multiplier at iteration :math:`k`,
-        :math:`\eta` is the Lagrange multiplier learning rate,
-        :math:`J^{C}_{\pi_\theta}` is the cost of the current policy,
-        and :math:`C` is the cost limit.
+            \lambda_{k+1} = \lambda_k + \eta (J^{C}_{\pi_{\theta}} - C)
+
+        where :math:`\lambda_k` is the Lagrange multiplier at iteration :math:`k`, :math:`\eta` is
+        the Lagrange multiplier learning rate, :math:`J^{C}_{\pi_{\theta}}` is the cost of the current
+        policy, and :math:`C` is the cost limit.
 
         Then in each iteration of the policy update, FOCOPS calculates current policy's
         distribution, which used to calculate the policy loss.
-
-        Args:
-            self (object): object of the class.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
         self._lagrange.update_lagrange_multiplier(Jc)
 
         data = self._buf.get()
@@ -181,14 +190,15 @@
                 old_mean,
                 old_std,
             ),
             batch_size=self._cfgs.algo_cfgs.batch_size,
             shuffle=True,
         )
 
+        final_steps = self._cfgs.algo_cfgs.update_iters
         for i in track(range(self._cfgs.algo_cfgs.update_iters), description='Updating...'):
             for (
                 obs,
                 act,
                 logp,
                 target_value_r,
                 target_value_c,
@@ -210,19 +220,20 @@
                 torch.distributions.kl.kl_divergence(old_distribution, new_distribution)
                 .sum(-1, keepdim=True)
                 .mean()
                 .item()
             )
             kl = distributed.dist_avg(kl)
 
+            self._logger.store({'Train/KL': kl})
             if self._cfgs.algo_cfgs.kl_early_stop and kl > self._cfgs.algo_cfgs.target_kl:
+                final_steps = i + 1
                 self._logger.log(f'Early stopping at iter {i + 1} due to reaching max kl')
                 break
 
         self._logger.store(
-            **{
-                'Train/StopIter': i + 1,  # pylint: disable=undefined-loop-variable
+            {
+                'Train/StopIter': final_steps,
                 'Value/Adv': adv_r.mean().item(),
-                'Train/KL': kl,
                 'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier,
             },
         )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/crpo.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/crpo.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,44 +28,47 @@
     References:
         - Title: CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee.
         - Authors: Tengyu Xu, Yingbin Liang, Guanghui Lan.
         - URL: `CRPO <https://arxiv.org/pdf/2011.05869.pdf>`_.
     """
 
     def __init__(self, env_id: str, cfgs: Config) -> None:
+        """Initialize an instance of :class:`OnCRPO`."""
         super().__init__(env_id, cfgs)
-        self._rew_update = 0
-        self._cost_update = 0
+        self._rew_update: int = 0
+        self._cost_update: int = 0
 
     def _init_log(self) -> None:
-        r"""Log the CRPO specific information.
+        """Log the CRPO specific information.
 
-        .. list-table::
-
-            *   -   Things to log
-                -   Description
-            *   -  ``Misc/RewUpdate``
-                -   The number of times the reward is updated.
-            *   -  ``Misc/CostUpdate``
-                -   The number of times the cost is updated.
+        +-----------------+--------------------------------------------+
+        | Things to log   | Description                                |
+        +=================+============================================+
+        | Misc/RewUpdate  | The number of times the reward is updated. |
+        +-----------------+--------------------------------------------+
+        | Misc/CostUpdate | The number of times the cost is updated.   |
+        +-----------------+--------------------------------------------+
         """
         super()._init_log()
         self._logger.register_key('Misc/RewUpdate')
         self._logger.register_key('Misc/CostUpdate')
 
     def _compute_adv_surrogate(self, adv_r: torch.Tensor, adv_c: torch.Tensor) -> torch.Tensor:
         """Compute the advantage surrogate.
 
-        In CRPO algorithm, we first judge whether the cost is within the limit.
-        If the cost is within the limit, we use the advantage of the policy.
-        Otherwise, we use the advantage of the cost.
+        In CRPO algorithm, we first judge whether the cost is within the limit. If the cost is
+        within the limit, we use the advantage of the policy. Otherwise, we use the advantage of the
+        cost.
 
         Args:
-            adv_r (torch.Tensor): The advantage of the policy.
-            adv_c (torch.Tensor): The advantage of the cost.
+            adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
+
+        Returns:
+            The ``advantage`` chosen from ``reward_advantage`` and ``cost_advantage``.
         """
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         if Jc <= self._cfgs.algo_cfgs.cost_limit + self._cfgs.algo_cfgs.distance:
             self._rew_update += 1
             return adv_r
         self._cost_update += 1
         return -adv_c
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,60 +8,96 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of the PDO algorithm."""
+"""Implementation of the Reward Constrained Policy Optimization algorithm."""
 
 import torch
 
 from omnisafe.algorithms import registry
-from omnisafe.algorithms.on_policy.base.policy_gradient import PolicyGradient
+from omnisafe.algorithms.on_policy.base.natural_pg import NaturalPG
 from omnisafe.common.lagrange import Lagrange
 
 
 @registry.register
-class PDO(PolicyGradient):
-    """The Lagrange version of the Policy Gradient algorithm.
+class RCPO(NaturalPG):
+    """Reward Constrained Policy Optimization.
 
-    A simple combination of the :class:`Lagrange` method and the :class:`PolicyGradient` algorithm.
+    References:
+        - Title: Reward Constrained Policy Optimization.
+        - Authors: Chen Tessler, Daniel J. Mankowitz, Shie Mannor.
+        - URL: `Reward Constrained Policy Optimization <https://arxiv.org/abs/1805.11074>`_
     """
 
     def _init(self) -> None:
+        """The initialization of the algorithm.
+
+        Here we additionally initialize the Lagrange multiplier.
+        """
         super()._init()
-        self._lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
+        self._lagrange: Lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
 
     def _init_log(self) -> None:
+        """Log the RCPO specific information.
+
+        +----------------------------+--------------------------+
+        | Things to log              | Description              |
+        +============================+==========================+
+        | Metrics/LagrangeMultiplier | The Lagrange multiplier. |
+        +----------------------------+--------------------------+
+        """
         super()._init_log()
-        self._logger.register_key('Metrics/LagrangeMultiplier')
+        self._logger.register_key('Metrics/LagrangeMultiplier', min_and_max=True)
 
     def _update(self) -> None:
-        r"""Update actor, critic, running statistics as we used in the :class:`PolicyGradient` algorithm.
+        r"""Update actor, critic, as we used in the :class:`PolicyGradient` algorithm.
 
-        Additionally, we update the Lagrange multiplier parameter,
-        by calling the :meth:`update_lagrange_multiplier` method.
+        Additionally, we update the Lagrange multiplier parameter by calling the
+        :meth:`update_lagrange_multiplier` method.
 
         .. note::
-            The :meth:`compute_loss_pi` is defined in the :class:`PolicyGradient` algorithm.
-            When a lagrange multiplier is used,
-            the :meth:`compute_loss_pi` method will return the loss of the policy as:
+            The :meth:`compute_loss_pi` is defined in the :class:`PolicyGradient` algorithm. When a
+            lagrange multiplier is used, the :meth:`compute_loss_pi` method will return the loss of
+            the policy as:
 
             .. math::
-                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[ \frac{\pi_\theta(a_t|s_t)}{\pi_\theta^{old}(a_t|s_t)}
-                [A^{R}(s_t, a_t) - \lambda A^{C}(s_t, a_t)] \right]
+
+                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[
+                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old} (a_t|s_t)}
+                    [ A^{R} (s_t, a_t) - \lambda A^{C} (s_t, a_t) ]
+                \right]
 
             where :math:`\lambda` is the Lagrange multiplier parameter.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
         self._lagrange.update_lagrange_multiplier(Jc)
         # then update the policy and value function
         super()._update()
 
-        self._logger.store(**{'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier})
+        self._logger.store({'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier})
 
     def _compute_adv_surrogate(self, adv_r: torch.Tensor, adv_c: torch.Tensor) -> torch.Tensor:
+        r"""Compute surrogate loss.
+
+        RCPO uses the following surrogate loss:
+
+        .. math::
+
+            L = \frac{1}{1 + \lambda} [
+                A^{R}_{\pi_{\theta}} (s, a)
+                - \lambda A^C_{\pi_{\theta}} (s, a)
+            ]
+
+        Args:
+            adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
+
+        Returns:
+            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
+        """
         penalty = self._lagrange.lagrangian_multiplier.item()
         return (adv_r - penalty * adv_c) / (1 + penalty)
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,67 +31,72 @@
 
     def _init(self) -> None:
         """Initialize the PPOLag specific model.
 
         The PPOLag algorithm uses a Lagrange multiplier to balance the cost and reward.
         """
         super()._init()
-        self._lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
+        self._lagrange: Lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
 
     def _init_log(self) -> None:
-        r"""Log the PPOLag specific information.
+        """Log the PPOLag specific information.
 
-        .. list-table::
-
-            *   -   Things to log
-                -   Description
-            *   -   ``Metrics/LagrangeMultiplier``
-                -   The Lagrange multiplier.
+        +----------------------------+--------------------------+
+        | Things to log              | Description              |
+        +============================+==========================+
+        | Metrics/LagrangeMultiplier | The Lagrange multiplier. |
+        +----------------------------+--------------------------+
         """
         super()._init_log()
-        self._logger.register_key('Metrics/LagrangeMultiplier')
+        self._logger.register_key('Metrics/LagrangeMultiplier', min_and_max=True)
 
     def _update(self) -> None:
-        r"""Update actor, critic, running statistics as we used in the :class:`PolicyGradient` algorithm.
+        r"""Update actor, critic, as we used in the :class:`PolicyGradient` algorithm.
 
-        Additionally, we update the Lagrange multiplier parameter,
-        by calling the :meth:`update_lagrange_multiplier()` method.
+        Additionally, we update the Lagrange multiplier parameter by calling the
+        :meth:`update_lagrange_multiplier` method.
 
         .. note::
-            The :meth:`_loss_pi()` is defined in the :class:`PolicyGradient` algorithm.
-            When a lagrange multiplier is used,
-            the :meth:`_loss_pi()` method will return the loss of the policy as:
+            The :meth:`_loss_pi` is defined in the :class:`PolicyGradient` algorithm. When a
+            lagrange multiplier is used, the :meth:`_loss_pi` method will return the loss of the
+            policy as:
 
             .. math::
-                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[ \frac{\pi_\theta(a_t|s_t)}{\pi_\theta^{old}(a_t|s_t)}
-                [A^{R}_{\pi_{\theta}}(s_t, a_t) - \lambda A^{C}_{\pi_{\theta}}(s_t, a_t)] \right]
 
-            where :math:`\lambda` is the Lagrange multiplier parameter.
+                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[
+                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old}(a_t|s_t)}
+                    [ A^{R}_{\pi_{\theta}} (s_t, a_t) - \lambda A^{C}_{\pi_{\theta}} (s_t, a_t) ]
+                \right]
 
-        Args:
-            self (object): object of the class.
+            where :math:`\lambda` is the Lagrange multiplier parameter.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         assert not np.isnan(Jc), 'cost for updating lagrange multiplier is nan'
         # first update Lagrange multiplier parameter
         self._lagrange.update_lagrange_multiplier(Jc)
         # then update the policy and value function
         super()._update()
 
-        self._logger.store(**{'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier})
+        self._logger.store({'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier})
 
     def _compute_adv_surrogate(self, adv_r: torch.Tensor, adv_c: torch.Tensor) -> torch.Tensor:
         r"""Compute surrogate loss.
 
         PPOLag uses the following surrogate loss:
 
         .. math::
-            L = \frac{1}{1 + \lambda} [A^{R}_{\pi_{\theta}}(s, a)
-            - \lambda A^C_{\pi_{\theta}}(s, a)]
+
+            L = \frac{1}{1 + \lambda} [
+                A^{R}_{\pi_{\theta}} (s, a)
+                - \lambda A^C_{\pi_{\theta}} (s, a)
+            ]
 
         Args:
-            adv (torch.Tensor): reward advantage
-            cost_adv (torch.Tensor): cost advantage
+            adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
+
+        Returns:
+            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
         """
         penalty = self._lagrange.lagrangian_multiplier.item()
         return (adv_r - penalty * adv_c) / (1 + penalty)
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,66 +30,71 @@
 
     def _init(self) -> None:
         """Initialize the TRPOLag specific model.
 
         The TRPOLag algorithm uses a Lagrange multiplier to balance the cost and reward.
         """
         super()._init()
-        self._lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
+        self._lagrange: Lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
 
     def _init_log(self) -> None:
-        r"""Log the TRPOLag specific information.
+        """Log the TRPOLag specific information.
 
-        .. list-table::
-
-            *   -   Things to log
-                -   Description
-            *   -   ``Metrics/LagrangeMultiplier``
-                -   The Lagrange multiplier.
+        +----------------------------+--------------------------+
+        | Things to log              | Description              |
+        +============================+==========================+
+        | Metrics/LagrangeMultiplier | The Lagrange multiplier. |
+        +----------------------------+--------------------------+
         """
         super()._init_log()
-        self._logger.register_key('Metrics/LagrangeMultiplier')
+        self._logger.register_key('Metrics/LagrangeMultiplier', min_and_max=True)
 
     def _update(self) -> None:
-        r"""Update actor, critic, running statistics as we used in the :class:`PolicyGradient` algorithm.
+        r"""Update actor, critic, as we used in the :class:`PolicyGradient` algorithm.
 
-        Additionally, we update the Lagrange multiplier parameter,
-        by calling the :meth:`update_lagrange_multiplier()` method.
+        Additionally, we update the Lagrange multiplier parameter by calling the
+        :meth:`update_lagrange_multiplier` method.
 
         .. note::
-            The :meth:`_loss_pi()` is defined in the :class:`PolicyGradient` algorithm.
-            When a lagrange multiplier is used,
-            the :meth:`_loss_pi()` method will return the loss of the policy as:
+            The :meth:`_loss_pi` is defined in the :class:`PolicyGradient` algorithm. When a
+            lagrange multiplier is used, the :meth:`_loss_pi` method will return the loss of the
+            policy as:
 
             .. math::
-                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[ \frac{\pi_\theta(a_t|s_t)}{\pi_\theta^{old}(a_t|s_t)}
-                [A^{R}_{\pi_{\theta}}(s_t, a_t) - \lambda A^{C}_{\pi_{\theta}}(s_t, a_t)] \right]
 
-            where :math:`\lambda` is the Lagrange multiplier parameter.
+                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[
+                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old} (a_t|s_t)}
+                    [ A^{R}_{\pi_{\theta}} (s_t, a_t) - \lambda A^{C}_{\pi_{\theta}} (s_t, a_t) ]
+                \right]
 
-        Args:
-            self (object): object of the class.
+            where :math:`\lambda` is the Lagrange multiplier parameter.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
         self._lagrange.update_lagrange_multiplier(Jc)
         # then update the policy and value function
         super()._update()
 
-        self._logger.store(**{'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier})
+        self._logger.store({'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier})
 
     def _compute_adv_surrogate(self, adv_r: torch.Tensor, adv_c: torch.Tensor) -> torch.Tensor:
         r"""Compute surrogate loss.
 
-        PPOLag uses the following surrogate loss:
+        TRPOLag uses the following surrogate loss:
 
         .. math::
-            L = \frac{1}{1 + \lambda} [A^{R}_{\pi_{\theta}}(s, a)
-            - \lambda A^C_{\pi_{\theta}}(s, a)]
+
+            L = \frac{1}{1 + \lambda} [
+                A^{R}_{\pi_{\theta}} (s, a)
+                - \lambda A^C_{\pi_{\theta}} (s, a)
+            ]
 
         Args:
-            adv (torch.Tensor): reward advantage
-            cost_adv (torch.Tensor): cost advantage
+            adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
+
+        Returns:
+            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
         """
         penalty = self._lagrange.lagrangian_multiplier.item()
         return (adv_r - penalty * adv_c) / (1 + penalty)
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/penalty_function/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/penalty_function/p3o.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/p3o.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the P3O algorithm."""
 
 import torch
 import torch.nn.functional as F
+from torch.nn.utils.clip_grad import clip_grad_norm_
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.on_policy.base.ppo import PPO
 from omnisafe.utils import distributed
 
 
 @registry.register
@@ -29,111 +30,103 @@
     References:
         - Title: Penalized Proximal Policy Optimization for Safe Reinforcement Learning
         - Authors: Linrui Zhang, Li Shen, Long Yang, Shixiang Chen, Bo Yuan, Xueqian Wang, Dacheng Tao.
         - URL: `P3O <https://arxiv.org/pdf/2205.11814.pdf>`_
     """
 
     def _init_log(self) -> None:
-        r"""Log the P3O specific information.
+        """Log the P3O specific information.
 
-        .. list-table::
-
-            *   -   Things to log
-                -   Description
-            *   -  ``Loss/Loss_pi_cost``
-                -   The loss of the cost performance.
+        +-------------------+-----------------------------------+
+        | Things to log     | Description                       |
+        +===================+===================================+
+        | Loss/Loss_pi_cost | The loss of the cost performance. |
+        +-------------------+-----------------------------------+
         """
         super()._init_log()
         self._logger.register_key('Loss/Loss_pi_cost', delta=True)
 
     def _loss_pi_cost(
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_c: torch.Tensor,
     ) -> torch.Tensor:
         r"""Compute the performance of cost on this moment.
 
-        Detailedly, we compute the loss of cost of policy cost from real cost.
+        We compute the loss of cost of policy cost from real cost.
 
         .. math::
-            L = \mathbb{E}_{\pi} \left[ \frac{\pi^{'}(a|s)}{\pi(a|s)} A^{C}_{\pi_\theta}(s, a) \right]
 
-        where :math:`A^{C}_{\pi_\theta}(s, a)` is the cost advantage,
-        :math:`\pi(a|s)` is the old policy,
-        :math:`\pi^{'}(a|s)` is the current policy.
+            L = \mathbb{E}_{\pi} \left[
+                \frac{\pi^{'} (a|s)}{\pi (a|s)} A^{C}_{\pi_{\theta}} (s, a)
+            \right]
+
+        where :math:`A^{C}_{\pi_{\theta}} (s, a)` is the cost advantage, :math:`\pi (a|s)` is the
+        old policy, and :math:`\pi^{'} (a|s)` is the current policy.
 
         Args:
-            obs (torch.Tensor): Observation.
-            act (torch.Tensor): Action.
-            logp (torch.Tensor): Log probability of action.
-            adv_c (torch.Tensor): Cost advantage.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            act (torch.Tensor): The ``action`` sampled from buffer.
+            logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            torch.Tensor: The loss of cost of policy cost from real cost.
+            The loss of the cost performance.
         """
         self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
         ratio = torch.exp(logp_ - logp)
         surr_cadv = (ratio * adv_c).mean()
         Jc = self._logger.get_stats('Metrics/EpCost')[0] - self._cfgs.algo_cfgs.cost_limit
         loss_cost = self._cfgs.algo_cfgs.kappa * F.relu(surr_cadv + Jc)
+        self._logger.store({'Loss/Loss_pi_cost': loss_cost.mean().item()})
         return loss_cost.mean()
 
     def _update_actor(
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_r: torch.Tensor,
         adv_c: torch.Tensor,
     ) -> None:
-        r"""Update policy network under a double for loop.
+        """Update policy network under a double for loop.
 
-            The pseudo code is shown below:
+        The pseudo code is shown below:
 
-            .. code-block:: python
+        .. code-block:: python
 
-                for _ in range(self.cfgs.actor_iters):
-                    for _ in range(self.cfgs.num_mini_batches):
-                        # Get mini-batch data
-                        # Compute loss
-                        # Update network
-
-            .. warning::
-                For some ``KL divergence`` based algorithms (e.g. TRPO, CPO, etc.),
-                the ``KL divergence`` between the old policy and the new policy is calculated.
-                And the ``KL divergence`` is used to determine whether the update is successful.
-                If the ``KL divergence`` is too large, the update will be terminated.
+            for _ in range(self.cfgs.actor_iters):
+                for _ in range(self.cfgs.num_mini_batches):
+                    # Get mini-batch data
+                    # Compute loss
+                    # Update network
+
+        .. warning::
+            For some ``KL divergence`` based algorithms (e.g. TRPO, CPO, etc.), the ``KL divergence``
+            between the old policy and the new policy is calculated. And the ``KL divergence`` is
+            used to determine whether the update is successful. If the ``KL divergence`` is too
+            large, the update will be terminated.
 
         Args:
             obs (torch.Tensor): ``observation`` stored in buffer.
             act (torch.Tensor): ``action`` stored in buffer.
-            log_p (torch.Tensor): ``log_p`` stored in buffer.
-            adv (torch.Tensor): ``advantage`` stored in buffer.
+            logp (torch.Tensor): ``log_p`` stored in buffer.
+            adv_r (torch.Tensor): ``reward_advantage`` stored in buffer.
             adv_c (torch.Tensor): ``cost_advantage`` stored in buffer.
         """
-        loss_reward, info = self._loss_pi(obs, act, logp, adv_r)
+        loss_reward = self._loss_pi(obs, act, logp, adv_r)
         loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
 
         loss = loss_reward + loss_cost
 
         self._actor_critic.actor_optimizer.zero_grad()
         loss.backward()
         if self._cfgs.algo_cfgs.use_max_grad_norm:
-            torch.nn.utils.clip_grad_norm_(
+            clip_grad_norm_(
                 self._actor_critic.actor.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
         distributed.avg_grads(self._actor_critic.actor)
         self._actor_critic.actor_optimizer.step()
-
-        self._logger.store(
-            **{
-                'Train/Entropy': info['entropy'],
-                'Train/PolicyRatio': info['ratio'],
-                'Train/PolicyStd': info['std'],
-                'Loss/Loss_pi': loss_reward.mean().item(),
-                'Loss/Loss_pi_cost': loss_cost.mean().item(),
-            },
-        )
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/second_order/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/second_order/cpo.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/cpo.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self._logger.register_key('Misc/Nu_star')
         self._logger.register_key('Misc/OptimCase')
 
     # pylint: disable-next=too-many-arguments,too-many-locals
     def _cpo_search_step(
         self,
         step_direction: torch.Tensor,
-        grad: torch.Tensor,
+        grads: torch.Tensor,
         p_dist: torch.distributions.Distribution,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_r: torch.Tensor,
         adv_c: torch.Tensor,
         loss_reward_before: float,
@@ -69,59 +69,64 @@
         total_steps: int = 15,
         decay: float = 0.8,
         violation_c: int = 0,
         optim_case: int = 0,
     ) -> tuple[torch.Tensor, int]:
         r"""Use line-search to find the step size that satisfies the constraint.
 
-        CPO uses line-search to find the step size that satisfies the constraint.
-        The constraint is defined as:
+        CPO uses line-search to find the step size that satisfies the constraint. The constraint is
+        defined as:
 
         .. math::
-            J^C(\theta + \alpha \delta) - J^C(\theta) \leq \max \{0, c\}\\
-            D_{KL}(\pi_{\theta}(\cdot|s) || \pi_{\theta + \alpha \delta}(\cdot|s)) \leq \delta_{KL}
+
+            J^C (\theta + \alpha \delta) - J^C (\theta) \leq \max \{ 0, c \} \\
+            D_{KL} (\pi_{\theta} (\cdot|s) || \pi_{\theta + \alpha \delta} (\cdot|s)) \leq \delta_{KL}
 
         where :math:`\delta_{KL}` is the constraint of KL divergence, :math:`\alpha` is the step size,
         :math:`c` is the violation of constraint.
 
         Args:
             step_dir (torch.Tensor): The step direction.
             g_flat (torch.Tensor): The gradient of the policy.
             p_dist (torch.distributions.Distribution): The old policy distribution.
             obs (torch.Tensor): The observation.
             act (torch.Tensor): The action.
-            log_p (torch.Tensor): The log probability of the action.
+            logp (torch.Tensor): The log probability of the action.
             adv (torch.Tensor): The advantage.
-            cost_adv (torch.Tensor): The cost advantage.
+            adv_c (torch.Tensor): The cost advantage.
             loss_pi_before (float): The loss of the policy before the update.
             total_steps (int, optional): The total steps to search. Defaults to 15.
             decay (float, optional): The decay rate of the step size. Defaults to 0.8.
-            c (int, optional): The violation of constraint. Defaults to 0.
+            violation_c (int, optional): The violation of constraint. Defaults to 0.
             optim_case (int, optional): The optimization case. Defaults to 0.
+
+        Returns:
+            A tuple of final step direction and the size of acceptance steps.
         """
         # get distance each time theta goes towards certain direction
         step_frac = 1.0
         # get and flatten parameters from pi-net
         theta_old = get_flat_params_from(self._actor_critic.actor)
         # reward improvement, g-flat as gradient of reward
-        expected_reward_improve = grad.dot(step_direction)
+        expected_reward_improve = grads.dot(step_direction)
 
+        kl = torch.zeros(1)
         # while not within_trust_region and not finish all steps:
         for step in range(total_steps):
             # get new theta
             new_theta = theta_old + step_frac * step_direction
             # set new theta as new actor parameters
             set_param_values_to_model(self._actor_critic.actor, new_theta)
             # the last acceptance steps to next step
             acceptance_step = step + 1
 
             with torch.no_grad():
                 try:
                     # loss of policy reward from target/expected reward
-                    loss_reward, _ = self._loss_pi(obs=obs, act=act, logp=logp, adv=adv_r)
+                    loss_reward = self._loss_pi(obs=obs, act=act, logp=logp, adv=adv_r)
                 except ValueError:
                     step_frac *= decay
                     continue
                 # loss of cost of policy cost from real/expected reward
                 loss_cost = self._loss_pi_cost(obs=obs, act=act, logp=logp, adv_c=adv_c)
                 # compute KL distance between new and old policy
                 q_dist = self._actor_critic.actor(obs)
@@ -162,15 +167,15 @@
         else:
             # if didn't find a step satisfy those conditions
             self._logger.log('INFO: no suitable step found...')
             step_direction = torch.zeros_like(step_direction)
             acceptance_step = 0
 
         self._logger.store(
-            **{
+            {
                 'Train/KL': kl,
             },
         )
 
         set_param_values_to_model(self._actor_critic.actor, theta_old)
         return step_frac * step_direction, acceptance_step
 
@@ -179,79 +184,61 @@
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_c: torch.Tensor,
     ) -> torch.Tensor:
         r"""Compute the performance of cost on this moment.
 
-        Detailedly, we compute the loss of cost of policy cost from real cost.
+        We compute the loss of cost of policy cost from real cost.
 
         .. math::
-            L = \mathbb{E}_{\pi} \left[ \frac{\pi^{'}(a|s)}{\pi(a|s)} A^C(s, a) \right]
 
-        where :math:`A^C(s, a)` is the cost advantage,
-        :math:`\pi(a|s)` is the old policy,
-        :math:`\pi^{'}(a|s)` is the current policy.
+            L = \mathbb{E}_{\pi} \left[ \frac{\pi^{'} (a|s)}{\pi (a|s)} A^C (s, a) \right]
+
+        where :math:`A^C (s, a)` is the cost advantage, :math:`\pi (a|s)` is the old policy,
+        and :math:`\pi^{'} (a|s)` is the current policy.
 
         Args:
-            obs (torch.Tensor): Observation.
-            act (torch.Tensor): Action.
-            logp (torch.Tensor): Log probability of action.
-            adv_c (torch.Tensor): Cost advantage.
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            act (torch.Tensor): The ``action`` sampled from buffer.
+            logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
+            adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            torch.Tensor: The loss of cost of policy cost from real cost.
+            The loss of the cost performance.
         """
         self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
         ratio = torch.exp(logp_ - logp)
         return (ratio * adv_c).mean()
 
-    # pylint: disable=invalid-name,too-many-arguments,too-many-locals
-    def _update_actor(
+    # pylint: disable=invalid-name
+    def _determine_case(
         self,
-        obs: torch.Tensor,
-        act: torch.Tensor,
-        logp: torch.Tensor,
-        adv_r: torch.Tensor,
-        adv_c: torch.Tensor,
-    ) -> None:
-        self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
-        theta_old = get_flat_params_from(self._actor_critic.actor)
-        self._actor_critic.actor.zero_grad()
-        loss_reward, info = self._loss_pi(obs, act, logp, adv_r)
-        loss_reward_before = distributed.dist_avg(loss_reward).item()
-        p_dist = self._actor_critic.actor(obs)
-
-        loss_reward.backward()
-        distributed.avg_grads(self._actor_critic.actor)
-
-        grad = -get_flat_gradients_from(self._actor_critic.actor)
-        x = conjugate_gradients(self._fvp, grad, self._cfgs.algo_cfgs.cg_iters)
-        assert torch.isfinite(x).all(), 'x is not finite'
-        xHx = x.dot(self._fvp(x))
-        assert xHx.item() >= 0, 'xHx is negative'
-        alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
-
-        self._actor_critic.zero_grad()
-        loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
-        loss_cost_before = distributed.dist_avg(loss_cost).item()
-
-        loss_cost.backward()
-        distributed.avg_grads(self._actor_critic.actor)
+        b_grads: torch.Tensor,
+        ep_costs: torch.Tensor,
+        q: torch.Tensor,
+        r: torch.Tensor,
+        s: torch.Tensor,
+    ) -> tuple[int, torch.Tensor, torch.Tensor]:
+        """Determine the case of the trust region update.
 
-        b_grad = get_flat_gradients_from(self._actor_critic.actor)
-        ep_costs = self._logger.get_stats('Metrics/EpCost')[0] - self._cfgs.algo_cfgs.cost_limit
-
-        p = conjugate_gradients(self._fvp, b_grad, self._cfgs.algo_cfgs.cg_iters)
-        q = xHx
-        r = grad.dot(p)
-        s = b_grad.dot(p)
+        Args:
+            b_grad (torch.Tensor): Gradient of the cost function.
+            ep_costs (torch.Tensor): Cost of the current episode.
+            q (torch.Tensor): The quadratic term of the quadratic approximation of the cost function.
+            r (torch.Tensor): The linear term of the quadratic approximation of the cost function.
+            s (torch.Tensor): The constant term of the quadratic approximation of the cost function.
 
-        if b_grad.dot(b_grad) <= 1e-6 and ep_costs < 0:
+        Returns:
+            optim_case: The case of the trust region update.
+            A: The quadratic term of the quadratic approximation of the cost function.
+            B: The linear term of the quadratic approximation of the cost function.
+        """
+        if b_grads.dot(b_grads) <= 1e-6 and ep_costs < 0:
             # feasible step and cost grad is zero: use plain TRPO update...
             A = torch.zeros(1)
             B = torch.zeros(1)
             optim_case = 4
         else:
             assert torch.isfinite(r).all(), 'r is not finite'
             assert torch.isfinite(s).all(), 's is not finite'
@@ -274,48 +261,64 @@
                 self._logger.log('Alert! Attempting feasible recovery!', 'yellow')
             else:
                 # x = 0 infeasible, and safety half space is outside trust region
                 # ==> whole trust region is infeasible, try to fail gracefully
                 optim_case = 0
                 self._logger.log('Alert! Attempting infeasible recovery!', 'red')
 
+        return optim_case, A, B
+
+    # pylint: disable=invalid-name, too-many-arguments, too-many-locals
+    def _step_direction(
+        self,
+        optim_case: int,
+        xHx: torch.Tensor,
+        x: torch.Tensor,
+        A: torch.Tensor,
+        B: torch.Tensor,
+        q: torch.Tensor,
+        p: torch.Tensor,
+        r: torch.Tensor,
+        s: torch.Tensor,
+        ep_costs: torch.Tensor,
+    ) -> tuple[torch.Tensor, ...]:
         if optim_case in (3, 4):
             # under 3 and 4 cases directly use TRPO method
             alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
             nu_star = torch.zeros(1)
             lambda_star = 1 / (alpha + 1e-8)
             step_direction = alpha * x
 
         elif optim_case in (1, 2):
 
-            def project(data: torch.Tensor, low: float, high: float) -> torch.Tensor:
+            def project(data: torch.Tensor, low: torch.Tensor, high: torch.Tensor) -> torch.Tensor:
                 """Project data to [low, high] interval."""
-                return torch.max(torch.min(data, torch.tensor(high)), torch.tensor(low))
+                return torch.clamp(data, low, high)
 
             #  analytical Solution to LQCLP, employ lambda,nu to compute final solution of OLOLQC
             #  λ=argmax(f_a(λ),f_b(λ)) = λa_star or λb_star
             #  computing formula shown in appendix, lambda_a and lambda_b
             lambda_a = torch.sqrt(A / B)
             lambda_b = torch.sqrt(q / (2 * self._cfgs.algo_cfgs.target_kl))
             # λa_star = Proj(lambda_a ,0 ~ r/c)  λb_star=Proj(lambda_b,r/c~ +inf)
             # where projection(str,b,c)=max(b,min(str,c))
             # may be regarded as a projection from effective region towards safety region
             r_num = r.item()
             eps_cost = ep_costs + 1e-8
             if ep_costs < 0:
-                lambda_a_star = project(lambda_a, 0.0, r_num / eps_cost)
-                lambda_b_star = project(lambda_b, r_num / eps_cost, torch.inf)
+                lambda_a_star = project(lambda_a, torch.as_tensor(0.0), r_num / eps_cost)
+                lambda_b_star = project(lambda_b, r_num / eps_cost, torch.as_tensor(torch.inf))
             else:
-                lambda_a_star = project(lambda_a, r_num / eps_cost, torch.inf)
-                lambda_b_star = project(lambda_b, 0.0, r_num / eps_cost)
+                lambda_a_star = project(lambda_a, r_num / eps_cost, torch.as_tensor(torch.inf))
+                lambda_b_star = project(lambda_b, torch.as_tensor(0.0), r_num / eps_cost)
 
-            def f_a(lam):
+            def f_a(lam: torch.Tensor) -> torch.Tensor:
                 return -0.5 * (A / (lam + 1e-8) + B * lam) - r * ep_costs / (s + 1e-8)
 
-            def f_b(lam):
+            def f_b(lam: torch.Tensor) -> torch.Tensor:
                 return -0.5 * (q / (lam + 1e-8) + 2 * self._cfgs.algo_cfgs.target_kl * lam)
 
             lambda_star = (
                 lambda_a_star if f_a(lambda_a_star) >= f_b(lambda_b_star) else lambda_b_star
             )
 
             # discard all negative values with torch.clamp(x, min=0)
@@ -327,17 +330,99 @@
         else:  # case == 0
             # purely decrease costs
             # without further check
             lambda_star = torch.zeros(1)
             nu_star = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (s + 1e-8))
             step_direction = -nu_star * p
 
+        return step_direction, lambda_star, nu_star
+
+    # pylint: disable=invalid-name,too-many-arguments,too-many-locals
+    def _update_actor(
+        self,
+        obs: torch.Tensor,
+        act: torch.Tensor,
+        logp: torch.Tensor,
+        adv_r: torch.Tensor,
+        adv_c: torch.Tensor,
+    ) -> None:
+        """Update policy network.
+
+        Constrained Policy Optimization updates policy network using the
+        `conjugate gradient <https://en.wikipedia.org/wiki/Conjugate_gradient_method>`_ algorithm,
+        following the steps:
+
+        - Compute the gradient of the policy.
+        - Compute the step direction.
+        - Search for a step size that satisfies the constraint.
+        - Update the policy network.
+
+        Args:
+            obs (torch.Tensor): The observation tensor.
+            act (torch.Tensor): The action tensor.
+            logp (torch.Tensor): The log probability of the action.
+            adv_r (torch.Tensor): The reward advantage tensor.
+            adv_c (torch.Tensor): The cost advantage tensor.
+        """
+        self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
+        theta_old = get_flat_params_from(self._actor_critic.actor)
+        self._actor_critic.actor.zero_grad()
+        loss_reward = self._loss_pi(obs, act, logp, adv_r)
+        loss_reward_before = distributed.dist_avg(loss_reward).item()
+        p_dist = self._actor_critic.actor(obs)
+
+        loss_reward.backward()
+        distributed.avg_grads(self._actor_critic.actor)
+
+        grads = -get_flat_gradients_from(self._actor_critic.actor)
+        x = conjugate_gradients(self._fvp, grads, self._cfgs.algo_cfgs.cg_iters)
+        assert torch.isfinite(x).all(), 'x is not finite'
+        xHx = x.dot(self._fvp(x))
+        assert xHx.item() >= 0, 'xHx is negative'
+        alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
+
+        self._actor_critic.zero_grad()
+        loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
+        loss_cost_before = distributed.dist_avg(loss_cost).item()
+
+        loss_cost.backward()
+        distributed.avg_grads(self._actor_critic.actor)
+
+        b_grads = get_flat_gradients_from(self._actor_critic.actor)
+        ep_costs = self._logger.get_stats('Metrics/EpCost')[0] - self._cfgs.algo_cfgs.cost_limit
+
+        p = conjugate_gradients(self._fvp, b_grads, self._cfgs.algo_cfgs.cg_iters)
+        q = xHx
+        r = grads.dot(p)
+        s = b_grads.dot(p)
+
+        optim_case, A, B = self._determine_case(
+            b_grads=b_grads,
+            ep_costs=ep_costs,
+            q=q,
+            r=r,
+            s=s,
+        )
+
+        step_direction, lambda_star, nu_star = self._step_direction(
+            optim_case=optim_case,
+            xHx=xHx,
+            x=x,
+            A=A,
+            B=B,
+            q=q,
+            p=p,
+            r=r,
+            s=s,
+            ep_costs=ep_costs,
+        )
+
         step_direction, accept_step = self._cpo_search_step(
             step_direction=step_direction,
-            grad=grad,
+            grads=grads,
             p_dist=p_dist,
             obs=obs,
             act=act,
             logp=logp,
             adv_r=adv_r,
             adv_c=adv_c,
             loss_reward_before=loss_reward_before,
@@ -347,31 +432,28 @@
             optim_case=optim_case,
         )
 
         theta_new = theta_old + step_direction
         set_param_values_to_model(self._actor_critic.actor, theta_new)
 
         with torch.no_grad():
-            loss_reward, info = self._loss_pi(obs, act, logp, adv_r)
+            loss_reward = self._loss_pi(obs, act, logp, adv_r)
             loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
             loss = loss_reward + loss_cost
 
         self._logger.store(
-            **{
+            {
                 'Loss/Loss_pi': loss.item(),
-                'Train/Entropy': info['entropy'],
-                'Train/PolicyRatio': info['ratio'],
-                'Train/PolicyStd': info['std'],
                 'Misc/AcceptanceStep': accept_step,
                 'Misc/Alpha': alpha.item(),
                 'Misc/FinalStepNorm': step_direction.norm().mean().item(),
                 'Misc/xHx': xHx.mean().item(),
                 'Misc/H_inv_g': x.norm().item(),  # H^-1 g
-                'Misc/gradient_norm': torch.norm(grad).mean().item(),
-                'Misc/cost_gradient_norm': torch.norm(b_grad).mean().item(),
+                'Misc/gradient_norm': torch.norm(grads).mean().item(),
+                'Misc/cost_gradient_norm': torch.norm(b_grads).mean().item(),
                 'Misc/Lambda_star': lambda_star.item(),
                 'Misc/Nu_star': nu_star.item(),
                 'Misc/OptimCase': int(optim_case),
                 'Misc/A': A.item(),
                 'Misc/B': B.item(),
                 'Misc/q': q.item(),
                 'Misc/r': r.item(),
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/on_policy/second_order/pcpo.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/pcpo.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,78 +44,77 @@
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_r: torch.Tensor,
         adv_c: torch.Tensor,
     ) -> None:
         """Update policy network.
 
-        PCPO updates policy network using the conjugate gradient algorithm,
-        following the steps:
+        PCPO updates policy network using the conjugate gradient algorithm, following the steps:
 
         - Compute the gradient of the policy.
         - Compute the step direction.
         - Search for a step size that satisfies the constraint. (Both KL divergence and cost limit).
         - Update the policy network.
 
         Args:
             obs (torch.Tensor): The observation tensor.
             act (torch.Tensor): The action tensor.
-            log_p (torch.Tensor): The log probability of the action.
-            adv (torch.Tensor): The advantage tensor.
-            cost_adv (torch.Tensor): The cost advantage tensor.
+            logp (torch.Tensor): The log probability of the action.
+            adv_r (torch.Tensor): The reward advantage tensor.
+            adv_c (torch.Tensor): The cost advantage tensor.
         """
         # pylint: disable=invalid-name
         self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
         theta_old = get_flat_params_from(self._actor_critic.actor)
         self._actor_critic.actor.zero_grad()
-        loss_reward, info = self._loss_pi(obs, act, logp, adv_r)
+        loss_reward = self._loss_pi(obs, act, logp, adv_r)
         loss_reward_before = distributed.dist_avg(loss_reward).item()
         p_dist = self._actor_critic.actor(obs)
 
         loss_reward.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
-        grad = -get_flat_gradients_from(self._actor_critic.actor)
-        x = conjugate_gradients(self._fvp, grad, self._cfgs.algo_cfgs.cg_iters)
+        grads = -get_flat_gradients_from(self._actor_critic.actor)
+        x = conjugate_gradients(self._fvp, grads, self._cfgs.algo_cfgs.cg_iters)
         assert torch.isfinite(x).all(), 'x is not finite'
         xHx = x.dot(self._fvp(x))
         H_inv_g = self._fvp(x)
         assert xHx.item() >= 0, 'xHx is negative'
         alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
 
         self._actor_critic.zero_grad()
         loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
         loss_cost_before = distributed.dist_avg(loss_cost).item()
 
         loss_cost.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
-        b_grad = get_flat_gradients_from(self._actor_critic.actor)
+        b_grads = get_flat_gradients_from(self._actor_critic.actor)
         ep_costs = self._logger.get_stats('Metrics/EpCost')[0] - self._cfgs.algo_cfgs.cost_limit
 
         self._logger.log(f'c = {ep_costs}')
-        self._logger.log(f'b^T b = {b_grad.dot(b_grad).item()}')
+        self._logger.log(f'b^T b = {b_grads.dot(b_grads).item()}')
 
-        p = conjugate_gradients(self._fvp, b_grad, self._cfgs.algo_cfgs.cg_iters)
+        p = conjugate_gradients(self._fvp, b_grads, self._cfgs.algo_cfgs.cg_iters)
         q = xHx
-        r = grad.dot(p)
-        s = b_grad.dot(p)
+        r = grads.dot(p)
+        s = b_grads.dot(p)
 
         step_direction = (
             torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (q + 1e-8)) * H_inv_g
             - torch.clamp_min(
                 (torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / q) * r + ep_costs) / s,
                 torch.tensor(0.0, device=self._device),
             )
             * p
         )  # pylint: disable=invalid-name
 
         step_direction, accept_step = self._cpo_search_step(
             step_direction=step_direction,
-            grad=grad,
+            grads=grads,
             p_dist=p_dist,
             obs=obs,
             act=act,
             logp=logp,
             adv_r=adv_r,
             adv_c=adv_c,
             loss_reward_before=loss_reward_before,
@@ -123,31 +122,28 @@
             total_steps=200,
             violation_c=ep_costs,
         )
         theta_new = theta_old + step_direction
         set_param_values_to_model(self._actor_critic.actor, theta_new)
 
         with torch.no_grad():
-            loss_reward, info = self._loss_pi(obs, act, logp, adv_r)
+            loss_reward = self._loss_pi(obs, act, logp, adv_r)
             loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
             loss = loss_reward + loss_cost
 
         self._logger.store(
-            **{
+            {
                 'Loss/Loss_pi': loss.item(),
-                'Train/Entropy': info['entropy'],
-                'Train/PolicyRatio': info['ratio'],
-                'Train/PolicyStd': info['std'],
                 'Misc/AcceptanceStep': accept_step,
                 'Misc/Alpha': alpha.item(),
                 'Misc/FinalStepNorm': step_direction.norm().mean().item(),
                 'Misc/xHx': xHx.mean().item(),
                 'Misc/H_inv_g': x.norm().item(),  # H^-1 g
-                'Misc/gradient_norm': torch.norm(grad).mean().item(),
-                'Misc/cost_gradient_norm': torch.norm(b_grad).mean().item(),
+                'Misc/gradient_norm': torch.norm(grads).mean().item(),
+                'Misc/cost_gradient_norm': torch.norm(b_grads).mean().item(),
                 'Misc/Lambda_star': 1.0,
                 'Misc/Nu_star': 1.0,
                 'Misc/OptimCase': int(1),
                 'Misc/A': 1.0,
                 'Misc/B': 1.0,
                 'Misc/q': q.item(),
                 'Misc/r': r.item(),
```

### Comparing `omnisafe-0.3.0/omnisafe/algorithms/registry.py` & `omnisafe-0.4.0/omnisafe/algorithms/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,60 +10,58 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Registry for algorithms."""
 
+from __future__ import annotations
+
 import inspect
+from typing import Any
 
 
 class Registry:
     """A registry to map strings to classes.
 
     Args:
         name (str): Registry name.
     """
 
-    def __init__(self, name) -> None:
-        self._name = name
-        self._module_dict = {}
-
-    def __repr__(self) -> str:
-        return (
-            f'{self.__class__.__name__ }(name={self._name}, items={list(self._module_dict.keys())})'
-        )
+    def __init__(self, name: str) -> None:
+        """Initialize an instance of :class:`Registry`."""
+        self._name: str = name
+        self._module_dict: dict[str, type] = {}
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Return the name of the registry."""
         return self._name
 
-    @property
-    def module_dict(self):
-        """Return a dict mapping names to classes."""
-        return self._module_dict
-
-    def get(self, key):
+    def get(self, key: str) -> Any:
         """Get the class that has been registered under the given key."""
-        return self._module_dict.get(key, None)
+        res = self._module_dict.get(key)
+        if res is None:
+            raise KeyError(f'{key} is not in the {self.name} registry')
+        return res
 
-    def _register_module(self, module_class):
+    def _register_module(self, module_class: type) -> None:
         """Register a module.
+
         Args:
-            module (:obj:`nn.Module`): Module to be registered.
+            module_class (type): Module to be registered.
         """
         if not inspect.isclass(module_class):
             raise TypeError(f'module must be a class, but got {type(module_class)}')
         module_name = module_class.__name__
         if module_name in self._module_dict:
             raise KeyError(f'{module_name} is already registered in {self.name}')
         self._module_dict[module_name] = module_class
 
-    def register(self, cls):
+    def register(self, cls: type) -> type:
         """Register a module class."""
         self._register_module(cls)
         return cls
 
 
 REGISTRY = Registry('OmniSafe')
```

### Comparing `omnisafe-0.3.0/omnisafe/common/__init__.py` & `omnisafe-0.4.0/omnisafe/common/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/common/buffer/__init__.py` & `omnisafe-0.4.0/omnisafe/common/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/common/buffer/base.py` & `omnisafe-0.4.0/omnisafe/common/buffer/vector_offpolicy_buffer.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,139 +8,131 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Abstract base class for buffer."""
+"""Implementation of VectorOffPolicyBuffer."""
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-
 import torch
 from gymnasium.spaces import Box
 
-from omnisafe.typing import OmnisafeSpace
+from omnisafe.common.buffer.offpolicy_buffer import OffPolicyBuffer
+from omnisafe.typing import DEVICE_CPU, OmnisafeSpace
 
 
-class BaseBuffer(ABC):
-    """Abstract base class for buffer."""
+class VectorOffPolicyBuffer(OffPolicyBuffer):
+    """Vectorized on-policy buffer.
 
-    def __init__(
-        self,
-        obs_space: OmnisafeSpace,
-        act_space: OmnisafeSpace,
-        size: int,
-        device: torch.device = 'cpu',
-    ) -> None:
-        """Initialize the buffer.
+    The vector-off-policy buffer is a vectorized version of the off-policy buffer. It stores the
+    data in a single tensor, and the data of each environment is stored in a separate column.
 
-        .. warning::
-            The buffer only supports Box spaces.
+    .. warning::
+        The buffer only supports Box spaces.
 
-        In  base buffer, we store the following data:
+    Args:
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        size (int): The size of the buffer.
+        batch_size (int): The batch size of the buffer.
+        num_envs (int): The number of environments.
+        device (torch.device, optional): The device of the buffer. Defaults to
+            ``torch.device('cpu')``.
 
-        .. list-table::
+    Attributes:
+        data (dict[str, torch.Tensor]): The data of the buffer.
 
-            *   -   Name
-                -   Shape
-                -   Dtype
-                -   Description
-            *   -   obs
-                -   (size, obs_space.shape)
-                -   torch.float32
-                -   The observation.
-            *   -   act
-                -   (size, act_space.shape)
-                -   torch.float32
-                -   The action.
-            *   -   reward
-                -   (size, )
-                -   torch.float32
-                -   Single step reward.
-            *   -   cost
-                -   (size, )
-                -   torch.float32
-                -   Single step cost.
-            *   -   done
-                -   (size, )
-                -   torch.float32
-                -   Whether the episode is done.
+    Raises:
+        NotImplementedError: If the observation space or the action space is not Box.
+        NotImplementedError: If the action space or the action space is not Box.
+    """
 
-        Args:
-            obs_space (OmnisafeSpace): The observation space.
-            act_space (OmnisafeSpace): The action space.
-            size (int): The size of the buffer.
-            device (torch.device): The device of the buffer.
-
-        Attributes:
-            data (dict[str, torch.Tensor]): The data of the buffer.
-            _size (int): The size of the buffer.
-            _device (torch.device): The device of the buffer.
-
-        """
-        device = torch.device(device)
+    def __init__(  # pylint: disable=super-init-not-called,too-many-arguments
+        self,
+        obs_space: OmnisafeSpace,
+        act_space: OmnisafeSpace,
+        size: int,
+        batch_size: int,
+        num_envs: int,
+        device: torch.device = DEVICE_CPU,
+    ) -> None:
+        """Initialize an instance of :class:`VectorOffPolicyBuffer`."""
+        self._num_envs: int = num_envs
+        self._ptr: int = 0
+        self._size: int = 0
+        self._max_size: int = size
+        self._batch_size: int = batch_size
+        self._device: torch.device = device
         if isinstance(obs_space, Box):
-            obs_buf = torch.zeros((size, *obs_space.shape), dtype=torch.float32, device=device)
+            obs_buf = torch.zeros(
+                (size, num_envs, *obs_space.shape),
+                dtype=torch.float32,
+                device=device,
+            )
+            next_obs_buf = torch.zeros(
+                (size, num_envs, *obs_space.shape),
+                dtype=torch.float32,
+                device=device,
+            )
         else:
             raise NotImplementedError
+
         if isinstance(act_space, Box):
-            act_buf = torch.zeros((size, *act_space.shape), dtype=torch.float32, device=device)
+            act_buf = torch.zeros(
+                (size, num_envs, *act_space.shape),
+                dtype=torch.float32,
+                device=device,
+            )
         else:
             raise NotImplementedError
 
-        self.data: dict[str, torch.Tensor] = {
+        self.data = {
             'obs': obs_buf,
             'act': act_buf,
-            'reward': torch.zeros(size, dtype=torch.float32, device=device),
-            'cost': torch.zeros(size, dtype=torch.float32, device=device),
-            'done': torch.zeros(size, dtype=torch.float32, device=device),
+            'reward': torch.zeros((size, num_envs), dtype=torch.float32, device=device),
+            'cost': torch.zeros((size, num_envs), dtype=torch.float32, device=device),
+            'done': torch.zeros((size, num_envs), dtype=torch.float32, device=device),
+            'next_obs': next_obs_buf,
         }
-        self._size = size
-        self._device = device
-
-    @property
-    def device(self) -> torch.device:
-        """Return the device of the buffer."""
-        return self._device
 
     @property
-    def size(self) -> int:
-        """Return the size of the buffer."""
-        return self._size
-
-    def __len__(self) -> int:
-        """Return the length of the buffer."""
-        return self._size
+    def num_envs(self) -> int:
+        """The number of parallel environments."""
+        return self._num_envs
 
-    def add_field(self, name: str, shape: tuple, dtype: torch.dtype):
+    def add_field(self, name: str, shape: tuple[int, ...], dtype: torch.dtype) -> None:
         """Add a field to the buffer.
 
-        Example:
+        Examples:
             >>> buffer = BaseBuffer(...)
             >>> buffer.add_field('new_field', (2, 3), torch.float32)
             >>> buffer.data['new_field'].shape
             >>> (buffer.size, 2, 3)
 
         Args:
             name (str): The name of the field.
-            shape (tuple): The shape of the field.
+            shape (tuple of int): The shape of the field.
             dtype (torch.dtype): The dtype of the field.
         """
-        self.data[name] = torch.zeros((self._size, *shape), dtype=dtype, device=self._device)
-
-    @abstractmethod
-    def store(self, **data: torch.Tensor):
-        """Store a transition in the buffer.
+        self.data[name] = torch.zeros(
+            (self._max_size, self._num_envs, *shape),
+            dtype=dtype,
+            device=self._device,
+        )
 
-        .. warning::
-            This is an abstract method.
+    def sample_batch(self) -> dict[str, torch.Tensor]:
+        """Sample a batch of data from the buffer.
 
-        Example:
-            >>> buffer = BaseBuffer(...)
-            >>> buffer.store(obs=obs, act=act, reward=reward, cost=cost, done=done)
-
-        Args:
-            data (torch.Tensor): The data to store.
+        Returns:
+            The sampled batch of data.
         """
+        idx = torch.randint(
+            0,
+            self._size,
+            (self._batch_size * self._num_envs,),
+            device=self._device,
+        )
+        env_idx = torch.arange(self._num_envs, device=self._device).repeat(self._batch_size)
+        return {key: value[idx, env_idx] for key, value in self.data.items()}
```

### Comparing `omnisafe-0.3.0/omnisafe/common/buffer/offpolicy_buffer.py` & `omnisafe-0.4.0/omnisafe/common/buffer/offpolicy_buffer.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,63 +16,52 @@
 
 from __future__ import annotations
 
 import torch
 from gymnasium.spaces import Box
 
 from omnisafe.common.buffer.base import BaseBuffer
-from omnisafe.typing import OmnisafeSpace
+from omnisafe.typing import DEVICE_CPU, OmnisafeSpace
 
 
 class OffPolicyBuffer(BaseBuffer):
-    """A ReplayBuffer for off_policy Algorithms."""
+    r"""A ReplayBuffer for off_policy Algorithms.
+
+    .. warning::
+        The buffer only supports Box spaces.
+
+    Compared to the base buffer, the off-policy buffer stores extra data:
+
+    +----------+---------------------------+---------------+----------------------------------------+
+    | Name     | Shape                     | Dtype         | Description                            |
+    +==========+===========================+===============+========================================+
+    | next_obs | (size, \*obs_space.shape) | torch.float32 | The next observation from environment. |
+    +----------+---------------------------+---------------+----------------------------------------+
+
+    Args:
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        size (int): The size of the buffer.
+        batch_size (int): The batch size of the buffer.
+        device (torch.device, optional): The device of the buffer. Defaults to
+            ``torch.device('cpu')``.
+
+    Attributes:
+        data (dict[str, torch.Tensor]): The data stored in the buffer.
+    """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         size: int,
         batch_size: int,
-        device: torch.device = 'cpu',
+        device: torch.device = DEVICE_CPU,
     ) -> None:
-        """Initialize the off policy buffer.
-
-        .. warning::
-            The buffer only supports Box spaces.
-
-        Compared to the base buffer, the off-policy buffer stores extra data:
-
-        .. list-table::
-
-            *   -   Name
-                -   Shape
-                -   Dtype
-                -   Description
-            *   -   next_obs
-                -   (batch_size, obs_space.shape)
-                -   torch.float32
-                -   The next observation.
-
-        Args:
-            obs_space (OmnisafeSpace): The observation space.
-            act_space (OmnisafeSpace): The action space.
-            size (int): The size of the buffer.
-            batch_size (int): The batch size of the buffer.
-            device (torch.device, optional): The device of the buffer. Defaults to
-                torch.device('cpu').
-
-        Attributes:
-            data (dict[str, torch.Tensor]): The data stored in the buffer.
-            _ptr (int): The pointer of the buffer.
-            _size (int): The size of the buffer.
-            _max_size (int): The maximum size of the buffer.
-            _batch_size (int): The batch size of the buffer.
-
-        """
-        device = torch.device(device)
+        """Initialize an instance of :class:`OffPolicyBuffer`."""
         super().__init__(obs_space, act_space, size, device)
         if isinstance(obs_space, Box):
             self.data['next_obs'] = torch.zeros(
                 (size, *obs_space.shape),
                 dtype=torch.float32,
                 device=device,
             )
@@ -86,34 +75,43 @@
 
         assert (
             self._max_size > self._batch_size
         ), 'The size of the buffer must be larger than the batch size.'
 
     @property
     def max_size(self) -> int:
-        """Return the maximum size of the buffer."""
+        """Return the max size of the buffer."""
         return self._max_size
 
     @property
+    def size(self) -> int:
+        """Return the current size of the buffer."""
+        return self._size
+
+    @property
     def batch_size(self) -> int:
         """Return the batch size of the buffer."""
         return self._batch_size
 
-    def store(self, **data: torch.Tensor):
+    def store(self, **data: torch.Tensor) -> None:
         """Store data into the buffer.
 
         .. hint::
-            The ReplayBuffer is a circular buffer. When the buffer is full, the
-            oldest data will be overwritten.
+            The ReplayBuffer is a circular buffer. When the buffer is full, the oldest data will be
+            overwritten.
 
         Args:
             data (torch.Tensor): The data to be stored.
         """
         for key, value in data.items():
             self.data[key][self._ptr] = value
         self._ptr = (self._ptr + 1) % self._max_size
         self._size = min(self._size + 1, self._max_size)
 
     def sample_batch(self) -> dict[str, torch.Tensor]:
-        """Sample a batch of data from the buffer."""
+        """Sample a batch of data from the buffer.
+
+        Returns:
+            The sampled batch of data.
+        """
         idxs = torch.randint(0, self._size, (self._batch_size,))
         return {key: value[idxs] for key, value in self.data.items()}
```

### Comparing `omnisafe-0.3.0/omnisafe/common/buffer/onpolicy_buffer.py` & `omnisafe-0.4.0/omnisafe/common/buffer/onpolicy_buffer.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,150 +15,124 @@
 """Implementation of OnPolicyBuffer."""
 
 from __future__ import annotations
 
 import torch
 
 from omnisafe.common.buffer.base import BaseBuffer
-from omnisafe.typing import AdvatageEstimator, OmnisafeSpace
+from omnisafe.typing import DEVICE_CPU, AdvatageEstimator, OmnisafeSpace
 from omnisafe.utils import distributed
 from omnisafe.utils.math import discount_cumsum
 
 
 class OnPolicyBuffer(BaseBuffer):  # pylint: disable=too-many-instance-attributes
     """A buffer for storing trajectories experienced by an agent interacting with the environment.
 
-    Besides, The buffer also provides the functionality of calculating the advantages of state-action pairs,
-    ranging from ``GAE``, ``GAE-RTG`` ,``V-trace`` to ``Plain`` method.
+    Besides, The buffer also provides the functionality of calculating the advantages of
+    state-action pairs, ranging from ``GAE``, ``GAE-RTG`` ,``V-trace`` to ``Plain`` method.
+
+    .. warning::
+        The buffer only supports Box spaces.
+
+    Compared to the base buffer, the on-policy buffer stores extra data:
+
+    +----------------+---------+---------------+----------------------------------------+
+    | Name           | Shape   | Dtype         | Shape                                  |
+    +================+=========+===============+========================================+
+    | discounted_ret | (size,) | torch.float32 | The discounted sum of return.          |
+    +----------------+---------+---------------+----------------------------------------+
+    | value_r        | (size,) | torch.float32 | The value estimated by reward critic.  |
+    +----------------+---------+---------------+----------------------------------------+
+    | value_c        | (size,) | torch.float32 | The value estimated by cost critic.    |
+    +----------------+---------+---------------+----------------------------------------+
+    | adv_r          | (size,) | torch.float32 | The advantage of the reward.           |
+    +----------------+---------+---------------+----------------------------------------+
+    | adv_c          | (size,) | torch.float32 | The advantage of the cost.             |
+    +----------------+---------+---------------+----------------------------------------+
+    | target_value_r | (size,) | torch.float32 | The target value of the reward critic. |
+    +----------------+---------+---------------+----------------------------------------+
+    | target_value_c | (size,) | torch.float32 | The target value of the cost critic.   |
+    +----------------+---------+---------------+----------------------------------------+
+    | logp           | (size,) | torch.float32 | The log probability of the action.     |
+    +----------------+---------+---------------+----------------------------------------+
+
+    Args:
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        size (int): The size of the buffer.
+        gamma (float): The discount factor.
+        lam (float): The lambda factor for calculating the advantages.
+        lam_c (float): The lambda factor for calculating the advantages of the critic.
+        advantage_estimator (AdvatageEstimator): The advantage estimator.
+        penalty_coefficient (float, optional): The penalty coefficient. Defaults to 0.
+        standardized_adv_r (bool, optional): Whether to standardize the advantages of the actor.
+            Defaults to False.
+        standardized_adv_c (bool, optional): Whether to standardize the advantages of the critic.
+            Defaults to False.
+        device (torch.device, optional): The device to store the data. Defaults to
+            ``torch.device('cpu')``.
+
+    Attributes:
+        ptr (int): The pointer of the buffer.
+        path_start (int): The start index of the current path.
+        max_size (int): The maximum size of the buffer.
+        data (dict): The data stored in the buffer.
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        device (torch.device): The device to store the data.
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         size: int,
         gamma: float,
         lam: float,
         lam_c: float,
         advantage_estimator: AdvatageEstimator,
         penalty_coefficient: float = 0,
         standardized_adv_r: bool = False,
         standardized_adv_c: bool = False,
-        device: torch.device = 'cpu',
+        device: torch.device = DEVICE_CPU,
     ) -> None:
-        """Initialize the on-policy buffer.
-
-        .. warning::
-            The buffer only supports Box spaces.
-
-        Compared to the base buffer, the on-policy buffer stores extra data:
-
-        .. list-table::
-
-            *   -   Name
-                -   Shape
-                -   Dtype
-                -   Description
-            *   -   discounted_ret
-                -   (size, )
-                -   torch.float32
-                -   The discounted return.
-            *   -   target_value_r
-                -   (size, )
-                -   torch.float32
-                -   The target value of the reward critic.
-            *   -   adv_r
-                -   (size, )
-                -   torch.float32
-                -   The advantage of the reward.
-            *   -   value_r
-                -   (size, )
-                -   torch.float32
-                -   The value estimated by reward critic.
-            *   -   target_value_c
-                -   (size, )
-                -   torch.float32
-                -   The target value of the cost critic.
-            *   -   adv_c
-                -   (size, )
-                -   torch.float32
-                -   The advantage of the critic.
-            *   -   value_c
-                -   (size, )
-                -   torch.float32
-                -   The value estimated by cost critic.
-            *   -   logp
-                -   (size, )
-                -   torch.float32
-                -   The log probability of the action.
-
-        Args:
-            obs_space (OmnisafeSpace): The observation space.
-            act_space (OmnisafeSpace): The action space.
-            size (int): The size of the buffer.
-            gamma (float): The discount factor.
-            lam (float): The lambda factor for calculating the advantages.
-            lam_c (float): The lambda factor for calculating the advantages of the critic.
-            advantage_estimator (AdvatageEstimator): The advantage estimator.
-            penalty_coefficient (float, optional): The penalty coefficient. Defaults to 0.
-            standardized_adv_r (bool, optional): Whether to standardize the advantages of the actor. Defaults to False.
-            standardized_adv_c (bool, optional): Whether to standardize the advantages of the critic. Defaults to False.
-            device (torch.device, optional): The device to store the data. Defaults to torch.device('cpu').
-
-        Attributes:
-            _standardized_adv_r (bool): Whether to standardize the advantages of the actor.
-            _standardized_adv_c (bool): Whether to standardize the advantages of the critic.
-            _gamma (float): The discount factor.
-            _lam (float): The lambda factor for calculating the advantages.
-            _lam_c (float): The lambda factor for calculating the advantages of the critic.
-            _penalty_coefficient (float): The penalty coefficient.
-            _advantage_estimator (AdvatageEstimator): The advantage estimator.
-            ptr (int): The pointer of the buffer.
-            path_start (int): The start index of the current path.
-            max_size (int): The maximum size of the buffer.
-            data (dict): The data stored in the buffer.
-            obs_space (OmnisafeSpace): The observation space.
-            act_space (OmnisafeSpace): The action space.
-            device (torch.device): The device to store the data.
-
-        """
-        device = torch.device(device)
+        """Initialize an instance of :class:`OnPolicyBuffer`."""
         super().__init__(obs_space, act_space, size, device)
-        self._standardized_adv_r = standardized_adv_r
-        self._standardized_adv_c = standardized_adv_c
+
+        self._standardized_adv_r: bool = standardized_adv_r
+        self._standardized_adv_c: bool = standardized_adv_c
         self.data['adv_r'] = torch.zeros((size,), dtype=torch.float32, device=device)
         self.data['discounted_ret'] = torch.zeros((size,), dtype=torch.float32, device=device)
         self.data['value_r'] = torch.zeros((size,), dtype=torch.float32, device=device)
         self.data['target_value_r'] = torch.zeros((size,), dtype=torch.float32, device=device)
         self.data['adv_c'] = torch.zeros((size,), dtype=torch.float32, device=device)
         self.data['value_c'] = torch.zeros((size,), dtype=torch.float32, device=device)
         self.data['target_value_c'] = torch.zeros((size,), dtype=torch.float32, device=device)
         self.data['logp'] = torch.zeros((size,), dtype=torch.float32, device=device)
 
-        self._gamma = gamma
-        self._lam = lam
-        self._lam_c = lam_c
-        self._penalty_coefficient = penalty_coefficient
-        self._advantage_estimator = advantage_estimator
-
+        self._gamma: float = gamma
+        self._lam: float = lam
+        self._lam_c: float = lam_c
+        self._penalty_coefficient: float = penalty_coefficient
+        self._advantage_estimator: AdvatageEstimator = advantage_estimator
         self.ptr: int = 0
         self.path_start_idx: int = 0
-        self.max_size = size
+        self.max_size: int = size
 
         assert self._penalty_coefficient >= 0, 'penalty_coefficient must be non-negative!'
         assert self._advantage_estimator in ['gae', 'gae-rtg', 'vtrace', 'plain']
 
     @property
     def standardized_adv_r(self) -> bool:
-        """Get the standardized_adv_r."""
+        """Whether to standardize the advantages of the actor."""
         return self._standardized_adv_r
 
     @property
     def standardized_adv_c(self) -> bool:
-        """Get the standardized_adv_c."""
+        """Whether to standardize the advantages of the critic."""
         return self._standardized_adv_c
 
     def store(self, **data: torch.Tensor) -> None:
         """Store data into the buffer.
 
         .. warning::
             The total size of the data must be less than the buffer size.
@@ -179,24 +153,23 @@
         """Finish the current path and calculate the advantages of state-action pairs.
 
         On-policy algorithms need to calculate the advantages of state-action pairs
         after the path is finished. This function calculates the advantages of
         state-action pairs and stores them in the buffer, following the steps:
 
         .. hint::
-
             #. Calculate the discounted return.
             #. Calculate the advantages of the reward.
             #. Calculate the advantages of the cost.
 
         Args:
             last_value_r (torch.Tensor, optional): The value of the last state of the current path.
-            Defaults to torch.zeros(1).
+                Defaults to torch.zeros(1).
             last_value_c (torch.Tensor, optional): The value of the last state of the current path.
-            Defaults to torch.zeros(1).
+                Defaults to torch.zeros(1).
         """
         if last_value_r is None:
             last_value_r = torch.zeros(1, device=self._device)
         if last_value_c is None:
             last_value_c = torch.zeros(1, device=self._device)
 
         path_slice = slice(self.path_start_idx, self.ptr)
@@ -229,38 +202,36 @@
 
         self.path_start_idx = self.ptr
 
     def get(self) -> dict[str, torch.Tensor]:
         """Get the data in the buffer.
 
         .. hint::
+            We provide a trick to standardize the advantages of state-action pairs. We calculate the
+            mean and standard deviation of the advantages of state-action pairs and then standardize
+            the advantages of state-action pairs. You can turn on this trick by setting the
+            ``standardized_adv_r`` to ``True``. The same trick is applied to the advantages of the
+            cost.
 
-            We provide a trick to standardize the advantages of state-action pairs.
-            We calculate the mean and standard deviation of the advantages of state-action pairs
-            and then standardize the advantages of state-action pairs.
-            You can turn on this trick by setting the ``standardized_adv_r`` to ``True``.
-            The same trick is applied to the advantages of the cost.
-
+        Returns:
+            The data stored and calculated in the buffer.
         """
         self.ptr, self.path_start_idx = 0, 0
 
         data = {
             'obs': self.data['obs'],
             'act': self.data['act'],
             'target_value_r': self.data['target_value_r'],
             'adv_r': self.data['adv_r'],
             'logp': self.data['logp'],
             'discounted_ret': self.data['discounted_ret'],
             'adv_c': self.data['adv_c'],
             'target_value_c': self.data['target_value_c'],
         }
 
-        # self.data['adv_r'] = torch.zeros_like(self.data['adv_r'])
-        # self.data['adv_c'] = torch.zeros_like(self.data['adv_c'])
-
         adv_mean, adv_std, *_ = distributed.dist_statistics_scalar(data['adv_r'])
         cadv_mean, *_ = distributed.dist_statistics_scalar(data['adv_c'])
         if self._standardized_adv_r:
             data['adv_r'] = (data['adv_r'] - adv_mean) / (adv_std + 1e-8)
         if self._standardized_adv_c:
             data['adv_c'] = data['adv_c'] - cadv_mean
 
@@ -271,60 +242,64 @@
         values: torch.Tensor,
         rewards: torch.Tensor,
         lam: float,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         r"""Compute the estimated advantage.
 
         Three methods are supported:
+
         - GAE (Generalized Advantage Estimation)
 
-        GAE is a variance reduction method for the actor-critic algorithm.
-        It is proposed in the paper `High-Dimensional Continuous Control Using Generalized Advantage Estimation
-        <https://arxiv.org/abs/1506.02438>`_.
+            GAE is a variance reduction method for the actor-critic algorithm. It is proposed in the
+            paper `High-Dimensional Continuous Control Using Generalized Advantage Estimation <https://arxiv.org/abs/1506.02438>`_.
 
-        GAE calculates the advantage using the following formula:
+            GAE calculates the advantage using the following formula:
 
-        .. math::
-            A_t = \sum_{k=0}^{n-1} (\lambda \gamma)^k \delta_{t+k}
+            .. math::
+
+                A_t = \sum_{k=0}^{n-1} (\lambda \gamma)^k \delta_{t+k}
 
-        where :math:`\delta_{t+k} = r_{t+k} + \gamma*V(s_{t+k+1}) - V(s_{t+k})`
-        When :math:`\lambda =1`, GAE reduces to the Monte Carlo method,
-        which is unbiased but has high variance.
-        When :math:`\lambda =0`, GAE reduces to the TD(1) method,
-        which is biased but has low variance.
+            where :math:`\delta_{t+k} = r_{t+k} + \gamma*V(s_{t+k+1}) - V(s_{t+k})`. When
+            :math:`\lambda =1`, GAE reduces to the Monte Carlo method, which is unbiased but has high
+            variance. When :math:`\lambda =0`, GAE reduces to the TD(1) method, which is biased but has
+            low variance.
 
         - V-trace
 
-        V-trace is a variance reduction method for the actor-critic algorithm.
-        It is proposed in the paper
-        `IMPALA: Scalable Distributed Deep-RL with Importance Weighted Actor-Learner Architectures
-        <https://arxiv.org/abs/1802.01561>`_.
+            V-trace is a variance reduction method for the actor-critic algorithm. It is proposed in
+            the paper `IMPALA: Scalable Distributed Deep-RL with Importance Weighted Actor-Learner Architectures <https://arxiv.org/abs/1802.01561>`_.
 
-        V-trace calculates the advantage using the following formula:
+            V-trace calculates the advantage using the following formula:
 
-        .. math::
-            A_t = \sum_{k=0}^{n-1} (\lambda \gamma)^k \delta_{t+k} +
-            (\lambda \gamma)^n * \rho_{t+n} * (1 - d_{t+n}) * (V(x_{t+n}) - b_{t+n})
+            .. math::
+
+                A_t = \sum_{k=0}^{n-1} (\lambda \gamma)^k \delta_{t+k} +
+                    (\lambda \gamma)^n \rho_{t+n} (1 - d_{t+n}) (V(x_{t+n}) - b_{t+n})
 
-        where :math:`\delta_{t+k} = r_{t+k} + \gamma*V(s_{t+k+1}) - V(s_{t+k})`,
-        :math:`\rho_{t+k} =\frac{\pi(a_{t+k}|s_{t+k})}{b_{t+k}}`,
-        :math:`b_{t+k}` is the behavior policy,
-        and :math:`d_{t+k}` is the done flag.
+            where :math:`\delta_{t+k} = r_{t+k} + \gamma*V(s_{t+k+1}) - V(s_{t+k})`,
+            :math:`\rho_{t+k} = \frac{\pi(a_{t+k}|s_{t+k})}{b_{t+k}}`, :math:`b_{t+k}` is the
+            behavior policy, and :math:`d_{t+k}` is the done flag.
 
         - Plain
 
-        Plain method is the original actor-critic algorithm.
-        It is unbiased but has high variance.
+            Plain method is the original actor-critic algorithm. It is unbiased but has high
+            variance.
 
         Args:
-            vals (np.array): The value of states.
-            rews (np.array): The reward of states.
-            lam (float, optional): The lambda factor for GAE. Defaults to 0.95.
-        """
+            vals (torch.Tensor): The value of states.
+            rews (torch.Tensor): The reward of states.
+            lam (float): The lambda parameter in GAE formula.
 
+        Returns:
+            adv (torch.Tensor): The estimated advantage.
+            target_value (torch.Tensor): The target value for the value function.
+
+        Raises:
+            NotImplementedError: If the advantage estimator is not supported.
+        """  # pylint: disable=line-too-long
         if self._advantage_estimator == 'gae':
             # GAE formula: A_t = \sum_{k=0}^{n-1} (lam*gamma)^k delta_{t+k}
             deltas = rewards[:-1] + self._gamma * values[1:] - values[:-1]
             adv = discount_cumsum(deltas, self._gamma * lam)
             target_value = adv + values[:-1]
 
         elif self._advantage_estimator == 'gae-rtg':
@@ -370,38 +345,42 @@
         gamma: float = 0.99,
         rho_bar: float = 1.0,
         c_bar: float = 1.0,
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         r"""This function is used to calculate V-trace targets.
 
         .. math::
+
             A_t = \sum_{k=0}^{n-1} (\lambda \gamma)^k \delta_{t+k} +
-            (\lambda \gamma)^n * \rho_{t+n} * (1 - d_{t+n}) * (V(x_{t+n}) - b_{t+n})
+                (\lambda \gamma)^n \rho_{t+n} (1 - d_{t+n}) (V(x_{t+n}) - b_{t+n})
 
-        Calculate V-trace targets for off-policy actor-critic learning recursively.
-        For more details,
-        please refer to the paper: `Espeholt et al. 2018, IMPALA <https://arxiv.org/abs/1802.01561>`_.
+        Calculate V-trace targets for off-policy actor-critic learning recursively. For more
+        details, please refer to the paper: `Espeholt et al. 2018, IMPALA <https://arxiv.org/abs/1802.01561>`_.
 
         Args:
-            policy_action_probs (torch.Tensor): action probabilities of policy network, shape=(sequence_length,)
-            values (torch.Tensor): state values, shape=(sequence_length+1,)
-            rewards (torch.Tensor): rewards, shape=(sequence_length+1,)
-            behavior_action_probs (torch.Tensor): action probabilities of behavior network, shape=(sequence_length,)
-            gamma (float): discount factor
-            rho_bar (float): clip rho
-            c_bar (float): clip c
+            policy_action_probs (torch.Tensor): Action probabilities of the policy.
+            values (torch.Tensor): The value of states.
+            rewards (torch.Tensor): The reward of states.
+            behavior_action_probs (torch.Tensor): Action probabilities of the behavior policy.
+            gamma (float, optional): The discount factor. Defaults to 0.99.
+            rho_bar (float, optional): The maximum value of importance weights. Defaults to 1.0.
+            c_bar (float, optional): The maximum value of clipped importance weights. Defaults to 1.0.
 
         Returns:
-            tuple: V-trace targets, shape=(batch_size, sequence_length)
+            V-trace targets, shape=(batch_size, sequence_length)
+
+        Raises:
+            AssertionError: If the input tensors are scalars.
+            AssertionError: If c_bar is greater than rho_bar.
         """
-        assert values.ndim == 1, 'Please provide 1d-arrays'
-        assert rewards.ndim == 1
-        assert policy_action_probs.ndim == 1
-        assert behavior_action_probs.ndim == 1
-        assert c_bar <= rho_bar
+        assert values.ndim == 1, 'Please provide arrays instead of scalars'
+        assert rewards.ndim == 1, 'Please provide arrays instead of scalars'
+        assert policy_action_probs.ndim == 1, 'Please provide arrays instead of scalars'
+        assert behavior_action_probs.ndim == 1, 'Please provide arrays instead of scalars'
+        assert c_bar <= rho_bar, 'c_bar should be less than or equal to rho_bar'
 
         sequence_length = policy_action_probs.shape[0]
         # pylint: disable-next=assignment-from-no-return
         rhos = torch.div(policy_action_probs, behavior_action_probs)
         clip_rhos = torch.min(
             rhos,
             torch.as_tensor(rho_bar),
```

### Comparing `omnisafe-0.3.0/omnisafe/common/buffer/vector_offpolicy_buffer.py` & `omnisafe-0.4.0/omnisafe/common/buffer/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,132 +8,127 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of VectorOffPolicyBuffer."""
+"""Abstract base class for buffer."""
 
 from __future__ import annotations
 
+from abc import ABC, abstractmethod
+
 import torch
 from gymnasium.spaces import Box
 
-from omnisafe.common.buffer.offpolicy_buffer import OffPolicyBuffer
-from omnisafe.typing import OmnisafeSpace
+from omnisafe.typing import DEVICE_CPU, OmnisafeSpace
+
+
+class BaseBuffer(ABC):
+    r"""Abstract base class for buffer.
 
+    .. warning::
+        The buffer only supports Box spaces.
 
-class VectorOffPolicyBuffer(OffPolicyBuffer):
-    """A VectorReplayBuffer for OffPolicy Algorithms."""
+    In base buffer, we store the following data:
+
+    +--------+---------------------------+---------------+-----------------------------------+
+    | Name   | Shape                     | Dtype         | Description                       |
+    +========+===========================+===============+===================================+
+    | obs    | (size, \*obs_space.shape) | torch.float32 | The observation from environment. |
+    +--------+---------------------------+---------------+-----------------------------------+
+    | act    | (size, \*act_space.shape) | torch.float32 | The action from agent.            |
+    +--------+---------------------------+---------------+-----------------------------------+
+    | reward | (size,)                   | torch.float32 | Single step reward.               |
+    +--------+---------------------------+---------------+-----------------------------------+
+    | cost   | (size,)                   | torch.float32 | Single step cost.                 |
+    +--------+---------------------------+---------------+-----------------------------------+
+    | done   | (size,)                   | torch.float32 | Whether the episode is done.      |
+    +--------+---------------------------+---------------+-----------------------------------+
+
+
+    Args:
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        size (int): The size of the buffer.
+        device (torch.device): The device of the buffer. Defaults to ``torch.device('cpu')``.
+
+    Attributes:
+        data (dict[str, torch.Tensor]): The data of the buffer.
+
+    Raises:
+        NotImplementedError: If the observation space or the action space is not Box.
+        NotImplementedError: If the action space or the action space is not Box.
+    """
 
-    def __init__(  # pylint: disable=super-init-not-called,too-many-arguments
+    def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         size: int,
-        batch_size: int,
-        num_envs: int,
-        device: torch.device = 'cpu',
+        device: torch.device = DEVICE_CPU,
     ) -> None:
-        """Initialize the off policy buffer.
-
-        The vector-off-policy buffer is a vectorized version of the off-policy buffer.
-        It stores the data in a single tensor, and the data of each environment is
-        stored in a separate column.
-
-        .. warning::
-            The buffer only supports Box spaces.
-
-        Args:
-            obs_space (OmnisafeSpace): The observation space.
-            act_space (OmnisafeSpace): The action space.
-            size (int): The size of the buffer.
-            batch_size (int): The batch size of the buffer.
-            num_envs (int): The number of environments.
-            device (torch.device, optional): The device of the buffer. Defaults to
-                torch.device('cpu').
-
-        Attributes:
-            data (Dict[str, torch.Tensor]): The data of the buffer.
-            _ptr (int): The pointer of the buffer.
-            _size (int): The size of the buffer.
-            _max_size (int): The maximum size of the buffer.
-            _batch_size (int): The batch size of the buffer.
-            _num_envs (int): The number of environments.
-
-        """
-        device = torch.device(device)
-        self._num_envs = num_envs
+        """Initialize an instance of :class:`BaseBuffer`."""
+        self._device: torch.device = device
         if isinstance(obs_space, Box):
-            obs_buf = torch.zeros(
-                (size, num_envs, *obs_space.shape),
-                dtype=torch.float32,
-                device=device,
-            )
-            next_obs_buf = torch.zeros(
-                (size, num_envs, *obs_space.shape),
-                dtype=torch.float32,
-                device=device,
-            )
+            obs_buf = torch.zeros((size, *obs_space.shape), dtype=torch.float32, device=device)
         else:
             raise NotImplementedError
-
         if isinstance(act_space, Box):
-            act_buf = torch.zeros(
-                (size, num_envs, *act_space.shape),
-                dtype=torch.float32,
-                device=device,
-            )
+            act_buf = torch.zeros((size, *act_space.shape), dtype=torch.float32, device=device)
         else:
             raise NotImplementedError
 
-        self.data = {
+        self.data: dict[str, torch.Tensor] = {
             'obs': obs_buf,
             'act': act_buf,
-            'reward': torch.zeros((size, num_envs), dtype=torch.float32, device=device),
-            'cost': torch.zeros((size, num_envs), dtype=torch.float32, device=device),
-            'done': torch.zeros((size, num_envs), dtype=torch.float32, device=device),
-            'next_obs': next_obs_buf,
+            'reward': torch.zeros(size, dtype=torch.float32, device=device),
+            'cost': torch.zeros(size, dtype=torch.float32, device=device),
+            'done': torch.zeros(size, dtype=torch.float32, device=device),
         }
+        self._size: int = size
 
-        self._ptr: int = 0
-        self._size: int = 0
-        self._max_size: int = size
-        self._batch_size: int = batch_size
-        self._device = device
+    @property
+    def device(self) -> torch.device:
+        """The device of the buffer."""
+        return self._device
 
     @property
-    def num_envs(self) -> int:
-        """Return the number of environments."""
-        return self._num_envs
+    def size(self) -> int:
+        """The size of the buffer."""
+        return self._size
+
+    def __len__(self) -> int:
+        """Return the length of the buffer."""
+        return self._size
 
-    def add_field(self, name: str, shape: tuple, dtype: torch.dtype):
+    def add_field(self, name: str, shape: tuple[int, ...], dtype: torch.dtype) -> None:
         """Add a field to the buffer.
 
-        Example:
+        Examples:
             >>> buffer = BaseBuffer(...)
             >>> buffer.add_field('new_field', (2, 3), torch.float32)
             >>> buffer.data['new_field'].shape
             >>> (buffer.size, 2, 3)
 
         Args:
             name (str): The name of the field.
-            shape (tuple): The shape of the field.
+            shape (tuple of int): The shape of the field.
             dtype (torch.dtype): The dtype of the field.
         """
-        self.data[name] = torch.zeros(
-            (self._max_size, self._num_envs, *shape),
-            dtype=dtype,
-            device=self._device,
-        )
-
-    def sample_batch(self) -> dict[str, torch.Tensor]:
-        """Sample a batch from the buffer."""
-        idx = torch.randint(
-            0,
-            self._size,
-            (self._batch_size * self._num_envs,),
-            device=self._device,
-        )
-        env_idx = torch.arange(self._num_envs, device=self._device).repeat(self._batch_size)
-        return {key: value[idx, env_idx] for key, value in self.data.items()}
+        self.data[name] = torch.zeros((self._size, *shape), dtype=dtype, device=self._device)
+
+    @abstractmethod
+    def store(self, **data: torch.Tensor) -> None:
+        """Store a transition in the buffer.
+
+        .. warning::
+            This is an abstract method.
+
+        Examples:
+            >>> buffer = BaseBuffer(...)
+            >>> buffer.store(obs=obs, act=act, reward=reward, cost=cost, done=done)
+
+        Args:
+            data (torch.Tensor): The data to store.
+        """
```

### Comparing `omnisafe-0.3.0/omnisafe/common/buffer/vector_onpolicy_buffer.py` & `omnisafe-0.4.0/omnisafe/common/buffer/vector_onpolicy_buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,72 +15,69 @@
 """Implementation of VectorOnPolicyBuffer."""
 
 from __future__ import annotations
 
 import torch
 
 from omnisafe.common.buffer.onpolicy_buffer import OnPolicyBuffer
-from omnisafe.typing import AdvatageEstimator, OmnisafeSpace
+from omnisafe.typing import DEVICE_CPU, AdvatageEstimator, OmnisafeSpace
 from omnisafe.utils import distributed
 
 
 class VectorOnPolicyBuffer(OnPolicyBuffer):
-    """Vectorized on-policy buffer."""
+    """Vectorized on-policy buffer.
+
+    The vector-on-policy buffer is used to store the data from vector environments. The data is
+    stored in a list of on-policy buffers, each of which corresponds to one environment.
+
+    .. warning::
+        The buffer only supports Box spaces.
+
+    Args:
+        obs_space (OmnisafeSpace): Observation space.
+        act_space (OmnisafeSpace): Action space.
+        size (int): Size of the buffer.
+        gamma (float): Discount factor.
+        lam (float): Lambda for GAE.
+        lam_c (float): Lambda for GAE for cost.
+        advantage_estimator (AdvatageEstimator): Advantage estimator.
+        penalty_coefficient (float): Penalty coefficient.
+        standardized_adv_r (bool): Whether to standardize the advantage for reward.
+        standardized_adv_c (bool): Whether to standardize the advantage for cost.
+        num_envs (int, optional): Number of environments. Defaults to 1.
+        device (torch.device, optional): Device to store the data. Defaults to
+            ``torch.device('cpu')``.
+
+    Attributes:
+        buffers (list[OnPolicyBuffer]): List of on-policy buffers.
+    """
 
     def __init__(  # pylint: disable=super-init-not-called,too-many-arguments
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         size: int,
         gamma: float,
         lam: float,
         lam_c: float,
         advantage_estimator: AdvatageEstimator,
         penalty_coefficient: float,
         standardized_adv_r: bool,
         standardized_adv_c: bool,
         num_envs: int = 1,
-        device: torch.device = 'cpu',
+        device: torch.device = DEVICE_CPU,
     ) -> None:
-        """Initialize the vector-on-policy buffer.
-
-        The vector-on-policy buffer is used to store the data from vector environments.
-        The data is stored in a list of on-policy buffers, each of which corresponds to
-        one environment.
-
-        .. warning::
-            The buffer only supports Box spaces.
-
-        Args:
-            obs_space (OmnisafeSpace): Observation space.
-            act_space (OmnisafeSpace): Action space.
-            size (int): Size of the buffer.
-            gamma (float): Discount factor.
-            lam (float): Lambda for GAE.
-            lam_c (float): Lambda for GAE for cost.
-            advantage_estimator (AdvatageEstimator): Advantage estimator.
-            penalty_coefficient (float): Penalty coefficient.
-            standardized_adv_r (bool): Whether to standardize the advantage for reward.
-            standardized_adv_c (bool): Whether to standardize the advantage for cost.
-            num_envs (int, optional): Number of environments. Defaults to 1.
-            device (torch.device, optional): Device to store the data. Defaults to torch.device('cpu').
-
-        Attributes:
-            buffers (List[OnPolicyBuffer]): List of on-policy buffers.
-            _num_buffers (int): Number of buffers.
-            _standardized_adv_r (bool): Whether to standardize the advantage for reward.
-            _standardized_adv_c (bool): Whether to standardize the advantage for cost.
+        """Initialize an instance of :class:`VectorOnPolicyBuffer`."""
+        self._num_buffers: int = num_envs
+        self._standardized_adv_r: bool = standardized_adv_r
+        self._standardized_adv_c: bool = standardized_adv_c
 
-        """
-        self._num_buffers = num_envs
-        self._standardized_adv_r = standardized_adv_r
-        self._standardized_adv_c = standardized_adv_c
         if num_envs < 1:
             raise ValueError('num_envs must be greater than 0.')
-        self.buffers = [
+        self.buffers: list[OnPolicyBuffer] = [
             OnPolicyBuffer(
                 obs_space=obs_space,
                 act_space=act_space,
                 size=size,
                 gamma=gamma,
                 lam=lam,
                 lam_c=lam_c,
@@ -89,24 +86,23 @@
                 device=device,
             )
             for _ in range(num_envs)
         ]
 
     @property
     def num_buffers(self) -> int:
-        """Get the number of buffers."""
+        """Number of buffers."""
         return self._num_buffers
 
     def store(self, **data: torch.Tensor) -> None:
         """Store data into the buffer.
 
         .. hint::
-            The data should be a list of tensors, each of which corresponds to one environment.
-            Then the data will be stored into the corresponding buffer.
-
+            The data should be a list of tensors, each of which corresponds to one environment. Then
+            the data will be stored into the corresponding buffer.
         """
         for i, buffer in enumerate(self.buffers):
             buffer.store(**{k: v[i] for k, v in data.items()})
 
     def finish_path(
         self,
         last_value_r: torch.Tensor | None = None,
@@ -114,26 +110,35 @@
         idx: int = 0,
     ) -> None:
         """Get the data in the buffer.
 
         In vector-on-policy buffer, we get the data from each buffer and then concatenate them.
 
         .. hint::
-
-            We provide a trick to standardize the advantages of state-action pairs.
-            We calculate the mean and standard deviation of the advantages of state-action pairs
-            and then standardize the advantages of state-action pairs.
-            You can turn on this trick by setting the ``standardized_adv_r`` to ``True``.
-            The same trick is applied to the advantages of the cost.
-
+            We provide a trick to standardize the advantages of state-action pairs. We calculate the
+            mean and standard deviation of the advantages of state-action pairs and then standardize
+            the advantages of state-action pairs. You can turn on this trick by setting the
+            ``standardized_adv_r`` to ``True``. The same trick is applied to the advantages of the
+            cost.
         """
         self.buffers[idx].finish_path(last_value_r, last_value_c)
 
     def get(self) -> dict[str, torch.Tensor]:
-        """Get the data from the buffer."""
+        """Get the data in the buffer.
+
+        .. hint::
+            We provide a trick to standardize the advantages of state-action pairs. We calculate the
+            mean and standard deviation of the advantages of state-action pairs and then standardize
+            the advantages of state-action pairs. You can turn on this trick by setting the
+            ``standardized_adv_r`` to ``True``. The same trick is applied to the advantages of the
+            cost.
+
+        Returns:
+            The data stored and calculated in the buffer.
+        """
         data_pre = {k: [v] for k, v in self.buffers[0].get().items()}
         for buffer in self.buffers[1:]:
             for k, v in buffer.get().items():
                 data_pre[k].append(v)
         data = {k: torch.cat(v, dim=0) for k, v in data_pre.items()}
 
         adv_mean, adv_std, *_ = distributed.dist_statistics_scalar(data['adv_r'])
```

### Comparing `omnisafe-0.3.0/omnisafe/common/experiment_grid.py` & `omnisafe-0.4.0/omnisafe/common/experiment_grid.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,20 @@
 """Implementation of the Experiment Grid."""
 
 from __future__ import annotations
 
 import json
 import os
 import string
-import time
 from concurrent.futures import ProcessPoolExecutor as Pool
 from copy import deepcopy
-from textwrap import dedent
-from typing import Any
+from typing import Any, Callable
 
 import numpy as np
 from rich.console import Console
-from tqdm import trange
 
 from omnisafe.algorithms import ALGORITHM2TYPE
 from omnisafe.common.statistics_tools import StatisticsTools
 from omnisafe.evaluator import Evaluator
 from omnisafe.utils.exp_grid_tools import all_bools, valid_str
 from omnisafe.utils.tools import (
     assert_with_exit,
@@ -40,59 +37,69 @@
     recursive_check_config,
     recursive_dict2json,
 )
 
 
 # pylint: disable-next=too-many-instance-attributes
 class ExperimentGrid:
-    """Tool for running many experiments given hyper-parameters ranges."""
+    """Tool for running many experiments given hyper-parameters ranges.
 
-    def __init__(self, exp_name='') -> None:
-        """Initialize the ExperimentGrid.
+    Args:
+        exp_name (str, optional): Name of the experiment grid. Defaults to ''.
 
-        Args:
-            exp_name (str): Name of the experiment grid.
-        """
+    Attributes:
+        keys (list[str]): The keys of the configurations for the experiments.
+        vals (list[Any]): The values of the configurations for the experiments.
+        shs (list[str]): The shorthands of the configurations for the experiments.
+        in_names (list[bool]): Whether the shorthand is included in the name of the experiment.
+        div_line_width (int): The width of the dividing line.
+        name (str): Name of the experiment grid.
+        default_shorthand (bool): Whether GridSearch provides default shorthands.
+        wait_defore_launch (int): Tells the GridSearch how many seconds to pause for before
+            launching experiments.
+        foce_datastamp (bool): Whether to automatically insert a date and time stamp into the names
+            of save directories.
+        log_dir (str): The directory for saving the logs.
+    """
+
+    _statistical_tools: StatisticsTools
+    log_dir: str
+    _evaluator: Evaluator
+
+    def __init__(self, exp_name: str = '') -> None:
+        """Initialize an instance of :class:`ExperimentGrid`."""
         self.keys: list[str] = []
         self.vals: list[Any] = []
         self.shs: list[str] = []
-        self.in_names: list[str] = []
-        self.div_line_width = 80
+        self.in_names: list[bool] = []
+        self.div_line_width: int = 80
         assert isinstance(exp_name, str), 'Name has to be a string.'
-        self.name = exp_name
-        self._console = Console()
-        self.log_dir: str
-
+        self.name: str = exp_name
+        self._console: Console = Console()
         # Whether GridSearch provides automatically-generated default shorthands
-        self.default_shorthand = True
-
+        self.default_shorthand: bool = True
         # Tells the GridSearch how many seconds to pause for before launching experiments
-        self.wait_defore_launch = 0
-
+        self.wait_defore_launch: int = 0
         # Whether to automatically insert a date and time stamp into the names of save directories
-        self.foce_datastamp = False
-
-        self._statistical_tools: StatisticsTools
-        self._evaluator: Evaluator
+        self.foce_datastamp: bool = False
 
     def print(self) -> None:
         """Print a helpful report about the experiment grid.
 
-        This function prints a helpful report about the experiment grid, including
-        the name of the experiment grid, the parameters being varied, and the
-        possible values for each parameter.
+        This function prints a helpful report about the experiment grid, including the name of the
+        experiment grid, the parameters being varied, and the possible values for each parameter.
 
         In Command Line:
 
-        .. code-block:: bash
+        .. code-block:: text
 
             ===================== ExperimentGrid [test] runs over parameters: =====================
             env_name                                [env]
             ['SafetyPointGoal1-v0', 'MountainCar-v0', 'Acrobot-v1']
-            algo                               [algo]
+            algo                                    [algo]
             ['SAC', 'DDPG', 'TD3']
             seed                                    [seed]
             [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
         """
         print('=' * self.div_line_width)
 
         # Prepare announcement at top of printing. If the ExperimentGrid has a
@@ -125,99 +132,114 @@
         else:
             nvars_seedless = nvars_total
         print(' Variants, counting seeds: '.ljust(40), nvars_total)
         print(' Variants, not counting seeds: '.ljust(40), nvars_seedless)
         print()
         print('=' * self.div_line_width)
 
-    def _default_shorthand(self, key):
-        r"""Default shorthand.
+    def _default_shorthand(self, key: str) -> str:
+        """Get the default shorthand.
+
         Create a default shorthand for the key, built from the first
         three letters of each colon-separated part.
         But if the first three letters contains something which isn't
         alphanumeric, shear that off.
 
-        Example:
+        Examples:
             >>> _default_shorthand('env_name:SafetyPointGoal1-v0')
             'env'
 
         Args:
-            key (string): Name of parameter.
-        """
+            key (str): Name of parameter.
 
+        Returns:
+            Shorthand of parameter.
+        """
         valid_chars = f'{string.ascii_letters}{string.digits}'
 
-        def shear(value):
+        def shear(value: str) -> str:
             return ''.join(z for z in value[:3] if z in valid_chars)
 
         return '-'.join([shear(x) for x in key.split(':')])
 
-    def add(self, key, vals, shorthand=None, in_name=False):
-        r"""Add a parameter (key) to the grid config, with potential values (vals).
+    def add(
+        self,
+        key: str,
+        vals: list[Any] | Any,
+        shorthand: str | None = None,
+        in_name: bool = False,
+    ) -> None:
+        """Add a parameter (key) to the grid config, with potential values (vals).
 
-        By default, if a shorthand isn't given, one is automatically generated
-        from the key using the first three letters of each colon-separated
-        term.
+        By default, if a shorthand isn't given, one is automatically generated from the key using
+        the first three letters of each colon-separated term.
 
         .. hint::
-
             This function is called in ``omnisafe/examples/benchmarks/run_experiment_grid.py``.
 
-        Example:
+        Examples:
             >>> add('env_id', ['SafetyPointGoal1-v0', 'MountainCar-v0', 'Acrobot-v1'])
             >>> add('algo', ['SAC', 'DDPG', 'TD3'])
             >>> add('seed', [0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
 
         Args:
-            key (string): Name of parameter.
-
-            vals (value or list of values): Allowed values of parameter.
-
-            shorthand (string): Optional, shortened name of parameter. For
-                example, maybe the parameter ``steps_per_epoch`` is shortened
-                to ``steps``.
-
-            in_name (bool): When constructing variant names, force the
-                inclusion of this parameter into the name.
+            key (str): Name of parameter.
+            vals (list or object): Possible values for parameter.
+            shorthand (str, optional): Shorthand for parameter.
+            in_name (bool, optional): Whether to include this parameter in the experiment name.
         """
         assert isinstance(key, str), 'Key must be a string.'
-        assert shorthand is None or isinstance(shorthand, str), 'Shorthand must be a string.'
         if not isinstance(vals, list):
             vals = [vals]
         if self.default_shorthand and shorthand is None:
             shorthand = self._default_shorthand(key)
         self.keys.append(key)
         self.vals.append(vals)
-        self.shs.append(shorthand)
+        assert len(set(self.keys)) == len(self.keys), f'Duplicate key: `{key}`'
+        assert len(set(vals)) == len(vals), f'Duplicate values in {vals} for key: `{key}`'
+        if shorthand is not None:
+            self.shs.append(shorthand)
         self.in_names.append(in_name)
 
-    def variant_name(self, variant):
-        r"""Given a variant (dict of valid param/value pairs), make an exp_name.
+    def variant_name(self, variant: dict[str, Any]) -> str:
+        """Given a variant (dict of valid param/value pairs), make an exp_name.
 
-        A variant's name is constructed as the grid name (if you've given it
-        one), plus param names (or shorthands if available) and values
-        separated by underscores.
+        A variant's name is constructed as the grid name (if you've given it one), plus param names
+        (or shorthands if available) and values separated by underscores.
 
         ..warning::
             if ``seed`` is a parameter, it is not included in the name.
 
-        Example:
+        Examples:
             >>> variant_name({'env_id': 'SafetyPointGoal1-v0', 'algo': 'SAC', 'seed': 0})
-            exp_name = 'SafetyPointGoal1-v0_SAC_0'
+            'SafetyPointGoal1-v0_SAC_0'
 
         Args:
-            variant (dict): Variant dictionary.
+            variant (dict[str, Any]): Variant dictionary.
+
+        Returns:
+            Experiment name.
         """
 
-        def get_val(value, key):
-            # utility method for getting the correct value out of a variant
-            # given as a nested dict. Assumes that a parameter name, k,
-            # describes a path into the nested dict, such that k='a:b:c'
-            # corresponds to value=variant['a']['b']['c']. Uses recursion
-            # to get this
+        def get_val(value: dict[str, Any], key: str) -> Any:
+            """Get value from variant.
+
+            Utility method for getting the correct value out of a variant
+            given as a nested dict. Assumes that a parameter name, k,
+            describes a path into the nested dict, such that k='a:b:c'
+            corresponds to value=variant['a']['b']['c']. Uses recursion
+            to get this.
+
+            Args:
+                value (dict[str, Any]): Variant dictionary.
+                key (str): Key of variant dictionary.
+
+            Returns:
+                Value of variant dictionary.
+            """
             print('value', value, 'key', key)
             if key in value:
                 return value[key]
 
             splits = key.split(':')
             k_0, k_1 = splits[0], ':'.join(splits[1:])
             return get_val(value[k_0], k_1)
@@ -246,46 +268,48 @@
                     # only include in the name if it's True for this variant.
                     var_name += ('_' + param_name) if variant_val else ''
                 else:
                     var_name += '_' + param_name + valid_str(variant_val)
 
         return var_name.lstrip('_')
 
-    def update_dict(self, total_dict, item_dict):
+    def update_dict(self, total_dict: dict[str, Any], item_dict: dict[str, Any]) -> None:
         """Updater of multi-level dictionary.
 
-        This function is used to update the total dictionary with the item
-        dictionary.
+        This function is used to update the total dictionary with the item dictionary.
 
         Args:
-            total_dict (dict): Total dictionary.
-            item_dict (dict): Item dictionary.
+            total_dict (dict[str, Any]): Total dictionary.
+            item_dict (dict[str, Any]): Item dictionary.
         """
         for idd in item_dict:
             total_value = total_dict.get(idd)
             item_value = item_dict.get(idd)
 
             if total_value is None:
                 total_dict.update({idd: item_value})
             elif isinstance(item_value, dict):
                 self.update_dict(total_value, item_value)
                 total_dict.update({idd: total_value})
             else:
                 total_value = item_value
                 total_dict.update({idd: total_value})
 
-    def _variants(self, keys, vals):
+    def _variants(self, keys: list[str], vals: list[Any]) -> list[dict[str, Any]]:
         """Recursively builds list of valid variants.
 
         Args:
-            keys (list): List of keys.
-            vals (list): List of values.
+            keys (keys: list[str]): List of keys.
+            vals (list[Any]): List of values.
+
+        Returns:
+            List of valid variants.
         """
         if len(keys) == 1:
-            pre_variants: list[dict] = [{}]
+            pre_variants: list[dict[str, Any]] = [{}]
         else:
             pre_variants = self._variants(keys[1:], vals[1:])
 
         variants = []
         for val in vals[0]:
             for pre_v in pre_variants:
                 current_variants = deepcopy(pre_v)
@@ -295,34 +319,32 @@
                 for key in reversed(key_list[:-1]):
                     v_temp = {key: v_temp}
                 self.update_dict(current_variants, v_temp)
                 variants.append(current_variants)
 
         return variants
 
-    def variants(self):
-        r"""Makes a list of dict, where each dict is a valid config in the grid.
-
-        There is special handling for variant parameters whose names take
-        the form ``'full:param:name'``.
+    def variants(self) -> list[dict[str, Any]]:
+        """Makes a list of dict, where each dict is a valid config in the grid.
 
-        The colons are taken to indicate that these parameters should
-        have a nested dict structure. eg, if there are two params,
+        There is special handling for variant parameters whose names take the form
+        ``'full:param:name'``.
 
-        .. hint::
+        The colons are taken to indicate that these parameters should have a nested dict structure.
+        For example, if there are two params,
 
-            ====================  ===
-            Key                   Val
-            ====================  ===
-            ``'base:param:a'``    1
-            ``'base:param:b'``    2
-            ``'base:param:c'``    3
-            ``'special:d'``       4
-            ``'special:e'``       5
-            ====================  ===
+        ====================  ===
+        Key                   Val
+        ====================  ===
+        ``'base:param:a'``    1
+        ``'base:param:b'``    2
+        ``'base:param:c'``    3
+        ``'special:d'``       4
+        ``'special:e'``       5
+        ====================  ===
 
         the variant dict will have the structure
 
         .. parsed-literal::
 
             {
                 'base': {
@@ -333,63 +355,65 @@
                     }
                 },
                 'special': {
                     'd': 4,
                     'e': 5
                 }
             }
+
+        Returns:
+            List of valid and not duplicate variants.
         """
         flat_variants = self._variants(self.keys, self.vals)
 
-        def unflatten_var(var):
+        def check_duplicate(var: dict[str, Any]) -> dict[str, Any]:
             """Build the full nested dict version of var, based on key names."""
-            new_var: dict = {}
-            unflatten_set = set()
+            new_var: dict[str, Any] = {}
+            unflatten_set: set = set()
 
             for key, value in var.items():
-                if ':' in key:
-                    splits = key.split(':')
-                    k_0 = splits[0]
-                    assert k_0 not in new_var or isinstance(
-                        new_var[k_0],
-                        dict,
-                    ), "You can't assign multiple values to the same key."
-
-                    if k_0 not in new_var:
-                        new_var[k_0] = {}
-
-                    sub_k = ':'.join(splits[1:])
-                    new_var[k_0][sub_k] = value
-                    unflatten_set.add(k_0)
-                else:
-                    assert key not in new_var, "You can't assign multiple values to the same key."
-                    new_var[key] = value
+                assert key not in new_var, "You can't assign multiple values to the same key."
+                new_var[key] = value
 
             # make sure to fill out the nested dict.
             for key in unflatten_set:
-                new_var[key] = unflatten_var(new_var[key])
+                new_var[key] = check_duplicate(new_var[key])
 
             return new_var
 
-        return [unflatten_var(var) for var in flat_variants]
+        return [check_duplicate(var) for var in flat_variants]
 
     # pylint: disable-next=too-many-locals
-    def run(self, thunk, num_pool=1, parent_dir=None, is_test=False, gpu_id=None):
-        r"""Run each variant in the grid with function 'thunk'.
+    def run(
+        self,
+        thunk: Callable[[str, str, str, dict[str, Any]], tuple[float, float, int]],
+        num_pool: int = 1,
+        parent_dir: str | None = None,
+        is_test: bool = False,
+        gpu_id: list[int] | None = None,
+    ) -> None:
+        """Run each variant in the grid with function 'thunk'.
+
+        Note: 'thunk' must be either a callable function, or a string. If it is a string, it must be
+        the name of a parameter whose values are all callable functions.
+
+        Uses ``call_experiment`` to actually launch each experiment, and gives each variant a name
+        using ``self.variant_name()``.
+
+        Maintenance note: the args for ExperimentGrid.run should track closely to the args for
+        ``call_experiment``. However, ``seed`` is omitted because we presume the user may add it as
+        a parameter in the grid.
 
-        Note: 'thunk' must be either a callable function, or a string. If it is
-        a string, it must be the name of a parameter whose values are all
-        callable functions.
-
-        Uses ``call_experiment`` to actually launch each experiment, and gives
-        each variant a name using ``self.variant_name()``.
-
-        Maintenance note: the args for ExperimentGrid.run should track closely
-        to the args for call_experiment. However, ``seed`` is omitted because
-        we presume the user may add it as a parameter in the grid.
+        Args:
+            thunk (Callable): Function to be called.
+            num_pool (int, optional): Number of processes to run in parallel. Defaults to 1.
+            parent_dir (str or None, optional): Parent directory to save the experiment results.
+                Defaults to None.
+            is_test (bool, optional): Whether to run the experiment in test mode. Defaults to False.
+            gpu_id (list of int or None, optional): List of GPU IDs to use. Defaults to None.
         """
         if parent_dir is None:
             self.log_dir = os.path.join('./', 'exp-x', self.name)
         else:
             self.log_dir = os.path.join(parent_dir, self.name)
         assert_with_exit(
             not os.path.exists(self.log_dir),
@@ -412,41 +436,14 @@
         line = '=' * self.div_line_width
 
         self._console.print('\nPreparing to run the following experiments...', style='bold green')
         joined_var_names = '\n'.join(var_names)
         announcement = f'\n{joined_var_names}\n\n{line}'
         print(announcement)
 
-        if self.wait_defore_launch > 0:
-            self._console.print(
-                dedent(
-                    """
-                    Launch delayed to give you a few seconds to review your experiments.
-
-                    To customize or disable this behavior, change WAIT_BEFORE_LAUNCH in
-                    spinup/user_config.py.
-
-                    """,
-                ),
-                style='cyan, bold',
-                end='',
-            )
-            print(line)
-            wait, steps = self.wait_defore_launch, 100
-            prog_bar = trange(
-                steps,
-                desc='Launching in...',
-                leave=False,
-                ncols=self.div_line_width,
-                mininterval=0.25,
-                bar_format='{desc}: {bar}| {remaining} {elapsed}',
-            )
-            for _ in prog_bar:
-                time.sleep(wait / steps)
-
         pool = Pool(max_workers=num_pool)
         # run the variants.
         results = []
         exp_names = []
 
         for idx, var in enumerate(variants):
             self.check_variant_vaild(var)
@@ -459,147 +456,184 @@
                 self.update_dict(var, {'train_cfgs': {'device': device}})
             exp_name = recursive_dict2json(clean_var)
             hashed_exp_name = var['env_id'][:30] + '---' + hash_string(exp_name)
             exp_names.append(':'.join((hashed_exp_name[:5], exp_name)))
             exp_log_dir = os.path.join(self.log_dir, hashed_exp_name, '')
             var['logger_cfgs'].update({'log_dir': exp_log_dir})
             self.save_same_exps_config(exp_log_dir, var)
-            results.append(pool.submit(thunk, idx, var['algo'], var['env_id'], var))
+            results.append(pool.submit(thunk, str(idx), var['algo'], var['env_id'], var))
         pool.shutdown()
 
         if not is_test:
             self.save_results(exp_names, variants, results)
         self._init_statistical_tools()
 
-    def save_results(self, exp_names, variants, results):
-        """Save results to a file."""
+    def save_results(
+        self,
+        exp_names: list[str],
+        variants: list[dict[str, Any]],
+        results: list,
+    ) -> None:
+        """Save results to a file.
+
+        Args:
+            exp_names (list of str): List of experiment names.
+            variants (list[dict[str, Any]]): List of experiment variants.
+            results (list): List of experiment results.
+        """
         path = os.path.join(self.log_dir, 'exp-x-results.txt')
         str_len = max(len(exp_name) for exp_name in exp_names)
         exp_names = [exp_name.ljust(str_len) for exp_name in exp_names]
         with open(path, 'a+', encoding='utf-8') as f:
             for idx, _ in enumerate(variants):
                 f.write(exp_names[idx] + ': ')
                 reward, cost, ep_len = results[idx].result()
                 f.write('reward:' + str(round(reward, 2)) + ',')
                 f.write('cost:' + str(round(cost, 2)) + ',')
                 f.write('ep_len:' + str(ep_len))
                 f.write('\n')
 
-    def save_same_exps_config(self, exps_log_dir, variant):
-        """Save experiment grid configurations as json."""
+    def save_same_exps_config(self, exps_log_dir: str, variant: dict[str, Any]) -> None:
+        """Save experiment grid configurations as json.
+
+        Args:
+            exps_log_dir (str): Experiment log directory.
+            variant (dict[str, Any]): Experiment variant.
+        """
         os.makedirs(exps_log_dir, exist_ok=True)
         path = os.path.join(exps_log_dir, 'exps_config.json')
         json_config = json.dumps(variant, indent=4)
         with open(path, encoding='utf-8', mode='a+') as f:
             f.write('\n' + json_config)
 
-    def save_grid_config(self):
+    def save_grid_config(self) -> None:
         """Save experiment grid configurations as json."""
         os.makedirs(self.log_dir, exist_ok=True)
         path = os.path.join(self.log_dir, 'grid_config.json')
         self._console.print(
             'Save with config of experiment grid in grid_config.json',
             style='yellow bold',
         )
         json_config = json.dumps(dict(zip(self.keys, self.vals)), indent=4)
         with open(path, encoding='utf-8', mode='w') as f:
             f.write(json_config)
 
-    def check_variant_vaild(self, variant):
-        """Check if the variant is valid."""
+    def check_variant_vaild(self, variant: dict[str, Any]) -> None:
+        """Check if the variant is valid.
+
+        Args:
+            variant (dict[str, Any]): Experiment variant to be checked.
+        """
         path = os.path.dirname(os.path.abspath(__file__))
         algo_type = ALGORITHM2TYPE.get(variant['algo'], '')
         cfg_path = os.path.join(path, '..', 'configs', algo_type, f"{variant['algo']}.yaml")
         default_config = load_yaml(cfg_path)['defaults']
         recursive_check_config(variant, default_config, exclude_keys=('algo', 'env_id'))
 
-    def _init_statistical_tools(self):
+    def _init_statistical_tools(self) -> None:
         """Initialize statistical tools."""
         self._statistical_tools = StatisticsTools()
         self._evaluator = Evaluator()
 
     def analyze(
         self,
         parameter: str,
-        values: list = None,
-        compare_num: int = None,
-        cost_limit: float = None,
-    ):
+        values: list[Any] | None = None,
+        compare_num: int | None = None,
+        cost_limit: float | None = None,
+        show_image: bool = False,
+    ) -> None:
         """Analyze the experiment results.
 
-        Args:
-            parameter (str): name of parameter to analyze.
-            values (list): specific values of attribute,
-                if it is specified, will only compare values in it.
-            compare_num (int): number of values to compare,
-                if it is specified, will combine any potential combination to compare.
-            cost_limit (float): value for one line showed on graph to indicate cost.
-
-        .. Note::
+        .. note::
             `values` and `compare_num` cannot be set at the same time.
+
+        Args:
+            parameter (str): Name of parameter to analyze.
+            values (list[Any] or None, optional): Specific values of attribute, if it is specified,
+                will only compare values in it. Defaults to None.
+            compare_num (int or None, optional): Number of values to compare, if it is specified,
+                will combine any potential combination to compare. Defaults to None.
+            cost_limit (float or None, optional): Value for one line showed on graph to indicate
+                cost. Defaults to None.
+            show_image (bool): Whether to show graph image in GUI windows.
         """
         assert self._statistical_tools is not None, 'Please run run() first!'
         self._statistical_tools.load_source(self.log_dir)
-        self._statistical_tools.draw_graph(parameter, values, compare_num, cost_limit)
+        self._statistical_tools.draw_graph(
+            parameter,
+            values,
+            compare_num,
+            cost_limit,
+            show_image=show_image,
+        )
 
-    def evaluate(self, num_episodes: int = 10, cost_criteria: float = 1.0):
+    def evaluate(self, num_episodes: int = 10, cost_criteria: float = 1.0) -> None:
         """Agent Evaluation.
 
         Args:
-            num_episodes (int): number of episodes to evaluate.
-            cost_criteria (float): cost criteria for evaluation.
+            num_episodes (int, optional): Number of episodes to evaluate. Defaults to 10.
+            cost_criteria (float, optional): Cost criteria for evaluation. Defaults to 1.0.
         """
         assert self._evaluator is not None, 'Please run run() first!'
+        param_dir = os.scandir(self.log_dir)
         # pylint: disable-next=too-many-nested-blocks
-        for set_of_params in os.scandir(self.log_dir):
+        for set_of_params in param_dir:
             if set_of_params.is_dir():
-                for single_exp in os.scandir(set_of_params):
+                exp_dir = os.scandir(set_of_params)
+                for single_exp in exp_dir:
                     if single_exp.is_dir():
-                        for single_seed in os.scandir(single_exp):
-                            for model in os.scandir(os.path.join(single_seed, 'torch_save')):
+                        seed_dir = os.scandir(single_exp)
+                        for single_seed in seed_dir:
+                            model_dir = os.scandir(os.path.join(single_seed, 'torch_save'))
+                            for model in model_dir:
                                 if model.is_file() and model.name.split('.')[-1] == 'pt':
                                     self._evaluator.load_saved(
-                                        save_dir=single_seed,
+                                        save_dir=single_seed.path,
                                         model_name=model.name,
                                     )
                                     self._evaluator.evaluate(
                                         num_episodes=num_episodes,
                                         cost_criteria=cost_criteria,
                                     )
+                            model_dir.close()
+                        seed_dir.close()
+                exp_dir.close()
+        param_dir.close()
 
-    # pylint: disable-next=too-many-arguments
     def render(
         self,
         num_episodes: int = 10,
         render_mode: str = 'rgb_array',
         camera_name: str = 'track',
         width: int = 256,
         height: int = 256,
-    ):
+    ) -> None:  # pragma: no cover
         """Evaluate and render some episodes.
 
         Args:
-            num_episodes (int): number of episodes to render.
-            render_mode (str): render mode, can be 'rgb_array', 'depth_array' or 'human'.
-            camera_name (str): camera name, specify the camera which you use to capture
-                images.
-            width (int): width of the rendered image.
-            height (int): height of the rendered image.
+            num_episodes (int, optional): Number of episodes to render. Defaults to 10.
+            render_mode (str, optional): Render mode, can be 'rgb_array', 'depth_array' or 'human'.
+                Defaults to 'rgb_array'.
+            camera_name (str, optional): Camera name, specify the camera which you use to capture
+                images. Defaults to 'track'.
+            width (int, optional): The width of the rendered image. Defaults to 256.
+            height (int, optional): The height of the rendered image. Defaults to 256.
         """
         assert self._evaluator is not None, 'Please run run() first!'
         # pylint: disable-next=too-many-nested-blocks
         for set_of_params in os.scandir(self.log_dir):
             if set_of_params.is_dir():
                 for single_exp in os.scandir(set_of_params):
                     if single_exp.is_dir():
                         for single_seed in os.scandir(single_exp):
                             for model in os.scandir(os.path.join(single_seed, 'torch_save')):
                                 if model.is_file() and model.name.split('.')[-1] == 'pt':
                                     self._evaluator.load_saved(
-                                        save_dir=single_seed,
+                                        save_dir=single_seed.path,
                                         model_name=model.name,
                                         render_mode=render_mode,
                                         camera_name=camera_name,
                                         width=width,
                                         height=height,
                                     )
                                     self._evaluator.render(num_episodes=num_episodes)
```

### Comparing `omnisafe-0.3.0/omnisafe/common/logger.py` & `omnisafe-0.4.0/omnisafe/common/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import os
 import time
 from collections import deque
 from typing import Any, Deque, TextIO
 
 import numpy as np
 import torch
-import tqdm
 import wandb
 from rich import print  # pylint: disable=redefined-builtin
 from rich.console import Console
 from rich.table import Table
 
 from omnisafe.utils.config import Config
 from omnisafe.utils.distributed import dist_statistics_scalar, get_rank
@@ -39,137 +38,125 @@
 # bug is that it attempts to import distutils then access distutils.version without actually
 # importing distutils.version.  We can workaround this by prepopulating the distutils.version
 # submodule in the distutils module.
 
 try:  # noqa: SIM105
     # pylint: disable-next=wrong-import-order,unused-import,deprecated-module
     import distutils.version  # isort:skip  # noqa: F401
-except ImportError:
+except ImportError:  # pragma: no cover
     pass
 
 # pylint: disable-next=wrong-import-order
-from torch.utils.tensorboard import SummaryWriter  # isort:skip
+from torch.utils.tensorboard.writer import SummaryWriter  # isort:skip
 
 
 class Logger:  # pylint: disable=too-many-instance-attributes
     """Implementation of the Logger.
 
-    A logger to record the training process.
-    It can record the training process to a file and print it to the console.
-    It can also record the training process to tensorboard.
+    A logger to record the training process. It can record the training process to a file and print
+    it to the console. It can also record the training process to tensorboard.
 
     The logger can record the following data:
 
-    .. code-block:: bash
+    .. code-block:: text
 
         ----------------------------------------------
         |       Name      |            Value         |
         ----------------------------------------------
         |    Train/Epoch  |             25           |
         |  Metrics/EpCost |            24.56         |
         |  Metrics/EpLen  |            1000          |
         |  Metrics/EpRet  |            13.24         |
         |  Metrics/EpStd  |            0.12          |
         ----------------------------------------------
+
+    Args:
+        output_dir (str): The output directory.
+        exp_name (str): The experiment name.
+        output_fname (str, optional): The output file name. Defaults to 'progress.csv'.
+        seed (int, optional): The random seed. Defaults to 0.
+        use_tensorboard (bool, optional): Whether to use tensorboard. Defaults to True.
+        use_wandb (bool, optional): Whether to use wandb. Defaults to False.
+        config (Config or None, optional): The config. Defaults to None.
+        models (list[torch.nn.Module] or None, optional): The models. Defaults to None.
     """
 
     def __init__(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         output_dir: str,
         exp_name: str,
         output_fname: str = 'progress.csv',
-        verbose: bool = True,
         seed: int = 0,
         use_tensorboard: bool = True,
         use_wandb: bool = False,
         config: Config | None = None,
         models: list[torch.nn.Module] | None = None,
     ) -> None:
-        """Initialize the logger.
-
-        Args:
-            output_dir: The directory to save the log file.
-            exp_name: The name of the experiment.
-            output_fname: The name of the log file.
-            verbose: Whether to print the log to the console.
-            seed: The random seed.
-            use_tensorboard: Whether to use tensorboard.
-            use_wandb: Whether to use wandb.
-            config: The config of the experiment.
-            models: The models to be saved.
-        """
+        """Initialize an instance of :class:`Logger`."""
         hms_time = time.strftime('%Y-%m-%d-%H-%M-%S', time.localtime())
         relpath = hms_time
 
         if seed is not None:
             relpath = f'seed-{str(seed).zfill(3)}-{relpath}'
 
-        self._hms_time = hms_time
-        self._log_dir = os.path.join(output_dir, exp_name, relpath)
-        self._verbose = verbose
-        self._maste_proc = get_rank() == 0
-        self._console = Console()
+        self._hms_time: str = hms_time
+        self._log_dir: str = os.path.join(output_dir, exp_name, relpath)
+        self._maste_proc: bool = get_rank() == 0
+        self._console: Console = Console()
 
-        self._output_file: TextIO
         if self._maste_proc:
             os.makedirs(self._log_dir, exist_ok=True)
-            self._output_file = open(  # noqa: SIM115 # pylint: disable=consider-using-with
+            self._output_file: TextIO = open(  # noqa: SIM115 # pylint: disable=consider-using-with
                 os.path.join(self._log_dir, output_fname),
                 encoding='utf-8',
                 mode='w',
             )
             atexit.register(self._output_file.close)
             self.log(f'Logging data to {self._output_file.name}', 'cyan', bold=True)
             self._csv_writer = csv.writer(self._output_file)
 
         self._epoch: int = 0
         self._first_row: bool = True
         self._what_to_save: dict[str, Any] | None = None
         self._data: dict[str, Deque[int | float] | list[int | float]] = {}
-        self._headers_windwos: dict[str, int | None] = {}
+        self._headers_windows: dict[str, int | None] = {}
         self._headers_minmax: dict[str, bool] = {}
         self._headers_delta: dict[str, bool] = {}
         self._current_row: dict[str, int | float] = {}
 
         if config is not None:
             self.save_config(config)
-            self._config = config
+            self._config: Config = config
 
-        self._use_tensorboard = use_tensorboard
-        self._use_wandb = use_wandb
+        self._use_tensorboard: bool = use_tensorboard
+        self._use_wandb: bool = use_wandb
 
         if self._use_tensorboard and self._maste_proc:
             self._tensorboard_writer = SummaryWriter(log_dir=os.path.join(self._log_dir, 'tb'))
 
-        if self._use_wandb and self._maste_proc:
+        if self._use_wandb and self._maste_proc:  # pragma: no cover
             project: str = self._config.logger_cfgs.get('wandb_project', 'omnisafe')
             name: str = f'{exp_name}-{relpath}'
             print('project', project, 'name', name)
             wandb.init(project=project, name=name, dir=self._log_dir, config=config)
             if config is not None:
                 wandb.config.update(config)
             if models is not None:
                 for model in models:
                     wandb.watch(model)
 
-        if not self._verbose:
-            assert (
-                'epochs' in self._config
-            ), 'epochs must be specified in the config file when verbose is False'
-            self._proc_bar = tqdm.tqdm(total=self._config['epochs'], desc='Epochs')
-
     def log(self, msg: str, color: str = 'green', bold: bool = False) -> None:
         """Log the message to the console and the file.
 
         Args:
             msg (str): The message to be logged.
-            color (int): The color of the message.
-            bold (bool): Whether to use bold font.
+            color (str, optional): The color of the message. Defaults to 'green'.
+            bold (bool, optional): Whether the message is bold. Defaults to False.
         """
-        if self._verbose and self._maste_proc:
+        if self._maste_proc:
             style = ' '.join([color, 'bold' if bold else ''])
             self._console.print(msg, style=style)
 
     def save_config(self, config: Config) -> None:
         """Save the configuration to the log directory.
 
         Args:
@@ -180,15 +167,15 @@
             with open(os.path.join(self._log_dir, 'config.json'), encoding='utf-8', mode='w') as f:
                 f.write(config.tojson())
 
     def setup_torch_saver(self, what_to_save: dict[str, Any]) -> None:
         """Setup the torch saver.
 
         Args:
-            what_to_save (dict): The dict of the things to be saved.
+            what_to_save (dict[str, Any]): The dict of the things to be saved.
         """
         self._what_to_save = what_to_save
 
     def torch_save(self) -> None:
         """Save the torch model."""
         if self._maste_proc:
             assert self._what_to_save is not None, 'Please setup torch saver first'
@@ -208,63 +195,78 @@
         min_and_max: bool = False,
         delta: bool = False,
     ) -> None:
         """Register a key to the logger.
 
         The logger can record the following data:
 
-        .. code-block:: bash
+        .. code-block:: text
 
             ----------------------------------------------------
             |       Name            |            Value         |
             ----------------------------------------------------
             |    Train/Epoch        |             25           |
             |  Metrics/EpCost/Min   |            22.38         |
             |  Metrics/EpCost/Max   |            25.48         |
             |  Metrics/EpCost/Mean  |            23.93         |
             ----------------------------------------------------
 
         Args:
-            key (str): The key to be registered.
-            window_length (int): The window length for the key, \
-                if window_length is None, the key will be averaged in epoch.
-            min_and_max (bool): Whether to record the min and max value of the key.
-            delta (bool): Whether to record the delta value of the key.
+            key (str): The name of the key.
+            window_length (int or None, optional): The length of the window. Defaults to None.
+            min_and_max (bool, optional): Whether to record the min and max value. Defaults to False.
+            delta (bool, optional): Whether to record the delta value. Defaults to False.
         """
-        assert (key and f'{key}/Mean') not in self._current_row, f'Key {key} has been registered'
+        assert key not in self._current_row, f'Key {key} has been registered'
+        self._current_row[key] = 0
         if min_and_max:
-            self._current_row[f'{key}/Mean'] = 0
             self._current_row[f'{key}/Min'] = 0
             self._current_row[f'{key}/Max'] = 0
             self._current_row[f'{key}/Std'] = 0
             self._headers_minmax[key] = True
+            self._headers_minmax[f'{key}/Min'] = False
+            self._headers_minmax[f'{key}/Max'] = False
+            self._headers_minmax[f'{key}/Std'] = False
 
         else:
-            self._current_row[key] = 0
             self._headers_minmax[key] = False
 
         if delta:
             self._current_row[f'{key}/Delta'] = 0
             self._headers_delta[key] = True
+            self._headers_delta[f'{key}/Delta'] = False
+            self._headers_minmax[f'{key}/Delta'] = False
         else:
             self._headers_delta[key] = False
 
         if window_length is not None:
             self._data[key] = deque(maxlen=window_length)
-            self._headers_windwos[key] = window_length
+            self._headers_windows[key] = window_length
         else:
             self._data[key] = []
-            self._headers_windwos[key] = None
+            self._headers_windows[key] = None
 
-    def store(self, **kwargs: int | float | np.ndarray | torch.Tensor) -> None:
+    def store(
+        self,
+        data: dict[str, int | float | np.ndarray | torch.Tensor] | None = None,
+        /,
+        **kwargs: int | float | np.ndarray | torch.Tensor,
+    ) -> None:
         """Store the data to the logger.
 
+        .. note ::
+            The data stored in ``data`` will be updated by ``kwargs``.
+
         Args:
-            **kwargs: The data to be stored.
+            data (dict[str, int | float | np.ndarray | torch.Tensor] or None, optional): The data to
+                be stored. Defaults to None.
+            **kwargs (int, float, np.ndarray, or torch.Tensor): The data to be stored.
         """
+        if data is not None:
+            kwargs.update(data)
         for key, val in kwargs.items():
             assert key in self._current_row, f'Key {key} has not been registered'
             if isinstance(val, (int, float)):
                 self._data[key].append(val)
             elif isinstance(val, torch.Tensor):
                 self._data[key].append(val.mean().item())
             elif isinstance(val, np.ndarray):
@@ -274,34 +276,31 @@
 
     def dump_tabular(self) -> None:
         """Dump the tabular data to the console and the file.
 
         The dumped data will be separated by the following steps:
 
         .. hint::
-
             - If the key is registered with window_length, the data will be averaged in the window.
             - Write the data to the csv file.
             - Write the data to the tensorboard.
             - Update the progress logger.
-
         """
         self._update_current_row()
         table = Table('Metrics', 'Value')
         if self._maste_proc:
             self._epoch += 1
-            if self._verbose:
-                key_lens = list(map(len, self._current_row.keys()))
-                max_key_len = max(15, *key_lens)
-                for key, val in self._current_row.items():
+            key_lens = list(map(len, self._current_row.keys()))
+            max_key_len = max(15, *key_lens)
+            for key, val in self._current_row.items():
+                if self._headers_minmax[key]:
+                    table.add_row(f'{key}/Mean'[:max_key_len], str(val)[:max_key_len])
+                else:
                     table.add_row(key[:max_key_len], str(val)[:max_key_len])
 
-            else:
-                self._proc_bar.update(1)
-
             if self._first_row:
                 self._csv_writer.writerow(self._current_row.keys())
                 self._first_row = False
             self._csv_writer.writerow(self._current_row.values())
             self._output_file.flush()
 
             if self._use_tensorboard:
@@ -315,50 +314,57 @@
 
     def _update_current_row(self) -> None:
         """Update the current row.
 
         Update the current row with the data stored in the logger.
         """
         for key in self._data:
+            old_data = self._current_row[key]
             if self._headers_minmax[key]:
-                old_data = self._current_row[f'{key}/Mean']
                 mean, min_val, max_val, std = self.get_stats(key, True)
-                self._current_row[f'{key}/Mean'] = mean
+                self._current_row[key] = mean
                 self._current_row[f'{key}/Min'] = min_val
                 self._current_row[f'{key}/Max'] = max_val
                 self._current_row[f'{key}/Std'] = std
             else:
-                old_data = self._current_row[key]
                 mean = self.get_stats(key, False)[0]
                 self._current_row[key] = mean
 
             if self._headers_delta[key]:
                 self._current_row[f'{key}/Delta'] = mean - old_data
 
-            if self._headers_windwos[key] is None:
+            if self._headers_windows[key] is None:
                 self._data[key] = []
 
-    def get_stats(self, key, min_and_max: bool = False) -> tuple[int | float, ...]:
+    def get_stats(
+        self,
+        key: str,
+        min_and_max: bool = False,
+    ) -> tuple[int | float, ...]:
         """Get the statistics of the key.
 
         Args:
             key (str): The key to be registered.
-            min_and_max (bool): Whether to record the min and max value of the key.
+            min_and_max (bool, optional): Whether to record the min and max value of the key.
+                Defaults to False.
+
+        Returns:
+            The mean value of the key or (mean, min, max, std) of the key.
         """
         assert key in self._current_row, f'Key {key} has not been registered'
         vals = self._data[key]
         if isinstance(vals, deque):
             vals = list(vals)
 
         if min_and_max:
             mean, std, min_val, max_val = dist_statistics_scalar(
                 torch.tensor(vals),
                 with_min_and_max=True,
             )
-            return mean.item(), min_val.item(), max_val.item(), std.item()
+            return mean.item(), min_val.mean().item(), max_val.mean().item(), std.item()
 
         mean, std = dist_statistics_scalar(  # pylint: disable=unbalanced-tuple-unpacking
             torch.tensor(vals),
         )
         return (mean.item(),)
 
     @property
```

### Comparing `omnisafe-0.3.0/omnisafe/common/normalizer.py` & `omnisafe-0.4.0/omnisafe/common/normalizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,35 @@
 
 from __future__ import annotations
 
 from typing import Any, Mapping
 
 import torch
 import torch.nn as nn
+from torch.nn.modules.module import _IncompatibleKeys
 
 
 class Normalizer(nn.Module):
-    """Calculate normalized raw_data from running mean and std
+    """Calculate normalized raw_data from running mean and std.
 
     References:
         - Title: Updating Formulae and a Pairwise Algorithm for Computing Sample Variances
         - Author: Tony F. Chan, Gene H. Golub, Randall J. LeVeque
         - URL: http://i.stanford.edu/pub/cstr/reports/cs/tr/79/773/CS-TR-79-773.pdf
     """
 
+    _mean: torch.Tensor  # running mean
+    _sumsq: torch.Tensor  # running sum of squares
+    _var: torch.Tensor  # running variance
+    _std: torch.Tensor  # running standard deviation
+    _count: torch.Tensor  # number of samples
+    _clip: torch.Tensor  # clip value
+
     def __init__(self, shape: tuple[int, ...], clip: float = 1e6) -> None:
-        """Initialize the normalize."""
+        """Initialize an instance of :class:`Normalizer`."""
         super().__init__()
         if shape == ():
             self.register_buffer('_mean', torch.tensor(0.0))
             self.register_buffer('_sumsq', torch.tensor(0.0))
             self.register_buffer('_var', torch.tensor(0.0))
             self.register_buffer('_std', torch.tensor(0.0))
             self.register_buffer('_count', torch.tensor(0))
@@ -45,23 +53,16 @@
             self.register_buffer('_mean', torch.zeros(*shape))
             self.register_buffer('_sumsq', torch.zeros(*shape))
             self.register_buffer('_var', torch.zeros(*shape))
             self.register_buffer('_std', torch.zeros(*shape))
             self.register_buffer('_count', torch.tensor(0))
             self.register_buffer('_clip', clip * torch.ones(*shape))
 
-        self._mean: torch.Tensor  # running mean
-        self._sumsq: torch.Tensor  # running sum of squares
-        self._var: torch.Tensor  # running variance
-        self._std: torch.Tensor  # running standard deviation
-        self._count: torch.Tensor  # number of samples
-        self._clip: torch.Tensor  # clip value
-
-        self._shape = shape
-        self._first = True
+        self._shape: tuple[int, ...] = shape
+        self._first: bool = True
 
     @property
     def shape(self) -> tuple[int, ...]:
         """Return the shape of the normalize."""
         return self._shape
 
     @property
@@ -71,41 +72,50 @@
 
     @property
     def std(self) -> torch.Tensor:
         """Return the std of the normalize."""
         return self._std
 
     def forward(self, data: torch.Tensor) -> torch.Tensor:
-        """Normalize the data."""
+        """Normalize the data.
+
+        Args:
+            data (torch.Tensor): raw data to be normalized.
+
+        Returns:
+            The normalized data.
+        """
         return self.normalize(data)
 
     def normalize(self, data: torch.Tensor) -> torch.Tensor:
         """Normalize the data.
 
         .. hint::
-
             - If the data is the first data, the data will be used to initialize the mean and std.
             - If the data is not the first data, the data will be normalized by the mean and std.
             - Update the mean and std by the data.
 
         Args:
-            data: raw data to be normalized.
+            data (torch.Tensor): The raw data to be normalized.
+
+        Returns:
+            The normalized data.
         """
         data = data.to(self._mean.device)
         self._push(data)
         if self._count <= 1:
             return data
         output = (data - self._mean) / self._std
         return torch.clamp(output, -self._clip, self._clip)
 
     def _push(self, raw_data: torch.Tensor) -> None:
         """Update the mean and std by the raw_data.
 
         Args:
-            raw_data: raw data to be normalized.
+            raw_data (torch.Tensor): The raw data to be normalized.
         """
         if raw_data.shape == self._shape:
             raw_data = raw_data.unsqueeze(0)
         assert raw_data.shape[1:] == self._shape, 'data shape must be equal to (batch_size, *shape)'
 
         if self._first:
             self._mean = torch.mean(raw_data, dim=0)
@@ -125,10 +135,24 @@
             sumq_raw = torch.sum((raw_data - mean_raw) ** 2, dim=0)
             self._sumsq += sumq_raw + delta**2 * self._count * count_raw / count
             self._count = count
         self._var = self._sumsq / (self._count - 1)
         self._std = torch.sqrt(self._var)
         self._std = torch.max(self._std, 1e-2 * torch.ones_like(self._std))
 
-    def load_state_dict(self, state_dict: Mapping[str, Any], strict: bool = True):
+    def load_state_dict(
+        self,
+        state_dict: Mapping[str, Any],
+        strict: bool = True,
+    ) -> _IncompatibleKeys:
+        """Load the state_dict to the normalizer.
+
+        Args:
+            state_dict (Mapping[str, Any]): The state_dict to be loaded.
+            strict (bool, optional): Whether to strictly enforce that the keys in :attr:`state_dict`.
+                Defaults to True.
+
+        Returns:
+            The loaded normalizer.
+        """
         self._first = False
         return super().load_state_dict(state_dict, strict)
```

### Comparing `omnisafe-0.3.0/omnisafe/common/pid_lagrange.py` & `omnisafe-0.4.0/omnisafe/common/pid_lagrange.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,33 +14,45 @@
 # ==============================================================================
 """Implementation of PID Lagrange."""
 
 from __future__ import annotations
 
 import abc
 from collections import deque
-from typing import Deque
 
 
 # pylint: disable-next=too-few-public-methods,too-many-instance-attributes
 class PIDLagrangian(abc.ABC):  # noqa: B024
-    """Abstract base class for Lagrangian-base Algorithms.
+    """PID version of Lagrangian.
 
-    Similar to the :class:`Lagrange` module, this module implements the PID version of the lagrangian method.
+    Similar to the :class:`Lagrange` module, this module implements the PID version of the
+    lagrangian method.
 
     .. note::
-        The PID-Lagrange is more general than the Lagrange, and can be used in any policy gradient algorithm.
-        As PID_Lagrange use the PID controller to control the lagrangian multiplier,
-        it is more stable than the naive Lagrange.
+        The PID-Lagrange is more general than the Lagrange, and can be used in any policy gradient
+        algorithm. As PID_Lagrange use the PID controller to control the lagrangian multiplier, it
+        is more stable than the naive Lagrange.
+
+    Args:
+        pid_kp (float): The proportional gain of the PID controller.
+        pid_ki (float): The integral gain of the PID controller.
+        pid_kd (float): The derivative gain of the PID controller.
+        pid_d_delay (int): The delay of the derivative term.
+        pid_delta_p_ema_alpha (float): The exponential moving average alpha of the delta_p.
+        pid_delta_d_ema_alpha (float): The exponential moving average alpha of the delta_d.
+        sum_norm (bool): Whether to use the sum norm.
+        diff_norm (bool): Whether to use the diff norm.
+        penalty_max (int): The maximum penalty.
+        lagrangian_multiplier_init (float): The initial value of the lagrangian multiplier.
+        cost_limit (float): The cost limit.
 
     References:
-
-    - Title: Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
-    - Authors: Joshua Achiam, David Held, Aviv Tamar, Pieter Abbeel.
-    - URL: `PID Lagrange <https://arxiv.org/abs/2007.03964>`_
+        - Title: Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
+        - Authors: Joshua Achiam, David Held, Aviv Tamar, Pieter Abbeel.
+        - URL: `PID Lagrange <https://arxiv.org/abs/2007.03964>`_
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         pid_kp: float,
         pid_ki: float,
@@ -48,73 +60,66 @@
         pid_d_delay: int,
         pid_delta_p_ema_alpha: float,
         pid_delta_d_ema_alpha: float,
         sum_norm: bool,
         diff_norm: bool,
         penalty_max: int,
         lagrangian_multiplier_init: float,
-        cost_limit: int,
+        cost_limit: float,
     ) -> None:
-        """Initialize PIDLagrangian.
-
-        Args:
-            pid_kp: The proportional gain of the PID controller.
-            pid_ki: The integral gain of the PID controller.
-            pid_kd: The derivative gain of the PID controller.
-            pid_d_delay: The delay of the derivative term of the PID controller.
-            pid_delta_p_ema_alpha: The exponential moving average alpha of the proportional term of the PID controller.
-            pid_delta_d_ema_alpha: The exponential moving average alpha of the derivative term of the PID controller.
-            sum_norm: Whether to normalize the sum of the cost.
-            diff_norm: Whether to normalize the difference of the cost.
-            penalty_max: The maximum penalty.
-            lagrangian_multiplier_init: The initial value of the lagrangian multiplier.
-            cost_limit: The cost limit.
-        """
-        self.pid_kp = pid_kp
-        self.pid_ki = pid_ki
-        self.pid_kd = pid_kd
-        self.pid_d_delay = pid_d_delay
-        self.pid_delta_p_ema_alpha = pid_delta_p_ema_alpha
-        self.pid_delta_d_ema_alpha = pid_delta_d_ema_alpha
-        self.penalty_max = penalty_max
-        self.sum_norm = sum_norm
-        self.diff_norm = diff_norm
-        self.pid_i = lagrangian_multiplier_init
-        self.cost_ds: Deque[float] = deque(maxlen=self.pid_d_delay)
-        self.cost_ds.append(0)
-        self._delta_p: float = 0
-        self._cost_d: float = 0
-        self.cost_limit: float = cost_limit
-        self.cost_penalty: float = 0
+        """Initialize an instance of :class:`PIDLagrangian`."""
+        self._pid_kp: float = pid_kp
+        self._pid_ki: float = pid_ki
+        self._pid_kd: float = pid_kd
+        self._pid_d_delay = pid_d_delay
+        self._pid_delta_p_ema_alpha: float = pid_delta_p_ema_alpha
+        self._pid_delta_d_ema_alpha: float = pid_delta_d_ema_alpha
+        self._penalty_max: int = penalty_max
+        self._sum_norm: bool = sum_norm
+        self._diff_norm: bool = diff_norm
+        self._pid_i: float = lagrangian_multiplier_init
+        self._cost_ds: deque[float] = deque(maxlen=self._pid_d_delay)
+        self._cost_ds.append(0.0)
+        self._delta_p: float = 0.0
+        self._cost_d: float = 0.0
+        self._cost_limit: float = cost_limit
+        self._cost_penalty: float = 0.0
+
+    @property
+    def lagrangian_multiplier(self) -> float:
+        """The lagrangian multiplier."""
+        return self._cost_penalty
 
     def pid_update(self, ep_cost_avg: float) -> None:
         r"""Update the PID controller.
 
-        Detailedly, PID controller update the lagrangian multiplier following the next equation:
+        PID controller update the lagrangian multiplier following the next equation:
 
         .. math::
+
             \lambda_{t+1} = \lambda_t + (K_p e_p + K_i \int e_p dt + K_d \frac{d e_p}{d t}) \eta
 
         where :math:`e_p` is the error between the current episode cost and the cost limit,
-        :math:`K_p`, :math:`K_i`, :math:`K_d` are the PID parameters, and :math:`\eta` is the learning rate.
+        :math:`K_p`, :math:`K_i`, :math:`K_d` are the PID parameters, and :math:`\eta` is the
+        learning rate.
 
         Args:
             ep_cost_avg (float): The average cost of the current episode.
         """
-        delta = float(ep_cost_avg - self.cost_limit)
-        self.pid_i = max(0.0, self.pid_i + delta * self.pid_ki)
-        if self.diff_norm:
-            self.pid_i = max(0.0, min(1.0, self.pid_i))
-        a_p = self.pid_delta_p_ema_alpha
+        delta = float(ep_cost_avg - self._cost_limit)
+        self._pid_i = max(0.0, self._pid_i + delta * self._pid_ki)
+        if self._diff_norm:
+            self._pid_i = max(0.0, min(1.0, self._pid_i))
+        a_p = self._pid_delta_p_ema_alpha
         self._delta_p *= a_p
         self._delta_p += (1 - a_p) * delta
-        a_d = self.pid_delta_d_ema_alpha
+        a_d = self._pid_delta_d_ema_alpha
         self._cost_d *= a_d
         self._cost_d += (1 - a_d) * float(ep_cost_avg)
-        pid_d = max(0.0, self._cost_d - self.cost_ds[0])
-        pid_o = self.pid_kp * self._delta_p + self.pid_i + self.pid_kd * pid_d
-        self.cost_penalty = max(0.0, pid_o)
-        if self.diff_norm:
-            self.cost_penalty = min(1.0, self.cost_penalty)
-        if not (self.diff_norm or self.sum_norm):
-            self.cost_penalty = min(self.cost_penalty, self.penalty_max)
-        self.cost_ds.append(self._cost_d)
+        pid_d = max(0.0, self._cost_d - self._cost_ds[0])
+        pid_o = self._pid_kp * self._delta_p + self._pid_i + self._pid_kd * pid_d
+        self._cost_penalty = max(0.0, pid_o)
+        if self._diff_norm:
+            self._cost_penalty = min(1.0, self._cost_penalty)
+        if not (self._diff_norm or self._sum_norm):
+            self._cost_penalty = min(self._cost_penalty, self._penalty_max)
+        self._cost_ds.append(self._cost_d)
```

### Comparing `omnisafe-0.3.0/omnisafe/common/statistics_tools.py` & `omnisafe-0.4.0/omnisafe/common/statistics_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,45 +16,51 @@
 
 from __future__ import annotations
 
 import itertools
 import json
 import os
 from copy import deepcopy
+from typing import Any, Generator
 
 from omnisafe.utils.plotter import Plotter
 from omnisafe.utils.tools import assert_with_exit, hash_string, recursive_dict2json, update_dict
 
 
 class StatisticsTools:
     """Analyze experiments results launched by experiment grid.
 
-    Users can choose any parameters to compare the results.
-    Aiming to help users to find the best hyperparameters faster.
+    Users can choose any parameters to compare the results. Aiming to help users to find the best
+    hyperparameter faster.
+
+    Attributes:
+        grid_config_dir (str): The directory of grid_config.json.
+        decompressed_grid_config (dict[str, Any]): The decompressed grid_config.json.
+        path_map_img_name (dict[str, Any]): The map from path to image name.
+        grid_config (dict[str, Any]): The grid_config.json.
+        exp_dir (str): The experiment directory.
+        plotter (Plotter): The plotter.
     """
 
+    grid_config_dir: str
+    decompressed_grid_config: dict[str, Any]
+    path_map_img_name: dict[str, Any]
+    grid_config: dict[str, Any]
+    exp_dir: str
+
     def __init__(self) -> None:
-        self.exp_dir: str  # experiment directory
-        self.grid_config_dir: str  # experiment's config directory
-        self.grid_config: dict  # experiment's config
-        # decompressed grid config
-        # e.g. {'algo_cfgs:update_cycle': 2048} -> {'algo_cfgs': {'update_cycle': 2048}}
-        self.decompressed_grid_config: dict
-        # map the path of data to the config which generate the name of image
-        self.path_map_img_name: dict
-        # plotter instance
-        self.plotter = Plotter()
+        """Initialize an instance of :class:`StatisticsTools`."""
+        self.plotter: Plotter = Plotter()
 
     def load_source(self, path: str) -> None:
         """Load experiment results.
 
         Args:
-            path (str): experiment directory.
+            path (str): The experiment directory.
         """
-
         # recursively find directory which is generated by experiment grid
         grid_config_dirs = []
         for root, _, files in os.walk(path):
             if 'grid_config.json' in files:
                 grid_config_dirs.append(files)
                 self.grid_config_dir = os.path.join(root, 'grid_config.json')
                 self.exp_dir = root
@@ -76,103 +82,126 @@
             raise FileNotFoundError(
                 'The config file is not found in the save directory.',
             ) from error
 
     def draw_graph(
         self,
         parameter: str,
-        values: list = None,
-        compare_num: int = None,
-        cost_limit: float = None,
-    ):
+        values: list[Any] | None = None,
+        compare_num: int | None = None,
+        cost_limit: float | None = None,
+        smooth: int = 1,
+        show_image: bool = False,
+    ) -> None:
         """Draw graph.
 
         Args:
-            parameter (str): name of parameter to analyze.
-            values (list): specific values of attribute,
-                if it is specified, will only compare values in it.
-            compare_num (int): number of values to compare,
-                if it is specified, will combine any potential combination to compare.
-            cost_limit (float) the cost limit to show in graphs by a single line.
-        .. Note::
+            parameter (str): The parameter to compare.
+            values (list[Any] or None, optional): The values of the parameter to compare. Defaults
+                to None.
+            compare_num (int or None, optional): The number of values to compare. Defaults to None.
+            cost_limit (float or None, optional): The cost limit of the experiment. Defaults to None.
+            smooth (int, optional): The smooth window size. Defaults to 1.
+            show_image (bool): Whether to show graph image in GUI windows.
+
+        .. note::
             `values` and `compare_num` cannot be set at the same time.
         """
         # check whether operation is valid
         assert_with_exit(
             not (values and compare_num),
             'values and compare_num cannot be set at the same time',
         )
         assert_with_exit(hasattr(self, 'grid_config'), 'please load source first')
         assert_with_exit(
             parameter in self.grid_config,
             f'parameter scope `{parameter}` is not in {self.grid_config}',
         )
 
         # decompress the grid config
-        decompressed_cfgs = {}
+        decompressed_cfgs: dict = {}
         for k, v in self.grid_config.items():
             update_dict(decompressed_cfgs, self.decompress_key(k, v))
         self.decompressed_grid_config = decompressed_cfgs
         parameter_values = self.get_compressed_key(self.decompressed_grid_config, parameter)
 
         # make config groups via the combination of parameter values
         if not (values or compare_num):
             compare_num = len(parameter_values)
         graph_paths = self.make_config_groups(parameter, parameter_values, values, compare_num)
 
         for graph_dict in graph_paths:
             legend = []
             log_dirs = []
-            for (param, value), path in graph_dict.items():  # noqa: B007
+            img_name_cfgs = {}
+            for (_, value), path in graph_dict.items():
                 legend += [f'{value}']
                 log_dirs += [path]
-                img_name_cfgs = self.path_map_img_name[path]
-            decompressed_img_name_cfgs = {}
+            img_name_cfgs = self.path_map_img_name[list(graph_dict.values())[-1]]
+            decompressed_img_name_cfgs: dict = {}
             for k, v in img_name_cfgs.items():
                 update_dict(decompressed_img_name_cfgs, self.decompress_key(k, v[0]))
             save_name = (
-                param[:10]  # pylint: disable=undefined-loop-variable
+                list(graph_dict.keys())[-1][0][:10]  # pylint: disable=undefined-loop-variable
                 + '---'
                 + decompressed_img_name_cfgs['env_id'][:30]
                 + '---'
                 + hash_string(recursive_dict2json(decompressed_img_name_cfgs))
             )
             try:
                 self.plotter.make_plots(
                     log_dirs,
                     legend,
                     'Steps',
                     'Rewards',
                     False,
                     cost_limit,
-                    1,
+                    smooth,
                     None,
                     None,
                     'mean',
                     save_name=save_name,
+                    show_image=show_image,
                 )
-            except RuntimeError:
+            except Exception:  # noqa # pylint: disable=broad-except
                 print(
                     f'Cannot generate graph for {save_name[:5] + str(decompressed_img_name_cfgs)}',
                 )
+                print(Exception)
 
-    def make_config_groups(self, parameter, parameter_values: list, values: list, compare_num: int):
+    def make_config_groups(
+        self,
+        parameter: str,
+        parameter_values: list[str],
+        values: list[Any] | None = None,
+        compare_num: int | None = None,
+    ) -> list[dict[tuple[str, Any], str]]:
         """Make config groups.
 
         Each group contains a list of config paths to compare.
+
+        .. warning::
+            `values` and `compare_num` cannot be set at the same time.
+
         Args:
-            parameter (str): name of parameter to analyze.
-            parameter_values (list): values of parameter.
-            values (list): specific values of attribute,
-                if it is specified, will only compare values in it.
-            compare_num (int): number of values to compare,
-                if it is specified, will combine any potential combination to compare.
+            parameter (str): The parameter to compare.
+            parameter_values (list[str]): The values of the parameter to compare.
+            values (list[Any] or None, optional): The values of the parameter to compare. Defaults
+                to None.
+            compare_num (int or None, optional): The number of values to compare. Defaults to None.
+
+        Returns:
+            A list of graph paths.
         """
         self.path_map_img_name = {}
+        parameter_values_combination: list[tuple] = []
         graph_groups: list[list] = []
+        assert (values is not None) ^ (
+            compare_num is not None
+        ), 'The values and compare_num cannot be set at the same time'
         if values:
             assert_with_exit(
                 all(v in parameter_values for v in values),
                 f'values `{values}` of parameter `{parameter}` is not subset of `{parameter_values}`',
             )
             # if values is specified, will only compare values in it
             parameter_values_combination = [tuple(values)]
@@ -182,15 +211,14 @@
                 (
                     f'compare_num `{compare_num}` is larger than number of values '
                     f'`{len(parameter_values)}` of parameter `{parameter}`'
                 ),
             )
             # if compare_num is specified, will combine any potential combination to compare
             parameter_values_combination = list(self.combine(parameter_values, compare_num))
-
         group_config = deepcopy(self.grid_config)
         # value of parameter is determined above
         group_config.pop(parameter)
         # seed is not a parameter
         group_config.pop('seed')
         if 'train_cfgs' in group_config:
             group_config['train_cfgs'].pop('device', None)
@@ -198,18 +226,18 @@
         # fix them in a single graph and only vary values of parameter which is specified by us
         for pinned_config in self.dict_permutations(group_config):
             group_config.update(pinned_config)
             for compare_value in parameter_values_combination:
                 group_config[parameter] = list(compare_value)
                 img_name_cfgs = deepcopy(group_config)
                 graph_groups.append(
-                    (
+                    [
                         img_name_cfgs,
                         self.variants(list(group_config.keys()), list(group_config.values())),
-                    ),
+                    ],
                 )
 
         graph_paths = []
         for img_name_cfgs, graph in graph_groups:
             paths = {}
             for path_dict in graph:
                 exp_name = (
@@ -219,37 +247,48 @@
                 self.path_map_img_name[path] = img_name_cfgs
                 para_val = (parameter, self.get_compressed_key(path_dict, parameter))
                 paths[para_val] = path
             graph_paths.append(paths)
 
         return graph_paths
 
-    def decompress_key(self, compressed_key, value):
+    def decompress_key(self, compressed_key: str, value: Any) -> dict[str, Any]:
         """This function is used to convert the custom configurations to dict.
 
         .. note::
-            This function is used to convert the custom configurations to dict.
-            For example, if the custom configurations are ``train_cfgs:use_wandb`` and ``True``,
-            then the output dict will be ``{'train_cfgs': {'use_wandb': True}}``.
+            This function is used to convert the custom configurations to dict. For example, if the
+            custom configurations are ``train_cfgs:use_wandb`` and ``True``, then the output dict
+            will be ``{'train_cfgs': {'use_wandb': True}}``.
 
         Args:
-            key (str): nested keys joined by `:`.
-            value (list): value.
+            compressed_key (str): The compressed key.
+            value (Any): The value of the compressed key.
+
+        Returns:
+            The decompressed dict.
         """
         keys_split = compressed_key.replace('-', '_').split(':')
         return_dict = {keys_split[-1]: value}
 
         for key in reversed(keys_split[:-1]):
             return_dict = {key.replace('-', '_'): return_dict}
         return return_dict
 
-    def _variants(self, keys, vals):
-        """Recursively builds list of valid variants."""
+    def _variants(self, keys: list[str], vals: list[Any]) -> list[dict[str, Any]]:
+        """Recursively builds list of valid variants.
+
+        Args:
+            keys (list[str]): The keys of the config.
+            vals (list[Any]): The values of the config.
+
+        Returns:
+            List of valid variants.
+        """
         if len(keys) == 1:
-            pre_variants: list[dict] = [{}]
+            pre_variants: list[dict[str, Any]] = [{}]
         else:
             pre_variants = self._variants(keys[1:], vals[1:])
 
         variants = []
         for val in vals[0]:
             for pre_v in pre_variants:
                 current_variants = deepcopy(pre_v)
@@ -259,122 +298,135 @@
                 for key in reversed(key_list[:-1]):
                     v_temp = {key: v_temp}
                 self.update_dict(current_variants, v_temp)
                 variants.append(current_variants)
 
         return variants
 
-    def update_dict(self, total_dic, item_dic):
-        """Updater of multi-level dictionary."""
-        for idd in item_dic:
-            total_value = total_dic.get(idd)
-            item_value = item_dic.get(idd)
+    def update_dict(self, total_dict: dict[str, Any], item_dict: dict[str, Any]) -> None:
+        """Updater of multi-level dictionary.
+
+        Args:
+            total_dict (dict[str, Any]): The total dictionary.
+            item_dict (dict[str, Any]): The item dictionary.
+        """
+        for idd in item_dict:
+            total_value = total_dict.get(idd)
+            item_value = item_dict.get(idd)
 
             if total_value is None:
-                total_dic.update({idd: item_value})
+                total_dict.update({idd: item_value})
             elif isinstance(item_value, dict):
                 self.update_dict(total_value, item_value)
-                total_dic.update({idd: total_value})
+                total_dict.update({idd: total_value})
             else:
                 total_value = item_value
-                total_dic.update({idd: total_value})
+                total_dict.update({idd: total_value})
 
-    def variants(self, keys, vals):
-        r"""Makes a list of dict, where each dict is a valid config in the grid.
+    def variants(self, keys: list[str], vals: list[Any]) -> list[dict[str, Any]]:
+        """Makes a list of dict, where each dict is a valid config in the grid.
 
-        There is special handling for variant parameters whose names take
-        the form
+        There is special handling for variant parameters whose names take the form
 
-            ``'full:param:name'``.
+            ``'full:param:name'``
 
-        The colons are taken to indicate that these parameters should
-        have a nested dict structure. eg, if there are two params,
+        The colons are taken to indicate that these parameters should have a nested dict structure.
+        For example, if there are two params,
 
-            ====================  ===
-            Key                   Val
-            ====================  ===
-            ``'base:param:a'``    1
-            ``'base:param:b'``    2
-            ====================  ===
+        ====================  ===
+        Key                   Val
+        ====================  ===
+        ``'base:param:a'``    1
+        ``'base:param:b'``    2
+        ====================  ===
 
         the variant dict will have the structure
 
         .. parsed-literal::
 
             variant = {
                 base: {
                     param : {
                         a : 1,
                         b : 2
                         }
                     }
                 }
+
+        Args:
+            keys (list[str]): The keys of the config.
+            vals (list[Any]): The values of the config.
+
+        Returns:
+            List of valid and not duplicate variants.
         """
         flat_variants = self._variants(keys, vals)
 
-        def unflatten_var(var):
+        def check_duplicate(var: dict[str, Any]) -> dict[str, Any]:
             """Build the full nested dict version of var, based on key names."""
             new_var: dict = {}
-            unflatten_set = set()
 
             for key, value in var.items():
-                if ':' in key:
-                    splits = key.split(':')
-                    k_0 = splits[0]
-                    assert k_0 not in new_var or isinstance(
-                        new_var[k_0],
-                        dict,
-                    ), "You can't assign multiple values to the same key."
-
-                    if k_0 not in new_var:
-                        new_var[k_0] = {}
-
-                    sub_k = ':'.join(splits[1:])
-                    new_var[k_0][sub_k] = value
-                    unflatten_set.add(k_0)
-                else:
-                    assert key not in new_var, "You can't assign multiple values to the same key."
-                    new_var[key] = value
-
-            # make sure to fill out the nested dict.
-            for key in unflatten_set:
-                new_var[key] = unflatten_var(new_var[key])
+                assert key not in new_var, "You can't assign multiple values to the same key."
+                new_var[key] = value
 
             return new_var
 
-        return [unflatten_var(var) for var in flat_variants]
+        return [check_duplicate(var) for var in flat_variants]
+
+    def combine(self, sequence: list[str], num_choosen: int) -> Generator:
+        """Combine elements in sequence to n elements.
+
+        Args:
+            sequence (list[str]): The sequence to be combined.
+            num_choosen (int): The number of elements to be combined.
 
-    def combine(self, sequence, num_choosen):
-        """Combine elements in sequence to n elements."""
+        Returns:
+            The generator of the combined elements.
+        """
         if num_choosen == 1:
             for i in sequence:
                 yield (i,)
         else:
-            for i, item in enumerate(sequence):
-                for nxt in self.combine(sequence[i + 1 :], num_choosen - 1):
+            for idx, item in enumerate(sequence):
+                for nxt in self.combine(sequence[idx + 1 :], num_choosen - 1):
                     yield (item, *nxt)
 
-    def dict_permutations(self, input_dict):
+    def dict_permutations(self, input_dict: dict[str, Any]) -> list[dict[str, Any]]:
         """Generate all possible combinations of the values in a dictionary.
 
-        Takes a dictionary with string keys and list values, and returns a dictionary
-        with all possible combinations of the lists as values for each key.
+        Takes a dictionary with string keys and list values, and returns a dictionary with all
+        possible combinations of the lists as values for each key.
+
+        Args:
+            input_dict (dict[str, Any]): The input dictionary.
+
+        Returns:
+            The list of all possible combinations of the values in a dictionary.
         """
         keys = list(input_dict.keys())
         values = list(input_dict.values())
         value_combinations = list(itertools.product(*values))
 
         result = []
         for combination in value_combinations:
             new_dict = {}
             for i, item in enumerate(keys):
                 new_dict[item] = [combination[i]]
             result.append(new_dict)
 
         return result
 
-    def get_compressed_key(self, dictionary, key):
-        """Get the value of the key."""
+    def get_compressed_key(self, dictionary: dict[str, Any], key: str) -> Any:
+        """Get the compressed value of the key.
+
+        Args:
+            dictionary (dict[str, Any]): the uncompressed dictionary.
+            key (str): the key.
+
+        Returns:
+            The compressed value of the key.
+        """
         inner_config = dictionary
         for k in key.split(':'):
             inner_config = inner_config[k]
         return inner_config
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/off-policy/DDPG.yaml` & `omnisafe-0.4.0/omnisafe/configs/off-policy/TD3.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -19,29 +19,29 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 1000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2000
     # number of steps per sample
-    steps_per_sample: 1
+    update_cycle: 1
     # number of iterations to update the policy
     update_iters: 1
     # The size of replay buffer
-    size: 100000
+    size: 1000000
     # The size of batch
     batch_size: 256
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
@@ -60,14 +60,18 @@
     start_learning_steps: 25000
     # The delay step of policy update
     policy_delay: 2
     # Whether to use the exploration noise
     use_exploration_noise: True
     # The exploration noise
     exploration_noise: 0.1
+    # The policy noise
+    policy_noise: 0.2
+    # policy_noise_clip
+    policy_noise_clip: 0.5
     # use cost
     use_cost: False
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
@@ -75,42 +79,34 @@
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 100
+    window_lens: 10
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type
     actor_type: mlp
     # linear learning rate decay
-    linear_lr_decay: True
+    linear_lr_decay: False
     # Configuration of Actor network
     actor:
       # Size of hidden layers
       hidden_sizes: [256, 256]
       # Activation function
       activation: relu
       # The learning rate of Actor network
       lr: 0.0003
     # Configuration of Critic network
     critic:
       # The number of critic networks
-      num_critics: 1
+      num_critics: 2
       # Size of hidden layers
       hidden_sizes: [256, 256]
       # Activation function
       activation: relu
       # The learning rate of Critic network
       lr: 0.0003
-
-SafetyHumanoidVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize observation
-    obs_normalize: True
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/off-policy/SAC.yaml` & `omnisafe-0.4.0/omnisafe/configs/off-policy/SAC.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -19,29 +19,29 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 1000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2000
     # number of steps per sample
-    steps_per_sample: 1
+    update_cycle: 1
     # number of iterations to update the policy
     update_iters: 1
     # The size of replay buffer
-    size: 100000
+    size: 1000000
     # The size of batch
     batch_size: 256
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
@@ -53,27 +53,27 @@
     # critic norm coefficient
     critic_norm_coeff: 0.001
     # The soft update coefficient
     polyak: 0.005
     # The discount factor of GAE
     gamma: 0.99
     # Actor perdorm random action before `start_learning_steps` steps
-    start_learning_steps: 5000
+    start_learning_steps: 10000
     # The delay step of policy update
     policy_delay: 2
     # Whether to use the exploration noise
-    use_exploration_noise: True
+    use_exploration_noise: False
     # The exploration noise
     exploration_noise: 0.1
     # The policy noise
     policy_noise: 0.2
     # policy_noise_clip
     policy_noise_clip: 0.5
     # The value of alpha
-    alpha: 0.2
+    alpha: 0.01
     # Whether to use auto alpha
     auto_alpha: False
     # use cost
     use_cost: False
   # logger configurations
   logger_cfgs:
     # use wandb for logging
@@ -83,23 +83,23 @@
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 100
+    window_lens: 10
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type
     actor_type: gaussian_sac
     # linear learning rate decay
-    linear_lr_decay: True
+    linear_lr_decay: False
     # Configuration of Actor network
     actor:
       # Size of hidden layers
       hidden_sizes: [256, 256]
       # Activation function
       activation: relu
       # The learning rate of Actor network
@@ -110,13 +110,7 @@
       num_critics: 2
       # Size of hidden layers
       hidden_sizes: [256, 256]
       # Activation function
       activation: relu
       # The learning rate of Critic network
       lr: 0.0003
-
-SafetySwimmerVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize observation
-    reward_normalize: True
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/off-policy/TD3.yaml` & `omnisafe-0.4.0/omnisafe/configs/off-policy/DDPG.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -19,29 +19,29 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 1000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2000
     # number of steps per sample
-    steps_per_sample: 1
+    update_cycle: 1
     # number of iterations to update the policy
     update_iters: 1
     # The size of replay buffer
-    size: 100000
+    size: 1000000
     # The size of batch
     batch_size: 256
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
@@ -55,23 +55,19 @@
     # The soft update coefficient
     polyak: 0.005
     # The discount factor of GAE
     gamma: 0.99
     # Actor perdorm random action before `start_learning_steps` steps
     start_learning_steps: 25000
     # The delay step of policy update
-    policy_delay: 2
+    policy_delay: 1
     # Whether to use the exploration noise
     use_exploration_noise: True
     # The exploration noise
     exploration_noise: 0.1
-    # The policy noise
-    policy_noise: 0.2
-    # policy_noise_clip
-    policy_noise_clip: 0.5
     # use cost
     use_cost: False
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
@@ -79,15 +75,15 @@
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 100
+    window_lens: 10
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type
     actor_type: mlp
     # linear learning rate decay
@@ -99,26 +95,14 @@
       # Activation function
       activation: relu
       # The learning rate of Actor network
       lr: 0.0003
     # Configuration of Critic network
     critic:
       # The number of critic networks
-      num_critics: 2
+      num_critics: 1
       # Size of hidden layers
       hidden_sizes: [256, 256]
       # Activation function
       activation: relu
       # The learning rate of Critic network
       lr: 0.0003
-
-SafetyAntVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize observation
-    obs_normalize: True
-
-SafetySwimmerVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize observation
-    reward_normalize: True
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/CPO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/CPO.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
@@ -114,34 +114,34 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: None
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
 
-SafetyHopperVelocity-v4:
+SafetyHopperVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: True
     # normalize observation
     obs_normalize: True
 
-SafetyWalker2dVelocity-v4:
+SafetyWalker2dVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: True
     # normalize observation
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/CUP.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/CUP.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -19,35 +19,35 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: True
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/FOCOPS.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/FOCOPS.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,35 +19,35 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: True
     # The threshold for KL divergence in each policy update
     focops_eta: 0.02
     # The hyperparameters related to the greediness of the algorithm
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/IPO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/IPO.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/NaturalPG.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/TRPO.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
@@ -60,16 +60,14 @@
     gamma: 0.99
     # cost discount factor
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
-    # clip ratio
-    clip: 0.2
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
@@ -114,54 +112,54 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: None
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
 
-SafetyAntVelocity-v4:
+SafetyAntVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: True
     # normalize cost
     cost_normalize: False
     # normalize observation
     obs_normalize: True
 
-SafetyHalfCheetahVelocity-v4:
+SafetyHalfCheetahVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: True
     # normalize cost
     cost_normalize: False
     # normalize observation
-    obs_normalize: True
+    obs_normalize: False
 
-SafetyHumanoidVelocity-v4:
+SafetyHumanoidVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: True
     # normalize cost
     cost_normalize: False
     # normalize observation
     obs_normalize: True
 
-SafetySwimmerVelocity-v4:
+SafetySwimmerVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: True
     # normalize cost
     cost_normalize: False
     # normalize observation
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/OnCRPO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/OnCRPO.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/P3O.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/P3O.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,23 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # the coefficient of cost penalty
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/PCPO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/PCPO.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
@@ -114,34 +114,34 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: None
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
 
-SafetyHopperVelocity-v4:
+SafetyHopperVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: True
     # normalize observation
     obs_normalize: True
 
-SafetyWalker2dVelocity-v4:
+SafetyWalker2dVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: True
     # normalize observation
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/PDO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/PDO.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/PPO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/PPOLag.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -19,35 +19,35 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: True
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
@@ -71,15 +71,15 @@
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
-    use_cost: False
+    use_cost: True
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -114,7 +114,17 @@
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.0003
+  # lagrangian configurations
+  lagrange_cfgs:
+    # Tolerance of constraint violation
+    cost_limit: 25.0
+    # Initial value of lagrangian multiplier
+    lagrangian_multiplier_init: 0.001
+    # Learning rate of lagrangian multiplier
+    lambda_lr: 0.035
+    # Type of lagrangian optimizer
+    lambda_optimizer: "Adam"
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/PPOLag.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/RCPO.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -27,31 +27,31 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
-    update_iters: 40
+    update_iters: 10
     # batch size for each iteration
-    batch_size: 64
+    batch_size: 128
     # target kl divergence
-    target_kl: 0.02
+    target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
     cost_normalize: True
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
-    kl_early_stop: True
+    kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
     max_grad_norm: 40.0
     # use critic norm
     use_critic_norm: True
     # critic norm coefficient
@@ -60,26 +60,32 @@
     gamma: 0.99
     # cost discount factor
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
-    # clip ratio
-    clip: 0.2
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
     use_cost: True
+    # Damping value for conjugate gradient
+    cg_damping: 0.1
+    # Number of conjugate gradient iterations
+    cg_iters: 15
+    # Subsampled observation
+    fvp_obs: None
+    # The sub-sampling rate of the observation
+    fvp_sample_freq: 1
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -93,38 +99,48 @@
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type, options: gaussian, gaussian_learning
     actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: True
+    linear_lr_decay: False
     # exploration noise anneal
     exploration_noise_anneal: False
     # std upper bound, and lower bound
     std_range: [0.5, 0.1]
     # actor network configurations
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: 0.001
   # lagrangian configurations
   lagrange_cfgs:
     # Tolerance of constraint violation
     cost_limit: 25.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
     lambda_lr: 0.035
     # Type of lagrangian optimizer
     lambda_optimizer: "Adam"
+
+SafetyHumanoidVelocity-v1:
+  # algorithm configurations
+  algo_cfgs:
+    # normalize reward
+    reward_normalize: True
+    # normalize cost
+    cost_normalize: True
+    # normalize observation
+    obs_normalize: True
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/PolicyGradient.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/NaturalPG.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -27,31 +27,31 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
-    batch_size: 64
+    batch_size: 128
     # target kl divergence
-    target_kl: 0.02
+    target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
-    kl_early_stop: True
+    kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
     max_grad_norm: 40.0
     # use critic norm
     use_critic_norm: True
     # critic norm coefficient
@@ -60,24 +60,34 @@
     gamma: 0.99
     # cost discount factor
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
+    # clip ratio
+    clip: 0.2
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
     use_cost: False
+    # Damping value for conjugate gradient
+    cg_damping: 0.1
+    # Number of conjugate gradient iterations
+    cg_iters: 15
+    # Subsampled observation
+    fvp_obs: None
+    # The sub-sampling rate of the observation
+    fvp_sample_freq: 1
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -91,28 +101,28 @@
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type, options: gaussian, gaussian_learning
     actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: True
+    linear_lr_decay: False
     # exploration noise anneal
     exploration_noise_anneal: False
     # std upper bound, and lower bound
     std_range: [0.5, 0.1]
     # actor network configurations
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: 0.001
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/RCPO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -23,31 +23,31 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 2
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 1000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
@@ -69,23 +69,33 @@
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
-    use_cost: True
+    use_cost: False
     # Damping value for conjugate gradient
     cg_damping: 0.1
     # Number of conjugate gradient iterations
     cg_iters: 15
     # Subsampled observation
     fvp_obs: None
     # The sub-sampling rate of the observation
     fvp_sample_freq: 1
+    # The safety budget, equal to the cost limit
+    safety_budget: 25.0
+    # the upper bound of safety budget
+    upper_budget: 25.0
+    # The saute gamma
+    saute_gamma: 0.999
+    # The max length of the episode
+    max_ep_len: 1000
+    # The reward when the agent is unsafe
+    unsafe_reward: -1.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -112,35 +122,25 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: None
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
-  # lagrangian configurations
-  lagrange_cfgs:
-    # Tolerance of constraint violation
-    cost_limit: 25.0
-    # Initial value of lagrangian multiplier
-    lagrangian_multiplier_init: 0.001
-    # Learning rate of lagrangian multiplier
-    lambda_lr: 0.035
-    # Type of lagrangian optimizer
-    lambda_optimizer: "Adam"
-
-SafetyHumanoidVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: True
-    # normalize observation
-    obs_normalize: True
+  # controller configurations
+  control_cfgs:
+    # The Kp of PID controller
+    kp: 1.0
+    # The Ki of PID controller
+    ki: 0.001
+    # The Kd of PID controller
+    kd: 0.01
+    # The polyak coefficient of the target
+    polyak: 0.995
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/TRPO.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOSaute.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 2
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 1000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
@@ -78,14 +78,22 @@
     cg_damping: 0.1
     # Number of conjugate gradient iterations
     cg_iters: 15
     # Subsampled observation
     fvp_obs: None
     # The sub-sampling rate of the observation
     fvp_sample_freq: 1
+    # The safety budget, equal to the cost limit
+    safety_budget: 25.0
+    # The saute gamma
+    saute_gamma: 0.999
+    # The max length of the episode
+    max_ep_len: 1000
+    # The reward when the agent is unsafe
+    unsafe_reward: -1.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -112,55 +120,15 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: None
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
-
-SafetyAntVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: True
-
-SafetyHalfCheetahVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: False
-
-SafetyHumanoidVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: True
-
-SafetySwimmerVelocity-v4:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: True
```

### Comparing `omnisafe-0.3.0/omnisafe/configs/on-policy/TRPOLag.yaml` & `omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOLag.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1024000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    update_cycle: 2048
+    steps_per_epoch: 2048
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
@@ -114,15 +114,15 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: None
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
@@ -133,25 +133,25 @@
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
     lambda_lr: 0.035
     # Type of lagrangian optimizer
     lambda_optimizer: "Adam"
 
-SafetyHopperVelocity-v4:
+SafetyHopperVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: True
     # normalize observation
     obs_normalize: True
 
-SafetyWalker2dVelocity-v4:
+SafetyWalker2dVelocity-v1:
   # algorithm configurations
   algo_cfgs:
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: True
     # normalize observation
```

### Comparing `omnisafe-0.3.0/omnisafe/envs/__init__.py` & `omnisafe-0.4.0/omnisafe/envs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,11 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Environment api for omnisafe."""
+"""Environment API for OmniSafe."""
 
 from omnisafe.envs.core import CMDP, env_register, make, support_envs
+from omnisafe.envs.mujoco_env import MujocoEnv
 from omnisafe.envs.safety_gymnasium_env import SafetyGymnasiumEnv
+from omnisafe.envs.safety_gymnasium_modelbased import SafetyGymnasiumModelBased
```

### Comparing `omnisafe-0.3.0/omnisafe/envs/core.py` & `omnisafe-0.4.0/omnisafe/envs/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,32 +18,35 @@
 
 import inspect
 from abc import ABC, abstractmethod
 from typing import Any
 
 import torch
 
-from omnisafe.typing import OmnisafeSpace
+from omnisafe.typing import DEVICE_CPU, OmnisafeSpace
+
+
+__all__ = [
+    'CMDP',
+    'Wrapper',
+    'env_register',
+    'support_envs',
+    'make',
+]
 
 
 class CMDP(ABC):
     """The core class of the environment.
 
-    The CMDP class is the core class of the environment. It defines the basic
-    interface of the environment. The environment should inherit from this class
-    and implement the abstract methods.
+    The CMDP class is the core class of the environment. It defines the basic interface of the
+    environment. The environment should inherit from this class and implement the abstract methods.
 
     Attributes:
-        _support_envs (List[str]): the supported environments.
-        _action_space (OmnisafeSpace): the action space of the environment.
-        _observation_space (OmnisafeSpace): the observation space of the environment.
-        _num_envs (int): the parallel environments, for env that not support parallel, num_envs should be 1
-        _time_limit (Optional[int]): the time limit of the environment, if None, the environment is infinite.
-        need_time_limit_wrapper (bool): whether the environment need time limit wrapper.
-        need_auto_reset_wrapper (bool): whether the environment need auto reset wrapper.
+        need_time_limit_wrapper (bool): Whether the environment need time limit wrapper.
+        need_auto_reset_wrapper (bool): Whether the environment need auto reset wrapper.
     """
 
     _support_envs: list[str]
     _action_space: OmnisafeSpace
     _observation_space: OmnisafeSpace
     _metadata: dict[str, Any]
 
@@ -53,273 +56,271 @@
     need_auto_reset_wrapper: bool
 
     @classmethod
     def support_envs(cls) -> list[str]:
         """The supported environments.
 
         Returns:
-            List[str]: the supported environments.
+            The supported environments.
         """
         return cls._support_envs
 
     @abstractmethod
-    def __init__(self, env_id: str, **kwargs) -> None:
-        """Initialize the environment.
-
-        Args:
-            env_id (str): the environment id.
-        """
+    def __init__(self, env_id: str, **kwargs: Any) -> None:
+        """Initialize an instance of :class:`CMDP`."""
         assert (
             env_id in self.support_envs()
         ), f'env_id {env_id} is not supported by {self.__class__.__name__}'
 
     @property
     def action_space(self) -> OmnisafeSpace:
-        """The action space of the environment.
-
-        Returns:
-            OmnisafeSpace: the action space.
-        """
+        """The action space of the environment."""
         return self._action_space
 
     @property
     def observation_space(self) -> OmnisafeSpace:
-        """The observation space of the environment.
-
-        Returns:
-            OmnisafeSpace: the observation space.
-        """
+        """The observation space of the environment."""
         return self._observation_space
 
     @property
     def metadata(self) -> dict[str, Any]:
-        """The metadata of the environment.
-
-        Returns:
-            Dict[str, Any]: the metadata.
-        """
+        """The metadata of the environment."""
         return self._metadata
 
     @property
     def num_envs(self) -> int:
-        """The parallel environments.
-
-        Returns:
-            int: the parallel environments.
-        """
+        """The number of parallel environments."""
         return self._num_envs
 
     @property
     def time_limit(self) -> int | None:
-        """The time limit of the environment.
-
-        Returns:
-            Optional[int]: the time limit of the environment.
-        """
+        """The time limit of the environment."""
         return self._time_limit
 
     @abstractmethod
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
 
     @abstractmethod
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
-        """Resets the environment and returns an initial observation.
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+        """Reset the environment and returns an initial observation.
 
         Args:
-            seed (Optional[int]): seed for the environment.
+            seed (int or None): Seed for the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): the initial observation of the space.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The initial observation of the space.
+            info: Some information logged by the environment.
         """
 
     @abstractmethod
     def set_seed(self, seed: int) -> None:
-        """Sets the seed for this env's random number generator(s).
+        """Set the seed for this env's random number generator(s).
 
         Args:
-            seed (int): the seed to use.
+            seed (int): The seed to use.
         """
 
     @abstractmethod
     def sample_action(self) -> torch.Tensor:
         """Sample an action from the action space.
 
         Returns:
-            torch.Tensor: the sampled action.
+            The sampled action.
         """
 
     @abstractmethod
     def render(self) -> Any:
         """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
-            Any: the render frames, we recommend to use `np.ndarray` which could construct video by moviepy.
+            The render frames, we recommend to use `np.ndarray` which could construct video by
+            moviepy.
         """
 
     def save(self) -> dict[str, torch.nn.Module]:
         """Save the important components of the environment.
+
+        .. note::
+            The saved components will be stored in the wrapped environment. If the environment is
+            not wrapped, the saved components will be empty dict. common wrappers are obs_normalize,
+            reward_normalize, and cost_normalize.
+
         Returns:
-            Dict[str, torch.nn.Module]: the saved components.
+            The saved components.
         """
         return {}
 
     @abstractmethod
     def close(self) -> None:
         """Close the environment."""
 
 
 class Wrapper(CMDP):
     """The wrapper class of the environment.
 
-    The Wrapper class is the wrapper class of the environment. It defines the basic
-    interface of the environment wrapper. The environment wrapper should inherit
-    from this class and implement the abstract methods.
+    The Wrapper class is the wrapper class of the environment. It defines the basic interface of the
+    environment wrapper. The environment wrapper should inherit from this class and implement the
+    abstract methods.
 
-    Attributes:
-        _env (CMDP): the environment.
+    Args:
+        env (CMDP): The environment.
+        device (torch.device): The device to use. Defaults to ``torch.device('cpu')``.
 
+    Attributes:
+        _env (CMDP): The environment.
     """
 
-    def __init__(self, env: CMDP, device: torch.device) -> None:
-        """Initialize the wrapper.
-
-        Args:
-            env (CMDP): the environment.
-
-        Attributes:
-            _env (CMDP): the environment.
-            _device (torch.device): the device of the environment.
-        """
-        self._env = env
-        self._device = device
+    def __init__(self, env: CMDP, device: torch.device = DEVICE_CPU) -> None:
+        """Initialize an instance of :class:`Wrapper`."""
+        self._env: CMDP = env
+        self._device: torch.device = device
 
     def __getattr__(self, name: str) -> Any:
         """Get the attribute of the environment.
 
         Args:
-            name (str): the attribute name.
+            name (str): The attribute name.
 
         Returns:
-            Any: the attribute.
+            The attribute.
         """
         if name.startswith('_'):
             raise AttributeError(f'attempted to get missing private attribute {name}')
         return getattr(self._env, name)
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         return self._env.step(action)
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
-        """Resets the environment and returns an initial observation.
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+        """Reset the environment and returns an initial observation.
 
         Args:
-            seed (Optional[int]): seed for the environment.
+            seed (int or None): Seed for the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): the initial observation of the space.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The initial observation of the space.
+            info: Some information logged by the environment.
         """
         return self._env.reset(seed)
 
     def set_seed(self, seed: int) -> None:
-        """Sets the seed for this env's random number generator(s).
+        """Set the seed for this env's random number generator(s).
 
         Args:
-            seed (int): the seed to use.
+            seed (int): The random seed to use.
         """
         self._env.set_seed(seed)
 
     def sample_action(self) -> torch.Tensor:
         """Sample an action from the action space.
 
         Returns:
-            torch.Tensor: the sampled action.
+            The sampled action.
         """
         return self._env.sample_action()
 
     def render(self) -> Any:
         """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
-            Any: the render frames, we recommend to use `np.ndarray` which could construct video by moviepy.
+            The render frames, we recommend to use `np.ndarray` which could construct video by
+            moviepy.
         """
         return self._env.render()
 
     def save(self) -> dict[str, torch.nn.Module]:
         """Save the important components of the environment.
 
+        .. note::
+            The saved components will be stored in the wrapped environment. If the environment is
+            not wrapped, the saved components will be empty dict. common wrappers are obs_normalize,
+            reward_normalize, and cost_normalize.
+
         Returns:
-            Dict[str, torch.nn.Module]: the saved components.
+            The saved components.
         """
         return self._env.save()
 
     def close(self) -> None:
         """Close the environment."""
         self._env.close()
 
 
 class EnvRegister:
     """The environment register.
 
-    The EnvRegister is used to register the environment class. It provides the
-    method to get the environment class by the environment id.
+    The EnvRegister is used to register the environment class. It provides the method to get the
+    environment class by the environment id.
 
-    Example:
+    Examples:
         >>> from omnisafe.envs.core import env_register
         >>> from cunstom_env import CustomEnv
         >>> @env_register
-        >>> class CustomEnv():
-
-    Attributes:
-        _class (Dict[str, Type[CMDP]]): the registered environment class.
-        _support_envs (Dict[str, List[str]]): the environment ids supported by the environment class.
+        ... class CustomEnv:
+        ...     ...
     """
 
     def __init__(self) -> None:
-        self._class: dict[str, type[CMDP]] = {}
-        self._support_envs: dict[str, list[str]] = {}
+        """Initialize an instance of :class:`EnvRegister`."""
+        self._class: dict[str, type[CMDP]]
+        self._support_envs: dict[str, list[str]]
+        self._class = {}
+        self._support_envs = {}
 
     def _register(self, env_class: type[CMDP]) -> None:
         """Register the environment class.
 
         Args:
-            env_class (Type[CMDP]): the environment class.
+            env_class (type[CMDP]): The environment class.
         """
         if not inspect.isclass(env_class):
             raise TypeError(f'{env_class} must be a class')
         class_name = env_class.__name__
         if not issubclass(env_class, CMDP):
             raise TypeError(f'{class_name} must be subclass of CMDP')
         if class_name in self._class:
@@ -328,31 +329,31 @@
         self._class[class_name] = env_class
         self._support_envs[class_name] = env_ids
 
     def register(self, env_class: type[CMDP]) -> type[CMDP]:
         """Register the environment class.
 
         Args:
-            env_class (Type[CMDP]): the environment class.
+            env_class (type[CMDP]): The environment class.
 
         Returns:
-            Type[CMDP]: the environment class.
+            The environment class.
         """
         self._register(env_class)
         return env_class
 
     def get_class(self, env_id: str, class_name: str | None) -> type[CMDP]:
         """Get the environment class.
 
         Args:
-            env_id (str): the environment id.
-            class_name (Optional[str]): the environment class name.
+            env_id (str): The environment id.
+            class_name (str or None): The environment class name.
 
         Returns:
-            Type[CMDP]: the environment class.
+            The environment class.
         """
         if class_name is not None:
             assert class_name in self._class, f'{class_name} is not registered'
             assert (
                 env_id in self._support_envs[class_name]
             ), f'{env_id} is not supported by {class_name}'
             return self._class[class_name]
@@ -362,40 +363,31 @@
                 return self._class[cls_name]
         raise ValueError(f'{env_id} is not supported by any environment class')
 
     def support_envs(self) -> list[str]:
         """The supported environments.
 
         Returns:
-            List[str]: the supported environments.
+            The supported environments.
         """
         return list({env_id for env_ids in self._support_envs.values() for env_id in env_ids})
 
 
 ENV_REGISTRY = EnvRegister()
 
 env_register = ENV_REGISTRY.register
 support_envs = ENV_REGISTRY.support_envs
 
 
-def make(env_id: str, class_name: str | None = None, **kwargs) -> CMDP:
+def make(env_id: str, class_name: str | None = None, **kwargs: Any) -> CMDP:
     """Create an environment.
 
     Args:
-        env_id (str): the environment id.
-        class_name (Optional[str]): the environment class name.
+        env_id (str): The environment id.
+        class_name (str or None): The environment class name.
         **kwargs: the keyword arguments for the environment initialization.
 
     Returns:
-        CMDP: the environment.
+        The environment class.
     """
     env_class = ENV_REGISTRY.get_class(env_id, class_name)
     return env_class(env_id, **kwargs)
-
-
-__all__ = [
-    'CMDP',
-    'Wrapper',
-    'env_register',
-    'support_envs',
-    'make',
-]
```

### Comparing `omnisafe-0.3.0/omnisafe/envs/safety_gymnasium_env.py` & `omnisafe-0.4.0/omnisafe/envs/safety_gymnasium_env.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,38 +8,47 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Environments in the Safety Gymnasium."""
+"""Environments in the Safety-Gymnasium."""
 
 from __future__ import annotations
 
 from typing import Any
 
 import numpy as np
 import safety_gymnasium
 import torch
 
 from omnisafe.envs.core import CMDP, env_register
+from omnisafe.typing import DEVICE_CPU, Box
 
 
 @env_register
 class SafetyGymnasiumEnv(CMDP):
     """Safety Gymnasium Environment.
 
+    Args:
+        env_id (str): Environment id.
+        num_envs (int, optional): Number of environments. Defaults to 1.
+        device (torch.device, optional): Device to store the data. Defaults to
+            ``torch.device('cpu')``.
+        **kwargs (Any): Other arguments.
+
     Attributes:
-        _support_envs (list[str]): List of supported environments.
         need_auto_reset_wrapper (bool): Whether to use auto reset wrapper.
         need_time_limit_wrapper (bool): Whether to use time limit wrapper.
     """
 
-    _support_envs = [
+    need_auto_reset_wrapper: bool = False
+    need_time_limit_wrapper: bool = False
+    _support_envs: list[str] = [
         'SafetyPointGoal0-v0',
         'SafetyPointGoal1-v0',
         'SafetyPointGoal2-v0',
         'SafetyPointButton0-v0',
         'SafetyPointButton1-v0',
         'SafetyPointButton2-v0',
         'SafetyPointPush0-v0',
@@ -68,75 +77,84 @@
         'SafetyAntButton2-v0',
         'SafetyAntPush0-v0',
         'SafetyAntPush1-v0',
         'SafetyAntPush2-v0',
         'SafetyAntCircle0-v0',
         'SafetyAntCircle1-v0',
         'SafetyAntCircle2-v0',
-        'SafetyHalfCheetahVelocity-v4',
-        'SafetyHopperVelocity-v4',
-        'SafetySwimmerVelocity-v4',
-        'SafetyWalker2dVelocity-v4',
-        'SafetyAntVelocity-v4',
-        'SafetyHumanoidVelocity-v4',
+        'SafetyHalfCheetahVelocity-v1',
+        'SafetyHopperVelocity-v1',
+        'SafetySwimmerVelocity-v1',
+        'SafetyWalker2dVelocity-v1',
+        'SafetyAntVelocity-v1',
+        'SafetyHumanoidVelocity-v1',
     ]
-    need_auto_reset_wrapper = False
-    need_time_limit_wrapper = False
 
     def __init__(
         self,
         env_id: str,
         num_envs: int = 1,
-        device: torch.device = 'cpu',
-        **kwargs,
+        device: torch.device = DEVICE_CPU,
+        **kwargs: Any,
     ) -> None:
-        """Initialize the environment.
-
-        Args:
-            env_id (str): Environment id.
-            num_envs (int, optional): Number of environments. Defaults to 1.
-            device (torch.device, optional): Device to store the data. Defaults to 'cpu'.
-            **kwargs: Other arguments.
-        """
+        """Initialize an instance of :class:`SafetyGymnasiumEnv`."""
         super().__init__(env_id)
+        self._num_envs = num_envs
+        self._device = torch.device(device)
         if num_envs > 1:
             self._env = safety_gymnasium.vector.make(env_id=env_id, num_envs=num_envs, **kwargs)
+            assert isinstance(self._env.single_action_space, Box), 'Only support Box action space.'
+            assert isinstance(
+                self._env.single_observation_space,
+                Box,
+            ), 'Only support Box observation space.'
             self._action_space = self._env.single_action_space
             self._observation_space = self._env.single_observation_space
         else:
+            self.need_time_limit_wrapper = True
+            self.need_auto_reset_wrapper = True
             self._env = safety_gymnasium.make(id=env_id, autoreset=True, **kwargs)
+            assert isinstance(self._env.action_space, Box), 'Only support Box action space.'
+            assert isinstance(
+                self._env.observation_space,
+                Box,
+            ), 'Only support Box observation space.'
             self._action_space = self._env.action_space
             self._observation_space = self._env.observation_space
-
-        self._num_envs = num_envs
         self._metadata = self._env.metadata
-        self._device = torch.device(device)
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Step the environment.
 
         .. note::
-
-            OmniSafe use auto reset wrapper to reset the environment when the episode is
-            terminated. So the ``obs`` will be the first observation of the next episode.
-            And the true ``final_observation`` in ``info`` will be stored in the ``final_observation`` key of ``info``.
+            OmniSafe uses auto reset wrapper to reset the environment when the episode is
+            terminated. So the ``obs`` will be the first observation of the next episode. And the
+            true ``final_observation`` in ``info`` will be stored in the ``final_observation`` key
+            of ``info``.
 
         Args:
             action (torch.Tensor): Action to take.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         obs, reward, cost, terminated, truncated, info = self._env.step(
             action.detach().cpu().numpy(),
         )
         obs, reward, cost, terminated, truncated = (
             torch.as_tensor(x, dtype=torch.float32, device=self._device)
             for x in (obs, reward, cost, terminated, truncated)
@@ -152,23 +170,24 @@
                 info['final_observation'],
                 dtype=torch.float32,
                 device=self._device,
             )
 
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment.
 
         Args:
-            seed (int, optional): Seed to reset the environment. Defaults to None.
+            seed (int or None, optional): Seed to reset the environment.
+                Defaults to None.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: Agent's observation of the current environment.
+            info: Some information logged by the environment.
         """
         obs, info = self._env.reset(seed=seed)
         return torch.as_tensor(obs, dtype=torch.float32, device=self._device), info
 
     def set_seed(self, seed: int) -> None:
         """Set the seed for the environment.
 
@@ -177,26 +196,26 @@
         """
         self.reset(seed=seed)
 
     def sample_action(self) -> torch.Tensor:
         """Sample a random action.
 
         Returns:
-            torch.Tensor: A random action.
+            A random action.
         """
         return torch.as_tensor(
             self._env.action_space.sample(),
             dtype=torch.float32,
             device=self._device,
         )
 
     def render(self) -> Any:
         """Render the environment.
 
         Returns:
-            Any: Rendered environment.
+            Rendered image.
         """
         return self._env.render()
 
     def close(self) -> None:
         """Close the environment."""
         self._env.close()
```

### Comparing `omnisafe-0.3.0/omnisafe/envs/wrapper.py` & `omnisafe-0.4.0/omnisafe/envs/wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,85 +12,92 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Wrapper for the environment."""
 
 from __future__ import annotations
 
+from typing import Any
+
 import numpy as np
 import torch
 from gymnasium import spaces
 
 from omnisafe.common import Normalizer
 from omnisafe.envs.core import CMDP, Wrapper
 
 
 class TimeLimit(Wrapper):
     """Time limit wrapper for the environment.
 
-    Example:
+    .. warning::
+        The time limit wrapper only supports single environment.
+
+    Examples:
         >>> env = TimeLimit(env, time_limit=100)
 
+    Args:
+        env (CMDP): The environment to wrap.
+        time_limit (int): The time limit for each episode.
+        device (torch.device): The torch device to use.
+
     Attributes:
         _time_limit (int): The time limit for each episode.
         _time (int): The current time step.
     """
 
     def __init__(self, env: CMDP, time_limit: int, device: torch.device) -> None:
-        """Initialize the time limit wrapper.
-
-        .. warning::
-            The time limit wrapper only supports single environment.
-
-        Args:
-            env (CMDP): The environment to wrap.
-            time_limit (int): The time limit for each episode.
-        """
+        """Initialize an instance of :class:`TimeLimit`."""
         super().__init__(env=env, device=device)
-
         assert self.num_envs == 1, 'TimeLimit only supports single environment'
-
-        self._time_limit: int = time_limit
         self._time: int = 0
+        self._time_limit: int = time_limit
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment.
 
         .. note::
             Additionally, the time step will be reset to 0.
 
         Args:
-            seed (int, optional): The seed for the environment. Defaults to None.
+            seed (int or None, optional): The seed for the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): the initial observation of the space.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The initial observation of the space.
+            info: Some information logged by the environment.
         """
         self._time = 0
         return super().reset(seed)
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         .. note::
             Additionally, the time step will be increased by 1.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         obs, reward, cost, terminated, truncated, info = super().step(action)
 
         self._time += 1
         truncated = torch.tensor(
             self._time >= self._time_limit,
             dtype=torch.bool,
@@ -99,45 +106,56 @@
 
         return obs, reward, cost, terminated, truncated, info
 
 
 class AutoReset(Wrapper):
     """Auto reset the environment when the episode is terminated.
 
-    Example:
+    Examples:
         >>> env = AutoReset(env)
 
+    Args:
+        env (CMDP): The environment to wrap.
+        device (torch.device): The torch device to use.
     """
 
     def __init__(self, env: CMDP, device: torch.device) -> None:
+        """Initialize an instance of :class:`AutoReset`."""
         super().__init__(env=env, device=device)
 
         assert self.num_envs == 1, 'AutoReset only supports single environment'
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         .. note::
-            If the episode is terminated, the environment will be reset.
-            The ``obs`` will be the first observation of the new episode.
-            And the true final observation will be stored in ``info['final_observation']``.
+            If the episode is terminated, the environment will be reset. The ``obs`` will be the
+            first observation of the new episode. And the true final observation will be stored in
+            ``info['final_observation']``.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         obs, reward, cost, terminated, truncated, info = super().step(action)
 
         if terminated or truncated:
             new_obs, new_info = self.reset()
             assert (
                 'final_observation' not in new_info
@@ -152,345 +170,447 @@
 
         return obs, reward, cost, terminated, truncated, info
 
 
 class ObsNormalize(Wrapper):
     """Normalize the observation.
 
-    Example:
+    Examples:
         >>> env = ObsNormalize(env)
-        >>> norm = Normalizer(env.observation_space.shape) # load saved normalizer
+        >>> norm = Normalizer(env.observation_space.shape)  # load saved normalizer
         >>> env = ObsNormalize(env, norm)
 
-    Attributes:
-        _obs_normalizer (Normalizer): The normalizer for the observation.
+    Args:
+        env (CMDP): The environment to wrap.
+        device (torch.device): The torch device to use.
+        norm (Normalizer or None, optional): The normalizer to use. Defaults to None.
     """
 
     def __init__(self, env: CMDP, device: torch.device, norm: Normalizer | None = None) -> None:
+        """Initialize an instance of :class:`ObsNormalize`."""
         super().__init__(env=env, device=device)
         assert isinstance(self.observation_space, spaces.Box), 'Observation space must be Box'
+        self._obs_normalizer: Normalizer
 
         if norm is not None:
             self._obs_normalizer = norm.to(self._device)
         else:
             self._obs_normalizer = Normalizer(self.observation_space.shape, clip=5).to(self._device)
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         .. note::
             The observation and the ``info['final_observation']`` will be normalized.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         obs, reward, cost, terminated, truncated, info = super().step(action)
         if 'final_observation' in info:
             final_obs_slice = info['_final_observation'] if self.num_envs > 1 else slice(None)
             info['final_observation'] = info['final_observation'].to(self._device)
             info['original_final_observation'] = info['final_observation']
             info['final_observation'][final_obs_slice] = self._obs_normalizer.normalize(
                 info['final_observation'][final_obs_slice],
             )
         info['original_obs'] = obs
         obs = self._obs_normalizer.normalize(obs)
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
-        """Resets the environment and returns an initial observation.
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+        """Reset the environment and returns an initial observation.
 
         Args:
-            seed (Optional[int]): seed for the environment.
+            seed (int or None, optional): Seed for the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): the initial observation of the space.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The initial observation of the space.
+            info: Some information logged by the environment.
         """
         obs, info = super().reset(seed)
         info['original_obs'] = obs
         obs = self._obs_normalizer.normalize(obs)
         return obs, info
 
     def save(self) -> dict[str, torch.nn.Module]:
-        """Save the normalizer.
+        """Save the observation normalizer.
 
         .. note::
-            When evaluating the saved model, the normalizer should be loaded.
+            The saved components will be stored in the wrapped environment. If the environment is
+            not wrapped, the saved components will be empty dict. common wrappers are obs_normalize,
+            reward_normalize, and cost_normalize. When evaluating the saved model, the normalizer
+            should be loaded.
 
         Returns:
-            dict[str, torch.nn.Module]: The saved normalizer.
+            The saved components, that is the observation normalizer.
         """
         saved = super().save()
         saved['obs_normalizer'] = self._obs_normalizer
         return saved
 
 
 class RewardNormalize(Wrapper):
     """Normalize the reward.
 
-    Example:
+    Examples:
         >>> env = RewardNormalize(env)
         >>> norm = Normalizer(()) # load saved normalizer
         >>> env = RewardNormalize(env, norm)
 
+    Args:
+        env (CMDP): The environment to wrap.
+        device (torch.device): The torch device to use.
+        norm (Normalizer or None, optional): The normalizer to use. Defaults to None.
     """
 
     def __init__(self, env: CMDP, device: torch.device, norm: Normalizer | None = None) -> None:
-        """Initialize the reward normalizer.
-
-        Args:
-            env (CMDP): The environment to wrap.
-            norm (Optional[Normalizer], optional): The normalizer to use. Defaults to None.
-
-        """
+        """Initialize an instance of :class:`RewardNormalize`."""
         super().__init__(env=env, device=device)
+        self._reward_normalizer: Normalizer
+
         if norm is not None:
             self._reward_normalizer = norm.to(self._device)
         else:
             self._reward_normalizer = Normalizer((), clip=5).to(self._device)
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
-
         .. note::
-            The reward will be normalized for agent training.
-            Then the original reward will be stored in ``info['original_reward']`` for logging.
+            The reward will be normalized for agent training. Then the original reward will be
+            stored in ``info['original_reward']`` for logging.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         obs, reward, cost, terminated, truncated, info = super().step(action)
         info['original_reward'] = reward
         reward = self._reward_normalizer.normalize(reward)
         return obs, reward, cost, terminated, truncated, info
 
     def save(self) -> dict[str, torch.nn.Module]:
-        """Save the normalizer.
+        """Save the reward normalizer.
+
+        .. note::
+            The saved components will be stored in the wrapped environment. If the environment is
+            not wrapped, the saved components will be empty dict. common wrappers are obs_normalize,
+            reward_normalize, and cost_normalize.
 
         Returns:
-            dict[str, torch.nn.Module]: The saved normalizer.
+            The saved components, that is the reward normalizer.
         """
         saved = super().save()
         saved['reward_normalizer'] = self._reward_normalizer
         return saved
 
 
 class CostNormalize(Wrapper):
     """Normalize the cost.
 
-    Example:
+    Examples:
         >>> env = CostNormalize(env)
         >>> norm = Normalizer(()) # load saved normalizer
         >>> env = CostNormalize(env, norm)
+
+    Args:
+        env (CMDP): The environment to wrap.
+        device (torch.device): The torch device to use.
+        norm (Normalizer or None, optional): The normalizer to use. Defaults to None.
     """
 
     def __init__(self, env: CMDP, device: torch.device, norm: Normalizer | None = None) -> None:
-        """Initialize the cost normalizer.
-
-        Args:
-            env (CMDP): The environment to wrap.
-            norm (Normalizer, optional): The normalizer to use. Defaults to None.
-        """
+        """Initialize an instance of :class:`CostNormalize`."""
         super().__init__(env=env, device=device)
+        self._cost_normalizer: Normalizer
+
         if norm is not None:
-            self._obs_normalizer = norm.to(self._device)
+            self._cost_normalizer = norm.to(self._device)
         else:
             self._cost_normalizer = Normalizer((), clip=5).to(self._device)
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         .. note::
-            The cost will be normalized for agent training.
-            Then the original reward will be stored in ``info['original_cost']`` for logging.
+            The cost will be normalized for agent training. Then the original reward will be stored
+            in ``info['original_cost']`` for logging.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         obs, reward, cost, terminated, truncated, info = super().step(action)
         info['original_cost'] = cost
         cost = self._cost_normalizer.normalize(cost)
         return obs, reward, cost, terminated, truncated, info
 
     def save(self) -> dict[str, torch.nn.Module]:
+        """Save the cost normalizer.
+
+        .. note::
+            The saved components will be stored in the wrapped environment. If the environment is
+            not wrapped, the saved components will be empty dict. common wrappers are obs_normalize,
+            reward_normalize, and cost_normalize.
+
+        Returns:
+            The saved components, that is the cost normalizer.
+        """
         saved = super().save()
         saved['cost_normalizer'] = self._cost_normalizer
         return saved
 
 
 class ActionScale(Wrapper):
     """Scale the action space to a given range.
 
-    Example:
+    Examples:
         >>> env = ActionScale(env, low=-1, high=1)
         >>> env.action_space
         Box(-1.0, 1.0, (1,), float32)
+
+    Args:
+        env (CMDP): The environment to wrap.
+        device (torch.device): The device to use.
+        low (int or float): The lower bound of the action space.
+        high (int or float): The upper bound of the action space.
     """
 
     def __init__(
         self,
         env: CMDP,
         device: torch.device,
         low: int | float,
         high: int | float,
     ) -> None:
-        """Initialize the wrapper.
-
-        Args:
-            env: The environment to wrap.
-            low: The lower bound of the action space.
-            high: The upper bound of the action space.
-        """
+        """Initialize an instance of :class:`ActionScale`."""
         super().__init__(env=env, device=device)
         assert isinstance(self.action_space, spaces.Box), 'Action space must be Box'
 
-        self._old_min_action = torch.tensor(
+        self._old_min_action: torch.Tensor = torch.tensor(
             self.action_space.low,
             dtype=torch.float32,
             device=self._device,
         )
-        self._old_max_action = torch.tensor(
+        self._old_max_action: torch.Tensor = torch.tensor(
             self.action_space.high,
             dtype=torch.float32,
             device=self._device,
         )
 
         min_action = np.zeros(self.action_space.shape, dtype=self.action_space.dtype) + low
         max_action = np.zeros(self.action_space.shape, dtype=self.action_space.dtype) + high
-        self._action_space = spaces.Box(
+        self._action_space: spaces.Box = spaces.Box(
             low=min_action,
             high=max_action,
             shape=self.action_space.shape,
-            dtype=self.action_space.dtype,  # type: ignore
+            dtype=self.action_space.dtype,  # type: ignore[arg-type]
         )
 
-        self._min_action = torch.tensor(min_action, dtype=torch.float32, device=self._device)
-        self._max_action = torch.tensor(max_action, dtype=torch.float32, device=self._device)
+        self._min_action: torch.Tensor = torch.tensor(
+            min_action,
+            dtype=torch.float32,
+            device=self._device,
+        )
+        self._max_action: torch.Tensor = torch.tensor(
+            max_action,
+            dtype=torch.float32,
+            device=self._device,
+        )
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         .. note::
             The action will be scaled to the original range for agent training.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         action = self._old_min_action + (self._old_max_action - self._old_min_action) * (
             action - self._min_action
         ) / (self._max_action - self._min_action)
         return super().step(action)
 
 
-class Unsqueeze(Wrapper):
-    """Unsqueeze the observation, reward, cost, terminated, truncated and info.
+class ActionRepeat(Wrapper):
+    """Repeat ab action given times.
 
     Example:
-        >>> env = Unsqueeze(env)
+        >>> env = ActionRepeat(env, times=3)
     """
 
-    def __init__(self, env: CMDP, device: torch.device) -> None:
+    def __init__(
+        self,
+        env: CMDP,
+        times: int,
+        device: torch.device,
+    ) -> None:
         """Initialize the wrapper.
 
         Args:
             env: The environment to wrap.
+            times: The number of times to repeat the action.
             device: The device to use.
         """
         super().__init__(env=env, device=device)
+        self._times = times
+        self._device = device
+
+    def step(
+        self,
+        action: torch.Tensor,
+    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+        """Run self._times timesteps of the environment's dynamics using the agent actions."""
+        rewards, costs = torch.tensor(0.0).to(self._device), torch.tensor(0.0).to(self._device)
+        for _step, _ in enumerate(range(self._times)):
+            obs, reward, cost, terminated, truncated, info = super().step(action)
+            rewards += reward
+            costs += cost
+            goal_met = info.get('goal_met', False)
+            if terminated or truncated or goal_met:
+                break
+        info['num_step'] = _step + 1
+        return obs, rewards, costs, terminated, truncated, info
+
+
+class Unsqueeze(Wrapper):
+    """Unsqueeze the observation, reward, cost, terminated, truncated and info.
+
+    Examples:
+        >>> env = Unsqueeze(env)
+    """
+
+    def __init__(self, env: CMDP, device: torch.device) -> None:
+        """Initialize an instance of :class:`Unsqueeze`."""
+        super().__init__(env=env, device=device)
         assert self.num_envs == 1, 'Unsqueeze only works with single environment'
         assert isinstance(self.observation_space, spaces.Box), 'Observation space must be Box'
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Run one timestep of the environment's dynamics using the agent actions.
 
         .. note::
             The vector information will be unsqueezed to (1, dim) for agent training.
 
         Args:
-            action (torch.Tensor): action.
+            action (torch.Tensor): The action from the agent or random.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         action = action.squeeze(0)
         obs, reward, cost, terminated, truncated, info = super().step(action)
         obs, reward, cost, terminated, truncated = (
             x.unsqueeze(0) for x in (obs, reward, cost, terminated, truncated)
         )
         for k, v in info.items():
             if isinstance(v, torch.Tensor):
                 info[k] = v.unsqueeze(0)
 
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
-        """Resets the environment and returns a new observation.
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+        """Reset the environment and returns a new observation.
 
         .. note::
             The vector information will be unsqueezed to (1, dim) for agent training.
 
         Args:
-            seed (int): The seed to use for the environment.
+            seed (int or None, optional): Set the seed for the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): The initial observation of the space. Initial reward is assumed to be 0.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The initial observation of the space.
+            info: Some information logged by the environment.
         """
         obs, info = super().reset(seed)
         obs = obs.unsqueeze(0)
         for k, v in info.items():
             if isinstance(v, torch.Tensor):
                 info[k] = v.unsqueeze(0)
```

### Comparing `omnisafe-0.3.0/omnisafe/evaluator.py` & `omnisafe-0.4.0/omnisafe/adapter/modelbased_adapter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,334 +1,382 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of Evaluator."""
-
+"""Model-based Adapter for OmniSafe."""
 from __future__ import annotations
 
-import json
-import os
-import warnings
-from typing import Any
+import time
+from typing import Any, Callable
 
-import numpy as np
 import torch
-from gymnasium.spaces import Box
-from gymnasium.utils.save_video import save_video
 
-from omnisafe.common import Normalizer
-from omnisafe.envs.core import CMDP, make
-from omnisafe.envs.wrapper import ActionScale, ObsNormalize, TimeLimit
-from omnisafe.models.actor import ActorBuilder
-from omnisafe.models.base import Actor
+from omnisafe.adapter.online_adapter import OnlineAdapter
+from omnisafe.common.logger import Logger
+from omnisafe.envs.core import make, support_envs
+from omnisafe.envs.wrapper import (
+    ActionRepeat,
+    ActionScale,
+    AutoReset,
+    CostNormalize,
+    ObsNormalize,
+    RewardNormalize,
+    TimeLimit,
+    Unsqueeze,
+)
 from omnisafe.utils.config import Config
 
 
-class Evaluator:  # pylint: disable=too-many-instance-attributes
-    """This class includes common evaluation methods for safe RL algorithms."""
+class ModelBasedAdapter(
+    OnlineAdapter,
+):  # pylint: disable=too-many-instance-attributes,super-init-not-called
+    """Model Based Adapter for OmniSafe.
+
+    :class:`ModelBasedAdapter` is used to adapt the environment to the model-based training.
+
+
+    Args:
+        env_id (str): The environment id.
+        num_envs (int): The number of environments.
+        seed (int): The random seed.
+        cfgs (Config): The configuration.
+        kwargs(dict): The other keyword arguments.
+
+    Attributes:
+        _env_id (str): The environment id.
+        _device (torch.device): The device.
+        _env (CMDP): The environment.
+        _cfgs (Config): The configuration.
+        _ep_ret (torch.Tensor): The episode return.
+        _ep_cost (torch.Tensor): The episode cost.
+        _ep_len (torch.Tensor): The episode length.
+        _last_dynamics_update (float): The last time of dynamics update.
+        _last_policy_update (float): The last time of policy update.
+        _last_eval (float): The last time of evaluation.
+        coordinate_observation_space (OmnisafeSpace): The coordinate observation space.
+        lidar_observation_space (OmnisafeSpace): The lidar observation space.
+        task (str): The task. eg. The task of SafetyPointGoal-v0 is 'goal'
+    """
 
-    # pylint: disable-next=too-many-arguments
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
-        env: CMDP | None = None,
-        actor: Actor | None = None,
-        render_mode: str | None = None,
+        env_id: str,
+        num_envs: int,
+        seed: int,
+        cfgs: Config,
+        **kwargs: Any,
     ) -> None:
-        """Initialize the evaluator.
+        """Initialize the model-based adapter."""
+        assert env_id in support_envs(), f'Env {env_id} is not supported.'
 
-        Args:
-            env (gymnasium.Env): the environment. if None, the environment will be created from the config.
-            pi (omnisafe.algos.models.actor.Actor): the policy. if None, the policy will be created from the config.
-            obs_normalize (omnisafe.algos.models.obs_normalize): the observation Normalize.
-        """
-        # set the attributes
-        self._env: CMDP = env
-        self._actor: Actor = actor
+        self._env_id = env_id
+        self._device = cfgs.train_cfgs.device
 
-        # used when load model from saved file.
-        self._cfgs: Config
-        self._save_dir: str
-        self._model_name: str
+        self._env = make(env_id, num_envs=num_envs, device=cfgs.train_cfgs.device, **kwargs)
 
-        self._dividing_line = '\n' + '#' * 50 + '\n'
+        # wrap the environment, use the action repeat in model-based setting.
+        self._wrapper(
+            obs_normalize=cfgs.algo_cfgs.obs_normalize,
+            reward_normalize=cfgs.algo_cfgs.reward_normalize,
+            cost_normalize=cfgs.algo_cfgs.cost_normalize,
+            action_repeat=cfgs.algo_cfgs.action_repeat,
+        )
+        self._env.set_seed(seed)
+        self._cfgs = cfgs
+        if hasattr(self._env, 'coordinate_observation_space') and hasattr(
+            self._env,
+            'lidar_observation_space',
+        ):
+            self.coordinate_observation_space = self._env.coordinate_observation_space
+            self.lidar_observation_space = self._env.lidar_observation_space
+        else:
+            self.coordinate_observation_space = None
+            self.lidar_observation_space = None
+        if hasattr(self._env, 'task'):
+            self.task = self._env.task
+        else:
+            self.task = None
 
-        self.__set_render_mode(render_mode)
+        self._ep_ret: torch.Tensor
+        self._ep_cost: torch.Tensor
+        self._ep_len: torch.Tensor
+        self._current_obs, _ = self.reset()
+        self._max_ep_len = 1000
+        self._reset_log()
+        self._last_dynamics_update = 0
+        self._last_policy_update = 0
+        self._last_eval = 0
+        self._first_log = False
 
-    def __set_render_mode(self, render_mode: str):
-        """Set the render mode.
+    def get_goal_flag_from_obs_tensor(self, obs: torch.Tensor) -> torch.Tensor | None:
+        """Get goal flag from tensor observation.
 
         Args:
-            play (bool): whether to play the video.
-            save_replay (bool): whether to save the video.
+            obs (torch.Tensor): The observation.
         """
-        # set the render mode
-        if render_mode in ['human', 'rgb_array', 'rgb_array_list', None]:
-            self._render_mode = render_mode
-        else:
-            raise NotImplementedError('The render mode is not implemented.')
+        return (
+            self._env.get_goal_flag_from_obs_tensor(obs)
+            if hasattr(self._env, 'get_goal_flag_from_obs_tensor')
+            else None
+        )
 
-    def __load_cfgs(self, save_dir: str):
-        """Load the config from the save directory.
+    def get_cost_from_obs_tensor(self, obs: torch.Tensor) -> torch.Tensor | None:
+        """Get cost from tensor observation.
 
         Args:
-            save_dir (str): directory where the model is saved.
+            obs (torch.Tensor): The observation.
         """
-        cfg_path = os.path.join(save_dir, 'config.json')
-        try:
-            with open(cfg_path, encoding='utf-8') as file:
-                kwargs = json.load(file)
-        except FileNotFoundError as error:
-            raise FileNotFoundError(
-                f'The config file is not found in the save directory{save_dir}.',
-            ) from error
-        self._cfgs = Config.dict2config(kwargs)
+        return (
+            self._env.get_cost_from_obs_tensor(obs)
+            if hasattr(self._env, 'get_cost_from_obs_tensor')
+            else None
+        )
 
-    def __load_model_and_env(self, save_dir: str, model_name: str, env_kwargs: dict[str, Any]):
-        """Load the model from the save directory.
+    def get_lidar_from_coordinate(self, obs: torch.Tensor) -> torch.Tensor | None:
+        """Get lidar from numpy coordinate.
 
         Args:
-            save_dir (str): directory where the model is saved.
-            model_name (str): name of the model.
+            obs (np.ndarray): The observation.
         """
-        # load the saved model
-        model_path = os.path.join(save_dir, 'torch_save', model_name)
-        try:
-            model_params = torch.load(model_path)
-        except FileNotFoundError as error:
-            raise FileNotFoundError('The model is not found in the save directory.') from error
-
-        # load the environment
-        self._env = make(**env_kwargs)
-
-        observation_space = self._env.observation_space
-        action_space = self._env.action_space
-
-        assert isinstance(observation_space, Box), 'The observation space must be Box.'
-        assert isinstance(action_space, Box), 'The action space must be Box.'
-
-        if self._cfgs['algo_cfgs']['obs_normalize']:
-            obs_normalizer = Normalizer(shape=observation_space.shape, clip=5)
-            obs_normalizer.load_state_dict(model_params['obs_normalizer'])
-            self._env = ObsNormalize(self._env, device='cpu', norm=obs_normalizer)
-        if self._env.need_time_limit_wrapper:
-            self._env = TimeLimit(self._env, device='cpu', time_limit=1000)
-        self._env = ActionScale(self._env, device='cpu', low=-1.0, high=1.0)
-
-        actor_type = self._cfgs['model_cfgs']['actor_type']
-        pi_cfg = self._cfgs['model_cfgs']['actor']
-        weight_initialization_mode = self._cfgs['model_cfgs']['weight_initialization_mode']
-        actor_builder = ActorBuilder(
-            obs_space=observation_space,
-            act_space=action_space,
-            hidden_sizes=pi_cfg['hidden_sizes'],
-            activation=pi_cfg['activation'],
-            weight_initialization_mode=weight_initialization_mode,
+        return (
+            self._env.get_lidar_from_coordinate(obs)
+            if hasattr(self._env, 'get_lidar_from_coordinate')
+            else None
         )
-        self._actor = actor_builder.build_actor(actor_type)
-        self._actor.load_state_dict(model_params['pi'])
 
-    # pylint: disable-next=too-many-locals
-    def load_saved(
+    def render(self, *args: str, **kwargs: int) -> Any:
+        """Render the environment.
+
+        Args:
+            args (str): The arguments.
+            kwargs (int): The keyword arguments.
+        """
+        return self._env.render(*args, **kwargs)
+
+    def _wrapper(
         self,
-        save_dir: str,
-        model_name: str,
-        render_mode: str | None = None,
-        camera_name: str | None = None,
-        camera_id: int | None = None,
-        width: int = 256,
-        height: int = 256,
-    ):
-        """Load a saved model.
+        obs_normalize: bool = True,
+        reward_normalize: bool = True,
+        cost_normalize: bool = True,
+        action_repeat: int = 1,
+    ) -> None:
+        """Wrapper the environment.
+
+        .. hint::
+
+            OmniSafe supports the following wrappers:
+
+            .. list-table::
+
+                *   -   Wrapper
+                    -   Description
+                *   -   TimeLimit
+                    -   Limit the time steps of the environment.
+                *   -   AutoReset
+                    -   Reset the environment when the episode is done.
+                *   -   ObsNormalize
+                    -   Normalize the observation.
+                *   -   RewardNormalize
+                    -   Normalize the reward.
+                *   -   CostNormalize
+                    -   Normalize the cost.
+                *   -   ActionScale
+                    -   Scale the action.
+                *   -   ActionRepeat
+                    -   Repeat the action.
+                *   -   Unsqueeze
+                    -   Unsqueeze the step result for single environment case.
 
         Args:
-            save_dir (str): directory where the model is saved.
-            model_name (str): name of the model.
+            obs_normalize (bool): Whether to normalize the observation.
+            reward_normalize (bool): Whether to normalize the reward.
+            cost_normalize (bool): Whether to normalize the cost.
+            action_repeat (int): The action repeat times.
         """
-        # load the config
-        self._save_dir = save_dir
-        self._model_name = model_name
-
-        self.__load_cfgs(save_dir)
-
-        if render_mode is not None or self._render_mode is None:
-            self.__set_render_mode(render_mode)
-
-        env_kwargs = {
-            'env_id': self._cfgs['env_id'],
-            'num_envs': 1,
-            'render_mode': self._render_mode,
-            'camera_id': camera_id,
-            'camera_name': camera_name,
-            'width': width,
-            'height': height,
-        }
+        if self._env.need_time_limit_wrapper:
+            self._env = TimeLimit(self._env, device=self._device, time_limit=1000)
+        if self._env.need_auto_reset_wrapper:
+            self._env = AutoReset(self._env, device=self._device)
+        if obs_normalize:
+            self._env = ObsNormalize(self._env, device=self._device)
+        if reward_normalize:
+            self._env = RewardNormalize(self._env, device=self._device)
+        if cost_normalize:
+            self._env = CostNormalize(self._env, device=self._device)
+        self._env = ActionScale(self._env, device=self._device, low=-1.0, high=1.0)
+        self._env = ActionRepeat(self._env, times=action_repeat, device=self._device)
 
-        self.__load_model_and_env(save_dir, model_name, env_kwargs)
+        if self._env.num_envs == 1:
+            self._env = Unsqueeze(self._env, device=self._device)
 
-    def evaluate(
+    def roll_out(  # pylint: disable=too-many-arguments,too-many-locals
         self,
-        num_episodes: int = 10,
-        cost_criteria: float = 1.0,
-    ):
-        """Evaluate the agent for num_episodes episodes.
+        current_step: int,
+        roll_out_step: int,
+        use_actor_critic: bool,
+        act_func: Callable,
+        store_data_func: Callable,
+        update_dynamics_func: Callable,
+        logger: Logger,
+        use_eval: bool,
+        eval_func: Callable,
+        algo_reset_func: Callable,
+        update_actor_func: Callable,
+    ) -> int:
+        """Roll out the environment and store the data in the buffer.
 
         Args:
-            num_episodes (int): number of episodes to evaluate the agent.
-            cost_criteria (float): the cost criteria for the evaluation.
-
-        Returns:
-            (float, float, float): the average return, the average cost, and the average length of the episodes.
+            current_step (int): Current training step.
+            roll_out_step (int): Number of steps to roll out.
+            use_actor_critic (bool): Whether to use actor-critic.
+            act_func (Callable): Function to get action.
+            store_data_func (Callable): Function to store data.
+            update_dynamics_func (Callable): Function to update dynamics.
+            logger (Logger): Logger.
+            use_eval (bool): Whether to use evaluation.
+            eval_func (Callable): Function to evaluate the agent.
+            algo_reset_func (Callable): Function to reset the algorithm.
+            update_actor_func (Callable): Function to update the actor.
         """
-        if self._env is None or self._actor is None:
-            raise ValueError(
-                'The environment and the policy must be provided or created before evaluating the agent.',
+        epoch_start_time = time.time()
+
+        update_actor_critic_time = 0.0
+        update_dynamics_time = 0.0
+        if use_eval:
+            eval_time = 0.0
+
+        epoch_steps = 0
+
+        while epoch_steps < roll_out_step and current_step < self._cfgs.train_cfgs.total_steps:
+            action, action_info = act_func(current_step, self._current_obs, self._env)
+            next_state, reward, cost, terminated, truncated, info = self.step(action)
+            epoch_steps += info['num_step']
+            current_step += info['num_step']
+            self._log_value(reward=reward, cost=cost, info=info)
+
+            store_data_func(
+                current_step,
+                self._ep_len,
+                self._current_obs,
+                action,
+                reward,
+                cost,
+                terminated,
+                truncated,
+                next_state,
+                info,
+                action_info,
             )
+            self._current_obs = next_state
+            if terminated or truncated:
+                self._log_metrics(logger)
+                self._reset_log()
+                self._current_obs, _ = self.reset()
+                if algo_reset_func is not None:
+                    algo_reset_func(current_step)
+            if (
+                current_step % self._cfgs.algo_cfgs.update_dynamics_cycle
+                < self._cfgs.algo_cfgs.action_repeat
+                and current_step - self._last_dynamics_update
+                >= self._cfgs.algo_cfgs.update_dynamics_cycle
+            ):
+                update_dynamics_start = time.time()
+                update_dynamics_func(current_step)
+                self._last_dynamics_update = current_step
+                update_dynamics_time += time.time() - update_dynamics_start
+
+            if (
+                use_actor_critic
+                and current_step % self._cfgs.algo_cfgs.update_policy_cycle
+                < self._cfgs.algo_cfgs.action_repeat
+                and current_step - self._last_policy_update
+                >= self._cfgs.algo_cfgs.update_policy_cycle
+            ):
+                update_actor_critic_start = time.time()
+                update_actor_func(current_step)
+                self._last_policy_update = current_step
+                update_actor_critic_time += time.time() - update_actor_critic_start
+
+            if (
+                use_eval
+                and current_step % self._cfgs.evaluation_cfgs.eval_cycle
+                < self._cfgs.algo_cfgs.action_repeat
+                and current_step - self._last_eval >= self._cfgs.evaluation_cfgs.eval_cycle
+            ):
+                eval_start = time.time()
+                eval_func(current_step)
+                self._last_eval = current_step
+                eval_time += time.time() - eval_start
+
+        if not self._first_log or current_step >= self._cfgs.train_cfgs.total_steps:
+            self._log_metrics(logger)
+
+        epoch_time = time.time() - epoch_start_time
+        logger.store(**{'Time/Epoch': epoch_time})
+        logger.store(**{'Time/UpdateDynamics': update_dynamics_time})
+        roll_out_time = epoch_time - update_dynamics_time
+
+        if use_eval:
+            logger.store(**{'Time/Eval': eval_time})
+            roll_out_time -= eval_time
+
+        if use_actor_critic:
+            logger.store(**{'Time/UpdateActorCritic': update_actor_critic_time})
+            roll_out_time -= update_actor_critic_time
+        logger.store(**{'Time/Rollout': roll_out_time})
+        return current_step
 
-        episode_rewards: list[float] = []
-        episode_costs: list[float] = []
-        episode_lengths: list[float] = []
-
-        for episode in range(num_episodes):
-            obs, _ = self._env.reset()
-            ep_ret, ep_cost, length = 0.0, 0.0, 0.0
-
-            done = False
-            while not done:
-                with torch.no_grad():
-                    act = self._actor.predict(
-                        torch.as_tensor(obs, dtype=torch.float32),
-                        deterministic=False,
-                    )
-                obs, rew, cost, terminated, truncated, _ = self._env.step(act)
-
-                ep_ret += rew.item()
-                ep_cost += (cost_criteria**length) * cost.item()
-                length += 1
-
-                done = bool(terminated or truncated)
-
-            episode_rewards.append(ep_ret)
-            episode_costs.append(ep_cost)
-            episode_lengths.append(length)
-
-            print(f'Episode {episode+1} results:')
-            print(f'Episode reward: {ep_ret}')
-            print(f'Episode cost: {ep_cost}')
-            print(f'Episode length: {length}')
-
-        print(self._dividing_line)
-        print('Evaluation results:')
-        print(f'Average episode reward: {np.mean(episode_rewards)}')
-        print(f'Average episode cost: {np.mean(episode_costs)}')
-        print(f'Average episode length: {np.mean(episode_lengths)}')
-        return (
-            episode_rewards,
-            episode_costs,
-        )
+    def _log_value(
+        self,
+        reward: torch.Tensor,
+        cost: torch.Tensor,
+        info: dict,
+    ) -> None:
+        """Log value.
 
-    @property
-    def fps(self) -> int:
-        """The fps of the environment.
+        .. note::
+            OmniSafe uses :class:`RewardNormalizer` wrapper, so the original reward and cost will
+            be stored in ``info['original_reward']`` and ``info['original_cost']``.
 
-        Returns:
-            int: the fps.
+        Args:
+            reward (torch.Tensor): The reward.
+            cost (torch.Tensor): The cost.
+            info (dict): Information.
         """
-        try:
-            fps = self._env.metadata['render_fps']
-        except AttributeError:
-            fps = 30
-            warnings.warn('The fps is not found, use 30 as default.', stacklevel=2)
+        self._ep_ret += info.get('original_reward', reward).cpu()
+        self._ep_cost += info.get('original_cost', cost).cpu()
+        self._ep_len += info.get('num_step', 1)
 
-        return fps
-
-    def render(  # pylint: disable=too-many-locals,too-many-arguments,too-many-branches,too-many-statements
-        self,
-        num_episodes: int = 0,
-        save_replay_path: str | None = None,
-        max_render_steps: int = 2000,
-        cost_criteria: float = 1.0,
-    ):
-        """Render the environment for one episode.
+    def _log_metrics(self, logger: Logger) -> None:
+        """Log metrics.
 
         Args:
-            seed (int): seed for the environment. If None, the environment will be reset with a random seed.
-            save_replay_path (str): path to save the replay. If None, no replay is saved.
+            logger (Logger): Logger.
         """
+        self._first_log = True
+        logger.store(
+            **{
+                'Metrics/EpRet': self._ep_ret,
+                'Metrics/EpCost': self._ep_cost,
+                'Metrics/EpLen': self._ep_len,
+            },
+        )
+
+    def _reset_log(self, idx: int | None = None) -> None:  # pylint: disable=unused-argument
+        """Reset log.
 
-        if save_replay_path is None:
-            save_replay_path = os.path.join(self._save_dir, 'video', self._model_name.split('.')[0])
-        result_path = os.path.join(save_replay_path, 'result.txt')
-        print(self._dividing_line)
-        print(f'Saving the replay video to {save_replay_path},\n and the result to {result_path}.')
-        print(self._dividing_line)
-
-        horizon = 1000
-        frames = []
-        obs, _ = self._env.reset()
-        if self._render_mode == 'human':
-            self._env.render()
-        elif self._render_mode == 'rgb_array':
-            frames.append(self._env.render())
-
-        episode_rewards: list[float] = []
-        episode_costs: list[float] = []
-        episode_lengths: list[float] = []
-
-        for episode_idx in range(num_episodes):
-            step = 0
-            done = False
-            ep_ret, ep_cost, length = 0.0, 0.0, 0.0
-            while (
-                not done and step <= max_render_steps
-            ):  # a big number to make sure the episode will end
-                with torch.no_grad():
-                    act = self._actor.predict(obs, deterministic=False)
-                obs, rew, cost, terminated, truncated, _ = self._env.step(act)
-                step += 1
-                done = bool(terminated or truncated)
-                ep_ret += rew.item()
-                ep_cost += (cost_criteria**length) * cost.item()
-                length += 1
-
-                if self._render_mode == 'rgb_array':
-                    frames.append(self._env.render())
-
-            if self._render_mode == 'rgb_array_list':
-                frames = self._env.render()
-
-            if save_replay_path is not None:
-                save_video(
-                    frames,
-                    save_replay_path,
-                    fps=self.fps,
-                    episode_trigger=lambda x: True,
-                    video_length=horizon,
-                    episode_index=episode_idx,
-                    name_prefix='eval',
-                )
-            self._env.reset()
-            frames = []
-            episode_rewards.append(ep_ret)
-            episode_costs.append(ep_cost)
-            episode_lengths.append(length)
-            with open(result_path, 'a+', encoding='utf-8') as f:
-                print(f'Episode {episode_idx+1} results:', file=f)
-                print(f'Episode reward: {ep_ret}', file=f)
-                print(f'Episode cost: {ep_cost}', file=f)
-                print(f'Episode length: {length}', file=f)
-        with open(result_path, 'a+', encoding='utf-8') as f:
-            print(self._dividing_line)
-            print('Evaluation results:', file=f)
-            print(f'Average episode reward: {np.mean(episode_rewards)}', file=f)
-            print(f'Average episode cost: {np.mean(episode_costs)}', file=f)
-            print(f'Average episode length: {np.mean(episode_lengths)}', file=f)
+        Args:
+            idx (int | None): The index of the environment.
+        """
+        self._ep_ret = torch.zeros(1)
+        self._ep_cost = torch.zeros(1)
+        self._ep_len = torch.zeros(1)
```

### Comparing `omnisafe-0.3.0/omnisafe/models/__init__.py` & `omnisafe-0.4.0/omnisafe/models/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/models/actor/__init__.py` & `omnisafe-0.4.0/omnisafe/models/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/models/actor/actor_builder.py` & `omnisafe-0.4.0/omnisafe/models/actor/actor_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,65 +15,65 @@
 """Implementation of ActorBuilder."""
 
 from __future__ import annotations
 
 from omnisafe.models.actor.gaussian_learning_actor import GaussianLearningActor
 from omnisafe.models.actor.gaussian_sac_actor import GaussianSACActor
 from omnisafe.models.actor.mlp_actor import MLPActor
-from omnisafe.models.base import Actor
 from omnisafe.typing import Activation, ActorType, InitFunction, OmnisafeSpace
 
 
 # pylint: disable-next=too-few-public-methods
 class ActorBuilder:
     """Class for building actor networks.
 
-    Attributes:
-        _obs_space (OmnisafeSpace): Observation space.
-        _act_space (OmnisafeSpace): Action space.
-        _weight_initialization_mode (InitFunction): Weight initialization mode.
-        _activation (Activation): Activation function.
-        _hidden_sizes (list[int]): List of hidden layer sizes.
-
+    Args:
+        obs_space (OmnisafeSpace): Observation space.
+        act_space (OmnisafeSpace): Action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
     """
 
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
     ) -> None:
-        """Initialize ActorBuilder.
-
-        Args:
-            obs_space (OmnisafeSpace): Observation space.
-            act_space (OmnisafeSpace): Action space.
-            hidden_sizes (list): List of hidden layer sizes.
-            activation (Activation): Activation function.
-            weight_initialization_mode (InitFunction): Weight initialization mode.
-        """
-        self._obs_space = obs_space
-        self._act_space = act_space
-        self._weight_initialization_mode = weight_initialization_mode
-        self._activation = activation
-        self._hidden_sizes = hidden_sizes
+        """Initialize an instance of :class:`ActorBuilder`."""
+        self._obs_space: OmnisafeSpace = obs_space
+        self._act_space: OmnisafeSpace = act_space
+        self._weight_initialization_mode: InitFunction = weight_initialization_mode
+        self._activation: Activation = activation
+        self._hidden_sizes: list[int] = hidden_sizes
 
     # pylint: disable-next=too-many-return-statements
-    def build_actor(self, actor_type: ActorType) -> Actor:
+    def build_actor(
+        self,
+        actor_type: ActorType,
+    ) -> GaussianLearningActor | GaussianSACActor | MLPActor:
         """Build actor network.
 
         Currently, we support the following actor types:
             - ``gaussian_learning``: Gaussian actor with learnable standard deviation parameters.
             - ``gaussian_sac``: Gaussian actor with learnable standard deviation network.
             - ``mlp``: Multi-layer perceptron actor, used in ``DDPG`` and ``TD3``.
 
         Args:
-            actor_type (ActorType): Actor type.
+            actor_type (ActorType): Type of actor network, e.g. ``gaussian_learning``.
+
+        Returns:
+            Actor network, ranging from ``GaussianLearningActor``, ``GaussianSACActor`` to ``MLPActor``.
+
+        Raises:
+            NotImplementedError: If the actor type is not implemented.
         """
         if actor_type == 'gaussian_learning':
             return GaussianLearningActor(
                 self._obs_space,
                 self._act_space,
                 self._hidden_sizes,
                 activation=self._activation,
```

### Comparing `omnisafe-0.3.0/omnisafe/models/actor/gaussian_actor.py` & `omnisafe-0.4.0/omnisafe/models/actor/gaussian_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 
 from abc import ABC, abstractmethod
 
 from omnisafe.models.base import Actor
 
 
 class GaussianActor(Actor, ABC):
-    """A abstract class for normal distribution actor.
+    """An abstract class for normal distribution actor.
 
-    A NormalActor inherits from Actor and use Normal distribution to approximate
-    the policy function.
+    A NormalActor inherits from Actor and use Normal distribution to approximate the policy function.
 
     .. note::
         You can use this class to implement your own actor by inheriting it.
     """
 
     @property
     @abstractmethod
```

### Comparing `omnisafe-0.3.0/omnisafe/models/actor/gaussian_learning_actor.py` & `omnisafe-0.4.0/omnisafe/models/actor/mlp_actor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,126 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of GaussianStdNetActor."""
+"""Implementation of MLPActorActor."""
 
 from __future__ import annotations
 
 import torch
-import torch.nn as nn
-from torch.distributions import Distribution, Normal
+from torch.distributions import Distribution
 
-from omnisafe.models.actor.gaussian_actor import GaussianActor
+from omnisafe.models.base import Actor
 from omnisafe.typing import Activation, InitFunction, OmnisafeSpace
 from omnisafe.utils.model import build_mlp_network
 
 
 # pylint: disable-next=too-many-instance-attributes
-class GaussianLearningActor(GaussianActor):
-    """Implementation of GaussianLearningActor."""
+class MLPActor(Actor):
+    """Implementation of MLPActor.
+
+    MLPActor is a Gaussian actor with a learnable mean value. It is used in off-policy algorithms
+    such as ``DDPG``, ``TD3`` and so on.
+
+    Args:
+        obs_space (OmnisafeSpace): Observation space.
+        act_space (OmnisafeSpace): Action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        output_activation (Activation, optional): Output activation function. Defaults to ``'tanh'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+    """
 
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
+        output_activation: Activation = 'tanh',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
     ) -> None:
-        """Initialize GaussianLearningActor.
-
-        GaussianLearningActor is a Gaussian actor with a learnable standard deviation.
-        It is used in on-policy algorithms such as ``PPO``, ``TRPO`` and so on.
-
-        Args:
-            obs_space (OmnisafeSpace): Observation space.
-            act_space (OmnisafeSpace): Action space.
-            hidden_sizes (list): List of hidden layer sizes.
-            activation (Activation): Activation function.
-            weight_initialization_mode (InitFunction): Weight initialization mode.
-            shared (nn.Module): Shared module.
-        """
+        """Initialize an instance of :class:`MLPActor`."""
         super().__init__(obs_space, act_space, hidden_sizes, activation, weight_initialization_mode)
-        self.mean = build_mlp_network(
+
+        self.net: torch.nn.Module = build_mlp_network(
             sizes=[self._obs_dim, *self._hidden_sizes, self._act_dim],
             activation=activation,
+            output_activation=output_activation,
             weight_initialization_mode=weight_initialization_mode,
         )
-        self.log_std = nn.Parameter(torch.zeros(self._act_dim), requires_grad=True)
-
-    def _distribution(self, obs: torch.Tensor) -> Distribution:
-        """Get the distribution of the actor.
-
-        .. warning::
-            This method is not supposed to be called by users.
-            You should call :meth:`forward` instead.
-
-        Args:
-            obs (torch.Tensor): Observation.
-        """
-        mean = self.mean(obs)
-        std = torch.exp(self.log_std)
-        return Normal(mean, std)
+        self._noise: float = 0.1
 
-    def predict(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
+    def predict(
+        self,
+        obs: torch.Tensor,
+        deterministic: bool = True,
+    ) -> torch.Tensor:
         """Predict the action given observation.
 
         The predicted action depends on the ``deterministic`` flag.
 
         - If ``deterministic`` is ``True``, the predicted action is the mean of the distribution.
         - If ``deterministic`` is ``False``, the predicted action is sampled from the distribution.
 
         Args:
-            obs (torch.Tensor): Observation.
-            deterministic (bool): Whether to use deterministic policy.
+            obs (torch.Tensor): Observation from environments.
+            deterministic (bool, optional): Whether to use deterministic policy. Defaults to True.
         """
-        self._current_dist = self._distribution(obs)
-        self._after_inference = True
+        action = self.net(obs)
         if deterministic:
-            return self._current_dist.mean
-        return self._current_dist.rsample()
+            return action
+        with torch.no_grad():
+            noise = torch.normal(0, self._noise * torch.ones_like(action))
+            return torch.clamp(action + noise, -1, 1)
+
+    @property
+    def noise(self) -> float:
+        """Noise of the action."""
+        return self._noise
+
+    @noise.setter
+    def noise(self, noise: float) -> None:
+        """Set the action noise."""
+        assert noise >= 0, 'Noise should be non-negative.'
+        self._noise = noise
+
+    def _distribution(self, obs: torch.Tensor) -> Distribution:
+        raise NotImplementedError
 
     def forward(self, obs: torch.Tensor) -> Distribution:
-        """Forward method.
+        """Forward method implementation.
 
         Args:
-            obs (torch.Tensor): Observation.
+            obs (torch.Tensor): Observation from environments.
+
+        Returns:
+            The distribution of the action.
         """
-        self._current_dist = self._distribution(obs)
-        self._after_inference = True
-        return self._current_dist
+        return self._distribution(obs)
 
     def log_prob(self, act: torch.Tensor) -> torch.Tensor:
-        """Compute the log probability of the action given the current distribution.
-
-        .. warning::
-            You must call :meth:`forward` or :meth:`predict` before calling this method.
+        """Log probability of the action.
 
         Args:
-            act (torch.Tensor): Action.
+            act (torch.Tensor): Action tensor.
+
+        Raises:
+            NotImplementedError: The method is not implemented.
         """
-        assert self._after_inference, 'log_prob() should be called after predict() or forward()'
-        self._after_inference = False
-        return self._current_dist.log_prob(act).sum(axis=-1)
+        raise NotImplementedError
 
     @property
     def std(self) -> float:
-        """Get the standard deviation of the distribution."""
-        return torch.exp(self.log_std).mean().item()
-
-    @std.setter
-    def std(self, std: float) -> None:
-        """Set the standard deviation of the distribution.
-
-        .. hint::
-            This method is only used for annealing the standard deviation.
-            It can be called.
-
-        Args:
-            std (float): Standard deviation.
-        """
-        device = self.log_std.device
-        self.log_std.data.fill_(torch.log(torch.tensor(std, device=device)))
+        """Standard deviation of the distribution."""
+        return self._noise
```

### Comparing `omnisafe-0.3.0/omnisafe/models/actor/gaussian_sac_actor.py` & `omnisafe-0.4.0/omnisafe/models/actor/gaussian_sac_actor.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,69 +14,74 @@
 # ==============================================================================
 """Implementation of GaussianStdNetActor."""
 
 from __future__ import annotations
 
 import torch
 from torch import nn
-from torch.distributions import Distribution, Normal
+from torch.distributions import Normal
 
 from omnisafe.models.base import Actor
 from omnisafe.typing import Activation, InitFunction, OmnisafeSpace
 from omnisafe.utils.math import TanhNormal
 from omnisafe.utils.model import build_mlp_network
 
 
 class GaussianSACActor(Actor):
-    """Implementation of GaussianSACActor."""
+    """Implementation of GaussianSACActor.
+
+    GaussianSACActor is a Gaussian actor with a learnable standard deviation network.
+    It is used in ``SAC``, and other off-line or model-based algorithms related to ``SAC``.
+
+    Args:
+        obs_space (OmnisafeSpace): Observation space.
+        act_space (OmnisafeSpace): Action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+    """
+
+    _log2: torch.Tensor
+    _current_dist: Normal
 
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
     ) -> None:
-        """Initialize GaussianSACActor.
-
-        GaussianSACActor is a Gaussian actor with a learnable standard deviation network.
-        It is used in ``SAC``, and other off-line or model-based algorithms related to ``SAC``.
-
-        Args:
-            obs_space (OmnisafeSpace): Observation space.
-            act_space (OmnisafeSpace): Action space.
-            hidden_sizes (list): List of hidden layer sizes.
-            activation (Activation): Activation function.
-            weight_initialization_mode (InitFunction): Weight initialization mode.
-            shared (nn.Module): Shared module.
-        """
+        """Initialize an instance of :class:`GaussianSACActor`."""
         super().__init__(obs_space, act_space, hidden_sizes, activation, weight_initialization_mode)
-        self.net = build_mlp_network(
+
+        self.net: nn.Module = build_mlp_network(
             sizes=[self._obs_dim, *self._hidden_sizes, self._act_dim * 2],
             activation=activation,
             weight_initialization_mode=weight_initialization_mode,
         )
 
         self._current_raw_action: torch.Tensor | None = None
         self.register_buffer('_log2', torch.log(torch.tensor(2.0)))
-        self._log2: torch.Tensor
 
-    def _distribution(self, obs: torch.Tensor) -> Distribution:
+    def _distribution(self, obs: torch.Tensor) -> Normal:
         """Get the distribution of the actor.
 
         .. warning::
-
-            This method is not supposed to be called by users.
-            You should call :meth:`forward` instead.
+            This method is not supposed to be called by users. You should call :meth:`forward`
+            instead.
 
         **Specifically, this method will clip the standard deviation to a range of [-20, 2].**
 
         Args:
-            obs (torch.Tensor): Observation.
+            obs (torch.Tensor): Observation from environments.
+
+        Returns:
+            The normal distribution of the mean and standard deviation from the actor.
         """
         mean, log_std = self.net(obs).chunk(2, dim=-1)
         log_std = torch.clamp(log_std, min=-20, max=2)
         std = log_std.exp()
         return Normal(mean, std)
 
     def predict(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
@@ -84,55 +89,65 @@
 
         The predicted action depends on the ``deterministic`` flag.
 
         - If ``deterministic`` is ``True``, the predicted action is the mean of the distribution.
         - If ``deterministic`` is ``False``, the predicted action is sampled from the distribution.
 
         Args:
-            obs (torch.Tensor): Observation.
-            deterministic (bool): Whether to use deterministic policy.
+            obs (torch.Tensor): Observation from environments.
+            deterministic (bool, optional): Whether to use deterministic policy. Defaults to False.
+
+        Returns:
+            The mean of the distribution if ``deterministic`` is ``True``, otherwise the sampled
+            action.
         """
         self._current_dist = self._distribution(obs)
         self._after_inference = True
 
         action = self._current_dist.mean if deterministic else self._current_dist.rsample()
 
         self._current_raw_action = action
 
         return torch.tanh(action)
 
-    def forward(self, obs: torch.Tensor) -> Distribution:
+    def forward(self, obs: torch.Tensor) -> TanhNormal:
         """Forward method.
 
         Args:
-            obs (torch.Tensor): Observation.
+            obs (torch.Tensor): Observation from environments.
+
+        Returns:
+            The current distribution.
         """
         self._current_dist = self._distribution(obs)
         self._after_inference = True
         return TanhNormal(self._current_dist.mean, self._current_dist.stddev)
 
     def log_prob(self, act: torch.Tensor) -> torch.Tensor:
         r"""Compute the log probability of the action given the current distribution.
 
         .. warning::
             You must call :meth:`forward` or :meth:`predict` before calling this method.
 
         .. note::
-
-            In this method, we will regularize the log probability of the action.
-            The regularization is as follows:
+            In this method, we will regularize the log probability of the action. The regularization
+            is as follows:
 
             .. math::
 
-                \log \pi(a|s) = \log \pi(a|s) - \sum_{i=1}^n (2 \log 2 - a_i - \log (1 + e^{-2 a_i}))
+                \log \pi (a|s) = \log \pi (a|s) - \sum_{i=1}^n (2 \log 2 - a_i - \log (1 + e^{-2 a_i}))
 
-            where :math:`a` is the action, :math:`s` is the observation, and :math:`n` is the dimension of the action.
+            where :math:`a` is the action, :math:`s` is the observation, and :math:`n` is the
+            dimension of the action.
 
         Args:
             act (torch.Tensor): Action.
+
+        Returns:
+            Log probability of the action.
         """
         assert self._after_inference, 'log_prob() should be called after predict() or forward()'
         self._after_inference = False
 
         if self._current_raw_action is not None:
             logp = self._current_dist.log_prob(self._current_raw_action).sum(axis=-1)
             logp -= (
@@ -151,13 +166,13 @@
                 .sum(axis=-1)
             )
 
         return logp
 
     @property
     def std(self) -> float:
-        """Get the standard deviation of the normal distribution."""
+        """Standard deviation of the distribution."""
         return self._current_dist.stddev.mean().item()
 
     @std.setter
     def std(self, std: float) -> None:
         raise NotImplementedError('GaussianStdNetActor does not support setting std.')
```

### Comparing `omnisafe-0.3.0/omnisafe/models/actor/mlp_actor.py` & `omnisafe-0.4.0/omnisafe/models/actor/gaussian_learning_actor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,140 @@
-# Copyright 2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of MLPActorActor."""
+"""Implementation of GaussianLearningActor."""
 
 from __future__ import annotations
 
 import torch
-from torch.distributions import Distribution
+import torch.nn as nn
+from torch.distributions import Distribution, Normal
 
-from omnisafe.models.base import Actor
+from omnisafe.models.actor.gaussian_actor import GaussianActor
 from omnisafe.typing import Activation, InitFunction, OmnisafeSpace
 from omnisafe.utils.model import build_mlp_network
 
 
 # pylint: disable-next=too-many-instance-attributes
-class MLPActor(Actor):
-    """Implementation of MLPActor."""
+class GaussianLearningActor(GaussianActor):
+    """Implementation of GaussianLearningActor.
+
+    GaussianLearningActor is a Gaussian actor with a learnable standard deviation. It is used in
+    on-policy algorithms such as ``PPO``, ``TRPO`` and so on.
+
+    Args:
+        obs_space (OmnisafeSpace): Observation space.
+        act_space (OmnisafeSpace): Action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+    """
+
+    _current_dist: Normal
 
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
-        output_activation: Activation = 'identity',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
     ) -> None:
-        """Initialize MLPActor.
-
-        Args:
-            obs_space (OmnisafeSpace): Observation space.
-            act_space (OmnisafeSpace): Action space.
-            hidden_sizes (list): List of hidden layer sizes.
-            activation (Activation): Activation function.
-            output_activation (Activation): Output activation function.
-            weight_initialization_mode (InitFunction): Weight initialization mode.
-        """
+        """Initialize an instance of :class:`GaussianLearningActor`."""
         super().__init__(obs_space, act_space, hidden_sizes, activation, weight_initialization_mode)
-        self.net = build_mlp_network(
+
+        self.mean: nn.Module = build_mlp_network(
             sizes=[self._obs_dim, *self._hidden_sizes, self._act_dim],
             activation=activation,
-            output_activation=output_activation,
             weight_initialization_mode=weight_initialization_mode,
         )
-        self._noise = 0.2
-        self._noise_clip = 100
-        self.register_buffer('_act_min', torch.tensor(self._act_space.low, dtype=torch.float32))
-        self.register_buffer('_act_max', torch.tensor(self._act_space.high, dtype=torch.float32))
+        self.log_std: nn.Parameter = nn.Parameter(torch.zeros(self._act_dim), requires_grad=True)
 
-    def predict(
-        self,
-        obs: torch.Tensor,
-        deterministic: bool = True,
-    ) -> torch.Tensor:
+    def _distribution(self, obs: torch.Tensor) -> Normal:
+        """Get the distribution of the actor.
+
+        .. warning::
+            This method is not supposed to be called by users. You should call :meth:`forward`
+            instead.
+
+        Args:
+            obs (torch.Tensor): Observation from environments.
+
+        Returns:
+            The normal distribution of the mean and standard deviation from the actor.
+        """
+        mean = self.mean(obs)
+        std = torch.exp(self.log_std)
+        return Normal(mean, std)
+
+    def predict(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
         """Predict the action given observation.
 
         The predicted action depends on the ``deterministic`` flag.
 
         - If ``deterministic`` is ``True``, the predicted action is the mean of the distribution.
         - If ``deterministic`` is ``False``, the predicted action is sampled from the distribution.
 
         Args:
-            obs (torch.Tensor): Observation.
-            deterministic (bool): Whether to use deterministic policy.
+            obs (torch.Tensor): Observation from environments.
+            deterministic (bool, optional): Whether to use deterministic policy. Defaults to False.
+
+        Returns:
+            The mean of the distribution if ``deterministic`` is ``True``, otherwise the sampled
+            action.
         """
-        action = torch.tanh(self.net(obs))
+        self._current_dist = self._distribution(obs)
+        self._after_inference = True
         if deterministic:
-            return action
+            return self._current_dist.mean
+        return self._current_dist.rsample()
 
-        noise = torch.normal(0, self._noise * torch.ones_like(action))
-        noise = torch.clamp(noise, -self._noise_clip, self._noise_clip)
-        return torch.clamp(action + noise, self._act_min, self._act_max)
+    def forward(self, obs: torch.Tensor) -> Distribution:
+        """Forward method.
 
-    @property
-    def noise(self) -> float:
-        """Get the action noise."""
-        return self._noise
-
-    @noise.setter
-    def noise(self, noise: float) -> None:
-        """Set the action noise."""
-        assert noise >= 0, 'Noise should be non-negative.'
-        self._noise = noise
+        Args:
+            obs (torch.Tensor): Observation from environments.
 
-    @property
-    def noise_clip(self) -> float:
-        """Get the action noise bound."""
-        return self._noise_clip
-
-    @noise_clip.setter
-    def noise_clip(self, noise_clip: float) -> None:
-        assert noise_clip >= 0, 'Noise clip should be non-negative.'
-        self._noise_clip = noise_clip
+        Returns:
+            The current distribution.
+        """
+        self._current_dist = self._distribution(obs)
+        self._after_inference = True
+        return self._current_dist
+
+    def log_prob(self, act: torch.Tensor) -> torch.Tensor:
+        """Compute the log probability of the action given the current distribution.
 
-    def _distribution(self, obs: torch.Tensor) -> Distribution:
-        raise NotImplementedError
+        .. warning::
+            You must call :meth:`forward` or :meth:`predict` before calling this method.
 
-    def forward(self, obs: torch.Tensor) -> Distribution:
-        raise NotImplementedError
+        Args:
+            act (torch.Tensor): Action.
 
-    def log_prob(self, act: torch.Tensor) -> torch.Tensor:
-        raise NotImplementedError
+        Returns:
+            Log probability of the action.
+        """
+        assert self._after_inference, 'log_prob() should be called after predict() or forward()'
+        self._after_inference = False
+        return self._current_dist.log_prob(act).sum(axis=-1)
+
+    @property
+    def std(self) -> float:
+        """Standard deviation of the distribution."""
+        return torch.exp(self.log_std).mean().item()
+
+    @std.setter
+    def std(self, std: float) -> None:
+        device = self.log_std.device
+        self.log_std.data.fill_(torch.log(torch.tensor(std, device=device)))
```

### Comparing `omnisafe-0.3.0/omnisafe/models/actor_critic/__init__.py` & `omnisafe-0.4.0/omnisafe/models/actor_critic/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/omnisafe/models/actor_critic/actor_critic.py` & `omnisafe-0.4.0/omnisafe/models/actor_critic/actor_critic.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,90 +14,92 @@
 # ==============================================================================
 """Implementation of ActorCritic."""
 
 from __future__ import annotations
 
 import torch
 from torch import nn, optim
-from torch.optim.lr_scheduler import ConstantLR, LinearLR, _LRScheduler
+from torch.optim.lr_scheduler import ConstantLR, LinearLR
 
+from omnisafe.models.actor import GaussianLearningActor, GaussianSACActor, MLPActor
 from omnisafe.models.actor.actor_builder import ActorBuilder
-from omnisafe.models.actor.gaussian_learning_actor import GaussianLearningActor
+from omnisafe.models.base import Critic
 from omnisafe.models.critic.critic_builder import CriticBuilder
 from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils.config import ModelConfig
 from omnisafe.utils.schedule import PiecewiseSchedule, Schedule
 
 
 class ActorCritic(nn.Module):
     """Class for ActorCritic.
 
-    In ``omnisafe``, we combine the actor and critic into one this class.
+    In OmniSafe, we combine the actor and critic into one this class.
 
-    .. list-table::
-
-        *   -   Model
-            -   Description
-            -   Function
-        *   -   Actor
-            -   The policy network, input is observation, output is action.
-                Choose the actor from the following options:
-                :class:`MLPActor`, :class:`GaussianSACActor`,
-                :class:`GaussianLearningActor`.
-            -   Choose the action based on the observation.
-        *   -   Value Critic
-            -   The value network, input is observation, output is reward value.
-                Choose the critic from the following options:
-                :class:`QCritic`, :class:`VCritic`.
-            -   Estimate the reward value of the observation.
+    +-----------------+-----------------------------------------------+
+    | Model           | Description                                   |
+    +=================+===============================================+
+    | Actor           | Input is observation. Output is action.       |
+    +-----------------+-----------------------------------------------+
+    | Reward V Critic | Input is observation. Output is reward value. |
+    +-----------------+-----------------------------------------------+
+
+    Args:
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        model_cfgs (ModelConfig): The model configurations.
+        epochs (int): The number of epochs.
 
     Attributes:
         actor (Actor): The actor network.
         reward_critic (Critic): The critic network.
         std_schedule (Schedule): The schedule for the standard deviation of the Gaussian distribution.
     """
 
+    std_schedule: Schedule
+
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         model_cfgs: ModelConfig,
         epochs: int,
     ) -> None:
-        """Initialize ActorCritic."""
+        """Initialize an instance of :class:`ActorCritic`."""
         super().__init__()
-        self.actor = ActorBuilder(
+
+        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor = ActorBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.actor.hidden_sizes,
             activation=model_cfgs.actor.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
         ).build_actor(actor_type=model_cfgs.actor_type)
-        self.reward_critic = CriticBuilder(
+        self.reward_critic: Critic = CriticBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.critic.hidden_sizes,
             activation=model_cfgs.critic.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
             num_critics=1,
             use_obs_encoder=False,
         ).build_critic(critic_type='v')
         self.add_module('actor', self.actor)
         self.add_module('reward_critic', self.reward_critic)
 
-        if model_cfgs.actor.lr != 'None':
+        if model_cfgs.actor.lr is not None:
+            self.actor_optimizer: optim.Optimizer
             self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=model_cfgs.actor.lr)
-        if model_cfgs.critic.lr != 'None':
-            self.reward_critic_optimizer = optim.Adam(
+        if model_cfgs.critic.lr is not None:
+            self.reward_critic_optimizer: optim.Optimizer = optim.Adam(
                 self.reward_critic.parameters(),
                 lr=model_cfgs.critic.lr,
             )
-        if model_cfgs.actor.lr != 'None':
-            self.actor_scheduler: _LRScheduler
+        if model_cfgs.actor.lr is not None:
+            self.actor_scheduler: LinearLR | ConstantLR
             if model_cfgs.linear_lr_decay:
                 self.actor_scheduler = LinearLR(
                     self.actor_optimizer,
                     start_factor=1.0,
                     end_factor=0.0,
                     total_iters=epochs,
                     verbose=True,
@@ -106,63 +108,76 @@
                 self.actor_scheduler = ConstantLR(
                     self.actor_optimizer,
                     factor=1.0,
                     total_iters=epochs,
                     verbose=True,
                 )
 
-            self.std_schedule: Schedule
-
-    def step(self, obs: torch.Tensor, deterministic: bool = False) -> tuple[torch.Tensor, ...]:
+    def step(
+        self,
+        obs: torch.Tensor,
+        deterministic: bool = False,
+    ) -> tuple[torch.Tensor, ...]:
         """Choose the action based on the observation. used in rollout without gradient.
 
         Args:
-            obs: The observation.
-            deterministic: Whether to use deterministic action. default: False.
+            obs (torch.tensor): The observation.
+            deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
-            The action, value_r, and log_prob.
+            action: The deterministic action if ``deterministic`` is True, otherwise the action with
+                Gaussian noise.
+            value_r: The reward value of the observation.
+            log_prob: The log probability of the action.
         """
         with torch.no_grad():
             value_r = self.reward_critic(obs)
             act = self.actor.predict(obs, deterministic=deterministic)
             log_prob = self.actor.log_prob(act)
         return act, value_r[0], log_prob
 
-    def forward(self, obs: torch.Tensor, deterministic: bool = False) -> tuple[torch.Tensor, ...]:
+    def forward(
+        self,
+        obs: torch.Tensor,
+        deterministic: bool = False,
+    ) -> tuple[torch.Tensor, ...]:
         """Choose the action based on the observation. used in training with gradient.
 
         Args:
-            obs: The observation.
-            deterministic: Whether to use deterministic action. default: False.
+            obs (torch.tensor): The observation.
+            deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
-            The action, value_r, and log_prob.
+            action: The deterministic action if ``deterministic`` is True, otherwise the action with
+                Gaussian noise.
+            value_r: The reward value of the observation.
+            log_prob: The log probability of the action.
         """
         return self.step(obs, deterministic=deterministic)
 
-    def set_annealing(self, epochs: list[float], std: list[float]) -> None:
+    def set_annealing(self, epochs: list[int], std: list[float]) -> None:
         """Set the annealing mode for the actor.
 
         Args:
-            annealing: Whether to use annealing mode.
+            epochs (list of int): The list of epochs.
+            std (list of float): The list of standard deviation.
         """
         assert isinstance(
             self.actor,
             GaussianLearningActor,
         ), 'Only GaussianLearningActor support annealing.'
         self.std_schedule = PiecewiseSchedule(
             endpoints=list(zip(epochs, std)),
             outside_value=std[-1],
         )
 
     def annealing(self, epoch: int) -> None:
         """Set the annealing mode for the actor.
 
         Args:
-            epoch: The current epoch.
+            epoch (int): The current epoch.
         """
         assert isinstance(
             self.actor,
             GaussianLearningActor,
         ), 'Only GaussianLearningActor support annealing.'
         self.actor.std = self.std_schedule.value(epoch)
```

### Comparing `omnisafe-0.3.0/omnisafe/models/actor_critic/actor_q_critic.py` & `omnisafe-0.4.0/omnisafe/models/actor_critic/actor_q_critic.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,47 +10,48 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of ActorQCritic."""
 
+from __future__ import annotations
+
 from copy import deepcopy
 
 import torch
 from torch import nn, optim
-from torch.optim.lr_scheduler import ConstantLR, LinearLR, _LRScheduler
+from torch.optim.lr_scheduler import ConstantLR, LinearLR
 
+from omnisafe.models.actor import GaussianLearningActor, GaussianSACActor, MLPActor
 from omnisafe.models.actor.actor_builder import ActorBuilder
+from omnisafe.models.base import Critic
 from omnisafe.models.critic.critic_builder import CriticBuilder
 from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils.config import ModelConfig
 
 
 class ActorQCritic(nn.Module):
     """Class for ActorQCritic.
 
-    In ``omnisafe``, we combine the actor and critic into one this class.
-
-    .. list-table::
+    In OmniSafe, we combine the actor and critic into one this class.
 
-        *   -   Model
-            -   Description
-            -   Function
-        *   -   Actor
-            -   The policy network, input is observation, output is action.
-                Choose the actor from the following options:
-                :class:`MLPActor`, :class:`GaussianSACActor`,
-                :class:`GaussianLearningActor`.
-            -   Choose the action based on the observation.
-        *   -   Value Critic
-            -   The value network, input is observation, output is reward value.
-                Choose the critic from the following options:
-                :class:`QCritic`, :class:`VCritic`.
-            -   Estimate the reward value of the observation.
+    +-----------------+---------------------------------------------------+
+    | Model           | Description                                       |
+    +=================+===================================================+
+    | Actor           | Input is observation. Output is action.           |
+    +-----------------+---------------------------------------------------+
+    | Reward Q Critic | Input is obs-action pair. Output is reward value. |
+    +-----------------+---------------------------------------------------+
+
+    Args:
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        model_cfgs (ModelConfig): The model configurations.
+        epochs (int): The number of epochs.
 
     Attributes:
         actor (Actor): The actor network.
         target_actor (Actor): The target actor network.
         reward_critic (Critic): The critic network.
         target_reward_critic (Critic): The target critic network.
         actor_optimizer (Optimizer): The optimizer for the actor network.
@@ -62,48 +63,55 @@
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         model_cfgs: ModelConfig,
         epochs: int,
     ) -> None:
-        """Initialize ActorQCritic."""
+        """Initialize an instance of :class:`ActorQCritic`."""
         super().__init__()
-        self.actor = ActorBuilder(
+
+        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor = ActorBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.actor.hidden_sizes,
             activation=model_cfgs.actor.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
         ).build_actor(actor_type=model_cfgs.actor_type)
-        self.reward_critic = CriticBuilder(
+        self.reward_critic: Critic = CriticBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.critic.hidden_sizes,
             activation=model_cfgs.critic.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
             num_critics=model_cfgs.critic.num_critics,
             use_obs_encoder=False,
         ).build_critic(critic_type='q')
-        self.target_reward_critic = deepcopy(self.reward_critic)
+        self.target_reward_critic: Critic = deepcopy(self.reward_critic)
         for param in self.target_reward_critic.parameters():
             param.requires_grad = False
-        self.target_actor = deepcopy(self.actor)
+        self.target_actor: GaussianLearningActor | GaussianSACActor | MLPActor = deepcopy(
+            self.actor,
+        )
         for param in self.target_actor.parameters():
             param.requires_grad = False
         self.add_module('actor', self.actor)
         self.add_module('reward_critic', self.reward_critic)
 
-        self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=model_cfgs.actor.lr)
-        self.reward_critic_optimizer = optim.Adam(
-            self.reward_critic.parameters(),
-            lr=model_cfgs.critic.lr,
-        )
+        if model_cfgs.actor.lr is not None:
+            self.actor_optimizer: optim.Optimizer
+            self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=model_cfgs.actor.lr)
+        if model_cfgs.critic.lr is not None:
+            self.reward_critic_optimizer: optim.Optimizer
+            self.reward_critic_optimizer = optim.Adam(
+                self.reward_critic.parameters(),
+                lr=model_cfgs.critic.lr,
+            )
 
-        self.actor_scheduler: _LRScheduler
+        self.actor_scheduler: LinearLR | ConstantLR
         if model_cfgs.linear_lr_decay:
             self.actor_scheduler = LinearLR(
                 self.actor_optimizer,
                 start_factor=1.0,
                 end_factor=0.0,
                 total_iters=epochs,
                 verbose=True,
@@ -116,40 +124,42 @@
                 verbose=True,
             )
 
     def step(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
         """Choose the action based on the observation. used in rollout without gradient.
 
         Args:
-            obs: The observation.
-            deterministic: Whether to use deterministic action. default: False.
+            obs (torch.tensor): The observation.
+            deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
-            The action, value_r, and log_prob.
+            The deterministic action if ``deterministic`` is True, otherwise the action with
+            Gaussian noise.
         """
         with torch.no_grad():
             return self.actor.predict(obs, deterministic=deterministic)
 
     def forward(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
         """Choose the action based on the observation. used in training with gradient.
 
         Args:
-            obs: The observation.
-            deterministic: Whether to use deterministic action. default: False.
+            obs (torch.tensor): The observation.
+            deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
-            The action, value_r, and log_prob.
+            The deterministic action if ``deterministic`` is True, otherwise the action with
+            Gaussian noise.
         """
         return self.step(obs, deterministic=deterministic)
 
     def polyak_update(self, tau: float) -> None:
         """Update the target network with polyak averaging.
 
         Args:
-            tau: The polyak averaging factor.
+            tau (float): The polyak averaging factor.
         """
         for param, target_param in zip(
             self.reward_critic.parameters(),
             self.target_reward_critic.parameters(),
         ):
             target_param.data.copy_(tau * param.data + (1 - tau) * target_param.data)
         for param, target_param in zip(self.actor.parameters(), self.target_actor.parameters()):
```

### Comparing `omnisafe-0.3.0/omnisafe/models/actor_critic/constraint_actor_critic.py` & `omnisafe-0.4.0/omnisafe/models/actor_critic/constraint_actor_critic.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,47 +16,40 @@
 
 from __future__ import annotations
 
 import torch
 from torch import optim
 
 from omnisafe.models.actor_critic.actor_critic import ActorCritic
+from omnisafe.models.base import Critic
 from omnisafe.models.critic.critic_builder import CriticBuilder
 from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils.config import ModelConfig
 
 
 class ConstraintActorCritic(ActorCritic):
     """ConstraintActorCritic is a wrapper around ActorCritic that adds a cost critic to the model.
 
-    In ``omnisafe``, we combine the actor and critic into one this class.
+    In OmniSafe, we combine the actor and critic into one this class.
 
-        .. list-table::
-
-            *   -   Model
-                -   Description
-                -   Function
-            *   -   Actor
-                -   The policy network, input is observation, output is action.
-                    Choose the actor from the following options:
-                    :class:`MLPActor`, :class:`CategoricalActor`, :class:`GaussianAnnealingActor`,
-                    :class:`GaussianLearningActor`, :class:`GaussianStdNetActor`, :class:`MLPCholeskyActor`.
-                -   Choose the action based on the observation.
-            *   -   Reward Critic
-                -   The value network, input is observation,
-                    output is reward value.
-                    Choose the critic from the following options:
-                    :class:`QCritic`, :class:`VCritic`.
-                -   Estimate the reward value of the observation.
-            *   -   Cost Critic
-                -   The value network, input is observation,
-                    output is cost value.
-                    Choose the critic from the following options:
-                    :class:`QCritic`, :class:`VCritic`.
-                -   Estimate the cost value of the observation.
+    +-----------------+-----------------------------------------------+
+    | Model           | Description                                   |
+    +=================+===============================================+
+    | Actor           | Input is observation. Output is action.       |
+    +-----------------+-----------------------------------------------+
+    | Reward V Critic | Input is observation. Output is reward value. |
+    +-----------------+-----------------------------------------------+
+    | Cost V Critic   | Input is observation. Output is cost value.   |
+    +-----------------+-----------------------------------------------+
+
+    Args:
+        obs_space (OmnisafeSpace): The observation space.
+        act_space (OmnisafeSpace): The action space.
+        model_cfgs (ModelConfig): The model configurations.
+        epochs (int): The number of epochs.
 
     Attributes:
         actor (Actor): The actor network.
         reward_critic (Critic): The critic network.
         cost_critic (Critic): The critic network.
         std_schedule (Schedule): The schedule for the standard deviation of the Gaussian distribution.
     """
@@ -64,62 +57,73 @@
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         model_cfgs: ModelConfig,
         epochs: int,
     ) -> None:
-        """Initialize ConstraintActorCritic."""
+        """Initialize an instance of :class:`ConstraintActorCritic`."""
         super().__init__(obs_space, act_space, model_cfgs, epochs)
-        self.cost_critic = CriticBuilder(
+        self.cost_critic: Critic = CriticBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.critic.hidden_sizes,
             activation=model_cfgs.critic.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
             num_critics=1,
             use_obs_encoder=False,
         ).build_critic('v')
         self.add_module('cost_critic', self.cost_critic)
 
-        if model_cfgs.critic.lr != 'None':
+        if model_cfgs.critic.lr is not None:
+            self.cost_critic_optimizer: optim.Optimizer
             self.cost_critic_optimizer = optim.Adam(
                 self.cost_critic.parameters(),
                 lr=model_cfgs.critic.lr,
             )
 
-    def step(self, obs: torch.Tensor, deterministic: bool = False) -> tuple[torch.Tensor, ...]:
+    def step(
+        self,
+        obs: torch.Tensor,
+        deterministic: bool = False,
+    ) -> tuple[torch.Tensor, ...]:
         """Choose action based on observation.
 
         Args:
-            obs (torch.Tensor): Observation.
-            deterministic (bool): Whether to use deterministic policy.
+            obs (torch.Tensor): Observation from environments.
+            deterministic (bool, optional): Whether to use deterministic policy. Defaults to False.
 
         Returns:
-            action (torch.Tensor): Action.
-            value_r (torch.Tensor): Reward value.
-            value_c (torch.Tensor): Cost value.
-            log_prob (torch.Tensor): Log probability of action.
+            action: The deterministic action if ``deterministic`` is True, otherwise the action with
+                Gaussian noise.
+            value_r: The reward value of the observation.
+            value_c: The cost value of the observation.
+            log_prob: The log probability of the action.
         """
         with torch.no_grad():
             value_r = self.reward_critic(obs)
             value_c = self.cost_critic(obs)
 
             action = self.actor.predict(obs, deterministic=deterministic)
             log_prob = self.actor.log_prob(action)
 
         return action, value_r[0], value_c[0], log_prob
 
-    def forward(self, obs: torch.Tensor, deterministic: bool = False) -> tuple[torch.Tensor, ...]:
+    def forward(
+        self,
+        obs: torch.Tensor,
+        deterministic: bool = False,
+    ) -> tuple[torch.Tensor, ...]:
         """Choose action based on observation.
 
         Args:
-            obs (torch.Tensor): Observation.
-            deterministic (bool): Whether to use deterministic policy.
+            obs (torch.Tensor): Observation from environments.
+            deterministic (bool, optional): Whether to use deterministic policy. Defaults to False.
 
         Returns:
-            action (torch.Tensor): Action.
-            value_r (torch.Tensor): Reward value.
-            value_c (torch.Tensor): Cost value.
-            log_prob (torch.Tensor): Log probability of action.
+            action: The deterministic action if ``deterministic`` is True, otherwise the action with
+                Gaussian noise.
+            value_r: The reward value of the observation.
+            value_c: The cost value of the observation.
+            log_prob: The log probability of the action.
         """
         return self.step(obs, deterministic=deterministic)
```

### Comparing `omnisafe-0.3.0/omnisafe/models/base.py` & `omnisafe-0.4.0/omnisafe/models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,202 +22,187 @@
 import torch.nn as nn
 from gymnasium import spaces
 from torch.distributions import Distribution
 
 from omnisafe.typing import Activation, InitFunction, OmnisafeSpace
 
 
-class Actor(ABC, nn.Module):
+class Actor(nn.Module, ABC):
     """A abstract class for actor.
 
-    An actor approximates the policy function that maps observations to actions.
-    Actor is parameterized by a neural network that takes observations as input,
-    and outputs the mean and standard deviation of the action distribution.
+    An actor approximates the policy function that maps observations to actions. Actor is
+    parameterized by a neural network that takes observations as input, and outputs the mean and
+    standard deviation of the action distribution.
 
     .. note::
         You can use this class to implement your own actor by inheriting it.
 
-    Attributes:
-        _obs_space (OmnisafeSpace): observation space.
-        _act_space (OmnisafeSpace): action space.
-        _weight_initialization_mode (InitFunction): weight initialization mode.
-        _activation (Activation): activation function.
-        _hidden_sizes (list): hidden layer sizes.
-        _current_dist (Distribution): current distribution.
-        _after_inference (bool): whether the actor has been used to sample actions.
-        _obs_dim (int): observation dimension.
-        _act_dim (int): action dimension.
+    Args:
+        obs_space (OmnisafeSpace): observation space.
+        act_space (OmnisafeSpace): action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
     ) -> None:
-        """Initialize the base actor.
-
-        Args:
-            obs_space (OmnisafeSpace): observation space.
-            act_space (OmnisafeSpace): action space.
-            hidden_sizes (list): hidden layer sizes.
-            activation (Activation): activation function.
-            weight_initialization_mode (InitFunction, optional): weight initialization mode.
-                                                                Defaults to ``kaiming_uniform``.
-            shared (nn.Module, optional): shared module. Defaults to None.
-        """
+        """Initialize an instance of :class:`Actor`."""
         nn.Module.__init__(self)
-        self._obs_space = obs_space
-        self._act_space = act_space
-        self._weight_initialization_mode = weight_initialization_mode
-        self._activation = activation
-        self._hidden_sizes = hidden_sizes
-
-        self._current_dist: Distribution
+        self._obs_space: OmnisafeSpace = obs_space
+        self._act_space: OmnisafeSpace = act_space
+        self._weight_initialization_mode: InitFunction = weight_initialization_mode
+        self._activation: Activation = activation
+        self._hidden_sizes: list[int] = hidden_sizes
         self._after_inference: bool = False
 
         if isinstance(self._obs_space, spaces.Box) and len(self._obs_space.shape) == 1:
-            self._obs_dim = self._obs_space.shape[0]
+            self._obs_dim: int = self._obs_space.shape[0]
         else:
             raise NotImplementedError
 
         if isinstance(self._act_space, spaces.Box) and len(self._act_space.shape) == 1:
-            self._act_dim = self._act_space.shape[0]
+            self._act_dim: int = self._act_space.shape[0]
         else:
             raise NotImplementedError
 
     @abstractmethod
     def _distribution(self, obs: torch.Tensor) -> Distribution:
         r"""Return the distribution of action.
 
-        An actor generates a distribution, which is used to sample actions during training.
-        When training, the mean and the variance of the distribution are used to calculate the loss.
-        When testing, the mean of the distribution is used directly as actions.
+        An actor generates a distribution, which is used to sample actions during training. When
+        training, the mean and the variance of the distribution are used to calculate the loss. When
+        testing, the mean of the distribution is used directly as actions.
 
         For example, if the action is continuous, the actor can generate a Gaussian distribution.
 
         .. math::
-            p(a | s) = N(a | \mu(s), \sigma(s))
 
-        where :math:`\mu(s)` and :math:`\sigma(s)` are the mean and standard deviation of the distribution.
+            p (a | s) = N (\mu (s), \sigma (s))
+
+        where :math:`\mu (s)` and :math:`\sigma (s)` are the mean and standard deviation of the
+        distribution.
 
         .. warning::
-            The distribution is a private method, which is only used to sample actions during training.
-            You should not use it directly in your code,
-            instead, you should use the public method ``predict`` to sample actions.
+            The distribution is a private method, which is only used to sample actions during
+            training. You should not use it directly in your code, instead, you should use the
+            public method :meth:`predict` to sample actions.
 
         Args:
-            obs (torch.Tensor): observation.
+            obs (torch.Tensor): Observation from environments.
 
         Returns:
-            Distribution: the distribution of action.
+            The distribution of action.
         """
 
     @abstractmethod
     def forward(self, obs: torch.Tensor) -> Distribution:
-        r"""Return the distribution of action.
+        """Return the distribution of action.
 
         Args:
-            obs (torch.Tensor): observation.
+            obs (torch.Tensor): Observation from environments.
         """
 
     @abstractmethod
     def predict(
         self,
         obs: torch.Tensor,
         deterministic: bool = False,
     ) -> torch.Tensor:
         r"""Predict deterministic or stochastic action based on observation.
 
         - ``deterministic`` = ``True`` or ``False``
 
-        When training the actor,
-        one important trick to avoid local minimum is to use stochastic actions,
-        which can simply be achieved by sampling actions from the distribution
-        (set ``deterministic`` = ``False``).
-
-        When testing the actor,
-        we want to know the actual action that the agent will take,
-        so we should use deterministic actions (set ``deterministic`` = ``True``).
+        When training the actor, one important trick to avoid local minimum is to use stochastic
+        actions, which can simply be achieved by sampling actions from the distribution (set
+        ``deterministic=False``).
+
+        When testing the actor, we want to know the actual action that the agent will take, so we
+        should use deterministic actions (set ``deterministic=True``).
 
         .. math::
-            L = -\mathbb{E}_{s \sim p(s)} [\log p(a | s) A^R (s, a)]
 
-        where :math:`p(s)` is the distribution of observation,
-        :math:`p(a | s)` is the distribution of action,
-        and :math:`\log p(a | s)` is the log probability of action under the distribution.,
-        :math:`A^R (s, a)` is the advantage function.
+            L = -\mathbb{E}_{s \sim p(s)} [ \log p (a | s) A^R (s, a) ]
+
+        where :math:`p (s)` is the distribution of observation, :math:`p (a | s)` is the
+        distribution of action, and :math:`\log p (a | s)` is the log probability of action under
+        the distribution., and :math:`A^R (s, a)` is the advantage function.
 
         Args:
-            obs (torch.Tensor): observation.
+            obs (torch.Tensor): Observation from environments.
             deterministic (bool, optional): whether to predict deterministic action. Defaults to False.
         """
 
     @abstractmethod
     def log_prob(self, act: torch.Tensor) -> torch.Tensor:
-        r"""Return the log probability of action under the distribution.
+        """Return the log probability of action under the distribution.
 
-        ``log_prob`` only can be called after calling ``predict`` or ``forward``.
+        :meth:`log_prob` only can be called after calling :meth:`predict` or :meth:`forward`.
 
         Args:
-            obs (torch.Tensor): observation.
-            act (torch.Tensor): action.
+            act (torch.Tensor): The action.
 
         Returns:
-            torch.Tensor: the log probability of action under the distribution.
+            The log probability of action under the distribution.
         """
 
 
-class Critic(ABC, nn.Module):
+class Critic(nn.Module, ABC):
     """A abstract class for critic.
 
-    A critic approximates the value function that maps observations to values.
-    Critic is parameterized by a neural network that takes observations as input,
-    (Q critic also takes actions as input) and outputs the value of the observation.
+    A critic approximates the value function that maps observations to values. Critic is
+    parameterized by a neural network that takes observations as input, (Q critic also takes actions
+    as input) and outputs the value of the observation.
 
     .. note::
-        Omnisafe provides two types of critic:
+        OmniSafe provides two types of critic:
         Q critic (Input = ``observation`` + ``action`` , Output = ``value``),
         and V critic (Input = ``observation`` , Output = ``value``).
         You can also use this class to implement your own actor by inheriting it.
+
+    Args:
+        obs_space (OmnisafeSpace): observation space.
+        act_space (OmnisafeSpace): action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+        num_critics (int, optional): Number of critics. Defaults to 1.
+        use_obs_encoder (bool, optional): Whether to use observation encoder, only used in q critic.
+            Defaults to False.
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
         num_critics: int = 1,
         use_obs_encoder: bool = False,
     ) -> None:
-        """Initialize the base critic.
-
-        Args:
-            obs_space (OmnisafeSpace): observation space.
-            act_space (OmnisafeSpace): action space.
-            hidden_sizes (list): hidden layer sizes.
-            activation (Activation, optional): activation function. Defaults to 'relu'.
-            weight_initialization_mode (InitFunction, optional): weight initialization mode.
-                                                                Defaults to 'kaiming_uniform'.
-            shared (nn.Module, optional): shared module. Defaults to None.
-        """
+        """Initialize an instance of :class:`Critic`."""
         nn.Module.__init__(self)
-        self._obs_space = obs_space
-        self._act_space = act_space
-        self._weight_initialization_mode = weight_initialization_mode
-        self._activation = activation
-        self._hidden_sizes = hidden_sizes
-        self._num_critics = num_critics
-        self._use_obs_encoder = use_obs_encoder
+        self._obs_space: OmnisafeSpace = obs_space
+        self._act_space: OmnisafeSpace = act_space
+        self._weight_initialization_mode: InitFunction = weight_initialization_mode
+        self._activation: Activation = activation
+        self._hidden_sizes: list[int] = hidden_sizes
+        self._num_critics: int = num_critics
+        self._use_obs_encoder: bool = use_obs_encoder
 
         if isinstance(self._obs_space, spaces.Box) and len(self._obs_space.shape) == 1:
             self._obs_dim = self._obs_space.shape[0]
         else:
             raise NotImplementedError
 
         if isinstance(self._act_space, spaces.Box) and len(self._act_space.shape) == 1:
```

### Comparing `omnisafe-0.3.0/omnisafe/models/critic/__init__.py` & `omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,12 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""The abstract interfaces of Critic networks for the Actor-Critic algorithm."""
+"""Simmer Reinforcement Learning algorithms."""
 
-from omnisafe.models.critic.critic_builder import CriticBuilder
-from omnisafe.models.critic.q_critic import QCritic
-from omnisafe.models.critic.v_critic import VCritic
+from omnisafe.algorithms.on_policy.simmer.ppo_simmer_pid import PPOSimmerPID
+from omnisafe.algorithms.on_policy.simmer.trpo_simmer_pid import TRPOSimmerPID
+
+
+__all__ = [
+    'TRPOSimmerPID',
+    'PPOSimmerPID',
+]
```

### Comparing `omnisafe-0.3.0/omnisafe/models/critic/critic_builder.py` & `omnisafe-0.4.0/omnisafe/models/critic/critic_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,67 +20,72 @@
 from omnisafe.models.critic.q_critic import QCritic
 from omnisafe.models.critic.v_critic import VCritic
 from omnisafe.typing import Activation, CriticType, InitFunction, OmnisafeSpace
 
 
 # pylint: disable-next=too-few-public-methods
 class CriticBuilder:
-    """Implementation of CriticBuilder
+    """Implementation of CriticBuilder.
 
     .. note::
-
-        A :class:`CriticBuilder` is a class for building a critic network.
-        In ``omnisafe``, instead of building the critic network directly,
-        we build it by integrating various types of critic networks into the :class:`CriticBuilder`.
-        The advantage of this is that each type of critic has a uniform way of passing parameters.
-        This makes it easy for users to use existing critics,
-        and also facilitates the extension of new critic types.
+        A :class:`CriticBuilder` is a class for building a critic network. In OmniSafe, instead of
+        building the critic network directly, we build it by integrating various types of critic
+        networks into the :class:`CriticBuilder`. The advantage of this is that each type of critic
+        has a uniform way of passing parameters. This makes it easy for users to use existing
+        critics, and also facilitates the extension of new critic types.
+
+    Args:
+        obs_space (OmnisafeSpace): Observation space.
+        act_space (OmnisafeSpace): Action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+        num_critics (int, optional): Number of critics. Defaults to 1.
+        use_obs_encoder (bool, optional): Whether to use observation encoder, only used in q critic.
+            Defaults to False.
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
         num_critics: int = 1,
         use_obs_encoder: bool = False,
     ) -> None:
-        """Initialize CriticBuilder.
-
-        Args:
-            obs_space (OmnisafeSpace): Observation space.
-            act_space (OmnisafeSpace): Action space.
-            hidden_sizes (List[int]): Hidden sizes of the critic network.
-            activation (Activation): Activation function.
-            weight_initialization_mode (InitFunction): Weight initialization mode.
-            num_critics (int): Number of critics.
-            use_obs_encoder (bool): Whether to use observation encoder, only used in q critic.
-        """
-        self._obs_space = obs_space
-        self._act_space = act_space
-        self._weight_initialization_mode = weight_initialization_mode
-        self._activation = activation
-        self._hidden_sizes = hidden_sizes
-        self._num_critics = num_critics
-        self._use_obs_encoder = use_obs_encoder
+        """Initialize an instance of :class:`CriticBuilder`."""
+        self._obs_space: OmnisafeSpace = obs_space
+        self._act_space: OmnisafeSpace = act_space
+        self._weight_initialization_mode: InitFunction = weight_initialization_mode
+        self._activation: Activation = activation
+        self._hidden_sizes: list[int] = hidden_sizes
+        self._num_critics: int = num_critics
+        self._use_obs_encoder: bool = use_obs_encoder
 
     def build_critic(
         self,
         critic_type: CriticType,
     ) -> Critic:
         """Build critic.
 
         Currently, we support two types of critics: ``q`` and ``v``.
         If you want to add a new critic type, you can simply add it here.
 
         Args:
             critic_type (str): Critic type.
+
+        Returns:
+            V-Critic or Q-Critic.
+
+        Raises:
+            NotImplementedError: If the critic type is not ``q`` or ``v``.
         """
         if critic_type == 'q':
             return QCritic(
                 obs_space=self._obs_space,
                 act_space=self._act_space,
                 hidden_sizes=self._hidden_sizes,
                 activation=self._activation,
```

### Comparing `omnisafe-0.3.0/omnisafe/models/critic/q_critic.py` & `omnisafe-0.4.0/omnisafe/models/critic/q_critic.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,71 +23,68 @@
 from omnisafe.typing import Activation, InitFunction, OmnisafeSpace
 from omnisafe.utils.model import build_mlp_network
 
 
 class QCritic(Critic):
     """Implementation of QCritic.
 
-    A Q-function approximator that uses a multi-layer perceptron (MLP) to map observation-action pairs to Q-values.
-    This class is an inherit class of :class:`Critic`.
-    You can design your own Q-function approximator by inheriting this class or :class:`Critic`.
+    A Q-function approximator that uses a multi-layer perceptron (MLP) to map observation-action
+    pairs to Q-values. This class is an inherit class of :class:`Critic`. You can design your own
+    Q-function approximator by inheriting this class or :class:`Critic`.
+
+    The Q critic network has two modes:
+
+    .. hint::
+        - ``use_obs_encoder = False``: The input of the network is the concatenation of the
+            observation and action.
+        - ``use_obs_encoder = True``: The input of the network is the concatenation of the output of
+            the observation encoder and action.
+
+    For example, in :class:`DDPG`, the action is not directly concatenated with the observation, but
+    is concatenated with the output of the observation encoder.
+
+    .. note::
+        The Q critic network contains multiple critics, and the output of the network :meth`forward`
+        is a list of Q-values. If you want to get the single Q-value of a specific critic, you need
+        to use the index to get it.
+
+    Args:
+        obs_space (OmnisafeSpace): observation space.
+        act_space (OmnisafeSpace): action space.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+        num_critics (int, optional): Number of critics. Defaults to 1.
+        use_obs_encoder (bool, optional): Whether to use observation encoder, only used in q critic.
+            Defaults to False.
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
         num_critics: int = 1,
         use_obs_encoder: bool = False,
     ) -> None:
-        """Initialize the critic network.
-
-        The Q critic network has two modes:
-
-        .. hint::
-            -  ``use_obs_encoder`` = ``False`` :
-                The input of the network is the concatenation of the observation and action.
-            -  ``use_obs_encoder`` = ``True`` :
-                The input of the network is the concatenation of the output of the observation encoder and action.
-
-        For example, in :class:`DDPG`,
-        the action is not directly concatenated with the observation,
-        but is concatenated with the output of the observation encoder.
-
-        .. note::
-            The Q critic network contains multiple critics,
-            and the output of the network :meth`forward` is a list of Q-values.
-            If you want to get the single Q-value of a specific critic,
-            you need to use the index to get it.
-
-        Args:
-            obs_space (OmnisafeSpace): observation space.
-            act_space (OmnisafeSpace): action space.
-            hidden_sizes (list): list of hidden layer sizes.
-            activation (Activation): activation function.
-            weight_initialization_mode (InitFunction): weight initialization mode.
-            shared (nn.Module): shared network.
-            num_critics (int): number of critics.
-            use_obs_encoder (bool): whether to use observation encoder.
-
-        """
+        """Initialize an instance of :class:`QCritic`."""
         super().__init__(
             obs_space,
             act_space,
             hidden_sizes,
             activation,
             weight_initialization_mode,
             num_critics,
             use_obs_encoder,
         )
-        self.net_lst: list[nn.Module] = []
+        self.net_lst: list[nn.Sequential] = []
         for idx in range(self._num_critics):
             if self._use_obs_encoder:
                 obs_encoder = build_mlp_network(
                     [self._obs_dim, hidden_sizes[0]],
                     activation=activation,
                     output_activation=activation,
                     weight_initialization_mode=weight_initialization_mode,
@@ -111,24 +108,26 @@
     def forward(
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
     ) -> list[torch.Tensor]:
         """Forward function.
 
-        As a multi-critic network, the output of the network is a list of Q-values.
-        If you want to use it as a single-critic network,
-        you only need to set the ``num_critics`` parameter to 1 when initializing the network,
-        and then use the index 0 to get the Q-value.
+        As a multi-critic network, the output of the network is a list of Q-values. If you want to
+        use it as a single-critic network, you only need to set the ``num_critics`` parameter to 1
+        when initializing the network, and then use the index 0 to get the Q-value.
 
         Args:
-            obs (torch.Tensor): Observation.
+            obs (torch.Tensor): Observation from environments.
             act (torch.Tensor): Action.
+
+        Returns:
+            A list of Q critic values of action and observation pair.
         """
         res = []
         for critic in self.net_lst:
             if self._use_obs_encoder:
-                obs_encode = critic[0](obs)  # type: ignore
-                res.append(torch.squeeze(critic[1](torch.cat([obs_encode, act], dim=-1)), -1))  # type: ignore
+                obs_encode = critic[0](obs)
+                res.append(torch.squeeze(critic[1](torch.cat([obs_encode, act], dim=-1)), -1))
             else:
                 res.append(torch.squeeze(critic(torch.cat([obs, act], dim=-1)), -1))
         return res
```

### Comparing `omnisafe-0.3.0/omnisafe/models/critic/v_critic.py` & `omnisafe-0.4.0/omnisafe/models/critic/v_critic.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,45 +26,47 @@
 
 class VCritic(Critic):
     """Implementation of VCritic.
 
     A V-function approximator that uses a multi-layer perceptron (MLP) to map observations to V-values.
     This class is an inherit class of :class:`Critic`.
     You can design your own V-function approximator by inheriting this class or :class:`Critic`.
+
+    Args:
+        obs_dim (int): Observation dimension.
+        act_dim (int): Action dimension.
+        hidden_sizes (list of int): List of hidden layer sizes.
+        activation (Activation, optional): Activation function. Defaults to ``'relu'``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+        num_critics (int, optional): Number of critics. Defaults to 1.
     """
 
     def __init__(
         self,
         obs_space: OmnisafeSpace,
         act_space: OmnisafeSpace,
         hidden_sizes: list[int],
         activation: Activation = 'relu',
         weight_initialization_mode: InitFunction = 'kaiming_uniform',
         num_critics: int = 1,
     ) -> None:
-        """Initialize the critic network.
-
-        Args:
-            obs_dim (int): Observation dimension.
-            act_dim (int): Action dimension.
-            hidden_sizes (list): Hidden layer sizes.
-            activation (Activation): Activation function.
-            weight_initialization_mode (InitFunction): Weight initialization mode.
-            shared (nn.Module): Shared network.
-        """
+        """Initialize an instance of :class:`VCritic`."""
         super().__init__(
             obs_space,
             act_space,
             hidden_sizes,
             activation,
             weight_initialization_mode,
             num_critics,
             use_obs_encoder=False,
         )
-        self.net_lst: list[nn.Module] = []
+        self.net_lst: list[nn.Module]
+        self.net_lst = []
+
         for idx in range(self._num_critics):
             net = build_mlp_network(
                 sizes=[self._obs_dim, *self._hidden_sizes, 1],
                 activation=self._activation,
                 weight_initialization_mode=self._weight_initialization_mode,
             )
             self.net_lst.append(net)
@@ -76,12 +78,15 @@
     ) -> list[torch.Tensor]:
         """Forward function.
 
         Specifically, V function approximator maps observations to V-values.
 
         Args:
             obs (torch.Tensor): Observations.
+
+        Returns:
+            The V critic value of observation.
         """
         res = []
         for critic in self.net_lst:
             res.append(torch.squeeze(critic(obs), -1))
         return res
```

### Comparing `omnisafe-0.3.0/omnisafe/typing.py` & `omnisafe-0.4.0/omnisafe/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,24 +24,28 @@
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 
+import torch
 from gymnasium.spaces import Box, Discrete
+from torch.types import Device
 
 
 RenderFrame = TypeVar('RenderFrame')
 OmnisafeSpace = Union[Box, Discrete]
 Activation = Literal['identity', 'relu', 'sigmoid', 'softplus', 'tanh']
 AdvatageEstimator = Literal['gae', 'gae-rtg', 'vtrace', 'plain']
 InitFunction = Literal['kaiming_uniform', 'xavier_normal', 'glorot', 'xavier_uniform', 'orthogonal']
 CriticType = Literal['v', 'q']
 ActorType = Literal['gaussian_learning', 'gaussian_sac', 'mlp']
+DEVICE_CPU = torch.device('cpu')
+
 
 __all__ = [
     'Activation',
     'AdvatageEstimator',
     'InitFunction',
     'Callable',
     'List',
@@ -50,8 +54,11 @@
     'Tuple',
     'TypeVar',
     'Union',
     'Dict',
     'NamedTuple',
     'Any',
     'OmnisafeSpace',
+    'RenderFrame',
+    'Device',
+    'DEVICE_CPU',
 ]
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/__init__.py` & `omnisafe-0.4.0/omnisafe/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+"""Utility functions for OmniSafe."""
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/command_app.py` & `omnisafe-0.4.0/omnisafe/utils/command_app.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,104 +10,132 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the command interfaces."""
 
+
 import os
-import sys
 import warnings
-from typing import List
+from typing import Any, Dict, List
 
 import numpy as np
 import torch
 import typer
 import yaml
 from rich.console import Console
 
 import omnisafe
 from omnisafe.common.experiment_grid import ExperimentGrid
 from omnisafe.common.statistics_tools import StatisticsTools
-from omnisafe.typing import NamedTuple, Tuple
+from omnisafe.utils.exp_grid_tools import train as train_grid
 from omnisafe.utils.tools import assert_with_exit, custom_cfgs_to_dict, update_dict
 
 
 app = typer.Typer()
 console = Console()
 
 
 @app.command()
 def train(  # pylint: disable=too-many-arguments
     algo: str = typer.Option(
         'PPOLag',
-        help=f"algorithm to train{omnisafe.ALGORITHMS['all']}",
+        help=f"algorithm to train {omnisafe.ALGORITHMS['all']}",
         case_sensitive=False,
     ),
     env_id: str = typer.Option(
-        'SafetyHumanoidVelocity-v4',
+        'SafetyHumanoidVelocity-v1',
         help='the name of test environment',
         case_sensitive=False,
     ),
-    parallel: int = typer.Option(1, help='number of paralleled progress for calculations.'),
-    total_steps: int = typer.Option(1638400, help='total number of steps to train for algorithm'),
-    device: str = typer.Option('cpu', help='device to use for training'),
-    vector_env_nums: int = typer.Option(16, help='number of vector envs to use for training'),
-    torch_threads: int = typer.Option(16, help='number of threads to use for torch'),
+    parallel: int = typer.Option(
+        1,
+        help='number of paralleled progress for calculations.',
+    ),
+    total_steps: int = typer.Option(
+        1638400,
+        help='total number of steps to train for algorithm',
+    ),
+    device: str = typer.Option(
+        'cpu',
+        help='device to use for training',
+    ),
+    vector_env_nums: int = typer.Option(
+        16,
+        help='number of vector envs to use for training',
+    ),
+    torch_threads: int = typer.Option(
+        16,
+        help='number of threads to use for torch',
+    ),
     log_dir: str = typer.Option(
         os.path.abspath('.'),
         help='directory to save logs, default is current directory',
     ),
-    plot: bool = typer.Option(False, help='whether to plot the training curve after training'),
+    plot: bool = typer.Option(
+        False,
+        help='whether to plot the training curve after training',
+    ),
     render: bool = typer.Option(
         False,
         help='whether to render the trajectory of models saved during training',
     ),
     evaluate: bool = typer.Option(
         False,
         help='whether to evaluate the trajectory of models saved during training',
     ),
-    custom_cfgs: List[str] = typer.Option([], help='custom configuration for training'),
-):
-    """Train a single policy in OmniSafe via command line.
-
-    Example:
+    custom_cfgs: List[str] = typer.Option(
+        [],
+        help='custom configuration for training',
+    ),
+) -> None:
+    r"""Train a single policy in OmniSafe via command line.
 
-    .. code-block:: bash
+    Examples:
+        .. code-block:: bash
 
-        python -m omnisafe train --algo PPOLag --env_id SafetyPointGoal1-v0 --parallel 1
-        --total_steps 1000000 --device cpu --vector_env_nums 1
+            python -m omnisafe train --algo PPOLag --env_id SafetyPointGoal1-v0 --parallel 1 \
+                --total_steps 1000000 --device cpu --vector_env_nums 1
 
     Args:
-        algo: algorithm to train.
-        env_id: the name of test environment.
-        parallel: number of paralleled progress for calculations.
-        total_steps: total number of steps to train for algorithm
-        device: device to use for training.
-        vector_env_nums: number of vector envs to use for training
-        torch_threads: number of threads to use for torch.
-        log_dir: directory to save logs, default is current directory
-        custom_cfgs: custom configuration for training.
+        algo (str): Algorithm to train.
+        env_id (str): The name of test environment.
+        parallel (int, optional): Number of paralleled progress for calculations. Defaults to 1.
+        total_steps (int, optional): Total number of steps to train for algorithm. Defaults to
+            16384000.
+        device (str, optional): Device to use for training. Defaults to 'cpu'.
+        vector_env_nums (int, optional): Number of vector envs to use for training. Defaults to 16.
+        torch_threads (int, optional): Number of threads to use for torch. Defaults to 16.
+        log_dir (str, optional): Directory to save logs, default is current directory. Defaults to
+            ``os.path.abspath('.')``.
+        plot (bool, optional): Whether to plot the training curve after training. Defaults to False.
+        render (bool, optional): Whether to render the trajectory of models saved during training.
+            Defaults to False.
+        evaluate (bool, optional): Whether to evaluate the trajectory of models saved during
+            training. Defaults to False.
+        custom_cfgs (list of str, optional): Custom configuration for training. Defaults to ``[]``.
     """
     args = {
         'algo': algo,
         'env_id': env_id,
         'parallel': parallel,
         'total_steps': total_steps,
         'device': device,
         'vector_env_nums': vector_env_nums,
         'torch_threads': torch_threads,
     }
     keys = custom_cfgs[0::2]
-    values = list(custom_cfgs[1::2])
-    custom_cfgs = dict(zip(keys, values))
-    custom_cfgs.update({'logger_cfgs:log_dir': os.path.join(log_dir, 'train')})
+    values = custom_cfgs[1::2]
+    assert_with_exit(len(keys) == len(values), 'keys and values should be in pairs')
+    custom_cfgs_dict = dict(zip(keys, values))
+    custom_cfgs_dict.update({'logger_cfgs:log_dir': os.path.join(log_dir, 'train')})
 
-    parsed_custom_cfgs = {}
-    for k, v in custom_cfgs.items():
+    parsed_custom_cfgs: Dict[str, Any] = {}
+    for k, v in custom_cfgs_dict.items():
         update_dict(parsed_custom_cfgs, custom_cfgs_to_dict(k, v))
 
     agent = omnisafe.Agent(
         algo=algo,
         env_id=env_id,
         train_terminal_cfgs=args,
         custom_cfgs=parsed_custom_cfgs,
@@ -127,97 +155,53 @@
     if evaluate:
         try:
             agent.evaluate(num_episodes=10)
         except RuntimeError:
             console.print('failed to evaluate model', style='red bold')
 
 
-def train_grid(
-    exp_id: str,
-    algo: str,
-    env_id: str,
-    custom_cfgs: NamedTuple,
-) -> Tuple[float, float, float]:
-    """Train a policy from exp-x config with OmniSafe.
-
-    Example:
-
-    .. code-block:: bash
-
-        python -m omnisafe train_grid --exp_id exp-1 --algo PPOLag --env_id SafetyPointGoal1-v0
-        --parallel 1 --total_steps 1000000 --device cpu --vector_env_nums 1
-
-    Args:
-        exp_id (str): Experiment ID.
-        algo (str): Algorithm to train.
-        env_id (str): The name of test environment.
-        custom_cfgs (NamedTuple): Custom configurations.
-        num_threads (int, optional): Number of threads. Defaults to 6.
-    """
-    terminal_log_name = 'terminal.log'
-    error_log_name = 'error.log'
-    if 'seed' in custom_cfgs:
-        terminal_log_name = f'seed{custom_cfgs["seed"]}_{terminal_log_name}'
-        error_log_name = f'seed{custom_cfgs["seed"]}_{error_log_name}'
-    sys.stdout = sys.__stdout__
-    sys.stderr = sys.__stderr__
-    print(f'exp-x: {exp_id} is training...')
-    if not os.path.exists(custom_cfgs['logger_cfgs']['log_dir']):
-        os.makedirs(custom_cfgs['logger_cfgs']['log_dir'])
-    # pylint: disable-next=consider-using-with
-    sys.stdout = open(  # noqa: SIM115
-        os.path.join(f'{custom_cfgs["logger_cfgs"]["log_dir"]}', terminal_log_name),
-        'w',
-        encoding='utf-8',
-    )
-    # pylint: disable-next=consider-using-with
-    sys.stderr = open(  # noqa: SIM115
-        os.path.join(f'{custom_cfgs["logger_cfgs"]["log_dir"]}', error_log_name),
-        'w',
-        encoding='utf-8',
-    )
-    agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
-    reward, cost, ep_len = agent.learn()
-    return reward, cost, ep_len
-
-
 @app.command()
 def benchmark(
-    exp_name: str = typer.Argument(..., help='experiment name'),
-    num_pool: int = typer.Argument(..., help='number of paralleled experiments.'),
+    exp_name: str = typer.Argument(
+        ...,
+        help='experiment name',
+    ),
+    num_pool: int = typer.Argument(
+        ...,
+        help='number of paralleled experiments.',
+    ),
     config_path: str = typer.Argument(
         ...,
         help='path to config file, it is supposed to be yaml file, e.g. ./configs/ppo.yaml',
     ),
     gpu_range: str = typer.Option(
         None,
-        help='range of gpu to use, the format is as same as range in python,'
+        help='range of gpu to use, the format is as same as range in python, '
         'for example, use 2==range(2), 0:2==range(0,2), 0:2:1==range(0,2,1) to select gpu',
     ),
     log_dir: str = typer.Option(
         os.path.abspath('.'),
         help='directory to save logs, default is current directory',
     ),
     render: bool = typer.Option(
         False,
         help='whether to render the trajectory of models saved during training',
     ),
     evaluate: bool = typer.Option(
         False,
         help='whether to evaluate the trajectory of models saved during training',
     ),
-):
-    """Benchmark algorithms configured by .yaml file in OmniSafe via command line.
+) -> None:
+    r"""Benchmark algorithms configured by .yaml file in OmniSafe via command line.
 
-    Example:
+    Examples:
+        .. code-block:: bash
 
-    .. code-block:: bash
-
-        python -m omnisafe benchmark --exp_name exp-1 --num_pool 1 --config_path ./configs/
-        on-policy/PPOLag.yaml--log_dir ./runs
+            python -m omnisafe benchmark --exp_name exp-1 --num_pool 1 \
+                --config_path ./configs/on-policy/PPOLag.yaml --log_dir ./runs
 
     Args:
         exp_name: experiment name
         num_pool: number of paralleled experiments.
         config_path: path to config file, it is supposed to be yaml file
         log_dir: directory to save logs, default is current directory
     """
@@ -238,15 +222,15 @@
         )
     log_dir = os.path.join(log_dir, 'benchmark')
     eg = ExperimentGrid(exp_name=exp_name)
     for k, v in configs.items():
         eg.add(key=k, vals=v)
 
     gpu_id = None
-    if gpu_range is not None:
+    if gpu_range is not None:  # pragma: no cover
         assert_with_exit(
             len(gpu_range.split(':')) <= 3,
             'gpu_range must be like x:y:z format,'
             ' which means using gpu in [x, y) with step size z',
         )
         # Set the device.
         avaliable_gpus = list(range(torch.cuda.device_count()))
@@ -256,77 +240,98 @@
             warnings.warn('The GPU ID is not available, use CPU instead.', stacklevel=1)
             gpu_id = None
 
     eg.run(train_grid, num_pool=num_pool, parent_dir=log_dir, gpu_id=gpu_id)
 
     if render:
         try:
-            eg.render(num_episodes=10, render_mode='rgb_array', width=256, height=256)
-        except RuntimeError:
+            eg.render(num_episodes=1, render_mode='rgb_array', width=256, height=256)
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to render model', style='red bold')
+            console.print(Exception, style='red bold')
     if evaluate:
         try:
-            eg.evaluate(num_episodes=10)
-        except RuntimeError:
+            eg.evaluate(num_episodes=1)
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to evaluate model', style='red bold')
+            console.print(Exception, style='red bold')
 
 
 @app.command('eval')
 def evaluate_model(
     result_dir: str = typer.Argument(
         ...,
         help='directory of experiment results to evaluate, e.g. ./runs/PPO-{SafetyPointGoal1-v0}',
     ),
-    num_episode: int = typer.Option(10, help='number of episodes to render'),
-    render: bool = typer.Option(True, help='whether to render'),
+    num_episode: int = typer.Option(
+        10,
+        help='number of episodes to render',
+    ),
+    render: bool = typer.Option(
+        True,
+        help='whether to render',
+    ),
     render_mode: str = typer.Option(
         'rgb_array',
-        help="render mode('human', 'rgb_array', 'rgb_array_list', 'depth_array', 'depth_array_list')",
+        help="render mode ('human', 'rgb_array', 'rgb_array_list', 'depth_array', 'depth_array_list')",
     ),
-    camera_name: str = typer.Option('track', help='camera name to render'),
-    width: int = typer.Option(256, help='width of rendered image'),
-    height: int = typer.Option(256, help='height of rendered image'),
-):
-    """Evaluate a policy which trained by OmniSafe via command line.
-
-    Example:
+    camera_name: str = typer.Option(
+        'track',
+        help='camera name to render',
+    ),
+    width: int = typer.Option(
+        256,
+        help='width of rendered image',
+    ),
+    height: int = typer.Option(
+        256,
+        help='height of rendered image',
+    ),
+) -> None:
+    r"""Evaluate a policy which trained by OmniSafe via command line.
 
-    .. code-block:: bash
+    Examples:
+        .. code-block:: bash
 
-        python -m omnisafe eval --result_dir ./runs/PPOLag-{SafetyPointGoal1-v0} --num_episode 10
-        --render True --render_mode rgb_array --camera_name track --width 256 --height 256
+            python -m omnisafe eval --result_dir ./runs/PPOLag-{SafetyPointGoal1-v0} --num_episode 10 \
+                --render True --render_mode rgb_array --camera_name track --width 256 --height 256
 
     Args:
         result_dir (str): Directory of experiment results to evaluate.
         num_episode (int, optional): Number of episodes to render. Defaults to 10.
         render (bool, optional): Whether to render. Defaults to True.
-        render_mode (str, optional): Render mode('human', 'rgb_array', 'rgb_array_list',
-        'depth_array', 'depth_array_list'). Defaults to 'rgb_array'.
+        render_mode (str, optional): Render mode ('human', 'rgb_array', 'rgb_array_list',
+            'depth_array', 'depth_array_list'). Defaults to 'rgb_array'.
         camera_name (str, optional): Camera name to render. Defaults to 'track'.
         width (int, optional): Width of rendered image. Defaults to 256.
         height (int, optional): Height of rendered image. Defaults to 256.
     """
     evaluator = omnisafe.Evaluator(render_mode=render_mode)
     assert_with_exit(os.path.exists(result_dir), f'path{result_dir}, no torch_save directory')
-    for seed_dir in os.scandir(result_dir):
+
+    scan_result = os.scandir(result_dir)
+    for seed_dir in scan_result:
         if seed_dir.is_dir():
             models_dir = os.path.join(seed_dir.path, 'torch_save')
-            for item in os.scandir(models_dir):
+            scan_models = os.scandir(models_dir)
+            for item in scan_models:
                 if item.is_file() and item.name.split('.')[-1] == 'pt':
                     evaluator.load_saved(
-                        save_dir=seed_dir,
+                        save_dir=seed_dir.path,
                         model_name=item.name,
                         camera_name=camera_name,
                         width=width,
                         height=height,
                     )
                     if render:
                         evaluator.render(num_episodes=num_episode)
                     else:
                         evaluator.evaluate(num_episodes=num_episode)
+            scan_models.close()
+    scan_result.close()
 
 
 @app.command()
 def train_config(
     config_path: str = typer.Argument(
         ...,
         help='path to config file, it is supposed to be yaml file, e.g. ./configs/ppo.yaml',
@@ -340,28 +345,27 @@
         False,
         help='whether to render the trajectory of models saved during training',
     ),
     evaluate: bool = typer.Option(
         False,
         help='whether to evaluate the trajectory of models saved during training',
     ),
-):
-    """Train a policy configured by .yaml file in OmniSafe via command line.
-
-    Example:
+) -> None:
+    r"""Train a policy configured by .yaml file in OmniSafe via command line.
 
-    .. code-block:: bash
+    Examples:
+        .. code-block:: bash
 
-        python -m omnisafe train_config --config_path ./configs/on-policy/PPOLag.yaml --log_dir ./
-        runs
+            python -m omnisafe train_config --config_path ./configs/on-policy/PPOLag.yaml \
+                --log_dir ./runs
 
     Args:
         config_path (str): path to config file, it is supposed to be yaml file.
-        log_dir (str, optional): directory to save logs, default is current directory.
-        Defaults to os.path.join(os.getcwd()).
+        log_dir (str, optional): directory to save logs, default is current directory. Defaults to
+            ``os.path.join(os.getcwd())``.
     """
     assert_with_exit(config_path.endswith('.yaml'), 'config file must be yaml file')
     with open(config_path, encoding='utf-8') as file:
         try:
             args = yaml.load(file, Loader=yaml.FullLoader)  # noqa: S506
             assert args is not None, 'load file error'
         except yaml.YAMLError as exc:
@@ -372,26 +376,29 @@
     args.update({'logger_cfgs': {'log_dir': os.path.join(log_dir, 'train_dict')}})
     agent = omnisafe.Agent(algo=args['algo'], env_id=args['env_id'], custom_cfgs=args)
     agent.learn()
 
     if plot:
         try:
             agent.plot(smooth=1)
-        except RuntimeError:
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to plot data', style='red bold')
+            console.print(Exception, style='red bold')
     if render:
         try:
             agent.render(num_episodes=10, render_mode='rgb_array', width=256, height=256)
-        except RuntimeError:
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to render model', style='red bold')
+            console.print(Exception, style='red bold')
     if evaluate:
         try:
             agent.evaluate(num_episodes=10)
-        except RuntimeError:
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to evaluate model', style='red bold')
+            console.print(Exception, style='red bold')
 
 
 @app.command()
 def analyze_grid(
     path: str = typer.Argument(
         ...,
         help='path of experiment directory, these experiments are launched by omnisafe via experiment grid',
@@ -400,32 +407,45 @@
         ...,
         help='name of parameter to analyze',
     ),
     compare_num: int = typer.Option(
         None,
         help='number of values to compare, if it is specified, will combine any potential combination to compare',
     ),
-    cost_limit: int = typer.Option(
+    cost_limit: float = typer.Option(
         None,
         help='the cost limit to show in graphs by a single line',
     ),
-):
+    show_image: bool = typer.Option(
+        False,
+        help='whether to show the images in GUI windows',
+    ),
+) -> None:
     """Statistics tools for experiment grid.
 
-    Just specify in the name of the parameter of which value you want to compare,
-    then you can just specify how many values you want to compare in single graph at most,
-    and the function will automatically generate all possible combinations of the graph.
-    """
+    Just specify in the name of the parameter of which value you want to compare, then you can just
+    specify how many values you want to compare in single graph at most, and the function will
+    automatically generate all possible combinations of the graph.
 
+    Args:
+        path (str): Path of experiment directory, these experiments are launched by omnisafe via
+            experiment grid.
+        parameter (str): Name of parameter to analyze.
+        compare_num (int): Number of values to compare, if it is specified, will combine any
+            potential combination to compare
+        cost_limit (float): The cost limit.
+        show_image (bool): Whether to show the images in GUI windows.
+    """
     tools = StatisticsTools()
     tools.load_source(path)
 
     tools.draw_graph(
         parameter=parameter,
         values=None,
         compare_num=compare_num,
         cost_limit=cost_limit,
+        show_image=show_image,
     )
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/config.py` & `omnisafe-0.4.0/omnisafe/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 from omnisafe.typing import Activation, ActorType, AdvatageEstimator, InitFunction
 from omnisafe.utils.tools import load_yaml
 
 
 class Config(dict):
     """Config class for storing hyperparameters.
 
-    OmniSafe uses a Config class to store all hyperparameters.
-    OmniSafe store hyperparameters in a yaml file and load them into a Config object.
-    Then the Config class will check the hyperparameters are valid,
-    then pass them to the algorithm class.
+    OmniSafe uses a Config class to store all hyperparameters. OmniSafe store hyperparameters in a
+    yaml file and load them into a Config object. Then the Config class will check the
+    hyperparameters are valid, then pass them to the algorithm class.
 
     Attributes:
         seed (int): Random seed.
         device (str): Device to use for training.
         device_id (int): Device id to use for training.
         wrapper_type (str): Wrapper type.
         epochs (int): Number of epochs.
@@ -75,14 +74,17 @@
         env_name (str): Environment name.
         env_kwargs (dict): Environment keyword arguments.
         normalize_obs (bool): Whether to normalize observation.
         normalize_rew (bool): Whether to normalize reward.
         normalize_cost (bool): Whether to normalize cost.
         max_len (int): Maximum length.
         num_threads (int): Number of threads.
+
+    Args:
+        **kwargs (Any): Keyword arguments to set config.
     """
 
     seed: int
     device: str
     device_id: int
     wrapper_type: str
     epochs: int
@@ -123,15 +125,15 @@
     normalized_rew: bool
     normalized_cost: bool
     normalized_obs: bool
     max_len: int
     num_threads: int
 
     def __init__(self, **kwargs: Any) -> None:
-        """Initialize Config."""
+        """Initialize an instance of :class:`Config`."""
         for key, value in kwargs.items():
             if isinstance(value, dict):
                 self[key] = Config.dict2config(value)
             else:
                 self[key] = value
 
     def __getattr__(self, name: str) -> Any:
@@ -141,48 +143,59 @@
         except KeyError:
             return super().__getattribute__(name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         """Set attribute."""
         self[name] = value
 
-    def todict(self) -> dict:
-        """Convert Config to dictionary."""
-        config_dict = {}
+    def todict(self) -> dict[str, Any]:
+        """Convert Config to dictionary.
+
+        Returns:
+            The dictionary of Config.
+        """
+        config_dict: dict[str, Any] = {}
         for key, value in self.items():
             if isinstance(value, Config):
                 config_dict[key] = value.todict()
             else:
                 config_dict[key] = value
         return config_dict
 
     def tojson(self) -> str:
-        """Convert Config to json string."""
+        """Convert Config to json string.
+
+        Returns:
+            The json string of Config.
+        """
         return json.dumps(self.todict(), indent=4)
 
     @staticmethod
-    def dict2config(config_dict: dict) -> Config:
+    def dict2config(config_dict: dict[str, Any]) -> Config:
         """Convert dictionary to Config.
 
         Args:
-            config_dict (dict): dictionary to be converted.
+            config_dict (dict[str, Any]): The dictionary to be converted.
+
+        Returns:
+            The algorithm config.
         """
         config = Config()
         for key, value in config_dict.items():
             if isinstance(value, dict):
                 config[key] = Config.dict2config(value)
             else:
                 config[key] = value
         return config
 
     def recurisve_update(self, update_args: dict[str, Any]) -> None:
         """Recursively update args.
 
         Args:
-            update_args (Dict[str, Any]): args to be updated.
+            update_args (dict[str, Any]): Args to be updated.
         """
         for key, value in self.items():
             if key in update_args:
                 if isinstance(update_args[key], dict):
                     if isinstance(value, Config):
                         value.recurisve_update(update_args[key])
                         self[key] = value
@@ -205,27 +218,31 @@
     actor_type: ActorType
     actor: ModelConfig
     critic: ModelConfig
     hidden_sizes: list[int]
     activation: Activation
     std: list[float]
     use_obs_encoder: bool
-    lr: float
+    lr: float | None
 
 
 def get_default_kwargs_yaml(algo: str, env_id: str, algo_type: str) -> Config:
     """Get the default kwargs from ``yaml`` file.
 
     .. note::
-        This function search the ``yaml`` file by the algorithm name and environment name.
-        Make sure your new implemented algorithm or environment has the same name as the yaml file.
+        This function search the ``yaml`` file by the algorithm name and environment name. Make
+        sure your new implemented algorithm or environment has the same name as the yaml file.
 
     Args:
-        algo (str): algorithm name.
-        env_id (str): environment name.
+        algo (str): The algorithm name.
+        env_id (str): The environment name.
+        algo_type (str): The algorithm type.
+
+    Returns:
+        The default kwargs.
     """
     path = os.path.dirname(os.path.abspath(__file__))
     cfg_path = os.path.join(path, '..', 'configs', algo_type, f'{algo}.yaml')
     print(f'Loading {algo}.yaml from {cfg_path}')
     kwargs = load_yaml(cfg_path)
     default_kwargs = kwargs['defaults']
     env_spec_kwargs = kwargs[env_id] if env_id in kwargs else None
@@ -240,33 +257,50 @@
 
 def check_all_configs(configs: Config, algo_type: str) -> None:
     """Check all configs.
 
     This function is used to check the configs.
 
     Args:
-        configs (dict): configs to be checked.
-        algo_type (str): algorithm type.
+        configs (Config): The configs to be checked.
+        algo_type (str): The algorithm type.
     """
-
-    ## check algo configs
+    # check algo configs
     __check_algo_configs(configs.algo_cfgs, algo_type)
     __check_logger_configs(configs.logger_cfgs, algo_type)
+    __check_parallel_and_vectorized(configs, algo_type)
+
 
+def __check_parallel_and_vectorized(configs: Config, algo_type: str) -> None:
+    """Check parallel and vectorized configs.
 
-def __check_algo_configs(configs: Config, algo_type) -> None:
-    r"""Check algorithm configs.
+    This function is used to check the parallel and vectorized configs.
+
+    Args:
+        configs (Config): The configs to be checked.
+        algo_type (str): The algorithm type.
+    """
+    if algo_type in {'off-policy', 'model-based'}:
+        assert (
+            configs.train_cfgs.parallel == 1
+        ), 'off-policy or model-based only support parallel==1!'
+    if configs.algo in ['PPOEarlyTerminated', 'TRPOEarlyTerminated']:
+        assert (
+            configs.train_cfgs.vector_env_nums == 1
+        ), 'PPOEarlyTerminated or TRPOEarlyTerminated only support vector_env_nums == 1!'
 
 
+def __check_algo_configs(configs: Config, algo_type: str) -> None:
+    """Check algorithm configs.
+
     This function is used to check the algorithm configs.
 
     .. note::
-
         - ``update_iters`` must be greater than 0 and must be int.
-        - ``update_cycle`` must be greater than 0 and must be int.
+        - ``steps_per_epoch`` must be greater than 0 and must be int.
         - ``batch_size`` must be greater than 0 and must be int.
         - ``target_kl`` must be greater than 0 and must be float.
         - ``entropy_coeff`` must be in [0, 1] and must be float.
         - ``gamma`` must be in [0, 1] and must be float.
         - ``cost_gamma`` must be in [0, 1] and must be float.
         - ``lam`` must be in [0, 1] and must be float.
         - ``lam_c`` must be in [0, 1] and must be float.
@@ -280,24 +314,24 @@
         - ``use_cost`` must be bool.
         - ``max_grad_norm`` must be greater than 0 and must be float.
         - ``adv_estimation_method`` must be in [``gae``, ``v-trace``, ``gae-rtg``, ``plain``].
         - ``standardized_rew_adv`` must be bool.
         - ``standardized_cost_adv`` must be bool.
 
     Args:
-        configs (Config): configs to be checked.
-        algo_type (str): algorithm type.
+        configs (Config): The configs to be checked.
+        algo_type (str): The algorithm type.
     """
     if algo_type == 'on-policy':
         assert (
             isinstance(configs.update_iters, int) and configs.update_iters > 0
         ), 'update_iters must be int and greater than 0'
         assert (
-            isinstance(configs.update_cycle, int) and configs.update_cycle > 0
-        ), 'update_cycle must be int and greater than 0'
+            isinstance(configs.steps_per_epoch, int) and configs.steps_per_epoch > 0
+        ), 'steps_per_epoch must be int and greater than 0'
         assert (
             isinstance(configs.batch_size, int) and configs.batch_size > 0
         ), 'batch_size must be int and greater than 0'
         assert (
             isinstance(configs.target_kl, float) and configs.target_kl >= 0.0
         ), 'target_kl must be float and greater than 0.0'
         assert (
@@ -347,16 +381,21 @@
             isinstance(configs.penalty_coef, float)
             and configs.penalty_coef >= 0.0
             and configs.penalty_coef <= 1.0
         ), 'penalty_coef must be float, and it values must be [0.0, 1.0]'
         assert isinstance(configs.use_cost, bool), 'penalty_coef must be bool'
 
 
-def __check_logger_configs(configs: Config, algo_type) -> None:
-    """Check logger configs."""
+def __check_logger_configs(configs: Config, algo_type: str) -> None:
+    """Check logger configs.
+
+    Args:
+        configs (Config): The configs to be checked.
+        algo_type (str): The algorithm type.
+    """
     if algo_type == 'on-policy':
         assert isinstance(configs.use_wandb, bool) and isinstance(
             configs.wandb_project,
             str,
         ), 'use_wandb and wandb_project must be bool and string'
         assert isinstance(configs.use_tensorboard, bool), 'use_tensorboard must be bool'
         assert isinstance(configs.save_model_freq, int) and isinstance(
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/distributed.py` & `omnisafe-0.4.0/omnisafe/utils/distributed.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""torch.distributed for multi-processing"""
+"""Tools of torch.distributed for multi-processing."""
 
 from __future__ import annotations
 
 import os
 import subprocess
 import sys
 from typing import Any
@@ -24,16 +24,18 @@
 import numpy as np
 import torch
 import torch.distributed as dist
 from torch.distributed import ReduceOp
 
 
 def setup_distributed() -> None:
-    """Avoid slowdowns caused by each separate process's PyTorch,
-    using more than its fair share of CPU resources.
+    """Setup distributed training environment.
+
+    Avoid slowdowns caused by each separate process's PyTorch, using more than its fair share of CPU
+    resources.
     """
     old_num_threads = torch.get_num_threads()
     # decrease number of torch threads for MPI
     if old_num_threads > 1 and world_size() > 1:
         fair_num_threads = max(int(torch.get_num_threads() / world_size()), 1)
         torch.set_num_threads(fair_num_threads)
         print(
@@ -42,136 +44,126 @@
             flush=True,
         )
 
 
 def get_rank() -> int:
     """Get rank of calling process.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> get_rank()
         0
 
+    Returns:
+        The rank of calling process.
     """
     if os.getenv('MASTER_ADDR') is None:
         return 0
     return dist.get_rank()
 
 
-def is_master() -> bool:
-    """Test whether the process is the root process."""
-    return bool(get_rank() == 0)
-
-
 def world_size() -> int:
-    """Count active MPI processes."""
+    """Count active MPI processes.
+
+    Returns:
+        The number of active MPI processes.
+    """
     if os.getenv('MASTER_ADDR') is None:
         return 1
     return dist.get_world_size()
 
 
 reduce = dist.reduce
-allreduce = dist.all_reduce
+all_reduce = dist.all_reduce
 gather = dist.gather
-allgather = dist.all_gather
+all_gather = dist.all_gather
 broadcast = dist.broadcast
 scatter = dist.scatter
 
 
 def fork(
     parallel: int,
-    bind_to_core: bool = False,
-    use_number_of_threads: bool = False,
     device: str = 'cpu',
     manual_args: list[str] | None = None,
 ) -> bool:
     """The entrance of multi-processing.
 
-    Re-launches the current script with workers linked by MPI.
-    Also, terminates the original process that launched it.
-    Taken almost without modification from the Baselines function of the
+    Re-launches the current script with workers linked by MPI. Also, terminates the original process
+    that launched it. Taken almost without modification from the Baselines function of the
     `same name <https://github.com/openai/baselines/blob/master/baselines/common/mpi_fork.py>`_.
 
-    .. note::
-
-        Usage: if ``mpi_fork(n)`` : ``sys.exit()``
-
     Args:
-        parallel (int): number of processes to launch.
-        bind_to_core (bool, optional): Defaults to False.
-        use_number_of_threads (bool, optional): Defaults to False.
+        parallel (int): The number of processes to launch.
+        device (str, optional): The device to be used. Defaults to 'cpu'.
+        manual_args (list of str or None, optional): The arguments to be passed to the new
+            processes. Defaults to None.
     """
     backend = 'gloo' if device == 'cpu' else 'nccl'
     if os.getenv('MASTER_ADDR') is not None and os.getenv('IN_DIST') is None:
         dist.init_process_group(backend=backend)
         os.environ['IN_DIST'] = '1'
     # check if MPI is already setup..
     if parallel > 1 and os.getenv('MASTER_ADDR') is None:
         # MPI is not yet set up: quit parent process and start N child processes
+        os.environ['USE_DISTRIBUTED'] = '1'
         env = os.environ.copy()
         env.update(MKL_NUM_THREADS='1', OMP_NUM_THREADS='1', IN_MPI='1')
         args = [
             'torchrun',
             '--rdzv_backend',
             'c10d',
             '--rdzv_endpoint',
             'localhost:0',
             '--nproc_per_node',
             str(parallel),
         ]
-        if bind_to_core:
-            args += ['-bind-to', 'core']
-        if use_number_of_threads:
-            args += ['--use-hwthread-cpus']
         if manual_args is not None:
             args += manual_args
             print(manual_args)
         else:
             args += sys.argv
             print(sys.argv)
         # this is the parent process, spawn sub-processes..
-        subprocess.check_call(args, env=env)
+        subprocess.check_call(args, env=env)  # noqa: S603
         return True
     return False
 
 
 def avg_tensor(value: torch.Tensor) -> None:
     """Average a torch tensor over MPI processes.
 
-    Since torch and numpy share same memory space,
-    tensors of dim > 0 can be be manipulated through call by reference,
-    scalars must be assigned.
+    Since torch and numpy share same memory space, tensors of dim > 0 can be be manipulated through
+    call by reference, scalars must be assigned.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
         >>> avg_tensor(x)
         >>> x
         tensor(1.5)
 
     Args:
-        value (torch.Tensor): value to be averaged.
+        value (torch.Tensor): The value to be averaged.
     """
     assert isinstance(value, torch.Tensor)
     if world_size() > 1:
         assert len(value.shape) > 0
         avg_x = dist_avg(value)
         value[:] = avg_x[:]
 
 
 def avg_grads(module: torch.nn.Module) -> None:
     """Average contents of gradient buffers across MPI processes.
 
     .. note::
-
         This function only works when the training is multi-processing.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0, requires_grad=True)
         >>> y = x ** 2
         >>> y.backward()
         >>> x.grad
         tensor(2.)
         >>> # In process 1
@@ -181,32 +173,31 @@
         >>> x.grad
         tensor(4.)
         >>> avg_grads(x)
         >>> x.grad
         tensor(3.)
 
     Args:
-        module (torch.nn.Module): module to be averaged.
+        module (torch.nn.Module): The module in which grad need to be averaged.
     """
     if world_size() > 1:
         for parameter in module.parameters():
             if parameter.grad is not None:
                 p_grad = parameter.grad
                 avg_p_grad = dist_avg(parameter.grad)
                 p_grad[:] = avg_p_grad[:]
 
 
 def sync_params(module: torch.nn.Module) -> None:
     """Sync all parameters of module across all MPI processes.
 
     .. note::
-
         This function only works when the training is multi-processing.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> model = torch.nn.Linear(1, 1)
         >>> model.weight.data = torch.tensor([[1.]])
         >>> model.weight.data
         tensor([[1.]])
         >>> # In process 1
         >>> model = torch.nn.Linear(1, 1)
@@ -214,26 +205,26 @@
         >>> model.weight.data
         tensor([[2.]])
         >>> sync_params(model)
         >>> model.weight.data
         tensor([[1.]])
 
     Args:
-        module (torch.nn.Module): module to be synchronized.
+        module (torch.nn.Module): The module to be synchronized.
     """
     if world_size() > 1:
         for parameter in module.parameters():
             p_numpy = parameter.data
             broadcast(p_numpy, src=0)
 
 
 def avg_params(module: torch.nn.Module) -> None:
     """Average contents of all parameters across MPI processes.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> model = torch.nn.Linear(1, 1)
         >>> model.weight.data = torch.tensor([[1.]])
         >>> model.weight.data
         tensor([[1.]])
         >>> # In process 1
         >>> model = torch.nn.Linear(1, 1)
@@ -241,121 +232,146 @@
         >>> model.weight.data
         tensor([[2.]])
         >>> avg_params(model)
         >>> model.weight.data
         tensor([[1.5]])
 
     Args:
-        module (torch.nn.Module): module to be averaged.
+        module (torch.nn.Module): The module in which parameters need to be averaged.
     """
     if world_size() > 1:
         for parameter in module.parameters():
             param_tensor = parameter.data
             avg_param_tensor = dist_avg(param_tensor)
             param_tensor[:] = avg_param_tensor[:]
 
 
 def dist_avg(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
     """Average a tensor over distributed processes.
 
-    Example:
+    Examples:
+        >>> # In process 0
+        >>> x = torch.tensor(1.0)
+        >>> # In process 1
+        >>> x = torch.tensor(2.0)
+        >>> dist_avg(x)
+        tensor(1.5)
 
-    >>> # In process 0
-    >>> x = torch.tensor(1.0)
-    >>> # In process 1
-    >>> x = torch.tensor(2.0)
-    >>> dist_avg(x)
-    tensor(1.5)
+    Args:
+        value (np.ndarray, torch.Tensor, int, or float): value to be averaged.
 
+    Returns:
+        Averaged tensor.
     """
     return dist_sum(value) / world_size()
 
 
 def dist_max(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
     """Determine global maximum of tensor over distributed processes.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
         >>> dist_max(x)
         tensor(2.)
 
+    Args:
+        value (np.ndarray, torch.Tensor, int, or float): value to be find max value.
+
+    Returns:
+        Maximum tensor.
     """
     return dist_op(value, ReduceOp.MAX)
 
 
 def dist_min(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
     """Determine global minimum of tensor over distributed processes.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
         >>> dist_min(x)
         tensor(1.)
 
+    Args:
+        value (np.ndarray, torch.Tensor, int, or float): value to be find min value.
+
+    Returns:
+        Minimum tensor.
     """
     return dist_op(value, ReduceOp.MIN)
 
 
 def dist_sum(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
     """Sum a tensor over distributed processes.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
         >>> dist_sum(x)
         tensor(3.)
 
+    Args:
+        value (np.ndarray, torch.Tensor, int, or float): The value to be summed.
+
+    Returns:
+        Summed tensor.
     """
     return dist_op(value, ReduceOp.SUM)
 
 
 def dist_op(value: np.ndarray | torch.Tensor | int | float, operation: Any) -> torch.Tensor:
     """Multi-processing operation.
 
     .. note::
-
-        The operation can be ``ReduceOp.SUM``, ``ReduceOp.MAX``, ``ReduceOp.MIN``.
-        corresponding to :meth:`mpi_sum`, :meth:`mpi_max`, :meth:`mpi_min`, respectively.
+        The operation can be ``ReduceOp.SUM``, ``ReduceOp.MAX``, ``ReduceOp.MIN``. corresponding to
+        :meth:`dist_sum`, :meth:`dist_max`, :meth:`dist_min`, respectively.
 
     Args:
-        value (torch.Tensor): value to be operated.
+        value (np.ndarray, torch.Tensor, int, or float): The value to be operated.
         operation (ReduceOp): operation type.
+
+    Returns:
+        Operated (SUM, MAX, MIN) tensor.
     """
     if world_size() == 1:
         return torch.as_tensor(value, dtype=torch.float32)
     value_, scalar = ([value], True) if np.isscalar(value) else (value, False)
     value = torch.as_tensor(value_, dtype=torch.float32)
-    allreduce(value, op=operation)
+    all_reduce(value, op=operation)
     return value[0] if scalar else value
 
 
 def dist_statistics_scalar(
     value: torch.Tensor,
     with_min_and_max: bool = False,
 ) -> tuple[torch.Tensor, ...]:
     """Get mean/std and optional min/max of scalar x across MPI processes.
 
-    Example:
+    Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
         >>> dist_statistics_scalar(x)
         (tensor(1.5), tensor(0.5))
 
     Args:
-        value (torch.Tensor): value to be operated.
-        with_min_and_max (bool): whether to return min and max.
+        value (torch.Tensor): Value to be operated.
+        with_min_and_max (bool, optional): whether to return min and max. Defaults to False.
+
+    Returns:
+        The (mean, std) or (mean, std, min, max) of the input tensor, depends on the value of
+        ``with_min_and_max``.
     """
     global_sum = dist_sum(torch.sum(value))
     global_n = dist_sum(len(value))
     mean = global_sum / global_n
 
     global_sum_sq = dist_sum(torch.sum((value - mean) ** 2))
     # compute global std
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/model.py` & `omnisafe-0.4.0/omnisafe/utils/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 # limitations under the License.
 # ==============================================================================
 """This module contains the helper functions for the model."""
 
 from __future__ import annotations
 
 import numpy as np
-import torch
 from torch import nn
 
 from omnisafe.typing import Activation, InitFunction
 
 
 def initialize_layer(init_function: InitFunction, layer: nn.Linear) -> None:
     """Initialize the layer with the given initialization function.
 
-    The ``init_function`` can be chosen from:
-    ``kaiming_uniform``, ``xavier_normal``, ``glorot``,
+    The ``init_function`` can be chosen from: ``kaiming_uniform``, ``xavier_normal``, ``glorot``,
     ``xavier_uniform``, ``orthogonal``.
 
     Args:
         init_function (InitFunction): The initialization function.
         layer (nn.Linear): The layer to be initialized.
     """
     if init_function == 'kaiming_uniform':
@@ -47,19 +45,23 @@
 
 
 def get_activation(
     activation: Activation,
 ) -> type[nn.Identity] | type[nn.ReLU] | type[nn.Sigmoid] | type[nn.Softplus] | type[nn.Tanh]:
     """Get the activation function.
 
-    The ``activation`` can be chosen from:
-    ``identity``, ``relu``, ``sigmoid``, ``softplus``, ``tanh``.
+    The ``activation`` can be chosen from: ``identity``, ``relu``, ``sigmoid``, ``softplus``,
+    ``tanh``.
 
     Args:
         activation (Activation): The activation function.
+
+    Returns:
+        The activation function, ranging from ``nn.Identity``, ``nn.ReLU``, ``nn.Sigmoid``,
+        ``nn.Softplus`` to ``nn.Tanh``.
     """
     activations = {
         'identity': nn.Identity,
         'relu': nn.ReLU,
         'sigmoid': nn.Sigmoid,
         'softplus': nn.Softplus,
         'tanh': nn.Tanh,
@@ -72,70 +74,38 @@
     sizes: list[int],
     activation: Activation,
     output_activation: Activation = 'identity',
     weight_initialization_mode: InitFunction = 'kaiming_uniform',
 ) -> nn.Module:
     """Build the MLP network.
 
-    Example:
+    Examples:
         >>> build_mlp_network([64, 64, 64], 'relu', 'tanh')
         Sequential(
             (0): Linear(in_features=64, out_features=64, bias=True)
             (1): ReLU()
             (2): Linear(in_features=64, out_features=64, bias=True)
             (3): ReLU()
             (4): Linear(in_features=64, out_features=64, bias=True)
             (5): Tanh()
         )
 
     Args:
-        sizes (List[int]): The sizes of the layers.
+        sizes (list of int): The sizes of the layers.
         activation (Activation): The activation function.
-        output_activation (Activation): The output activation function.
-        weight_initialization_mode (InitFunction): The initialization function.
+        output_activation (Activation, optional): The output activation function. Defaults to
+            ``identity``.
+        weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
+            ``'kaiming_uniform'``.
+
+    Returns:
+        The MLP network.
     """
     activation_fn = get_activation(activation)
     output_activation_fn = get_activation(output_activation)
     layers = []
     for j in range(len(sizes) - 1):
         act_fn = activation_fn if j < len(sizes) - 2 else output_activation_fn
         affine_layer = nn.Linear(sizes[j], sizes[j + 1])
         initialize_layer(weight_initialization_mode, affine_layer)
         layers += [affine_layer, act_fn()]
     return nn.Sequential(*layers)
-
-
-def set_optimizer(
-    opt: str,
-    module: nn.Module | list[nn.Parameter],
-    learning_rate: float,
-) -> torch.optim.Optimizer:
-    """Returns an initialized optimizer from PyTorch.
-
-    .. note::
-
-        The optimizer can be chosen from the following list:
-
-        - Adam
-        - AdamW
-        - Adadelta
-        - Adagrad
-        - Adamax
-        - ASGD
-        - LBFGS
-        - RMSprop
-        - Rprop
-        - SGD
-
-    Args:
-        opt (str): optimizer name.
-        module (Union[nn.Module, List[nn.Parameter]]): module or parameters.
-        learning_rate (float): learning rate.
-    """
-    assert hasattr(torch.optim, opt), f'Optimizer={opt} not found in torch.'
-    optimizer = getattr(torch.optim, opt)
-
-    if isinstance(module, list):
-        return optimizer(module, lr=learning_rate)
-    if isinstance(module, nn.Module):
-        return optimizer(module.parameters(), lr=learning_rate)
-    raise TypeError(f'Invalid module type: {type(module)}')
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/plotter.py` & `omnisafe-0.4.0/omnisafe/utils/plotter.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,93 +9,130 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Plotter class for plotting data from experiments."""
+
+from __future__ import annotations
+
 import json
 import os
 import os.path as osp
+from typing import Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
+from pandas import DataFrame
 
 
 class Plotter:
     """Plotter class for plotting data from experiments.
-    Suppose you have run several experiments, with the aim of comparing performance
-    between different algorithms, resulting in a log directory structure of:
+
+    Suppose you have run several experiments, with the aim of comparing performance between
+    different algorithms, resulting in a log directory structure of:
+
+    .. code-block:: text
+
         runs/
-            SafetyAntVelocity-v4/
+            SafetyAntVelocity-v1/
                 CPO/
                     seed0/
                     seed5/
                     seed10/
                 PCPO/
                     seed0/
                     seed5/
                     seed10/
-            SafetyHalfCheetahVelocity-v4/
+            SafetyHalfCheetahVelocity-v1/
                 CPO/
                     seed0/
                     seed5/
                     seed10/
                 PCPO/
                     seed0/
                     seed5/
                     seed10/
-    Example:
-        You can easily produce a graph comparing CPO and PCPO in 'SafetyAntVelocity-v4' with:
-            python plot.py './runs/SafetyAntVelocity-v4/'
+
+    Examples:
+        You can easily produce a graph comparing CPO and PCPO in 'SafetyAntVelocity-v1' with:
+
+        .. code-block:: bash
+
+            python plot.py './runs/SafetyAntVelocity-v1/'
+
+    Attributes:
+        div_line_width (int): The width of the dividing line between subplots.
+        exp_idx (int): The index of the experiment.
+        units (dict[str, Any]): The units of the data.
     """
 
     def __init__(self) -> None:
-        self.div_line_width = 50
-        self.exp_idx = 0
-        self.units = {}
+        """Initialize an instance of :class:`Plotter`."""
+        self.div_line_width: int = 50
+        self.exp_idx: int = 0
+        self.units: dict[str, Any] = {}
 
     def plot_data(
         self,
-        sub_figures,
-        data,
-        xaxis='Steps',
-        value='Rewards',
-        condition='Condition1',
-        smooth=1,
-        **kwargs,
-    ):
-        """Plot data from a pandas dataframe."""
-
-        # smooth data with moving window average.
-        # smoothed_y[t] = average(y[t-k], y[t-k+1], ..., y[t+k-1], y[t+k])
-        # where the "smooth" param is width of that window (2k+1)
+        sub_figures: np.ndarray,
+        data: list[DataFrame],
+        xaxis: str = 'Steps',
+        value: str = 'Rewards',
+        condition: str = 'Condition1',
+        smooth: int = 1,
+        **kwargs: Any,
+    ) -> None:
+        """Plot data from a pandas dataframe.
+
+        .. note::
+            The ``smooth`` means smoothing the data with moving window average.
+
+        Example:
+            >>> smoothed_y[t] = average(y[t-k], y[t-k+1], ..., y[t+k-1], y[t+k])
+
+        where the "smooth" param is width of that window (2k+1)
+
+        Args:
+            sub_figures (np.ndarray): The subplots.
+            data (list of DataFrame): The data to plot.
+            xaxis (str, optional): The x-axis label. Defaults to 'Steps'.
+            value (str, optional): The y-axis label. Defaults to 'Rewards'.
+            condition (str, optional): The condition label. Defaults to 'Condition1'.
+            smooth (int, optional): The smoothing window size. Defaults to 1.
+            **kwargs (Any): Additional arguments.
+        """
         if smooth > 1:
             y = np.ones(smooth)
             for datum in data:
                 x = np.asarray(datum[value])
                 z = np.ones(len(x))
                 smoothed_x = np.convolve(x, y, 'same') / np.convolve(z, y, 'same')
                 datum[value] = smoothed_x
+                x = np.asarray(datum['Costs'])
+                z = np.ones(len(x))
+                smoothed_x = np.convolve(x, y, 'same') / np.convolve(z, y, 'same')
+                datum['Costs'] = smoothed_x
 
         if isinstance(data, list):
-            data = pd.concat(data, ignore_index=True)
+            data_to_plot = pd.concat(data, ignore_index=True)
         sns.lineplot(
-            data=data,
+            data=data_to_plot,
             x=xaxis,
             y='Rewards',
             hue=condition,
             errorbar='sd',
             ax=sub_figures[0],
             **kwargs,
         )
         sns.lineplot(
-            data=data,
+            data=data_to_plot,
             x=xaxis,
             y='Costs',
             hue=condition,
             errorbar='sd',
             ax=sub_figures[1],
             **kwargs,
         )
@@ -115,38 +152,49 @@
             ncol=6,
             handlelength=1,
             mode='expand',
             borderaxespad=0.0,
             prop={'size': 13},
         )
 
-        xscale = np.max(np.asarray(data[xaxis])) > 5e3
+        xscale = np.max(np.asarray(data_to_plot[xaxis], dtype=np.int32)) > 5e3
         if xscale:
             # just some formatting niceness: x-axis scale in scientific notation if max x is large
             plt.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
         plt.tight_layout(pad=0.5)
 
-    def get_datasets(self, logdir, condition=None):
+    def get_datasets(self, logdir: str, condition: str | None = None) -> list[DataFrame]:
         """Recursively look through logdir for files named "progress.txt".
 
         Assumes that any file "progress.txt" is a valid hit.
 
+        Args:
+            logdir (str): The directory to search for progress.txt files
+            condition (str or None, optional): The condition label. Defaults to None.
+
+        Returns:
+            The datasets.
+
+        Raise:
+            FileNotFoundError: If the config file is not found.
+            FileNotFoundError: If could not read from ``progress.csv`` file.
+            ValueError: If no Train/Epoch column in progress.csv.
         """
-        datasets = []
+        datasets: list[DataFrame] = []
         for root, _, files in os.walk(logdir):
             if 'progress.csv' in files:
                 exp_name = None
-                update_cycle = None
+                steps_per_epoch = None
                 try:
                     with open(os.path.join(root, 'config.json'), encoding='utf-8') as f:
                         config = json.load(f)
                         if 'exp_name' in config:
                             exp_name = config['algo']
-                            update_cycle = config['algo_cfgs']['update_cycle']
+                            steps_per_epoch = config['algo_cfgs']['steps_per_epoch']
                 except FileNotFoundError as error:
                     config_path = os.path.join(root, 'config.json')
                     raise FileNotFoundError(f'Could not read from {config_path}') from error
                 condition1 = condition or exp_name or 'exp'
                 condition2 = condition1 + '-' + str(self.exp_idx)
                 self.exp_idx += 1
                 if condition1 not in self.units:
@@ -166,29 +214,46 @@
                     'Metrics/TestEpCost' if 'Metrics/TestEpCost' in exp_data else 'Metrics/EpCost'
                 )
                 exp_data.insert(len(exp_data.columns), 'Unit', unit)
                 exp_data.insert(len(exp_data.columns), 'Condition1', condition1)
                 exp_data.insert(len(exp_data.columns), 'Condition2', condition2)
                 exp_data.insert(len(exp_data.columns), 'Rewards', exp_data[performance])
                 exp_data.insert(len(exp_data.columns), 'Costs', exp_data[cost_performance])
+                epoch = exp_data.get('Train/Epoch')
+                if epoch is None or steps_per_epoch is None:
+                    raise ValueError('No Train/Epoch column in progress.csv')
                 exp_data.insert(
                     len(exp_data.columns),
                     'Steps',
-                    exp_data['Train/Epoch'] * update_cycle,
+                    epoch * steps_per_epoch,
                 )
-
                 datasets.append(exp_data)
         return datasets
 
-    def get_all_datasets(self, all_logdirs, legend=None, select=None, exclude=None):
-        """
-        For every entry in all_logdirs,
-            1) check if the entry is a real directory and if it is, pull data from it;
+    def get_all_datasets(
+        self,
+        all_logdirs: list[str],
+        legend: list[str] | None = None,
+        select: str | None = None,
+        exclude: str | None = None,
+    ) -> list[DataFrame]:
+        """Get all the data from all the log directories.
 
+        For every entry in all_logdirs.
+            1) check if the entry is a real directory and if it is, pull data from it;
             2) if not, check to see if the entry is a prefix for a real directory, and pull data from that.
+
+        Args:
+            all_logdirs (list of str): List of log directories.
+            legend (list of str or None, optional): List of legend names. Defaults to None.
+            select (str or None, optional): Select logdirs that contain this string. Defaults to None.
+            exclude (str or None, optional): Exclude logdirs that contain this string. Defaults to None.
+
+        Returns:
+            All the data stored in a list of DataFrames.
         """
         logdirs = []
         for logdir in all_logdirs:
             if osp.isdir(logdir) and logdir[-1] == os.sep:
                 logdirs += [logdir]
             else:
                 basedir = osp.dirname(logdir)
@@ -221,130 +286,103 @@
             for log, leg in zip(logdirs, legend):
                 data += self.get_datasets(log, leg)
         else:
             for log in logdirs:
                 data += self.get_datasets(log)
         return data
 
+    # pylint: disable-next=too-many-arguments
     def make_plots(
         self,
-        all_logdirs,
-        legend=None,
-        xaxis=None,
-        values=None,
-        count=False,
-        cost_limit=None,
-        smooth=1,
-        select=None,
-        exclude=None,
-        estimator='mean',
-        save_dir='./',
-        save_name=None,
-        save_format='png',
-    ):  # pylint: disable=too-many-arguments
-        """Example usage:
-        Args:
-            logdir (strings): As many log directories (or prefixes to log
-                directories, which the plotter will automatically complete internally) as
-                you'd like to plot from.
-
-            legend (strings): Optional way to specify legend for the plot. The
-                plotter legend will automatically use the ``exp_name`` from the
-                config.json file, unless you tell it otherwise through this flag.
-                This only works if you provide a name for each directory that
-                will get plotted. (Note: this may not be the same as the number
-                of logdir args you provide! Recall that the plotter looks for
-                autocompletes of the logdir args: there may be more than one
-                match for a given logdir prefix, and you will need to provide a
-                legend string for each one of those matches---unless you have
-                removed some of them as candidates via selection or exclusion
-                rules (below).)
-
-            xaxis (string): Pick what column from data is used for the x-axis.
-                Defaults to ``TotalEnvInteracts``.
-
-            value (strings): Pick what columns from data to graph on the y-axis.
-                Submitting multiple values will produce multiple graphs. Defaults
-                to ``Performance``, which is not an actual output of any algorithm.
-                Instead, ``Performance`` refers to either ``AverageEpRet``, the
-                correct performance measure for the on-policy algorithms, or
-                ``AverageTestEpRet``, the correct performance measure for the
-                off-policy algorithms. The plotter will automatically figure out
-                which of ``AverageEpRet`` or ``AverageTestEpRet`` to report for
-                each separate logdir.
-
-            count: Optional flag. By default, the plotter shows y-values which
-                are averaged across all results that share an ``exp_name``,
-                which is typically a set of identical experiments that only vary
-                in random seed. But if you'd like to see all of those curves
-                separately, use the ``--count`` flag.
+        all_logdirs: list[str],
+        legend: list[str] | None = None,
+        xaxis: str = 'Steps',
+        value: str = 'Rewards',
+        count: bool = False,
+        cost_limit: float | None = None,
+        smooth: int = 1,
+        select: str | None = None,
+        exclude: str | None = None,
+        estimator: str = 'mean',
+        save_dir: str = './',
+        save_name: str | None = None,
+        save_format: str = 'png',
+        show_image: bool = False,
+    ) -> None:
+        """Make plots from the data in the specified log directories.
 
-            smooth (int): Smooth data by averaging it over a fixed window. This
-                parameter says how wide the averaging window will be.
-
-            select (strings): Optional selection rule: the plotter will only show
+        Args:
+            all_logdirs (list of str): As many log directories (or prefixes to log directories,
+                which the plotter will automatically complete internally) as you'd like to plot from.
+            legend (list of str or None, optional): Optional way to specify legend for the plot. The
+                plotter legend will automatically use the ``exp_name`` from the config.json file,
+                unless you tell it otherwise through this flag. This only works if you provide a
+                name for each directory that will get plotted. (Note: this may not be the same as
+                the number of logdir args you provide! Recall that the plotter looks for
+                autocompletes of the logdir args: there may be more than one match for a given
+                logdir prefix, and you will need to provide a legend string for each one of those
+                matches--unless you have removed some of them as candidates via selection or
+                exclusion rules (below).)
+            xaxis (str, optional): Pick what column from data is used for the x-axis. Defaults to
+                ``TotalEnvInteracts``.
+            value (str, optional): Pick what columns from data to graph on the y-axis. Submitting
+                multiple values will produce multiple graphs. Defaults to ``Performance``, which is
+                not an actual output of any algorithm. Instead, ``Performance`` refers to either
+                ``AverageEpRet``, the correct performance measure for the on-policy algorithms, or
+                ``AverageTestEpRet``, the correct performance measure for the off-policy algorithms.
+                The plotter will automatically figure out which of ``AverageEpRet`` or
+                ``AverageTestEpRet`` to report for each separate logdir.
+            count (bool, optional): Optional flag. By default, the plotter shows y-values which are
+                averaged across all results that share an ``exp_name``, which is typically a set of
+                identical experiments that only vary in random seed. But if you'd like to see all of
+                those curves separately, use the ``--count`` flag.
+            cost_limit (float or None, optional): Optional way to specify the cost limit of the plot.
+                Defaults to ``None``, which means the plot will not have a cost limit.
+            smooth (int, optional): Smooth data by averaging it over a fixed window. This parameter
+                says how wide the averaging window will be.
+            select (str or None, optional): Optional selection rule: the plotter will only show
                 curves from logdirs that contain all of these sub strings.
-
-            exclude (strings): Optional exclusion rule: plotter will only show
-                curves from logdirs that do not contain these sub strings.
-
+            exclude (str or None, optional): Optional exclusion rule: plotter will only show curves
+                from logdirs that do not contain these sub strings.
+            estimator (str, optional): Optional way to specify how to aggregate data across multiple
+                runs. Defaults to ``mean``.
+            save_dir (str, optional): Optional way to specify where to save the plot. Defaults to
+                ``./``.
+            save_name (str or None, optional): Optional way to specify the name of the plot.
+                Defaults to ``None``, which means the plot will be saved with the name of the first
+                logdir.
+            save_format (str, optional): Optional way to specify the format of the plot. Defaults
+                to ``png``.
+            show_image (bool, optional): Optional flag. If set, the plot will be displayed on screen.
+                Defaults to ``False``.
         """
+        assert xaxis is not None, 'Must specify xaxis'
         data = self.get_all_datasets(all_logdirs, legend, select, exclude)
-        values = values if isinstance(values, list) else [values]
         condition = 'Condition2' if count else 'Condition1'
         # choose what to show on main curve: mean? max? min?
         estimator = getattr(np, estimator)
         sns.set()
-        for value in values:
-            fig, axes = plt.subplots(
-                1,
-                2,
-                figsize=(15, 5),
-            )
-            self.plot_data(
-                axes,
-                data,
-                xaxis=xaxis,
-                value=value,
-                condition=condition,
-                smooth=smooth,
-                estimator=estimator,
-            )
-            if cost_limit:
-                axes[1].axhline(y=cost_limit, ls='--', c='black', linewidth=2)
-        plt.show()
+        fig, axes = plt.subplots(
+            1,
+            2,
+            figsize=(15, 5),
+        )
+        self.plot_data(
+            axes,
+            data,
+            xaxis=xaxis,
+            value=value,
+            condition=condition,
+            smooth=smooth,
+            estimator=estimator,
+        )
+        if cost_limit:
+            axes[1].axhline(y=cost_limit, ls='--', c='black', linewidth=2)
         if save_name is None:
             save_name = all_logdirs[0].split('/')[-1]
+        if show_image:
+            plt.show()
         fig.savefig(
             os.path.join(save_dir, f'{save_name}.{save_format}'),
             bbox_inches='tight',
             pad_inches=0.0,
         )
-
-
-if __name__ == '__main__':
-    import argparse
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--logdir', nargs='*')
-    parser.add_argument('--legend', '-l', nargs='*')
-    parser.add_argument('--xaxis', '-x', default='Steps')
-    parser.add_argument('--value', '-y', default='Rewards', nargs='*')
-    parser.add_argument('--count', action='store_true')
-    parser.add_argument('--smooth', '-s', type=int, default=1)
-    parser.add_argument('--select', nargs='*')
-    parser.add_argument('--exclude', nargs='*')
-    parser.add_argument('--estimator', default='mean')
-    args = parser.parse_args()
-
-    plotter = Plotter()
-    plotter.make_plots(
-        args.logdir,
-        args.legend,
-        args.xaxis,
-        args.value,
-        args.count,
-        smooth=args.smooth,
-        select=args.select,
-        exclude=args.exclude,
-        estimator=args.estimator,
-    )
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/schedule.py` & `omnisafe-0.4.0/omnisafe/utils/schedule.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,76 +9,94 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""helper class to generate scheduling params"""
+"""helper class to generate scheduling params."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Optional, Union
+from typing import Callable
 
 
-def _linear_interpolation(left, right, alpha):
+def _linear_interpolation(left: float, right: float, alpha: float) -> float:
     return left + alpha * (right - left)
 
 
 class Schedule(ABC):
-    """Schedule for a value based on the step"""
+    """Schedule for a value based on the step."""
 
     @abstractmethod
     def value(self, time: int | float) -> int | float:
-        """Value at time t.
-
-        Args:
-            t (float): Time.
-
-        Returns:
-            float: Value at time t.
-        """
+        """Value at time t."""
 
 
 # pylint: disable=too-few-public-methods
 class PiecewiseSchedule(Schedule):
-    """Piece-wise schedule for a value based on the step"""
+    """Piece-wise schedule for a value based on the step, from OpenAI baselines.
+
+    Args:
+        endpoints (list[tuple[int, float]]): List of pairs `(time, value)` meaning that schedule
+            will output `value` when `t==time`. All the values for time must be sorted in an
+            increasing order. When t is between two times, e.g. `(time_a, value_a)` and
+            `(time_b, value_b)`, such that `time_a <= t < time_b` then value outputs is interpolated
+            linearly between `value_a` and `value_b`.
+        outside_value (int or float): Value to use if `t` is before the first time in `endpoints` or
+            after the last one.
+    """
 
     def __init__(
         self,
         endpoints: list[tuple[int, float]],
-        outside_value=Optional[Union[int, float]],
+        outside_value: int | float,
     ) -> None:
-        """From OpenAI baselines"""
+        """Initialize an instance of :class:`PiecewiseSchedule`."""
         idxes = [e[0] for e in endpoints]
         assert idxes == sorted(idxes)
-        self._interpolation = _linear_interpolation
-        self._outside_value = outside_value
-        self._endpoints = endpoints
+        self._interpolation: Callable[[float, float, float], float] = _linear_interpolation
+        self._outside_value: int | float = outside_value
+        self._endpoints: list[tuple[int, float]] = endpoints
 
     def value(self, time: int | float) -> int | float:
         """Value at time t.
 
         Args:
-            t (float): Time.
+            time (int or float): Current time step.
+
+        Returns:
+            The interpolation value at time t or outside_value if t is before the first time in
+            endpoints of after the last one.
+
+        Raises:
+            AssertionError: If the time is not in the endpoints.
         """
         for (left_t, left), (right_t, right) in zip(self._endpoints[:-1], self._endpoints[1:]):
             if left_t <= time < right_t:
                 alpha = float(time - left_t) / (right_t - left_t)
                 return self._interpolation(left, right, alpha)
 
         # t does not belong to any of the pieces, so doom.
         assert self._outside_value is not None
         return self._outside_value
 
 
 class ConstantSchedule(Schedule):
-    """Constant schedule for a value"""
+    """Constant schedule for a value."""
 
-    def __init__(self, value) -> None:
-        """Value remains constant over time."""
-        self._v = value
+    def __init__(self, value: float) -> None:
+        """Initialize an instance of :class:`ConstantSchedule`."""
+        self._v: float = value
 
     def value(self, time: int | float) -> int | float:  # pylint: disable=unused-argument
-        """See Schedule.value"""
+        """Value at time t.
+
+        Args:
+            time (int or float): Current time step.
+
+        Returns:
+            The interpolation value at time t or outside_value if t is before the first time in
+            endpoints of after the last one.
+        """
         return self._v
```

### Comparing `omnisafe-0.3.0/omnisafe/utils/tools.py` & `omnisafe-0.4.0/omnisafe/utils/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,44 +8,57 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""tool_function_packages"""
+"""OmniSafe tools package."""
+
+from __future__ import annotations
 
 import hashlib
 import json
 import os
 import random
 import sys
+from typing import Any
 
 import numpy as np
 import torch
+import torch.backends.cudnn
 import yaml
 from rich.console import Console
+from torch.version import cuda as cuda_version
+
+from omnisafe.typing import DEVICE_CPU
 
 
 def get_flat_params_from(model: torch.nn.Module) -> torch.Tensor:
     """This function is used to get the flattened parameters from the model.
 
     .. note::
-        Some algorithms need to get the flattened parameters from the model,
-        such as the :class:`TRPO` and :class:`CPO` algorithm.
-        In these algorithms, the parameters are flattened and then used to calculate the loss.
+        Some algorithms need to get the flattened parameters from the model, such as the
+        :class:`TRPO` and :class:`CPO` algorithm. In these algorithms, the parameters are flattened
+        and then used to calculate the loss.
 
-    Example:
+    Examples:
         >>> model = torch.nn.Linear(2, 2)
         >>> model.weight.data = torch.tensor([[1.0, 2.0], [3.0, 4.0]])
         >>> get_flat_params_from(model)
         tensor([1., 2., 3., 4.])
 
     Args:
         model (torch.nn.Module): model to be flattened.
+
+    Returns:
+        Flattened parameters.
+
+    Raises:
+        AssertionError: If no gradients were found in model parameters.
     """
     flat_params = []
     for _, param in model.named_parameters():
         if param.requires_grad:
             data = param.data
             data = data.view(-1)  # flatten tensor
             flat_params.append(data)
@@ -53,49 +66,59 @@
     return torch.cat(flat_params)
 
 
 def get_flat_gradients_from(model: torch.nn.Module) -> torch.Tensor:
     """This function is used to get the flattened gradients from the model.
 
     .. note::
-        Some algorithms need to get the flattened gradients from the model,
-        such as the :class:`TRPO` and :class:`CPO` algorithm.
-        In these algorithms, the gradients are flattened and then used to calculate the loss.
+        Some algorithms need to get the flattened gradients from the model, such as the
+        :class:`TRPO` and :class:`CPO` algorithm. In these algorithms, the gradients are flattened
+        and then used to calculate the loss.
 
     Args:
-        model (torch.nn.Module): model to be flattened.
+        model (torch.nn.Module): The model to be flattened.
+
+    Returns:
+        Flattened gradients.
+
+    Raises:
+        AssertionError: If no gradients were found in model parameters.
     """
     grads = []
     for _, param in model.named_parameters():
         if param.requires_grad and param.grad is not None:
             grad = param.grad
             grads.append(grad.view(-1))  # flatten tensor and append
     assert grads, 'No gradients were found in model parameters.'
     return torch.cat(grads)
 
 
 def set_param_values_to_model(model: torch.nn.Module, vals: torch.Tensor) -> None:
     """This function is used to set the parameters to the model.
 
     .. note::
-        Some algorithms (e.g. TRPO, CPO, etc.) need to set the parameters to the model,
-        instead of using the ``optimizer.step()``.
+        Some algorithms (e.g. TRPO, CPO, etc.) need to set the parameters to the model, instead of
+        using the ``optimizer.step()``.
 
-    Example:
+    Examples:
         >>> model = torch.nn.Linear(2, 2)
         >>> model.weight.data = torch.tensor([[1.0, 2.0], [3.0, 4.0]])
         >>> vals = torch.tensor([1.0, 2.0, 3.0, 4.0])
         >>> set_param_values_to_model(model, vals)
         >>> model.weight.data
         tensor([[1., 2.],
                 [3., 4.]])
 
     Args:
-        model (torch.nn.Module): model to be set.
-        vals (torch.Tensor): parameters to be set.
+        model (torch.nn.Module): The model to be set.
+        vals (torch.Tensor): The parameters to be set.
+
+    Raises:
+        AssertionError: If the instance of the parameters is not ``torch.Tensor``, or the lengths of
+            the parameters and the model parameters do not match.
     """
     assert isinstance(vals, torch.Tensor)
     i: int = 0
     for _, param in model.named_parameters():
         if param.requires_grad:  # param has grad and, hence, must be set
             orig_size = param.size()
             size = np.prod(list(param.size()))
@@ -103,57 +126,62 @@
             # set new param values
             new_values = new_values.view(orig_size)
             param.data = new_values
             i += int(size)  # increment array position
     assert i == len(vals), f'Lengths do not match: {i} vs. {len(vals)}'
 
 
-def seed_all(seed: int):
+def seed_all(seed: int) -> None:
     """This function is used to set the random seed for all the packages.
 
     .. hint::
-        To reproduce the results, you need to set the random seed for all the packages.
-        Including ``numpy``, ``random``, ``torch``, ``torch.cuda``, ``torch.backends.cudnn``.
+        To reproduce the results, you need to set the random seed for all the packages. Including
+        ``numpy``, ``random``, ``torch``, ``torch.cuda``, ``torch.backends.cudnn``.
 
     .. warning::
-        If you want to use the ``torch.backends.cudnn.benchmark`` or ``torch.backends.cudnn.
-        deterministic`` and your ``cuda`` version is over 10.2, you need to set the
-        ``CUBLAS_WORKSPACE_CONFIG`` and ``PYTHONHASHSEED`` environment variables.
-    """
+        If you want to use the ``torch.backends.cudnn.benchmark`` or ``torch.backends.cudnn.deterministic``
+        and your ``cuda`` version is over 10.2, you need to set the ``CUBLAS_WORKSPACE_CONFIG`` and
+        ``PYTHONHASHSEED`` environment variables.
 
+    Args:
+        seed (int): The random seed.
+    """
     os.environ['PYTHONHASHSEED'] = str(seed)
 
     random.seed(seed)
     np.random.seed(seed)
 
     torch.manual_seed(seed)
     torch.cuda.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
     try:
         torch.use_deterministic_algorithms(True)
         torch.backends.cudnn.enabled = False
         torch.backends.cudnn.benchmark = False
-        if float(torch.version.cuda) >= 10.2:
+        if cuda_version is not None and float(cuda_version) >= 10.2:
             os.environ['CUBLAS_WORKSPACE_CONFIG'] = ':4096:8'
             os.environ['PYTHONHASHSEED'] = str(seed)
-    except AttributeError:
+    except AttributeError:  # pragma: no cover
         pass
 
 
-def custom_cfgs_to_dict(key_list, value):
+def custom_cfgs_to_dict(key_list: str, value: Any) -> dict[str, Any]:
     """This function is used to convert the custom configurations to dict.
 
     .. note::
-        This function is used to convert the custom configurations to dict.
-        For example, if the custom configurations are ``train_cfgs:use_wandb`` and ``True``,
-        then the output dict will be ``{'train_cfgs': {'use_wandb': True}}``.
+        This function is used to convert the custom configurations to dict. For example, if the
+        custom configurations are ``train_cfgs:use_wandb`` and ``True``, then the output dict will
+        be ``{'train_cfgs': {'use_wandb': True}}``.
 
     Args:
-        key_list (list): list of keys.
-        value: value.
+        key_list (str): list of keys.
+        value (Any): value.
+
+    Returns:
+        The converted dict.
     """
     if value == 'True':
         value = True
     elif value == 'False':
         value = False
     elif '.' in value:
         value = float(value)
@@ -168,104 +196,171 @@
     return_dict = {keys_split[-1]: value}
 
     for key in reversed(keys_split[:-1]):
         return_dict = {key.replace('-', '_'): return_dict}
     return return_dict
 
 
-def update_dict(total_dict, item_dict):
-    """Updater of multi-level dictionary."""
+def update_dict(total_dict: dict[str, Any], item_dict: dict[str, Any]) -> None:
+    """Updater of multi-level dictionary.
+
+    Args:
+        total_dict (dict[str, Any]): The total dictionary.
+        item_dict (dict[str, Any]): The item dictionary.
+
+    Examples:
+        >>> total_dict = {'a': {'b': 1, 'c': 2}}
+        >>> item_dict = {'a': {'b': 3, 'd': 4}}
+        >>> update_dict(total_dict, item_dict)
+        >>> total_dict
+        {'a': {'b': 3, 'c': 2, 'd': 4}}
+    """
     for idd in item_dict:
         total_value = total_dict.get(idd)
         item_value = item_dict.get(idd)
 
         if total_value is None:
             total_dict.update({idd: item_value})
         elif isinstance(item_value, dict):
             update_dict(total_value, item_value)
             total_dict.update({idd: total_value})
         else:
             total_value = item_value
             total_dict.update({idd: total_value})
 
 
-def load_yaml(path) -> dict:
+def load_yaml(path: str) -> dict[str, Any]:
     """Get the default kwargs from ``yaml`` file.
 
     .. note::
-        This function search the ``yaml`` file by the algorithm name and environment name.
-        Make sure your new implemented algorithm or environment has the same name as the yaml file.
+        This function search the ``yaml`` file by the algorithm name and environment name. Make sure
+        your new implemented algorithm or environment has the same name as the yaml file.
 
     Args:
-        path (str): path of the ``yaml`` file.
+        path (str): The path of the ``yaml`` file.
+
+    Returns:
+        The default kwargs.
+
+    Raises:
+        AssertionError: If the ``yaml`` file is not found.
     """
     with open(path, encoding='utf-8') as file:
         try:
             kwargs = yaml.load(file, Loader=yaml.FullLoader)  # noqa: S506
         except yaml.YAMLError as exc:
             raise AssertionError(f'{path} error: {exc}') from exc
 
     return kwargs
 
 
-def recursive_check_config(config, default_config, exclude_keys=()):
+def recursive_check_config(
+    config: dict[str, Any],
+    default_config: dict[str, Any],
+    exclude_keys: tuple[str, ...] = (),
+) -> None:
     """Check whether config is valid in default_config.
 
     Args:
-        config (dict): config to be checked.
-        default_config (dict): default config.
+        config (dict[str, Any]): The config to be checked.
+        default_config (dict[str, Any]): The default config.
+        exclude_keys (tuple of str, optional): The keys to be excluded. Defaults to ().
+
+    Raises:
+        AssertionError: If the type of the value is not the same as the default value.
+        KeyError: If the key is not in default_config.
     """
+    assert isinstance(config, dict), 'custom_cfgs must be a dict!'
     for key in config:
         if key not in default_config.keys() and key not in exclude_keys:
             raise KeyError(f'Invalid key: {key}')
         if isinstance(config[key], dict):
             recursive_check_config(config[key], default_config[key])
 
 
-def assert_with_exit(condition, msg) -> None:
+def assert_with_exit(condition: bool, msg: str) -> None:
     """Assert with message.
 
+    Examples:
+        >>> assert_with_exit(1 == 2, '1 must equal to 2')
+        AssertionError: 1 must equal to 2
+
     Args:
         condition (bool): condition to be checked.
         msg (str): message to be printed.
+
+    Raises:
+        AssertionError: If the condition is not satisfied.
     """
     try:
         assert condition
     except AssertionError:
         console = Console()
         console.print('ERROR: ' + msg, style='bold red')
         sys.exit(1)
 
 
-def recursive_dict2json(dict_obj) -> str:
+def recursive_dict2json(dict_obj: dict[str, Any]) -> str:
     """This function is used to recursively convert the dict to json.
 
     Args:
-        dict_obj (dict): dict to be converted.
+        dict_obj (dict[str, Any]): dict to be converted.
+
+    Returns:
+        The converted json string.
+
+    Raises:
+        AssertionError: If the instance of the input is not ``dict``.
     """
     assert isinstance(dict_obj, dict), 'Input must be a dict.'
-    flat_dict = {}
+    flat_dict: dict[str, Any] = {}
 
-    def _flatten_dict(dict_obj, path=''):
+    def _flatten_dict(dict_obj: dict[str, Any] | Any, path: str = '') -> None:
         if isinstance(dict_obj, dict):
             for key, value in dict_obj.items():
                 _flatten_dict(value, path + key + ':')
         else:
             flat_dict[path[:-1]] = dict_obj
 
     _flatten_dict(dict_obj)
     return json.dumps(flat_dict, sort_keys=True).replace('"', "'")
 
 
-def hash_string(string) -> str:
+def hash_string(string: str) -> str:
     """This function is used to generate the folder name.
 
     Args:
         string (str): string to be hashed.
+
+    Returns:
+        The hashed string.
     """
     salt = b'\xf8\x99/\xe4\xe6J\xd8d\x1a\x9b\x8b\x98\xa2\x1d\xff3*^\\\xb1\xc1:e\x11M=PW\x03\xa5\\h'
     # convert string to bytes and add salt
     salted_string = salt + string.encode('utf-8')
     # use sha256 to hash
     hash_object = hashlib.sha256(salted_string)
     # get the hex digest
     return hash_object.hexdigest()
+
+
+def get_device(device: torch.device | str | int = DEVICE_CPU) -> torch.device:
+    """Retrieve PyTorch device.
+
+    It checks that the requested device is available first. For now, it supports only cpu and cuda.
+    By default, it tries to use the gpu.
+
+    Args:
+        device (torch.device, str, or int, optional): The device to use. Defaults to
+            ``torch.device('cpu')``.
+
+    Returns:
+        The device to use.
+    """
+    # Force conversion to torch.device
+    device = torch.device(device)
+
+    # Cuda not available
+    if not torch.cuda.is_available() and device.type == torch.device('cuda').type:
+        return torch.device('cpu')
+
+    return device
```

### Comparing `omnisafe-0.3.0/omnisafe/version.py` & `omnisafe-0.4.0/omnisafe/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """OmniSafe: A comprehensive and reliable benchmark for safe reinforcement learning."""
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 __license__ = 'Apache License, Version 2.0'
 __author__ = 'OmniSafe Contributors'
 __release__ = True
 
 if not __release__:
     import os
     import subprocess
 
     try:
         prefix, sep, suffix = (
             subprocess.check_output(
-                ['git', 'describe', '--abbrev=7'],
+                ['git', 'describe', '--abbrev=7'],  # noqa: S603,S607
                 cwd=os.path.dirname(os.path.abspath(__file__)),
                 stderr=subprocess.DEVNULL,
                 text=True,
             )
             .strip()
             .lstrip('v')
             .replace('-', '.dev', 1)
```

### Comparing `omnisafe-0.3.0/omnisafe.egg-info/PKG-INFO` & `omnisafe-0.4.0/omnisafe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: omnisafe
-Version: 0.3.0
+Version: 0.4.0
 Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
-Home-page: https://github.com/PKU-MARL/omnisafe
 Author: OmniSafe Contributors
-Author-email: jiamg.ji@gmail.com
 License: Apache License, Version 2.0
-Project-URL: Homepage, https://github.com/PKU-MARL/omnisafe
-Project-URL: Repository, https://github.com/PKU-MARL/omnisafe
+Project-URL: Homepage, https://github.com/OmniSafeAI/omnisafe
+Project-URL: Repository, https://github.com/OmniSafeAI/omnisafe
 Project-URL: Documentation, https://omnisafe.readthedocs.io
-Project-URL: Bug Report, https://github.com/PKU-MARL/omnisafe/issues
+Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
 Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,45 +25,51 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
-  <img src="https://github.com/PKU-MARL/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
+  <img src="https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
 
 <div align="center">
 
-  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/PKU-MARL)
+  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/OmniSafeAI)
   [![PyPI](https://img.shields.io/pypi/v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe)
+  [![tests](https://img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/HEAD/tests)
   [![Documentation Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io)
   [![Downloads](https://static.pepy.tech/personalized-badge/omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/omnisafe)
-  [![GitHub Repo Stars](https://img.shields.io/github/stars/PKU-MARL/omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-MARL/OmniSafe/stargazers)
+  [![GitHub Repo Stars](https://img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)](https://github.com/OmniSafeAI/OmniSafe/stargazers)
   [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-  [![License](https://img.shields.io/github/license/PKU-MARL/OmniSafe?label=license)](#license)
-  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-MARL/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-MARL/omnisafe)
+  [![License](https://img.shields.io/github/license/OmniSafeAI/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/OmniSafeAI/omnisafe)
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/omnisafe/)
 
 </div>
 
 <p align="center">
   <a href="https://omnisafe.readthedocs.io">Documentation</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#installation">Installation</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#getting-started">Getting Started</a> |
-  <a href="https://github.com/PKU-MARL/omnisafe#license">License</a>
+  <a href="https://github.com/OmniSafeAI/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#installation">Installation</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#getting-started">Getting Started</a> |
+  <a href="https://github.com/OmniSafeAI/omnisafe#license">License</a>
 </p>
 
 --------------------------------------------------------------------------------
 
 **This library is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open a GitHub issue or reach out. We'd love to hear about how you're using the library.**
 
-OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms. The field of RL has great potential to benefit society, but safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior. Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
-
-OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment. Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms. By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
+OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms.
+The field of RL has great potential to benefit the society, and safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior.
+Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
+
+OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment.
+Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms.
+By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
 
 --------------------------------------------------------------------------------
 
 ### Table of Contents  <!-- omit in toc --> <!-- markdownlint-disable heading-increment -->
 
 - [Implemented Algorithms](#implemented-algorithms)
   - [Latest SafeRL Papers](#latest-saferl-papers)
@@ -78,19 +82,16 @@
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
   - [Examples](#examples)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
-    - [Important Hints](#important-hints)
-  - [1. Run Agent from preset yaml file](#1-run-agent-from-preset-yaml-file)
-  - [2. Run agent with custom cfg](#2-run-agent-with-custom-cfg)
-  - [3. Run Agent from custom terminal config](#3-run-agent-from-custom-terminal-config)
-  - [4. Evaluate Saved Policy](#4-evaluate-saved-policy)
+  - [Important Hints](#important-hints)
+  - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
 ## Implemented Algorithms
@@ -136,14 +137,16 @@
 #### Model-Based Safe
 
 - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789)
 - [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
 - [X] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
 - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - [ ] **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
+- [X] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
+- [X] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
 
 #### Offline Safe
 
 - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
 - [X] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
 - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003)
 - [ ] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
@@ -160,59 +163,60 @@
 
 ## Installation
 
 ### Prerequisites
 
 OmniSafe requires Python 3.8+ and PyTorch 1.10+.
 
+> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
+
 #### Install from source
 
 ```bash
 # Clone the repo
-git clone https://github.com/PKU-MARL/omnisafe
+git clone https://github.com/OmniSafeAI/omnisafe
 cd omnisafe
 
 # Create a conda environment
-conda create -n omnisafe python=3.8
+conda env create --file conda-recipe.yaml
 conda activate omnisafe
 
 # Install omnisafe
 pip install -e .
 ```
 
 #### Install from PyPI
+
 OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+
 ```bash
 pip install omnisafe
 ```
 
-
 ### Examples
 
 ```bash
 cd examples
 python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
 ```
 
-
 **algo:**
 | Type              | Name                                                             |
 | ----------------- | ---------------------------------------------------------------- |
 | `Base-On-Policy`  | `PolicyGradient, PPO`<br> `NaturalPG, TRPO`                      |
 | `Base-Off-Policy` | `DDPG, TD3, SAC`                                                 |
 | `Naive Lagrange`  | `RCPO, PPOLag, TRPOLag`<br> `DDPGLag, TD3Lag, SACLag`            |
 | `PID Lagrange`    | `CPPOPid, TRPOPid`                                               |
 | `First Order`     | `FOCOPS, CUP`                                                    |
 | `Second Order`    | `SDDPG, CPO, PCPO`                                               |
 | `Saute RL`        | `PPOSaute, PPOLagSaute`                                          |
 | `Simmer RL`       | `PPOSimmerQ, PPOSimmerPid` <br> `PPOLagSimmerQ, PPOLagSimmerPid` |
 | `EarlyTerminated` | `PPOEarlyTerminated` <br> `PPOLagEarlyTerminated`                |
 | `Model-Based`     | `CAP, MBPPOLag, SafeLOOP`                                        |
 
-
 **env-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/), here a list of envs that safety-gymnasium supports.
 
 <table border="1">
 <thead>
   <tr>
     <th>Category</th>
     <th>Task</th>
@@ -236,29 +240,28 @@
   <tr>
     <td>Circle[012]</td>
   </tr>
   <tr>
     <td>Safe Velocity</td>
     <td>Velocity</td>
     <td>HalfCheetah, Hopper, Swimmer, Walker2d, Ant, Humanoid</td>
-    <td>SafetyHumanoidVelocity-v4</td>
+    <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
 More information about environments, please refer to [Safety Gymnasium](https://www.safety-gymnasium.com/)
 
 **parallel:** `Number of parallels`
 
-
 #### Try with CLI
 
 **A video example**
 
-![Segmentfault](https://github.com/PKU-MARL/omnisafe/blob/main/images/CLI_example.svg)
+![Segmentfault](https://github.com/OmniSafeAI/omnisafe/blob/main/images/CLI_example.svg)
 
 ```bash
 pip install omnisafe
 
 omnisafe --help # Ask for help
 
 omnisafe benchmark --help # The benchmark also can be replaced with 'eval', 'train', 'train-config'
@@ -267,94 +270,47 @@
 omnisafe benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml
 
 # Quick evaluating and rendering your trained policy, just specify: 1.path of algorithm which you trained
 omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
 
 # Quick training some algorithms to validate your thoughts
 # Note: use `key1:key2`, your can select key of hyperparameters which are recursively contained, and use `--custom-cfgs`, you can add custom cfgs via CLI
-omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:update_cycle --custom-cfgs 1024
+omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024
 
 # Quick training some algorithms via a saved config file, the format is as same as default format
 omnisafe train-config ./saved_source/train_config.yaml
 ```
 
-
 --------------------------------------------------------------------------------
 
 ## Getting Started
-#### Important Hints
-- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
-### 1. Run Agent from preset yaml file
-
-```python
-import omnisafe
-
-env_id = 'SafetyPointGoal1-v0'
-agent = omnisafe.Agent('PPOLag', env_id)
-agent.learn()
-```
 
-### 2. Run agent with custom cfg
-```python
-import omnisafe
-
-env_id = 'SafetyPointGoal1-v0'
-custom_cfgs = {
-    'train_cfgs': {
-        'total_steps': 1024000,
-        'vector_env_nums': 1,
-        'parallel': 1,
-    },
-    'algo_cfgs': {
-        'update_cycle': 2048,
-        'update_iters': 1,
-    },
-    'logger_cfgs': {
-        'use_wandb': False,
-    },
-}
-agent = omnisafe.Agent('PPOLag', env_id, custom_cfgs=custom_cfgs)
-agent.learn()
-```
-
-### 3. Run Agent from custom terminal config
-
-You can also run agent from a custom terminal config. You can set any config in a corresponding yaml file.
-
-For example, you can run `PPOLag` agent on `SafetyPointGoal1-v0` environment with `total_steps=1024000`, `vector_env_nums=1` and `parallel=1` by:
+### Important Hints
 
-```bash
-cd examples
-python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
-```
-
-### 4. Evaluate Saved Policy
-
-```python
-import os
+- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
 
-import omnisafe
+### Quickstart: Colab on the Cloud
 
+Explore OmniSafe easily and quickly through a series of colab notebooks:
 
-# Just fill your experiment's log directory in here.
-# Such as: ~/omnisafe/runs/SafetyPointGoal1-v0/CPO/seed-000-2022-12-25_14-45-05
-LOG_DIR = ''
+- [Getting Started](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand on it.
+- [CLI Command](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
 
-evaluator = omnisafe.Evaluator()
-for item in os.scandir(os.path.join(LOG_DIR, 'torch_save')):
-    if item.is_file() and item.name.split('.')[-1] == 'pt':
-        evaluator.load_saved_model(save_dir=LOG_DIR, model_name=item.name)
-        evaluator.render(num_episode=10, camera_name='track', width=256, height=256)
-```
+We take great pleasure in collaborating with our users to create tutorials in various languages.
+Please refer to our list of currently supported languages.
+If you are interested in translating the tutorial into a new language or improving an existing version, kindly submit a PR to us.
 
 --------------------------------------------------------------------------------
 
 ## Changelog
-See [CHANGELOG.md](https://github.com/PKU-MARL/omnisafe/blob/main/CHANGELOG.md).
+
+See [CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
 
 ## The OmniSafe Team
 
-OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/PKU-MARL/people/PKU-YYang). Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-MARL/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
+OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-YYang).
+Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
+If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
 
 OmniSafe is released under Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,154 +1,161 @@
-Metadata-Version: 2.1 Name: omnisafe Version: 0.3.0 Summary: A comprehensive
-and reliable benchmark for safe reinforcement learning. Home-page: https://
-github.com/PKU-MARL/omnisafe Author: OmniSafe Contributors Author-email:
-jiamg.ji@gmail.com License: Apache License, Version 2.0 Project-URL: Homepage,
-https://github.com/PKU-MARL/omnisafe Project-URL: Repository, https://
-github.com/PKU-MARL/omnisafe Project-URL: Documentation, https://
-omnisafe.readthedocs.io Project-URL: Bug Report, https://github.com/PKU-MARL/
-omnisafe/issues Keywords: Safe Reinforcement Learning,Reinforcement
-Learning,PyTorch Classifier: Development Status :: 4 - Beta Classifier: License
-:: OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: lint Provides-Extra: test License-
-File: LICENSE
-        [https://github.com/PKU-MARL/omnisafe/raw/HEAD/images/logo.png]
+Metadata-Version: 2.1 Name: omnisafe Version: 0.4.0 Summary: A comprehensive
+and reliable benchmark for safe reinforcement learning. Author: OmniSafe
+Contributors License: Apache License, Version 2.0 Project-URL: Homepage, https:
+//github.com/OmniSafeAI/omnisafe Project-URL: Repository, https://github.com/
+OmniSafeAI/omnisafe Project-URL: Documentation, https://omnisafe.readthedocs.io
+Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
+Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
+Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
+Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: lint Provides-Extra: test License-File: LICENSE
+       [https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png]
 [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)]
-     (https://github.com/PKU-MARL) [![PyPI](https://img.shields.io/pypi/v/
-   omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![Documentation
-Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://
- omnisafe.readthedocs.io) [![Downloads](https://static.pepy.tech/personalized-
-                                    badge/
+    (https://github.com/OmniSafeAI) [![PyPI](https://img.shields.io/pypi/v/
+  omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
+      img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/
+test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/
+   HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
+  omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io) [![Downloads]
+                 (https://static.pepy.tech/personalized-badge/
  omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)]
       (https://pepy.tech/project/omnisafe) [![GitHub Repo Stars](https://
- img.shields.io/github/stars/PKU-MARL/omnisafe?color=brightgreen&logo=github)]
-   (https://github.com/PKU-MARL/OmniSafe/stargazers) [![codestyle](https://
+img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)]
+  (https://github.com/OmniSafeAI/OmniSafe/stargazers) [![codestyle](https://
  img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-      black) [![License](https://img.shields.io/github/license/PKU-MARL/
+     black) [![License](https://img.shields.io/github/license/OmniSafeAI/
 OmniSafe?label=license)](#license) [![CodeCov](https://img.shields.io/codecov/
- c/github/PKU-MARL/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-
-                                MARL/omnisafe)
+  c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/
+   OmniSafeAI/omnisafe) [![Open In Colab](https://colab.research.google.com/
+ assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/
+                                  omnisafe/)
    Documentation | Implemented_Algorithms | Installation | Getting_Started |
                                     License
 -------------------------------------------------------------------------------
 - **This library is currently under heavy development - if you have suggestions
 on the API or use-cases you'd like to be covered, please open a GitHub issue or
 reach out. We'd love to hear about how you're using the library.** OmniSafe is
 an infrastructural framework designed to accelerate safe reinforcement learning
 (RL) research by providing a comprehensive and reliable benchmark for safe RL
-algorithms. The field of RL has great potential to benefit society, but safety
-concerns are a significant issue, and RL algorithms have raised concerns about
-unintended harm or unsafe behavior. Safe RL intends to develop algorithms that
-minimize the risk of unintended harm or unsafe behavior, but there is currently
-a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe addresses
-these issues by providing more than 40 experimentally validated algorithms and
-a sound and efficient simulation environment. Researchers can use OmniSafe to
-conduct experiments and verify their ideas, ensuring consistency and enabling
-more efficient development of safe RL algorithms. By using OmniSafe as a
-benchmark, researchers can evaluate the performance of their own safe RL
-algorithms and contribute to the advancement of safe RL research. -------------
-------------------------------------------------------------------- ### Table
-of Contents   - [Implemented Algorithms](#implemented-algorithms) - [Latest
-SafeRL Papers](#latest-saferl-papers) - [List of Algorithms](#list-of-
-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-Policy Safe](#off-
-policy-safe) - [Model-Based Safe](#model-based-safe) - [Offline Safe](#offline-
-safe) - [Others](#others) - [Installation](#installation) - [Prerequisites]
-(#prerequisites) - [Install from source](#install-from-source) - [Install from
-PyPI](#install-from-pypi) - [Examples](#examples) - [Try with CLI](#try-with-
-cli) - [Getting Started](#getting-started) - [Important Hints](#important-
-hints) - [1. Run Agent from preset yaml file](#1-run-agent-from-preset-yaml-
-file) - [2. Run agent with custom cfg](#2-run-agent-with-custom-cfg) - [3. Run
-Agent from custom terminal config](#3-run-agent-from-custom-terminal-config) -
-[4. Evaluate Saved Policy](#4-evaluate-saved-policy) - [Changelog](#changelog)
-- [The OmniSafe Team](#the-omnisafe-team) - [License](#license) ---------------
------------------------------------------------------------------ ##
-Implemented Algorithms The supported interface algorithms currently include:
-### Latest SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy
-Optimization for Safe Reinforcement Learning (APPO) - **[NeurIPS 2022]**
-[Constrained Update Projection Approach to Safe Policy Optimization (CUP)]
-(https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]** [Effects of Safety
-State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/
-2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning
-via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/
-abs/2210.07573) - **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
-Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- **[ICML 2022]** [Constrained Variational Policy Optimization for Safe
-Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) - **[IJCAI
-2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement
-Learning](https://arxiv.org/abs/2205.11814) - **[ICLR 2022]** [Constrained
-Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) ###
-List of Algorithms #### On-Policy Safe - [X] [The Lagrange version of PPO (PPO-
-Lag)](https://cdn.openai.com/safexp-short.pdf) - [X] [The Lagrange version of
-TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]**
-[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
-achiam17a) - [X] **[ICLR 2019]** [Reward Constrained Policy Optimization
-(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [X] **[ICML 2020]**
-[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
-Lag)](https://arxiv.org/abs/2007.03964) - [X] **[NeurIPS 2020]** [First Order
-Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
-2002.06506) - [X] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
-under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [X] **[ICLR
-2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
-openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML 2021]** [CRPO: A New Approach
-for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
-abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
-for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf)
-#### Off-Policy Safe - [X] The Lagrange version of TD3 (TD3-Lag) - [X] The
-Lagrange version of DDPG (DDPG-Lag) - [X] The Lagrange version of SAC (SAC-Lag)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous
-Control (SDDPG)](https://arxiv.org/abs/1901.10031) - [X] **[ICML 2019]**
-[Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG-
-modular)](https://arxiv.org/abs/1901.10031) - [ ] **[ICML 2022]** [Constrained
+algorithms. The field of RL has great potential to benefit the society, and
+safety concerns are a significant issue, and RL algorithms have raised concerns
+about unintended harm or unsafe behavior. Safe RL intends to develop algorithms
+that minimize the risk of unintended harm or unsafe behavior, but there is
+currently a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe
+addresses these issues by providing more than 40 experimentally validated
+algorithms and a sound and efficient simulation environment. Researchers can
+use OmniSafe to conduct experiments and verify their ideas, ensuring
+consistency and enabling more efficient development of safe RL algorithms. By
+using OmniSafe as a benchmark, researchers can evaluate the performance of
+their own safe RL algorithms and contribute to the advancement of safe RL
+research. ---------------------------------------------------------------------
+----------- ### Table of Contents   - [Implemented Algorithms](#implemented-
+algorithms) - [Latest SafeRL Papers](#latest-saferl-papers) - [List of
+Algorithms](#list-of-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-
+Policy Safe](#off-policy-safe) - [Model-Based Safe](#model-based-safe) -
+[Offline Safe](#offline-safe) - [Others](#others) - [Installation]
+(#installation) - [Prerequisites](#prerequisites) - [Install from source]
+(#install-from-source) - [Install from PyPI](#install-from-pypi) - [Examples]
+(#examples) - [Try with CLI](#try-with-cli) - [Getting Started](#getting-
+started) - [Important Hints](#important-hints) - [Quickstart: Colab on the
+Cloud](#quickstart-colab-on-the-cloud) - [Changelog](#changelog) - [The
+OmniSafe Team](#the-omnisafe-team) - [License](#license) ----------------------
+---------------------------------------------------------- ## Implemented
+Algorithms The supported interface algorithms currently include: ### Latest
+SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe
+Reinforcement Learning (APPO) - **[NeurIPS 2022]** [Constrained Update
+Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/
+2209.07089) - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
+Exploration (Simmer)](https://arxiv.org/abs/2206.02675) - **[NeurIPS 2022]**
+[Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy
+Optimization Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]**
+[SautÃ© RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
+(SauteRL)](https://arxiv.org/abs/2202.06558) - **[ICML 2022]** [Constrained
 Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https:/
-/arxiv.org/abs/2201.11927) #### Model-Based Safe - [ ] **[NeurIPS 2021]** [Safe
-Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
-abs/2202.07789) - [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
-Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]**
-[Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
-(CAP)](https://arxiv.org/abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based
-Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
-Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
-Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) #### Offline Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)]
-(https://arxiv.org/abs/1812.02900) - [X] [The Constrained version of CRR (C-
-CRR)](https://proceedings.neurips.cc/paper/2020/hash/
-588cb956d6bbe67078f29f8de420a13d-Abstract.html) - [ ] **[AAAI 2022]**
-[Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ]
-(https://arxiv.org/abs/2107.09003) - [ ] **[ICLR 2022 (Spotlight)]**
-[COptiDICE: Offline Constrained Reinforcement Learning via Stationary
-Distribution Correction Estimation](https://arxiv.org/abs/
-2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
+/arxiv.org/abs/2201.11927) - **[IJCAI 2022]** [Penalized Proximal Policy
+Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
+- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models
+(LA-MBDA)](https://arxiv.org/abs/2201.09802) - **[AAAI 2022]** [Conservative
+and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https:/
+/arxiv.org/abs/2112.07701) ### List of Algorithms #### On-Policy Safe - [X]
+[The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
+short.pdf) - [X] [The Lagrange version of TRPO (TRPO-Lag)](https://
+cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]** [Constrained Policy
+Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [X] **[ICLR
+2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
+forum?id=SkfrvsA9FX) - [X] **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
+(FOCOPS)](https://arxiv.org/abs/2002.06506) - [X] **[AAAI 2020]** [IPO:
+Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
+abs/1910.09615) - [X] **[ICLR 2020]** [Projection-Based Constrained Policy
+Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML
+2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
+Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
+Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
+arxiv.org/pdf/2205.11814.pdf) #### Off-Policy Safe - [X] The Lagrange version
+of TD3 (TD3-Lag) - [X] The Lagrange version of DDPG (DDPG-Lag) - [X] The
+Lagrange version of SAC (SAC-Lag) - [X] **[ICML 2019]** [Lyapunov-based Safe
+Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/
+1901.10031) - [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for
+Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031) - [ ] **
+[ICML 2022]** [Constrained Variational Policy Optimization for Safe
+Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) #### Model-
+Based Safe - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining
+the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [X] **[CoRL 2021
+(Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://
+arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]** [Conservative and Adaptive
+Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/
+abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement
+Learning via a Constrained Proximal Policy Optimization Algorithm](https://
+arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained Policy
+Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
+2201.09802) - [X] **[ICML 2022 Workshop]** [Constrained Model-based
+Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
+arxiv.org/abs/2010.07968) - [X] **[NeurIPS 2018]** [Constrained Cross-Entropy
+Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
+paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) #### Offline
+Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/
+1812.02900) - [X] [The Constrained version of CRR (C-CRR)](https://
+proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-
+Abstract.html) - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe
+Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003) - [ ] **
+[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement
+Learning via Stationary Distribution Correction Estimation](https://arxiv.org/
+abs/2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
 Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) ####
 Others - [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)]
 (https://arxiv.org/abs/1801.08757) - [ ] **[RA-L 2021]** [Recovery RL: Safe
 Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/
 2010.15920) - [X] **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
 Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
 - [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
 Exploration](https://arxiv.org/abs/2206.02675) --------------------------------
 ------------------------------------------------ ## Installation ###
-Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. #### Install
-from source ```bash # Clone the repo git clone https://github.com/PKU-MARL/
-omnisafe cd omnisafe # Create a conda environment conda create -n omnisafe
-python=3.8 conda activate omnisafe # Install omnisafe pip install -e . ``` ####
-Install from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
-omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
-(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
-omnisafe ``` ### Examples ```bash cd examples python train_policy.py --algo
-PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device
-cpu --vector-env-nums 1 --torch-threads 1 ``` **algo:** | Type | Name | | -----
------------- | ---------------------------------------------------------------
-- | | `Base-On-Policy` | `PolicyGradient, PPO`
+Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
+test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
+versions of macOS. We will accept PRs related to Windows, but do not officially
+support it. #### Install from source ```bash # Clone the repo git clone https:/
+/github.com/OmniSafeAI/omnisafe cd omnisafe # Create a conda environment conda
+env create --file conda-recipe.yaml conda activate omnisafe # Install omnisafe
+pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [![PyPI]
+(https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
+pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
+omnisafe?label=status). ```bash pip install omnisafe ``` ### Examples ```bash
+cd examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 -
+-parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
+threads 1 ``` **algo:** | Type | Name | | ----------------- | -----------------
+----------------------------------------------- | | `Base-On-Policy` |
+`PolicyGradient, PPO`
 `NaturalPG, TRPO` | | `Base-Off-Policy` | `DDPG, TD3, SAC` | | `Naive Lagrange`
 | `RCPO, PPOLag, TRPOLag`
 `DDPGLag, TD3Lag, SACLag` | | `PID Lagrange` | `CPPOPid, TRPOPid` | | `First
 Order` | `FOCOPS, CUP` | | `Second Order` | `SDDPG, CPO, PCPO` | | `Saute RL` |
 `PPOSaute, PPOLagSaute` | | `Simmer RL` | `PPOSimmerQ, PPOSimmerPid`
 `PPOLagSimmerQ, PPOLagSimmerPid` | | `EarlyTerminated` | `PPOEarlyTerminated`
 `PPOLagEarlyTerminated` | | `Model-Based` | `CAP, MBPPOLag, SafeLOOP` | **env-
@@ -157,63 +164,54 @@
  ____________________________________________________________________________
 |Category_______|Task_______|Agent___________________|Example________________|
 |               |Goal[012]__|                        |                       |
 |Safe Navigation|Button[012]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |Push[012]__|                        |                       |
 |_______________|Circle[012]|________________________|_______________________|
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
-|Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v4                     |
+|Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_______________|___________|Humanoid________________|_______________________|
 More information about environments, please refer to [Safety Gymnasium](https:/
 /www.safety-gymnasium.com/) **parallel:** `Number of parallels` #### Try with
-CLI **A video example** ![Segmentfault](https://github.com/PKU-MARL/omnisafe/
+CLI **A video example** ![Segmentfault](https://github.com/OmniSafeAI/omnisafe/
 blob/main/images/CLI_example.svg) ```bash pip install omnisafe omnisafe --help
 # Ask for help omnisafe benchmark --help # The benchmark also can be replaced
 with 'eval', 'train', 'train-config' # Quick benchmarking for your research,
 just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path
 of the config file(refer to omnisafe/examples/benchmarks for format) omnisafe
 benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml # Quick
 evaluating and rendering your trained policy, just specify: 1.path of algorithm
 which you trained omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-
 episode 1 # Quick training some algorithms to validate your thoughts # Note:
 use `key1:key2`, your can select key of hyperparameters which are recursively
 contained, and use `--custom-cfgs`, you can add custom cfgs via CLI omnisafe
 train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs
-algo_cfgs:update_cycle --custom-cfgs 1024 # Quick training some algorithms via
-a saved config file, the format is as same as default format omnisafe train-
-config ./saved_source/train_config.yaml ``` -----------------------------------
---------------------------------------------- ## Getting Started #### Important
-Hints - `train_cfgs:torch_threads` is especially important for training speed,
-and is varying with users' machine, this value shouldn't be too small or too
-large. ### 1. Run Agent from preset yaml file ```python import omnisafe env_id
-= 'SafetyPointGoal1-v0' agent = omnisafe.Agent('PPOLag', env_id) agent.learn()
-``` ### 2. Run agent with custom cfg ```python import omnisafe env_id =
-'SafetyPointGoal1-v0' custom_cfgs = { 'train_cfgs': { 'total_steps': 1024000,
-'vector_env_nums': 1, 'parallel': 1, }, 'algo_cfgs': { 'update_cycle': 2048,
-'update_iters': 1, }, 'logger_cfgs': { 'use_wandb': False, }, } agent =
-omnisafe.Agent('PPOLag', env_id, custom_cfgs=custom_cfgs) agent.learn() ``` ###
-3. Run Agent from custom terminal config You can also run agent from a custom
-terminal config. You can set any config in a corresponding yaml file. For
-example, you can run `PPOLag` agent on `SafetyPointGoal1-v0` environment with
-`total_steps=1024000`, `vector_env_nums=1` and `parallel=1` by: ```bash cd
-examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --
-parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
-threads 1 ``` ### 4. Evaluate Saved Policy ```python import os import omnisafe
-# Just fill your experiment's log directory in here. # Such as: ~/omnisafe/
-runs/SafetyPointGoal1-v0/CPO/seed-000-2022-12-25_14-45-05 LOG_DIR = ''
-evaluator = omnisafe.Evaluator() for item in os.scandir(os.path.join(LOG_DIR,
-'torch_save')): if item.is_file() and item.name.split('.')[-1] == 'pt':
-evaluator.load_saved_model(save_dir=LOG_DIR, model_name=item.name)
-evaluator.render(num_episode=10, camera_name='track', width=256, height=256)
-``` ---------------------------------------------------------------------------
------ ## Changelog See [CHANGELOG.md](https://github.com/PKU-MARL/omnisafe/
-blob/main/CHANGELOG.md). ## The OmniSafe Team OmniSafe is mainly developed by
-the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/
-orgs/PKU-MARL/people/PKU-YYang). Our SafeRL research team members include
-[Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/
-Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://
-github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai
-Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-
-2077). If you have any questions in the process of using omnisafe, don't
-hesitate to ask your questions on [the GitHub issue page](https://github.com/
-PKU-MARL/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
-## License OmniSafe is released under Apache License 2.0.
+algo_cfgs:steps_per_epoch --custom-cfgs 1024 # Quick training some algorithms
+via a saved config file, the format is as same as default format omnisafe
+train-config ./saved_source/train_config.yaml ``` -----------------------------
+--------------------------------------------------- ## Getting Started ###
+Important Hints - `train_cfgs:torch_threads` is especially important for
+training speed, and is varying with users' machine, this value shouldn't be too
+small or too large. ### Quickstart: Colab on the Cloud Explore OmniSafe easily
+and quickly through a series of colab notebooks: - [Getting Started](https://
+colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that
+users can quickly hand on it. - [CLI Command](https://
+colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
+take great pleasure in collaborating with our users to create tutorials in
+various languages. Please refer to our list of currently supported languages.
+If you are interested in translating the tutorial into a new language or
+improving an existing version, kindly submit a PR to us. ----------------------
+---------------------------------------------------------- ## Changelog See
+[CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
+## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research team
+directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-
+YYang). Our SafeRL research team members include [Borong Zhang](https://
+github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https:/
+/github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang
+Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/
+XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any
+questions in the process of using omnisafe, don't hesitate to ask your
+questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/
+issues/new/choose), we will reply to you in 2-3 working days. ## License
+OmniSafe is released under Apache License 2.0.
```

### Comparing `omnisafe-0.3.0/pyproject.toml` & `omnisafe-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,44 +16,39 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    'Intended Audience :: Science/Research',
-    'Topic :: Scientific/Engineering :: Artificial Intelligence',
-    'Topic :: Software Development :: Libraries :: Python Modules',
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "safety-gymnasium >= 0.1.0",
-    "torch >= 1.10.0, < 2.0.0a0",
+    "torch >= 1.10.0",
     "numpy >= 1.20.0",
     "tensorboard >= 2.8.0",
     "wandb >= 0.13.0",
-    "psutil >= 5.9.1",
-    "scipy >= 1.7.0",
-    "joblib >= 1.2.0",
     "pyyaml >= 6.0",
-    "types-pyyaml >= 6.0",
-    "xmltodict >= 0.13.0",
     "moviepy >= 1.0.0",
     "typing-extensions >= 4.0.0",
     "typer[all] >= 0.7.0",
     "seaborn >= 0.12.2",
     "pandas >=  1.5.3",
     "matplotlib >= 3.7.1",
 ]
 dynamic = ["version", "entry-points"]
 
 [project.urls]
-Homepage = "https://github.com/PKU-MARL/omnisafe"
-Repository = "https://github.com/PKU-MARL/omnisafe"
+Homepage = "https://github.com/OmniSafeAI/omnisafe"
+Repository = "https://github.com/OmniSafeAI/omnisafe"
 Documentation = "https://omnisafe.readthedocs.io"
-"Bug Report" = "https://github.com/PKU-MARL/omnisafe/issues"
+"Bug Report" = "https://github.com/OmniSafeAI/omnisafe/issues"
 
 [project.optional-dependencies]
 lint = [
     "isort >= 5.11.0",
     "black >= 22.6.0",
     "pylint[spelling] >= 2.15.0",
     "mypy >= 0.990",
@@ -61,15 +56,21 @@
     "flake8-bugbear",
     "ruff",
     "doc8",
     "pydocstyle",
     "pyenchant",
     "pre-commit",
 ]
-test = ['pytest', 'pytest-cov', 'pytest-xdist']
+test = ["pytest", "pytest-cov", "pytest-xdist"]
+
+[project.scripts]
+omnisafe = "omnisafe.utils.command_app:app"
+
+[tool.setuptools]
+include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["omnisafe", "omnisafe.*"]
 
 # Linter tools #################################################################
 
 [tool.black]
@@ -147,20 +148,14 @@
 ]
 ignore = [
     # E501: line too long
     # W505: doc line too long
     # too long docstring due to long example blocks
     "E501",
     "W505",
-    # TODO: Remove this four ignores
-    # ANN001: missing type annotation for function argument
-    # ANN003: missing type annotation for `**kwargs`
-    # ANN201: missing return type annotation for public function
-    # ANN202: missing return type annotation for private function
-    "ANN001","ANN003","ANN201","ANN202",
     # ANN101: missing type annotation for `self` in method
     # ANN102: missing type annotation for `cls` in classmethod
     "ANN101",
     "ANN102",
     # ANN401: dynamically typed expressions (typing.Any) are disallowed
     "ANN401",
     # S101: use of `assert` detected
```

### Comparing `omnisafe-0.3.0/tests/test_buffer.py` & `omnisafe-0.4.0/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/tests/test_cli.py` & `omnisafe-0.4.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             '--algo',
             'PPO',
             '--total-steps',
             '1024',
             '--vector-env-nums',
             '1',
             '--custom-cfgs',
-            'algo_cfgs:update_cycle',
+            'algo_cfgs:steps_per_epoch',
             '--custom-cfgs',
             '1024',
             '--plot',
             # '--render',
             '--evaluate',
         ],
     )
```

### Comparing `omnisafe-0.3.0/tests/test_model.py` & `omnisafe-0.4.0/tests/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         use_obs_encoder=use_obs_encoder,
     )
     obs = torch.randn(obs_dim, dtype=torch.float32)
     act = torch.randn(act_dim, dtype=torch.float32)
     q_critic = builder.build_critic(critic_type='q')
     v_critic = builder.build_critic(critic_type='v')
     with pytest.raises(NotImplementedError):
-        builder.build_critic(critic_type='invalid')  # type: ignore
+        builder.build_critic(critic_type='invalid')
 
     out1 = q_critic(obs, act)[0]
     out2 = v_critic(obs)[0]
     assert out1.shape == torch.Size([]), f'q_critic output shape is {out1.shape}'
     assert out2.shape == torch.Size([]), f'v_critic output shape is {out2.shape}'
 
 
@@ -89,38 +89,49 @@
         act_space=act_space,
         hidden_sizes=[hidden_sizes, hidden_sizes],
         activation=activation,
     )
     obs = torch.randn(obs_dim, dtype=torch.float32)
     actor_learning = builder.build_actor(actor_type='gaussian_learning')
     actor_sac = builder.build_actor(actor_type='gaussian_sac')
+    actor_mlp = builder.build_actor(actor_type='mlp')
     with pytest.raises(NotImplementedError):
-        builder.build_actor(actor_type='invalid')  # type: ignore
+        builder.build_actor(actor_type='invalid')
 
     _ = actor_learning(obs)
     action = actor_learning.predict(obs, deterministic)
     assert action.shape == torch.Size([act_dim]), f'actor output shape is {action.shape}'
-    lopp = actor_learning.log_prob(action)
-    assert lopp.shape == torch.Size([]), f'actor log_prob shape is {lopp.shape}'
-    actor_learning.std = 0.9  # type: ignore
-    assert (actor_learning.std - 0.9) < 1e-4, f'actor std is {actor_learning.std}'  # type: ignore
+    logp = actor_learning.log_prob(action)
+    assert logp.shape == torch.Size([]), f'actor log_prob shape is {logp.shape}'
+    actor_learning.std = 0.9
+    assert (actor_learning.std - 0.9) < 1e-4, f'actor std is {actor_learning.std}'
 
     _ = actor_sac(obs)
     action = actor_sac.predict(obs, deterministic)
     assert action.shape == torch.Size([act_dim]), f'actor output shape is {action.shape}'
-    lopp = actor_sac.log_prob(action)
-    assert lopp.shape == torch.Size([]), f'actor log_prob shape is {lopp.shape}'
+    logp = actor_sac.log_prob(action)
+    assert logp.shape == torch.Size([]), f'actor log_prob shape is {logp.shape}'
     with pytest.raises(NotImplementedError):
-        actor_sac.std = 0.9  # type: ignore
-    assert isinstance(actor_sac.std, float), f'actor std is {actor_sac.std}'  # type: ignore
+        actor_sac.std = 0.9
+    assert isinstance(actor_sac.std, float), f'actor std is {actor_sac.std}'
+
+    action = actor_mlp.predict(obs, deterministic)
+    actor_mlp.noise = 0.1
+    assert actor_mlp.noise == 0.1, f'actor noise is {actor_mlp.noise}'
+    with pytest.raises(AssertionError):
+        actor_mlp.noise = -0.1
+    with pytest.raises(NotImplementedError):
+        actor_mlp(obs)
+    with pytest.raises(NotImplementedError):
+        actor_mlp.log_prob(action)
 
 
 @helpers.parametrize(
     linear_lr_decay=[True, False],
-    lr=['None', 1e-3],
+    lr=[None, 1e-3],
 )
 def test_actor_critic(
     linear_lr_decay: bool,
     lr,
 ):
     """Test actor critic."""
     obs_dim = 10
```

### Comparing `omnisafe-0.3.0/tests/test_normalizer.py` & `omnisafe-0.4.0/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/tests/test_statistics_tools.py` & `omnisafe-0.4.0/tests/test_statistics_tools.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.3.0/tests/test_utils.py` & `omnisafe-0.4.0/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,46 +12,76 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Test utils"""
 
 from __future__ import annotations
 
-import os
-import sys
-
 import pytest
 import torch
 from torch import nn
 from torch.distributions import Normal
 
 import helpers
-import omnisafe
 from omnisafe.common.experiment_grid import ExperimentGrid
 from omnisafe.typing import Activation, InitFunction
 from omnisafe.utils.config import Config, check_all_configs, get_default_kwargs_yaml
 from omnisafe.utils.distributed import fork
+from omnisafe.utils.exp_grid_tools import train
 from omnisafe.utils.math import (
     SafeTanhTransformer,
     TanhNormal,
     discount_cumsum,
     get_diagonal,
     get_transpose,
 )
 from omnisafe.utils.model import get_activation, initialize_layer
 from omnisafe.utils.schedule import ConstantSchedule, PiecewiseSchedule
+from omnisafe.utils.tools import assert_with_exit, custom_cfgs_to_dict, update_dict
+
+
+def test_update_dict():
+    d = {'a': 1, 'b': {'c': 2}}
+    update_dict(d, {'a': 2, 'b': {'d': 3}, 'e': {'f': 4}})
+    assert d == {'a': 2, 'b': {'c': 2, 'd': 3}, 'e': {'f': 4}}
+
+
+def test_assert_with_exit():
+    with pytest.raises(SystemExit):
+        assert_with_exit(False, 'test')
+
+
+def test_custom_cfgs_to_dict():
+    unparsed_args = {
+        'str': 'PPOLag',
+        'str_true': 'True',
+        'str_false': 'False',
+        'float': '1.0',
+        'digit': '2',
+        'list': '[a,b,c]',
+    }
+    custom_cfgs = {}
+    for k, v in unparsed_args.items():
+        update_dict(custom_cfgs, custom_cfgs_to_dict(k, v))
+    print(custom_cfgs)
+    assert custom_cfgs['str'] == unparsed_args['str']
+    assert custom_cfgs['str_true'] is True
+    assert custom_cfgs['str_false'] is False
+    assert custom_cfgs['float'] == float(unparsed_args['float'])
+    assert custom_cfgs['digit'] == int(unparsed_args['digit'])
+    assert custom_cfgs['list'] == ['a', 'b', 'c']
 
 
 def test_config():
     """Test config"""
     cfg = Config(a=1, b={'c': 2})
     cfg.a = 2
     cfg.recurisve_update({'a': {'d': 3}, 'e': {'f': 4}})
-
     cfg = get_default_kwargs_yaml('PPO', 'Simple-v0', 'on-policy')
+    cfg.recurisve_update({'exp_name': 'test_configs', 'env_id': 'Simple-v0', 'algo': 'PPO'})
     check_all_configs(cfg, 'on-policy')
 
 
 def test_distributed():
     fork(parallel=2, manual_args=['distribution_train.py'])
 
 
@@ -98,78 +128,40 @@
 
     random_tensor = torch.clamp(random_tensor, -0.999999, 0.999999)
     tanh = SafeTanhTransformer()
     assert torch.allclose(tanh(random_tensor), torch.tanh(random_tensor))
     assert torch.allclose(tanh.inv(random_tensor), torch.atanh(random_tensor))
 
 
-def train(
-    exp_id: str,
-    algo: str,
-    env_id: str,
-    custom_cfgs: Config,
-    num_threads: int = 6,
-) -> tuple[float, float, float]:
-    """Train a policy from exp-x config with OmniSafe.
-    Args:
-        exp_id (str): Experiment ID.
-        algo (str): Algorithm to train.
-        env_id (str): The name of test environment.
-        custom_cfgs (NamedTuple): Custom configurations.
-        num_threads (int, optional): Number of threads. Defaults to 6.
-    """
-    torch.set_num_threads(num_threads)
-    sys.stdout = sys.__stdout__
-    sys.stderr = sys.__stderr__
-    print(f'exp-x: {exp_id} is training...')
-    USE_REDIRECTION = True
-    if USE_REDIRECTION:
-        if not os.path.exists(custom_cfgs['data_dir']):
-            os.makedirs(custom_cfgs['data_dir'], exist_ok=True)
-        sys.stdout = open(  # noqa: SIM115
-            f'{custom_cfgs["data_dir"]}terminal.log',
-            'w',
-            encoding='utf-8',
-        )
-        sys.stderr = open(  # noqa: SIM115
-            f'{custom_cfgs["data_dir"]}error.log',
-            'w',
-            encoding='utf-8',
-        )
-    agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
-    reward, cost, ep_len = agent.learn()
-    return reward, cost, ep_len
-
-
 def test_train(
     exp_name='make_test_exp_grid',
     algo='CPO',
-    env_id='SafetyHalfCheetahVelocity-v4',
+    env_id='SafetyHalfCheetahVelocity-v1',
 ):
     """Test train."""
     eg = ExperimentGrid(exp_name=exp_name)
     eg.add('algo', [algo])
     eg.add('env_id', [env_id])
     eg.add('logger_cfgs:use_wandb', [False])
-    eg.add('algo_cfgs:update_cycle', [512])
+    eg.add('algo_cfgs:steps_per_epoch', [512])
     eg.add('train_cfgs:total_steps', [1024, 2048])
     eg.add('train_cfgs:vector_env_nums', [1])
     eg.run(train, num_pool=1, is_test=True)
 
 
 @helpers.parametrize(
     init_function=['kaiming_uniform', 'xavier_normal', 'glorot', 'xavier_uniform', 'orthogonal'],
 )
 def test_initalize(init_function: InitFunction):
     """Test initialize."""
     layer = nn.Linear(3, 3)
     initialize_layer(init_function=init_function, layer=layer)
 
     with pytest.raises(TypeError) as e:
-        initialize_layer(init_function='test', layer=layer)  # type: ignore
+        initialize_layer(init_function='test', layer=layer)
     assert e.value.args[0] == 'Invalid initialization function: test'
 
 
 @helpers.parametrize(activations=['identity', 'relu', 'sigmoid', 'softplus', 'tanh'])
 def test_get_activation(activations: Activation):
     """Test get_activation."""
     get_activation(activations)
```


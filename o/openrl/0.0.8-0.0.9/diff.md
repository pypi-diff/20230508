# Comparing `tmp/openrl-0.0.8.tar.gz` & `tmp/openrl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrl-0.0.8.tar", last modified: Sat May  6 12:05:19 2023, max compression
+gzip compressed data, was "openrl-0.0.9.tar", last modified: Mon May  8 11:19:00 2023, max compression
```

## Comparing `openrl-0.0.8.tar` & `openrl-0.0.9.tar`

### file list

```diff
@@ -1,174 +1,175 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.866665 openrl-0.0.8/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.8/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.8/LICENSE.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)    13317 2023-05-06 12:05:19.866443 openrl-0.0.8/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)    12168 2023-05-06 12:04:43.000000 openrl-0.0.8/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.838034 openrl-0.0.8/openrl/
--rw-r--r--   0 4paradigm   (501) staff       (20)      371 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.839690 openrl-0.0.8/openrl/algorithms/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/algorithms/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/algorithms/base_algorithm.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/algorithms/ppo.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.840782 openrl-0.0.8/openrl/buffers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/normal_buffer.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/buffers/replay_data.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.842390 openrl-0.0.8/openrl/buffers/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/utils/obs_data.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.843063 openrl-0.0.8/openrl/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/cli/train.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.843432 openrl-0.0.8/openrl/configs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/configs/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/configs/config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.844701 openrl-0.0.8/openrl/drivers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/drivers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/drivers/base_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/drivers/onpolicy_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/drivers/rl_driver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.844985 openrl-0.0.8/openrl/envs/
--rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.845518 openrl-0.0.8/openrl/envs/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/common/build_envs.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/common/registration.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.845755 openrl-0.0.8/openrl/envs/gymnasium/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.8/openrl/envs/gymnasium/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.847878 openrl-0.0.8/openrl/envs/mpe/
--rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/mpe_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/multi_discrete.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/multiagent_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/rendering.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/scenario.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.848290 openrl-0.0.8/openrl/envs/mpe/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/scenarios/simple_spread.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.848965 openrl-0.0.8/openrl/envs/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/nlp/daily_dialog_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/nlp_env.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.850316 openrl-0.0.8/openrl/envs/nlp/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/custom_text_generation_pools.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/distribution.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/evaluation_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.850624 openrl-0.0.8/openrl/envs/nlp/utils/metrics/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/metrics/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/metrics/meteor.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/observation.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/sampler.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/text_generation_pool.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.851426 openrl-0.0.8/openrl/envs/vec_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/async_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/base_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/sync_venv.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.852262 openrl-0.0.8/openrl/envs/vec_env/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/utils/numpy_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/utils/share_memory.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.852982 openrl-0.0.8/openrl/envs/vec_env/vec_info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/base_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/nlp_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1221 2023-05-04 10:32:54.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/simple_vec_info.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.853959 openrl-0.0.8/openrl/envs/vec_env/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2227 2023-05-04 10:32:54.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/reward_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.854802 openrl-0.0.8/openrl/envs/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/extra_wrappers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/multiagent_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.855783 openrl-0.0.8/openrl/modules/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/base_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.856353 openrl-0.0.8/openrl/modules/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/common/base_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3441 2023-04-28 09:15:51.000000 openrl-0.0.8/openrl/modules/common/ppo_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/model_config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.857615 openrl-0.0.8/openrl/modules/networks/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/base_policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/base_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/policy_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/modules/networks/policy_value_network_gpt.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.859879 openrl-0.0.8/openrl/modules/networks/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/attention.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/cnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/distributed_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/distributions.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/mix.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/mlp.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.860560 openrl-0.0.8/openrl/modules/networks/utils/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/base_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/causal_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/hf_generation_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/popart.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/rnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/transformer_act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/ppo_module.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/rl_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.862167 openrl-0.0.8/openrl/modules/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/utils/valuenorm.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.862761 openrl-0.0.8/openrl/rewards/
--rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/rewards/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      570 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/rewards/base_reward.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/rewards/nlp_reward.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.863041 openrl-0.0.8/openrl/runners/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/runners/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.863805 openrl-0.0.8/openrl/runners/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      188 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/runners/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/runners/common/base_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4024 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/runners/common/chat_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6067 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/runners/common/ppo_agent.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864040 openrl-0.0.8/openrl/supports/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864175 openrl-0.0.8/openrl/supports/opendata/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opendata/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864457 openrl-0.0.8/openrl/supports/opendata/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opendata/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opendata/utils/opendata_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864980 openrl-0.0.8/openrl/supports/opengpu/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opengpu/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4184 2023-05-04 10:32:54.000000 openrl-0.0.8/openrl/supports/opengpu/gpu_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7114 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/supports/opengpu/manager.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.865417 openrl-0.0.8/openrl/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.839014 openrl-0.0.8/openrl.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)    13317 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     4554 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      278 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-05-06 12:05:19.866704 openrl-0.0.8/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     3149 2023-05-06 12:04:43.000000 openrl-0.0.8/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.865592 openrl-0.0.8/tests/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.865898 openrl-0.0.8/tests/project/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/project/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/project/test_version.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.866200 openrl-0.0.8/tests/test_buffer/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/test_buffer/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/test_buffer/test_buffer.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.192651 openrl-0.0.9/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.9/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.9/LICENSE.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)    13540 2023-05-08 11:19:00.192202 openrl-0.0.9/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)    12391 2023-05-08 11:10:58.000000 openrl-0.0.9/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.143714 openrl-0.0.9/openrl/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      425 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.146210 openrl-0.0.9/openrl/algorithms/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/algorithms/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/algorithms/base_algorithm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/algorithms/ppo.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.147665 openrl-0.0.9/openrl/buffers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/normal_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/buffers/replay_data.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.149771 openrl-0.0.9/openrl/buffers/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/utils/obs_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.151417 openrl-0.0.9/openrl/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/cli/train.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.152020 openrl-0.0.9/openrl/configs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/configs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/configs/config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.154729 openrl-0.0.9/openrl/drivers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/drivers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/drivers/base_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/drivers/onpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/drivers/rl_driver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.155191 openrl-0.0.9/openrl/envs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.156324 openrl-0.0.9/openrl/envs/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/common/build_envs.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/common/registration.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.156937 openrl-0.0.9/openrl/envs/gymnasium/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.9/openrl/envs/gymnasium/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.160596 openrl-0.0.9/openrl/envs/mpe/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/mpe_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/multi_discrete.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/multiagent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/rendering.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/scenario.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.161044 openrl-0.0.9/openrl/envs/mpe/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/scenarios/simple_spread.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.161788 openrl-0.0.9/openrl/envs/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/nlp/daily_dialog_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/nlp_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.163348 openrl-0.0.9/openrl/envs/nlp/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/custom_text_generation_pools.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/distribution.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/evaluation_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.163853 openrl-0.0.9/openrl/envs/nlp/utils/metrics/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/metrics/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/metrics/meteor.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/observation.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/sampler.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/text_generation_pool.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.165249 openrl-0.0.9/openrl/envs/vec_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/async_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8061 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/envs/vec_env/base_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/sync_venv.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.167122 openrl-0.0.9/openrl/envs/vec_env/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/vec_env/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/utils/numpy_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/utils/share_memory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/vec_env/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.169258 openrl-0.0.9/openrl/envs/vec_env/vec_info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/base_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/nlp_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1221 2023-05-04 10:32:54.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/simple_vec_info.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.170356 openrl-0.0.9/openrl/envs/vec_env/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2227 2023-05-04 10:32:54.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/reward_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.172264 openrl-0.0.9/openrl/envs/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/extra_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/multiagent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.174284 openrl-0.0.9/openrl/modules/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/base_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.175409 openrl-0.0.9/openrl/modules/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/common/base_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3456 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/modules/common/ppo_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/model_config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.176931 openrl-0.0.9/openrl/modules/networks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/base_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/base_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/policy_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/modules/networks/policy_value_network_gpt.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.180223 openrl-0.0.9/openrl/modules/networks/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/attention.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/cnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/distributed_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/distributions.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/mix.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/mlp.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.181617 openrl-0.0.9/openrl/modules/networks/utils/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/base_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/causal_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/hf_generation_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/popart.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/rnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/transformer_act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/ppo_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/rl_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.183328 openrl-0.0.9/openrl/modules/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/utils/valuenorm.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.185098 openrl-0.0.9/openrl/rewards/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/rewards/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      570 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/rewards/base_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/rewards/nlp_reward.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.185717 openrl-0.0.9/openrl/runners/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/runners/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.187769 openrl-0.0.9/openrl/runners/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      188 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/runners/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/runners/common/base_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4024 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/runners/common/chat_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2849 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/runners/common/ppo_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4596 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/runners/common/rl_agent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.188247 openrl-0.0.9/openrl/supports/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.188575 openrl-0.0.9/openrl/supports/opendata/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opendata/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.189206 openrl-0.0.9/openrl/supports/opendata/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opendata/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opendata/utils/opendata_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.190217 openrl-0.0.9/openrl/supports/opengpu/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opengpu/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4184 2023-05-04 10:32:54.000000 openrl-0.0.9/openrl/supports/opengpu/gpu_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7114 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/supports/opengpu/manager.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191038 openrl-0.0.9/openrl/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.145386 openrl-0.0.9/openrl.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    13540 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4588 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      278 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-05-08 11:19:00.192706 openrl-0.0.9/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3149 2023-05-06 12:04:43.000000 openrl-0.0.9/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191221 openrl-0.0.9/tests/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191581 openrl-0.0.9/tests/project/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/project/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/project/test_version.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191945 openrl-0.0.9/tests/test_buffer/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/test_buffer/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/test_buffer/test_buffer.py
```

### Comparing `openrl-0.0.8/LICENSE` & `openrl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/LICENSE.txt` & `openrl-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/PKG-INFO` & `openrl-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.8
+Version: 0.0.9
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -49,15 +49,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.8 is updated on May 4, 2023 
+OpenRL-v0.0.9 is updated on May 6, 2023 
 
 The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
@@ -120,18 +120,21 @@
 ```
 
 安装完成后，用户可以直接通过命令行查看OpenRL的版本：
 ```bash
 openrl --version
 ```
 
+**Tips**：无需安装，通过Colab在线试用OpenRL: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
+
 ## 使用Docker
 
 OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
 如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+
 ```bash
 sudo docker pull openrllab/openrl-cpu
 ```
 
 如果用户想要通过显卡加速训练，则可以通过以下命令获取：
 ```bash
 sudo docker pull openrllab/openrl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.8 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.0.9 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
@@ -40,15 +40,15 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.8 is updated on May 4, 2023
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.9 is updated on May 6, 2023
 The main branch is the latest version of OpenRL, which is under active
 development. If you just want to have a try with OpenRL, you can switch to the
 stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
 (https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
 openrl-docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
@@ -82,15 +82,19 @@
 [Acknowledgments](#acknowledgments) ## å®è£
 ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
 æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
 https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ``` ## ä½¿ç¨Docker
+```bash openrl --version ```
+**Tips**ï¼æ éå®è£ï¼éè¿Colabå¨çº¿è¯ç¨OpenRL: [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
+## ä½¿ç¨Docker
 OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
 å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
 ```bash sudo docker pull openrllab/openrl-cpu ```
 å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
 ```bash sudo docker pull openrllab/openrl ```
 éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
 ```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
```

### Comparing `openrl-0.0.8/README.md` & `openrl-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.8 is updated on May 4, 2023 
+OpenRL-v0.0.9 is updated on May 6, 2023 
 
 The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
@@ -93,18 +93,21 @@
 ```
 
 安装完成后，用户可以直接通过命令行查看OpenRL的版本：
 ```bash
 openrl --version
 ```
 
+**Tips**：无需安装，通过Colab在线试用OpenRL: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
+
 ## 使用Docker
 
 OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
 如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+
 ```bash
 sudo docker pull openrllab/openrl-cpu
 ```
 
 如果用户想要通过显卡加速训练，则可以通过以下命令获取：
 ```bash
 sudo docker pull openrllab/openrl
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.8 is updated on May 4, 2023
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.9 is updated on May 6, 2023
 The main branch is the latest version of OpenRL, which is under active
 development. If you just want to have a try with OpenRL, you can switch to the
 stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
 (https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
 openrl-docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
@@ -66,15 +66,19 @@
 [Acknowledgments](#acknowledgments) ## å®è£
 ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
 æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
 https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ``` ## ä½¿ç¨Docker
+```bash openrl --version ```
+**Tips**ï¼æ éå®è£ï¼éè¿Colabå¨çº¿è¯ç¨OpenRL: [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
+## ä½¿ç¨Docker
 OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
 å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
 ```bash sudo docker pull openrllab/openrl-cpu ```
 å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
 ```bash sudo docker pull openrllab/openrl ```
 éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
 ```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
```

### Comparing `openrl-0.0.8/openrl/algorithms/__init__.py` & `openrl-0.0.9/openrl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/algorithms/base_algorithm.py` & `openrl-0.0.9/openrl/algorithms/base_algorithm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/algorithms/ppo.py` & `openrl-0.0.9/openrl/algorithms/ppo.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/buffers/__init__.py` & `openrl-0.0.9/openrl/buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/buffers/normal_buffer.py` & `openrl-0.0.9/openrl/buffers/normal_buffer.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/buffers/replay_data.py` & `openrl-0.0.9/openrl/buffers/replay_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/buffers/utils/__init__.py` & `openrl-0.0.9/openrl/buffers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/buffers/utils/obs_data.py` & `openrl-0.0.9/openrl/buffers/utils/obs_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/buffers/utils/util.py` & `openrl-0.0.9/openrl/buffers/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/cli/__init__.py` & `openrl-0.0.9/openrl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/cli/cli.py` & `openrl-0.0.9/openrl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/cli/train.py` & `openrl-0.0.9/openrl/cli/train.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/configs/__init__.py` & `openrl-0.0.9/openrl/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/configs/config.py` & `openrl-0.0.9/openrl/configs/config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/drivers/__init__.py` & `openrl-0.0.9/openrl/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/drivers/onpolicy_driver.py` & `openrl-0.0.9/openrl/drivers/onpolicy_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/drivers/rl_driver.py` & `openrl-0.0.9/openrl/drivers/rl_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/common/__init__.py` & `openrl-0.0.9/openrl/envs/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/common/build_envs.py` & `openrl-0.0.9/openrl/envs/common/build_envs.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/common/registration.py` & `openrl-0.0.9/openrl/envs/common/registration.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/gymnasium/__init__.py` & `openrl-0.0.9/openrl/envs/gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/mpe/__init__.py` & `openrl-0.0.9/openrl/envs/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/mpe/core.py` & `openrl-0.0.9/openrl/envs/mpe/core.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/mpe/mpe_env.py` & `openrl-0.0.9/openrl/envs/mpe/mpe_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/mpe/multi_discrete.py` & `openrl-0.0.9/openrl/envs/mpe/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/mpe/multiagent_env.py` & `openrl-0.0.9/openrl/envs/mpe/multiagent_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/mpe/rendering.py` & `openrl-0.0.9/openrl/envs/mpe/rendering.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/mpe/scenarios/simple_spread.py` & `openrl-0.0.9/openrl/envs/mpe/scenarios/simple_spread.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/__init__.py` & `openrl-0.0.9/openrl/envs/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/daily_dialog_env.py` & `openrl-0.0.9/openrl/envs/nlp/daily_dialog_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/custom_text_generation_pools.py` & `openrl-0.0.9/openrl/envs/nlp/utils/custom_text_generation_pools.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/distribution.py` & `openrl-0.0.9/openrl/envs/nlp/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/evaluation_utils.py` & `openrl-0.0.9/openrl/envs/nlp/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/metrics/__init__.py` & `openrl-0.0.9/openrl/envs/nlp/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/metrics/meteor.py` & `openrl-0.0.9/openrl/envs/nlp/utils/metrics/meteor.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/observation.py` & `openrl-0.0.9/openrl/envs/nlp/utils/observation.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/sampler.py` & `openrl-0.0.9/openrl/envs/nlp/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/nlp/utils/text_generation_pool.py` & `openrl-0.0.9/openrl/envs/nlp/utils/text_generation_pool.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/async_venv.py` & `openrl-0.0.9/openrl/envs/vec_env/async_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/base_venv.py` & `openrl-0.0.9/openrl/envs/vec_env/base_venv.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
+import sys
 import warnings
 from abc import ABC, abstractmethod
 from typing import Any, List, Optional, Sequence, Union
 
 import gymnasium as gym
 import numpy as np
 
 from openrl.envs.vec_env.utils.util import tile_images
 
+IN_COLAB = "google.colab" in sys.modules
+
 
 class BaseVecEnv(
     ABC,
 ):
     """
     An abstract vectorized environment.
 
@@ -154,18 +157,23 @@
         except NotImplementedError:
             warnings.warn(f"Render not defined for {self}")
             return
 
         # Create a big image by tiling images from subprocesses
         bigimg = tile_images(imgs)
         if mode == "human":
-            import cv2  # pytype:disable=import-error
+            if IN_COLAB:
+                from google.colab.patches import cv2_imshow
+
+                cv2_imshow(bigimg[:, :, ::-1])
+            else:
+                import cv2  # pytype:disable=import-error
 
-            cv2.imshow("Vec_Env:{}".format(self.env_name), bigimg[:, :, ::-1])
-            cv2.waitKey(1)
+                cv2.imshow("Vec_Env:{}".format(self.env_name), bigimg[:, :, ::-1])
+                cv2.waitKey(1)
         elif mode in [None, "rgb_array"]:
             return bigimg
         else:
             raise NotImplementedError(f"Render mode {mode} is not supported by VecEnvs")
 
     def _get_images(self) -> Sequence[np.ndarray]:
         """
```

### Comparing `openrl-0.0.8/openrl/envs/vec_env/sync_venv.py` & `openrl-0.0.9/openrl/envs/vec_env/sync_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/utils/__init__.py` & `openrl-0.0.9/openrl/envs/vec_env/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/utils/numpy_utils.py` & `openrl-0.0.9/openrl/envs/vec_env/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/utils/share_memory.py` & `openrl-0.0.9/openrl/envs/vec_env/utils/share_memory.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/utils/util.py` & `openrl-0.0.9/openrl/envs/vec_env/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/vec_info/__init__.py` & `openrl-0.0.9/openrl/envs/vec_env/vec_info/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/vec_info/base_vec_info.py` & `openrl-0.0.9/openrl/envs/vec_env/vec_info/base_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/vec_info/nlp_vec_info.py` & `openrl-0.0.9/openrl/envs/vec_env/vec_info/nlp_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/vec_info/simple_vec_info.py` & `openrl-0.0.9/openrl/envs/vec_env/vec_info/simple_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/wrappers/__init__.py` & `openrl-0.0.9/openrl/envs/vec_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/wrappers/base_wrapper.py` & `openrl-0.0.9/openrl/envs/vec_env/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/wrappers/reward_wrapper.py` & `openrl-0.0.9/openrl/envs/vec_env/wrappers/reward_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py` & `openrl-0.0.9/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/wrappers/base_wrapper.py` & `openrl-0.0.9/openrl/envs/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/wrappers/extra_wrappers.py` & `openrl-0.0.9/openrl/envs/wrappers/extra_wrappers.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/wrappers/multiagent_wrapper.py` & `openrl-0.0.9/openrl/envs/wrappers/multiagent_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/envs/wrappers/util.py` & `openrl-0.0.9/openrl/envs/wrappers/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/__init__.py` & `openrl-0.0.9/openrl/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/base_module.py` & `openrl-0.0.9/openrl/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/common/base_net.py` & `openrl-0.0.9/openrl/modules/common/base_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/common/ppo_net.py` & `openrl-0.0.9/openrl/modules/common/ppo_net.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 from typing import Any, Dict, Optional, Tuple, Union
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 
 from openrl.configs.config import create_config_parser
 from openrl.modules.common.base_net import BaseNet
 from openrl.modules.ppo_module import PPOModule
 from openrl.utils.util import set_seed
@@ -37,15 +37,15 @@
         n_rollout_threads: int = 1,
         model_dict: Optional[Dict[str, Any]] = None,
     ) -> None:
         super().__init__()
 
         if cfg is None:
             cfg_parser = create_config_parser()
-            cfg = cfg_parser.parse_args()
+            cfg = cfg_parser.parse_args([])
 
         set_seed(cfg.seed)
         env.reset(seed=cfg.seed)
 
         cfg.n_rollout_threads = n_rollout_threads
         cfg.learner_n_rollout_threads = cfg.n_rollout_threads
```

### Comparing `openrl-0.0.8/openrl/modules/model_config.py` & `openrl-0.0.9/openrl/modules/model_config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/__init__.py` & `openrl-0.0.9/openrl/modules/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/base_policy_network.py` & `openrl-0.0.9/openrl/modules/networks/base_policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/base_value_network.py` & `openrl-0.0.9/openrl/modules/networks/base_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/policy_network.py` & `openrl-0.0.9/openrl/modules/networks/policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/policy_value_network.py` & `openrl-0.0.9/openrl/modules/networks/policy_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/policy_value_network_gpt.py` & `openrl-0.0.9/openrl/modules/networks/policy_value_network_gpt.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/act.py` & `openrl-0.0.9/openrl/modules/networks/utils/act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/attention.py` & `openrl-0.0.9/openrl/modules/networks/utils/attention.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/cnn.py` & `openrl-0.0.9/openrl/modules/networks/utils/cnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/distributed_utils.py` & `openrl-0.0.9/openrl/modules/networks/utils/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/distributions.py` & `openrl-0.0.9/openrl/modules/networks/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/mix.py` & `openrl-0.0.9/openrl/modules/networks/utils/mix.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/mlp.py` & `openrl-0.0.9/openrl/modules/networks/utils/mlp.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/nlp/base_policy.py` & `openrl-0.0.9/openrl/modules/networks/utils/nlp/base_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/nlp/causal_policy.py` & `openrl-0.0.9/openrl/modules/networks/utils/nlp/causal_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/nlp/hf_generation_utils.py` & `openrl-0.0.9/openrl/modules/networks/utils/nlp/hf_generation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/popart.py` & `openrl-0.0.9/openrl/modules/networks/utils/popart.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/rnn.py` & `openrl-0.0.9/openrl/modules/networks/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/utils/transformer_act.py` & `openrl-0.0.9/openrl/modules/networks/utils/transformer_act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/networks/value_network.py` & `openrl-0.0.9/openrl/modules/networks/value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/ppo_module.py` & `openrl-0.0.9/openrl/modules/ppo_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/rl_module.py` & `openrl-0.0.9/openrl/modules/rl_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/utils/__init__.py` & `openrl-0.0.9/openrl/modules/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/utils/util.py` & `openrl-0.0.9/openrl/modules/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/modules/utils/valuenorm.py` & `openrl-0.0.9/openrl/modules/utils/valuenorm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/rewards/__init__.py` & `openrl-0.0.9/openrl/rewards/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/rewards/base_reward.py` & `openrl-0.0.9/openrl/rewards/base_reward.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/rewards/nlp_reward.py` & `openrl-0.0.9/openrl/rewards/nlp_reward.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/runners/__init__.py` & `openrl-0.0.9/openrl/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/runners/common/base_agent.py` & `openrl-0.0.9/openrl/runners/common/base_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/runners/common/chat_agent.py` & `openrl-0.0.9/openrl/runners/common/chat_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/runners/common/ppo_agent.py` & `openrl-0.0.9/openrl/runners/common/rl_agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,24 +19,20 @@
 import pathlib
 from typing import Dict, Optional, Tuple, Union
 
 import gym
 import numpy as np
 import torch
 
-from openrl.algorithms.ppo import PPOAlgorithm as TrainAlgo
-from openrl.buffers import NormalReplayBuffer as ReplayBuffer
 from openrl.buffers.utils.obs_data import ObsData
-from openrl.drivers.onpolicy_driver import OnPolicyDriver as Driver
 from openrl.runners.common.base_agent import BaseAgent, SelfAgent
-from openrl.utils.logger import Logger
 from openrl.utils.util import _t2n
 
 
-class PPOAgent(BaseAgent):
+class RLAgent(BaseAgent):
     def __init__(
         self,
         net: Optional[torch.nn.Module] = None,
         env: Union[gym.Env, str] = None,
         run_dir: Optional[str] = None,
         env_num: Optional[int] = None,
         rank: int = 0,
@@ -78,64 +74,20 @@
             assert (not self._use_wandb) and (not self._use_tensorboard), (
                 "run_dir must be set when using wandb or tensorboard. Please set"
                 " run_dir in the config file or pass run_dir in the"
                 " command line."
             )
 
         if self._cfg.experiment_name == "":
-            self.exp_name = "ppo"
+            self.exp_name = "rl"
         else:
             self.exp_name = self._cfg.experiment_name
 
     def train(self: SelfAgent, total_time_steps: int) -> None:
-        self._cfg.num_env_steps = total_time_steps
-
-        self.config = {
-            "cfg": self._cfg,
-            "num_agents": self.agent_num,
-            "run_dir": self.run_dir,
-            "envs": self._env,
-            "device": self.net.device,
-        }
-
-        trainer = TrainAlgo(
-            cfg=self._cfg,
-            init_module=self.net.module,
-            device=self.net.device,
-            agent_num=self.agent_num,
-        )
-
-        buffer = ReplayBuffer(
-            self._cfg,
-            self.agent_num,
-            self._env.observation_space,
-            self._env.action_space,
-            data_client=None,
-        )
-
-        logger = Logger(
-            cfg=self._cfg,
-            project_name="PPOAgent",
-            scenario_name=self._env.env_name,
-            wandb_entity=self._cfg.wandb_entity,
-            exp_name=self.exp_name,
-            log_path=self.run_dir,
-            use_wandb=self._use_wandb,
-            use_tensorboard=self._use_tensorboard,
-        )
-        driver = Driver(
-            config=self.config,
-            trainer=trainer,
-            buffer=buffer,
-            client=self.client,
-            rank=self.rank,
-            world_size=self.world_size,
-            logger=logger,
-        )
-        driver.run()
+        raise NotImplementedError
 
     def act(
         self,
         observation: Union[np.ndarray, Dict[str, np.ndarray]],
         deterministic: bool = True,
     ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
         assert self.net is not None, "net is None"
```

### Comparing `openrl-0.0.8/openrl/supports/__init__.py` & `openrl-0.0.9/openrl/supports/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/supports/opendata/__init__.py` & `openrl-0.0.9/openrl/supports/opendata/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/supports/opendata/utils/__init__.py` & `openrl-0.0.9/openrl/supports/opendata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/supports/opendata/utils/opendata_utils.py` & `openrl-0.0.9/openrl/supports/opendata/utils/opendata_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/supports/opengpu/__init__.py` & `openrl-0.0.9/openrl/supports/opengpu/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/supports/opengpu/gpu_info.py` & `openrl-0.0.9/openrl/supports/opengpu/gpu_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/supports/opengpu/manager.py` & `openrl-0.0.9/openrl/supports/opengpu/manager.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/utils/__init__.py` & `openrl-0.0.9/openrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/utils/logger.py` & `openrl-0.0.9/openrl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl/utils/util.py` & `openrl-0.0.9/openrl/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/openrl.egg-info/PKG-INFO` & `openrl-0.0.9/openrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.8
+Version: 0.0.9
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -49,15 +49,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.8 is updated on May 4, 2023 
+OpenRL-v0.0.9 is updated on May 6, 2023 
 
 The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
@@ -120,18 +120,21 @@
 ```
 
 安装完成后，用户可以直接通过命令行查看OpenRL的版本：
 ```bash
 openrl --version
 ```
 
+**Tips**：无需安装，通过Colab在线试用OpenRL: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
+
 ## 使用Docker
 
 OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
 如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+
 ```bash
 sudo docker pull openrllab/openrl-cpu
 ```
 
 如果用户想要通过显卡加速训练，则可以通过以下命令获取：
 ```bash
 sudo docker pull openrllab/openrl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.8 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.0.9 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
@@ -40,15 +40,15 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.8 is updated on May 4, 2023
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.9 is updated on May 6, 2023
 The main branch is the latest version of OpenRL, which is under active
 development. If you just want to have a try with OpenRL, you can switch to the
 stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
 (https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
 openrl-docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
@@ -82,15 +82,19 @@
 [Acknowledgments](#acknowledgments) ## å®è£
 ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
 æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
 https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ``` ## ä½¿ç¨Docker
+```bash openrl --version ```
+**Tips**ï¼æ éå®è£ï¼éè¿Colabå¨çº¿è¯ç¨OpenRL: [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
+## ä½¿ç¨Docker
 OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
 å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
 ```bash sudo docker pull openrllab/openrl-cpu ```
 å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
 ```bash sudo docker pull openrllab/openrl ```
 éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
 ```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
```

### Comparing `openrl-0.0.8/openrl.egg-info/SOURCES.txt` & `openrl-0.0.9/openrl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 openrl/rewards/base_reward.py
 openrl/rewards/nlp_reward.py
 openrl/runners/__init__.py
 openrl/runners/common/__init__.py
 openrl/runners/common/base_agent.py
 openrl/runners/common/chat_agent.py
 openrl/runners/common/ppo_agent.py
+openrl/runners/common/rl_agent.py
 openrl/supports/__init__.py
 openrl/supports/opendata/__init__.py
 openrl/supports/opendata/utils/__init__.py
 openrl/supports/opendata/utils/opendata_utils.py
 openrl/supports/opengpu/__init__.py
 openrl/supports/opengpu/gpu_info.py
 openrl/supports/opengpu/manager.py
```

### Comparing `openrl-0.0.8/setup.py` & `openrl-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/tests/__init__.py` & `openrl-0.0.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/tests/project/__init__.py` & `openrl-0.0.9/tests/project/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/tests/project/test_version.py` & `openrl-0.0.9/tests/project/test_version.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/tests/test_buffer/__init__.py` & `openrl-0.0.9/tests/test_buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.8/tests/test_buffer/test_buffer.py` & `openrl-0.0.9/tests/test_buffer/test_buffer.py`

 * *Files identical despite different names*


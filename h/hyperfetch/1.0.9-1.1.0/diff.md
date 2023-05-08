# Comparing `tmp/hyperfetch-1.0.9.tar.gz` & `tmp/hyperfetch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfetch-1.0.9.tar", last modified: Thu Apr 27 13:04:28 2023, max compression
+gzip compressed data, was "hyperfetch-1.1.0.tar", last modified: Mon May  8 16:02:57 2023, max compression
```

## Comparing `hyperfetch-1.0.9.tar` & `hyperfetch-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.479568 hyperfetch-1.0.9/
--rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.9/LICENSE
--rw-rw-rw-   0        0        0    10466 2023-04-27 13:04:28.479568 hyperfetch-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.9/README.md
--rw-rw-rw-   0        0        0     1690 2023-04-27 13:04:04.000000 hyperfetch-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 13:04:28.479568 hyperfetch-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.456411 hyperfetch-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.464232 hyperfetch-1.0.9/src/hyperfetch/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/__init__.py
--rw-rw-rw-   0        0        0    10569 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/alg_samplers.py
--rw-rw-rw-   0        0        0      654 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/auth_connection.py
--rw-rw-rw-   0        0        0     2118 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/callbacks.py
--rw-rw-rw-   0        0        0    34085 2023-04-27 12:55:49.000000 hyperfetch-1.0.9/src/hyperfetch/manager.py
--rw-rw-rw-   0        0        0     4994 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/tuning.py
--rw-rw-rw-   0        0        0      825 2023-04-27 12:48:32.000000 hyperfetch-1.0.9/src/hyperfetch/util.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:04:28.478575 hyperfetch-1.0.9/src/hyperfetch.egg-info/
--rw-rw-rw-   0        0        0    10466 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 13:04:28.000000 hyperfetch-1.0.9/src/hyperfetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.916342 hyperfetch-1.1.0/
+-rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7281 2023-05-08 16:02:57.916342 hyperfetch-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4916 2023-05-08 16:01:58.000000 hyperfetch-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1615 2023-05-08 16:02:31.000000 hyperfetch-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:02:57.916342 hyperfetch-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.879988 hyperfetch-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.887355 hyperfetch-1.1.0/src/hyperfetch/
+-rw-rw-rw-   0        0        0        0 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/alg_samplers.py
+-rw-rw-rw-   0        0        0      654 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/auth_connection.py
+-rw-rw-rw-   0        0        0     1934 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/callbacks.py
+-rw-rw-rw-   0        0        0    33572 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/manager.py
+-rw-rw-rw-   0        0        0     4994 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/tuning.py
+-rw-rw-rw-   0        0        0     1183 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/util.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.915425 hyperfetch-1.1.0/src/hyperfetch.egg-info/
+-rw-rw-rw-   0        0        0     7281 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      261 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/top_level.txt
```

### Comparing `hyperfetch-1.0.9/LICENSE` & `hyperfetch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.9/pyproject.toml` & `hyperfetch-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,53 +4,53 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["hyperfetch"]
 
 [project]
 name = "hyperfetch"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Karoline Sund Wahl", email="karolines.wahl@gmail.com" },
 ]
-description = "HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application."
+description = "HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application. Currently only available on Linux."
 readme = "README.md"
 requires-python = ">=3.9, <3.11.0"
 license = {file = "LICENSE"}
 keywords = ["reinforcement learning", "hyperparameters", "replication"]
 
 classifiers = [
       'Development Status :: 3 - Alpha',
       'Intended Audience :: Developers',
       'License :: OSI Approved :: BSD License',
-      'Operating System :: Microsoft :: Windows :: Windows 11',
       'Operating System :: POSIX :: Linux',
-      'Programming Language :: Python :: 3.8',
       'Programming Language :: Python :: 3.9',
       'Programming Language :: Python :: 3.10',
       'Framework :: FastAPI',
 ]
 
 dependencies = [
+      'setuptools==64.0.3',
+      'swig==4.0.2',
+      'box2d-py==2.3.8',
       'python-benedict==0.30.0',
       'codecarbon==2.1.4',
-      'torch== 1.11',
-      'gym==0.21.0',
       'pandas==2.0.1',
       'PyYAML==6.0',
       'motor==3.1.2',
       'numpy==1.24.3',
+      'gym==0.21.0',
+      'torch>=1.13.1',
       'optuna==3.1.1',
       'stable-baselines3==1.8.0',
       'rl-zoo3==1.8.0',
       'python-dotenv==1.0.0',
-      'starlette==0.26.1'
+      'starlette==0.26.1',
 ]
 
 [project.urls]
-"Backend" = "https://github.com/karolisw/hyperFetch"
-"Website" = "https://github.com/karolisw/hyperFetch/tree/frontend"
+"Website" = "https://www.hyperfetch.online/"
 "Source" = "https://github.com/karolisw/hyperFetch"
 
 [project.scripts]
 tune = "hyperfetch.tuning:tune_cli"
 save = "hyperfetch.tuning:save_cli"
```

### Comparing `hyperfetch-1.0.9/src/hyperfetch/alg_samplers.py` & `hyperfetch-1.1.0/src/hyperfetch/alg_samplers.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.9/src/hyperfetch/auth_connection.py` & `hyperfetch-1.1.0/src/hyperfetch/auth_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 load_dotenv(".env")
 
 MAX_CONNECTIONS_COUNT = int(os.getenv("MAX_CONNECTIONS_COUNT", 10))
 MIN_CONNECTIONS_COUNT = int(os.getenv("MIN_CONNECTIONS_COUNT", 10))
 
 ALLOWED_HOSTS = CommaSeparatedStrings(os.getenv("ALLOWED_HOSTS", "*"))
 
-MONGODB_URL = os.getenv("MONGODB_URL", "mongodb+srv://admin:adminKaroline12@hyperfetch.qwivycp.mongodb.net/test")
+MONGODB_URL = os.getenv("MONGODB_URL", "mongodb+srv://admin:adminKaroline12@hyperfetch.zxjvuqd.mongodb.net/test")
 MONGO_DB = os.getenv("MONGO_DB", "hyperfetch")
 MONGO_COLLECTION = os.getenv("MONGO_COLLECTION", "runs")
 
 database_name = MONGO_DB
 run_collection_name = MONGO_COLLECTION
```

### Comparing `hyperfetch-1.0.9/src/hyperfetch/callbacks.py` & `hyperfetch-1.1.0/src/hyperfetch/callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,32 +29,28 @@
             trial: optuna.Trial,
             n_eval_episodes: int = 5,
             eval_freq: int = 10000,
             deterministic: bool = True,
             verbose: int = 0,
             best_model_save_path: Optional[str] = None,
             log_path: Optional[str] = None,
-            callback_on_new_best=None,
-            reward_threshold=None
 
     ) -> None:
         super().__init__(
             eval_env=eval_env,
             n_eval_episodes=n_eval_episodes,
             eval_freq=eval_freq,
             deterministic=deterministic,
             verbose=verbose,
             best_model_save_path=best_model_save_path,
             log_path=log_path
-            # callback_on_new_best=callback_on_new_best
         )
         self.trial = trial
         self.eval_idx = 0
         self.is_pruned = False
-        # self.reward_threshold = reward_threshold
 
     def _on_step(self) -> bool:
         if self.eval_freq > 0 and self.n_calls % self.eval_freq == 0:
             super()._on_step()
             self.eval_idx += 1
             # Report the mean reward to optuna
             self.trial.report(self.last_mean_reward, self.eval_idx)
```

### Comparing `hyperfetch-1.0.9/src/hyperfetch/manager.py` & `hyperfetch-1.1.0/src/hyperfetch/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,35 +13,22 @@
 import torch
 from gym import spaces
 from optuna.integration import SkoptSampler
 from optuna.pruners import SuccessiveHalvingPruner, MedianPruner, NopPruner, HyperbandPruner, PercentilePruner, \
     PatientPruner, ThresholdPruner
 from optuna.samplers import RandomSampler, TPESampler, CmaEsSampler, NSGAIISampler
 from optuna.trial import FrozenTrial
-from stable_baselines3 import PPO, DQN, A2C, TD3, SAC
 from stable_baselines3.common.env_util import make_vec_env
 from stable_baselines3.common.preprocessing import is_image_space, is_image_space_channels_first
 from stable_baselines3.common.vec_env import VecTransposeImage, is_vecenv_wrapped
 from stable_baselines3.common.vec_env.vec_frame_stack import VecFrameStack
 from .util import *
 from .alg_samplers import ALG_HP_SAMPLER
 from .callbacks import TrialEvalCallback, ThresholdExceeded
-
-
-def _select_model(alg, **kwargs):
-    if alg == "ppo":
-        return PPO(**kwargs)
-    elif alg == "dqn":
-        return DQN(**kwargs)
-    elif alg == "a2c":
-        return A2C(**kwargs)
-    elif alg == "td3":
-        return TD3(**kwargs)
-    elif alg == "sac":
-        return SAC(**kwargs)
+from .util import _select_model
 
 
 class Manager:
     def __init__(self, config_path):
         """
         :param config_path: Must be specified to avoid error
 
@@ -139,22 +126,18 @@
             except ValueError:
                 pass
             return
 
         # Set pytorch num threads to 1 for faster training.
         torch.set_num_threads(1)
 
-        # Using config args, the sampler and pruner is selected
         # Select sampler and pruner and assign to self
         sampler = self._select_sampler()
         pruner = self._select_pruner()
 
-        # Do not prune before 1/3 of the max budget is used.
-        # pruner = MedianPruner(n_startup_trials=N_STARTUP_TRIALS, n_warmup_steps=N_EVALUATIONS // 3)
-
         study = optuna.create_study(sampler=sampler, pruner=pruner, study_name=self.project_name,
                                     direction="maximize")
         try:
             if self.reward_threshold is None:
                 study.optimize(self.objective, n_jobs=self.n_jobs, n_trials=self.n_trials)  # , timeout=600)
             else:
                 study.optimize(self.objective, n_jobs=self.n_jobs, n_trials=self.n_trials,
@@ -381,14 +364,15 @@
         self.n_jobs = data['n_jobs']
         self.n_evaluations = data['n_evaluations']
         self.n_trials = data['n_trials']
         self.n_warmup_steps = data['n_warmup_steps']
         self.n_min_trials = data['n_min_trials']
 
         # Verify the pruner in separate method
+        # Verify the pruner in separate method
         self._pruner_check(path_to_config)
         self._sampler_check(path_to_config)
 
     # Supporting method to the '_verify_config' method
     def _pruner_check(self, path_to_config) -> None:
 
         stream = open(path_to_config, 'r')
```

### Comparing `hyperfetch-1.0.9/src/hyperfetch/tuning.py` & `hyperfetch-1.1.0/src/hyperfetch/tuning.py`

 * *Files identical despite different names*


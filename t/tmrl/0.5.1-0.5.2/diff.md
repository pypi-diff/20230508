# Comparing `tmp/tmrl-0.5.1.tar.gz` & `tmp/tmrl-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmrl-0.5.1.tar", last modified: Fri Mar 24 06:52:57 2023, max compression
+gzip compressed data, was "tmrl-0.5.2.tar", last modified: Mon May  8 16:03:59 2023, max compression
```

## Comparing `tmrl-0.5.1.tar` & `tmrl-0.5.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.310289 tmrl-0.5.1/
--rw-rw-rw-   0        0        0     1110 2022-08-24 22:59:56.000000 tmrl-0.5.1/LICENSE
--rw-rw-rw-   0        0        0       58 2022-08-24 22:59:56.000000 tmrl-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0    29980 2023-03-24 06:52:57.305283 tmrl-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    28509 2023-03-21 23:10:55.000000 tmrl-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-24 06:52:57.310289 tmrl-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     5876 2023-03-24 06:44:39.000000 tmrl-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.127529 tmrl-0.5.1/tmrl/
--rw-rw-rw-   0        0        0     1430 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/__init__.py
--rw-rw-rw-   0        0        0     3951 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/__main__.py
--rw-rw-rw-   0        0        0     5386 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/actor.py
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.148346 tmrl-0.5.1/tmrl/config/
--rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/config/__init__.py
--rw-rw-rw-   0        0        0     5096 2023-03-24 06:44:21.000000 tmrl-0.5.1/tmrl/config/config_constants.py
--rw-rw-rw-   0        0        0     8112 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/config/config_objects.py
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.210188 tmrl-0.5.1/tmrl/custom/
--rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/custom/__init__.py
--rw-rw-rw-   0        0        0    18358 2023-03-24 06:44:21.000000 tmrl-0.5.1/tmrl/custom/custom_algorithms.py
--rw-rw-rw-   0        0        0     9634 2023-01-14 20:36:22.000000 tmrl-0.5.1/tmrl/custom/custom_checkpoints.py
--rw-rw-rw-   0        0        0    13405 2023-03-24 06:44:39.000000 tmrl-0.5.1/tmrl/custom/custom_gym_interfaces.py
--rw-rw-rw-   0        0        0    20373 2023-01-14 20:11:42.000000 tmrl-0.5.1/tmrl/custom/custom_memories.py
--rw-rw-rw-   0        0        0    30048 2023-03-24 06:44:21.000000 tmrl-0.5.1/tmrl/custom/custom_models.py
--rw-rw-rw-   0        0        0     1430 2023-01-14 20:11:42.000000 tmrl-0.5.1/tmrl/custom/custom_preprocessors.py
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.264739 tmrl-0.5.1/tmrl/custom/utils/
--rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/custom/utils/__init__.py
--rw-rw-rw-   0        0        0     5732 2023-03-24 06:44:21.000000 tmrl-0.5.1/tmrl/custom/utils/compute_reward.py
--rw-rw-rw-   0        0        0     2313 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/custom/utils/control_gamepad.py
--rw-rw-rw-   0        0        0     3182 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/custom/utils/control_keyboard.py
--rw-rw-rw-   0        0        0     1762 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/custom/utils/control_mouse.py
--rw-rw-rw-   0        0        0     9275 2023-01-06 00:42:48.000000 tmrl-0.5.1/tmrl/custom/utils/nn.py
--rw-rw-rw-   0        0        0     4853 2023-03-04 08:14:15.000000 tmrl-0.5.1/tmrl/custom/utils/tools.py
--rw-rw-rw-   0        0        0     3170 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/custom/utils/window.py
--rw-rw-rw-   0        0        0     1116 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/envs.py
--rw-rw-rw-   0        0        0     9705 2023-01-14 20:11:42.000000 tmrl-0.5.1/tmrl/memory.py
--rw-rw-rw-   0        0        0    31458 2023-03-22 01:26:23.000000 tmrl-0.5.1/tmrl/networking.py
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.286788 tmrl-0.5.1/tmrl/tools/
--rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/tools/__init__.py
--rw-rw-rw-   0        0        0     1457 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/tools/benchmark_environment.py
--rw-rw-rw-   0        0        0     2621 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/tools/check_environment.py
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.297442 tmrl-0.5.1/tmrl/tools/init_package/
--rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/tools/init_package/__init__.py
--rw-rw-rw-   0        0        0    28067 2022-08-24 22:59:56.000000 tmrl-0.5.1/tmrl/tools/init_package/init_pywin32.py
--rw-rw-rw-   0        0        0     2951 2023-02-05 00:12:49.000000 tmrl-0.5.1/tmrl/tools/record.py
--rw-rw-rw-   0        0        0     1279 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/tools/save_replays.py
--rw-rw-rw-   0        0        0     1390 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/training.py
--rw-rw-rw-   0        0        0    11114 2023-01-14 20:11:42.000000 tmrl-0.5.1/tmrl/training_offline.py
--rw-rw-rw-   0        0        0    10255 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/util.py
--rw-rw-rw-   0        0        0     2031 2023-03-21 23:10:55.000000 tmrl-0.5.1/tmrl/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-03-24 06:52:57.140821 tmrl-0.5.1/tmrl.egg-info/
--rw-rw-rw-   0        0        0    29980 2023-03-24 06:52:56.000000 tmrl-0.5.1/tmrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1124 2023-03-24 06:52:56.000000 tmrl-0.5.1/tmrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 06:52:56.000000 tmrl-0.5.1/tmrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-03-24 06:52:56.000000 tmrl-0.5.1/tmrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-24 06:52:56.000000 tmrl-0.5.1/tmrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.594897 tmrl-0.5.2/
+-rw-rw-rw-   0        0        0     1110 2022-08-24 22:59:56.000000 tmrl-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-08-24 22:59:56.000000 tmrl-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    29980 2023-05-08 16:03:59.579313 tmrl-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    28509 2023-03-21 23:10:55.000000 tmrl-0.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:03:59.594897 tmrl-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     5876 2023-05-08 15:49:59.000000 tmrl-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.389555 tmrl-0.5.2/tmrl/
+-rw-rw-rw-   0        0        0     1430 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/__init__.py
+-rw-rw-rw-   0        0        0     3951 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/__main__.py
+-rw-rw-rw-   0        0        0     5386 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/actor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.426045 tmrl-0.5.2/tmrl/config/
+-rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/config/__init__.py
+-rw-rw-rw-   0        0        0     5084 2023-05-08 15:44:14.000000 tmrl-0.5.2/tmrl/config/config_constants.py
+-rw-rw-rw-   0        0        0     8112 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/config/config_objects.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.468888 tmrl-0.5.2/tmrl/custom/
+-rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/custom/__init__.py
+-rw-rw-rw-   0        0        0    16427 2023-05-08 15:44:14.000000 tmrl-0.5.2/tmrl/custom/custom_algorithms.py
+-rw-rw-rw-   0        0        0     9634 2023-01-14 20:36:22.000000 tmrl-0.5.2/tmrl/custom/custom_checkpoints.py
+-rw-rw-rw-   0        0        0    13279 2023-05-08 15:44:14.000000 tmrl-0.5.2/tmrl/custom/custom_gym_interfaces.py
+-rw-rw-rw-   0        0        0    20373 2023-01-14 20:11:42.000000 tmrl-0.5.2/tmrl/custom/custom_memories.py
+-rw-rw-rw-   0        0        0    29156 2023-05-08 15:44:14.000000 tmrl-0.5.2/tmrl/custom/custom_models.py
+-rw-rw-rw-   0        0        0     1430 2023-01-14 20:11:42.000000 tmrl-0.5.2/tmrl/custom/custom_preprocessors.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.532300 tmrl-0.5.2/tmrl/custom/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/custom/utils/__init__.py
+-rw-rw-rw-   0        0        0     5732 2023-05-08 15:44:14.000000 tmrl-0.5.2/tmrl/custom/utils/compute_reward.py
+-rw-rw-rw-   0        0        0     2313 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/custom/utils/control_gamepad.py
+-rw-rw-rw-   0        0        0     3182 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/custom/utils/control_keyboard.py
+-rw-rw-rw-   0        0        0     1762 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/custom/utils/control_mouse.py
+-rw-rw-rw-   0        0        0     9275 2023-01-06 00:42:48.000000 tmrl-0.5.2/tmrl/custom/utils/nn.py
+-rw-rw-rw-   0        0        0     5019 2023-05-08 15:44:14.000000 tmrl-0.5.2/tmrl/custom/utils/tools.py
+-rw-rw-rw-   0        0        0     3170 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/custom/utils/window.py
+-rw-rw-rw-   0        0        0     1116 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/envs.py
+-rw-rw-rw-   0        0        0     9705 2023-01-14 20:11:42.000000 tmrl-0.5.2/tmrl/memory.py
+-rw-rw-rw-   0        0        0    31418 2023-03-30 19:52:01.000000 tmrl-0.5.2/tmrl/networking.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.563602 tmrl-0.5.2/tmrl/tools/
+-rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/tools/__init__.py
+-rw-rw-rw-   0        0        0     1457 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/tools/benchmark_environment.py
+-rw-rw-rw-   0        0        0     2621 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/tools/check_environment.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.579313 tmrl-0.5.2/tmrl/tools/init_package/
+-rw-rw-rw-   0        0        0        0 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/tools/init_package/__init__.py
+-rw-rw-rw-   0        0        0    28067 2022-08-24 22:59:56.000000 tmrl-0.5.2/tmrl/tools/init_package/init_pywin32.py
+-rw-rw-rw-   0        0        0     2951 2023-02-05 00:12:49.000000 tmrl-0.5.2/tmrl/tools/record.py
+-rw-rw-rw-   0        0        0     1280 2023-05-08 15:44:14.000000 tmrl-0.5.2/tmrl/tools/save_replays.py
+-rw-rw-rw-   0        0        0     1390 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/training.py
+-rw-rw-rw-   0        0        0    11114 2023-01-14 20:11:42.000000 tmrl-0.5.2/tmrl/training_offline.py
+-rw-rw-rw-   0        0        0    10255 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/util.py
+-rw-rw-rw-   0        0        0     2031 2023-03-21 23:10:55.000000 tmrl-0.5.2/tmrl/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:03:59.421265 tmrl-0.5.2/tmrl.egg-info/
+-rw-rw-rw-   0        0        0    29980 2023-05-08 16:03:59.000000 tmrl-0.5.2/tmrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1124 2023-05-08 16:03:59.000000 tmrl-0.5.2/tmrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:03:59.000000 tmrl-0.5.2/tmrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-05-08 16:03:59.000000 tmrl-0.5.2/tmrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-08 16:03:59.000000 tmrl-0.5.2/tmrl.egg-info/top_level.txt
```

### Comparing `tmrl-0.5.1/LICENSE` & `tmrl-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/PKG-INFO` & `tmrl-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.5.1
+Version: 0.5.2
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.5.1.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.5.2.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.5.1/README.md` & `tmrl-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/setup.py` & `tmrl-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,21 +123,21 @@
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name='tmrl',
-    version='0.5.1',
+    version='0.5.2',
     description='Network-based framework for real-time robot learning',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords='reinforcement learning, robot learning, trackmania, self driving, roborace',
     url='https://github.com/trackmania-rl/tmrl',
-    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.5.1.tar.gz',
+    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.5.2.tar.gz',
     author='Yann Bouteiller, Edouard Geze',
     author_email='yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr',
     license='MIT',
     install_requires=install_req,
     classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
```

### Comparing `tmrl-0.5.1/tmrl/__init__.py` & `tmrl-0.5.2/tmrl/__init__.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/__main__.py` & `tmrl-0.5.2/tmrl/__main__.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/actor.py` & `tmrl-0.5.2/tmrl/actor.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/config/config_constants.py` & `tmrl-0.5.2/tmrl/config/config_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 # DEBUGGING AND BENCHMARKING: ===================================
 
 CRC_DEBUG = False  # Only for checking the consistency of the custom networking methods, set it to False otherwise. Caution: difficult to handle if reset transitions are collected.
 CRC_DEBUG_SAMPLES = 100  # Number of samples collected in CRC_DEBUG mode
 PROFILE_TRAINER = False  # Will profile each epoch in the Trainer when True
 SYNCHRONIZE_CUDA = False  # Set to True for profiling, False otherwise
-DEBUG_MODEL = TMRL_CONFIG["DEBUG_MODEL_EVERY"] if "DEBUG_MODEL_EVERY" in TMRL_CONFIG.keys() else -1
+DEBUG_MODE = TMRL_CONFIG["DEBUG_MODE"] if "DEBUG_MODE" in TMRL_CONFIG.keys() else False
 
 # FILE SYSTEM: =================================================
 
 PATH_DATA = TMRL_FOLDER
 logging.debug(f" PATH_DATA:{PATH_DATA}")
 
 MODEL_HISTORY = TMRL_CONFIG["SAVE_MODEL_EVERY"]  # 0 for not saving history, x for saving model history every x new model received by RolloutWorker
```

### Comparing `tmrl-0.5.1/tmrl/config/config_objects.py` & `tmrl-0.5.2/tmrl/config/config_objects.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/custom_algorithms.py` & `tmrl-0.5.2/tmrl/custom/custom_algorithms.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,55 +14,14 @@
 from tmrl.util import cached_property
 from tmrl.training import TrainingAgent
 import tmrl.config.config_constants as cfg
 
 import logging
 
 
-if cfg.DEBUG_MODEL > 0:
-    import matplotlib.pyplot as plt
-    from matplotlib.lines import Line2D
-    import wandb
-
-    def plot_grad_flow(model):
-        named_parameters = model.named_parameters()
-        ave_grads = []
-        max_grads = []
-        layers = []
-        for n, p in named_parameters:
-            if p.requires_grad:  # and ("bias" not in n):
-                if p.grad is None:
-                    continue
-                layers.append(n)
-                ave_grads.append(p.grad.detach().abs().mean().cpu())
-                max_grads.append(p.grad.detach().abs().max().cpu())
-        plt.figure(figsize=(15, 7))
-        plt.bar(np.arange(len(max_grads)), max_grads, alpha=0.1, lw=1, color="c")
-        plt.bar(np.arange(len(max_grads)), ave_grads, alpha=0.1, lw=1, color="b")
-        plt.hlines(0, 0, len(ave_grads) + 1, lw=2, color="k")
-        plt.xticks(range(0, len(ave_grads), 1), layers, rotation="vertical")
-        plt.xlim(left=0, right=len(ave_grads))
-        plt.ylim(bottom=0.0, top=max(max_grads))  # zoom in on the lower gradient regions
-        plt.xlabel("Layers")
-        plt.ylabel("average gradient")
-        plt.title("Gradient flow")
-        plt.grid(True)
-        plt.legend([Line2D([0], [0], color="c", lw=4),
-                    Line2D([0], [0], color="b", lw=4),
-                    Line2D([0], [0], color="k", lw=4)], ['max-gradient', 'mean-gradient', 'zero-gradient'])
-        plt.tight_layout()
-        plt.draw()
-        res = wandb.Image(plt)
-        plt.close()
-        return res
-else:
-    def plot_grad_flow(model):
-        return None
-
-
 # Soft Actor-Critic ====================================================================================================
 
 
 @dataclass(eq=0)
 class SpinupSacAgent(TrainingAgent):  # Adapted from Spinup
     observation_space: type
     action_space: type
@@ -100,30 +59,19 @@
             # Note: we optimize the log of the entropy coeff which is slightly different from the paper
             # as discussed in https://github.com/rail-berkeley/softlearning/issues/37
             self.log_alpha = torch.log(torch.ones(1, device=self.device) * self.alpha).requires_grad_(True)
             self.alpha_optimizer = Adam([self.log_alpha], lr=self.lr_entropy)
         else:
             self.alpha_t = torch.tensor(float(self.alpha)).to(self.device)
 
-        self.debug_model_every = cfg.DEBUG_MODEL
-        self.debug_model = self.debug_model_every > 0
-        self.debug_model_cpt = self.debug_model_every - 1
-
     def get_actor(self):
         return self.model_nograd.actor
 
     def train(self, batch):
 
-        debug_model_now = False
-        if self.debug_model:
-            self.debug_model_cpt += 1
-            if self.debug_model_cpt == self.debug_model_every:
-                debug_model_now = True
-                self.debug_model_cpt = 0
-
         o, a, r, o2, d, _ = batch
 
         pi, logp_pi = self.model.actor(o)
         # FIXME? log_prob = log_prob.reshape(-1, 1)
 
         # loss_alpha:
 
@@ -165,17 +113,14 @@
         # MSE loss against Bellman backup
         loss_q1 = ((q1 - backup)**2).mean()
         loss_q2 = ((q2 - backup)**2).mean()
         loss_q = (loss_q1 + loss_q2) / 2  # averaged for homogeneity with REDQ
 
         self.q_optimizer.zero_grad()
         loss_q.backward()
-        if debug_model_now:
-            im_q1 = plot_grad_flow(self.model.q1)
-            im_q2 = plot_grad_flow(self.model.q2)
         self.q_optimizer.step()
 
         # Freeze Q-networks so you don't waste computational effort
         # computing gradients for them during the policy learning step.
         self.model.q1.requires_grad_(False)
         self.model.q2.requires_grad_(False)
 
@@ -189,16 +134,14 @@
         q_pi = torch.min(q1_pi, q2_pi)
 
         # Entropy-regularized policy loss
         loss_pi = (alpha_t * logp_pi - q_pi).mean()
 
         self.pi_optimizer.zero_grad()
         loss_pi.backward()
-        if debug_model_now:
-            im_pi = plot_grad_flow(self.model.actor)
         self.pi_optimizer.step()
 
         # Unfreeze Q-networks so you can optimize it at next DDPG step.
         self.model.q1.requires_grad_(True)
         self.model.q2.requires_grad_(True)
 
         # Finally, update target networks by polyak averaging.
@@ -207,112 +150,110 @@
                 # NB: We use an in-place operations "mul_", "add_" to update target
                 # params, as opposed to "mul" and "add", which would make new tensors.
                 p_targ.data.mul_(self.polyak)
                 p_targ.data.add_((1 - self.polyak) * p.data)
 
         # FIXME: remove debug info
         with torch.no_grad():
-            q1_o2_a2 = self.model.q1(o2, a2)
-            q2_o2_a2 = self.model.q2(o2, a2)
-            q1_targ_pi = self.model_target.q1(o, pi)
-            q2_targ_pi = self.model_target.q2(o, pi)
-            q1_targ_a = self.model_target.q1(o, a)
-            q2_targ_a = self.model_target.q2(o, a)
-
-            diff_q1pt_qpt = (q1_pi_targ - q_pi_targ).detach()
-            diff_q2pt_qpt = (q2_pi_targ - q_pi_targ).detach()
-            diff_q1_q1t_a2 = (q1_o2_a2 - q1_pi_targ).detach()
-            diff_q2_q2t_a2 = (q2_o2_a2 - q2_pi_targ).detach()
-            diff_q1_q1t_pi = (q1_pi - q1_targ_pi).detach()
-            diff_q2_q2t_pi = (q2_pi - q2_targ_pi).detach()
-            diff_q1_q1t_a = (q1 - q1_targ_a).detach()
-            diff_q2_q2t_a = (q2 - q2_targ_a).detach()
-            diff_q1_backup = (q1 - backup).detach()
-            diff_q2_backup = (q2 - backup).detach()
-            diff_q1_backup_r = (q1 - backup + r).detach()
-            diff_q2_backup_r = (q2 - backup + r).detach()
-
-            ret_dict = dict(
-                loss_actor=loss_pi.detach(),
-                loss_critic=loss_q.detach(),
-                # debug:
-                debug_log_pi=logp_pi.detach().mean(),
-                debug_log_pi_std=logp_pi.detach().std(),
-                debug_logp_a2=logp_a2.detach().mean(),
-                debug_logp_a2_std=logp_a2.detach().std(),
-                debug_q_a1=q_pi.detach().mean(),
-                debug_q_a1_std=q_pi.detach().std(),
-                debug_q_a1_targ=q_pi_targ.detach().mean(),
-                debug_q_a1_targ_std=q_pi_targ.detach().std(),
-                debug_backup=backup.detach().mean(),
-                debug_backup_std=backup.detach().std(),
-                debug_q1=q1.detach().mean(),
-                debug_q1_std=q1.detach().std(),
-                debug_q2=q2.detach().mean(),
-                debug_q2_std=q2.detach().std(),
-                debug_diff_q1=diff_q1_backup.mean(),
-                debug_diff_q1_std=diff_q1_backup.std(),
-                debug_diff_q2=diff_q2_backup.mean(),
-                debug_diff_q2_std=diff_q2_backup.std(),
-                debug_diff_r_q1=diff_q1_backup_r.mean(),
-                debug_diff_r_q1_std=diff_q1_backup_r.std(),
-                debug_diff_r_q2=diff_q2_backup_r.mean(),
-                debug_diff_r_q2_std=diff_q2_backup_r.std(),
-                debug_diff_q1pt_qpt=diff_q1pt_qpt.mean(),
-                debug_diff_q2pt_qpt=diff_q2pt_qpt.mean(),
-                debug_diff_q1_q1t_a2=diff_q1_q1t_a2.mean(),
-                debug_diff_q2_q2t_a2=diff_q2_q2t_a2.mean(),
-                debug_diff_q1_q1t_pi=diff_q1_q1t_pi.mean(),
-                debug_diff_q2_q2t_pi=diff_q2_q2t_pi.mean(),
-                debug_diff_q1_q1t_a=diff_q1_q1t_a.mean(),
-                debug_diff_q2_q2t_a=diff_q2_q2t_a.mean(),
-                debug_diff_q1pt_qpt_std=diff_q1pt_qpt.std(),
-                debug_diff_q2pt_qpt_std=diff_q2pt_qpt.std(),
-                debug_diff_q1_q1t_a2_std=diff_q1_q1t_a2.std(),
-                debug_diff_q2_q2t_a2_std=diff_q2_q2t_a2.std(),
-                debug_diff_q1_q1t_pi_std=diff_q1_q1t_pi.std(),
-                debug_diff_q2_q2t_pi_std=diff_q2_q2t_pi.std(),
-                debug_diff_q1_q1t_a_std=diff_q1_q1t_a.std(),
-                debug_diff_q2_q2t_a_std=diff_q2_q2t_a.std(),
-                debug_r=r.detach().mean(),
-                debug_r_std=r.detach().std(),
-                debug_d=d.detach().mean(),
-                debug_d_std=d.detach().std(),
-                debug_a_0=a[:, 0].detach().mean(),
-                debug_a_0_std=a[:, 0].detach().std(),
-                debug_a_1=a[:, 1].detach().mean(),
-                debug_a_1_std=a[:, 1].detach().std(),
-                debug_a_2=a[:, 2].detach().mean(),
-                debug_a_2_std=a[:, 2].detach().std(),
-                debug_a1_0=pi[:, 0].detach().mean(),
-                debug_a1_0_std=pi[:, 0].detach().std(),
-                debug_a1_1=pi[:, 1].detach().mean(),
-                debug_a1_1_std=pi[:, 1].detach().std(),
-                debug_a1_2=pi[:, 2].detach().mean(),
-                debug_a1_2_std=pi[:, 2].detach().std(),
-                debug_a2_0=a2[:, 0].detach().mean(),
-                debug_a2_0_std=a2[:, 0].detach().std(),
-                debug_a2_1=a2[:, 1].detach().mean(),
-                debug_a2_1_std=a2[:, 1].detach().std(),
-                debug_a2_2=a2[:, 2].detach().mean(),
-                debug_a2_2_std=a2[:, 2].detach().std(),
-            )  # FIXME: remove debug info
+
+            if not cfg.DEBUG_MODE:
+                ret_dict = dict(
+                    loss_actor=loss_pi.detach(),
+                    loss_critic=loss_q.detach(),
+                )
+            else:
+                q1_o2_a2 = self.model.q1(o2, a2)
+                q2_o2_a2 = self.model.q2(o2, a2)
+                q1_targ_pi = self.model_target.q1(o, pi)
+                q2_targ_pi = self.model_target.q2(o, pi)
+                q1_targ_a = self.model_target.q1(o, a)
+                q2_targ_a = self.model_target.q2(o, a)
+
+                diff_q1pt_qpt = (q1_pi_targ - q_pi_targ).detach()
+                diff_q2pt_qpt = (q2_pi_targ - q_pi_targ).detach()
+                diff_q1_q1t_a2 = (q1_o2_a2 - q1_pi_targ).detach()
+                diff_q2_q2t_a2 = (q2_o2_a2 - q2_pi_targ).detach()
+                diff_q1_q1t_pi = (q1_pi - q1_targ_pi).detach()
+                diff_q2_q2t_pi = (q2_pi - q2_targ_pi).detach()
+                diff_q1_q1t_a = (q1 - q1_targ_a).detach()
+                diff_q2_q2t_a = (q2 - q2_targ_a).detach()
+                diff_q1_backup = (q1 - backup).detach()
+                diff_q2_backup = (q2 - backup).detach()
+                diff_q1_backup_r = (q1 - backup + r).detach()
+                diff_q2_backup_r = (q2 - backup + r).detach()
+
+                ret_dict = dict(
+                    loss_actor=loss_pi.detach(),
+                    loss_critic=loss_q.detach(),
+                    # debug:
+                    debug_log_pi=logp_pi.detach().mean(),
+                    debug_log_pi_std=logp_pi.detach().std(),
+                    debug_logp_a2=logp_a2.detach().mean(),
+                    debug_logp_a2_std=logp_a2.detach().std(),
+                    debug_q_a1=q_pi.detach().mean(),
+                    debug_q_a1_std=q_pi.detach().std(),
+                    debug_q_a1_targ=q_pi_targ.detach().mean(),
+                    debug_q_a1_targ_std=q_pi_targ.detach().std(),
+                    debug_backup=backup.detach().mean(),
+                    debug_backup_std=backup.detach().std(),
+                    debug_q1=q1.detach().mean(),
+                    debug_q1_std=q1.detach().std(),
+                    debug_q2=q2.detach().mean(),
+                    debug_q2_std=q2.detach().std(),
+                    debug_diff_q1=diff_q1_backup.mean(),
+                    debug_diff_q1_std=diff_q1_backup.std(),
+                    debug_diff_q2=diff_q2_backup.mean(),
+                    debug_diff_q2_std=diff_q2_backup.std(),
+                    debug_diff_r_q1=diff_q1_backup_r.mean(),
+                    debug_diff_r_q1_std=diff_q1_backup_r.std(),
+                    debug_diff_r_q2=diff_q2_backup_r.mean(),
+                    debug_diff_r_q2_std=diff_q2_backup_r.std(),
+                    debug_diff_q1pt_qpt=diff_q1pt_qpt.mean(),
+                    debug_diff_q2pt_qpt=diff_q2pt_qpt.mean(),
+                    debug_diff_q1_q1t_a2=diff_q1_q1t_a2.mean(),
+                    debug_diff_q2_q2t_a2=diff_q2_q2t_a2.mean(),
+                    debug_diff_q1_q1t_pi=diff_q1_q1t_pi.mean(),
+                    debug_diff_q2_q2t_pi=diff_q2_q2t_pi.mean(),
+                    debug_diff_q1_q1t_a=diff_q1_q1t_a.mean(),
+                    debug_diff_q2_q2t_a=diff_q2_q2t_a.mean(),
+                    debug_diff_q1pt_qpt_std=diff_q1pt_qpt.std(),
+                    debug_diff_q2pt_qpt_std=diff_q2pt_qpt.std(),
+                    debug_diff_q1_q1t_a2_std=diff_q1_q1t_a2.std(),
+                    debug_diff_q2_q2t_a2_std=diff_q2_q2t_a2.std(),
+                    debug_diff_q1_q1t_pi_std=diff_q1_q1t_pi.std(),
+                    debug_diff_q2_q2t_pi_std=diff_q2_q2t_pi.std(),
+                    debug_diff_q1_q1t_a_std=diff_q1_q1t_a.std(),
+                    debug_diff_q2_q2t_a_std=diff_q2_q2t_a.std(),
+                    debug_r=r.detach().mean(),
+                    debug_r_std=r.detach().std(),
+                    debug_d=d.detach().mean(),
+                    debug_d_std=d.detach().std(),
+                    debug_a_0=a[:, 0].detach().mean(),
+                    debug_a_0_std=a[:, 0].detach().std(),
+                    debug_a_1=a[:, 1].detach().mean(),
+                    debug_a_1_std=a[:, 1].detach().std(),
+                    debug_a_2=a[:, 2].detach().mean(),
+                    debug_a_2_std=a[:, 2].detach().std(),
+                    debug_a1_0=pi[:, 0].detach().mean(),
+                    debug_a1_0_std=pi[:, 0].detach().std(),
+                    debug_a1_1=pi[:, 1].detach().mean(),
+                    debug_a1_1_std=pi[:, 1].detach().std(),
+                    debug_a1_2=pi[:, 2].detach().mean(),
+                    debug_a1_2_std=pi[:, 2].detach().std(),
+                    debug_a2_0=a2[:, 0].detach().mean(),
+                    debug_a2_0_std=a2[:, 0].detach().std(),
+                    debug_a2_1=a2[:, 1].detach().mean(),
+                    debug_a2_1_std=a2[:, 1].detach().std(),
+                    debug_a2_2=a2[:, 2].detach().mean(),
+                    debug_a2_2_std=a2[:, 2].detach().std(),
+                )
 
         if self.learn_entropy_coef:
             ret_dict["loss_entropy_coef"] = loss_alpha.detach()
-        ret_dict["entropy_coef"] = alpha_t.item()  # FIXME: indent
-
-        if debug_model_now:
-            wandb.log(
-                {
-                    "grads_q1": im_q1,
-                    "grads_q2": im_q2,
-                    "grads_pi": im_pi,
-                }
-            )
+            ret_dict["entropy_coef"] = alpha_t.item()
 
         return ret_dict
 
 
 # REDQ-SAC =============================================================================================================
 
 @dataclass(eq=0)
```

### Comparing `tmrl-0.5.1/tmrl/custom/custom_checkpoints.py` & `tmrl-0.5.2/tmrl/custom/custom_checkpoints.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/custom_gym_interfaces.py` & `tmrl-0.5.2/tmrl/custom/custom_gym_interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # third-party imports
 from rtgym import RealTimeGymInterface
 
 # local imports
 import tmrl.config.config_constants as cfg
 from tmrl.custom.utils.compute_reward import RewardFunction
 from tmrl.custom.utils.control_gamepad import control_gamepad, gamepad_reset, gamepad_close_finish_pop_up_tm20
+from tmrl.custom.utils.control_mouse import mouse_close_finish_pop_up_tm20
 from tmrl.custom.utils.control_keyboard import apply_control, keyres
-from tmrl.custom.utils.control_mouse import mouse_close_finish_pop_up_tm20, mouse_save_replay_tm20
 from tmrl.custom.utils.window import WindowInterface
-from tmrl.custom.utils.tools import Lidar, TM2020OpenPlanetClient
+from tmrl.custom.utils.tools import Lidar, TM2020OpenPlanetClient, save_ghost
 
 # Globals ==============================================================================================================
 
 NB_OBS_FORWARD = 500  # this allows (and rewards) 50m cuts
 
 # Interface for Trackmania 2020 ========================================================================================
 
@@ -35,27 +35,27 @@
     """
     This is the API needed for the algorithm to control TrackMania 2020
     """
     def __init__(self,
                  img_hist_len: int = 4,
                  gamepad: bool = False,
                  min_nb_steps_before_failure: int = int(3.5 * 20),
-                 save_replay: bool = False,
+                 save_replays: bool = False,
                  grayscale: bool = True,
                  resize_to=(64, 64),
                  finish_reward=cfg.REWARD_END_OF_TRACK,
                  constant_penalty=cfg.CONSTANT_PENALTY):
         """
         Base rtgym interface for TrackMania 2020 (Full environment)
 
         Args:
             img_hist_len: int: history of images that are part of observations
             gamepad: bool: whether to use a virtual gamepad for control
             min_nb_steps_before_failure: int: episode is done if not receiving reward during this nb of timesteps
-            save_replay: bool: whether to save TrackMania replays
+            save_replays: bool: whether to save TrackMania replays on successful episodes
             grayscale: bool: whether to output grayscale images or color images
             resize_to: Tuple[int, int]: resize output images to this (width, height)
             finish_reward: float: reward when passing the finish line
             constant_penalty: float: constant reward given at each time-step
         """
         self.last_time = None
         self.img_hist_len = img_hist_len
@@ -64,15 +64,15 @@
         self.reward_function = None
         self.client = None
         self.gamepad = gamepad
         self.j = None
         self.window_interface = None
         self.small_window = None
         self.min_nb_steps_before_failure = min_nb_steps_before_failure
-        self.save_replay = save_replay
+        self.save_replays = save_replays
         self.grayscale = grayscale
         self.resize_to = resize_to
         self.finish_reward = finish_reward
         self.constant_penalty = constant_penalty
 
         self.initialized = False
 
@@ -179,14 +179,17 @@
 
     def wait(self):
         """
         Non-blocking function
         The agent stays 'paused', waiting in position
         """
         self.send_control(self.get_default_action())
+        if self.save_replays:
+            save_ghost()
+            time.sleep(1.0)
         self.reset_race()
         time.sleep(0.5)
         self.close_finish_pop_up_tm20()
 
     def get_obs_rew_terminated_info(self):
         """
         returns the observation, the reward, and a terminated signal for end of episode
@@ -207,16 +210,14 @@
         imgs = np.array(list(self.img_hist))
         obs = [speed, gear, rpm, imgs]
         end_of_track = bool(data[8])
         info = {}
         if end_of_track:
             terminated = True
             rew += self.finish_reward
-            if self.save_replay:
-                mouse_save_replay_tm20(True)
         rew += self.constant_penalty
         rew = np.float32(rew)
         return obs, rew, terminated, info
 
     def get_observation_space(self):
         """
         must be a Tuple
@@ -244,16 +245,16 @@
         """
         initial action at episode start
         """
         return np.array([0.0, 0.0, 0.0], dtype='float32')
 
 
 class TM2020InterfaceLidar(TM2020Interface):
-    def __init__(self, img_hist_len=1, gamepad=False, min_nb_steps_before_failure=int(20 * 3.5), save_replay: bool = False):
-        super().__init__(img_hist_len, gamepad, min_nb_steps_before_failure, save_replay)
+    def __init__(self, img_hist_len=1, gamepad=False, min_nb_steps_before_failure=int(20 * 3.5), save_replays: bool = False):
+        super().__init__(img_hist_len, gamepad, min_nb_steps_before_failure, save_replays)
         self.window_interface = None
         self.lidar = None
 
     def grab_lidar_speed_and_data(self):
         img = self.window_interface.screenshot()[:, :, :3]
         data = self.client.retrieve_data()
         speed = np.array([
@@ -292,16 +293,14 @@
         imgs = np.array(list(self.img_hist), dtype='float32')
         obs = [speed, imgs]
         end_of_track = bool(data[8])
         info = {}
         if end_of_track:
             rew += self.finish_reward
             terminated = True
-            if self.save_replay:
-                mouse_save_replay_tm20()
         rew += self.constant_penalty
         rew = np.float32(rew)
         return obs, rew, terminated, info
 
     def get_observation_space(self):
         """
         must be a Tuple
@@ -342,16 +341,14 @@
         imgs = np.array(list(self.img_hist), dtype='float32')
         obs = [speed, progress, imgs]
         end_of_track = bool(data[8])
         info = {}
         if end_of_track:
             rew += self.finish_reward
             terminated = True
-            if self.save_replay:
-                mouse_save_replay_tm20()
         rew += self.constant_penalty
         rew = np.float32(rew)
         return obs, rew, terminated, info
 
     def get_observation_space(self):
         """
         must be a Tuple
```

### Comparing `tmrl-0.5.1/tmrl/custom/custom_memories.py` & `tmrl-0.5.2/tmrl/custom/custom_memories.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/custom_models.py` & `tmrl-0.5.2/tmrl/custom/custom_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -553,39 +553,20 @@
         pi_distribution = Normal(mu, std)
         if test:
             pi_action = mu
         else:
             pi_action = pi_distribution.rsample()
 
         if with_logprob:
-            """
-            NB: SB3:
-            
-             def log_prob(self, actions: th.Tensor, gaussian_actions: Optional[th.Tensor] = None) -> th.Tensor:
-                # Inverse tanh
-                # Naive implementation (not stable): 0.5 * torch.log((1 + x) / (1 - x))
-                # We use numpy to avoid numerical instability
-                if gaussian_actions is None:
-                    # It will be clipped to avoid NaN when inversing tanh
-                    gaussian_actions = TanhBijector.inverse(actions)
-        
-                # Log likelihood for a Gaussian distribution
-                log_prob = super().log_prob(gaussian_actions)
-                # Squash correction (from original SAC implementation)
-                # this comes from the fact that tanh is bijective and differentiable
-                log_prob -= th.sum(th.log(1 - actions**2 + self.epsilon), dim=1)
-                return log_prob
-            
-            """
             logp_pi = pi_distribution.log_prob(pi_action).sum(axis=-1)
             # NB: this is from Spinup:
-            # logp_pi -= (2 * (np.log(2) - pi_action - F.softplus(-2 * pi_action))).sum(axis=1)  # FIXME?
+            logp_pi -= (2 * (np.log(2) - pi_action - F.softplus(-2 * pi_action))).sum(axis=1)  # FIXME: this formula is mathematically wrong, no idea why it seems to work
             # Whereas SB3 does this:
-            logp_pi -= torch.sum(torch.log(1 - torch.tanh(pi_action) ** 2 + EPSILON), dim=1)  # TODO: double check
-            # log_prob -= th.sum(th.log(1 - actions**2 + self.epsilon), dim=1)
+            # logp_pi -= torch.sum(torch.log(1 - torch.tanh(pi_action) ** 2 + EPSILON), dim=1)  # TODO: double check
+            # # log_prob -= th.sum(th.log(1 - actions**2 + self.epsilon), dim=1)
         else:
             logp_pi = None
 
         pi_action = torch.tanh(pi_action)
         pi_action = self.act_limit * pi_action
 
         pi_action = pi_action.squeeze()
```

### Comparing `tmrl-0.5.1/tmrl/custom/custom_preprocessors.py` & `tmrl-0.5.2/tmrl/custom/custom_preprocessors.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/utils/compute_reward.py` & `tmrl-0.5.2/tmrl/custom/utils/compute_reward.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/utils/control_gamepad.py` & `tmrl-0.5.2/tmrl/custom/utils/control_gamepad.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/utils/control_keyboard.py` & `tmrl-0.5.2/tmrl/custom/utils/control_keyboard.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/utils/control_mouse.py` & `tmrl-0.5.2/tmrl/custom/utils/control_mouse.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/utils/nn.py` & `tmrl-0.5.2/tmrl/custom/utils/nn.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/custom/utils/tools.py` & `tmrl-0.5.2/tmrl/custom/utils/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,144 +1,156 @@
-# standard library imports
-import math
-import os
-import socket
-import struct
-import time
-from pathlib import Path
-from threading import Lock, Thread
-
-# third-party imports
-import cv2
-import numpy as np
-
-# local imports
-from tmrl.config.config_constants import LIDAR_BLACK_THRESHOLD
-
-
-class TM2020OpenPlanetClient:
-    def __init__(self, host='127.0.0.1', port=9000, struct_str='<' + 'f' * 11):
-        self._struct_str = struct_str
-        self.nb_floats = self._struct_str.count('f')
-        self.nb_uint64 = self._struct_str.count('Q')
-        self._nb_bytes = self.nb_floats * 4 + self.nb_uint64 * 8
-
-        self._host = host
-        self._port = port
-
-        # Threading attributes:
-        self.__lock = Lock()
-        self.__data = None
-        self.__t_client = Thread(target=self.__client_thread, args=(), kwargs={}, daemon=True)
-        self.__t_client.start()
-
-    def __client_thread(self):
-        """
-        Thread of the client.
-        This listens for incoming data until the object is destroyed
-        TODO: handle disconnection
-        """
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-            s.connect((self._host, self._port))
-            data_raw = b''
-            while True:  # main loop
-                while len(data_raw) < self._nb_bytes:
-                    data_raw += s.recv(1024)
-                div = len(data_raw) // self._nb_bytes
-                data_used = data_raw[(div - 1) * self._nb_bytes:div * self._nb_bytes]
-                data_raw = data_raw[div * self._nb_bytes:]
-                self.__lock.acquire()
-                self.__data = data_used
-                self.__lock.release()
-
-    def retrieve_data(self, sleep_if_empty=0.01, timeout=10.0):
-        """
-        Retrieves the most recently received data
-        Use this function to retrieve the most recently received data
-        This blocks if nothing has been received so far
-        """
-        c = True
-        t_start = None
-        while c:
-            self.__lock.acquire()
-            if self.__data is not None:
-                data = struct.unpack(self._struct_str, self.__data)
-                c = False
-                self.__data = None
-            self.__lock.release()
-            if c:
-                if t_start is None:
-                    t_start = time.time()
-                t_now = time.time()
-                assert t_now - t_start < timeout, f"OpenPlanet stopped sending data since more than {timeout}s."
-                time.sleep(sleep_if_empty)
-        return data
-
-
-def armin(tab):
-    nz = np.nonzero(tab)[0]
-    if len(nz) != 0:
-        return nz[0].item()
-    else:
-        return len(tab) - 1
-
-
-class Lidar:
-    def __init__(self, im):
-        self._set_axis_lidar(im)
-        self.black_threshold = LIDAR_BLACK_THRESHOLD
-
-    def _set_axis_lidar(self, im):
-        h, w, _ = im.shape
-        self.h = h
-        self.w = w
-        self.road_point = (44*h//49, w//2)
-        min_dist = 20
-        list_ax_x = []
-        list_ax_y = []
-        for angle in range(90, 280, 10):
-            axis_x = []
-            axis_y = []
-            x = self.road_point[0]
-            y = self.road_point[1]
-            dx = math.cos(math.radians(angle))
-            dy = math.sin(math.radians(angle))
-            lenght = False
-            dist = min_dist
-            while not lenght:
-                newx = int(x + dist * dx)
-                newy = int(y + dist * dy)
-                if newx <= 0 or newy <= 0 or newy >= w - 1:
-                    lenght = True
-                    list_ax_x.append(np.array(axis_x))
-                    list_ax_y.append(np.array(axis_y))
-                else:
-                    axis_x.append(newx)
-                    axis_y.append(newy)
-                dist = dist + 1
-        self.list_axis_x = list_ax_x
-        self.list_axis_y = list_ax_y
-
-    def lidar_20(self, img, show=False):
-        h, w, _ = img.shape
-        if h != self.h or w != self.w:
-            self._set_axis_lidar(img)
-        distances = []
-        if show:
-            color = (255, 0, 0)
-            thickness = 4
-            img = cv2.cvtColor(img, cv2.COLOR_RGBA2RGB)
-        for axis_x, axis_y in zip(self.list_axis_x, self.list_axis_y):
-            index = armin(np.all(img[axis_x, axis_y] < self.black_threshold, axis=1))
-            if show:
-                img = cv2.line(img, (self.road_point[1], self.road_point[0]), (axis_y[index], axis_x[index]), color, thickness)
-            index = np.float32(index)
-            distances.append(index)
-        res = np.array(distances, dtype=np.float32)
-        if show:
-            cv2.imshow("Environment", img)
-            cv2.waitKey(1)
-        return res
-
-
-if __name__ == "__main__":
-    pass
+# standard library imports
+import math
+import os
+import socket
+import struct
+import time
+from pathlib import Path
+from threading import Lock, Thread
+
+# third-party imports
+import cv2
+import numpy as np
+
+# local imports
+from tmrl.config.config_constants import LIDAR_BLACK_THRESHOLD
+
+
+class TM2020OpenPlanetClient:
+    def __init__(self, host='127.0.0.1', port=9000, struct_str='<' + 'f' * 11):
+        self._struct_str = struct_str
+        self.nb_floats = self._struct_str.count('f')
+        self.nb_uint64 = self._struct_str.count('Q')
+        self._nb_bytes = self.nb_floats * 4 + self.nb_uint64 * 8
+
+        self._host = host
+        self._port = port
+
+        # Threading attributes:
+        self.__lock = Lock()
+        self.__data = None
+        self.__t_client = Thread(target=self.__client_thread, args=(), kwargs={}, daemon=True)
+        self.__t_client.start()
+
+    def __client_thread(self):
+        """
+        Thread of the client.
+        This listens for incoming data until the object is destroyed
+        TODO: handle disconnection
+        """
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+            s.connect((self._host, self._port))
+            data_raw = b''
+            while True:  # main loop
+                while len(data_raw) < self._nb_bytes:
+                    data_raw += s.recv(1024)
+                div = len(data_raw) // self._nb_bytes
+                data_used = data_raw[(div - 1) * self._nb_bytes:div * self._nb_bytes]
+                data_raw = data_raw[div * self._nb_bytes:]
+                self.__lock.acquire()
+                self.__data = data_used
+                self.__lock.release()
+
+    def retrieve_data(self, sleep_if_empty=0.01, timeout=10.0):
+        """
+        Retrieves the most recently received data
+        Use this function to retrieve the most recently received data
+        This blocks if nothing has been received so far
+        """
+        c = True
+        t_start = None
+        while c:
+            self.__lock.acquire()
+            if self.__data is not None:
+                data = struct.unpack(self._struct_str, self.__data)
+                c = False
+                self.__data = None
+            self.__lock.release()
+            if c:
+                if t_start is None:
+                    t_start = time.time()
+                t_now = time.time()
+                assert t_now - t_start < timeout, f"OpenPlanet stopped sending data since more than {timeout}s."
+                time.sleep(sleep_if_empty)
+        return data
+
+
+def save_ghost(host='127.0.0.1', port=10000):
+    """
+    Saves the current ghost
+
+    Args:
+        host (str): IP address of the ghost-saving server
+        port (int): Port of the ghost-saving server
+    """
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        s.connect((host, port))
+
+
+def armin(tab):
+    nz = np.nonzero(tab)[0]
+    if len(nz) != 0:
+        return nz[0].item()
+    else:
+        return len(tab) - 1
+
+
+class Lidar:
+    def __init__(self, im):
+        self._set_axis_lidar(im)
+        self.black_threshold = LIDAR_BLACK_THRESHOLD
+
+    def _set_axis_lidar(self, im):
+        h, w, _ = im.shape
+        self.h = h
+        self.w = w
+        self.road_point = (44*h//49, w//2)
+        min_dist = 20
+        list_ax_x = []
+        list_ax_y = []
+        for angle in range(90, 280, 10):
+            axis_x = []
+            axis_y = []
+            x = self.road_point[0]
+            y = self.road_point[1]
+            dx = math.cos(math.radians(angle))
+            dy = math.sin(math.radians(angle))
+            lenght = False
+            dist = min_dist
+            while not lenght:
+                newx = int(x + dist * dx)
+                newy = int(y + dist * dy)
+                if newx <= 0 or newy <= 0 or newy >= w - 1:
+                    lenght = True
+                    list_ax_x.append(np.array(axis_x))
+                    list_ax_y.append(np.array(axis_y))
+                else:
+                    axis_x.append(newx)
+                    axis_y.append(newy)
+                dist = dist + 1
+        self.list_axis_x = list_ax_x
+        self.list_axis_y = list_ax_y
+
+    def lidar_20(self, img, show=False):
+        h, w, _ = img.shape
+        if h != self.h or w != self.w:
+            self._set_axis_lidar(img)
+        distances = []
+        if show:
+            color = (255, 0, 0)
+            thickness = 4
+            img = cv2.cvtColor(img, cv2.COLOR_RGBA2RGB)
+        for axis_x, axis_y in zip(self.list_axis_x, self.list_axis_y):
+            index = armin(np.all(img[axis_x, axis_y] < self.black_threshold, axis=1))
+            if show:
+                img = cv2.line(img, (self.road_point[1], self.road_point[0]), (axis_y[index], axis_x[index]), color, thickness)
+            index = np.float32(index)
+            distances.append(index)
+        res = np.array(distances, dtype=np.float32)
+        if show:
+            cv2.imshow("Environment", img)
+            cv2.waitKey(1)
+        return res
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `tmrl-0.5.1/tmrl/custom/utils/window.py` & `tmrl-0.5.2/tmrl/custom/utils/window.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/envs.py` & `tmrl-0.5.2/tmrl/envs.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/memory.py` & `tmrl-0.5.2/tmrl/memory.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/networking.py` & `tmrl-0.5.2/tmrl/networking.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,15 +710,15 @@
             nb_steps (int): number of steps to perform to compute the benchmark
             test (int): whether the actor is called in test or train mode
         """
         obs, info = self.reset(collect_samples=False)
         for _ in range(nb_steps):
             obs, rew, terminated, truncated, info = self.step(obs=obs, test=test, collect_samples=False)
             if terminated or truncated:
-                obs, info = self.reset(collect_samples=False)
+                break
         print_with_timestamp(f"Benchmark results:\n{self.env.benchmarks()}")
 
     def send_and_clear_buffer(self):
         """
         Sends the buffered samples to the `Server`.
         """
         self.__endpoint.produce(self.buffer, "trainers")
```

### Comparing `tmrl-0.5.1/tmrl/tools/benchmark_environment.py` & `tmrl-0.5.2/tmrl/tools/benchmark_environment.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/tools/check_environment.py` & `tmrl-0.5.2/tmrl/tools/check_environment.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/tools/init_package/init_pywin32.py` & `tmrl-0.5.2/tmrl/tools/init_package/init_pywin32.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/tools/record.py` & `tmrl-0.5.2/tmrl/tools/record.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/tools/save_replays.py` & `tmrl-0.5.2/tmrl/tools/save_replays.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from tmrl.envs import GenericGymEnv
 from tmrl.networking import RolloutWorker
 from tmrl.util import partial
 
 
 def save_replays(nb_replays=np.inf):
     config = cfg_obj.CONFIG_DICT
-    config['interface_kwargs'] = {'save_replay': True}
+    config['interface_kwargs'] = {'save_replays': True}
     rw = RolloutWorker(env_cls=partial(GenericGymEnv, id="real-time-gym-v1", gym_kwargs={"config": config}),
                        actor_module_cls=partial(cfg_obj.POLICY),
                        sample_compressor=cfg_obj.SAMPLE_COMPRESSOR,
                        device='cuda' if cfg.CUDA_INFERENCE else 'cpu',
                        server_ip=cfg.SERVER_IP_FOR_WORKER,
                        model_path=cfg.MODEL_PATH_WORKER,
                        obs_preprocessor=cfg_obj.OBS_PREPROCESSOR,
```

### Comparing `tmrl-0.5.1/tmrl/training.py` & `tmrl-0.5.2/tmrl/training.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/training_offline.py` & `tmrl-0.5.2/tmrl/training_offline.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/util.py` & `tmrl-0.5.2/tmrl/util.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl/wrappers.py` & `tmrl-0.5.2/tmrl/wrappers.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.5.1/tmrl.egg-info/PKG-INFO` & `tmrl-0.5.2/tmrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.5.1
+Version: 0.5.2
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.5.1.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.5.2.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.5.1/tmrl.egg-info/SOURCES.txt` & `tmrl-0.5.2/tmrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*


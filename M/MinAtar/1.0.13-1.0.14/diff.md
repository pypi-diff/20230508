# Comparing `tmp/MinAtar-1.0.13.tar.gz` & `tmp/MinAtar-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinAtar-1.0.13.tar", last modified: Mon May  8 16:56:26 2023, max compression
+gzip compressed data, was "MinAtar-1.0.14.tar", last modified: Mon May  8 17:31:51 2023, max compression
```

## Comparing `MinAtar-1.0.13.tar` & `MinAtar-1.0.14.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 16:56:26.966907 MinAtar-1.0.13/
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 16:56:26.960840 MinAtar-1.0.13/MinAtar.egg-info/
--rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-08 16:56:26.000000 MinAtar-1.0.13/MinAtar.egg-info/PKG-INFO
--rw-r--r--   0 kjyoung    (502) staff       (20)      496 2023-05-08 16:56:26.000000 MinAtar-1.0.13/MinAtar.egg-info/SOURCES.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)        1 2023-05-08 16:56:26.000000 MinAtar-1.0.13/MinAtar.egg-info/dependency_links.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)       47 2023-05-08 16:56:26.000000 MinAtar-1.0.13/MinAtar.egg-info/entry_points.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)      198 2023-05-08 16:56:26.000000 MinAtar-1.0.13/MinAtar.egg-info/requires.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)        8 2023-05-08 16:56:26.000000 MinAtar-1.0.13/MinAtar.egg-info/top_level.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-08 16:56:26.966701 MinAtar-1.0.13/PKG-INFO
--rw-r--r--   0 kjyoung    (502) staff       (20)    13921 2023-05-08 16:21:18.000000 MinAtar-1.0.13/README.md
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 16:56:26.963264 MinAtar-1.0.13/minatar/
--rw-r--r--   0 kjyoung    (502) staff       (20)       36 2021-11-05 15:11:24.000000 MinAtar-1.0.13/minatar/__init__.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     3935 2023-05-08 16:54:56.000000 MinAtar-1.0.13/minatar/environment.py
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 16:56:26.966215 MinAtar-1.0.13/minatar/environments/
--rw-r--r--   0 kjyoung    (502) staff       (20)       15 2021-11-05 15:11:24.000000 MinAtar-1.0.13/minatar/environments/__init__.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     6222 2023-05-08 16:54:56.000000 MinAtar-1.0.13/minatar/environments/asterix.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     5100 2023-05-08 16:54:56.000000 MinAtar-1.0.13/minatar/environments/breakout.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     5819 2023-05-08 16:54:56.000000 MinAtar-1.0.13/minatar/environments/freeway.py
--rw-r--r--   0 kjyoung    (502) staff       (20)    13034 2023-05-08 16:54:56.000000 MinAtar-1.0.13/minatar/environments/seaquest.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     6887 2023-05-08 16:54:56.000000 MinAtar-1.0.13/minatar/environments/space_invaders.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     4085 2021-11-05 15:11:24.000000 MinAtar-1.0.13/minatar/gui.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     3232 2023-05-08 16:54:56.000000 MinAtar-1.0.13/minatar/gym.py
--rw-r--r--   0 kjyoung    (502) staff       (20)       93 2022-04-10 19:37:26.000000 MinAtar-1.0.13/pyproject.toml
--rw-r--r--   0 kjyoung    (502) staff       (20)       38 2023-05-08 16:56:26.967002 MinAtar-1.0.13/setup.cfg
--rw-r--r--   0 kjyoung    (502) staff       (20)      877 2023-05-08 16:54:56.000000 MinAtar-1.0.13/setup.py
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.631857 MinAtar-1.0.14/
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.623069 MinAtar-1.0.14/MinAtar.egg-info/
+-rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/PKG-INFO
+-rw-r--r--   0 kjyoung    (502) staff       (20)      496 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/SOURCES.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)        1 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/dependency_links.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)       47 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/entry_points.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)      198 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/requires.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)        8 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/top_level.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-08 17:31:51.631412 MinAtar-1.0.14/PKG-INFO
+-rw-r--r--   0 kjyoung    (502) staff       (20)    14086 2023-05-08 17:20:45.000000 MinAtar-1.0.14/README.md
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.625642 MinAtar-1.0.14/minatar/
+-rw-r--r--   0 kjyoung    (502) staff       (20)       36 2021-11-05 15:11:24.000000 MinAtar-1.0.14/minatar/__init__.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     3935 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environment.py
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.630689 MinAtar-1.0.14/minatar/environments/
+-rw-r--r--   0 kjyoung    (502) staff       (20)       15 2021-11-05 15:11:24.000000 MinAtar-1.0.14/minatar/environments/__init__.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     6222 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/asterix.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     5100 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/breakout.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     5819 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/freeway.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)    13034 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/seaquest.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     6887 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/space_invaders.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     4085 2021-11-05 15:11:24.000000 MinAtar-1.0.14/minatar/gui.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     3252 2023-05-08 17:20:45.000000 MinAtar-1.0.14/minatar/gym.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)       93 2022-04-10 19:37:26.000000 MinAtar-1.0.14/pyproject.toml
+-rw-r--r--   0 kjyoung    (502) staff       (20)       38 2023-05-08 17:31:51.632012 MinAtar-1.0.14/setup.cfg
+-rw-r--r--   0 kjyoung    (502) staff       (20)      877 2023-05-08 17:20:45.000000 MinAtar-1.0.14/setup.py
```

### Comparing `MinAtar-1.0.13/README.md` & `MinAtar-1.0.14/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,45 +65,46 @@
 python examples/human_play.py -g <game>
 ```
 Use the arrow keys to move and space bar to fire. Press q to quit and r to reset.
 
 Finally, we provide a simple implementations of DQN in `dqn.py` and online actor-critic with eligibility traces in `AC_lambda.py`.
 
 
-## OpenAI Gym Wrapper
-MinAtar is fully compatible with the latest OpenAI Gym version (0.26).
-A Gym environment can be constructed as follows:
-```bash
-import gym
+## Gymnasium Wrapper
+MinAtar is fully compatible with [Gymnasium](https://gymnasium.farama.org/).
+A Gymnasium environment can be constructed as follows:
+```python
+import gymnasium as gym
 env = gym.make('MinAtar/<game-id>')
 ````
-The following game IDs ara available: Asterix-v0, Breakout-v0, Freeway-v0, Seaquest-v0, SpaceInvaders-v0, Asterix-v1, Breakout-v1, Freeway-v1, Seaquest-v1, SpaceInvaders-v1.  
+The following game IDs are available: Asterix-v0, Breakout-v0, Freeway-v0, Seaquest-v0, SpaceInvaders-v0, Asterix-v1, Breakout-v1, Freeway-v1, Seaquest-v1, SpaceInvaders-v1.  
 For each game, in the v0 versions the action set has all 6 available actions (some of which are equivalent to no-op depending on the game),
 while in the v1 versions the action set is reduced to just the minimal actions for each game.  
 Note that the results included in this repo and the associated paper use the full action set of 6 actions.
 
-> If you want to use the old Gym API (without the `truncated` flag, and with the old `reset()` and `seed()` methods),
-install MinAtar 1.0.11 by running:
-```bash
-pip install minatar==1.0.11
-```
+> If you want to use the latest OpenAI Gym API (v0.26),
+install MinAtar v1.0.13 by running `pip install minatar==1.0.13`
+
+> If you want to use old OpenAI Gym API (without the `truncated` flag, and with the old `reset()` and `seed()` methods),
+install MinAtar v1.0.11 by running `pip install minatar==1.0.11`
 
 ## Visualizing the Environments
 We provide 2 ways to visualize a MinAtar environment.
 
 ### Using Environment.display_state()
 The Environment class includes a simple visualizer using matplotlib in the `display_state()` function. To use it simply call:
 ```python
 env = Environment('breakout')
 env.display_state(50)
 # train, do steps, ...
 env.close_display()
 ```
 or, if you're using the gym interface:
 ```python
+import gymnasium as gym
 env = gym.make('MinAtar/Breakout-v1')
 env.game.display_state(50)
 # train, do steps, ...
 env.game.close_display()
 ```
 The argument is the number of milliseconds to display the state before continuing execution.
```

### Comparing `MinAtar-1.0.13/minatar/environment.py` & `MinAtar-1.0.14/minatar/environment.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.13/minatar/environments/asterix.py` & `MinAtar-1.0.14/minatar/environments/asterix.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.13/minatar/environments/breakout.py` & `MinAtar-1.0.14/minatar/environments/breakout.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.13/minatar/environments/freeway.py` & `MinAtar-1.0.14/minatar/environments/freeway.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.13/minatar/environments/seaquest.py` & `MinAtar-1.0.14/minatar/environments/seaquest.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.13/minatar/environments/space_invaders.py` & `MinAtar-1.0.14/minatar/environments/space_invaders.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.13/minatar/gui.py` & `MinAtar-1.0.14/minatar/gui.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.13/minatar/gym.py` & `MinAtar-1.0.14/minatar/gym.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Adapted from https://github.com/qlan3/gym-games
 import numpy as np
-import gym
-from gym import spaces
-from gym.envs import register
+import gymnasium as gym
+from gymnasium import spaces
+from gymnasium.envs.registration import register
 
 try:
     import seaborn as sns
 except:
     import logging
     logging.warning("Cannot import seaborn."
         "Will not be able to train from pixel observations.")
@@ -80,16 +80,16 @@
         return 0
 
 
 def register_envs():
     for game in ["asterix", "breakout", "freeway", "seaquest", "space_invaders"]:
         name = game.title().replace('_', '')
         register(
-            id="{}-v0".format(name),
+            id="MinAtar/{}-v0".format(name),
             entry_point="minatar.gym:BaseEnv",
-            kwargs=dict(game=game, display_time=50, use_minimal_action_set=False),
+            kwargs=dict(game=game, use_minimal_action_set=False),
         )
         register(
-            id="{}-v1".format(name),
+            id="MinAtar/{}-v1".format(name),
             entry_point="minatar.gym:BaseEnv",
-            kwargs=dict(game=game, display_time=50, use_minimal_action_set=True),
+            kwargs=dict(game=game, use_minimal_action_set=True),
         )
```

### Comparing `MinAtar-1.0.13/setup.py` & `MinAtar-1.0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 entry_points = {
     'gym.envs': ['MinAtar=minatar.gym:register_envs']
 }
 
 setup(
     name='MinAtar',
-    version='1.0.13',
+    version='1.0.14',
     description='A miniaturized version of the Arcade Learning Environment.',
     url='https://github.com/kenjyoung/MinAtar',
     author='Kenny Young',
     author_email='kjyoung@ualberta.ca',
     license='GPL',
     packages=packages,
     entry_points=entry_points,
```


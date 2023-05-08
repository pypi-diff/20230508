# Comparing `tmp/gym-trading-env-0.3.0.tar.gz` & `tmp/gym-trading-env-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.3.0.tar", last modified: Sun May  7 09:52:45 2023, max compression
+gzip compressed data, was "gym-trading-env-0.3.1.tar", last modified: Mon May  8 21:06:55 2023, max compression
```

## Comparing `gym-trading-env-0.3.0.tar` & `gym-trading-env-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.615556 gym-trading-env-0.3.0/
--rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       44 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4428 2023-05-07 09:52:45.613554 gym-trading-env-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2566 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/README.md
--rw-rw-rw-   0        0        0      853 2023-05-07 08:41:42.000000 gym-trading-env-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 09:52:45.615556 gym-trading-env-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.434849 gym-trading-env-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.497874 gym-trading-env-0.3.0/src/gym_trading_env/
--rw-rw-rw-   0        0        0      333 2023-04-13 13:15:17.000000 gym-trading-env-0.3.0/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.3.0/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0    16488 2023-05-07 08:31:47.000000 gym-trading-env-0.3.0/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2504 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.584573 gym-trading-env-0.3.0/src/gym_trading_env/templates/
--rw-rw-rw-   0        0        0     3878 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/src/gym_trading_env/templates/index.html
-drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.609553 gym-trading-env-0.3.0/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-13 09:31:51.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-10 08:13:00.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.540553 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0     4428 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 21:06:55.116114 gym-trading-env-0.3.1/
+-rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       44 2023-05-06 13:10:40.000000 gym-trading-env-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4428 2023-05-08 21:06:55.115115 gym-trading-env-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2566 2023-05-06 13:10:40.000000 gym-trading-env-0.3.1/README.md
+-rw-rw-rw-   0        0        0      853 2023-05-08 21:06:06.000000 gym-trading-env-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 21:06:55.117118 gym-trading-env-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 21:06:55.041133 gym-trading-env-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 21:06:55.068118 gym-trading-env-0.3.1/src/gym_trading_env/
+-rw-rw-rw-   0        0        0      333 2023-04-13 13:15:17.000000 gym-trading-env-0.3.1/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.3.1/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0    16681 2023-05-08 20:42:28.000000 gym-trading-env-0.3.1/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2504 2023-05-06 13:10:40.000000 gym-trading-env-0.3.1/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:06:55.102117 gym-trading-env-0.3.1/src/gym_trading_env/templates/
+-rw-rw-rw-   0        0        0     3878 2023-05-06 13:10:40.000000 gym-trading-env-0.3.1/src/gym_trading_env/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-05-08 21:06:55.112114 gym-trading-env-0.3.1/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.3.1/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.3.1/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-13 09:31:51.000000 gym-trading-env-0.3.1/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-10 08:13:00.000000 gym-trading-env-0.3.1/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:06:55.099114 gym-trading-env-0.3.1/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0     4428 2023-05-08 21:06:54.000000 gym-trading-env-0.3.1/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-05-08 21:06:55.000000 gym-trading-env-0.3.1/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 21:06:54.000000 gym-trading-env-0.3.1/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-08 21:06:54.000000 gym-trading-env-0.3.1/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-08 21:06:54.000000 gym-trading-env-0.3.1/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.3.0/LICENSE.txt` & `gym-trading-env-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/PKG-INFO` & `gym-trading-env-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.0 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.1 Summary: A simple,
 easy, customizable Open IA Gym environments for trading. Author-email: Clement
 Perroud
 perroud.pro@gmail.com> License: MIT License Copyright (c) [year] [fullname]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `gym-trading-env-0.3.0/README.md` & `gym-trading-env-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/pyproject.toml` & `gym-trading-env-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.3.0"
+version = "0.3.1"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env/downloader.py` & `gym-trading-env-0.3.1/src/gym_trading_env/downloader.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env/environments.py` & `gym-trading-env-0.3.1/src/gym_trading_env/environments.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     :param initial_position: You can specify the initial position of the environment or set it to 'random'. It must contained in the list parameter 'positions'.
     :type initial_position: optional - float or int
 
     :param include_position_in_features: Whether or not you want the current position to be added to the step observations. If windows is set an int, it will add the last N-step positions.
     :type include_position_in_features: optional - bool
 
-    :param max_episode_duration: Can be set to an Integer or to 'max'. If a interger value is set, each episode will be truncated after reaching the max amount of steps (by returning `truncated` as `True`) and each episode will start at a random starting point to maximize exploration.
+    :param max_episode_duration: If a integer value is used, each episode will be truncated after reaching the desired max duration in steps (by returning `truncated` as `True`). When using a max duration, each episode will start at a random starting point.
     :type max_episode_duration: optional - int or 'max'
 
     :param verbose: If 0, no log is outputted. If 1, the env send episode result logs.
     :type verbose: optional - int
     
     :param name: The name of the environment (eg. 'BTC/USDT')
     :type name: optional - str
@@ -238,30 +238,38 @@
             reward = 0
         )
         if not done:
             reward = self.reward_function(self.historical_info)
             self.historical_info["reward", -1] = reward
 
         if done or truncated:
+            self.calculate_metrics()
             self.log()
 
         return self._get_obs(),  self.historical_info["reward", -1], done, truncated, self.historical_info[-1]
     def add_metric(self, name, function):
         self.log_metrics.append({
             'name': name,
             'function': function
         })
+    def calculate_metrics(self):
+        self.results_metrics = {
+            "Market Return" : f"{100*self.historical_info['data_close', -1] / self.historical_info['data_close', 0] -1:5.2f}%",
+            "Portfolio Return" : f"{100*self.historical_info['portfolio_valuation', -1] / self.historical_info['portfolio_valuation', 0] -1:5.2f}%",
+        }
+
+        for metric in self.log_metrics:
+            self.results_metrics[metric['name']] = metric['function'](self.historical_info)
+    def get_metrics(self):
+        return self.results_metrics
     def log(self):
         if self.verbose > 0:
-            market_return = self.historical_info["data_close", -1] / self.historical_info["data_close", 0] -1
-            portfolio_return = self.historical_info["portfolio_valuation", -1] / self.historical_info["portfolio_valuation", 0] -1
-
-            text = f"""Market Return : {100*market_return:5.2f}%   |   Portfolio Return : {100*portfolio_return:5.2f}%"""
-            for metric in self.log_metrics:
-                text += f"   |   {metric['name']} : {metric['function'](self.historical_info)}"
+            text = ""
+            for key, value in self.results_metrics.items():
+                text += f"{key} : {value}   |   "
             print(text)
     def save_for_render(self, dir = "render_logs"):
         assert "open" in self.df and "high" in self.df and "low" in self.df and "close" in self.df, "Your DataFrame needs to contain columns : open, high, low, close to render !"
         columns = list(set(self.historical_info.columns) - set([f"date_{col}" for col in self._info_columns]))
         history_df = pd.DataFrame(
             self.historical_info[columns], columns= columns
         )
@@ -321,15 +329,15 @@
                     "MultiDatasetTradingEnv",
                     dataset_dir= 'examples/data/*.pkl',
                     preprocess= preprocess,
                 )
     
     :type preprocess: function<pandas.DataFrame->pandas.DataFrame>
 
-    :param episodes_between_dataset_switch: The number of time a dataset will be used for an episode before switching to another dataset. It can be useful for performances when `max_episode_duration` is low.
+    :param episodes_between_dataset_switch: Number of times a dataset is used to create an episode, before moving on to another dataset. It can be useful for performances when `max_episode_duration` is low.
     :type episodes_between_dataset_switch: optional - int
 
     """
     def __init__(self,
                 dataset_dir, 
                 *args,
```

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env/renderer.py` & `gym-trading-env-0.3.1/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env/templates/index.html` & `gym-trading-env-0.3.1/src/gym_trading_env/templates/index.html`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.3.1/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.3.1/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.3.1/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.3.1/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.0 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.1 Summary: A simple,
 easy, customizable Open IA Gym environments for trading. Author-email: Clement
 Perroud
 perroud.pro@gmail.com> License: MIT License Copyright (c) [year] [fullname]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `gym-trading-env-0.3.0/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.3.1/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*


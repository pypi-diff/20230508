# Comparing `tmp/cluster_experiments-0.6.4.tar.gz` & `tmp/cluster_experiments-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.6.4.tar", last modified: Mon May  8 15:04:56 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.6.5.tar", last modified: Mon May  8 15:13:25 2023, max compression
```

## Comparing `cluster_experiments-0.6.4.tar` & `cluster_experiments-0.6.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.457354 cluster_experiments-0.6.4/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.4/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.4/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:04:56.456561 cluster_experiments-0.6.4/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-16 08:27:58.000000 cluster_experiments-0.6.4/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.399978 cluster_experiments-0.6.4/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.4/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.4/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.6.4/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-05-08 15:04:11.000000 cluster_experiments-0.6.4/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.4/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:04:15.000000 cluster_experiments-0.6.4/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.4/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.409382 cluster_experiments-0.6.4/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-08 15:04:56.457610 cluster_experiments-0.6.4/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:04:15.000000 cluster_experiments-0.6.4/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.419463 cluster_experiments-0.6.4/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.4/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.424293 cluster_experiments-0.6.4/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.4/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.6.4/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.429557 cluster_experiments-0.6.4/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.6.4/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.6.4/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.4/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.432569 cluster_experiments-0.6.4/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2023-05-08 15:04:11.000000 cluster_experiments-0.6.4/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.445940 cluster_experiments-0.6.4/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.4/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.6.4/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.4/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.455113 cluster_experiments-0.6.4/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:04:15.000000 cluster_experiments-0.6.4/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.4/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.4/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.4/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.4/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.4/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.6.4/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.444192 cluster_experiments-0.6.5/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.5/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.5/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:13:25.443566 cluster_experiments-0.6.5/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-16 08:27:58.000000 cluster_experiments-0.6.5/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.403521 cluster_experiments-0.6.5/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.5/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.5/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.6.5/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5609 2023-05-08 15:13:10.000000 cluster_experiments-0.6.5/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.5/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.6.5/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.5/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.410104 cluster_experiments-0.6.5/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-08 15:13:25.444445 cluster_experiments-0.6.5/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:13:10.000000 cluster_experiments-0.6.5/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.418656 cluster_experiments-0.6.5/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.5/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.422461 cluster_experiments-0.6.5/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.5/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.6.5/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.425910 cluster_experiments-0.6.5/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.6.5/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.6.5/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.5/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.428103 cluster_experiments-0.6.5/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2879 2023-05-08 15:13:10.000000 cluster_experiments-0.6.5/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.436096 cluster_experiments-0.6.5/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.5/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.6.5/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.5/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.442745 cluster_experiments-0.6.5/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.6.5/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.5/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.5/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.5/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.5/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.5/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.6.5/tests/utils.py
```

### Comparing `cluster_experiments-0.6.4/LICENSE` & `cluster_experiments-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/README.md` & `cluster_experiments-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments/__init__.py` & `cluster_experiments-0.6.5/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments/cupac.py` & `cluster_experiments-0.6.5/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.6.5/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments/perturbator.py` & `cluster_experiments-0.6.5/cluster_experiments/perturbator.py`

 * *Files 19% similar despite different names*

```diff
@@ -100,14 +100,27 @@
         """Like sample without replacement,
         but if you are to sample more than 100% of the data,
         it just returns the whole dataframe."""
         if n >= len(df):
             return df
         return df.sample(n=n)
 
+    def _data_checks(self, df: pd.DataFrame, average_effect: float) -> None:
+        """Check that outcome is indeed binary, and average effect is in (-1, 1)"""
+
+        if set(df[self.target_col].unique()) != {0, 1}:
+            raise ValueError(
+                f"Target column must be binary, found {set(df[self.target_col].unique())}"
+            )
+
+        if average_effect > 1 or average_effect < -1:
+            raise ValueError(
+                f"Average effect must be in (-1, 1), found {average_effect}"
+            )
+
     def perturbate(
         self, df: pd.DataFrame, average_effect: Optional[float] = None
     ) -> pd.DataFrame:
         """
         Usage:
 
         ```python
@@ -118,14 +131,16 @@
         perturbator.perturbate(df, average_effect=0.1)
         ```
         """
 
         df = df.copy().reset_index(drop=True)
         average_effect = self.get_average_effect(average_effect)
 
+        self._data_checks(df, average_effect)
+
         from_target, to_target = 1, 0
         if average_effect > 0:
             from_target, to_target = 0, 1
 
         n_transformed = abs(int(average_effect * len(df.query(self.treated_query))))
         idx = list(
             # Sample of negative cases in group B
```

### Comparing `cluster_experiments-0.6.4/cluster_experiments/power_analysis.py` & `cluster_experiments-0.6.5/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments/power_config.py` & `cluster_experiments-0.6.5/cluster_experiments/power_config.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments/random_splitter.py` & `cluster_experiments-0.6.5/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments/washover.py` & `cluster_experiments-0.6.5/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.6.5/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.6.5/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/setup.py` & `cluster_experiments-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.6.4",
+    version="0.6.5",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.6.4/tests/analysis/test_analysis.py` & `cluster_experiments-0.6.5/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/cupac/test_aggregator.py` & `cluster_experiments-0.6.5/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.6.5/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/examples.py` & `cluster_experiments-0.6.5/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.6.5/tests/perturbator/test_perturbator.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,9 +63,23 @@
         == avg_target
     )
 
 
 def test_binary_raises():
     binary_df_repeated = pd.concat([binary_df for _ in range(50)])
     bp = BinaryPerturbator()
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="average_effect must be provided"):
         bp.perturbate(binary_df_repeated)
+
+
+@pytest.mark.parametrize("average_effect", [(-1.1), (1.1)])
+def test_binary_raises_out_of_limit(average_effect):
+    bp = BinaryPerturbator()
+    with pytest.raises(ValueError, match="Average effect must be in"):
+        bp.perturbate(binary_df, average_effect=average_effect)
+
+
+def test_binary_raises_non_binary_target():
+    bp = BinaryPerturbator()
+    binary_df["target"] = binary_df["target"] + 0.01
+    with pytest.raises(ValueError, match="must be binary"):
+        bp.perturbate(binary_df, average_effect=0.05)
```

### Comparing `cluster_experiments-0.6.4/tests/power_analysis/conftest.py` & `cluster_experiments-0.6.5/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.6.5/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.6.5/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.6.5/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.6.5/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.6.5/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.6.5/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/splitter/conftest.py` & `cluster_experiments-0.6.5/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/splitter/test_splitter.py` & `cluster_experiments-0.6.5/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.6.5/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/splitter/test_time_col.py` & `cluster_experiments-0.6.5/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/splitter/test_washover.py` & `cluster_experiments-0.6.5/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/test_docs.py` & `cluster_experiments-0.6.5/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/test_non_clustered.py` & `cluster_experiments-0.6.5/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.4/tests/utils.py` & `cluster_experiments-0.6.5/tests/utils.py`

 * *Files identical despite different names*


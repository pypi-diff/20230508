# Comparing `tmp/cluster_experiments-0.6.3.tar.gz` & `tmp/cluster_experiments-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.6.3.tar", last modified: Fri Apr 28 14:01:07 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.6.4.tar", last modified: Mon May  8 15:04:56 2023, max compression
```

## Comparing `cluster_experiments-0.6.3.tar` & `cluster_experiments-0.6.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.883882 cluster_experiments-0.6.3/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.3/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.3/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-28 14:01:07.883206 cluster_experiments-0.6.3/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-16 08:27:58.000000 cluster_experiments-0.6.3/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.807871 cluster_experiments-0.6.3/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.3/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.3/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.6.3/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-03-01 11:31:23.000000 cluster_experiments-0.6.3/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.3/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17760 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.3/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.817867 cluster_experiments-0.6.3/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-04-28 14:01:07.884106 cluster_experiments-0.6.3/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-04-28 14:00:38.000000 cluster_experiments-0.6.3/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.828481 cluster_experiments-0.6.3/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.3/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.833027 cluster_experiments-0.6.3/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.3/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.838031 cluster_experiments-0.6.3/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.6.3/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.3/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.841395 cluster_experiments-0.6.3/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.864424 cluster_experiments-0.6.3/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.3/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.6.3/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.3/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.881544 cluster_experiments-0.6.3/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5743 2023-04-05 14:50:51.000000 cluster_experiments-0.6.3/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.3/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.3/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.3/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.3/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.3/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.457354 cluster_experiments-0.6.4/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.4/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.4/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:04:56.456561 cluster_experiments-0.6.4/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-16 08:27:58.000000 cluster_experiments-0.6.4/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.399978 cluster_experiments-0.6.4/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.4/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.4/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.6.4/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-05-08 15:04:11.000000 cluster_experiments-0.6.4/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.4/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:04:15.000000 cluster_experiments-0.6.4/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.4/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.409382 cluster_experiments-0.6.4/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-08 15:04:56.000000 cluster_experiments-0.6.4/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-08 15:04:56.457610 cluster_experiments-0.6.4/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:04:15.000000 cluster_experiments-0.6.4/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.419463 cluster_experiments-0.6.4/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.4/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.424293 cluster_experiments-0.6.4/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.4/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.6.4/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.429557 cluster_experiments-0.6.4/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.6.4/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.6.4/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.4/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.432569 cluster_experiments-0.6.4/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2023-05-08 15:04:11.000000 cluster_experiments-0.6.4/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.445940 cluster_experiments-0.6.4/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.4/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.6.4/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.4/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.4/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:04:56.455113 cluster_experiments-0.6.4/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:04:15.000000 cluster_experiments-0.6.4/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.4/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.4/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.4/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.4/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.4/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.4/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.4/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.6.4/tests/utils.py
```

### Comparing `cluster_experiments-0.6.3/LICENSE` & `cluster_experiments-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/README.md` & `cluster_experiments-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments/__init__.py` & `cluster_experiments-0.6.4/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments/cupac.py` & `cluster_experiments-0.6.4/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.6.4/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments/perturbator.py` & `cluster_experiments-0.6.4/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments/power_analysis.py` & `cluster_experiments-0.6.4/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments/power_config.py` & `cluster_experiments-0.6.4/cluster_experiments/power_config.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments/random_splitter.py` & `cluster_experiments-0.6.4/cluster_experiments/random_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     def _get_time_col_cluster(self, df: pd.DataFrame) -> pd.Series:
         df = df.copy()
         df[self.time_col] = pd.to_datetime(df[self.time_col])
         # Given the switch frequency, truncate the time column to the switch frequency
         # Using pandas frequency aliases: https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
         if "W" in self.switch_frequency or "M" in self.switch_frequency:
             return df[self.time_col].dt.to_period(self.switch_frequency).dt.start_time
-        return df[self.time_col].dt.floor(self.switch_frequency, ambiguous="infer")
+        return df[self.time_col].dt.floor(self.switch_frequency)
 
     def _prepare_switchback_df(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df.copy()
         # Build time_col switchback column
         # Overwriting column, this is the worst! If we use the column as a covariate, we're screwed. Needs improvement
         df[_original_time_column(self.time_col)] = df[self.time_col]
         df[self.time_col] = self._get_time_col_cluster(df)
```

### Comparing `cluster_experiments-0.6.3/cluster_experiments/washover.py` & `cluster_experiments-0.6.4/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.6.4/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.6.4/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/setup.py` & `cluster_experiments-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.6.3",
+    version="0.6.4",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.6.3/tests/analysis/test_analysis.py` & `cluster_experiments-0.6.4/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/cupac/test_aggregator.py` & `cluster_experiments-0.6.4/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.6.4/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/examples.py` & `cluster_experiments-0.6.4/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.6.4/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/power_analysis/conftest.py` & `cluster_experiments-0.6.4/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.6.4/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.6.4/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.6.4/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.6.4/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.6.4/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.6.4/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/splitter/conftest.py` & `cluster_experiments-0.6.4/tests/splitter/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,15 +153,15 @@
                 pd.to_datetime("2022-01-01 00:31:00"),
                 pd.to_datetime("2022-01-01 01:14:00"),
                 pd.to_datetime("2022-01-01 01:31:00"),
             ],
             "treatment": ["A", "A", "B", "B"],
             "city": ["TGN"] * 4,
         }
-    ).assign(time=lambda x: x["original___time"].dt.floor("1h", ambiguous="infer"))
+    ).assign(time=lambda x: x["original___time"].dt.floor("1h"))
     return df
 
 
 @pytest.fixture
 def washover_df_no_switch():
     df = pd.DataFrame(
         {
@@ -172,15 +172,15 @@
                 pd.to_datetime("2022-01-01 01:31:00"),
                 pd.to_datetime("2022-01-01 02:01:00"),
                 pd.to_datetime("2022-01-01 02:31:00"),
             ],
             "treatment": ["A", "A", "B", "B", "B", "B"],
             "city": ["TGN"] * 6,
         }
-    ).assign(time=lambda x: x["original___time"].dt.floor("1h", ambiguous="infer"))
+    ).assign(time=lambda x: x["original___time"].dt.floor("1h"))
     return df
 
 
 @pytest.fixture
 def washover_df_multi_city():
     df = pd.DataFrame(
         {
@@ -193,15 +193,15 @@
                 pd.to_datetime("2022-01-01 02:31:00"),
             ]
             * 2,
             "treatment": ["A", "A", "B", "B", "B", "B"]
             + ["A", "A", "A", "A", "B", "B"],
             "city": ["TGN"] * 6 + ["BCN"] * 6,
         }
-    ).assign(time=lambda x: x["original___time"].dt.floor("1h", ambiguous="infer"))
+    ).assign(time=lambda x: x["original___time"].dt.floor("1h"))
     return df
 
 
 @pytest.fixture
 def washover_split_df(n):
     # Return
     return pd.DataFrame(
```

### Comparing `cluster_experiments-0.6.3/tests/splitter/test_splitter.py` & `cluster_experiments-0.6.4/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.6.4/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/splitter/test_time_col.py` & `cluster_experiments-0.6.4/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/splitter/test_washover.py` & `cluster_experiments-0.6.4/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/test_docs.py` & `cluster_experiments-0.6.4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/test_non_clustered.py` & `cluster_experiments-0.6.4/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.3/tests/utils.py` & `cluster_experiments-0.6.4/tests/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/DeepRetail-0.0.5.tar.gz` & `tmp/DeepRetail-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\u0138780\yForecasting_Github\DeepRetail\dist\.tmp-ame6ps54\DeepRetail-0.0.5.tar", last modified: Thu Mar 23 09:40:25 2023, max compression
+gzip compressed data, was "C:\Users\u0138780\yForecasting_Github\DeepRetail\dist\.tmp-16h3am6s\DeepRetail-0.0.6.tar", last modified: Mon May  8 09:04:07 2023, max compression
```

## Comparing `DeepRetail-0.0.5.tar` & `DeepRetail-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:25.005438 DeepRetail-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.866425 DeepRetail-0.0.5/DeepRetail/
--rw-rw-rw-   0        0        0        0 2023-02-15 11:39:40.000000 DeepRetail-0.0.5/DeepRetail/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.909424 DeepRetail-0.0.5/DeepRetail/data/
--rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.5/DeepRetail/data/__init__.py
--rw-rw-rw-   0        0        0    16945 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/data/casereaders.py
--rw-rw-rw-   0        0        0     9392 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/data/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.932437 DeepRetail-0.0.5/DeepRetail/evaluation/
--rw-rw-rw-   0        0        0       41 2023-02-20 14:22:28.000000 DeepRetail-0.0.5/DeepRetail/evaluation/__init__.py
--rw-rw-rw-   0        0        0    10987 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/evaluation/base.py
--rw-rw-rw-   0        0        0     9136 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/evaluation/metrics.py
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.944423 DeepRetail-0.0.5/DeepRetail/forecasting/
--rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.5/DeepRetail/forecasting/__init__.py
--rw-rw-rw-   0        0        0    22867 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/forecasting/statistical.py
--rw-rw-rw-   0        0        0     1929 2023-03-02 14:21:40.000000 DeepRetail-0.0.5/DeepRetail/forecasting/utils.py
--rw-rw-rw-   0        0        0       49 2023-02-15 11:39:40.000000 DeepRetail-0.0.5/DeepRetail/hierarchical.py
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.963428 DeepRetail-0.0.5/DeepRetail/reconciliation/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:21:40.000000 DeepRetail-0.0.5/DeepRetail/reconciliation/__init__.py
--rw-rw-rw-   0        0        0    24670 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/reconciliation/cross_sectional.py
--rw-rw-rw-   0        0        0    35145 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/reconciliation/cross_temporal.py
--rw-rw-rw-   0        0        0    33014 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/reconciliation/temporal.py
--rw-rw-rw-   0        0        0    18106 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/reconciliation/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.971441 DeepRetail-0.0.5/DeepRetail/transformations/
--rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.5/DeepRetail/transformations/__init__.py
--rw-rw-rw-   0        0        0    13147 2023-03-23 09:36:05.000000 DeepRetail-0.0.5/DeepRetail/transformations/formats.py
--rw-rw-rw-   0        0        0       61 2023-03-23 09:39:56.000000 DeepRetail-0.0.5/DeepRetail/version.py
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.999426 DeepRetail-0.0.5/DeepRetail/visuals/
--rw-rw-rw-   0        0        0       15 2023-02-20 14:22:28.000000 DeepRetail-0.0.5/DeepRetail/visuals/__init__.py
--rw-rw-rw-   0        0        0     9337 2023-03-02 14:21:40.000000 DeepRetail-0.0.5/DeepRetail/visuals/evaluation.py
-drwxrwxrwx   0        0        0        0 2023-03-23 09:40:24.897423 DeepRetail-0.0.5/DeepRetail.egg-info/
--rw-rw-rw-   0        0        0     3684 2023-03-23 09:40:24.000000 DeepRetail-0.0.5/DeepRetail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      899 2023-03-23 09:40:24.000000 DeepRetail-0.0.5/DeepRetail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 09:40:24.000000 DeepRetail-0.0.5/DeepRetail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-03-23 09:40:24.000000 DeepRetail-0.0.5/DeepRetail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-23 09:40:24.000000 DeepRetail-0.0.5/DeepRetail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-06-19 22:52:26.000000 DeepRetail-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3684 2023-03-23 09:40:25.003450 DeepRetail-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2887 2023-03-23 09:39:56.000000 DeepRetail-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-03-23 09:40:25.006424 DeepRetail-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-03-23 09:39:56.000000 DeepRetail-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.040992 DeepRetail-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:06.979977 DeepRetail-0.0.6/DeepRetail/
+-rw-rw-rw-   0        0        0        0 2023-02-15 11:39:40.000000 DeepRetail-0.0.6/DeepRetail/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.002993 DeepRetail-0.0.6/DeepRetail/data/
+-rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/data/__init__.py
+-rw-rw-rw-   0        0        0    17039 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/data/casereaders.py
+-rw-rw-rw-   0        0        0     9392 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/data/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.008993 DeepRetail-0.0.6/DeepRetail/evaluation/
+-rw-rw-rw-   0        0        0       41 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/evaluation/__init__.py
+-rw-rw-rw-   0        0        0    12675 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/evaluation/base.py
+-rw-rw-rw-   0        0        0     9213 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/evaluation/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.014993 DeepRetail-0.0.6/DeepRetail/exploratory/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/exploratory/__init__.py
+-rw-rw-rw-   0        0        0     2238 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/exploratory/eda.py
+-rw-rw-rw-   0        0        0     9337 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/exploratory/visuals.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.021993 DeepRetail-0.0.6/DeepRetail/forecasting/
+-rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/forecasting/__init__.py
+-rw-rw-rw-   0        0        0    21566 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/forecasting/ml.py
+-rw-rw-rw-   0        0        0    23005 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/forecasting/statistical.py
+-rw-rw-rw-   0        0        0     8229 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/forecasting/utils.py
+-rw-rw-rw-   0        0        0       49 2023-02-15 11:39:40.000000 DeepRetail-0.0.6/DeepRetail/hierarchical.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.032994 DeepRetail-0.0.6/DeepRetail/reconciliation/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:21:40.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/__init__.py
+-rw-rw-rw-   0        0        0    24670 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/cross_sectional.py
+-rw-rw-rw-   0        0        0    35145 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/cross_temporal.py
+-rw-rw-rw-   0        0        0    32997 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/temporal.py
+-rw-rw-rw-   0        0        0    18106 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.037993 DeepRetail-0.0.6/DeepRetail/transformations/
+-rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/transformations/__init__.py
+-rw-rw-rw-   0        0        0     9740 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/transformations/decomposition.py
+-rw-rw-rw-   0        0        0    14647 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/transformations/formats.py
+-rw-rw-rw-   0        0        0       61 2023-05-08 09:02:57.000000 DeepRetail-0.0.6/DeepRetail/version.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:04:06.997992 DeepRetail-0.0.6/DeepRetail.egg-info/
+-rw-rw-rw-   0        0        0     3799 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-06-19 22:52:26.000000 DeepRetail-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3799 2023-05-08 09:04:07.039993 DeepRetail-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3002 2023-05-08 09:02:57.000000 DeepRetail-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 09:04:07.040992 DeepRetail-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-05-08 09:02:57.000000 DeepRetail-0.0.6/setup.py
```

### Comparing `DeepRetail-0.0.5/DeepRetail/data/casereaders.py` & `DeepRetail-0.0.6/DeepRetail/data/casereaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,30 +519,34 @@
     # Adding any extra information. For example DF -> duty free
     products.loc[:, "Extras"] = [id[11:] if len(id) > 11 else np.nan for id in ids]
 
     # Drop a duplicate column
     products = products.drop("AANTAL_SIG", axis=1)
 
     # take items per products
-    print(products.columns)
+    # print(products.columns)
     item_per_prod = products[["PRODUCT_CODE", "Cigars_Num", "FAM"]]
 
     # Adding the number of cigars per product!
     df = pd.merge(df, item_per_prod, on="PRODUCT_CODE", how="left")
     # Multiply to get the cigars => the actual sales!
     df["Sales"] = df["QTY_INVOICED"] * df["Cigars_Num"]
     # Drop used columns
     df = df.drop(["Cigars_Num", "QTY_INVOICED"], axis=1)
 
+    # filter some nan values
+    df = df[~df['FAM'].isna()]
+    df = df.dropna()
+
     # groupby on product level
     df["product_id"] = [id.split("-")[0] for id in df["PRODUCT_CODE"]]
 
     # Add the family:
     df["product_id"] = [
-        str(fam) + str(id) for fam, id in zip(df["FAM"], df["product_id"])
+        str(fam) + '_' + str(id) for fam, id in zip(df["FAM"], df["product_id"])
     ]
 
     df = df.groupby(["product_id", "ORDER_DATE"]).agg({"Sales": "sum"}).reset_index()
 
     # keep columns
     cols = ["unique_id", "date", "y"]
     df.columns = cols
```

### Comparing `DeepRetail-0.0.5/DeepRetail/data/dataloader.py` & `DeepRetail-0.0.6/DeepRetail/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.5/DeepRetail/evaluation/base.py` & `DeepRetail-0.0.6/DeepRetail/evaluation/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from DeepRetail.transformations.formats import transaction_df, pivoted_df
 from DeepRetail.evaluation.metrics import mse, mae, rmsse, scaled_error
-from DeepRetail.visuals.evaluation import (
+from DeepRetail.exploratory.visuals import (
     visualize_forecasts,
     plot_single_hist_boxplot,
     plot_box,
     plot_line,
 )
 import pandas as pd
 
@@ -38,14 +38,52 @@
         scores_dict[name] = metric(
             true, forecasted, naive_mse=insample_mse, naive_mae=in_sample_mae
         )
 
     return pd.Series(scores_dict)
 
 
+def calculate_scores_updated(df, metrics):
+    """
+    Calculates the scores for the full dataframe.
+    An updated version
+
+    Args:
+        df (pd.DataFrame): The dataframe of predictions
+        metrics (list): A list of metrics to be calculated
+
+    Returns:
+        pd.DataFrame: A dataframe with the scores
+
+    """
+    # Get the names of the metrics
+    metric_names = [metric.__name__ for metric in metrics]
+    # Get the in-sample scores
+    in_sample_mse = df["in_sample_Naive_mse"].unique()[0]
+    in_sample_mae = df["in_sample_Naive_mae"].unique()[0]
+
+    # Drop the two columns
+    df = df.drop(["in_sample_Naive_mse", "in_sample_Naive_mae"], axis=1)
+
+    # Estimate the error
+    # For every metric:
+    for metric, name in zip(metrics, metric_names):
+        df[name] = df.apply(
+            lambda x: metric(
+                x["True"],
+                x["y"],
+                naive_mse=in_sample_mse,
+                naive_mae=in_sample_mae,
+            ),
+            axis=1,
+        )
+    # return
+    return df
+
+
 class Evaluator(object):
     """
     Class for evaluating the performance of a forecasting model.
 
     Args:
         original_df (pd.DataFrame): The original input DataFrame containing the time series data.
         result_df (pd.DataFrame): The DataFrame containing the predicted values.
@@ -146,15 +184,15 @@
 
         # Keeps only relevant columns
         in_sample_metrics = in_sample_metrics[
             ["in_sample_Naive_mse", "in_sample_Naive_mae"]
         ]
         return in_sample_metrics.reset_index()
 
-    def evaluate(self, metrics, group_scores_by=["unique_id", "Model", "fh", "cv"]):
+    def evaluate(self, metrics, group_scores_by=None, opperator="mean"):
         """
         Evaluates the predictions and calculates the specified metrics for each group.
 
         Args:
             metrics (list): A list of metrics to be calculated for each group. Each metric should be a function that
                             takes two arguments: a NumPy array of true values and a NumPy array of predicted values. The
                             list of metrics can also include optional arguments to be passed to the metric function.
@@ -170,26 +208,44 @@
 
         # Merge with the predictions dataframe
         merged_result_df = pd.merge(
             self.result_df, in_sample_metrics, on="unique_id", how="left"
         )
 
         # estimate the scores
-        evaluation_df = pd.DataFrame(
-            merged_result_df.groupby(group_scores_by).apply(
-                calculate_group_scores, metrics=metrics
+        evaluation_df = calculate_scores_updated(merged_result_df, metrics)
+
+        # Make some changes
+        metric_names = [metric.__name__ for metric in metrics]
+        cols_to_keep = ["unique_id", "Model", "fh", "cv"] + metric_names
+        
+        evaluation_df = evaluation_df[evaluation_df['Model'] != 'index']
+        evaluation_df = evaluation_df[cols_to_keep]
+
+        # do the grouping
+        if group_scores_by is not None:
+            evaluation_df = (
+                evaluation_df.groupby(group_scores_by).agg(opperator).reset_index()
             )
-        ).reset_index()
+
+
+        return evaluation_df
+
+        # evaluation_df = pd.DataFrame(
+        #    merged_result_df.groupby(group_scores_by).apply(
+        #        calculate_group_scores, metrics=metrics
+        #    )
+        # ).reset_index()
 
         # add the metrics to the object
         # self.evaluated_metrics = metrics
         # self.evaluate_df = evaluation_df
         # return self.evaluation_df
 
-        return evaluation_df
+        #return evaluation_df
 
     def plot_error_distribution(
         self,
         metrics=[rmsse, scaled_error],
         group_scores_by=["unique_id", "Model", "fh", "cv"],
     ):
         """
```

### Comparing `DeepRetail-0.0.5/DeepRetail/evaluation/metrics.py` & `DeepRetail-0.0.6/DeepRetail/evaluation/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,17 +113,17 @@
         predicted (np.array): The predicted values.
 
     Returns:
         np.array: The percentage error.
     """
 
     # % Error
-    return simple_error(actual, predicted) / (
-        actual + e
-    )  # The small e asserts that division is not with 0
+    # in case the actual is zero return zero
+    error = simple_error(actual, predicted, **kwargs)/actual if actual != 0 else 0
+    return error
 
 
 def naive_forecasts(actual, lag=1):
     """
     Calculates the naive forecasts for a given lag.
 
     Args:
@@ -300,9 +300,10 @@
     elif len(train) > 0:
         # Getting the naive predictions
         y_naive = naive_forecasts(train, lag)
         # And the mse
         denom = mse(train[lag:], y_naive)
     else:
         raise ValueError("Provide in-sample mse or the training data ")
-    error = np.sqrt(num / np.maximum(denom, e))
+    # error = np.sqrt(num / np.maximum(denom, e))
+    error = np.sqrt(num/denom) if denom != 0 else 0
     return error
```

### Comparing `DeepRetail-0.0.5/DeepRetail/forecasting/statistical.py` & `DeepRetail-0.0.6/DeepRetail/forecasting/statistical.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,14 +329,17 @@
 
         # Add to the object
         self.forecast_df = y_pred
 
         # add the fh and cv
         self.add_fh_cv()
 
+        # Remove the index from the models if there
+        self.forecast_df = self.forecast_df[self.forecast_df['Model'] != 'index']
+
         # return
         return self.forecast_df
 
     def add_fh_cv(self):
         """
         Adds the forecasting horizon and cross-validation information to the forecast results.
```

### Comparing `DeepRetail-0.0.5/DeepRetail/reconciliation/cross_sectional.py` & `DeepRetail-0.0.6/DeepRetail/reconciliation/cross_sectional.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.5/DeepRetail/reconciliation/cross_temporal.py` & `DeepRetail-0.0.6/DeepRetail/reconciliation/cross_temporal.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.5/DeepRetail/reconciliation/temporal.py` & `DeepRetail-0.0.6/DeepRetail/reconciliation/temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -580,15 +580,15 @@
         # I need to see how I will use the holdout and the cv paremeter
         self.original_df = original_df
 
         # If we have holdout:
         if self.holdout:
             # Initialize variables
 
-            end_point = self.bottom_level_numeric_freq + self.cv - 1
+            end_point = self.max_freq + self.cv - 1
 
             # Initialize lists for train and test
             self.resampled_train_dfs = []
             self.resampled_test_dfs = []
 
             for z in range(self.cv):
                 # Manual cross-validation
```

### Comparing `DeepRetail-0.0.5/DeepRetail/reconciliation/utils.py` & `DeepRetail-0.0.6/DeepRetail/reconciliation/utils.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.5/DeepRetail/transformations/formats.py` & `DeepRetail-0.0.6/DeepRetail/transformations/formats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+from DeepRetail.transformations.decomposition import MSTL
 
 
 def pivoted_df(df, target_frequency=None, agg_func=None, fill_values=True):
     """
     Converts a transaction df to a pivoted df.
     Each row is a unique id and columns are the dates.
     Missing values are filled with zeros by default.
@@ -375,7 +376,60 @@
         df["cross_sectional_level"] = df["cross_sectional_level"].astype(cat_dtype)
 
         # sort the dataframe based on the "levels" column
         df = df.sort_values(by="cross_sectional_level")
 
     # Return
     return df
+
+
+def get_reminder(df, periods):
+    """
+    Decompose a time series and return the residuals.
+
+    Args:
+        df (pd.DataFrame):
+            A DataFrame containing the time series data
+        periods (list):
+            A list of periods to use for the decomposition (e.g. [7, 30, 365])
+
+    Returns:
+        residuals (pd.DataFrame):
+            A DataFrame containing the residuals of the decomposition
+    """
+    # Extract the values of the DataFrame
+    vals = df.values
+
+    # Use the MSTL function to decompose the time series and extract the residuals
+    res_only = [MSTL(ts, periods=periods).fit().resid for ts in vals]
+
+    return res_only
+
+
+def MinMaxScaler_custom(x, feature_range=(0, 1)):
+    """
+    Performs MinMaxScaling on a numpy array.
+    Follows the documentation from sklearn.
+
+    Args:
+        x (np.array):
+            The array to be scaled.
+        feature_range (tuple):
+            The range of the output.
+
+    Returns:
+        np.array:
+            The scaled array.
+
+    References:
+         https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html
+    """
+
+    # Extract some values
+    x_min, x_max = x.min(), x.max()
+    feature_min, feature_max = feature_range
+
+    # Perform scalling
+    X_std = (x - x_min) / (x_max - x_min)
+    X_scaled = X_std * (feature_max - feature_min) + feature_min
+
+    return X_scaled
```

### Comparing `DeepRetail-0.0.5/DeepRetail/visuals/evaluation.py` & `DeepRetail-0.0.6/DeepRetail/exploratory/visuals.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.5/DeepRetail.egg-info/PKG-INFO` & `DeepRetail-0.0.6/DeepRetail.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepRetail
-Version: 0.0.5
+Version: 0.0.6
 Summary: Forecasting package for retail using Deep Learning AI.
 Home-page: https://github.com/yForecasting/DeepRetail
 Author: Yves R. Sagaert
 Author-email: yves.r.sagaert@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeepRetail
-<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.5-blue">
+<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.6-blue">
 
 Python package on deep learning AI and machine learning for Retail
 
 This package is developed by the AI team at [VIVES University of Applied Sciences](https://www.vives.be/en/research/centre-expertise-business-management) and is used in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/).
 
 ___
 
@@ -99,8 +99,8 @@
 
 
 ## Disclaimer
 `DeepRetail` is an open-source package. We do our best to make this package robust and stable, but we do not take liability for any errors or instability. 
 
 ## Support
 
-The [AI team](https://yforecasting.github.io/) at VIVES University of Applied Sciences builds and maintains `DeepRetail` to make it simple and accessible. We are using this software in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/). A special thanks to Ruben Vanhecke and Filotas Theodosiou for their contribution.
+The [AI team](https://yforecasting.github.io/) at VIVES University of Applied Sciences builds and maintains `DeepRetail` to make it simple and accessible. We are using this software in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/). A special thanks to Ruben Vanhecke and Filotas Theodosiou for their contribution. The [maintenance workflow](https://github.com/yForecasting/DeepRetail/blob/main/MAINTAINING.md) can be found here.
```

### Comparing `DeepRetail-0.0.5/DeepRetail.egg-info/SOURCES.txt` & `DeepRetail-0.0.6/DeepRetail.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 DeepRetail.egg-info/top_level.txt
 DeepRetail/data/__init__.py
 DeepRetail/data/casereaders.py
 DeepRetail/data/dataloader.py
 DeepRetail/evaluation/__init__.py
 DeepRetail/evaluation/base.py
 DeepRetail/evaluation/metrics.py
+DeepRetail/exploratory/__init__.py
+DeepRetail/exploratory/eda.py
+DeepRetail/exploratory/visuals.py
 DeepRetail/forecasting/__init__.py
+DeepRetail/forecasting/ml.py
 DeepRetail/forecasting/statistical.py
 DeepRetail/forecasting/utils.py
 DeepRetail/reconciliation/__init__.py
 DeepRetail/reconciliation/cross_sectional.py
 DeepRetail/reconciliation/cross_temporal.py
 DeepRetail/reconciliation/temporal.py
 DeepRetail/reconciliation/utils.py
 DeepRetail/transformations/__init__.py
-DeepRetail/transformations/formats.py
-DeepRetail/visuals/__init__.py
-DeepRetail/visuals/evaluation.py
+DeepRetail/transformations/decomposition.py
+DeepRetail/transformations/formats.py
```

### Comparing `DeepRetail-0.0.5/LICENSE` & `DeepRetail-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.5/PKG-INFO` & `DeepRetail-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepRetail
-Version: 0.0.5
+Version: 0.0.6
 Summary: Forecasting package for retail using Deep Learning AI.
 Home-page: https://github.com/yForecasting/DeepRetail
 Author: Yves R. Sagaert
 Author-email: yves.r.sagaert@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeepRetail
-<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.5-blue">
+<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.6-blue">
 
 Python package on deep learning AI and machine learning for Retail
 
 This package is developed by the AI team at [VIVES University of Applied Sciences](https://www.vives.be/en/research/centre-expertise-business-management) and is used in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/).
 
 ___
 
@@ -99,8 +99,8 @@
 
 
 ## Disclaimer
 `DeepRetail` is an open-source package. We do our best to make this package robust and stable, but we do not take liability for any errors or instability. 
 
 ## Support
 
-The [AI team](https://yforecasting.github.io/) at VIVES University of Applied Sciences builds and maintains `DeepRetail` to make it simple and accessible. We are using this software in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/). A special thanks to Ruben Vanhecke and Filotas Theodosiou for their contribution.
+The [AI team](https://yforecasting.github.io/) at VIVES University of Applied Sciences builds and maintains `DeepRetail` to make it simple and accessible. We are using this software in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/). A special thanks to Ruben Vanhecke and Filotas Theodosiou for their contribution. The [maintenance workflow](https://github.com/yForecasting/DeepRetail/blob/main/MAINTAINING.md) can be found here.
```

### Comparing `DeepRetail-0.0.5/README.md` & `DeepRetail-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DeepRetail
-<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.5-blue">
+<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.6-blue">
 
 Python package on deep learning AI and machine learning for Retail
 
 This package is developed by the AI team at [VIVES University of Applied Sciences](https://www.vives.be/en/research/centre-expertise-business-management) and is used in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/).
 
 ___
 
@@ -79,8 +79,8 @@
 
 
 ## Disclaimer
 `DeepRetail` is an open-source package. We do our best to make this package robust and stable, but we do not take liability for any errors or instability. 
 
 ## Support
 
-The [AI team](https://yforecasting.github.io/) at VIVES University of Applied Sciences builds and maintains `DeepRetail` to make it simple and accessible. We are using this software in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/). A special thanks to Ruben Vanhecke and Filotas Theodosiou for their contribution.
+The [AI team](https://yforecasting.github.io/) at VIVES University of Applied Sciences builds and maintains `DeepRetail` to make it simple and accessible. We are using this software in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/). A special thanks to Ruben Vanhecke and Filotas Theodosiou for their contribution. The [maintenance workflow](https://github.com/yForecasting/DeepRetail/blob/main/MAINTAINING.md) can be found here.
```

### Comparing `DeepRetail-0.0.5/setup.py` & `DeepRetail-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 
 setuptools.setup(
     author="Yves R. Sagaert",
     author_email="yves.r.sagaert@gmail.com",
     name='DeepRetail',
     license="GNU GPLv3",
     description='Forecasting package for retail using Deep Learning AI.',
-    version='v0.0.5',
+    version='v0.0.6',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/yForecasting/DeepRetail',
     packages=setuptools.find_packages(),
     include_package_data=True,
     python_requires=">=3.5",
     # Enable install requires when publishing on the normal PyPi
     install_requires=[
         'pandas',
         'matplotlib',
         'numpy',
         'statsforecast',
         'numba',
-        'openpyxl'
+        'openpyxl',
+        'tsfeatures',
+        'statsmodels'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
```


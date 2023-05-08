# Comparing `tmp/auto_ts-0.0.69.tar.gz` & `tmp/auto_ts-0.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_ts-0.0.69.tar", last modified: Fri Mar 24 12:39:14 2023, max compression
+gzip compressed data, was "auto_ts-0.0.70.tar", last modified: Mon May  8 12:30:57 2023, max compression
```

## Comparing `auto_ts-0.0.69.tar` & `auto_ts-0.0.70.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-03-24 12:39:14.089576 auto_ts-0.0.69/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14603 2023-03-24 12:39:14.084579 auto_ts-0.0.69/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12805 2023-02-22 13:28:29.000000 auto_ts-0.0.69/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-03-24 12:39:13.053693 auto_ts-0.0.69/auto_ts/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    56556 2022-08-16 12:09:26.000000 auto_ts-0.0.69/auto_ts/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      370 2023-02-22 13:29:39.000000 auto_ts-0.0.69/auto_ts/__version__.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-03-24 12:39:13.341993 auto_ts-0.0.69/auto_ts/models/
--rwxrwxrwx   0 ram       (1000) ram       (1000)      229 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/__init__.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-03-24 12:39:13.622229 auto_ts-0.0.69/auto_ts/models/ar_based/
--rwxrwxrwx   0 ram       (1000) ram       (1000)      159 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/ar_based/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11666 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/ar_based/build_arima.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    16410 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/ar_based/build_arima_base.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     4148 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/ar_based/build_autoarimax.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18472 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/ar_based/build_sarimax.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12940 2022-01-17 23:08:01.000000 auto_ts-0.0.69/auto_ts/models/ar_based/build_var.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     6502 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/ar_based/param_finder.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     3061 2022-08-16 11:58:44.000000 auto_ts-0.0.69/auto_ts/models/build_base.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    62805 2023-03-24 12:28:54.000000 auto_ts-0.0.69/auto_ts/models/build_ml.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    28728 2023-02-22 13:28:29.000000 auto_ts-0.0.69/auto_ts/models/build_prophet.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     5032 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/models/build_pyflux.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    30950 2022-01-30 16:58:11.000000 auto_ts-0.0.69/auto_ts/models/ml_models.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-03-24 12:39:13.772907 auto_ts-0.0.69/auto_ts/test/
--rwxrwxrwx   0 ram       (1000) ram       (1000)        0 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/test/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2921 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/test/test_auto_sarimax.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    79421 2023-02-22 13:28:30.000000 auto_ts-0.0.69/auto_ts/test/test_auto_ts.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12037 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/test/test_var.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-03-24 12:39:14.039575 auto_ts-0.0.69/auto_ts/utils/
--rwxrwxrwx   0 ram       (1000) ram       (1000)      710 2022-01-23 02:50:48.000000 auto_ts-0.0.69/auto_ts/utils/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      246 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/utils/colors.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17493 2023-03-24 12:34:01.000000 auto_ts-0.0.69/auto_ts/utils/eda.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    25349 2022-01-30 16:19:03.000000 auto_ts-0.0.69/auto_ts/utils/etl.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1264 2021-08-27 20:33:30.000000 auto_ts-0.0.69/auto_ts/utils/logging.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     4782 2021-12-07 02:01:15.000000 auto_ts-0.0.69/auto_ts/utils/metrics.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11033 2022-01-22 20:15:38.000000 auto_ts-0.0.69/auto_ts/utils/my_encoders.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     9979 2021-12-07 01:54:05.000000 auto_ts-0.0.69/auto_ts/utils/val.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-03-24 12:39:13.168690 auto_ts-0.0.69/auto_ts.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14603 2023-03-24 12:39:12.000000 auto_ts-0.0.69/auto_ts.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      975 2023-03-24 12:39:12.000000 auto_ts-0.0.69/auto_ts.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-03-24 12:39:12.000000 auto_ts-0.0.69/auto_ts.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      181 2023-03-24 12:39:12.000000 auto_ts-0.0.69/auto_ts.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-03-24 12:39:12.000000 auto_ts-0.0.69/auto_ts.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-03-24 12:39:14.092579 auto_ts-0.0.69/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1072 2023-03-24 12:36:58.000000 auto_ts-0.0.69/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.808270 auto_ts-0.0.70/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15123 2023-05-08 12:30:57.808270 auto_ts-0.0.70/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13237 2023-03-27 12:13:14.000000 auto_ts-0.0.70/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:56.890657 auto_ts-0.0.70/auto_ts/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    56587 2023-05-08 11:45:35.000000 auto_ts-0.0.70/auto_ts/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      370 2023-05-07 15:58:16.000000 auto_ts-0.0.70/auto_ts/__version__.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.153786 auto_ts-0.0.70/auto_ts/models/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      229 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/__init__.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.432228 auto_ts-0.0.70/auto_ts/models/ar_based/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      159 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11666 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_arima.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    16527 2023-05-08 11:46:10.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_arima_base.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     4148 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_autoarimax.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18472 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_sarimax.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12940 2022-01-17 23:08:01.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_var.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     6502 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/param_finder.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     3061 2022-08-16 11:58:44.000000 auto_ts-0.0.70/auto_ts/models/build_base.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    62805 2023-03-24 12:28:54.000000 auto_ts-0.0.70/auto_ts/models/build_ml.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    28736 2023-05-08 11:21:05.000000 auto_ts-0.0.70/auto_ts/models/build_prophet.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     5032 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/build_pyflux.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    30950 2022-01-30 16:58:11.000000 auto_ts-0.0.70/auto_ts/models/ml_models.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.587582 auto_ts-0.0.70/auto_ts/test/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        0 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/test/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     2921 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/test/test_auto_sarimax.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    79421 2023-02-22 13:28:30.000000 auto_ts-0.0.70/auto_ts/test/test_auto_ts.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12037 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/test/test_var.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.792641 auto_ts-0.0.70/auto_ts/utils/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      710 2022-01-23 02:50:48.000000 auto_ts-0.0.70/auto_ts/utils/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      246 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/utils/colors.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17493 2023-03-24 12:34:01.000000 auto_ts-0.0.70/auto_ts/utils/eda.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    25355 2023-05-07 16:15:31.000000 auto_ts-0.0.70/auto_ts/utils/etl.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1264 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/utils/logging.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     5020 2023-05-08 12:21:03.000000 auto_ts-0.0.70/auto_ts/utils/metrics.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11033 2022-01-22 20:15:38.000000 auto_ts-0.0.70/auto_ts/utils/my_encoders.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     9979 2021-12-07 01:54:05.000000 auto_ts-0.0.70/auto_ts/utils/val.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.006638 auto_ts-0.0.70/auto_ts.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15123 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      975 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      181 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-05-08 12:30:57.823891 auto_ts-0.0.70/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1072 2023-03-27 12:09:31.000000 auto_ts-0.0.70/setup.py
```

### Comparing `auto_ts-0.0.69/PKG-INFO` & `auto_ts-0.0.70/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: auto_ts
-Version: 0.0.69
+Version: 0.0.70
 Summary: Automatically Build Multiple Time Series models fast - now with Facebook Prophet!
 Home-page: https://github.com/AutoViML/Auto_TS
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: <!DOCTYPE html>
         <html>
         <head>
         </head>
         <body>
         
         ![auto-ts](logo.png)
         
+        <h1 id="mar-update">March 2023 Update:</h1>
+        <p style="font-family:verdana">We have now upgraded FB Prophet to the latest version which is simply called prophet. <br>
+        If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise error!):
+        
+        ```
+        !pip install auto-ts --no-deps --ignore-installed
+        !pip install 'fsspec>=0.3.3'
+        !pip install statsmodels --upgrade
+        !pip install pmdarima
+        ```
+        
         <h1 id="aug-update">Aug 2022 Update:</h1>
         <p style="font-family:verdana">You can now add FB Prophet arguments directly into Auto_TimeSeries using the kwargs argument. See example below:
         
         ![fb-prophet](add_fb_prophet.png)
         
         <h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
         <p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.</p>
```

#### html2text {}

```diff
@@ -1,12 +1,19 @@
-Metadata-Version: 2.1 Name: auto_ts Version: 0.0.69 Summary: Automatically
+Metadata-Version: 2.1 Name: auto_ts Version: 0.0.70 Summary: Automatically
 Build Multiple Time Series models fast - now with Facebook Prophet! Home-page:
 https://github.com/AutoViML/Auto_TS Author: Ram Seshadri License: Apache
 License 2.0 Description:
 ![auto-ts](logo.png)
+****** March 2023 Update: ******
+We have now upgraded FB Prophet to the latest version which is simply called
+prophet.
+If you are using Colab or Kaggle kernel and want to install auto_ts, please use
+the following steps (otherwise error!): ``` !pip install auto-ts --no-deps --
+ignore-installed !pip install 'fsspec>=0.3.3' !pip install statsmodels --
+upgrade !pip install pmdarima ```
 ****** Aug 2022 Update: ******
 You can now add FB Prophet arguments directly into Auto_TimeSeries using the
 kwargs argument. See example below: ![fb-prophet](add_fb_prophet.png)
 ****** Auto_TS: Auto_TimeSeries ******
 Automatically build multiple Time Series models using a Single Line of Code.
 Now updated with Dask.
 Auto_timeseries is a complex model building utility for time series data. Since
```

### Comparing `auto_ts-0.0.69/README.md` & `auto_ts-0.0.70/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 <html>
 <head>
 </head>
 <body>
 
 ![auto-ts](logo.png)
 
+<h1 id="mar-update">March 2023 Update:</h1>
+<p style="font-family:verdana">We have now upgraded FB Prophet to the latest version which is simply called prophet. <br>
+If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise error!):
+
+```
+!pip install auto-ts --no-deps --ignore-installed
+!pip install 'fsspec>=0.3.3'
+!pip install statsmodels --upgrade
+!pip install pmdarima
+```
+
 <h1 id="aug-update">Aug 2022 Update:</h1>
 <p style="font-family:verdana">You can now add FB Prophet arguments directly into Auto_TimeSeries using the kwargs argument. See example below:
 
 ![fb-prophet](add_fb_prophet.png)
 
 <h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
 <p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,15 @@
 ![auto-ts](logo.png)
+****** March 2023 Update: ******
+We have now upgraded FB Prophet to the latest version which is simply called
+prophet.
+If you are using Colab or Kaggle kernel and want to install auto_ts, please use
+the following steps (otherwise error!): ``` !pip install auto-ts --no-deps --
+ignore-installed !pip install 'fsspec>=0.3.3' !pip install statsmodels --
+upgrade !pip install pmdarima ```
 ****** Aug 2022 Update: ******
 You can now add FB Prophet arguments directly into Auto_TimeSeries using the
 kwargs argument. See example below: ![fb-prophet](add_fb_prophet.png)
 ****** Auto_TS: Auto_TimeSeries ******
 Automatically build multiple Time Series models using a Single Line of Code.
 Now updated with Dask.
 Auto_timeseries is a complex model building utility for time series data. Since
```

### Comparing `auto_ts-0.0.69/auto_ts/__init__.py` & `auto_ts-0.0.70/auto_ts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,15 +664,15 @@
 
             self.ml_dict[name]['model'] = model
             self.ml_dict[name]['forecast'] = forecast_df_folds
             self.ml_dict[name][self.score_type] = score_val
             self.ml_dict[name]['model_build'] = model_build
 
 
-        if self.__any_contained_in_list(what_list=['var','Var','VAR', 'stats', 'best'], in_list=self.model_type):
+        if self.__any_contained_in_list(what_list=['var','Var','VAR', 'best'], in_list=self.model_type):
             ########### Let's build a VAR Model - but first we have to shift the predictor vars ####
 
             if ts_df.shape[0] > 1000 and self.__any_contained_in_list(what_list=['stats', 'best'], in_list=self.model_type):
                 print(colorful.BOLD + '\n===============================================' + colorful.END)
                 print("Skipping VAR Model since dataset is > 1000 rows and it will take too long")
                 print(colorful.BOLD + '===============================================' + colorful.END)
             else:
@@ -968,20 +968,20 @@
             bestmodel = self.get_best_model_build()
             self.model = bestmodel
         ##### Now make predictions using model given ######
         try:
             if isinstance(testdata, pd.Series) or isinstance(testdata, pd.DataFrame):
                 # During training, we internally converted a column datetime index to the dataframe date time index
                 # We need to do the same while predicing for consistence
-                if (model == 'ML') or self.get_best_model_name() == 'ML' or (model == 'best' and self.get_best_model_name() == 'ML'):
+                if (model.lower() == 'ml') or self.get_best_model_name().lower() == 'ml' or (model.lower() == 'best' and self.get_best_model_name().lower() == 'ml'):
                     ### Now do the predictions using the final model asked to be predicted ###
                     predictions = bestmodel.predict(testdata,simple=simple, time_interval=time_interval)
                 elif model.lower() == 'prophet' or self.get_best_model_name() == 'Prophet':
                     predictions = bestmodel.predict(testdata,simple=simple)
-                elif self.get_best_model_name() == 'VAR':
+                elif self.get_best_model_name().lower() == 'var':
                     predictions = bestmodel.predict(testdata,simple=simple)
                 else:
                     predictions = bestmodel.predict(testdata,simple=simple)
             elif type(testdata) == dask.dataframe.core.DataFrame:
                 # During training, we internally converted a column datetime index to the dataframe date time index
                 # We need to do the same while predicing for consistence
                 if (model == 'ML') or self.get_best_model_name() == 'ML' or (model == 'best' and self.get_best_model_name() == 'ML'):
```

### Comparing `auto_ts-0.0.69/auto_ts/models/ar_based/build_arima.py` & `auto_ts-0.0.70/auto_ts/models/ar_based/build_arima.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/ar_based/build_arima_base.py` & `auto_ts-0.0.70/auto_ts/models/ar_based/build_arima_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,18 @@
             # (sklearn) based cross_val_score, we need to do this since we dont get individual folds
             # back for cross_val_score. If at a later point in time, we can get this, then,
             # we can revert back to dividing by individual fold std values.
             norm_rmse_folds2 = rmse_folds/ts_df[self.original_target_col].values.std()  # Same as what was there in print_dynamic_rmse()
 
             print(f"\nSARIMAX RMSE (all folds): {np.mean(rmse_folds):.4f}")
             print(f"SARIMAX Norm RMSE (all folds): {(np.mean(norm_rmse_folds2)*100):.0f}%\n")
-            print_ts_model_stats(extra_concatenated['original'],extra_concatenated['predicted'], "auto_SARIMAX")
+            try:
+                print_ts_model_stats(extra_concatenated['original'],extra_concatenated['predicted'], "auto_SARIMAX")
+            except:
+                print('Unable to print model stats. Continuing...')
 
         ###############################################
         #### Refit the model on the entire dataset ####
         ###############################################
         auto_arima_model = self.find_best_parameters(data = ts_df)
         self.model = auto_arima_model
         self.refit(ts_df=ts_df)
@@ -350,15 +353,15 @@
             else:
                 try:
                     res = self.model.get_forecast(self.forecast_period)
                 except Exception as e:
                     print(e)
                     print("Model was trained with train dataframe. Please make sure you are passing a test data frame.")
                     return
-
+        
         res_frame = res.summary_frame()
         res_frame.rename(columns = {'mean':'yhat'}, inplace=True)
 
         if simple:
             res_frame = res_frame['yhat']
             res_frame = res_frame.squeeze() # Convert to a pandas series object
         else:
```

### Comparing `auto_ts-0.0.69/auto_ts/models/ar_based/build_autoarimax.py` & `auto_ts-0.0.70/auto_ts/models/ar_based/build_autoarimax.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/ar_based/build_sarimax.py` & `auto_ts-0.0.70/auto_ts/models/ar_based/build_sarimax.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/ar_based/build_var.py` & `auto_ts-0.0.70/auto_ts/models/ar_based/build_var.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/ar_based/param_finder.py` & `auto_ts-0.0.70/auto_ts/models/ar_based/param_finder.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/build_base.py` & `auto_ts-0.0.70/auto_ts/models/build_base.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/build_ml.py` & `auto_ts-0.0.70/auto_ts/models/build_ml.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/build_prophet.py` & `auto_ts-0.0.70/auto_ts/models/build_prophet.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
             #cv_micro = np.sqrt(mean_squared_error(y_trues.values, y_preds.values))
             #print('Average CV RMSE of all predictions (micro) = %0.5f' %cv_micro)
 
             try:
                 print_ts_model_stats(extra_concatenated['original'], extra_concatenated['predicted'], "Prophet")
             except:
-                print('Error: Not able to plot Prophet CV results')
+                print('Not able to plot Prophet CV results. Continuing...')
 
             forecast_df_folds = extra_concatenated['predicted'].values
             #print("  End of Prophet Cross Validation")
             print('Time Taken = %0.0f seconds' %((time.time()-start_time)))
 
         #### Now you need to fit Prophet on the whole train data set ##########
         dftx = dft.head(len(dft))
```

### Comparing `auto_ts-0.0.69/auto_ts/models/build_pyflux.py` & `auto_ts-0.0.70/auto_ts/models/build_pyflux.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/models/ml_models.py` & `auto_ts-0.0.70/auto_ts/models/ml_models.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/test/test_auto_sarimax.py` & `auto_ts-0.0.70/auto_ts/test/test_auto_sarimax.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/test/test_auto_ts.py` & `auto_ts-0.0.70/auto_ts/test/test_auto_ts.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/test/test_var.py` & `auto_ts-0.0.70/auto_ts/test/test_var.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/utils/__init__.py` & `auto_ts-0.0.70/auto_ts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/utils/eda.py` & `auto_ts-0.0.70/auto_ts/utils/eda.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/utils/etl.py` & `auto_ts-0.0.70/auto_ts/utils/etl.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         If dask_xgboost_flag is set to True it returns both a dask as well as pandas DataFrame.
         If dask_xgboost_flag is set to False it returns both of them as pandas DataFrames.
 
     Outputs:
         dft: dask DataFrame
         filename: pandas DataFrame
     """
+    
     if isinstance(filename, str):
         filename = pd.read_csv(filename, sep=sep, parse_dates=[ts_column])
     ### If filename is not a string, it must be a dataframe and can be loaded
     if dask_xgboost_flag:
         if type(filename) == dask.dataframe.core.DataFrame:
             print('    Since dask_xgboost_flag is True, and input is dask, continuing...')
         else:
```

### Comparing `auto_ts-0.0.69/auto_ts/utils/logging.py` & `auto_ts-0.0.70/auto_ts/utils/logging.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/utils/metrics.py` & `auto_ts-0.0.70/auto_ts/utils/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Tuple
 import numpy as np  # type: ignore
 import pandas as pd  # type: ignore
 import matplotlib.pyplot as plt # type: ignore
 from sklearn.metrics import mean_absolute_error, mean_squared_error # type: ignore
-
+import pdb
 
 def print_static_rmse(actual: np.array, predicted: np.array, start_from: int=0, verbose: int=0):
     """
     this calculates the ratio of the rmse error to the standard deviation of the actuals.
     This ratio should be below 1 for a model to be considered useful.
     The comparison starts from the row indicated in the "start_from" variable.
     """
@@ -47,54 +47,61 @@
     norm_rmse = rmse/actuals.std()
     print('RMSE = {:,.2f}'.format(rmse))
     print('Std Deviation of Actuals = {:,.2f}'.format(actuals.std()))
     print('Normalized RMSE = %0.0f%%' %(100*norm_rmse))
     return rmse, norm_rmse
 
 
-def print_rmse(y: np.array, y_hat: np.array) -> float:
+def print_rmse(y: np.array, y_hat: np.array):
     """
     Calculating Root Mean Square Error https://en.wikipedia.org/wiki/Root-mean-square_deviation
     """
     mse = np.mean((y - y_hat)**2)
     return np.sqrt(mse)
 
 
-def print_mape(y: np.array, y_hat: np.array) -> float:
+def print_mape(y: np.array, y_hat: np.array):
     """
     Calculating Mean Absolute Percent Error https://en.wikipedia.org/wiki/Mean_absolute_percentage_error
     """
     try:
         perc_err = (100*(y - y_hat))/y
         return np.mean(abs(perc_err))
     except:
         return np.nan
-import pdb
+
+
 def print_ts_model_stats(actuals: np.array, predicted: np.array, title="Model"):
     """
     This program prints and returns MAE, RMSE, MAPE.
     If you like the MAE and RMSE as a percentage of something, just give that number
     in the input as "number_as_percentage" and it will return the MAE and RMSE as a
     ratio of that number. Returns MAE, MAE_as_percentage, and RMSE_as_percentage
     """
-    number_as_percentage = actuals.std()
-    plt.figure(figsize=(15,8))
-    dfplot = pd.DataFrame([actuals,predicted]).T
-    dfplot.columns = ['Actual','Forecast']
-    dfplot = dfplot.sort_index()
-    plt.plot(dfplot)
-    plt.legend(['actual','forecast'])
-    plt.title('%s: Actual vs Forecast in expanding (training) Window Cross Validation' %title, fontsize=20)
+    try:
+        number_as_percentage = actuals.std()
+        if (predicted.index == actuals.index).all():
+            dfplot = pd.DataFrame(actuals).join(pd.DataFrame(predicted))
+        else:
+            dfplot = pd.DataFrame([actuals.values, predicted.values]).T
+            dfplot.columns = ['Actual','Forecast']
+        dfplot = dfplot.sort_index()
+        plt.figure(figsize=(15,8))
+        plt.plot(dfplot)
+        plt.legend(['original','predicted'])
+        plt.title('%s: Actual vs Forecast in expanding (training) Window Cross Validation' %title, fontsize=20)
+    except:
+        pass
     print('\n-------------------------------------------')
     print('Model Cross Validation Results:')
     print('-------------------------------------------')
     mae = mean_absolute_error(actuals, predicted)
     mse = mean_squared_error(actuals, predicted)
     print('    MAE (Mean Absolute Error = %0.2f' %mae)
-    rmse = print_rmse(actuals, predicted)
+    rmse = np.sqrt(mean_squared_error(actuals,predicted))
     print('    MSE (Mean Squared Error = %0.2f' %mse)
     mape = print_mape(actuals, predicted)
     print("    MAPE (Mean Absolute Percent Error) = %0.0f%%" %(mape))
     print("    RMSE (Root Mean Squared Error) = %0.04f" %(rmse))
     # Normalized RMSE print('RMSE = {:,.Of}'.format(rmse))
     print('    Normalized RMSE (MinMax) = %0.0f%%' %(100*rmse/abs(actuals.max()-actuals.min())))
     rmse_asp = (np.sqrt(mean_squared_error(actuals,predicted))/number_as_percentage)*100
```

### Comparing `auto_ts-0.0.69/auto_ts/utils/my_encoders.py` & `auto_ts-0.0.70/auto_ts/utils/my_encoders.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts/utils/val.py` & `auto_ts-0.0.70/auto_ts/utils/val.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/auto_ts.egg-info/PKG-INFO` & `auto_ts-0.0.70/auto_ts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: auto-ts
-Version: 0.0.69
+Version: 0.0.70
 Summary: Automatically Build Multiple Time Series models fast - now with Facebook Prophet!
 Home-page: https://github.com/AutoViML/Auto_TS
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: <!DOCTYPE html>
         <html>
         <head>
         </head>
         <body>
         
         ![auto-ts](logo.png)
         
+        <h1 id="mar-update">March 2023 Update:</h1>
+        <p style="font-family:verdana">We have now upgraded FB Prophet to the latest version which is simply called prophet. <br>
+        If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise error!):
+        
+        ```
+        !pip install auto-ts --no-deps --ignore-installed
+        !pip install 'fsspec>=0.3.3'
+        !pip install statsmodels --upgrade
+        !pip install pmdarima
+        ```
+        
         <h1 id="aug-update">Aug 2022 Update:</h1>
         <p style="font-family:verdana">You can now add FB Prophet arguments directly into Auto_TimeSeries using the kwargs argument. See example below:
         
         ![fb-prophet](add_fb_prophet.png)
         
         <h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
         <p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.</p>
```

#### html2text {}

```diff
@@ -1,12 +1,19 @@
-Metadata-Version: 2.1 Name: auto-ts Version: 0.0.69 Summary: Automatically
+Metadata-Version: 2.1 Name: auto-ts Version: 0.0.70 Summary: Automatically
 Build Multiple Time Series models fast - now with Facebook Prophet! Home-page:
 https://github.com/AutoViML/Auto_TS Author: Ram Seshadri License: Apache
 License 2.0 Description:
 ![auto-ts](logo.png)
+****** March 2023 Update: ******
+We have now upgraded FB Prophet to the latest version which is simply called
+prophet.
+If you are using Colab or Kaggle kernel and want to install auto_ts, please use
+the following steps (otherwise error!): ``` !pip install auto-ts --no-deps --
+ignore-installed !pip install 'fsspec>=0.3.3' !pip install statsmodels --
+upgrade !pip install pmdarima ```
 ****** Aug 2022 Update: ******
 You can now add FB Prophet arguments directly into Auto_TimeSeries using the
 kwargs argument. See example below: ![fb-prophet](add_fb_prophet.png)
 ****** Auto_TS: Auto_TimeSeries ******
 Automatically build multiple Time Series models using a Single Line of Code.
 Now updated with Dask.
 Auto_timeseries is a complex model building utility for time series data. Since
```

### Comparing `auto_ts-0.0.69/auto_ts.egg-info/SOURCES.txt` & `auto_ts-0.0.70/auto_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.69/setup.py` & `auto_ts-0.0.70/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="auto_ts",
-    version="0.0.69",
+    version="0.0.70",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Build Multiple Time Series models fast - now with Facebook Prophet!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/Auto_TS",
```


# Comparing `tmp/phdu-1.9b1.tar.gz` & `tmp/phdu-1.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.9b1.tar", last modified: Mon May  8 08:08:51 2023, max compression
+gzip compressed data, was "phdu-1.9b2.tar", last modified: Mon May  8 08:19:46 2023, max compression
```

## Comparing `phdu-1.9b1.tar` & `phdu-1.9b2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.9b1/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:08:51.302374 phdu-1.9b1/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.9b1/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.299040 phdu-1.9b1/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.9b1/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.9b1/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    30838 2023-05-08 08:08:03.000000 phdu-1.9b1/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.9b1/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.299040 phdu-1.9b1/phdu.egg-info/
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/requires.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-05-08 08:08:51.302374 phdu-1.9b1/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-05-08 08:08:40.000000 phdu-1.9b1/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.238990 phdu-1.9b2/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.9b2/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:19:46.238990 phdu-1.9b2/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.9b2/README.md
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu/
+-rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/clustering.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/decomposition.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/np_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/pd_utils.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu/plots/
+-rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/plots/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/plots/_mpl.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/plots/base.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.9b2/phdu/plots/plotly_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/script_fmt.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu/stats/
+-rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/_integration.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.9b2/phdu/stats/_plots.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/_preprocess.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    30742 2023-05-08 08:18:56.000000 phdu-1.9b2/phdu/stats/bootstrap.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/conf_interval.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/corr.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.238990 phdu-1.9b2/phdu/stats/rtopy/
+-rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.238990 phdu-1.9b2/phdu/stats/test/
+-rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/test/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/test/_adherence.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/test/permutation.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.9b2/phdu/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu.egg-info/
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/requires.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/top_level.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-05-08 08:19:46.238990 phdu-1.9b2/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-05-08 08:19:41.000000 phdu-1.9b2/setup.py
```

### Comparing `phdu-1.9b1/LICENSE.md` & `phdu-1.9b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/PKG-INFO` & `phdu-1.9b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b1
+Version: 1.9b2
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b1/README.md` & `phdu-1.9b2/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/_helper.py` & `phdu-1.9b2/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/clustering.py` & `phdu-1.9b2/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/decomposition.py` & `phdu-1.9b2/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/np_utils.py` & `phdu-1.9b2/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/pd_utils.py` & `phdu-1.9b2/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/plots/base.py` & `phdu-1.9b2/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/plots/plotly_utils.py` & `phdu-1.9b2/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/script_fmt.py` & `phdu-1.9b2/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/stats/_integration.py` & `phdu-1.9b2/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/stats/_plots.py` & `phdu-1.9b2/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/stats/bootstrap.py` & `phdu-1.9b2/phdu/stats/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     """
     B = a.shape[axis]
     if account_equal:
         return ((a < score).sum(axis=axis) + (a <= score).sum(axis=axis)) / (2 * B)
     else:
         return (a < score).sum(axis=axis) / B
 
-def _resample(data, data2, use_numba, statistic, R, n_min=5, smooth=False, stack_data=True, aggregator=_nb_mean, **kwargs):
+def _resample(data, data2, use_numba, statistic, R, n_min=5, smooth=False, aggregator=_nb_mean, **kwargs):
     """
     Resample using normal resampling if data2 is None.
     Else uses block resampling with data and data2.
     """
     if data2 is None:
         if data.ndim == 1:
             data = data[:, None]
@@ -295,22 +295,22 @@
             theta_hat_b = None
         else:
             resample_func = resample_nb if use_numba else resample
             theta_hat_b = resample_func(data, statistic, R=R, output_len=output_len, smooth=smooth, **kwargs).squeeze()
     else:
         is_block = isinstance(data, tuple)
         if is_block:
-            if stack_data:
-                sample_stat = statistic(np.hstack(data), np.hstack(data2))
-            else:
-                sample_stat = statistic(np.array([aggregator(di) for di in data]), np.array([aggregator(di) for di in data2]))
+            # if stack_data:
+            #     sample_stat = statistic(np.hstack(data), np.hstack(data2))
+            # else:
+            sample_stat = statistic(np.array([aggregator(di) for di in data]), np.array([aggregator(di) for di in data2]))
             total_N = lambda data: np.sum([d.shape[0] for d in data])
             N = min([total_N(data), total_N(data2)])
             resample_func = resample_block_nb if use_numba else resample_block
-            resample_kwargs = dict(stack_data=stack_data, aggregator=aggregator)
+            resample_kwargs = dict(aggregator=aggregator)
         else:
             if data.ndim == 1:
                 data = data[:, None]
             if data2.ndim == 1:
                 data2 = data2[:, None]
             sample_stat = statistic(data, data2)
             N = min([len(data), len(data2)])
@@ -322,24 +322,23 @@
         else:
             output_len = 1
         if N < n_min:
             warnings.warn(f"N={N} < n_min={n_min}. Avoiding computation (returning NaNs) ...")
             theta_hat_b = None
         else:
             theta_hat_b = resample_func(data, data2, statistic, R=R, output_len=output_len, **resample_kwargs, **kwargs).squeeze()
-            if stack_data and is_block:
-                data = np.hstack(data)
-                data2 = np.hstack(data2)
+            # if stack_data and is_block:
+            #     data = np.hstack(data)
+            #     data2 = np.hstack(data2)
     return data, data2, theta_hat_b, sample_stat, N
 
 def CI_bca(data, statistic, data2=None, alternative='two-sided', alpha=0.05, R=int(1e5), account_equal=False, use_numba=True, n_min=5, **kwargs):
     """
     If data2 is provided, assumes a block resampling and statistic takes two arguments.
     Optional kwargs for aggregating data, data2 before computing the statistic:
-            stack_data = False,
             aggregator = @njit
                          def nb_mean(x):
                              return np.mean(x)
     """
     if alternative == 'two-sided':
         probs = np.array([alpha/2, 1 - alpha/2])
     elif alternative == 'less':
@@ -561,15 +560,14 @@
         raise ValueError(f"alternative '{alternative}' not valid. Available: 'two-sided', 'less', 'greater'.")
     return CI
 
 def CI_percentile(data, statistic, data2=None, R=int(1e5), alpha=0.05, smooth=False, alternative='two-sided', n_min=3, use_numba=True, **kwargs):
     """
     If data2 is provided, statistic takes two arguments and assumes block resampling if the input data are tuples.
     Optional kwargs for aggregating data, data2 before computing the statistic:
-            stack_data = False,
             aggregator = @njit
                          def nb_mean(x):
                              return np.mean(x)
     """
     data, data2, boot_sample, sample_stat, N = _resample(data, data2, use_numba, statistic, R=R, n_min=n_min, smooth=smooth, **kwargs)
     if boot_sample is None:
         return np.array([np.NaN, np.NaN])
```

### Comparing `phdu-1.9b1/phdu/stats/conf_interval.py` & `phdu-1.9b2/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/stats/corr.py` & `phdu-1.9b2/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/stats/rtopy/_helper.py` & `phdu-1.9b2/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/stats/rtopy/resample.py` & `phdu-1.9b2/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/stats/test/permutation.py` & `phdu-1.9b2/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu/storage.py` & `phdu-1.9b2/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/phdu.egg-info/PKG-INFO` & `phdu-1.9b2/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b1
+Version: 1.9b2
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b1/phdu.egg-info/SOURCES.txt` & `phdu-1.9b2/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.9b1/setup.py` & `phdu-1.9b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.9.b1',
+    version='1.9.b2',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```


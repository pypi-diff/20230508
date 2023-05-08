# Comparing `tmp/phdu-1.9b2.tar.gz` & `tmp/phdu-1.9b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.9b2.tar", last modified: Mon May  8 08:19:46 2023, max compression
+gzip compressed data, was "phdu-1.9b3.tar", last modified: Mon May  8 09:35:08 2023, max compression
```

## Comparing `phdu-1.9b2.tar` & `phdu-1.9b3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.238990 phdu-1.9b2/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.9b2/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:19:46.238990 phdu-1.9b2/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.9b2/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.9b2/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.9b2/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    30742 2023-05-08 08:18:56.000000 phdu-1.9b2/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.238990 phdu-1.9b2/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.238990 phdu-1.9b2/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.9b2/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.9b2/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.9b2/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:19:46.235657 phdu-1.9b2/phdu.egg-info/
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/requires.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-05-08 08:19:46.000000 phdu-1.9b2/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-05-08 08:19:46.238990 phdu-1.9b2/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-05-08 08:19:41.000000 phdu-1.9b2/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.9b3/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 09:35:08.701977 phdu-1.9b3/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.9b3/README.md
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.698644 phdu-1.9b3/phdu/
+-rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/clustering.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/decomposition.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/np_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/pd_utils.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.698644 phdu-1.9b3/phdu/plots/
+-rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/plots/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/plots/_mpl.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/plots/base.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.9b3/phdu/plots/plotly_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/script_fmt.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/phdu/stats/
+-rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/_integration.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.9b3/phdu/stats/_plots.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/_preprocess.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    31044 2023-05-08 09:34:15.000000 phdu-1.9b3/phdu/stats/bootstrap.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/conf_interval.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/corr.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/phdu/stats/rtopy/
+-rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/phdu/stats/test/
+-rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/test/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/test/_adherence.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/test/permutation.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.9b3/phdu/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.698644 phdu-1.9b3/phdu.egg-info/
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/requires.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/top_level.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-05-08 09:35:08.701977 phdu-1.9b3/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-05-08 09:34:41.000000 phdu-1.9b3/setup.py
```

### Comparing `phdu-1.9b2/LICENSE.md` & `phdu-1.9b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/PKG-INFO` & `phdu-1.9b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b2
+Version: 1.9b3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b2/README.md` & `phdu-1.9b3/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/_helper.py` & `phdu-1.9b3/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/clustering.py` & `phdu-1.9b3/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/decomposition.py` & `phdu-1.9b3/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/np_utils.py` & `phdu-1.9b3/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/pd_utils.py` & `phdu-1.9b3/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/plots/base.py` & `phdu-1.9b3/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/plots/plotly_utils.py` & `phdu-1.9b3/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/script_fmt.py` & `phdu-1.9b3/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/stats/_integration.py` & `phdu-1.9b3/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/stats/_plots.py` & `phdu-1.9b3/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/stats/bootstrap.py` & `phdu-1.9b3/phdu/stats/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,15 @@
         power = 1 - fail_low - fail_high
         results['violations-low'].append(fail_low)
         results['violations-high'].append(fail_high)
         results['power'].append(power)
     return pd.DataFrame(results, index=N_values)
 
 def power_analysis(data, statistic, low, high, output_len=1, N_values=np.array([5, 10, 25, 50, 100, 200]), recenter=False, seed=0, seed_N=int(1e9),
-                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3), R_N=int(1e5), alpha_low=0.025, alpha_high=0.025):
+                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3), R_N=int(1e4), alpha_low=0.05, alpha_high=0.05):
     """
     Stable bootstrap power and sample-size calculation for accepting H0 with confidence (1 - alpha_low - alpha_high).
     Computes violations on the studentized equivalent for the low and high bound of H0.
     Takes into account the variability in the original sample (size n):   bootstrap estimate, SE of the bootstrap estimate.
                                      and in the future sample (size N):   bootstrap estimate.
     See Efron-Tshibirani: An introduction to the bootstrap,  p. 381-384.
 
@@ -663,19 +663,24 @@
         nested_estimate_n = resample_nb(d_n, statistic, seed=seed+3+i, R=R_se_nested, output_len=output_len)
         estimate_n[i] = estimate_n_i
         se_estimate_n[i] = np.sqrt(np.diag(cov(nested_estimate_n, estimate_n_i, recenter=recenter)))
 
     # Violations of studentized endpoints.
     results = defaultdict(list)
     for N in N_values:
-        estimate_N = resample_nb(data, statistic, N=N, R=R_N, seed=seed_N, output_len=output_len)
-        estimate_N_low, estimate_N_high = np.percentile(estimate_N, [100*alpha_low, 100*(1-alpha_high)], axis=0)
+        estimate_N_low = np.empty((R, output_len))
+        estimate_N_high = np.empty((R, output_len))
+        for i in range(R):
+            estimate_N = resample_nb(data, statistic, N=N, R=R_N, seed=seed_N+i, output_len=output_len)
+            estimate_N_low[i] = np.percentile(estimate_N, 100*alpha_low, axis=0)
+            estimate_N_high[i] = np.percentile(estimate_N, 100*(1-alpha_high), axis=0)
         T_l = (estimate_n - estimate_N_low) / se_estimate_n
         T_h = (estimate_n - estimate_N_high) / se_estimate_n
         low_violations = (T_l > low_studentized).mean()
         high_violations = (T_h < high_studentized).mean()
-        power = 1 - low_violations - high_violations
+        # power = 1 - low_violations - high_violations. Wrong, there can be overlap
+        power = 1 - ( (T_l > low_studentized) | (T_h < high_studentized) ).mean()
         results['violations-low'].append(low_violations)
         results['violations-high'].append(high_violations)
         results['power'].append(power)
 
     return pd.DataFrame(results, index=N_values)
```

### Comparing `phdu-1.9b2/phdu/stats/conf_interval.py` & `phdu-1.9b3/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/stats/corr.py` & `phdu-1.9b3/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/stats/rtopy/_helper.py` & `phdu-1.9b3/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/stats/rtopy/resample.py` & `phdu-1.9b3/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/stats/test/permutation.py` & `phdu-1.9b3/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu/storage.py` & `phdu-1.9b3/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/phdu.egg-info/PKG-INFO` & `phdu-1.9b3/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b2
+Version: 1.9b3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b2/phdu.egg-info/SOURCES.txt` & `phdu-1.9b3/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.9b2/setup.py` & `phdu-1.9b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.9.b2',
+    version='1.9.b3',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```


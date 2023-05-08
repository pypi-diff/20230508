# Comparing `tmp/phdu-1.8b3.tar.gz` & `tmp/phdu-1.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.8b3.tar", last modified: Fri Apr 28 14:31:31 2023, max compression
+gzip compressed data, was "phdu-1.9b1.tar", last modified: Mon May  8 08:08:51 2023, max compression
```

## Comparing `phdu-1.8b3.tar` & `phdu-1.9b1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.8b3/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-04-28 14:31:31.040145 phdu-1.8b3/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.8b3/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.036811 phdu-1.8b3/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.036811 phdu-1.8b3/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.8b3/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.8b3/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    27792 2023-04-19 09:32:30.000000 phdu-1.8b3/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.8b3/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.036811 phdu-1.8b3/phdu.egg-info/
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/requires.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-04-28 14:31:31.040145 phdu-1.8b3/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-04-28 14:30:59.000000 phdu-1.8b3/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.9b1/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:08:51.302374 phdu-1.9b1/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.9b1/README.md
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.299040 phdu-1.9b1/phdu/
+-rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/clustering.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/decomposition.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/np_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/pd_utils.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/plots/
+-rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/plots/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/plots/_mpl.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/plots/base.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.9b1/phdu/plots/plotly_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/script_fmt.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/stats/
+-rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/_integration.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.9b1/phdu/stats/_plots.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/_preprocess.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    30838 2023-05-08 08:08:03.000000 phdu-1.9b1/phdu/stats/bootstrap.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/conf_interval.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/corr.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/stats/rtopy/
+-rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.302374 phdu-1.9b1/phdu/stats/test/
+-rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/test/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.9b1/phdu/stats/test/_adherence.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.9b1/phdu/stats/test/permutation.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.9b1/phdu/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 08:08:51.299040 phdu-1.9b1/phdu.egg-info/
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/requires.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-05-08 08:08:51.000000 phdu-1.9b1/phdu.egg-info/top_level.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-05-08 08:08:51.302374 phdu-1.9b1/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-05-08 08:08:40.000000 phdu-1.9b1/setup.py
```

### Comparing `phdu-1.8b3/LICENSE.md` & `phdu-1.9b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/PKG-INFO` & `phdu-1.9b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.8b3
+Version: 1.9b1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.8b3/README.md` & `phdu-1.9b1/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/_helper.py` & `phdu-1.9b1/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/clustering.py` & `phdu-1.9b1/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/decomposition.py` & `phdu-1.9b1/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/np_utils.py` & `phdu-1.9b1/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/pd_utils.py` & `phdu-1.9b1/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/plots/base.py` & `phdu-1.9b1/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/plots/plotly_utils.py` & `phdu-1.9b1/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/script_fmt.py` & `phdu-1.9b1/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/stats/_integration.py` & `phdu-1.9b1/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/stats/_plots.py` & `phdu-1.9b1/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/stats/bootstrap.py` & `phdu-1.9b1/phdu/stats/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         boot_sample[i] = func(x, y)
     return boot_sample
 
 @njit
 def resample_nb_X(X, R=int(1e5), seed=0, smooth=False, N=0):
     """X: array of shape (N_samples, n_vars)."""
     np.random.seed(seed)
-    n, output_len = X.shape
+    n, num_vars = X.shape
     if N == 0:
         N = n
     idxs_resampling = np.random.randint(low=0, high=n, size=R*N)
-    data_resampled = X[idxs_resampling].reshape(R, N, output_len)
+    data_resampled = X[idxs_resampling].reshape(R, N, num_vars)
     if smooth:
         def x_in_percentile(x):
             low, high  = np.percentile(x, [5, 95])
             z = x[(x>low) & (x<high)]
             return z
         def std_percentile(x):
             z = x_in_percentile(x)
@@ -106,44 +106,92 @@
 def _nb_mean(x):
     """
     njit version of numpy mean.
     """
     return np.mean(x)
 
 @njit
-def resample_block_nb(X, Y, func, output_len=1, R=int(1e5), seed=0, stack_data=True, aggregator=_nb_mean):
+def resample_block_nb(X, Y, func, output_len=1, R=int(1e4), R_B=int(1e3), seed=0, aggregator=_nb_mean):
     """
-    X, Y:         ragged arrays or tuples. Each element is an array containing the data for a block.
+    This function follows the following procedure:
+    1. Resamples paired blocks of data (X_k, Y_k) R times. k denotes the block label.
+    2. For each subset  X_k and Y_k, resample their contents R_B times.
+    3. Calculate the aggregated values of X_k and Y_k. Let's call them X_k^* and Y_k^*.
+    4. Compute the statistic of interest (func) using X_k^* and Y_k^*. Notice that now paired statistics can be used.
+
+    X, Y:         ragged arrays or tuples. Each element is an array containing the data for a block. Ensure there are no NaNs.
     func:         numba function f: X,Y  ->  Z,   Z: 1D array of size output_len.
     aggregator:   numba function for aggregating data from a block.
     """
     np.random.seed(seed)
-    def stack(arr_list):
-        return np.array([a for arr in arr_list for a in arr])
-
-    n_x = [len(x) for x in X]
-    n_y = [len(y) for y in Y]
-    idxs_resampling_x = [np.random.randint(low=0, high=n, size=R*n) for n in n_x]
-    idxs_resampling_y = [np.random.randint(low=0, high=n, size=R*n) for n in n_y]
-    X_resampled = [x[idxs_resampling].reshape(R, n) for x, n, idxs_resampling in zip(X, n_x, idxs_resampling_x)]
-    Y_resampled = [y[idxs_resampling].reshape(R, n) for y, n, idxs_resampling in zip(Y, n_y, idxs_resampling_y)]
+    R_T = R * R_B
+    boot_sample = np.empty((R_T, output_len))
 
-    boot_sample = np.empty((R, output_len))
-    if stack_data:
-        for i in range(R):
-            Xi = stack([x[i] for x in X_resampled])
-            Yi = stack([y[i] for y in Y_resampled])
-            boot_sample[i] = func(Xi, Yi)
-    else:
-        for i in range(R):
-            Xi = np.array([aggregator(x[i]) for x in X_resampled])
-            Yi = np.array([aggregator(y[i]) for y in Y_resampled])
-            boot_sample[i] = func(Xi, Yi)
+    num_blocks = len(X)
+    assert num_blocks == len(Y), "X and Y must have the same # blocks"
+    idxs_resampling_blocks = np.random.randint(low=0, high=num_blocks, size=R*num_blocks).reshape(R, num_blocks)
+
+    for i, idx_blocks in enumerate(idxs_resampling_blocks):
+        Xi = [X[k] for k in idx_blocks]
+        Yi = [Y[k] for k in idx_blocks]
+        n_Xi = [len(x) for x in Xi]
+        n_Yi = [len(y) for y in Yi]
+        idxs_resampling_Xi = [np.random.randint(low=0, high=n, size=R_B*n).reshape(R_B, n) for n in n_Xi]
+        idxs_resampling_Yi = [np.random.randint(low=0, high=n, size=R_B*n).reshape(R_B, n) for n in n_Yi]
+
+        idx_start = i * R_B
+        for j in range(R_B):
+            Xi_resampled = [x[idxs_resampling_Xi[k][j]] for k, x in enumerate(Xi)]
+            Yi_resampled = [y[idxs_resampling_Yi[k][j]] for k, y in enumerate(Yi)]
+            Xij = np.array([aggregator(x) for x in Xi_resampled])
+            Yij = np.array([aggregator(y) for y in Yi_resampled])
+            boot_sample[idx_start + j] = func(Xij, Yij)
     return boot_sample
 
+# Maybe numba adds compatibility for arrays with dtype=np.ndarray in the future.
+# @njit
+# def resample_block_nb(X, Y, func, output_len=1, R=int(1e4), R_B=int(1e3), seed=0, aggregator=_nb_mean):
+#
+#     This function follows the following procedure:
+#     1. Resamples paired blocks of data (X_k, Y_k) R times. k denotes the block label.
+#     2. For each subset  X_k and Y_k, resample their contents R_B times.
+#     3. Calculate the aggregated values of X_k and Y_k. Let's call them X_k^* and Y_k^*.
+#     4. Compute the statistic of interest (func) using X_k^* and Y_k^*. Notice that now paired statistics can be used.
+
+#     X, Y:         ragged arrays or tuples. Each element is an array containing the data for a block.
+#     func:         numba function f: X,Y  ->  Z,   Z: 1D array of size output_len.
+#     aggregator:   numba function for aggregating data from a block.
+#
+#     np.random.seed(seed)
+#     R_T = R * R_B
+#     boot_sample = np.empty((R_T, output_len))
+
+#     X = np.array(X, dtype=object)
+#     Y = np.array(Y, dtype=object)
+#     data = np.vstack((X, Y)).T
+#     num_blocks = data.shape[0]
+#     idxs_resampling_blocks = np.random.randint(low=0, high=num_blocks, size=R*num_blocks)
+#     data_resampled = data[idxs_resampling_blocks].reshape(R, num_blocks, 2)
+#     data_resampled = np.swapaxes(data_resampled, 1, 2)
+
+#     for i, (Xi, Yi) in enumerate(data_resampled):
+#         n_Xi = [len(x) for x in Xi]
+#         n_Yi = [len(y) for y in Yi]
+#         idxs_resampling_Xi = [np.random.randint(low=0, high=n, size=R_B*n) for n in n_Xi]
+#         idxs_resampling_Yi = [np.random.randint(low=0, high=n, size=R_B*n) for n in n_Yi]
+#         Xi_resampled = [x[idxs_resampling].reshape(R_B, n) for x, n, idxs_resampling in zip(Xi, n_Xi, idxs_resampling_Xi)]
+#         Yi_resampled = [y[idxs_resampling].reshape(R_B, n) for y, n, idxs_resampling in zip(Yi, n_Yi, idxs_resampling_Yi)]
+
+#         idx_start = i * R_B
+#         for j in range(R_B):
+#             Xij = np.array([aggregator(x[j]) for x in Xi_resampled])
+#             Yij = np.array([aggregator(y[j]) for y in Yi_resampled])
+#             boot_sample[idx_start + j] = func(Xij, Yij)
+#     return boot_sample
+
 def resample(X, func, output_len=1, R=int(1e4), seed=0):
     """X: array of shape (N_samples, n_vars)."""
     np.random.seed(seed)
     N = X.shape[0]
     idxs_resampling = np.random.randint(low=0, high=N, size=R*N)
     data_resampled = X[idxs_resampling].reshape(R, N, X.shape[1])
 
@@ -582,18 +630,18 @@
         fail_high = (data_resampled > high).mean()
         power = 1 - fail_low - fail_high
         results['violations-low'].append(fail_low)
         results['violations-high'].append(fail_high)
         results['power'].append(power)
     return pd.DataFrame(results, index=N_values)
 
-def power_analysis(data, statistic, low, high, output_len=1, N_values=np.array([5, 10, 25, 50, 100, 200]), recenter=False, seed=0,
-                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3)):
+def power_analysis(data, statistic, low, high, output_len=1, N_values=np.array([5, 10, 25, 50, 100, 200]), recenter=False, seed=0, seed_N=int(1e9),
+                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3), R_N=int(1e5), alpha_low=0.025, alpha_high=0.025):
     """
-    Stable bootstrap power and sample-size calculation for accepting H0.
+    Stable bootstrap power and sample-size calculation for accepting H0 with confidence (1 - alpha_low - alpha_high).
     Computes violations on the studentized equivalent for the low and high bound of H0.
     Takes into account the variability in the original sample (size n):   bootstrap estimate, SE of the bootstrap estimate.
                                      and in the future sample (size N):   bootstrap estimate.
     See Efron-Tshibirani: An introduction to the bootstrap,  p. 381-384.
 
     Returns: dataframe with index=N_values, columns=[low_fails, high_fails, power].
     """
@@ -617,17 +665,19 @@
         nested_estimate_n = resample_nb(d_n, statistic, seed=seed+3+i, R=R_se_nested, output_len=output_len)
         estimate_n[i] = estimate_n_i
         se_estimate_n[i] = np.sqrt(np.diag(cov(nested_estimate_n, estimate_n_i, recenter=recenter)))
 
     # Violations of studentized endpoints.
     results = defaultdict(list)
     for N in N_values:
-        estimate_N = resample_nb(data, statistic, N=N, R=R, seed=seed+2, output_len=output_len)
-        T = (estimate_n - estimate_N) / se_estimate_n
-        low_violations = (T >= low_studentized).mean()
-        high_violations = (T <= high_studentized).mean()
+        estimate_N = resample_nb(data, statistic, N=N, R=R_N, seed=seed_N, output_len=output_len)
+        estimate_N_low, estimate_N_high = np.percentile(estimate_N, [100*alpha_low, 100*(1-alpha_high)], axis=0)
+        T_l = (estimate_n - estimate_N_low) / se_estimate_n
+        T_h = (estimate_n - estimate_N_high) / se_estimate_n
+        low_violations = (T_l > low_studentized).mean()
+        high_violations = (T_h < high_studentized).mean()
         power = 1 - low_violations - high_violations
         results['violations-low'].append(low_violations)
         results['violations-high'].append(high_violations)
         results['power'].append(power)
 
     return pd.DataFrame(results, index=N_values)
```

### Comparing `phdu-1.8b3/phdu/stats/conf_interval.py` & `phdu-1.9b1/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/stats/corr.py` & `phdu-1.9b1/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/stats/rtopy/_helper.py` & `phdu-1.9b1/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/stats/rtopy/resample.py` & `phdu-1.9b1/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/stats/test/permutation.py` & `phdu-1.9b1/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu/storage.py` & `phdu-1.9b1/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/phdu.egg-info/PKG-INFO` & `phdu-1.9b1/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.8b3
+Version: 1.9b1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.8b3/phdu.egg-info/SOURCES.txt` & `phdu-1.9b1/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.8b3/setup.py` & `phdu-1.9b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.8.b3',
+    version='1.9.b1',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```


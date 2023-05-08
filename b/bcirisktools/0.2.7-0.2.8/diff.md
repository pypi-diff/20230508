# Comparing `tmp/bcirisktools-0.2.7.tar.gz` & `tmp/bcirisktools-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bcirisktools-0.2.7.tar", last modified: Fri Mar 17 16:08:24 2023, max compression
+gzip compressed data, was "bcirisktools-0.2.8.tar", last modified: Mon May  8 19:53:24 2023, max compression
```

## Comparing `bcirisktools-0.2.7.tar` & `bcirisktools-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-03-17 16:08:24.000000 bcirisktools-0.2.7/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      617 2023-03-17 16:08:24.000000 bcirisktools-0.2.7/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.2.7/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-03-17 16:08:23.000000 bcirisktools-0.2.7/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.2.7/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-03-02 03:11:23.000000 bcirisktools-0.2.7/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.2.7/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.2.7/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    10025 2023-03-17 16:07:55.000000 bcirisktools-0.2.7/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-03-02 03:02:45.000000 bcirisktools-0.2.7/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-03-03 16:20:47.000000 bcirisktools-0.2.7/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-03-17 16:08:23.000000 bcirisktools-0.2.7/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      617 2023-03-17 16:08:23.000000 bcirisktools-0.2.7/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      402 2023-03-17 16:08:23.000000 bcirisktools-0.2.7/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-03-17 16:08:23.000000 bcirisktools-0.2.7/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-03-17 16:08:23.000000 bcirisktools-0.2.7/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-03-17 16:08:23.000000 bcirisktools-0.2.7/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.2.7/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-03-17 16:08:24.000000 bcirisktools-0.2.7/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-03-17 16:08:00.000000 bcirisktools-0.2.7/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-08 19:53:24.799000 bcirisktools-0.2.8/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.2.8/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-05-08 19:53:24.791000 bcirisktools-0.2.8/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.2.8/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-08 19:53:24.660000 bcirisktools-0.2.8/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.2.8/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-03-02 03:11:23.000000 bcirisktools-0.2.8/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.2.8/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.2.8/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    10025 2023-03-23 00:01:50.000000 bcirisktools-0.2.8/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5719 2023-05-08 19:51:53.000000 bcirisktools-0.2.8/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-03-03 16:20:47.000000 bcirisktools-0.2.8/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-08 19:53:24.770000 bcirisktools-0.2.8/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-05-08 19:53:24.000000 bcirisktools-0.2.8/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-05-08 19:53:24.000000 bcirisktools-0.2.8/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-05-08 19:53:24.000000 bcirisktools-0.2.8/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-05-08 19:53:24.000000 bcirisktools-0.2.8/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-05-08 19:53:24.000000 bcirisktools-0.2.8/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.2.8/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-05-08 19:53:24.804000 bcirisktools-0.2.8/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-05-08 19:53:16.000000 bcirisktools-0.2.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bcirisktools-0.2.7/README.md` & `bcirisktools-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.7/bcirisktools/input_filters.py` & `bcirisktools-0.2.8/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.7/bcirisktools/metrics_bci.py` & `bcirisktools-0.2.8/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.7/bcirisktools/modeling.py` & `bcirisktools-0.2.8/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.7/bcirisktools/shapley_report.py` & `bcirisktools-0.2.8/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.7/bcirisktools/stability.py` & `bcirisktools-0.2.8/bcirisktools/stability.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             expected = df_feat.iloc[:, i] + 10e-20
             df_out.iloc[:, i + 1] = (actual - expected) * np.log(actual / expected)
 
         # Preparamos salida y append
         df_out = df_out.drop(columns=df_feat.columns[0])
         df_out = pd.DataFrame(df_out.sum()).rename(columns={0: a_variable}).T
         df_out["cuantil"] = quantiles
-        df_append = df_append.append(df_out)
+        df_append = pd.concat([df_append, df_out], axis=1)
 
     # Semaforo de estabilidad
     df_append["status"] = "🟢"
     df_append["status_2"] = "low"
 
     cond1 = (df_append.iloc[:, :-3] >= 0.1) & (df_append.iloc[:, :-3] < 0.2)
     cond1 = cond1.any(axis=1)
```

### Comparing `bcirisktools-0.2.7/bcirisktools/tree_crt.py` & `bcirisktools-0.2.8/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.7/setup.py` & `bcirisktools-0.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.2.7"
+VERSION = "0.2.8"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```


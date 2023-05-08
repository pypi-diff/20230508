# Comparing `tmp/abmap-0.1.0.tar.gz` & `tmp/abmap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/net/scratch3/scratch3-3/chihoim/ablm/dist/.tmp-cpdq81x1/abmap-0.1.0.tar", last modified: Tue May  2 23:54:04 2023, max compression
+gzip compressed data, was "/net/scratch3/scratch3-3/chihoim/ablm/dist/.tmp-l_3580qt/abmap-0.1.1.tar", last modified: Mon May  8 20:44:18 2023, max compression
```

## Comparing `abmap-0.1.0.tar` & `abmap-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 23:54:04.000000 abmap-0.1.0/
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1098 2023-02-28 02:48:26.000000 abmap-0.1.0/LICENSE.txt
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       15 2023-02-28 02:50:10.000000 abmap-0.1.0/MANIFEST.in
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-02 23:54:04.000000 abmap-0.1.0/PKG-INFO
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2174 2023-05-02 23:50:43.000000 abmap-0.1.0/README.md
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap/
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      398 2023-05-02 23:51:18.000000 abmap-0.1.0/abmap/__init__.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1747 2023-04-28 00:51:56.000000 abmap-0.1.0/abmap/__main__.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    10758 2023-04-28 00:51:56.000000 abmap-0.1.0/abmap/abmap_augment.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      437 2023-03-02 06:59:12.000000 abmap-0.1.0/abmap/base_config.py
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap/commands/
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       39 2023-03-02 05:58:52.000000 abmap-0.1.0/abmap/commands/__init__.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2395 2023-04-28 00:51:56.000000 abmap-0.1.0/abmap/commands/augment.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7470 2023-04-28 00:51:56.000000 abmap-0.1.0/abmap/commands/embed.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    20348 2023-05-02 01:26:42.000000 abmap-0.1.0/abmap/commands/train.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    12204 2023-03-05 19:41:16.000000 abmap-0.1.0/abmap/dataloader.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    12094 2023-03-02 06:10:26.000000 abmap-0.1.0/abmap/libraseq_preprocess.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    18789 2023-05-02 01:18:34.000000 abmap-0.1.0/abmap/model.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1531 2023-03-16 18:20:17.000000 abmap-0.1.0/abmap/mutate.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5626 2023-04-28 00:51:57.000000 abmap-0.1.0/abmap/plm_embed.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    14912 2023-04-28 00:51:57.000000 abmap-0.1.0/abmap/sabdab_preprocess.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5700 2023-04-21 14:55:50.000000 abmap-0.1.0/abmap/utils.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       18 2023-05-02 23:50:43.000000 abmap-0.1.0/abmap/version.py
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap.egg-info/
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap.egg-info/PKG-INFO
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      738 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap.egg-info/SOURCES.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        1 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap.egg-info/dependency_links.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       46 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap.egg-info/entry_points.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      125 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap.egg-info/requires.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       15 2023-05-02 23:54:04.000000 abmap-0.1.0/abmap.egg-info/top_level.txt
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 23:54:04.000000 abmap-0.1.0/analysis/
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        0 2023-02-24 06:16:30.000000 abmap-0.1.0/analysis/__init__.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    13874 2023-02-14 13:40:17.000000 abmap-0.1.0/analysis/briney_analysis.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     6033 2023-02-24 06:18:30.000000 abmap-0.1.0/analysis/covabdab_analyze.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    35361 2023-02-08 02:32:36.000000 abmap-0.1.0/analysis/desautels_analyze.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    37858 2023-02-08 02:32:36.000000 abmap-0.1.0/analysis/strucpred_analysis.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7143 2023-04-28 00:51:57.000000 abmap-0.1.0/analysis/thera_analysis.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      436 2023-05-02 23:53:42.000000 abmap-0.1.0/pyproject.toml
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       38 2023-05-02 23:54:04.000000 abmap-0.1.0/setup.cfg
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      986 2023-05-02 23:50:43.000000 abmap-0.1.0/setup.py
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 20:44:18.000000 abmap-0.1.1/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1098 2023-02-28 02:48:26.000000 abmap-0.1.1/LICENSE.txt
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       15 2023-02-28 02:50:10.000000 abmap-0.1.1/MANIFEST.in
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-08 20:44:18.000000 abmap-0.1.1/PKG-INFO
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2174 2023-05-02 23:50:43.000000 abmap-0.1.1/README.md
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      398 2023-05-02 23:51:18.000000 abmap-0.1.1/abmap/__init__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1747 2023-04-28 00:51:56.000000 abmap-0.1.1/abmap/__main__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    10758 2023-04-28 00:51:56.000000 abmap-0.1.1/abmap/abmap_augment.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      437 2023-03-02 06:59:12.000000 abmap-0.1.1/abmap/base_config.py
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap/commands/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       39 2023-03-02 05:58:52.000000 abmap-0.1.1/abmap/commands/__init__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2395 2023-04-28 00:51:56.000000 abmap-0.1.1/abmap/commands/augment.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7476 2023-05-08 20:43:23.000000 abmap-0.1.1/abmap/commands/embed.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    20348 2023-05-02 01:26:42.000000 abmap-0.1.1/abmap/commands/train.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    12204 2023-03-05 19:41:16.000000 abmap-0.1.1/abmap/dataloader.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    12094 2023-03-02 06:10:26.000000 abmap-0.1.1/abmap/libraseq_preprocess.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    18789 2023-05-02 01:18:34.000000 abmap-0.1.1/abmap/model.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1531 2023-03-16 18:20:17.000000 abmap-0.1.1/abmap/mutate.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5626 2023-04-28 00:51:57.000000 abmap-0.1.1/abmap/plm_embed.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    14912 2023-04-28 00:51:57.000000 abmap-0.1.1/abmap/sabdab_preprocess.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5700 2023-04-21 14:55:50.000000 abmap-0.1.1/abmap/utils.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       18 2023-05-02 23:50:43.000000 abmap-0.1.1/abmap/version.py
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap.egg-info/
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap.egg-info/PKG-INFO
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      738 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        1 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       46 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap.egg-info/entry_points.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      125 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap.egg-info/requires.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       15 2023-05-08 20:44:18.000000 abmap-0.1.1/abmap.egg-info/top_level.txt
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 20:44:18.000000 abmap-0.1.1/analysis/
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        0 2023-02-24 06:16:30.000000 abmap-0.1.1/analysis/__init__.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    13874 2023-02-14 13:40:17.000000 abmap-0.1.1/analysis/briney_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     6033 2023-02-24 06:18:30.000000 abmap-0.1.1/analysis/covabdab_analyze.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    35361 2023-02-08 02:32:36.000000 abmap-0.1.1/analysis/desautels_analyze.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    37858 2023-02-08 02:32:36.000000 abmap-0.1.1/analysis/strucpred_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7143 2023-04-28 00:51:57.000000 abmap-0.1.1/analysis/thera_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      436 2023-05-08 20:42:55.000000 abmap-0.1.1/pyproject.toml
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       38 2023-05-08 20:44:18.000000 abmap-0.1.1/setup.cfg
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      986 2023-05-02 23:50:43.000000 abmap-0.1.1/setup.py
```

### Comparing `abmap-0.1.0/LICENSE.txt` & `abmap-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/PKG-INFO` & `abmap-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abmap
-Version: 0.1.0
+Version: 0.1.1
 Summary: AbMAP: Antibody Mutagenesis Augmented Processing
 Author: Chiho Im, Taylor Sorenson, Abhinav Gupta, Rohit Singh
 Author-email: Chiho Im <chihoim@mit.edu>, Rohit Singh <rohitsingh@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `abmap-0.1.0/README.md` & `abmap-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/__main__.py` & `abmap-0.1.1/abmap/__main__.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/abmap_augment.py` & `abmap-0.1.1/abmap/abmap_augment.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/commands/augment.py` & `abmap-0.1.1/abmap/commands/augment.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/commands/embed.py` & `abmap-0.1.1/abmap/commands/embed.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     dev = torch.device(f'cuda:{device}' if torch.cuda.is_available() else "cpu")
 
     # Get list of files or casts single file as a list
     if os.path.isdir(input_path): input_iter = os.listdir(input_path)
     elif os.path.isfile(input_path): input_iter = list(input_path)
     
     outputs = []
-    for input in input_iter:
+    for input in tqdm(input_iter):
         with open(input, 'rb') as p:
             input_embed = pickle.load(p).to(dev)
         input_embed = torch.unsqueeze(input_embed, 0)
         try:
             assert len(input_embed.shape) == 3
         except:
             raise ValueError("input embedding should be of shape n'(CDR length) x d")
```

### Comparing `abmap-0.1.0/abmap/commands/train.py` & `abmap-0.1.1/abmap/commands/train.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/dataloader.py` & `abmap-0.1.1/abmap/dataloader.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/libraseq_preprocess.py` & `abmap-0.1.1/abmap/libraseq_preprocess.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/model.py` & `abmap-0.1.1/abmap/model.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/mutate.py` & `abmap-0.1.1/abmap/mutate.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/plm_embed.py` & `abmap-0.1.1/abmap/plm_embed.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/sabdab_preprocess.py` & `abmap-0.1.1/abmap/sabdab_preprocess.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap/utils.py` & `abmap-0.1.1/abmap/utils.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/abmap.egg-info/PKG-INFO` & `abmap-0.1.1/abmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abmap
-Version: 0.1.0
+Version: 0.1.1
 Summary: AbMAP: Antibody Mutagenesis Augmented Processing
 Author: Chiho Im, Taylor Sorenson, Abhinav Gupta, Rohit Singh
 Author-email: Chiho Im <chihoim@mit.edu>, Rohit Singh <rohitsingh@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `abmap-0.1.0/abmap.egg-info/SOURCES.txt` & `abmap-0.1.1/abmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/analysis/briney_analysis.py` & `abmap-0.1.1/analysis/briney_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/analysis/covabdab_analyze.py` & `abmap-0.1.1/analysis/covabdab_analyze.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/analysis/desautels_analyze.py` & `abmap-0.1.1/analysis/desautels_analyze.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/analysis/strucpred_analysis.py` & `abmap-0.1.1/analysis/strucpred_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/analysis/thera_analysis.py` & `abmap-0.1.1/analysis/thera_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.0/setup.py` & `abmap-0.1.1/setup.py`

 * *Files identical despite different names*


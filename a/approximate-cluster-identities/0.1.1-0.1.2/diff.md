# Comparing `tmp/approximate_cluster_identities-0.1.1.tar.gz` & `tmp/approximate_cluster_identities-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approximate_cluster_identities-0.1.1.tar", last modified: Mon May  8 11:10:03 2023, max compression
+gzip compressed data, was "approximate_cluster_identities-0.1.2.tar", last modified: Mon May  8 11:14:13 2023, max compression
```

## Comparing `approximate_cluster_identities-0.1.1.tar` & `approximate_cluster_identities-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/approximate_cluster_identities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:14:13.281011 approximate_cluster_identities-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 11:13:54.000000 approximate_cluster_identities-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-08 11:14:13.277011 approximate_cluster_identities-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-08 11:13:54.000000 approximate_cluster_identities-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:14:13.277011 approximate_cluster_identities-0.1.2/approximate_cluster_identities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:13:54.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-05-08 11:13:54.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:14:13.277011 approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-08 11:14:13.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 11:14:13.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:14:13.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 11:14:13.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:14:13.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 11:14:13.000000 approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:14:13.281011 approximate_cluster_identities-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-08 11:13:54.000000 approximate_cluster_identities-0.1.2/setup.py
```

### Comparing `approximate_cluster_identities-0.1.1/LICENSE` & `approximate_cluster_identities-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `approximate_cluster_identities-0.1.1/PKG-INFO` & `approximate_cluster_identities-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approximate_cluster_identities
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimisers.
 Author: Daniel Anderson
 Author-email: danp.anderson@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
@@ -56,25 +56,25 @@
 # Example output
 
 Example cluster plots for data in ```test/``` using ```--windowSize 1``` and ```--windowSize 100```.
 
 ### Window size = 1
 
 #### Mean identities
-![Mean identities](images/cluster_distances_window_1.mean.png)
+![Mean identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/cluster_distances_window_1.mean.png)
 #### Mode identities
-![Mode identities](images/cluster_distances_window_1.mode.png)
+![Mode identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_1.mode.png)
 #### Median identities
-![Median identities](images/cluster_distances_window_1.median.png)
+![Median identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_1.median.png)
 #### Range identities
-![Range of identities](images/cluster_distances_window_1.range.png)
+![Range of identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_1.range.png)
 
 ### Window size = 100
 
 #### Mean identities
-![Mean identities](images/cluster_distances_window_100.mean.png)
+![Mean identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.mean.png)
 #### Mode identities
-![Mode identities](images/cluster_distances_window_100.mode.png)
+![Mode identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.mode.png)
 #### Median identities
-![Median identities](images/cluster_distances_window_100.median.png)
+![Median identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.median.png)
 #### Range identities
-![Range of identities](images/cluster_distances_window_100.range.png)
+![Range of identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.range.png)
```

### Comparing `approximate_cluster_identities-0.1.1/README.md` & `approximate_cluster_identities-0.1.2/approximate_cluster_identities.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: approximate-cluster-identities
+Version: 0.1.2
+Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimisers.
+Author: Daniel Anderson
+Author-email: danp.anderson@outlook.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Approximate Cluster Identities (ACI)
 
 A python package to visualise the approximate within and between cluster identities of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
 
 # Installation
 ```
 pip install approximate-cluster-identities
@@ -42,25 +56,25 @@
 # Example output
 
 Example cluster plots for data in ```test/``` using ```--windowSize 1``` and ```--windowSize 100```.
 
 ### Window size = 1
 
 #### Mean identities
-![Mean identities](images/cluster_distances_window_1.mean.png)
+![Mean identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/cluster_distances_window_1.mean.png)
 #### Mode identities
-![Mode identities](images/cluster_distances_window_1.mode.png)
+![Mode identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_1.mode.png)
 #### Median identities
-![Median identities](images/cluster_distances_window_1.median.png)
+![Median identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_1.median.png)
 #### Range identities
-![Range of identities](images/cluster_distances_window_1.range.png)
+![Range of identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_1.range.png)
 
 ### Window size = 100
 
 #### Mean identities
-![Mean identities](images/cluster_distances_window_100.mean.png)
+![Mean identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.mean.png)
 #### Mode identities
-![Mode identities](images/cluster_distances_window_100.mode.png)
+![Mode identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.mode.png)
 #### Median identities
-![Median identities](images/cluster_distances_window_100.median.png)
+![Median identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.median.png)
 #### Range identities
-![Range of identities](images/cluster_distances_window_100.range.png)
+![Range of identities](https://github.com/Danderson123/approximate-cluster-identities/blob/main/images/images/cluster_distances_window_100.range.png)
```

### Comparing `approximate_cluster_identities-0.1.1/approximate_cluster_identities/__main__.py` & `approximate_cluster_identities-0.1.2/approximate_cluster_identities/__main__.py`

 * *Files identical despite different names*

### Comparing `approximate_cluster_identities-0.1.1/setup.py` & `approximate_cluster_identities-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='approximate_cluster_identities',
-    version='0.1.1',
+    version='0.1.2',
     description='A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimisers.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Daniel Anderson',
     author_email='danp.anderson@outlook.com',
     packages=find_packages(),
     install_requires=[
```


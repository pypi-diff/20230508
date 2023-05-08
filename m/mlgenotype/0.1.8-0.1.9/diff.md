# Comparing `tmp/mlgenotype-0.1.8.tar.gz` & `tmp/mlgenotype-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/cluster/ifs/projects/AlphaThal/github/mlgenotype/dist/.tmp-wxcei_lm/mlgenotype-0.1.8.tar", last modified: Sat May  6 02:12:16 2023, max compression
+gzip compressed data, was "/cluster/ifs/projects/AlphaThal/github/mlgenotype/dist/.tmp-akyd6_20/mlgenotype-0.1.9.tar", last modified: Sat May  6 02:22:27 2023, max compression
```

## Comparing `mlgenotype-0.1.8.tar` & `mlgenotype-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      995 2023-05-03 18:24:26.000000 mlgenotype-0.1.8/LICENSE.md
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       35 2023-05-05 19:32:32.000000 mlgenotype-0.1.8/MANIFEST.in
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/PKG-INFO
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      524 2023-05-03 22:37:53.000000 mlgenotype-0.1.8/README.md
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      864 2023-05-06 02:11:47.000000 mlgenotype-0.1.8/pyproject.toml
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      693 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/setup.cfg
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     8803 2023-05-04 01:38:57.000000 mlgenotype-0.1.8/setup.py
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       92 2023-05-05 21:28:24.000000 mlgenotype-0.1.8/src/mlgenotype/__init__.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       89 2023-05-03 22:40:34.000000 mlgenotype-0.1.8/src/mlgenotype/__main__.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     4888 2023-05-04 01:37:25.000000 mlgenotype-0.1.8/src/mlgenotype/figure1calcs.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     3207 2023-05-03 18:24:26.000000 mlgenotype-0.1.8/src/mlgenotype/rfgenotype.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     2752 2023-05-05 20:52:52.000000 mlgenotype-0.1.8/src/mlgenotype/rfmodelpredict.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     3625 2023-05-06 02:07:29.000000 mlgenotype-0.1.8/src/mlgenotype/rfmodeltrain.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     3792 2023-05-03 22:49:34.000000 mlgenotype-0.1.8/src/mlgenotype/rftrainpredict.py
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype.egg-info/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype.egg-info/PKG-INFO
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      527 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype.egg-info/SOURCES.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)        1 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype.egg-info/dependency_links.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      202 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype.egg-info/entry_points.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      106 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype.egg-info/requires.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       11 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/src/mlgenotype.egg-info/top_level.txt
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:12:16.000000 mlgenotype-0.1.8/tests/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      188 2023-05-05 21:37:26.000000 mlgenotype-0.1.8/tests/test_calls.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      995 2023-05-03 18:24:26.000000 mlgenotype-0.1.9/LICENSE.md
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       35 2023-05-05 19:32:32.000000 mlgenotype-0.1.9/MANIFEST.in
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/PKG-INFO
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      524 2023-05-03 22:37:53.000000 mlgenotype-0.1.9/README.md
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      864 2023-05-06 02:20:22.000000 mlgenotype-0.1.9/pyproject.toml
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      693 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/setup.cfg
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     8803 2023-05-04 01:38:57.000000 mlgenotype-0.1.9/setup.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       92 2023-05-05 21:28:24.000000 mlgenotype-0.1.9/src/mlgenotype/__init__.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       89 2023-05-03 22:40:34.000000 mlgenotype-0.1.9/src/mlgenotype/__main__.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     4888 2023-05-04 01:37:25.000000 mlgenotype-0.1.9/src/mlgenotype/figure1calcs.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     3207 2023-05-03 18:24:26.000000 mlgenotype-0.1.9/src/mlgenotype/rfgenotype.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     2752 2023-05-05 20:52:52.000000 mlgenotype-0.1.9/src/mlgenotype/rfmodelpredict.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     3621 2023-05-06 02:18:42.000000 mlgenotype-0.1.9/src/mlgenotype/rfmodeltrain.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     3792 2023-05-03 22:49:34.000000 mlgenotype-0.1.9/src/mlgenotype/rftrainpredict.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype.egg-info/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype.egg-info/PKG-INFO
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      527 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype.egg-info/SOURCES.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)        1 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype.egg-info/dependency_links.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      202 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype.egg-info/entry_points.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      106 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype.egg-info/requires.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       11 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/src/mlgenotype.egg-info/top_level.txt
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 02:22:27.000000 mlgenotype-0.1.9/tests/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      188 2023-05-05 21:37:26.000000 mlgenotype-0.1.9/tests/test_calls.py
```

### Comparing `mlgenotype-0.1.8/LICENSE.md` & `mlgenotype-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/PKG-INFO` & `mlgenotype-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgenotype
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package with utilities for training classifiers to recognize SVs in short read datasets
 Home-page: https://github.com/nhansen/mlgenotype
 Author: Nancy F Hansen, Gracelyn Hill, Jennifer Lin
 Author-email: "Nancy F. Hansen" <nhansen@mail.nih.gov>
 Project-URL: Homepage, https://github.com/nhansen/mlgenotype
 Project-URL: Bug Tracker, https://github.com/nhansen/mlgenotype/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlgenotype-0.1.8/README.md` & `mlgenotype-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/pyproject.toml` & `mlgenotype-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 48", "pytest"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlgenotype"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Nancy F. Hansen", email="nhansen@mail.nih.gov" },
 ]
 description = "A package with utilities for training classifiers to recognize SVs in short read datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `mlgenotype-0.1.8/setup.cfg` & `mlgenotype-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/setup.py` & `mlgenotype-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/src/mlgenotype/figure1calcs.py` & `mlgenotype-0.1.9/src/mlgenotype/figure1calcs.py`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/src/mlgenotype/rfgenotype.py` & `mlgenotype-0.1.9/src/mlgenotype/rfgenotype.py`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/src/mlgenotype/rfmodelpredict.py` & `mlgenotype-0.1.9/src/mlgenotype/rfmodelpredict.py`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/src/mlgenotype/rfmodeltrain.py` & `mlgenotype-0.1.9/src/mlgenotype/rfmodeltrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import argparse
-from mlgenotype.src import rfgenotype
+from mlgenotype import rfgenotype
 
 def init_argparse() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         usage="%(prog)s [OPTION] [FILE]...",
         description="Train a random forest model and write it and its accuracy stats out to the file system."
     )
     parser.add_argument(
```

### Comparing `mlgenotype-0.1.8/src/mlgenotype/rftrainpredict.py` & `mlgenotype-0.1.9/src/mlgenotype/rftrainpredict.py`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.8/src/mlgenotype.egg-info/PKG-INFO` & `mlgenotype-0.1.9/src/mlgenotype.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgenotype
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package with utilities for training classifiers to recognize SVs in short read datasets
 Home-page: https://github.com/nhansen/mlgenotype
 Author: Nancy F Hansen, Gracelyn Hill, Jennifer Lin
 Author-email: "Nancy F. Hansen" <nhansen@mail.nih.gov>
 Project-URL: Homepage, https://github.com/nhansen/mlgenotype
 Project-URL: Bug Tracker, https://github.com/nhansen/mlgenotype/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlgenotype-0.1.8/src/mlgenotype.egg-info/SOURCES.txt` & `mlgenotype-0.1.9/src/mlgenotype.egg-info/SOURCES.txt`

 * *Files identical despite different names*


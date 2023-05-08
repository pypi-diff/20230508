# Comparing `tmp/blitzgsea-1.3.8.tar.gz` & `tmp/blitzgsea-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blitzgsea-1.3.8.tar", last modified: Sun Apr 30 01:34:50 2023, max compression
+gzip compressed data, last modified: Sun Apr 30 02:13:35 2023, from Unix
```

## Comparing `blitzgsea-1.3.8.tar` & `blitzgsea-1.3.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:34:50.281338 blitzgsea-1.3.8/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-07-24 15:38:47.000000 blitzgsea-1.3.8/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)    12019 2023-04-30 01:34:50.280868 blitzgsea-1.3.8/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)    11461 2023-04-30 01:15:44.000000 blitzgsea-1.3.8/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:34:50.279758 blitzgsea-1.3.8/blitzgsea/
--rw-r--r--   0 maayanlab   (501) staff       (20)    15508 2023-04-29 01:49:21.000000 blitzgsea-1.3.8/blitzgsea/__init__.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2768 2023-04-28 02:23:48.000000 blitzgsea-1.3.8/blitzgsea/enrichr.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     7316 2022-07-24 15:38:47.000000 blitzgsea-1.3.8/blitzgsea/plot.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2594 2022-07-24 15:38:47.000000 blitzgsea-1.3.8/blitzgsea/shuffle.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:34:50.280599 blitzgsea-1.3.8/blitzgsea.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)    12019 2023-04-30 01:34:50.000000 blitzgsea-1.3.8/blitzgsea.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      272 2023-04-30 01:34:50.000000 blitzgsea-1.3.8/blitzgsea.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-04-30 01:34:50.000000 blitzgsea-1.3.8/blitzgsea.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      137 2023-04-30 01:34:50.000000 blitzgsea-1.3.8/blitzgsea.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       10 2023-04-30 01:34:50.000000 blitzgsea-1.3.8/blitzgsea.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-04-30 01:34:50.281509 blitzgsea-1.3.8/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1119 2023-04-30 01:34:07.000000 blitzgsea-1.3.8/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12019 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/PKG-INFO
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/blitzgsea/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-07-24 15:38:47.000000 ./blitzgsea-1.3.9/LICENSE
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/blitzgsea.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    32852 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/README.html
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11461 2023-04-30 01:15:44.000000 ./blitzgsea-1.3.9/README.md
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1104 2023-04-30 02:13:20.000000 ./blitzgsea-1.3.9/setup.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12019 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/blitzgsea.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      272 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/blitzgsea.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      137 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/blitzgsea.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       10 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/blitzgsea.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-04-30 02:13:35.000000 ./blitzgsea-1.3.9/blitzgsea.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)     7316 2022-07-24 15:38:47.000000 ./blitzgsea-1.3.9/blitzgsea/plot.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2768 2023-04-28 02:23:48.000000 ./blitzgsea-1.3.9/blitzgsea/enrichr.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)    15508 2023-04-29 01:49:21.000000 ./blitzgsea-1.3.9/blitzgsea/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2594 2022-07-24 15:38:47.000000 ./blitzgsea-1.3.9/blitzgsea/shuffle.py
```

### Comparing `blitzgsea-1.3.8/LICENSE` & `./blitzgsea-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.8/PKG-INFO` & `./blitzgsea-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blitzgsea
-Version: 1.3.8
+Version: 1.3.9
 Summary: Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.8 Summary: Package for fast
+Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.9 Summary: Package for fast
 calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE [blitzGSEA] [Installation](#installation) | [Example]
```

### Comparing `blitzgsea-1.3.8/README.md` & `./blitzgsea-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.8/blitzgsea/__init__.py` & `./blitzgsea-1.3.9/blitzgsea/__init__.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.8/blitzgsea/enrichr.py` & `./blitzgsea-1.3.9/blitzgsea/enrichr.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.8/blitzgsea/plot.py` & `./blitzgsea-1.3.9/blitzgsea/plot.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.8/blitzgsea/shuffle.py` & `./blitzgsea-1.3.9/blitzgsea/shuffle.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.8/blitzgsea.egg-info/PKG-INFO` & `./blitzgsea-1.3.9/blitzgsea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blitzgsea
-Version: 1.3.8
+Version: 1.3.9
 Summary: Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.8 Summary: Package for fast
+Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.9 Summary: Package for fast
 calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE [blitzGSEA] [Installation](#installation) | [Example]
```

### Comparing `blitzgsea-1.3.8/setup.py` & `./blitzgsea-1.3.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="blitzgsea",
-    version="1.3.8",
+    version="1.3.9",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/blitzgsea",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     package_data={
-        "blitzgsea": ["data/*", "README.html"]
+        "blitzgsea": ["data/*"]
     },
     include_package_data=True,
     install_requires=[
         'pandas>=1.1.5',
         'numpy',
         'scikit-learn',
         'progress',
```


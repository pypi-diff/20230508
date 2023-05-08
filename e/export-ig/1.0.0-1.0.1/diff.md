# Comparing `tmp/export_ig-1.0.0.tar.gz` & `tmp/export_ig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ig-1.0.0.tar", last modified: Mon May  8 05:22:14 2023, max compression
+gzip compressed data, was "export_ig-1.0.1.tar", last modified: Mon May  8 05:24:39 2023, max compression
```

## Comparing `export_ig-1.0.0.tar` & `export_ig-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:22:14.164178 export_ig-1.0.0/
--rw-r--r--   0 synch      (501) staff       (20)    11357 2023-05-08 05:17:43.000000 export_ig-1.0.0/LICENSE
--rw-r--r--   0 synch      (501) staff       (20)     1716 2023-05-08 05:22:14.164025 export_ig-1.0.0/PKG-INFO
--rw-r--r--   0 synch      (501) staff       (20)     1351 2023-05-08 05:17:46.000000 export_ig-1.0.0/README.md
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:22:14.162365 export_ig-1.0.0/export_ig/
--rw-r--r--   0 synch      (501) staff       (20)        0 2023-05-08 05:08:54.000000 export_ig-1.0.0/export_ig/__init__.py
--rw-r--r--   0 synch      (501) staff       (20)      555 2023-05-08 05:05:42.000000 export_ig-1.0.0/export_ig/color_utils.py
--rw-r--r--   0 synch      (501) staff       (20)     4416 2023-05-08 05:12:10.000000 export_ig-1.0.0/export_ig/export_ig.py
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:22:14.163808 export_ig-1.0.0/export_ig.egg-info/
--rw-r--r--   0 synch      (501) staff       (20)     1716 2023-05-08 05:22:14.000000 export_ig-1.0.0/export_ig.egg-info/PKG-INFO
--rw-r--r--   0 synch      (501) staff       (20)      328 2023-05-08 05:22:14.000000 export_ig-1.0.0/export_ig.egg-info/SOURCES.txt
--rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:22:14.000000 export_ig-1.0.0/export_ig.egg-info/dependency_links.txt
--rw-r--r--   0 synch      (501) staff       (20)       54 2023-05-08 05:22:14.000000 export_ig-1.0.0/export_ig.egg-info/entry_points.txt
--rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:13:33.000000 export_ig-1.0.0/export_ig.egg-info/not-zip-safe
--rw-r--r--   0 synch      (501) staff       (20)       19 2023-05-08 05:22:14.000000 export_ig-1.0.0/export_ig.egg-info/requires.txt
--rw-r--r--   0 synch      (501) staff       (20)       10 2023-05-08 05:22:14.000000 export_ig-1.0.0/export_ig.egg-info/top_level.txt
--rw-r--r--   0 synch      (501) staff       (20)       38 2023-05-08 05:22:14.164231 export_ig-1.0.0/setup.cfg
--rw-r--r--   0 synch      (501) staff       (20)      791 2023-05-08 05:21:32.000000 export_ig-1.0.0/setup.py
+drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:24:39.791681 export_ig-1.0.1/
+-rw-r--r--   0 synch      (501) staff       (20)    11357 2023-05-08 05:17:43.000000 export_ig-1.0.1/LICENSE
+-rw-r--r--   0 synch      (501) staff       (20)     1696 2023-05-08 05:24:39.791548 export_ig-1.0.1/PKG-INFO
+-rw-r--r--   0 synch      (501) staff       (20)     1331 2023-05-08 05:22:50.000000 export_ig-1.0.1/README.md
+drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:24:39.790614 export_ig-1.0.1/export_ig/
+-rw-r--r--   0 synch      (501) staff       (20)        0 2023-05-08 05:08:54.000000 export_ig-1.0.1/export_ig/__init__.py
+-rw-r--r--   0 synch      (501) staff       (20)      555 2023-05-08 05:05:42.000000 export_ig-1.0.1/export_ig/color_utils.py
+-rw-r--r--   0 synch      (501) staff       (20)     4416 2023-05-08 05:12:10.000000 export_ig-1.0.1/export_ig/export_ig.py
+drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:24:39.791394 export_ig-1.0.1/export_ig.egg-info/
+-rw-r--r--   0 synch      (501) staff       (20)     1696 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/PKG-INFO
+-rw-r--r--   0 synch      (501) staff       (20)      328 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/SOURCES.txt
+-rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/dependency_links.txt
+-rw-r--r--   0 synch      (501) staff       (20)       54 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/entry_points.txt
+-rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:13:33.000000 export_ig-1.0.1/export_ig.egg-info/not-zip-safe
+-rw-r--r--   0 synch      (501) staff       (20)       19 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/requires.txt
+-rw-r--r--   0 synch      (501) staff       (20)       10 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/top_level.txt
+-rw-r--r--   0 synch      (501) staff       (20)       38 2023-05-08 05:24:39.791720 export_ig-1.0.1/setup.cfg
+-rw-r--r--   0 synch      (501) staff       (20)      791 2023-05-08 05:23:27.000000 export_ig-1.0.1/setup.py
```

### Comparing `export_ig-1.0.0/LICENSE` & `export_ig-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.0/PKG-INFO` & `export_ig-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export_ig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for processing images for Instagram upload.
 Home-page: https://instagram.com/synch.poto
 Author: Sehyun Choi
 Author-email: choisehyun98@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -16,21 +16,21 @@
 Add padding around image, drop shadows.
 
 # How to Use
 
 Install packages.
 
 ```bash
-pip install -r requirements.txt
+pip install export_ig
 ```
 
 ## Run
 
 ```bash
-python export_ig.py --input_path "*.jpg" --output_folder padded/ --subfolder \
+export_ig --input_path "*.jpg" --output_folder padded/ --subfolder \
     --aspect_ratio 4x5 --shadow_offset 32 --radius 12 --shadow_color gray \
     --pad 100 --bg_color white \
     --n_jobs 10
 ```
 
 * `input_path`: glob string for input files. When using wildcard (*), make sure to
                 wrap it in quotes so that it does not get expanded by bash.
```

### Comparing `export_ig-1.0.0/README.md` & `export_ig-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 Add padding around image, drop shadows.
 
 # How to Use
 
 Install packages.
 
 ```bash
-pip install -r requirements.txt
+pip install export_ig
 ```
 
 ## Run
 
 ```bash
-python export_ig.py --input_path "*.jpg" --output_folder padded/ --subfolder \
+export_ig --input_path "*.jpg" --output_folder padded/ --subfolder \
     --aspect_ratio 4x5 --shadow_offset 32 --radius 12 --shadow_color gray \
     --pad 100 --bg_color white \
     --n_jobs 10
 ```
 
 * `input_path`: glob string for input files. When using wildcard (*), make sure to
                 wrap it in quotes so that it does not get expanded by bash.
```

### Comparing `export_ig-1.0.0/export_ig/color_utils.py` & `export_ig-1.0.1/export_ig/color_utils.py`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.0/export_ig/export_ig.py` & `export_ig-1.0.1/export_ig/export_ig.py`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.0/export_ig.egg-info/PKG-INFO` & `export_ig-1.0.1/export_ig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export-ig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for processing images for Instagram upload.
 Home-page: https://instagram.com/synch.poto
 Author: Sehyun Choi
 Author-email: choisehyun98@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -16,21 +16,21 @@
 Add padding around image, drop shadows.
 
 # How to Use
 
 Install packages.
 
 ```bash
-pip install -r requirements.txt
+pip install export_ig
 ```
 
 ## Run
 
 ```bash
-python export_ig.py --input_path "*.jpg" --output_folder padded/ --subfolder \
+export_ig --input_path "*.jpg" --output_folder padded/ --subfolder \
     --aspect_ratio 4x5 --shadow_offset 32 --radius 12 --shadow_color gray \
     --pad 100 --bg_color white \
     --n_jobs 10
 ```
 
 * `input_path`: glob string for input files. When using wildcard (*), make sure to
                 wrap it in quotes so that it does not get expanded by bash.
```

### Comparing `export_ig-1.0.0/setup.py` & `export_ig-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="export_ig",
-    version="1.0.0",
+    version="1.0.1",
     description="Package for processing images for Instagram upload.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     url="https://instagram.com/synch.poto",
```


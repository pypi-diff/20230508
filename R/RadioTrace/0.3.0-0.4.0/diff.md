# Comparing `tmp/radiotrace-0.3.0.tar.gz` & `tmp/RadioTrace-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiotrace-0.3.0.tar", last modified: Mon May  8 04:53:59 2023, max compression
+gzip compressed data, was "RadioTrace-0.4.0.tar", last modified: Mon May  8 05:01:16 2023, max compression
```

## Comparing `radiotrace-0.3.0.tar` & `RadioTrace-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 04:53:59.814398 radiotrace-0.3.0/
--rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 04:53:59.814248 radiotrace-0.3.0/PKG-INFO
--rw-r--r--   0 ljq        (501) staff       (20)     6678 2023-05-08 04:53:49.000000 radiotrace-0.3.0/README.md
-drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 04:53:59.813326 radiotrace-0.3.0/radiotrace/
--rw-r--r--   0 ljq        (501) staff       (20)      350 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/__init__.py
--rw-r--r--   0 ljq        (501) staff       (20)     1379 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/calPPS.py
--rw-r--r--   0 ljq        (501) staff       (20)     1428 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/get_projection.py
--rw-r--r--   0 ljq        (501) staff       (20)     2607 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/inference.py
--rw-r--r--   0 ljq        (501) staff       (20)      986 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/load.py
--rw-r--r--   0 ljq        (501) staff       (20)     1499 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/locate.py
--rw-r--r--   0 ljq        (501) staff       (20)     1601 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/utils.py
--rw-r--r--   0 ljq        (501) staff       (20)     3060 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/visualize.py
-drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 04:53:59.814034 radiotrace-0.3.0/radiotrace.egg-info/
--rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/PKG-INFO
--rw-r--r--   0 ljq        (501) staff       (20)      368 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/SOURCES.txt
--rw-r--r--   0 ljq        (501) staff       (20)        1 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/dependency_links.txt
--rw-r--r--   0 ljq        (501) staff       (20)      137 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/requires.txt
--rw-r--r--   0 ljq        (501) staff       (20)       11 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/top_level.txt
--rw-r--r--   0 ljq        (501) staff       (20)       38 2023-05-08 04:53:59.814446 radiotrace-0.3.0/setup.cfg
--rw-r--r--   0 ljq        (501) staff       (20)      837 2023-05-08 04:51:27.000000 radiotrace-0.3.0/setup.py
+drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 05:01:16.205673 RadioTrace-0.4.0/
+-rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 05:01:16.205524 RadioTrace-0.4.0/PKG-INFO
+-rw-r--r--   0 ljq        (501) staff       (20)     6678 2023-05-08 05:00:57.000000 RadioTrace-0.4.0/README.md
+drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 05:01:16.203572 RadioTrace-0.4.0/RadioTrace.egg-info/
+-rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 05:01:16.000000 RadioTrace-0.4.0/RadioTrace.egg-info/PKG-INFO
+-rw-r--r--   0 ljq        (501) staff       (20)      537 2023-05-08 05:01:16.000000 RadioTrace-0.4.0/RadioTrace.egg-info/SOURCES.txt
+-rw-r--r--   0 ljq        (501) staff       (20)        1 2023-05-08 05:01:16.000000 RadioTrace-0.4.0/RadioTrace.egg-info/dependency_links.txt
+-rw-r--r--   0 ljq        (501) staff       (20)      137 2023-05-08 05:01:16.000000 RadioTrace-0.4.0/RadioTrace.egg-info/requires.txt
+-rw-r--r--   0 ljq        (501) staff       (20)       11 2023-05-08 05:01:16.000000 RadioTrace-0.4.0/RadioTrace.egg-info/top_level.txt
+drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 05:01:16.205081 RadioTrace-0.4.0/radiotrace/
+-rw-r--r--   0 ljq        (501) staff       (20)      350 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/__init__.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1379 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/calPPS.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1428 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/get_projection.py
+-rw-r--r--   0 ljq        (501) staff       (20)     2607 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/inference.py
+-rw-r--r--   0 ljq        (501) staff       (20)      986 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/load.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1499 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/locate.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1601 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/utils.py
+-rw-r--r--   0 ljq        (501) staff       (20)     3060 2023-05-08 03:37:03.000000 RadioTrace-0.4.0/radiotrace/visualize.py
+-rw-r--r--   0 ljq        (501) staff       (20)       38 2023-05-08 05:01:16.205722 RadioTrace-0.4.0/setup.cfg
+-rw-r--r--   0 ljq        (501) staff       (20)      837 2023-05-08 05:01:04.000000 RadioTrace-0.4.0/setup.py
```

### Comparing `radiotrace-0.3.0/PKG-INFO` & `RadioTrace-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: radiotrace
-Version: 0.3.0
+Name: RadioTrace
+Version: 0.4.0
 Summary: package for quantify early-stage LUAD progression from CT image
 Home-page: https://github.com/LiJiaqi96/radiotrace
 Author: Jiaqi Li
 Author-email: li-jq18@mails.tsinghua.edu.cn
 License: MIT
 Description: # RadioTrace
         
@@ -97,24 +97,24 @@
         plt.title("Tumor")
         plt.subplot(122)
         plt.imshow(img2d, cmap="bone")
         plt.imshow(mask2d, alpha=0.5)
         plt.title("Stack mask")
         ```
         
-        ![p1](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p1.png?raw=true)
+        ![p1](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p1.png?raw=true)
         
         
         ### 3. Prepare data and load projection functions
         
         We use a deep learning model and a PCA transform function to project the tumor image to the PCA space of training set. Here we prepare the tumor image data for model input and then load the projection functions.  
         
         If you want to use GPU to do the inference, remember to specify the environment variable before loading the model.  
         
-        You will need some files such as pre-trained weights, transformation functions, etc. We have wrapped them into the package and please keep the paths unchanged. These files are also available on GitHub: https://github.com/LiJiaqi96/radiotrace.
+        You will need some files such as pre-trained weights, transformation functions, etc. We have wrapped them into the package and please keep the paths unchanged. These files are also available on GitHub: https://github.com/LiJiaqi96/RadioTrace.
         
         ```python
         size = [cal_tumor_size(tumor_mask)]
         tumor_image = [tumor_image]
         
         ## Optional: specify GPU device
         # os.environ['CUDA_VISIBLE_DEVICES'] = '1'
@@ -140,21 +140,21 @@
         
         We provide two visualization functions for users to visualize the reference trajectory and samples in the training set, as well as the relative position of the inference tumors.  
         
         ```python
         ## Visualize the reference only
         fig = visualize_reference(reference_data_path="./data/ref_data.json", curve_data_path="./data/curve_data.npy")
         ```
-        ![p2](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p2.png?raw=true)
+        ![p2](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p2.png?raw=true)
         
         ```python
         ## Visualize the reference and inference tumors. Use "transparency" argument to adjust the color of training samples.
         fig = visualize(reference_data_path="./data/ref_data.json", curve_data_path="./data/curve_data.npy", transparency=0.2)
         ```
-        ![p3](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p3.png?raw=true)
+        ![p3](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p3.png?raw=true)
         
         
         ### 6. Calculate pseudo-progression score (PPS)
         
         Finally, we quantify the progression status of the inference tumor(s). The PPS=0 indicates the earliest progression status. This step will return a list of PPS values.  
         
         ```python
```

### Comparing `radiotrace-0.3.0/README.md` & `RadioTrace-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,24 +89,24 @@
 plt.title("Tumor")
 plt.subplot(122)
 plt.imshow(img2d, cmap="bone")
 plt.imshow(mask2d, alpha=0.5)
 plt.title("Stack mask")
 ```
 
-![p1](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p1.png?raw=true)
+![p1](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p1.png?raw=true)
 
 
 ### 3. Prepare data and load projection functions
 
 We use a deep learning model and a PCA transform function to project the tumor image to the PCA space of training set. Here we prepare the tumor image data for model input and then load the projection functions.  
 
 If you want to use GPU to do the inference, remember to specify the environment variable before loading the model.  
 
-You will need some files such as pre-trained weights, transformation functions, etc. We have wrapped them into the package and please keep the paths unchanged. These files are also available on GitHub: https://github.com/LiJiaqi96/radiotrace.
+You will need some files such as pre-trained weights, transformation functions, etc. We have wrapped them into the package and please keep the paths unchanged. These files are also available on GitHub: https://github.com/LiJiaqi96/RadioTrace.
 
 ```python
 size = [cal_tumor_size(tumor_mask)]
 tumor_image = [tumor_image]
 
 ## Optional: specify GPU device
 # os.environ['CUDA_VISIBLE_DEVICES'] = '1'
@@ -132,21 +132,21 @@
 
 We provide two visualization functions for users to visualize the reference trajectory and samples in the training set, as well as the relative position of the inference tumors.  
 
 ```python
 ## Visualize the reference only
 fig = visualize_reference(reference_data_path="./data/ref_data.json", curve_data_path="./data/curve_data.npy")
 ```
-![p2](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p2.png?raw=true)
+![p2](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p2.png?raw=true)
 
 ```python
 ## Visualize the reference and inference tumors. Use "transparency" argument to adjust the color of training samples.
 fig = visualize(reference_data_path="./data/ref_data.json", curve_data_path="./data/curve_data.npy", transparency=0.2)
 ```
-![p3](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p3.png?raw=true)
+![p3](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p3.png?raw=true)
 
 
 ### 6. Calculate pseudo-progression score (PPS)
 
 Finally, we quantify the progression status of the inference tumor(s). The PPS=0 indicates the earliest progression status. This step will return a list of PPS values.  
 
 ```python
```

### Comparing `radiotrace-0.3.0/radiotrace/calPPS.py` & `RadioTrace-0.4.0/radiotrace/calPPS.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.3.0/radiotrace/get_projection.py` & `RadioTrace-0.4.0/radiotrace/get_projection.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.3.0/radiotrace/inference.py` & `RadioTrace-0.4.0/radiotrace/inference.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.3.0/radiotrace/load.py` & `RadioTrace-0.4.0/radiotrace/load.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.3.0/radiotrace/locate.py` & `RadioTrace-0.4.0/radiotrace/locate.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.3.0/radiotrace/utils.py` & `RadioTrace-0.4.0/radiotrace/utils.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.3.0/radiotrace/visualize.py` & `RadioTrace-0.4.0/radiotrace/visualize.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.3.0/radiotrace.egg-info/PKG-INFO` & `RadioTrace-0.4.0/RadioTrace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: radiotrace
-Version: 0.3.0
+Name: RadioTrace
+Version: 0.4.0
 Summary: package for quantify early-stage LUAD progression from CT image
 Home-page: https://github.com/LiJiaqi96/radiotrace
 Author: Jiaqi Li
 Author-email: li-jq18@mails.tsinghua.edu.cn
 License: MIT
 Description: # RadioTrace
         
@@ -97,24 +97,24 @@
         plt.title("Tumor")
         plt.subplot(122)
         plt.imshow(img2d, cmap="bone")
         plt.imshow(mask2d, alpha=0.5)
         plt.title("Stack mask")
         ```
         
-        ![p1](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p1.png?raw=true)
+        ![p1](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p1.png?raw=true)
         
         
         ### 3. Prepare data and load projection functions
         
         We use a deep learning model and a PCA transform function to project the tumor image to the PCA space of training set. Here we prepare the tumor image data for model input and then load the projection functions.  
         
         If you want to use GPU to do the inference, remember to specify the environment variable before loading the model.  
         
-        You will need some files such as pre-trained weights, transformation functions, etc. We have wrapped them into the package and please keep the paths unchanged. These files are also available on GitHub: https://github.com/LiJiaqi96/radiotrace.
+        You will need some files such as pre-trained weights, transformation functions, etc. We have wrapped them into the package and please keep the paths unchanged. These files are also available on GitHub: https://github.com/LiJiaqi96/RadioTrace.
         
         ```python
         size = [cal_tumor_size(tumor_mask)]
         tumor_image = [tumor_image]
         
         ## Optional: specify GPU device
         # os.environ['CUDA_VISIBLE_DEVICES'] = '1'
@@ -140,21 +140,21 @@
         
         We provide two visualization functions for users to visualize the reference trajectory and samples in the training set, as well as the relative position of the inference tumors.  
         
         ```python
         ## Visualize the reference only
         fig = visualize_reference(reference_data_path="./data/ref_data.json", curve_data_path="./data/curve_data.npy")
         ```
-        ![p2](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p2.png?raw=true)
+        ![p2](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p2.png?raw=true)
         
         ```python
         ## Visualize the reference and inference tumors. Use "transparency" argument to adjust the color of training samples.
         fig = visualize(reference_data_path="./data/ref_data.json", curve_data_path="./data/curve_data.npy", transparency=0.2)
         ```
-        ![p3](https://github.com/LiJiaqi96/radiotrace/blob/main/figures/p3.png?raw=true)
+        ![p3](https://github.com/LiJiaqi96/RadioTrace/blob/main/figures/p3.png?raw=true)
         
         
         ### 6. Calculate pseudo-progression score (PPS)
         
         Finally, we quantify the progression status of the inference tumor(s). The PPS=0 indicates the earliest progression status. This step will return a list of PPS values.  
         
         ```python
```

### Comparing `radiotrace-0.3.0/setup.py` & `RadioTrace-0.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    name="radiotrace",
-    version="0.3.0",
+    name="RadioTrace",
+    version="0.4.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "numpy>=1.17.0",
         "matplotlib>=3.1.3",
         "scikit-learn>=0.23.2",
         "scipy>=1.5.2",
```


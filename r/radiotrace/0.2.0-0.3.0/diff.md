# Comparing `tmp/radiotrace-0.2.0.tar.gz` & `tmp/radiotrace-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiotrace-0.2.0.tar", last modified: Mon May  8 03:43:38 2023, max compression
+gzip compressed data, was "radiotrace-0.3.0.tar", last modified: Mon May  8 04:53:59 2023, max compression
```

## Comparing `radiotrace-0.2.0.tar` & `radiotrace-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 03:43:38.832458 radiotrace-0.2.0/
--rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 03:43:38.832303 radiotrace-0.2.0/PKG-INFO
--rw-r--r--   0 ljq        (501) staff       (20)     6678 2023-05-08 03:37:03.000000 radiotrace-0.2.0/README.md
-drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 03:43:38.831396 radiotrace-0.2.0/radiotrace/
--rw-r--r--   0 ljq        (501) staff       (20)      350 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/__init__.py
--rw-r--r--   0 ljq        (501) staff       (20)     1379 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/calPPS.py
--rw-r--r--   0 ljq        (501) staff       (20)     1428 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/get_projection.py
--rw-r--r--   0 ljq        (501) staff       (20)     2607 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/inference.py
--rw-r--r--   0 ljq        (501) staff       (20)      986 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/load.py
--rw-r--r--   0 ljq        (501) staff       (20)     1499 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/locate.py
--rw-r--r--   0 ljq        (501) staff       (20)     1601 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/utils.py
--rw-r--r--   0 ljq        (501) staff       (20)     3060 2023-05-08 03:37:03.000000 radiotrace-0.2.0/radiotrace/visualize.py
-drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 03:43:38.832081 radiotrace-0.2.0/radiotrace.egg-info/
--rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 03:43:38.000000 radiotrace-0.2.0/radiotrace.egg-info/PKG-INFO
--rw-r--r--   0 ljq        (501) staff       (20)      368 2023-05-08 03:43:38.000000 radiotrace-0.2.0/radiotrace.egg-info/SOURCES.txt
--rw-r--r--   0 ljq        (501) staff       (20)        1 2023-05-08 03:43:38.000000 radiotrace-0.2.0/radiotrace.egg-info/dependency_links.txt
--rw-r--r--   0 ljq        (501) staff       (20)      137 2023-05-08 03:43:38.000000 radiotrace-0.2.0/radiotrace.egg-info/requires.txt
--rw-r--r--   0 ljq        (501) staff       (20)       11 2023-05-08 03:43:38.000000 radiotrace-0.2.0/radiotrace.egg-info/top_level.txt
--rw-r--r--   0 ljq        (501) staff       (20)       38 2023-05-08 03:43:38.832505 radiotrace-0.2.0/setup.cfg
--rw-r--r--   0 ljq        (501) staff       (20)      837 2023-05-08 03:43:34.000000 radiotrace-0.2.0/setup.py
+drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 04:53:59.814398 radiotrace-0.3.0/
+-rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 04:53:59.814248 radiotrace-0.3.0/PKG-INFO
+-rw-r--r--   0 ljq        (501) staff       (20)     6678 2023-05-08 04:53:49.000000 radiotrace-0.3.0/README.md
+drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 04:53:59.813326 radiotrace-0.3.0/radiotrace/
+-rw-r--r--   0 ljq        (501) staff       (20)      350 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/__init__.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1379 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/calPPS.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1428 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/get_projection.py
+-rw-r--r--   0 ljq        (501) staff       (20)     2607 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/inference.py
+-rw-r--r--   0 ljq        (501) staff       (20)      986 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/load.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1499 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/locate.py
+-rw-r--r--   0 ljq        (501) staff       (20)     1601 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/utils.py
+-rw-r--r--   0 ljq        (501) staff       (20)     3060 2023-05-08 03:37:03.000000 radiotrace-0.3.0/radiotrace/visualize.py
+drwxr-xr-x   0 ljq        (501) staff       (20)        0 2023-05-08 04:53:59.814034 radiotrace-0.3.0/radiotrace.egg-info/
+-rw-r--r--   0 ljq        (501) staff       (20)     8266 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/PKG-INFO
+-rw-r--r--   0 ljq        (501) staff       (20)      368 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/SOURCES.txt
+-rw-r--r--   0 ljq        (501) staff       (20)        1 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/dependency_links.txt
+-rw-r--r--   0 ljq        (501) staff       (20)      137 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/requires.txt
+-rw-r--r--   0 ljq        (501) staff       (20)       11 2023-05-08 04:53:59.000000 radiotrace-0.3.0/radiotrace.egg-info/top_level.txt
+-rw-r--r--   0 ljq        (501) staff       (20)       38 2023-05-08 04:53:59.814446 radiotrace-0.3.0/setup.cfg
+-rw-r--r--   0 ljq        (501) staff       (20)      837 2023-05-08 04:51:27.000000 radiotrace-0.3.0/setup.py
```

### Comparing `radiotrace-0.2.0/PKG-INFO` & `radiotrace-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: radiotrace
-Version: 0.2.0
+Version: 0.3.0
 Summary: package for quantify early-stage LUAD progression from CT image
 Home-page: https://github.com/LiJiaqi96/radiotrace
 Author: Jiaqi Li
 Author-email: li-jq18@mails.tsinghua.edu.cn
 License: MIT
-Description: # radiotrace
+Description: # RadioTrace
         
-        **radiotrace** is a Python package to quantify and visualize the progression status of early-stage lung adenocarcinoma (esLUAD) from CT images. It is designed and developed by Jiaqi Li from [XGlab](http://bioinfo.au.tsinghua.edu.cn/member/xuegonglab/), Tsinghua University. The work is collaborated with Prof. Wenzhao Zhong's group from Guangdong Provincial People's Hospital and Prof. Lin Yang's group from Shenzhen People's Hospital.
+        **RadioTrace** is a Python package to quantify and visualize the progression status of early-stage lung adenocarcinoma (esLUAD) from CT images. It is designed and developed by Jiaqi Li from [XGlab](http://bioinfo.au.tsinghua.edu.cn/member/xuegonglab/), Tsinghua University. The work is collaborated with Prof. Wenzhao Zhong's group from Guangdong Provincial People's Hospital and Prof. Lin Yang's group from Shenzhen People's Hospital.
         
-        **radiotrace** package is **free for academic use**. Please contact the authors for commercial usage.
+        **RadioTrace** package is **free for academic use**. Please contact the authors for commercial usage.
         
         ## Install
-        The **radiotrace** package integrates the use of Python and R. Don't worry, we have wrapped the R functions in the Python code and users only need to install some packages and then write Python code only.  
+        The **RadioTrace** package integrates the use of Python and R. Don't worry, we have wrapped the R functions in the Python code and users only need to install some packages and then write Python code only.  
         
         BTW, consider the potential conflicts of packages, we strongly suggest you to install the packages in a new [anaconda](https://www.anaconda.com/products/distribution) environment :)  
         
-        First let's install the python packages. Please pay special attention to PyTorch if you want to use GPU. It is easy to download the proper version of GPU version PyTorch from the official webpage (https://pytorch.org/get-started/locally/). In this case, make sure that you install the GPU version PyTorch before install **radiotrace**.  
+        First let's install the python packages. Please pay special attention to PyTorch if you want to use GPU. It is easy to download the proper version of GPU version PyTorch from the official webpage (https://pytorch.org/get-started/locally/). In this case, make sure that you install the GPU version PyTorch before install **RadioTrace**.  
         
-        After that, or if you only need CPU version PyTorch, install **radiotrace** packages.
+        After that, or if you only need CPU version PyTorch, install **RadioTrace** packages.
         ```
         pip install radiotrace
         ```
         
         Next, let's install the R packages. We also install the R using anaconda:  
         ```
         conda install -c conda-forge r-base
@@ -36,21 +36,21 @@
         
         The R package we need is the slingshot (Street et al., BMC Genomics, 2018), which can be installed from [Bioconductor](https://www.bioconductor.org/packages/release/bioc/html/slingshot.html). Here we use two lines of code to install these two packages:  
         ```R
         install.packages("BiocManager")  
         BiocManager::install("slingshot")
         ```
         
-        Now we have finished package installation. It's time to explore the use of **radiotrace**.  
+        Now we have finished package installation. It's time to explore the use of **RadioTrace**.  
         
         
         
         ## Tutorial
         
-        By running **radiotrace** package users are walking through several steps: Load image and segmentation, Locate and extract tumor, Load projection functions, Inference the emebedding vector(s) and coordinate(s) in PCA space, Visualization and Quantify progression status. Here we did clustering on the pixel-wise radiomic features.   
+        By running **RadioTrace** package users are walking through several steps: Load image and segmentation, Locate and extract tumor, Load projection functions, Inference the emebedding vector(s) and coordinate(s) in PCA space, Visualization and Quantify progression status. Here we did clustering on the pixel-wise radiomic features.   
         
         ### 0. Load packages
         
         ```python
         import os
         import numpy as np
         import matplotlib.pyplot as plt
```

### Comparing `radiotrace-0.2.0/README.md` & `radiotrace-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# radiotrace
+# RadioTrace
 
-**radiotrace** is a Python package to quantify and visualize the progression status of early-stage lung adenocarcinoma (esLUAD) from CT images. It is designed and developed by Jiaqi Li from [XGlab](http://bioinfo.au.tsinghua.edu.cn/member/xuegonglab/), Tsinghua University. The work is collaborated with Prof. Wenzhao Zhong's group from Guangdong Provincial People's Hospital and Prof. Lin Yang's group from Shenzhen People's Hospital.
+**RadioTrace** is a Python package to quantify and visualize the progression status of early-stage lung adenocarcinoma (esLUAD) from CT images. It is designed and developed by Jiaqi Li from [XGlab](http://bioinfo.au.tsinghua.edu.cn/member/xuegonglab/), Tsinghua University. The work is collaborated with Prof. Wenzhao Zhong's group from Guangdong Provincial People's Hospital and Prof. Lin Yang's group from Shenzhen People's Hospital.
 
-**radiotrace** package is **free for academic use**. Please contact the authors for commercial usage.
+**RadioTrace** package is **free for academic use**. Please contact the authors for commercial usage.
 
 ## Install
-The **radiotrace** package integrates the use of Python and R. Don't worry, we have wrapped the R functions in the Python code and users only need to install some packages and then write Python code only.  
+The **RadioTrace** package integrates the use of Python and R. Don't worry, we have wrapped the R functions in the Python code and users only need to install some packages and then write Python code only.  
 
 BTW, consider the potential conflicts of packages, we strongly suggest you to install the packages in a new [anaconda](https://www.anaconda.com/products/distribution) environment :)  
 
-First let's install the python packages. Please pay special attention to PyTorch if you want to use GPU. It is easy to download the proper version of GPU version PyTorch from the official webpage (https://pytorch.org/get-started/locally/). In this case, make sure that you install the GPU version PyTorch before install **radiotrace**.  
+First let's install the python packages. Please pay special attention to PyTorch if you want to use GPU. It is easy to download the proper version of GPU version PyTorch from the official webpage (https://pytorch.org/get-started/locally/). In this case, make sure that you install the GPU version PyTorch before install **RadioTrace**.  
 
-After that, or if you only need CPU version PyTorch, install **radiotrace** packages.
+After that, or if you only need CPU version PyTorch, install **RadioTrace** packages.
 ```
 pip install radiotrace
 ```
 
 Next, let's install the R packages. We also install the R using anaconda:  
 ```
 conda install -c conda-forge r-base
@@ -28,21 +28,21 @@
 
 The R package we need is the slingshot (Street et al., BMC Genomics, 2018), which can be installed from [Bioconductor](https://www.bioconductor.org/packages/release/bioc/html/slingshot.html). Here we use two lines of code to install these two packages:  
 ```R
 install.packages("BiocManager")  
 BiocManager::install("slingshot")
 ```
 
-Now we have finished package installation. It's time to explore the use of **radiotrace**.  
+Now we have finished package installation. It's time to explore the use of **RadioTrace**.  
 
 
 
 ## Tutorial
 
-By running **radiotrace** package users are walking through several steps: Load image and segmentation, Locate and extract tumor, Load projection functions, Inference the emebedding vector(s) and coordinate(s) in PCA space, Visualization and Quantify progression status. Here we did clustering on the pixel-wise radiomic features.   
+By running **RadioTrace** package users are walking through several steps: Load image and segmentation, Locate and extract tumor, Load projection functions, Inference the emebedding vector(s) and coordinate(s) in PCA space, Visualization and Quantify progression status. Here we did clustering on the pixel-wise radiomic features.   
 
 ### 0. Load packages
 
 ```python
 import os
 import numpy as np
 import matplotlib.pyplot as plt
```

### Comparing `radiotrace-0.2.0/radiotrace/calPPS.py` & `radiotrace-0.3.0/radiotrace/calPPS.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.2.0/radiotrace/get_projection.py` & `radiotrace-0.3.0/radiotrace/get_projection.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.2.0/radiotrace/inference.py` & `radiotrace-0.3.0/radiotrace/inference.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.2.0/radiotrace/load.py` & `radiotrace-0.3.0/radiotrace/load.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.2.0/radiotrace/locate.py` & `radiotrace-0.3.0/radiotrace/locate.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.2.0/radiotrace/utils.py` & `radiotrace-0.3.0/radiotrace/utils.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.2.0/radiotrace/visualize.py` & `radiotrace-0.3.0/radiotrace/visualize.py`

 * *Files identical despite different names*

### Comparing `radiotrace-0.2.0/radiotrace.egg-info/PKG-INFO` & `radiotrace-0.3.0/radiotrace.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: radiotrace
-Version: 0.2.0
+Version: 0.3.0
 Summary: package for quantify early-stage LUAD progression from CT image
 Home-page: https://github.com/LiJiaqi96/radiotrace
 Author: Jiaqi Li
 Author-email: li-jq18@mails.tsinghua.edu.cn
 License: MIT
-Description: # radiotrace
+Description: # RadioTrace
         
-        **radiotrace** is a Python package to quantify and visualize the progression status of early-stage lung adenocarcinoma (esLUAD) from CT images. It is designed and developed by Jiaqi Li from [XGlab](http://bioinfo.au.tsinghua.edu.cn/member/xuegonglab/), Tsinghua University. The work is collaborated with Prof. Wenzhao Zhong's group from Guangdong Provincial People's Hospital and Prof. Lin Yang's group from Shenzhen People's Hospital.
+        **RadioTrace** is a Python package to quantify and visualize the progression status of early-stage lung adenocarcinoma (esLUAD) from CT images. It is designed and developed by Jiaqi Li from [XGlab](http://bioinfo.au.tsinghua.edu.cn/member/xuegonglab/), Tsinghua University. The work is collaborated with Prof. Wenzhao Zhong's group from Guangdong Provincial People's Hospital and Prof. Lin Yang's group from Shenzhen People's Hospital.
         
-        **radiotrace** package is **free for academic use**. Please contact the authors for commercial usage.
+        **RadioTrace** package is **free for academic use**. Please contact the authors for commercial usage.
         
         ## Install
-        The **radiotrace** package integrates the use of Python and R. Don't worry, we have wrapped the R functions in the Python code and users only need to install some packages and then write Python code only.  
+        The **RadioTrace** package integrates the use of Python and R. Don't worry, we have wrapped the R functions in the Python code and users only need to install some packages and then write Python code only.  
         
         BTW, consider the potential conflicts of packages, we strongly suggest you to install the packages in a new [anaconda](https://www.anaconda.com/products/distribution) environment :)  
         
-        First let's install the python packages. Please pay special attention to PyTorch if you want to use GPU. It is easy to download the proper version of GPU version PyTorch from the official webpage (https://pytorch.org/get-started/locally/). In this case, make sure that you install the GPU version PyTorch before install **radiotrace**.  
+        First let's install the python packages. Please pay special attention to PyTorch if you want to use GPU. It is easy to download the proper version of GPU version PyTorch from the official webpage (https://pytorch.org/get-started/locally/). In this case, make sure that you install the GPU version PyTorch before install **RadioTrace**.  
         
-        After that, or if you only need CPU version PyTorch, install **radiotrace** packages.
+        After that, or if you only need CPU version PyTorch, install **RadioTrace** packages.
         ```
         pip install radiotrace
         ```
         
         Next, let's install the R packages. We also install the R using anaconda:  
         ```
         conda install -c conda-forge r-base
@@ -36,21 +36,21 @@
         
         The R package we need is the slingshot (Street et al., BMC Genomics, 2018), which can be installed from [Bioconductor](https://www.bioconductor.org/packages/release/bioc/html/slingshot.html). Here we use two lines of code to install these two packages:  
         ```R
         install.packages("BiocManager")  
         BiocManager::install("slingshot")
         ```
         
-        Now we have finished package installation. It's time to explore the use of **radiotrace**.  
+        Now we have finished package installation. It's time to explore the use of **RadioTrace**.  
         
         
         
         ## Tutorial
         
-        By running **radiotrace** package users are walking through several steps: Load image and segmentation, Locate and extract tumor, Load projection functions, Inference the emebedding vector(s) and coordinate(s) in PCA space, Visualization and Quantify progression status. Here we did clustering on the pixel-wise radiomic features.   
+        By running **RadioTrace** package users are walking through several steps: Load image and segmentation, Locate and extract tumor, Load projection functions, Inference the emebedding vector(s) and coordinate(s) in PCA space, Visualization and Quantify progression status. Here we did clustering on the pixel-wise radiomic features.   
         
         ### 0. Load packages
         
         ```python
         import os
         import numpy as np
         import matplotlib.pyplot as plt
```

### Comparing `radiotrace-0.2.0/setup.py` & `radiotrace-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="radiotrace",
-    version="0.2.0",
+    version="0.3.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "numpy>=1.17.0",
         "matplotlib>=3.1.3",
         "scikit-learn>=0.23.2",
         "scipy>=1.5.2",
```


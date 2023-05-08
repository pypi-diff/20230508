# Comparing `tmp/Perceptrone-viral3899-0.0.1.tar.gz` & `tmp/Perceptrone-viral3899-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Perceptron_Pypi/Perceptron_Pypi/dist/.tmp-en28k1ul/Perceptrone-viral3899-0.0.1.tar", last modified: Mon May  8 11:40:33 2023, max compression
+gzip compressed data, was "/home/runner/work/Perceptron_Pypi/Perceptron_Pypi/dist/.tmp-ksnb44q1/Perceptrone-viral3899-0.0.2.tar", last modified: Mon May  8 12:04:34 2023, max compression
```

## Comparing `Perceptrone-viral3899-0.0.1.tar` & `Perceptrone-viral3899-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 11:40:18.000000 Perceptrone-viral3899-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 11:40:18.000000 Perceptrone-viral3899-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 11:40:18.000000 Perceptrone-viral3899-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-08 11:40:18.000000 Perceptrone-viral3899-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/Perceptron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:40:18.000000 Perceptrone-viral3899-0.0.1/src/Perceptron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-08 11:40:18.000000 Perceptrone-viral3899-0.0.1/src/Perceptron/perceptron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/Perceptrone_viral3899.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/Perceptrone_viral3899.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/Perceptrone_viral3899.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/Perceptrone_viral3899.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/Perceptrone_viral3899.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 11:40:33.000000 Perceptrone-viral3899-0.0.1/src/Perceptrone_viral3899.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 12:04:22.000000 Perceptrone-viral3899-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 12:04:22.000000 Perceptrone-viral3899-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 12:04:22.000000 Perceptrone-viral3899-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-08 12:04:22.000000 Perceptrone-viral3899-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/Perceptron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:04:22.000000 Perceptrone-viral3899-0.0.2/src/Perceptron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-08 12:04:22.000000 Perceptrone-viral3899-0.0.2/src/Perceptron/perceptron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/Perceptrone_viral3899.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/Perceptrone_viral3899.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/Perceptrone_viral3899.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/Perceptrone_viral3899.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/Perceptrone_viral3899.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/Perceptrone_viral3899.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:04:34.000000 Perceptrone-viral3899-0.0.2/src/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-08 12:04:22.000000 Perceptrone-viral3899-0.0.2/src/logger/__init__.py
```

### Comparing `Perceptrone-viral3899-0.0.1/LICENSE` & `Perceptrone-viral3899-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Perceptrone-viral3899-0.0.1/PKG-INFO` & `Perceptrone-viral3899-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perceptrone-viral3899
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for perceptron
 Home-page: https://github.com/viral3899/Perceptron_PyPi
 Author: viral3899
 Author-email: viralsherarthiya1008@gmail.com
 Project-URL: Bug Tracker, https://github.com/viral3899/Perceptron_PyPi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Perceptrone-viral3899-0.0.1/setup.py` & `Perceptrone-viral3899-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 PKG_NAME = "Perceptrone"
 USER_NAME = "viral3899"
 PROJECT_NAME = "Perceptron_PyPi"
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 AUTHOR_NAME = 'Viral Sherathiya'
 AUTHOR_EMAIL = 'viralsherathiay1008@gmail.com'
 HYPHEN_E_DOT = '-e .'
 
 
 def get_requirements():
     """
     This Function returns the list of Requirements from requirements.txt & all the Packages.
     """
 
-    with open('./requirements.txt') as file_obj:
+    with open('requirements.txt') as file_obj:
         requirements = file_obj.readlines()
         requirements = [req.replace('\n', '') for req in requirements]
 
         if HYPHEN_E_DOT in requirements:
             requirements.remove(HYPHEN_E_DOT)
 
     return requirements
 
 
 setuptools.setup(
     name=f"{PKG_NAME}-{USER_NAME}",
-    version="0.0.1",
+    version="0.0.2",
     author=USER_NAME,
     author_email="viralsherarthiya1008@gmail.com",
     description="A package for perceptron",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/{USER_NAME}/{PROJECT_NAME}",
     project_urls={
@@ -43,11 +43,13 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
-    install_requires=['matplotlib==3.5.3', 'seaborn==0.12.2',
+    install_requires=
+    # get_requirements()
+    ['matplotlib==3.5.3', 'seaborn==0.12.2',
                       'pandas==1.3.5', 'numpy==1.21.6',
                       'joblib==1.2.0', 'ipykernel==6.16.2']
 )
```

### Comparing `Perceptrone-viral3899-0.0.1/src/Perceptron/perceptron.py` & `Perceptrone-viral3899-0.0.2/src/Perceptron/perceptron.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import joblib
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 from matplotlib.colors import ListedColormap
 plt.style.use("fivethirtyeight")
 
-from logger import logger
+from src.logger import logger
 
 
 class Perceptron:
     def __init__(self, eta: float = None, epochs: int = None):
         self.weights = np.random.rand(3) * 1e-4  # small Value
         training = (eta is not None) and (epochs is not None)
         if training:
```

### Comparing `Perceptrone-viral3899-0.0.1/src/Perceptrone_viral3899.egg-info/PKG-INFO` & `Perceptrone-viral3899-0.0.2/src/Perceptrone_viral3899.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perceptrone-viral3899
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for perceptron
 Home-page: https://github.com/viral3899/Perceptron_PyPi
 Author: viral3899
 Author-email: viralsherarthiya1008@gmail.com
 Project-URL: Bug Tracker, https://github.com/viral3899/Perceptron_PyPi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/monotonic derivative-0.4.tar.gz` & `tmp/monotonic derivative-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic derivative-0.4.tar", last modified: Mon May  8 08:49:10 2023, max compression
+gzip compressed data, was "monotonic derivative-0.5.tar", last modified: Mon May  8 08:55:28 2023, max compression
```

## Comparing `monotonic derivative-0.4.tar` & `monotonic derivative-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.322085 monotonic derivative-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 08:49:00.000000 monotonic derivative-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-08 08:49:10.322085 monotonic derivative-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-08 08:49:00.000000 monotonic derivative-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.318085 monotonic derivative-0.4/monotonic_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/curve_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/monotonic_derivative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.322085 monotonic derivative-0.4/monotonic_derivative.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:49:10.322085 monotonic derivative-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 08:49:00.000000 monotonic derivative-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.322085 monotonic derivative-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 08:49:00.000000 monotonic derivative-0.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 08:55:18.000000 monotonic derivative-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-08 08:55:28.809052 monotonic derivative-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-08 08:55:18.000000 monotonic derivative-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/monotonic_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/curve_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/monotonic_derivative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/monotonic_derivative.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:55:28.809052 monotonic derivative-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 08:55:18.000000 monotonic derivative-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 08:55:18.000000 monotonic derivative-0.5/tests/test.py
```

### Comparing `monotonic derivative-0.4/LICENSE` & `monotonic derivative-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.4/PKG-INFO` & `monotonic derivative-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic derivative
-Version: 0.4
+Version: 0.5
 Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -105,16 +105,16 @@
 
 #### Example
 
 ```python
 import numpy as np
 from monotonic_derivative.curve_smoothing import  curve_smoothing
 
-points = np.array([10, 55, 53, 40, 35, 5])
-best_individual = genetic_algorithm(points, alpha=0.5,save_plots = True)
+points = np.array([125, 55, 53, 40, 35, -25])
+best_individual = curve_smoothing(points, alpha=0.5,save_plots = True)
 #best_individual is the smoothed curve
 ```
 
 #### Result :
 
 This gif show how the genetic algorithm worked :
```

### Comparing `monotonic derivative-0.4/README.md` & `monotonic derivative-0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 
 #### Example
 
 ```python
 import numpy as np
 from monotonic_derivative.curve_smoothing import  curve_smoothing
 
-points = np.array([10, 55, 53, 40, 35, 5])
-best_individual = genetic_algorithm(points, alpha=0.5,save_plots = True)
+points = np.array([125, 55, 53, 40, 35, -25])
+best_individual = curve_smoothing(points, alpha=0.5,save_plots = True)
 #best_individual is the smoothed curve
 ```
 
 #### Result :
 
 This gif show how the genetic algorithm worked :
```

### Comparing `monotonic derivative-0.4/monotonic_derivative/curve_smoothing.py` & `monotonic derivative-0.5/monotonic_derivative/curve_smoothing.py`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.4/monotonic_derivative/monotonic_derivative.py` & `monotonic derivative-0.5/monotonic_derivative/monotonic_derivative.py`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.4/monotonic_derivative.egg-info/PKG-INFO` & `monotonic derivative-0.5/monotonic_derivative.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-derivative
-Version: 0.4
+Version: 0.5
 Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -105,16 +105,16 @@
 
 #### Example
 
 ```python
 import numpy as np
 from monotonic_derivative.curve_smoothing import  curve_smoothing
 
-points = np.array([10, 55, 53, 40, 35, 5])
-best_individual = genetic_algorithm(points, alpha=0.5,save_plots = True)
+points = np.array([125, 55, 53, 40, 35, -25])
+best_individual = curve_smoothing(points, alpha=0.5,save_plots = True)
 #best_individual is the smoothed curve
 ```
 
 #### Result :
 
 This gif show how the genetic algorithm worked :
```

### Comparing `monotonic derivative-0.4/setup.py` & `monotonic derivative-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="monotonic derivative",
-    version="0.4",
+    version="0.5",
     description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Adam Wecker",
     author_email="adam.wecker0@gmail.com",
     url="https://github.com/A-Wpro/monotonic_derivative",
     packages=["monotonic_derivative"],
```

### Comparing `monotonic derivative-0.4/tests/test.py` & `monotonic derivative-0.5/tests/test.py`

 * *Files identical despite different names*


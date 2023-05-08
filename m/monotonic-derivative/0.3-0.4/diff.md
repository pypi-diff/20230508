# Comparing `tmp/monotonic derivative-0.3.tar.gz` & `tmp/monotonic derivative-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic derivative-0.3.tar", last modified: Thu May  4 13:57:48 2023, max compression
+gzip compressed data, was "monotonic derivative-0.4.tar", last modified: Mon May  8 08:49:10 2023, max compression
```

## Comparing `monotonic derivative-0.3.tar` & `monotonic derivative-0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:48.725747 monotonic derivative-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 13:57:38.000000 monotonic derivative-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-04 13:57:48.725747 monotonic derivative-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 13:57:38.000000 monotonic derivative-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:48.725747 monotonic derivative-0.3/monotonic_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 13:57:38.000000 monotonic derivative-0.3/monotonic_derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 13:57:38.000000 monotonic derivative-0.3/monotonic_derivative/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-04 13:57:38.000000 monotonic derivative-0.3/monotonic_derivative/monotonic_derivative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:48.725747 monotonic derivative-0.3/monotonic_derivative.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-04 13:57:48.000000 monotonic derivative-0.3/monotonic_derivative.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 13:57:48.000000 monotonic derivative-0.3/monotonic_derivative.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:57:48.000000 monotonic derivative-0.3/monotonic_derivative.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 13:57:48.000000 monotonic derivative-0.3/monotonic_derivative.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 13:57:48.000000 monotonic derivative-0.3/monotonic_derivative.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:57:48.725747 monotonic derivative-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-04 13:57:38.000000 monotonic derivative-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:48.725747 monotonic derivative-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 13:57:38.000000 monotonic derivative-0.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.322085 monotonic derivative-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 08:49:00.000000 monotonic derivative-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-08 08:49:10.322085 monotonic derivative-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-08 08:49:00.000000 monotonic derivative-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.318085 monotonic derivative-0.4/monotonic_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/curve_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 08:49:00.000000 monotonic derivative-0.4/monotonic_derivative/monotonic_derivative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.322085 monotonic derivative-0.4/monotonic_derivative.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:49:10.000000 monotonic derivative-0.4/monotonic_derivative.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:49:10.322085 monotonic derivative-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 08:49:00.000000 monotonic derivative-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.322085 monotonic derivative-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 08:49:00.000000 monotonic derivative-0.4/tests/test.py
```

### Comparing `monotonic derivative-0.3/LICENSE` & `monotonic derivative-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.3/PKG-INFO` & `monotonic derivative-0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: monotonic derivative
-Version: 0.3
-Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
-Home-page: https://github.com/A-Wpro/monotonic_derivative
-Author: Adam Wecker
-Author-email: adam.wecker0@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Monotonic Derivative - A Python Library
 
 Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 
 ### Table of Contents
 
 - [Installation](#installation)
@@ -33,14 +17,16 @@
 
 ```
 pip install monotonic-derivative
 ```
 
 ### Usage
 
+#### Derivative tool:
+
 First, import the `ensure_monotonic_derivative` function from the `monotonic_derivative` module:
 
 ```python
 from monotonic_derivative import ensure_monotonic_derivative
 ```
 
 The primary function of the library, `ensure_monotonic_derivative`, takes the following arguments:
@@ -50,15 +36,15 @@
 - `degree`: int, the degree of the derivative to check for monotonicity (default: 2)
 - `force_negative_derivative`: bool, force the specified degree derivative to be monotonically decreasing if True (default: False)
 - `verbose`: bool, print additional information if True (default: False)
 - `save_plot`: bool, save the plots as PNG images if True (default: False)
 
 The function returns a modified numpy array of dependent variable data points (`modified_y`) that satisfy the specified monotonicity constraints.
 
-### Example
+#### Example
 
 ```python
 import numpy as np
 from monotonic_derivative import ensure_monotonic_derivative
 
 x = np.array([0, 1, 2, 3, 4, 5])
 y = np.array([100, 55, 53, 40, 35, 5])
@@ -78,14 +64,50 @@
 modified_y = [99.78638543 56.7089208  48.94131484 44.05868538 33.29107987  5.21361543]
 ```
 
 As you can see, slight change on y can totaly change how react the 2rd derivate.
 
 ![Derivative Example](./images/derivative.png)
 
+#### Genetic algorithm smoothing tool:
+
+```python
+### Test for curve smoothing with genetic algo
+from monotonic_derivative.curve_smoothing import  curve_smoothing
+```
+
+The primary function of the library, `curve_smoothing`, takes the following arguments:
+
+- `points`: numpy array, an array of Y-coordinates representing the original curve
+- `population_size`: int, the number of individuals in the population (default: 100)
+- `num_generations`: int, the number of generations to run the algorithm (default: 1000)
+- `mutation_rate`: float, the probability of a mutation occurring during reproduction (default: 0.1)
+- `alpha`: float, the trade-off between smoothness and similarity to the original curve (default: 0.5)
+- `save_plots`: bool, whether to save the progress of the algorithm as a GIF (default: False)
+- `output_folder`: str, the folder to save the progress GIF if `save_plots` is True (default: "output")
+
+The function returns the best individual (smoothed curve) found by the genetic algorithm as a numpy array.
+
+#### Example
+
+```python
+import numpy as np
+from monotonic_derivative.curve_smoothing import  curve_smoothing
+
+points = np.array([10, 55, 53, 40, 35, 5])
+best_individual = genetic_algorithm(points, alpha=0.5,save_plots = True)
+#best_individual is the smoothed curve
+```
+
+#### Result :
+
+This gif show how the genetic algorithm worked :
+
+![Derivative Example](./images/progress.gif)
+
 ### Real-life Applications
 
 In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
 
 The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
 
 ### Limit
```

### Comparing `monotonic derivative-0.3/README.md` & `monotonic derivative-0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: monotonic derivative
+Version: 0.4
+Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
+Home-page: https://github.com/A-Wpro/monotonic_derivative
+Author: Adam Wecker
+Author-email: adam.wecker0@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Monotonic Derivative - A Python Library
 
 Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 
 ### Table of Contents
 
 - [Installation](#installation)
@@ -17,14 +33,16 @@
 
 ```
 pip install monotonic-derivative
 ```
 
 ### Usage
 
+#### Derivative tool:
+
 First, import the `ensure_monotonic_derivative` function from the `monotonic_derivative` module:
 
 ```python
 from monotonic_derivative import ensure_monotonic_derivative
 ```
 
 The primary function of the library, `ensure_monotonic_derivative`, takes the following arguments:
@@ -34,15 +52,15 @@
 - `degree`: int, the degree of the derivative to check for monotonicity (default: 2)
 - `force_negative_derivative`: bool, force the specified degree derivative to be monotonically decreasing if True (default: False)
 - `verbose`: bool, print additional information if True (default: False)
 - `save_plot`: bool, save the plots as PNG images if True (default: False)
 
 The function returns a modified numpy array of dependent variable data points (`modified_y`) that satisfy the specified monotonicity constraints.
 
-### Example
+#### Example
 
 ```python
 import numpy as np
 from monotonic_derivative import ensure_monotonic_derivative
 
 x = np.array([0, 1, 2, 3, 4, 5])
 y = np.array([100, 55, 53, 40, 35, 5])
@@ -62,14 +80,50 @@
 modified_y = [99.78638543 56.7089208  48.94131484 44.05868538 33.29107987  5.21361543]
 ```
 
 As you can see, slight change on y can totaly change how react the 2rd derivate.
 
 ![Derivative Example](./images/derivative.png)
 
+#### Genetic algorithm smoothing tool:
+
+```python
+### Test for curve smoothing with genetic algo
+from monotonic_derivative.curve_smoothing import  curve_smoothing
+```
+
+The primary function of the library, `curve_smoothing`, takes the following arguments:
+
+- `points`: numpy array, an array of Y-coordinates representing the original curve
+- `population_size`: int, the number of individuals in the population (default: 100)
+- `num_generations`: int, the number of generations to run the algorithm (default: 1000)
+- `mutation_rate`: float, the probability of a mutation occurring during reproduction (default: 0.1)
+- `alpha`: float, the trade-off between smoothness and similarity to the original curve (default: 0.5)
+- `save_plots`: bool, whether to save the progress of the algorithm as a GIF (default: False)
+- `output_folder`: str, the folder to save the progress GIF if `save_plots` is True (default: "output")
+
+The function returns the best individual (smoothed curve) found by the genetic algorithm as a numpy array.
+
+#### Example
+
+```python
+import numpy as np
+from monotonic_derivative.curve_smoothing import  curve_smoothing
+
+points = np.array([10, 55, 53, 40, 35, 5])
+best_individual = genetic_algorithm(points, alpha=0.5,save_plots = True)
+#best_individual is the smoothed curve
+```
+
+#### Result :
+
+This gif show how the genetic algorithm worked :
+
+![Derivative Example](./images/progress.gif)
+
 ### Real-life Applications
 
 In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
 
 The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
 
 ### Limit
```

### Comparing `monotonic derivative-0.3/monotonic_derivative/monotonic_derivative.py` & `monotonic derivative-0.4/monotonic_derivative/monotonic_derivative.py`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.3/monotonic_derivative.egg-info/PKG-INFO` & `monotonic derivative-0.4/monotonic_derivative.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: monotonic-derivative
-Version: 0.3
-Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
+Version: 0.4
+Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,14 +33,16 @@
 
 ```
 pip install monotonic-derivative
 ```
 
 ### Usage
 
+#### Derivative tool:
+
 First, import the `ensure_monotonic_derivative` function from the `monotonic_derivative` module:
 
 ```python
 from monotonic_derivative import ensure_monotonic_derivative
 ```
 
 The primary function of the library, `ensure_monotonic_derivative`, takes the following arguments:
@@ -50,15 +52,15 @@
 - `degree`: int, the degree of the derivative to check for monotonicity (default: 2)
 - `force_negative_derivative`: bool, force the specified degree derivative to be monotonically decreasing if True (default: False)
 - `verbose`: bool, print additional information if True (default: False)
 - `save_plot`: bool, save the plots as PNG images if True (default: False)
 
 The function returns a modified numpy array of dependent variable data points (`modified_y`) that satisfy the specified monotonicity constraints.
 
-### Example
+#### Example
 
 ```python
 import numpy as np
 from monotonic_derivative import ensure_monotonic_derivative
 
 x = np.array([0, 1, 2, 3, 4, 5])
 y = np.array([100, 55, 53, 40, 35, 5])
@@ -78,14 +80,50 @@
 modified_y = [99.78638543 56.7089208  48.94131484 44.05868538 33.29107987  5.21361543]
 ```
 
 As you can see, slight change on y can totaly change how react the 2rd derivate.
 
 ![Derivative Example](./images/derivative.png)
 
+#### Genetic algorithm smoothing tool:
+
+```python
+### Test for curve smoothing with genetic algo
+from monotonic_derivative.curve_smoothing import  curve_smoothing
+```
+
+The primary function of the library, `curve_smoothing`, takes the following arguments:
+
+- `points`: numpy array, an array of Y-coordinates representing the original curve
+- `population_size`: int, the number of individuals in the population (default: 100)
+- `num_generations`: int, the number of generations to run the algorithm (default: 1000)
+- `mutation_rate`: float, the probability of a mutation occurring during reproduction (default: 0.1)
+- `alpha`: float, the trade-off between smoothness and similarity to the original curve (default: 0.5)
+- `save_plots`: bool, whether to save the progress of the algorithm as a GIF (default: False)
+- `output_folder`: str, the folder to save the progress GIF if `save_plots` is True (default: "output")
+
+The function returns the best individual (smoothed curve) found by the genetic algorithm as a numpy array.
+
+#### Example
+
+```python
+import numpy as np
+from monotonic_derivative.curve_smoothing import  curve_smoothing
+
+points = np.array([10, 55, 53, 40, 35, 5])
+best_individual = genetic_algorithm(points, alpha=0.5,save_plots = True)
+#best_individual is the smoothed curve
+```
+
+#### Result :
+
+This gif show how the genetic algorithm worked :
+
+![Derivative Example](./images/progress.gif)
+
 ### Real-life Applications
 
 In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
 
 The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
 
 ### Limit
```

### Comparing `monotonic derivative-0.3/setup.py` & `monotonic derivative-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="monotonic derivative",
-    version="0.3",
-    description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
+    version="0.4",
+    description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Adam Wecker",
     author_email="adam.wecker0@gmail.com",
     url="https://github.com/A-Wpro/monotonic_derivative",
     packages=["monotonic_derivative"],
     install_requires=["numpy", "scipy", "matplotlib", "imageio"],
```


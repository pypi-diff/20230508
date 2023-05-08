# Comparing `tmp/equal-odds-0.0.3.tar.gz` & `tmp/equal-odds-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equal-odds-0.0.3.tar", last modified: Mon Feb  6 15:36:56 2023, max compression
+gzip compressed data, was "equal-odds-0.0.4.tar", last modified: Mon May  8 09:28:23 2023, max compression
```

## Comparing `equal-odds-0.0.3.tar` & `equal-odds-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:36:56.131862 equal-odds-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-06 15:36:31.000000 equal-odds-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 15:36:31.000000 equal-odds-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-06 15:36:56.131862 equal-odds-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-06 15:36:31.000000 equal-odds-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:36:56.131862 equal-odds-0.0.3/equal_odds/
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-02-06 15:36:31.000000 equal-odds-0.0.3/equal_odds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-06 15:36:31.000000 equal-odds-0.0.3/equal_odds/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-02-06 15:36:31.000000 equal-odds-0.0.3/equal_odds/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-02-06 15:36:31.000000 equal-odds-0.0.3/equal_odds/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-02-06 15:36:31.000000 equal-odds-0.0.3/equal_odds/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-02-06 15:36:31.000000 equal-odds-0.0.3/equal_odds/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:36:56.131862 equal-odds-0.0.3/equal_odds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-06 15:36:56.000000 equal-odds-0.0.3/equal_odds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-06 15:36:56.000000 equal-odds-0.0.3/equal_odds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 15:36:56.000000 equal-odds-0.0.3/equal_odds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-06 15:36:56.000000 equal-odds-0.0.3/equal_odds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-06 15:36:56.000000 equal-odds-0.0.3/equal_odds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:36:56.131862 equal-odds-0.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-06 15:36:31.000000 equal-odds-0.0.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-06 15:36:31.000000 equal-odds-0.0.3/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-06 15:36:31.000000 equal-odds-0.0.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 15:36:56.131862 equal-odds-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-02-06 15:36:31.000000 equal-odds-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:28:23.203795 equal-odds-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 09:28:12.000000 equal-odds-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 09:28:12.000000 equal-odds-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-08 09:28:23.203795 equal-odds-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 09:28:12.000000 equal-odds-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:28:23.203795 equal-odds-0.0.4/equal_odds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-08 09:28:12.000000 equal-odds-0.0.4/equal_odds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 09:28:12.000000 equal-odds-0.0.4/equal_odds/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-05-08 09:28:12.000000 equal-odds-0.0.4/equal_odds/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-05-08 09:28:12.000000 equal-odds-0.0.4/equal_odds/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-08 09:28:12.000000 equal-odds-0.0.4/equal_odds/equal_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-08 09:28:12.000000 equal-odds-0.0.4/equal_odds/roc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:28:23.203795 equal-odds-0.0.4/equal_odds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-08 09:28:23.000000 equal-odds-0.0.4/equal_odds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-08 09:28:23.000000 equal-odds-0.0.4/equal_odds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:28:23.000000 equal-odds-0.0.4/equal_odds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 09:28:23.000000 equal-odds-0.0.4/equal_odds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 09:28:23.000000 equal-odds-0.0.4/equal_odds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:28:23.203795 equal-odds-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 09:28:12.000000 equal-odds-0.0.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 09:28:12.000000 equal-odds-0.0.4/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 09:28:12.000000 equal-odds-0.0.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:28:23.203795 equal-odds-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-08 09:28:12.000000 equal-odds-0.0.4/setup.py
```

### Comparing `equal-odds-0.0.3/LICENSE` & `equal-odds-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.3/PKG-INFO` & `equal-odds-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equal-odds
-Version: 0.0.3
+Version: 0.0.4
 Summary: _PACKAGE IN CONSTRUCTION_
 Home-page: https://github.com/AndreFCruz/equal-odds
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,21 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # equal-odds
 > This repository is under construction :construction:
 
-![badge for PyPI publishing status](https://github.com/AndreFCruz/equal-odds/actions/workflows/python-publish.yml/badge.svg)
+![PyPI publishing status](https://github.com/AndreFCruz/equal-odds/actions/workflows/python-publish.yml/badge.svg)
+![PyPI version](https://badgen.net/pypi/v/equal-odds)
+![OSI license](https://badgen.net/pypi/license/equal-odds)
+![Python compatibility](https://badgen.net/pypi/python/equal-odds)
+<!-- ![PyPI version](https://img.shields.io/pypi/v/equal-odds) -->
+<!-- ![OSI license](https://img.shields.io/pypi/l/equal-odds) -->
+<!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/equal-odds) -->
 
 A fast adjust
 
 ## Installing
 
 Install package from [PyPI](https://pypi.org/project/equal-odds/):
 ```
```

### Comparing `equal-odds-0.0.3/equal_odds/classifiers.py` & `equal-odds-0.0.4/equal_odds/classifiers.py`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.3/equal_odds/cvxpy_utils.py` & `equal-odds-0.0.4/equal_odds/cvxpy_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A set of helper functions for using cvxpy.
 """
 import logging
+import operator
 from itertools import product
 
 import numpy as np
 import cvxpy as cp
 from cvxpy.expressions.variable import Variable
 from cvxpy.expressions.expression import Expression
 
@@ -153,14 +154,15 @@
         groupwise_roc_hulls: dict[int, np.ndarray],
         fairness_tolerance: float,
         group_sizes_label_pos: np.ndarray,
         group_sizes_label_neg: np.ndarray,
         global_prevalence: float,
         false_positive_cost: float = 1.,
         false_negative_cost: float = 1.,
+        optimize_for_unfairness: bool = False,
     ) -> tuple[np.ndarray, np.ndarray]:
     """Computes the solution to finding the optimal fair (equal odds) classifier.
 
     Can relax the equal odds constraint by some given tolerance.
 
     Parameters
     ----------
@@ -168,14 +170,17 @@
         A dict mapping each group to the convex hull of the group's ROC curve.
         The convex hull is an np.array of shape (n_points, 2), containing the 
         points that form the convex hull of the ROC curve, sorted in COUNTER
         CLOCK-WISE order.
     fairness_tolerance : float
         A value for the tolerance when enforcing the equal odds fairness 
         constraint, i.e., equality of TPR and FPR among groups.
+        This corresponds to the max allowed violation of the fairness constraint.
+        NOTE: when `optimize_for_unfairness=True`, this instead corresponds
+        to the minimum allowed violation of the fairness constraint.
     group_sizes_label_pos : np.ndarray
         The relative or absolute number of positive samples in each group.
     group_sizes_label_neg : np.ndarray
         The relative or absolute number of negative samples in each group.
     global_prevalence : float
         The global prevalence of positive samples.
     false_positive_cost : float, optional
@@ -205,18 +210,30 @@
         # Global FPR is the average of group FPRs weighted by LNs in each group
         global_roc_point_var[0] == group_sizes_label_neg @ np.array([p[0] for p in groupwise_roc_points_vars]),
 
         # Global TPR is the average of group TPRs weighted by LPs in each group
         global_roc_point_var[1] == group_sizes_label_pos @ np.array([p[1] for p in groupwise_roc_points_vars]),
     ]
 
+    ### New as of v0.0.4: flip the sign for the fairness constraint
+    # this operator corresponds to whether the (l-inf) distance to fairness 
+    # should be 
+    # 1. (fair, default option) leq (<=) the given fairness tolerance, or
+    # 2. (unfair option) geq (>=) the given fairness tolerance;
+    fair_constraint_operator = operator.le
+    if optimize_for_unfairness:
+        fair_constraint_operator = operator.ge
+        logging.warning(f"> compute_equal_odds_optimum :: optimize_for_unfairness={optimize_for_unfairness}")
+
     # Relaxed equal odds constraints
     # 1st option - CONSTRAINT FOR: l-inf distance between any two group's ROCs being less than epsilon
     constraints += [
-        cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j]) <= fairness_tolerance
+        fair_constraint_operator(
+            cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j]),
+            fairness_tolerance)
         for i, j in product(range(n_groups), range(n_groups))
         if i < j
         # if i != j
     ]
 
     # # 2nd option - CONSTRAINT FOR: l-inf distance between any group's ROC and the global being less than epsilon
     # constraints += [
```

### Comparing `equal-odds-0.0.3/equal_odds/equal_odds.py` & `equal-odds-0.0.4/equal_odds/equal_odds.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     def __init__(
             self,
             predictor: Callable[[np.ndarray], np.ndarray],
             tolerance: float,
             false_pos_cost: float = 1.0,
             false_neg_cost: float = 1.0,
             max_roc_ticks: int = 1000,
+            optimize_for_unfairness: bool = False,
             seed: int = 42,
             # distance: str = 'max',    # TODO: add option to use l1 or linf distances
         ):
         """Initializes the relaxed equal odds wrapper.
 
         Parameters
         ----------
@@ -56,42 +57,59 @@
         false_pos_cost : float, optional
             The cost of a FALSE POSITIVE error, by default 1.0.
         false_neg_cost : float, optional
             The cost of a FALSE NEGATIVE error, by default 1.0.
         max_roc_ticks : int, optional
             The maximum number of ticks (points) in each group's ROC, when
             computing the optimal fair classifier, by default 1000.
+        optimize_for_unfairness : bool, optional
+            If `optimize_for_unfairness=True`, the specified tolerance will be
+            the minimum allowed disparity instead of the maximum allowed 
+            disparity.
+            This is useful to compute the entire fairness-accuracy frontier.
+            i.e., `tolerance=0.2 and optimize_for_unfairness` will find the 
+            classifier with highest accuracy given the constraint that 
+            disparity (distance to fairness) is above 0.2.
         seed : int
             A random seed used for reproducibility when producing randomized
             classifiers.
         """
         # Save arguments
         self.predictor = predictor
         self.tolerance = tolerance
         self.false_pos_cost = false_pos_cost
         self.false_neg_cost = false_neg_cost
         self.max_roc_ticks = max_roc_ticks
+        self.optimize_for_unfairness = optimize_for_unfairness
         self.seed = seed
 
+        if self.optimize_for_unfairness:
+            logging.warning(
+                "> `optimize_for_unfairness=True` :: "
+                "will optimize for highest accuracy given a minimum level "
+                "(`tolerance`) of disparity/unfairness. "
+                "USE WITH CARE!"
+            )
+
         # Initialize instance variables
         self._all_roc_data: dict = None
         self._all_roc_hulls: dict = None
         self._groupwise_roc_points: np.ndarray = None
         self._global_roc_point: np.ndarray = None
         self._global_prevalence: float = None
         self._realized_classifier: EnsembleGroupwiseClassifiers = None
-    
+
     @property
     def groupwise_roc_points(self) -> np.ndarray:
         return self._groupwise_roc_points
 
     @property
     def global_roc_point(self) -> np.ndarray:
         return self._global_roc_point
-    
+
     def cost(
             self,
             false_pos_cost: float = None,
             false_neg_cost: float = None,
         ) -> float:
         """Computes the theoretical cost of the solution found.
 
@@ -240,14 +258,15 @@
             groupwise_roc_hulls=self._all_roc_hulls,
             fairness_tolerance=self.tolerance,
             group_sizes_label_pos=group_sizes_label_pos,
             group_sizes_label_neg=group_sizes_label_neg,
             global_prevalence=self._global_prevalence,
             false_positive_cost=self.false_pos_cost,
             false_negative_cost=self.false_neg_cost,
+            optimize_for_unfairness=self.optimize_for_unfairness,
         )
 
         # Construct each group-specific classifier
         all_rand_clfs = {
             g: RandomizedClassifier.construct_at_target_ROC(
                 predictor=self.predictor,
                 roc_curve_data=self._all_roc_data[g],
```

### Comparing `equal-odds-0.0.3/equal_odds/roc_utils.py` & `equal-odds-0.0.4/equal_odds/roc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,19 +139,19 @@
     # NOTE: discarding points below the diagonal seems to lead to bugs later on, idk why...
     # Discard points in the interior of the convex hull,
     # and other useless points (below main diagonal)
     # points_above_diagonal = np.argwhere(roc_points[:, 1] >= roc_points[:, 0]).ravel()
     # hull_indices = sorted(set(hull.vertices) & set(points_above_diagonal))
 
     hull_indices = hull.vertices
-    
+
     logging.info(
         f"ROC convex hull contains {len(hull_indices) / init_num_points:.1%} "
         f"of the original points.")
-    
+
     return roc_points[hull_indices]
 
 
 def plot_polygon_edges(polygon_points, **kwargs):
     from matplotlib import pyplot as plt
     point_to_plot = np.vstack((polygon_points, polygon_points[0]))
     plt.plot(point_to_plot[:, 0], point_to_plot[:, 1], **kwargs)
```

### Comparing `equal-odds-0.0.3/equal_odds.egg-info/PKG-INFO` & `equal-odds-0.0.4/equal_odds.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equal-odds
-Version: 0.0.3
+Version: 0.0.4
 Summary: _PACKAGE IN CONSTRUCTION_
 Home-page: https://github.com/AndreFCruz/equal-odds
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,21 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # equal-odds
 > This repository is under construction :construction:
 
-![badge for PyPI publishing status](https://github.com/AndreFCruz/equal-odds/actions/workflows/python-publish.yml/badge.svg)
+![PyPI publishing status](https://github.com/AndreFCruz/equal-odds/actions/workflows/python-publish.yml/badge.svg)
+![PyPI version](https://badgen.net/pypi/v/equal-odds)
+![OSI license](https://badgen.net/pypi/license/equal-odds)
+![Python compatibility](https://badgen.net/pypi/python/equal-odds)
+<!-- ![PyPI version](https://img.shields.io/pypi/v/equal-odds) -->
+<!-- ![OSI license](https://img.shields.io/pypi/l/equal-odds) -->
+<!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/equal-odds) -->
 
 A fast adjust
 
 ## Installing
 
 Install package from [PyPI](https://pypi.org/project/equal-odds/):
 ```
```

### Comparing `equal-odds-0.0.3/setup.py` & `equal-odds-0.0.4/setup.py`

 * *Files identical despite different names*


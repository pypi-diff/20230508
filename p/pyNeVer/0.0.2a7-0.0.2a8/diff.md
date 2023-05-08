# Comparing `tmp/pyNeVer-0.0.2a7.tar.gz` & `tmp/pyNeVer-0.0.2a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNeVer-0.0.2a7.tar", last modified: Mon Mar 27 13:56:07 2023, max compression
+gzip compressed data, was "pyNeVer-0.0.2a8.tar", last modified: Mon May  8 14:27:36 2023, max compression
```

## Comparing `pyNeVer-0.0.2a7.tar` & `pyNeVer-0.0.2a8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:56:07.592723 pyNeVer-0.0.2a7/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-27 13:55:53.000000 pyNeVer-0.0.2a7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-27 13:55:53.000000 pyNeVer-0.0.2a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-03-27 13:56:07.592723 pyNeVer-0.0.2a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-03-27 13:55:53.000000 pyNeVer-0.0.2a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:56:07.588723 pyNeVer-0.0.2a7/pyNeVer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-03-27 13:56:07.000000 pyNeVer-0.0.2a7/pyNeVer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-27 13:56:07.000000 pyNeVer-0.0.2a7/pyNeVer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:56:07.000000 pyNeVer-0.0.2a7/pyNeVer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 13:56:07.000000 pyNeVer-0.0.2a7/pyNeVer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 13:56:07.000000 pyNeVer-0.0.2a7/pyNeVer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:56:07.588723 pyNeVer-0.0.2a7/pynever/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    31675 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/pytorch_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:56:07.592723 pyNeVer-0.0.2a7/pynever/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54623 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/strategies/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    59586 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/strategies/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/strategies/pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/strategies/smt_reading.py
--rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/strategies/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/strategies/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22617 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/pynever/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-27 13:56:07.592723 pyNeVer-0.0.2a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-27 13:55:54.000000 pyNeVer-0.0.2a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:36.299169 pyNeVer-0.0.2a8/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-08 14:27:22.000000 pyNeVer-0.0.2a8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 14:27:22.000000 pyNeVer-0.0.2a8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-08 14:27:36.299169 pyNeVer-0.0.2a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-08 14:27:22.000000 pyNeVer-0.0.2a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:36.295169 pyNeVer-0.0.2a8/pyNeVer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-08 14:27:36.000000 pyNeVer-0.0.2a8/pyNeVer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 14:27:36.000000 pyNeVer-0.0.2a8/pyNeVer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:27:36.000000 pyNeVer-0.0.2a8/pyNeVer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 14:27:36.000000 pyNeVer-0.0.2a8/pyNeVer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 14:27:36.000000 pyNeVer-0.0.2a8/pyNeVer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:36.295169 pyNeVer-0.0.2a8/pynever/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31675 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/pytorch_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:36.299169 pyNeVer-0.0.2a8/pynever/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54623 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/strategies/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59586 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/strategies/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/strategies/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20632 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/strategies/smt_reading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/strategies/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29343 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/strategies/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22617 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/pynever/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 14:27:36.299169 pyNeVer-0.0.2a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 14:27:23.000000 pyNeVer-0.0.2a8/setup.py
```

### Comparing `pyNeVer-0.0.2a7/LICENSE.txt` & `pyNeVer-0.0.2a8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/PKG-INFO` & `pyNeVer-0.0.2a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNeVer
-Version: 0.0.2a7
+Version: 0.0.2a8
 Summary: Package for the training, pruning and verification of neural networks.
 Home-page: https://github.com/NeVerTools/pyNeVer
 Author: Dario Guidotti
 Author-email: dario.guidotti@edu.unige.it
 License: GNU General Public License with Commons Clause License Condition v1.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyNeVer-0.0.2a7/README.md` & `pyNeVer-0.0.2a8/README.md`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pyNeVer.egg-info/PKG-INFO` & `pyNeVer-0.0.2a8/pyNeVer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNeVer
-Version: 0.0.2a7
+Version: 0.0.2a8
 Summary: Package for the training, pruning and verification of neural networks.
 Home-page: https://github.com/NeVerTools/pyNeVer
 Author: Dario Guidotti
 Author-email: dario.guidotti@edu.unige.it
 License: GNU General Public License with Commons Clause License Condition v1.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyNeVer-0.0.2a7/pyNeVer.egg-info/SOURCES.txt` & `pyNeVer-0.0.2a8/pyNeVer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/datasets.py` & `pyNeVer-0.0.2a8/pynever/datasets.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/networks.py` & `pyNeVer-0.0.2a8/pynever/networks.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/nodes.py` & `pyNeVer-0.0.2a8/pynever/nodes.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/pytorch_layers.py` & `pyNeVer-0.0.2a8/pynever/pytorch_layers.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/strategies/abstraction.py` & `pyNeVer-0.0.2a8/pynever/strategies/abstraction.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/strategies/conversion.py` & `pyNeVer-0.0.2a8/pynever/strategies/conversion.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/strategies/pruning.py` & `pyNeVer-0.0.2a8/pynever/strategies/pruning.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/strategies/smt_reading.py` & `pyNeVer-0.0.2a8/pynever/strategies/smt_reading.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,14 +410,33 @@
             assert b_leaf.is_leaf(), 'The node' + b_leaf + 'was not leaf'
 
             bias_mat[loop] = read_smt_num(b_leaf.data)
             loop += 1
 
         return bias_mat
 
+    @staticmethod
+    def remove_parentheses(cmd: str) -> str:
+        strip_idx = 0
+
+        # Forward
+        while cmd[strip_idx + 1] == '(':
+            strip_idx += 1
+
+        ret = cmd[strip_idx:]
+        strip_idx = len(ret)
+
+        # Backward
+        while ret[strip_idx - 1] == ')':
+            strip_idx -= 1
+
+        ret = ret[:strip_idx + 1]
+
+        return ret
+
     def get_components_of(self, vec_name: str) -> list:
         """
         This method reads the components of the given named vector and
         returns the corresponding list.
 
         Parameters
         ----------
@@ -453,33 +472,48 @@
         NeVerProperty
             The parsed property wrapped in the corresponding class
 
         """
 
         x_assert = self.__get_assert_commands_for(self.x_name)
         y_assert = self.__get_assert_commands_for(self.y_name)
+
         disjunct_list = []
         tree_converter = ExpressionTreeConverter()
 
         # If y_assert contains some 'OR' statement I should separate
         for a in y_assert:
             if '|' in a:
                 tree = tree_converter.build_from_infix(a)
                 disjunct_list.extend(tree.get_disjunctions_infix())
 
+        for i in range(len(disjunct_list)):
+            # Process 'and' in output property
+            if ' & ' in disjunct_list[i]:
+                disjunct_list[i] = disjunct_list[i].split(' & ')
+
+                count = 0
+                for a in disjunct_list[i]:
+                    disjunct_list[i][count] = self.remove_parentheses(a)
+                    count += 1
+
         # Refine assert statements
         for idx, a in enumerate(x_assert):
             x_assert[idx] = refine_smt_statement(a, self.x_name)
 
         if len(disjunct_list) == 0:
             for idx, a in enumerate(y_assert):
                 y_assert[idx] = refine_smt_statement(a, self.y_name)
         else:
-            for idx, a in enumerate(disjunct_list):
-                disjunct_list[idx] = refine_smt_statement(a, self.y_name)
+            for d_idx, statement in enumerate(disjunct_list):
+                if isinstance(statement, list):
+                    for idx, a in enumerate(statement):
+                        disjunct_list[d_idx][idx] = refine_smt_statement(a, self.y_name)
+                else:
+                    disjunct_list[d_idx] = refine_smt_statement(statement, self.y_name)
 
         # Warning without reasons. self.x, self.y ARE lists but PyCharm is not convinced
         self.in_coef_mat = self.__get_coef_mat(self.x, self.x_name, x_assert)
         self.in_bias_mat = self.__get_bias_mat(x_assert)
 
         if len(disjunct_list) == 0:  # If no 'OR' statements are present, just proceed normally
             self.out_coef_mat.append(self.__get_coef_mat(self.y, self.y_name, y_assert))
```

### Comparing `pyNeVer-0.0.2a7/pynever/strategies/training.py` & `pyNeVer-0.0.2a8/pynever/strategies/training.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/pynever/strategies/verification.py` & `pyNeVer-0.0.2a8/pynever/strategies/verification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+import copy
 import logging
 import operator
 import time
 from typing import List, Optional, Callable
 
 import numpy as np
 import torch
@@ -237,16 +238,19 @@
     Attributes
     ----------
 
     heuristic : str
         Heuristic used to decide the refinement level of the ReLU abstraction.
         At present can be only one of the following:
         - given_flags: the neuron to be refined are selected referring to the list given in params
-        - best_n_neurons: for each star the n best neuron to refine are selected based on the loss of precision
+        - best_n_neurons: for each star the best n neuron to refine are selected based on the loss of precision
           the abstraction would incur using the coarse over_approximation.
+        - overapprox: no neuron refinement.
+        - complete: full neuron refinement.
+        - mixed: equal number of neuron refined in each ReLU Layer.
 
     params : List
         Parameters for the heuristic of interest.
         If the heuristic is given_flags then params is a list whose first element is the list of refinement flags.
         If the heuristic is best_n_neurons then params is a list whose first element is the number of neurons to refine.
 
     refinement_level : int
@@ -261,14 +265,15 @@
     def __init__(self, heuristic: str = "best_n_neurons", params: List = None,
                  refinement_level: int = None):
 
         self.heuristic = heuristic
         self.params = params
         self.refinement_level = refinement_level
         self.logger = logging.getLogger(logger_name)
+        self.counterexample_stars = None
 
     @staticmethod
     def __build_abst_network(network: networks.NeuralNetwork, heuristic: str, params: List) -> abst.AbsSeqNetwork:
 
         if not isinstance(network, networks.SequentialNetwork):
             raise Exception("Only sequential networks are supported at present")
 
@@ -279,23 +284,35 @@
         while current_node is not None:
 
             if isinstance(current_node, nodes.FullyConnectedNode):
                 abst_network.add_node(abst.AbsFullyConnectedNode("ABST_" + current_node.identifier, current_node))
 
             elif isinstance(current_node, nodes.ReLUNode):
 
-                if params is None and heuristic == "best_n_neurons":
+                if heuristic == "overapprox":
                     temp_params = [0]
+                    temp_heuristic = "best_n_neurons"
+                elif heuristic == "complete":
+                    temp_params = [current_node.in_dim[0]]
+                    temp_heuristic = "best_n_neurons"
+                elif heuristic == "mixed":
+                    temp_params = params
+                    temp_heuristic = "best_n_neurons"
+                elif params is None and heuristic == "best_n_neurons":
+                    temp_params = [0]
+                    temp_heuristic = heuristic
                 elif params is None and heuristic == "given_flags":
                     temp_params = [False for i in range(len(current_node.in_dim[0]))]
+                    temp_heuristic = heuristic
                 else:
                     temp_params = params[relu_count]
+                    temp_heuristic = heuristic
 
                 abst_network.add_node(abst.AbsReLUNode("ABST_" + current_node.identifier, current_node,
-                                                       heuristic, temp_params))
+                                                       temp_heuristic, temp_params))
 
                 relu_count += 1
 
             else:
                 raise Exception(f"Node type: {current_node.__class__} not supported")
 
             current_node = network.get_next_node(current_node)
@@ -320,65 +337,87 @@
 
             current_node = abst_network.get_next_node(current_node)
 
         return output_starset, n_areas
 
     def verify(self, network: networks.NeuralNetwork, prop: Property) -> (bool, Optional[Tensor]):
 
+        self.counterexample_stars = None
         abst_network = self.__build_abst_network(network, self.heuristic, self.params)
-
         ver_start_time = time.perf_counter()
-
         if isinstance(prop, NeVerProperty):
 
             output_starset, n_areas = self.__compute_output_starset(abst_network, prop)
 
             out_coef_mat = prop.out_coef_mat
             out_bias_mat = prop.out_bias_mat
 
         else:
             raise Exception("Only NeVerProperty are supported at present")
 
-        or_verified = []
+        # Now we check the itersection of the output starset with the output halfspaces defined by the output
+        # constraints of our property of interest. We recall that the property is satisfiable if there exist at least
+        # one non-void intersection between the output starset and the halfspaces.
+        unsafe_stars = []
+        all_empty = []
         for i in range(len(out_coef_mat)):
 
-            verified = True
+            empty = True
             for star in output_starset.stars:
                 out_coef = out_coef_mat[i]
                 out_bias = out_bias_mat[i]
                 temp_star = abst.intersect_with_halfspace(star, out_coef, out_bias)
                 if not temp_star.check_if_empty():
-                    verified = False
+                    empty = False
+                    if self.heuristic == 'complete':
+                        unsafe_stars.append(temp_star)
 
-            or_verified.append(verified)
+            all_empty.append(empty)
 
-        final_verified = any(or_verified)
+        is_satisfied = not all(all_empty)
 
+        if len(unsafe_stars) > 0:
+            self.counterexample_stars = self.__get_counterexample_stars(prop, unsafe_stars)
         ver_end_time = time.perf_counter()
-        self.logger.info(f"Verification Result: {final_verified}.")
+        self.logger.info(f"The property is satisfiable: {is_satisfied}.")
         self.logger.info(f"Verification Time: {ver_end_time - ver_start_time}\n")
 
-        return final_verified
+        return is_satisfied
 
     def get_output_starset(self, network: networks.NeuralNetwork, prop: Property):
 
+        self.counterexample_stars = None
         abst_network = self.__build_abst_network(network, self.heuristic, self.params)
 
         computing_start_time = time.perf_counter()
 
         if isinstance(prop, NeVerProperty):
             output_starset, n_areas = self.__compute_output_starset(abst_network, prop)
         else:
             raise NotImplementedError
 
         computing_end_time = time.perf_counter()
         computing_time = computing_end_time - computing_start_time
 
         return output_starset, computing_time
 
+    def __get_counterexample_stars(self, prop: Property, unsafe_stars: List[abst.Star]):
+
+        if not isinstance(prop, NeVerProperty):
+            raise NotImplementedError
+
+        counterexample_stars = []
+        for unsafe_star in unsafe_stars:
+            temp_star = abst.Star(prop.in_coef_mat, prop.in_bias_mat)
+            temp_star.predicate_matrix = copy.deepcopy(unsafe_star.predicate_matrix)
+            temp_star.predicate_bias = copy.deepcopy(unsafe_star.predicate_bias)
+            counterexample_stars.append(temp_star)
+
+        return counterexample_stars
+
 
 class NeverVerificationRef(VerificationStrategy):
     """
     Class used to represent the Never verification strategy with counter example guided refinement.
 
     Attributes
     ----------
```

### Comparing `pyNeVer-0.0.2a7/pynever/utilities.py` & `pyNeVer-0.0.2a8/pynever/utilities.py`

 * *Files identical despite different names*

### Comparing `pyNeVer-0.0.2a7/setup.py` & `pyNeVer-0.0.2a8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyNeVer",
-    version="0.0.2.alpha7",
+    version="0.0.2.a8",
     author="Dario Guidotti",
     author_email="dario.guidotti@edu.unige.it",
     license='GNU General Public License with Commons Clause License Condition v1.0',
     description="Package for the training, pruning and verification of neural networks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NeVerTools/pyNeVer",
```


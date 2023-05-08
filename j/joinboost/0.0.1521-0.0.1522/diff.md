# Comparing `tmp/joinboost-0.0.1521.tar.gz` & `tmp/joinboost-0.0.1522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joinboost-0.0.1521.tar", last modified: Sat Mar  4 22:53:11 2023, max compression
+gzip compressed data, was "joinboost-0.0.1522.tar", last modified: Mon May  8 20:42:13 2023, max compression
```

## Comparing `joinboost-0.0.1521.tar` & `joinboost-0.0.1522.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-03-04 22:53:11.903759 joinboost-0.0.1521/
--rw-rw-r--   0 zach      (1002) zach      (1002)    11357 2022-10-17 20:12:04.000000 joinboost-0.0.1521/LICENSE
--rw-rw-r--   0 zach      (1002) zach      (1002)       34 2023-01-12 20:11:12.000000 joinboost-0.0.1521/MANIFEST.in
--rw-rw-r--   0 zach      (1002) zach      (1002)     2868 2023-03-04 22:53:11.903759 joinboost-0.0.1521/PKG-INFO
--rw-rw-r--   0 zach      (1002) zach      (1002)     2688 2023-03-04 22:52:18.000000 joinboost-0.0.1521/README.md
--rw-rw-r--   0 zach      (1002) zach      (1002)      226 2023-03-04 22:52:54.000000 joinboost-0.0.1521/pyproject.toml
--rw-rw-r--   0 zach      (1002) zach      (1002)       38 2023-03-04 22:53:11.903759 joinboost-0.0.1521/setup.cfg
--rw-rw-r--   0 zach      (1002) zach      (1002)      152 2023-01-12 20:10:27.000000 joinboost-0.0.1521/setup.py
-drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-03-04 22:53:11.903759 joinboost-0.0.1521/src/
-drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-03-04 22:53:11.903759 joinboost-0.0.1521/src/joinboost/
--rw-rw-r--   0 zach      (1002) zach      (1002)        0 2022-10-19 21:40:29.000000 joinboost-0.0.1521/src/joinboost/__init__.py
--rw-rw-r--   0 zach      (1002) zach      (1002)     3304 2022-10-19 18:39:31.000000 joinboost-0.0.1521/src/joinboost/aggregator.py
--rw-rw-r--   0 zach      (1002) zach      (1002)    17616 2023-03-04 22:51:54.000000 joinboost-0.0.1521/src/joinboost/app.py
--rw-rw-r--   0 zach      (1002) zach      (1002)    10014 2022-12-11 21:44:57.000000 joinboost-0.0.1521/src/joinboost/cjt.py
--rw-rw-r--   0 zach      (1002) zach      (1002)   227230 2022-10-26 02:53:18.000000 joinboost-0.0.1521/src/joinboost/d3graph.html
--rw-rw-r--   0 zach      (1002) zach      (1002)    11502 2023-03-03 00:00:35.000000 joinboost-0.0.1521/src/joinboost/executor.py
--rw-rw-r--   0 zach      (1002) zach      (1002)    13060 2023-03-03 00:51:21.000000 joinboost-0.0.1521/src/joinboost/joingraph.py
--rw-rw-r--   0 zach      (1002) zach      (1002)     2655 2023-03-03 00:26:27.000000 joinboost-0.0.1521/src/joinboost/semiring.py
-drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-03-04 22:53:11.903759 joinboost-0.0.1521/src/joinboost.egg-info/
--rw-rw-r--   0 zach      (1002) zach      (1002)     2868 2023-03-04 22:53:11.000000 joinboost-0.0.1521/src/joinboost.egg-info/PKG-INFO
--rw-rw-r--   0 zach      (1002) zach      (1002)      476 2023-03-04 22:53:11.000000 joinboost-0.0.1521/src/joinboost.egg-info/SOURCES.txt
--rw-rw-r--   0 zach      (1002) zach      (1002)        1 2023-03-04 22:53:11.000000 joinboost-0.0.1521/src/joinboost.egg-info/dependency_links.txt
--rw-rw-r--   0 zach      (1002) zach      (1002)       10 2023-03-04 22:53:11.000000 joinboost-0.0.1521/src/joinboost.egg-info/top_level.txt
--rw-rw-r--   0 zach      (1002) zach      (1002)     1767 2022-10-22 21:13:41.000000 joinboost-0.0.1521/src/test_joingraph.py
--rw-rw-r--   0 zach      (1002) zach      (1002)     9693 2023-02-21 01:58:28.000000 joinboost-0.0.1521/src/test_model_basic.py
--rw-rw-r--   0 zach      (1002) zach      (1002)     7643 2023-03-03 00:59:14.000000 joinboost-0.0.1521/src/test_model_reliable.py
+drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-05-08 20:42:13.612674 joinboost-0.0.1522/
+-rw-rw-r--   0 zach      (1002) zach      (1002)    11357 2022-10-17 20:12:04.000000 joinboost-0.0.1522/LICENSE
+-rw-rw-r--   0 zach      (1002) zach      (1002)       34 2023-01-12 20:11:12.000000 joinboost-0.0.1522/MANIFEST.in
+-rw-rw-r--   0 zach      (1002) zach      (1002)     3459 2023-05-08 20:42:13.612674 joinboost-0.0.1522/PKG-INFO
+-rw-rw-r--   0 zach      (1002) zach      (1002)     3279 2023-05-07 22:11:33.000000 joinboost-0.0.1522/README.md
+-rw-rw-r--   0 zach      (1002) zach      (1002)      226 2023-05-08 20:42:05.000000 joinboost-0.0.1522/pyproject.toml
+-rw-rw-r--   0 zach      (1002) zach      (1002)       38 2023-05-08 20:42:13.612674 joinboost-0.0.1522/setup.cfg
+-rw-rw-r--   0 zach      (1002) zach      (1002)      152 2023-01-12 20:10:27.000000 joinboost-0.0.1522/setup.py
+drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-05-08 20:42:13.608674 joinboost-0.0.1522/src/
+drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-05-08 20:42:13.612674 joinboost-0.0.1522/src/joinboost/
+-rw-rw-r--   0 zach      (1002) zach      (1002)        0 2022-10-19 21:40:29.000000 joinboost-0.0.1522/src/joinboost/__init__.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)     7474 2023-05-08 20:38:11.000000 joinboost-0.0.1522/src/joinboost/aggregator.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)    23103 2023-05-08 20:38:11.000000 joinboost-0.0.1522/src/joinboost/app.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)    10749 2023-05-08 20:38:11.000000 joinboost-0.0.1522/src/joinboost/cjt.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)   227230 2022-10-26 02:53:18.000000 joinboost-0.0.1522/src/joinboost/d3graph.html
+-rw-rw-r--   0 zach      (1002) zach      (1002)    47846 2023-05-08 20:38:11.000000 joinboost-0.0.1522/src/joinboost/executor.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)    22715 2023-05-08 00:22:41.000000 joinboost-0.0.1522/src/joinboost/joingraph.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)     3737 2023-05-06 22:10:55.000000 joinboost-0.0.1522/src/joinboost/preprocessor.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)     4272 2023-05-06 22:10:55.000000 joinboost-0.0.1522/src/joinboost/semiring.py
+drwxrwxr-x   0 zach      (1002) zach      (1002)        0 2023-05-08 20:42:13.612674 joinboost-0.0.1522/src/joinboost.egg-info/
+-rw-rw-r--   0 zach      (1002) zach      (1002)     3459 2023-05-08 20:42:13.000000 joinboost-0.0.1522/src/joinboost.egg-info/PKG-INFO
+-rw-rw-r--   0 zach      (1002) zach      (1002)      506 2023-05-08 20:42:13.000000 joinboost-0.0.1522/src/joinboost.egg-info/SOURCES.txt
+-rw-rw-r--   0 zach      (1002) zach      (1002)        1 2023-05-08 20:42:13.000000 joinboost-0.0.1522/src/joinboost.egg-info/dependency_links.txt
+-rw-rw-r--   0 zach      (1002) zach      (1002)       10 2023-05-08 20:42:13.000000 joinboost-0.0.1522/src/joinboost.egg-info/top_level.txt
+-rw-rw-r--   0 zach      (1002) zach      (1002)     2588 2023-05-07 01:01:09.000000 joinboost-0.0.1522/src/test_joingraph.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)    11364 2023-05-07 19:26:59.000000 joinboost-0.0.1522/src/test_model_basic.py
+-rw-rw-r--   0 zach      (1002) zach      (1002)    10154 2023-05-07 04:00:10.000000 joinboost-0.0.1522/src/test_model_reliable.py
```

### Comparing `joinboost-0.0.1521/LICENSE` & `joinboost-0.0.1522/LICENSE`

 * *Files identical despite different names*

### Comparing `joinboost-0.0.1521/PKG-INFO` & `joinboost-0.0.1522/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-Metadata-Version: 2.1
-Name: joinboost
-Version: 0.0.1521
-Summary: JoinBoost: In-Database Tree-Models over Many Tables
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JoinBoost: In-Database Tree-Models over Many Tables
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 JoinBoost is a Python library to help you train tree-models (decision trees, gradient boosting, random forests). 
 
+Note that many functionalities of JoinBoost are still under development. If you are interested in using JoinBoost, we are happy to provide direct supports. You can contact us through issues, or email zh2408@columbia.edu
+
 ## Why JoinBoost?
 
 JoinBoost algorithms follow LightGBM. However, JoinBoost trains models
 
 1. **Inside Database**: JoinBoost translates ML algorithms into SQL queries, and directly executes these queries in your databases. This means:
     - **Safety**: There is no data movement.
     - **Transformation**: You can directly do OLAP and data transformation in SQL.
@@ -45,15 +40,25 @@
 dataset.add_join("sales", "items", ["item_nbr"], ["item_nbr"])
 
 reg = DecisionTree(learning_rate=1, max_leaves=8)
 reg.fit(dataset)
 ```
 
 
-[Please Check out this notebook for Demo](https://anonymous.4open.science/r/JoinBoost-FBC4/demo/JoinBoostDemo.ipynb)
+[Please Check out this notebook for Demo](https://colab.research.google.com/github/zachary62/JoinBoost/blob/main/demo/JoinBoostDemo.ipynb)
+
+For dev: https://gitpod.io/new#https://github.com/zachary62/JoinBoost
+
+## Docs
+
+Documentation is currently under development. To build docs locally, download [Sphinx](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html) and run
+```bash
+make html
+```
+in the folder `docs`. The docs will be generated in the folder `docs/build/html`.
 
 ## Reproducibility
 
 The technical report of JoinBoost could be found under /technical directory.
 
 We note that some optimizations discussed in the paper (e.g., inter-query parallelism, DP) are still under development in the main codes. To reproduce the experiment results from the paper, we include the prototype codes for JoinBoost under /proto folder, which includes all the optimizations. We also include Jupyter Notebook to help you use these codes to train models over Favorita.
```

### Comparing `joinboost-0.0.1521/README.md` & `joinboost-0.0.1522/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+Metadata-Version: 2.1
+Name: joinboost
+Version: 0.0.1522
+Summary: JoinBoost: In-Database Tree-Models over Many Tables
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # JoinBoost: In-Database Tree-Models over Many Tables
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 JoinBoost is a Python library to help you train tree-models (decision trees, gradient boosting, random forests). 
 
+Note that many functionalities of JoinBoost are still under development. If you are interested in using JoinBoost, we are happy to provide direct supports. You can contact us through issues, or email zh2408@columbia.edu
+
 ## Why JoinBoost?
 
 JoinBoost algorithms follow LightGBM. However, JoinBoost trains models
 
 1. **Inside Database**: JoinBoost translates ML algorithms into SQL queries, and directly executes these queries in your databases. This means:
     - **Safety**: There is no data movement.
     - **Transformation**: You can directly do OLAP and data transformation in SQL.
@@ -38,15 +47,25 @@
 dataset.add_join("sales", "items", ["item_nbr"], ["item_nbr"])
 
 reg = DecisionTree(learning_rate=1, max_leaves=8)
 reg.fit(dataset)
 ```
 
 
-[Please Check out this notebook for Demo](https://anonymous.4open.science/r/JoinBoost-FBC4/demo/JoinBoostDemo.ipynb)
+[Please Check out this notebook for Demo](https://colab.research.google.com/github/zachary62/JoinBoost/blob/main/demo/JoinBoostDemo.ipynb)
+
+For dev: https://gitpod.io/new#https://github.com/zachary62/JoinBoost
+
+## Docs
+
+Documentation is currently under development. To build docs locally, download [Sphinx](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html) and run
+```bash
+make html
+```
+in the folder `docs`. The docs will be generated in the folder `docs/build/html`.
 
 ## Reproducibility
 
 The technical report of JoinBoost could be found under /technical directory.
 
 We note that some optimizations discussed in the paper (e.g., inter-query parallelism, DP) are still under development in the main codes. To reproduce the experiment results from the paper, we include the prototype codes for JoinBoost under /proto folder, which includes all the optimizations. We also include Jupyter Notebook to help you use these codes to train models over Favorita.
```

### Comparing `joinboost-0.0.1521/src/joinboost/app.py` & `joinboost-0.0.1522/src/joinboost/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,395 +1,590 @@
 import math
 from abc import ABC
+
+from .preprocessor import Preprocessor, RenameStep
+from .executor import SPJAData, PandasExecutor, ExecuteMode
 from .joingraph import JoinGraph
 from .semiring import *
-from .aggregator import Aggregator, Annotation, Message
+from .aggregator import *
 from .cjt import CJT
 from queue import PriorityQueue
 import numpy as np
 from typing import Union
 
 
 class App(ABC):
     def __init__(self):
         pass
-    
+
+
 class DummyModel(App):
     def __init__(self):
         super().__init__()
         self.semi_ring = varSemiRing()
         self.prefix = "joinboost_tmp_"
         self.model_def = []
-    
-    def fit(self,
-           jg: JoinGraph):
         
+    def fit(self, jg: JoinGraph):
+        self._fit(jg)
+    
+    def _fit(self, jg: JoinGraph):
         jg._preprocess()
-        self.semi_ring.init_columns_name(jg)
-        
+
         # get the gradient and hessian
         # for rmse, g is the sum and h is the count
-        agg_exp = self.semi_ring.col_sum((jg.get_target_var(), '1'))
-        g, h = jg.exe.execute_spja_query(agg_exp,
-                                          [jg.get_target_relation()],
-                                          mode = 3)[0]
-        
+        agg_exp = self.semi_ring.col_sum((jg.target_var, "1"))
+        spja_data = SPJAData(
+            aggregate_expressions=agg_exp, from_tables=[jg.target_relation]
+        )
+        g, h = jg.exe.execute_spja_query(spja_data, mode=ExecuteMode.EXECUTE)[0]
+
         prediction = g / h
         self.semi_ring.set_semi_ring(g, h)
-        
+
         # below currently only works for rmse
         self.count_ = h
         self.constant_ = prediction
-        
-        # store full join sql
-        self._full_join_sql = jg.get_full_join_sql()
 
     def predict(self, data: Union[str, JoinGraph], input_mode: int):
         return self.constant_
-    
+
 
 class DecisionTree(DummyModel):
-    def __init__(self,                
-                 max_leaves: int = 31,
-                 learning_rate: float = 1, 
-                 max_depth: int = 6,
-                 subsample: float = 1,
-                 debug: bool = False):
-        
+    def __init__(
+        self,
+        max_leaves: int = 31,
+        learning_rate: float = 1,
+        max_depth: int = 6,
+        subsample: float = 1,
+        debug: bool = False,
+    ):
+
         super().__init__()
         self.max_leaves = max_leaves
         self.learning_rate = learning_rate
         self.max_depth = max_depth
         self.subsample = subsample
         self.debug = debug
+        self.preprocessor = Preprocessor()
+
+    def _fit(self, jg: JoinGraph):
+        jg._preprocess()
+        
         
-    def fit(self,
-           jg: JoinGraph):
-        # super().fit(jg)
-        self.semi_ring.init_columns_name(jg)
+        # First, we run preprocess to rename reserved column name
+        # Create views for tables having conflicting column names with reserved words.
+        g, h = self.semi_ring.get_columns_name()
+
+        self.preprocessor.add_step(RenameStep(reserved_words=[g, h, "rowid"]))
+        self.preprocessor.run_preprocessing(jg)
+        jg = self.preprocessor.get_join_graph()
+
         # shall we first sample then fit dummy model, or first fit dummy model then sample?
         # the current solution is to first sample than fit dummy model
         self.cjt = CJT(semi_ring=self.semi_ring, join_graph=jg)
         self.create_sample()
-        super().fit(jg)
+
+        super()._fit(jg)
         
-        self.cjt.lift(self.cjt.get_target_var() + "- (" + str(self.constant_) + ")")
-        self.semi_ring.set_semi_ring(0, self.count_)
+        # substracting the target variable by means
+        exp = agg_to_sql(AggExpression(Aggregator.SUB, (self.cjt.target_var, str(self.constant_))))
         
+#         if isinstance(self.cjt.exe, PandasExecutor):
+#             exp = lambda row: row[self.cjt.target_var] - self.constant_
+
+        self.cjt.lift(exp)
+        self.semi_ring.set_semi_ring(0, self.count_)
+
         self.train_one()
-    
-    def create_sample(self, mode=1):
+
+    def create_sample(self, mode=ExecuteMode.WRITE_TO_TABLE):
         if self.subsample < 1:
             # TODO: Possible to sample 0 tuples.
             # Add check to make sure the sampled table has tuples
-            # For duckdb, mode 4 is only safe for single thread.
-            new_fact_name = self.cjt.exe.execute_spja_query(from_tables=[self.cjt.target_relation], 
-                                                            sample_rate=self.subsample,
-                                                            mode = mode)
+            spja_data = SPJAData(
+                from_tables=[self.cjt.target_relation],
+                sample_rate=self.subsample,
+            )
+            new_fact_name = self.cjt.exe.execute_spja_query(spja_data, mode=mode)
             self.cjt.replace(self.cjt.target_relation, new_fact_name)
-        
-    
-    def train_one(self, last = True):
+
+    def train_one(self, last=True):
         # store (node_id) -> cjt
         self.nodes = {}
         self.nodes[0] = self.cjt
-        
+
         # store a pq of split_candidates, sorted on the criteria
         # this one is a bit complex. TODO: simplify or make it a class
         self.split_candidates = PriorityQueue()
-        
+
         # leaf_nodes is used to compute the final models
         self.leaf_nodes = []
-        
+
         self._build_tree()
         if last:
             self._update_error()
-            
+
         self._build_model()
         # TODO: should clean all temp tables, not just messages
         if not self.debug:
             self._clean_messages()
-        
+
     def _build_model(self):
         cur_model_def = []
         for cur_cjt in self.leaf_nodes:
             annotations = cur_cjt.get_all_parsed_annotations()
             g, h = cur_cjt.get_semi_ring().get_value()
-            
-            pred = float(g / h)* self.learning_rate
+
+            pred = float(g / h) * self.learning_rate
             if annotations:
                 cur_model_def.append((pred, annotations))
         if cur_model_def:
             self.model_def.append(cur_model_def)
-        
+
     def compute_rmse(self, test_table: str):
+        target = self.preprocessor.get_original_target_name()
+
         # TODO: refactor
-        view = self.cjt.exe.case_query(test_table, '+', 'prediction', str(self.constant_),
-                                       self.model_def, [self.cjt.get_target_var()])
-        predict_agg = {'RMSE': 
-            (f'SQRT(AVG(POW({self.cjt.get_target_var()} - prediction, 2)))',
-             Aggregator.IDENTITY)}
-        predict = self.cjt.exe.execute_spja_query(predict_agg, [view], mode=4)
-        return self.cjt.exe.execute_spja_query(from_tables=[predict], 
-                                               mode=3)[0]
-    
-    # input_mode = 1 takes the full join's table name as input
-    # input_mode = 2 takes the join graph as input (assume fact table)
-    # input_mode = 3 takes the fact table's name as input (and automatically join it
-    # with dimensional tables used in training)
-    # TODO: support different outputs
-    # output_mode = 1 returns a numpy array
-    # output_mode = 2 stores the prediction in a table and returns table name
-    def predict(self, data: Union[str, JoinGraph], 
-                input_mode: int = 1,
-                output_mode: int = 1,):
-        
-        if input_mode == 1:
-            assert(isinstance(data, str))
-            view = self.cjt.exe.case_query(data, '+', 'prediction',
-                                           str(self.constant_), self.model_def,
-                                           [self.cjt.get_target_var()])
-
-        elif input_mode == 2:
-            assert(isinstance(data, JoinGraph))
-            # TODO
-            pass
-
-        elif input_mode == 3:
-            assert(isinstance(data, str))
-            view = self.cjt.exe.case_query(self._full_join_sql, '+', 'prediction', 
-                                           str(self.constant_), self.model_def,
-                                           [self.cjt.get_target_var()],
-                                           order_by=f'{data}.rowid')
+        view = self.cjt.exe.case_query(
+            test_table, "+", "prediction", str(self.constant_), self.model_def, [target]
+        )
+
+        predict_agg = {
+            "RMSE": (f"SQRT(AVG(POW({target} - prediction, 2)))", Aggregator.IDENTITY)
+        }
+        prediction_query_data = SPJAData(
+            aggregate_expressions=predict_agg, from_tables=[view]
+        )
+
+        predict = self.cjt.exe.execute_spja_query(
+            prediction_query_data, mode=ExecuteMode.NESTED_QUERY
+        )
+        rmse_query_data = SPJAData(from_tables=[predict])
+        return self.cjt.exe.execute_spja_query(
+            rmse_query_data, mode=ExecuteMode.EXECUTE
+        )[0]
+
+    # input_mode = "FULL_JOIN_JG" takes the join graph as input, with the full join specified by JG._target_relation
+    # input_mode = "FULL_JOIN_DF" takes the dataframe of full join's table name as input
+    # input_mode = "JOIN_GRAPH" takes the join graph as input (assume the same schema as training data)
+    # output_mode = "NUMPY" returns a numpy array
+    # output_mode = "WRITE_TO_TABLE" stores the prediction in a table and returns table name
+    def predict(
+        self,
+        joingraph: JoinGraph,
+        input_mode: str = "FULL_JOIN_JG",
+        output_mode: str = "NUMPY",
+    ):
+        input_modes = ["FULL_JOIN_JG", "FULL_JOIN_DF", "JOIN_GRAPH"]
+        output_modes = ["NUMPY", "WRITE_TO_TABLE"]
+        if input_mode not in input_modes:
+            raise Exception("Unsupported input_mode")
+        if output_mode not in output_modes:
+            raise Exception("Unsupported output_mode")
+
+        if input_mode == "FULL_JOIN_JG":
+            # TODO: one concern of full join is that, there would be ambiguity for features with the same name but from table
+            # E.g., R(A,B), S(A,B). They join on A, and B is a feature name shared by both.
+            # The full will have ambiguous naming, and may be renamed to (A, R.B, S.B)
+            # To avoid this, requires a rename mapping from users. By default, we consider renaming mapping which prefixes the feature with relation name.
+            view = joingraph.exe.case_query(
+                joingraph.target_relation,
+                "+",
+                "prediction",
+                str(self.constant_),
+                self.model_def,
+                [self.cjt.target_var],
+            )
+        if input_mode == "JOIN_GRAPH":
+            # TODO: reapply all the preprocessing steps
+            self._update_fact_table_column_name(jg=joingraph, check_rowid_col=True)
+
+            full_join = joingraph.get_full_join_sql()
+            # the reason why we order by rowid is because of the set semantics of the relational models
+            # e.g., for duckdb, join result has its row order shuffled, making it hard to decide the corresponding prediction
+            # we therefore sort by rowid to enforce the correct ordering
+            view = joingraph.exe.case_query(
+                full_join,
+                "+",
+                "prediction",
+                str(self.constant_),
+                self.model_def,
+                [self.cjt.target_var],
+                order_by=f"{joingraph.target_relation}.rowid",
+            )
+            self._update_fact_table_column_name(jg=joingraph, resume_rowid_col=True)
+
+        if output_mode == "NUMPY":
+            preds = joingraph.exe._execute_query(f"select prediction from {view};")
+            return np.array(preds)[:, 0]
+        elif output_mode == "WRITE_TO_TABLE":
+            return view
+
+    def _update_fact_table_column_name(
+        self, jg, check_rowid_col=False, resume_rowid_col=False
+    ):
+        """Rename/resume fact table's rowid column(if exists)."""
+
+        if jg.check_target_relation_contains_rowid_col():
+            if check_rowid_col:
+                old_name, new_name = "rowid", jg.target_rowid_colname
+
+            if resume_rowid_col:
+                old_name, new_name = jg.target_rowid_colname, "rowid"
 
-        preds = self.cjt.exe._execute_query(f"select prediction from {view};")
-        return np.array(preds)[:, 0]
+            sql = f"ALTER TABLE {jg.target_relation} RENAME COLUMN {old_name} TO {new_name};"
+            self.cjt.exe._execute_query(sql)
 
     def _clean_messages(self):
         for cjt in self.nodes.values():
             cjt.clean_message()
 
-    def _comp_annotations(self, r_name: str, attr: str, cur_value: str, obj: float, expanding_cjt: CJT):
-        attr_type = expanding_cjt.get_relation_schema()[r_name][attr]
+    def _comp_annotations(
+        self, r_name: str, attr: str, cur_value: str, obj: float, expanding_cjt: CJT
+    ):
+        attr_type = expanding_cjt.relation_schema[r_name][attr]
         g_col, h_col = self.semi_ring.get_columns_name()
 
         # TODO: remove window_query and everything is spja
-        if attr_type == 'LCAT':
+        if attr_type == "LCAT":
             group_by = [attr]
             absoprtion_view = expanding_cjt.absorption(r_name, [attr])
-            agg_exp = {attr: (attr, Aggregator.IDENTITY),
-                       'object': ((g_col, h_col), Aggregator.DIV),
-                       g_col: (g_col, Aggregator.IDENTITY),
-                       h_col: (h_col, Aggregator.IDENTITY)}
-            obj_view = self.cjt.exe.execute_spja_query(agg_exp, [absoprtion_view])
-            view_ord_by_obj = self.cjt.exe.window_query(obj_view, [attr], 'object', [g_col, h_col])
-            attr_view = self.cjt.exe.execute_spja_query({attr: (attr, Aggregator.IDENTITY)},
-                                                        [view_ord_by_obj],
-                                                        [f'{g_col}/{h_col} <=' + str(obj)])
-            attrs = [str(x[0])  for x in self.cjt.exe.execute_spja_query(from_tables=[attr_view], mode=3)]
-            l_annotation = (attr, Annotation.IN, attrs)
-            r_annotation = (attr, Annotation.NOT_IN, attrs)
-        elif cur_value == 'NULL':
-            l_annotation = (attr, Annotation.NULL, Annotation.NULL)
-            r_annotation = (attr, Annotation.NOT_NULL, Annotation.NOT_NULL)
-        elif attr_type == 'NUM':
-            l_annotation = (attr, Annotation.NOT_GREATER, cur_value)
-            r_annotation = (attr, Annotation.GREATER, cur_value)
-        elif attr_type == 'CAT':
-            l_annotation = (attr, Annotation.NOT_DISTINCT, cur_value)
-            r_annotation = (attr, Annotation.DISTINCT, cur_value)
+            agg_exp = {
+                attr: (attr, Aggregator.IDENTITY),
+                "object": ((g_col, h_col), Aggregator.DIV),
+                g_col: (g_col, Aggregator.IDENTITY),
+                h_col: (h_col, Aggregator.IDENTITY),
+            }
+            spja_data = SPJAData(
+                aggregate_expressions=agg_exp, from_tables=[absoprtion_view]
+            )
+            obj_view = self.cjt.exe.execute_spja_query(
+                spja_data, mode=ExecuteMode.NESTED_QUERY
+            )
+            view_ord_by_obj = self.cjt.exe.window_query(
+                obj_view, [attr], "object", [g_col, h_col]
+            )
+            attr_spja_data = SPJAData(
+                aggregate_expressions={attr: (attr, Aggregator.IDENTITY)},
+                from_tables=[view_ord_by_obj],
+                # TODO: the {g_col}/{h_col} should be a qualified attribute 
+                select_conds=[SelectionExpression(SELECTION.NOT_GREATER,(f"{g_col}/{h_col}",str(obj)))]
+                
+            )
+            attr_view = self.cjt.exe.execute_spja_query(
+                attr_spja_data, mode=ExecuteMode.NESTED_QUERY
+            )
+            attrs = [
+                str(x[0])
+                for x in self.cjt.exe.execute_spja_query(
+                    SPJAData(from_tables=[attr_view]), mode=ExecuteMode.EXECUTE
+                )
+            ]
+            agg_exp = {
+                attr: (attr, Aggregator.IDENTITY),
+                "object": ((g_col, h_col), Aggregator.DIV),
+                g_col: (g_col, Aggregator.IDENTITY),
+                h_col: (h_col, Aggregator.IDENTITY),
+            }
+            obj_spja_data = SPJAData(
+                aggregate_expressions=agg_exp, from_tables=[absoprtion_view]
+            )
+            obj_view = self.cjt.exe.execute_spja_query(
+                obj_spja_data, mode=ExecuteMode.NESTED_QUERY
+            )
+            view_ord_by_obj = self.cjt.exe.window_query(
+                obj_view, [attr], "object", [g_col, h_col]
+            )
+            attr_view_data = SPJAData(
+                aggregate_expressions={attr: (attr, Aggregator.IDENTITY)},
+                from_tables=[view_ord_by_obj],
+                select_conds=[SelectionExpression(SELECTION.NOT_GREATER,(f"{g_col}/{h_col}",str(obj)))]
+            )
+            attr_view = self.cjt.exe.execute_spja_query(
+                attr_view_data, mode=ExecuteMode.NESTED_QUERY
+            )
+
+            attrs = [
+                str(x[0])
+                for x in self.cjt.exe.execute_spja_query(
+                    SPJAData(from_tables=[attr_view]), mode=ExecuteMode.EXECUTE
+                )
+            ]
+            l_annotation = SelectionExpression(SELECTION.IN, (QualifiedAttribute(r_name,attr), attrs))
+            r_annotation = SelectionExpression(SELECTION.NOT_IN, (QualifiedAttribute(r_name,attr), attrs))
+        elif cur_value == "NULL":
+            l_annotation = SelectionExpression(SELECTION.NULL, QualifiedAttribute(r_name,attr))
+            r_annotation = SelectionExpression(SELECTION.NOT_NULL, QualifiedAttribute(r_name,attr))
+        elif attr_type == "NUM":
+            l_annotation = SelectionExpression(SELECTION.NOT_GREATER, (QualifiedAttribute(r_name,attr), cur_value))
+            r_annotation = SelectionExpression(SELECTION.GREATER, (QualifiedAttribute(r_name,attr), cur_value))
+        elif attr_type == "CAT":
+            l_annotation = SelectionExpression(SELECTION.NOT_DISTINCT, (QualifiedAttribute(r_name,attr), cur_value))
+            r_annotation = SelectionExpression(SELECTION.DISTINCT, (QualifiedAttribute(r_name,attr), cur_value))
         else:
-            raise Exception('Unsupported Split')
+            raise Exception("Unsupported Split")
         return l_annotation, r_annotation
 
     # get best split of current cjt
     def _get_best_split(self, cjt_id: int, cjt_depth: int):
         cjt = self.nodes[cjt_id]
         cur_semi_ring = cjt.get_semi_ring()
-        attr_meta = self.cjt.get_relation_schema()
+        attr_meta = self.cjt.relation_schema
         g_col, h_col = self.semi_ring.get_columns_name()
-        
+
         # criteria, (relation name, split attribute, split value, new s, new c)
-        best_criteria, best_criteria_ann = 0, ('', '', 0, 0, 0)
-        
+        best_criteria, best_criteria_ann = 0, ("", "", 0, 0, 0)
+
         if cjt_depth == self.max_depth:
-            self.split_candidates.put((-best_criteria, cjt_depth,) + best_criteria_ann + (cjt_id,))
+            self.split_candidates.put(
+                (
+                    -best_criteria,
+                    cjt_depth,
+                )
+                + best_criteria_ann
+                + (cjt_id,)
+            )
             return
-        
+
         g, h = cur_semi_ring.get_value()
-        const_ = float((g**2)/h)
-        for r_name in cjt.get_relations():
+        const_ = float((g**2) / h)
+        for r_name in cjt.relations:
             for attr in cjt.get_relation_features(r_name):
                 attr_type, group_by = self.cjt.get_type(r_name, attr), [attr]
-                absoprtion_view = cjt.absorption(r_name, group_by, mode=4)
-                if attr_type == 'NUM':
+                absoprtion_view = cjt.absorption(r_name, group_by)
+                if attr_type == "NUM":
                     agg_exp = cur_semi_ring.col_sum((g_col, h_col))
                     agg_exp[attr] = (attr, Aggregator.IDENTITY)
-                    view_to_max = self.cjt.exe.execute_spja_query(agg_exp,
-                                                                  [absoprtion_view], 
-                                                                  window_by=[attr],
-                                                                  mode=4)
-                
-                elif attr_type == 'LCAT':
+                    spja_data = SPJAData(
+                        aggregate_expressions=agg_exp,
+                        from_tables=[absoprtion_view],
+                        window_by=[attr],
+                    )
+                    view_to_max = self.cjt.exe.execute_spja_query(
+                        spja_data, mode=ExecuteMode.NESTED_QUERY
+                    )
+
+                elif attr_type == "LCAT":
                     # TODO: further optimization. We don't need to keep the attr.
                     # The only thing we care for splitting is the sum_s/sum_c
-                    agg_exp = {attr: (attr, Aggregator.IDENTITY),
-                               'object': ((g_col, h_col), Aggregator.DIV),
-                               g_col: (g_col, Aggregator.IDENTITY),
-                               h_col: (h_col, Aggregator.IDENTITY)}
-                    obj_view = self.cjt.exe.execute_spja_query(agg_exp, 
-                                                               [absoprtion_view],
-                                                               mode=4)
+                    agg_exp = {
+                        attr: (attr, Aggregator.IDENTITY),
+                        "object": ((g_col, h_col), Aggregator.DIV),
+                        g_col: (g_col, Aggregator.IDENTITY),
+                        h_col: (h_col, Aggregator.IDENTITY),
+                    }
+                    spja_data = SPJAData(
+                        aggregate_expressions=agg_exp, from_tables=[absoprtion_view]
+                    )
+                    obj_view = self.cjt.exe.execute_spja_query(
+                        spja_data, mode=ExecuteMode.NESTED_QUERY
+                    )
                     agg_exp = cur_semi_ring.col_sum((g_col, h_col))
                     agg_exp[attr] = (attr, Aggregator.IDENTITY)
-                    agg_exp['object'] = ('object', Aggregator.IDENTITY)
-                    view_to_max = self.cjt.exe.execute_spja_query(agg_exp,
-                                                                  [obj_view], 
-                                                                  window_by=['object'],
-                                                                  mode=4)
-                elif attr_type == 'CAT':
+                    agg_exp["object"] = ("object", Aggregator.IDENTITY)
+                    spja_data = SPJAData(
+                        aggregate_expressions=agg_exp,
+                        from_tables=[obj_view],
+                        window_by=["object"],
+                    )
+                    view_to_max = self.cjt.exe.execute_spja_query(
+                        spja_data, mode=ExecuteMode.NESTED_QUERY
+                    )
+                elif attr_type == "CAT":
                     view_to_max = absoprtion_view
-                    
+
+                # check if executor is of type PandasExecutor or DuckdbExecutor
+                # TODO: move this logic somewhere else
+                if isinstance(self.cjt.exe, PandasExecutor):
+                    func = (
+                        lambda row: (row[f"{g_col}"] / row[f"{h_col}"])
+                        * row[f"{g_col}"]
+                        + ((g - row["s"]) / (h - row["c"])) * (g - row["s"])
+                        if h > row["c"]
+                        else 0
+                    )
+                else:
+                    func = (
+                        "CASE WHEN "
+                        + str(h)
+                        + f" > {h_col} THEN (({g_col}/{h_col})*{g_col} + ("
+                        + str(g)
+                        + f"-{g_col})/("
+                        + str(h)
+                        + f"-{h_col})*("
+                        + str(g)
+                        + f"-{g_col})) ELSE 0 END"
+                    )
+
                 l2_agg_exp = {
                     attr: (attr, Aggregator.IDENTITY),
-                    'criteria': (
-                    f"""CASE WHEN {h} > {h_col}
-                            THEN (
-                                ({g_col} / {h_col}) * {g_col} +
-                                ({g} - {g_col}) / ({h} - {h_col}) * ({g} - {g_col})
-                            )
-                            ELSE 0
-                        END
-                    """, Aggregator.IDENTITY),
-                    
+                    "criteria": (func, Aggregator.IDENTITY_LAMBDA),
                     g_col: (g_col, Aggregator.IDENTITY),
                     h_col: (h_col, Aggregator.IDENTITY),
-                    
                 }
-                results = self.cjt.exe.execute_spja_query(l2_agg_exp, 
-                                                          [view_to_max], 
-                                                          order_by='criteria DESC', 
-                                                          limit=1, 
-                                                          mode=3)
+                spja_data = SPJAData(
+                    aggregate_expressions=l2_agg_exp,
+                    from_tables=[view_to_max],
+                    order_by=[("criteria", "DESC")],
+                    limit=1,
+                )
+                results = self.cjt.exe.execute_spja_query(
+                    spja_data, mode=ExecuteMode.EXECUTE
+                )
                 if not results:
                     continue
                 cur_value, cur_criteria, left_g, left_h = results[0]
+                # print((cur_value, cur_criteria, left_g, left_h))
                 if cur_criteria > best_criteria:
                     best_criteria = cur_criteria
                     # relation name, split attribute, split value, left gradient, left hessian
                     best_criteria_ann = (r_name, attr, str(cur_value), left_g, left_h)
-        self.split_candidates.put((const_-best_criteria, cjt_depth,) + best_criteria_ann + (cjt_id,))
-        
+        self.split_candidates.put(
+            (
+                const_ - float(best_criteria),
+                cjt_depth,
+            )
+            + best_criteria_ann
+            + (cjt_id,)
+        )
+
     # split the semi-ring according to current split
-    def split_semi_ring(self, 
-                        total_semi_ring: varSemiRing, 
-                        left_semi_ring: varSemiRing):
+    def split_semi_ring(
+        self, total_semi_ring: varSemiRing, left_semi_ring: varSemiRing
+    ):
         return left_semi_ring, total_semi_ring - left_semi_ring
-    
-    # don't update error for single ecision tree 
+
+    # don't update error for single ecision tree
     def _update_error(self):
         pass
-    
-    def _get_split_cjt(self, expanding_cjt: CJT, l_semi_ring: varSemiRing, r_semi_ring: varSemiRing):
-        l_cjt, r_cjt = expanding_cjt.copy_cjt(l_semi_ring), expanding_cjt.copy_cjt(r_semi_ring)
+
+    def _get_split_cjt(
+        self, expanding_cjt: CJT, l_semi_ring: varSemiRing, r_semi_ring: varSemiRing
+    ):
+        l_cjt, r_cjt = expanding_cjt.copy_cjt(l_semi_ring), expanding_cjt.copy_cjt(
+            r_semi_ring
+        )
         next_id = len(self.nodes)
-        
+
         self.nodes[next_id] = l_cjt
         self.nodes[next_id + 1] = r_cjt
-        
+
         return l_cjt, r_cjt, next_id, next_id + 1
 
     def _build_tree(self):
         self.cjt.calibration()
         self._get_best_split(0, 0)
-        
-        # while there are beneficial splits and doesn't read max leaves 
-        while not self.split_candidates.empty() and \
-              self.split_candidates.queue[0][0] < 0 and \
-              self.split_candidates.qsize() < self.max_leaves:
-            criteria, cur_level, r_name, attr, cur_value, left_g, left_h, c_id = self.split_candidates.get()
+
+        # while there are beneficial splits and doesn't read max leaves
+        while (
+            not self.split_candidates.empty()
+            and self.split_candidates.queue[0][0] < 0
+            and self.split_candidates.qsize() < self.max_leaves
+        ):
+            (
+                criteria,
+                cur_level,
+                r_name,
+                attr,
+                cur_value,
+                left_g,
+                left_h,
+                c_id,
+            ) = self.split_candidates.get()
             expanding_cjt = self.nodes[c_id]
-            
+
             l_semi_ring = expanding_cjt.semi_ring.copy()
             l_semi_ring.set_semi_ring(left_g, left_h)
-            
-            l_semi_ring, r_semi_ring = self.split_semi_ring(expanding_cjt.get_semi_ring(), l_semi_ring)
 
-            l_cjt, r_cjt, l_id, r_id = self._get_split_cjt(expanding_cjt=expanding_cjt,
-                                                           l_semi_ring=l_semi_ring,
-                                                           r_semi_ring=r_semi_ring)
+
+            l_semi_ring, r_semi_ring = self.split_semi_ring(
+                expanding_cjt.get_semi_ring(), l_semi_ring
+            )
+
+            l_cjt, r_cjt, l_id, r_id = self._get_split_cjt(
+                expanding_cjt=expanding_cjt,
+                l_semi_ring=l_semi_ring,
+                r_semi_ring=r_semi_ring,
+            )
             # TODO: objective has some rounding problem
             # currently it has an ugly solution. find a better solution
-            l_annotations, r_annotations = self._comp_annotations(r_name=r_name, 
-                                                                  attr=attr,
-                                                                  cur_value=cur_value,
-                                                                  obj=math.ceil(left_g / left_h * 100) / 100,
-                                                                  expanding_cjt=expanding_cjt)
-            
+            l_annotations, r_annotations = self._comp_annotations(
+                r_name=r_name,
+                attr=attr,
+                cur_value=cur_value,
+                obj=math.ceil(left_g / left_h * 100) / 100,
+                expanding_cjt=expanding_cjt,
+            )
+
             # add annotations according to split conditions
             l_cjt.add_annotations(r_name, l_annotations)
             r_cjt.add_annotations(r_name, r_annotations)
-            
+
             # for the leaf split_candidates that can't be splitted (e.g. meet max depth)
             # we still need message passing to fact table for semi-join selection
-            # but not necessarily downward_message_passing. 
+            # but not necessarily downward_message_passing.
             # Can be optimized to upward_message_passing(fact)
             l_cjt.downward_message_passing(r_name)
             r_cjt.downward_message_passing(r_name)
-            
+
             self._get_best_split(l_id, cur_level + 1)
+            # print('level, right g, h')
+            # print((cur_level, r_cjt.semi_ring.pair[0], r_cjt.semi_ring.pair[1]))
             self._get_best_split(r_id, cur_level + 1)
-                
+
         self.leaf_nodes = [self.nodes[ele[-1]] for ele in self.split_candidates.queue]
 
 
-        
 class GradientBoosting(DecisionTree):
     # TODO: add some checks. E.g., paramters have to be positive
-    def __init__(self,
-                 max_leaves: int = 31,
-                 learning_rate: float = 1, 
-                 max_depth: int = 6,
-                 iteration: int = 1,
-                 debug: bool = False):
-        super().__init__(max_leaves,learning_rate,max_depth,debug=debug)
+    def __init__(
+        self,
+        max_leaves: int = 31,
+        learning_rate: float = 1,
+        max_depth: int = 6,
+        iteration: int = 1,
+        debug: bool = False,
+    ):
+        super().__init__(max_leaves, learning_rate, max_depth, debug=debug)
         self.iteration = iteration
-    
-    def fit(self,
-           jg: JoinGraph):
-        super().fit(jg)
-        
+
+    def _fit(self, jg: JoinGraph):
+        super()._fit(jg)
+
         for _ in range(self.iteration - 1):
             self.train_one()
 
     def _update_error(self):
         for cur_cjt in self.leaf_nodes:
             cur_cond = []
-            target_relation = cur_cjt.get_target_relation()
+            target_relation = cur_cjt.target_relation
             g, h = cur_cjt.get_semi_ring().get_value()
             pred = g / h * self.learning_rate
-            _, join_conds = cur_cjt._get_income_messages(cur_cjt.get_target_relation(), condition=2)
-            join_conds += cur_cjt.get_parsed_annotations(target_relation)
+            _, join_conds = cur_cjt._get_income_messages(
+                cur_cjt.target_relation, condition=2
+            )
+
             g_col, _ = self.semi_ring.get_columns_name()
-            self.cjt.exe.update_query(f"{g_col}={g_col}-({pred})",
-                                      target_relation,
-                                      join_conds)
-            
+            self.cjt.exe.update_query(
+                f"{g_col}={g_col}-({pred})", target_relation, join_conds + cur_cjt.get_annotations(target_relation)
+            )
+
+
 class RandomForest(DecisionTree):
-    def __init__(self,
-                 max_leaves: int = 31,
-                 learning_rate: float = 1, 
-                 max_depth: int = 6,
-                 subsample: float = 1,
-                 iteration: int = 1,
-                 debug: bool = False):
-        super().__init__(max_leaves,learning_rate,max_depth,subsample,debug=debug)
+    def __init__(
+        self,
+        max_leaves: int = 31,
+        learning_rate: float = 1,
+        max_depth: int = 6,
+        subsample: float = 1,
+        iteration: int = 1,
+        debug: bool = False,
+    ):
+        super().__init__(max_leaves, learning_rate, max_depth, subsample, debug=debug)
         self.iteration = iteration
-        self.learning_rate = 1/iteration
-    
-    def fit(self,
-           jg: JoinGraph):
-        
+        self.learning_rate = 1 / iteration
+
+    def _fit(self, jg: JoinGraph):
+
         for _ in range(self.iteration):
-            super().fit(jg)
-            
-            
+            super()._fit(jg)
```

### Comparing `joinboost-0.0.1521/src/joinboost/cjt.py` & `joinboost-0.0.1522/src/joinboost/cjt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,218 +1,271 @@
 import copy
 from .semiring import SemiRing
 from .joingraph import JoinGraph
-from .executor import Executor
+from .executor import Executor, PandasExecutor, SPJAData, ExecuteMode
 from .aggregator import *
 
 
 class CJT(JoinGraph):
-    def __init__(self, 
-                 semi_ring: SemiRing, 
-                 join_graph: JoinGraph, 
-                 annotations: dict = {}):
+    def __init__(
+        self, semi_ring: SemiRing, join_graph: JoinGraph, annotations: dict = {}
+    ):
         self.message_id = 0
         self.semi_ring = semi_ring
-        super().__init__(join_graph.exe,
-                         join_graph.joins, 
-                         join_graph.relation_schema,
-                         join_graph.target_var,
-                         join_graph.target_relation)
+        super().__init__(
+            join_graph.exe,
+            join_graph.joins,
+            join_graph.relation_schema,
+            join_graph.target_var,
+            join_graph.target_relation,
+        )
         # CJT get the join structure from this
         self.annotations = annotations
 
-
     def get_message(self, from_table: str, to_table: str):
-        return self.joins[from_table][to_table]['message']
+        return self.joins[from_table][to_table]["message"]
 
-    def get_parsed_annotations(self, table):
-        if table not in self.annotations:
-            return []
-        return parse_ann({table: self.annotations[table]})
+    def get_annotations(self, table):
+        # return self.annotations[table] if in the dict, otherwise return empty list
+        return self.annotations.get(table, [])
+        # return selections_to_sql(self.annotations[table])
+
+    # not qualified by default becuase the join table is different from orginal table
+    def get_all_parsed_annotations(self, qualified: bool = False):
+        # self.annotations is a dict of selectionExpressions, and the key is the table name
+        list_of_ann = []
+        for _, value in self.annotations.items():
+            list_of_ann.extend(value)
 
-    def get_all_parsed_annotations(self):
-        return parse_ann(self.annotations, True)
+        return selections_to_sql(list_of_ann, qualified)
 
     def add_annotations(self, r_name: str, annotation: str):
         if r_name not in self.annotations:
             self.annotations[r_name] = [annotation]
         else:
             self.annotations[r_name].append(annotation)
 
     def clean_message(self):
         for from_table in self.joins:
             for to_table in self.joins[from_table]:
-                if self.joins[from_table][to_table]['message_type'] != Message.IDENTITY:
-                    m_name = self.joins[from_table][to_table]['message']
+                if self.joins[from_table][to_table]["message_type"] != Message.IDENTITY:
+                    m_name = self.joins[from_table][to_table]["message"]
                     self.exe.delete_table(m_name)
 
-    def get_semi_ring(self): 
+    def get_semi_ring(self):
         return self.semi_ring
 
     def copy_cjt(self, semi_ring: SemiRing):
         annotations = copy.deepcopy(self.annotations)
-        c_cjt = CJT(semi_ring=semi_ring, 
-                    join_graph=self, 
+        c_cjt = CJT(semi_ring=semi_ring, join_graph=self,
                     annotations=annotations)
         return c_cjt
 
     def get_root_neighbors(self):
-        joins, neighbors = self.get_joins(), {}
+        joins, neighbors = self.joins, {}
         for table in joins[self.target_relation]:
-            if self.joins[table][self.target_relation]['message_type'] != Message.IDENTITY:
-                neighbors[table] = (self.get_join_keys(self.target_relation, table),
-                                    self.get_message(table, self.target_relation))
+            if (
+                self.joins[table][self.target_relation]["message_type"]
+                != Message.IDENTITY
+            ):
+                neighbors[table] = (
+                    self.get_join_keys(self.target_relation, table),
+                    self.get_message(table, self.target_relation),
+                )
         return neighbors
-    
+
     def calibration(self, rooto_table: str = None):
         if not rooto_table:
             rooto_table = self.target_relation
-        self.upward_message_passing(rooto_table, m_type = Message.IDENTITY)
-        self.downward_message_passing(rooto_table, m_type = Message.FULL)
+        self.upward_message_passing(rooto_table, m_type=Message.IDENTITY)
+        self.downward_message_passing(rooto_table, m_type=Message.FULL)
 
-    def downward_message_passing(self, 
-                                 rooto_table: str = None, 
-                                 m_type: Message = Message.UNDECIDED):
+    def downward_message_passing(
+        self, rooto_table: str = None, m_type: Message = Message.UNDECIDED
+    ):
         msgs = []
         if not rooto_table:
             rooto_table = self.target_relation
         self._pre_dfs(rooto_table, m_type=m_type)
         return msgs
-    
+
     # TODO: this is not working if upward_message_passing from non-fact table
-    def upward_message_passing(self, rooto_table: str = None, 
-                               m_type: Message = Message.UNDECIDED):
+    def upward_message_passing(
+        self, rooto_table: str = None, m_type: Message = Message.UNDECIDED
+    ):
         if not rooto_table:
             rooto_table = self.target_relation
         self._post_dfs(rooto_table, m_type=m_type)
 
-    def _post_dfs(self, currento_table: str, 
-                  parent_table: str = None, 
-                  m_type: Message = Message.UNDECIDED):
-        jg = self.get_joins()
+    def _post_dfs(
+        self,
+        currento_table: str,
+        parent_table: str = None,
+        m_type: Message = Message.UNDECIDED,
+    ):
+        jg = self.joins
         if currento_table not in jg:
             return
         for c_neighbor in jg[currento_table]:
             if c_neighbor != parent_table:
                 self._post_dfs(c_neighbor, currento_table, m_type=m_type)
         if parent_table:
-            self._send_message(from_table=currento_table, to_table=parent_table, m_type=m_type)
-
-    def _pre_dfs(self, currento_table: str, 
-                 parent_table: str = None, 
-                 m_type: Message = Message.UNDECIDED):
-        joins = self.get_joins()
+            self._send_message(
+                from_table=currento_table, to_table=parent_table, m_type=m_type
+            )
+
+    def _pre_dfs(
+        self,
+        currento_table: str,
+        parent_table: str = None,
+        m_type: Message = Message.UNDECIDED,
+    ):
+        joins = self.joins
         if currento_table not in joins:
             return
         if currento_table == self.target_relation:
             m_type = Message.FULL
         for c_neighbor in joins[currento_table]:
             if c_neighbor != parent_table:
                 self._send_message(currento_table, c_neighbor, m_type=m_type)
                 self._pre_dfs(c_neighbor, currento_table, m_type=m_type)
 
-    def absorption(self, table: str, group_by: list, mode=4):
+    def absorption(self, table: str, group_by: list, mode=ExecuteMode.NESTED_QUERY):
         from_table_attrs = self.get_relation_features(table)
         incoming_messages, join_conds = self._get_income_messages(table)
-        
+
         cols = self.semi_ring.get_columns_name()
         aggregate_expressions = self.semi_ring.col_sum(cols)
         for attr in group_by:
-            aggregate_expressions[attr] = (table + "." + attr, Aggregator.IDENTITY)
-        
-        return self.exe.execute_spja_query(aggregate_expressions, 
-                                           from_tables=[m['message'] for m in incoming_messages]+[table], 
-                                           select_conds=join_conds+self.get_parsed_annotations(table),
-                                           group_by=[table + '.' + attr for attr in group_by], 
-                                           mode=mode)
+            aggregate_expressions[attr] = (
+                table + "." + attr, Aggregator.IDENTITY)
+
+        spja_data = SPJAData(
+            aggregate_expressions=aggregate_expressions,
+            from_tables=[m["message"] for m in incoming_messages] + [table],
+            join_conds=join_conds,
+            select_conds=self.get_annotations(table),
+            group_by=[table + "." + attr for attr in group_by],
+        )
+
+        return self.exe.execute_spja_query(spja_data, mode=mode)
 
-    
     # get the incoming message from one table to another
     # key function for message passing, Sec 3.3 of CJT paper
     # allow two types of join condition: 1 is for selection, 2 is for semi-join
-    def _get_income_messages(self, 
-                             table: str, 
-                             excluded_table: str = '', 
-                             condition=1, semi_join_opt=True):
+    def _get_income_messages(
+        self, table: str, excluded_table: str = "", condition=1, semi_join_opt=True
+    ):
         incoming_messages, join_conds = [], []
         for neighbour_table in self.joins[table]:
             # if neighbour_table != excluded_table:
             incoming_message = self.joins[neighbour_table][table]
-            if incoming_message['message_type'] == Message.IDENTITY:
+            if incoming_message["message_type"] == Message.IDENTITY:
                 continue
-            
+
             # semijoin optimization
             # Naively, the table is excluded
             # but we can use its message for semi-join to accelerate message passing
             if excluded_table == neighbour_table:
                 if semi_join_opt:
                     incoming_message = copy.deepcopy(incoming_message)
-                    incoming_message['message_type'] = Message.SELECTION
+                    incoming_message["message_type"] = Message.SELECTION
                 else:
                     continue
 
             # get the join conditions between from_table and incoming_message
-            l_join_keys, r_join_keys = self.get_join_keys(neighbour_table, table)
+            l_join_keys, r_join_keys = self.get_join_keys(
+                neighbour_table, table)
             incoming_messages.append(incoming_message)
             if condition == 1:
-                join_conds += [incoming_message["message"] + "." + l_join_keys[i] + " IS NOT DISTINCT FROM " +
-                               table + "." + r_join_keys[i] for i in range(len(l_join_keys))]
+                join_conds += [
+                    SelectionExpression(SELECTION.NOT_DISTINCT,
+                                        (QualifiedAttribute(incoming_message["message"], l_join_keys[i]),
+                                         QualifiedAttribute(table, r_join_keys[i])))
+                    for i in range(len(l_join_keys))
+                ]
             if condition == 2:
-                join_conds += ['(' + ','.join([table + '.' + key for key in r_join_keys]) + ') in (SELECT (' 
-                               + ','.join([incoming_message["message"] + '.' + key for key in l_join_keys]) 
-                               + ') FROM ' + incoming_message["message"] + ')']
+                join_conds += [
+                    SelectionExpression(SELECTION.SEMI_JOIN,
+                                        ([QualifiedAttribute(table, key) for key in r_join_keys],
+                                         [QualifiedAttribute(incoming_message["message"], key) for key in l_join_keys]))
+                ]
         return incoming_messages, join_conds
 
-
     # 3 message types: identity, selection, FULL
-    def _send_message(self, from_table: str, to_table: str, m_type: Message = Message.UNDECIDED):
-    # print('--Sending Message from', from_table, 'to', to_table, 'm_type is', m_type)
+    def _send_message(
+        self, from_table: str, to_table: str, m_type: Message = Message.UNDECIDED
+    ):
+        # print('--Sending Message from', from_table, 'to', to_table, 'm_type is', m_type)
         # identity message optimization
         if m_type == Message.IDENTITY:
-            self.joins[from_table][to_table].update({'message_type': m_type,})
+            self.joins[from_table][to_table].update(
+                {
+                    "message_type": m_type,
+                }
+            )
             return
-        
+
         if from_table not in self.joins and to_table not in self.joins[from_table]:
-            raise Exception('Table', from_table, 'and table', to_table, 'are not connected')
-        
+            raise Exception(
+                "Table", from_table, "and table", to_table, "are not connected"
+            )
+
         # join with incoming messages
-        incoming_messages, join_conds = self._get_income_messages(from_table, to_table)
-        
+        incoming_messages, join_conds = self._get_income_messages(
+            from_table, to_table)
+
         # assume fact table. Relax it for many-to-many!!
         if m_type == Message.UNDECIDED:
             if from_table == self.target_relation:
                 m_type = Message.FULL
             else:
                 m_type = Message.SELECTION
-                for message_type in [m['message_type'] for m in incoming_messages]:
+                for message_type in [m["message_type"] for m in incoming_messages]:
                     if message_type == Message.FULL:
                         m_type = Message.FULL
 
         # get the group_by key for this message
         l_join_keys, _ = self.get_join_keys(from_table, to_table)
-        
+
         # compute aggregation
         cols = self.semi_ring.get_columns_name()
-        aggregation = (self.semi_ring.col_sum(cols) if m_type == Message.FULL else {})
+        aggregation = self.semi_ring.col_sum(
+            cols) if m_type == Message.FULL else {}
         for attr in l_join_keys:
             aggregation[attr] = (from_table + "." + attr, Aggregator.IDENTITY)
 
-        message_name = self.exe.execute_spja_query(aggregation, 
-                                                    from_tables=[m['message'] for m in incoming_messages]+[from_table], 
-                                                    select_conds=join_conds+self.get_parsed_annotations(from_table),
-                                                    group_by=[from_table + '.' + attr for attr in l_join_keys], 
-                                                    mode=1)
-
-        self.joins[from_table][to_table].update({'message': message_name, 'message_type': m_type})
-    
-    # by default, lift the target variale
-    def lift(self, var = None):
+        spja_data = SPJAData(
+            aggregate_expressions=aggregation,
+            from_tables=[m["message"]
+                         for m in incoming_messages] + [from_table],
+            join_conds=join_conds,
+            select_conds=self.get_annotations(from_table),
+            group_by=[from_table + "." + attr for attr in l_join_keys],
+        )
+        message_name = self.exe.execute_spja_query(
+            spja_data, mode=ExecuteMode.WRITE_TO_TABLE
+        )
+
+        self.joins[from_table][to_table].update(
+            {"message": message_name, "message_type": m_type}
+        )
+
+    # by default, lift the target variable
+    def lift(self, var=None):
         if var is None:
             var = self.target_var
         lift_exp = self.semi_ring.lift_exp(var)
+        # TODO: remove hack
+        if isinstance(self.exe, PandasExecutor):
+            lift_exp["s"] = (var, Aggregator.IDENTITY_LAMBDA)
         # copy the rest attributes
         for attr in self.get_useful_attributes(self.target_relation):
             lift_exp[attr] = (attr, Aggregator.IDENTITY)
-        new_fact_name = self.exe.execute_spja_query(lift_exp,
-                                                    [self.target_relation],
-                                                    mode = 1)
+
+        spja_data = SPJAData(
+            aggregate_expressions=lift_exp, from_tables=[self.target_relation]
+        )
+        new_fact_name = self.exe.execute_spja_query(
+            spja_data, mode=ExecuteMode.WRITE_TO_TABLE
+        )
         self.replace(self.target_relation, new_fact_name)
```

### Comparing `joinboost-0.0.1521/src/joinboost/d3graph.html` & `joinboost-0.0.1522/src/joinboost/d3graph.html`

 * *Files identical despite different names*

### Comparing `joinboost-0.0.1521/src/joinboost.egg-info/PKG-INFO` & `joinboost-0.0.1522/src/joinboost.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: joinboost
-Version: 0.0.1521
+Version: 0.0.1522
 Summary: JoinBoost: In-Database Tree-Models over Many Tables
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JoinBoost: In-Database Tree-Models over Many Tables
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 JoinBoost is a Python library to help you train tree-models (decision trees, gradient boosting, random forests). 
 
+Note that many functionalities of JoinBoost are still under development. If you are interested in using JoinBoost, we are happy to provide direct supports. You can contact us through issues, or email zh2408@columbia.edu
+
 ## Why JoinBoost?
 
 JoinBoost algorithms follow LightGBM. However, JoinBoost trains models
 
 1. **Inside Database**: JoinBoost translates ML algorithms into SQL queries, and directly executes these queries in your databases. This means:
     - **Safety**: There is no data movement.
     - **Transformation**: You can directly do OLAP and data transformation in SQL.
@@ -45,15 +47,25 @@
 dataset.add_join("sales", "items", ["item_nbr"], ["item_nbr"])
 
 reg = DecisionTree(learning_rate=1, max_leaves=8)
 reg.fit(dataset)
 ```
 
 
-[Please Check out this notebook for Demo](https://anonymous.4open.science/r/JoinBoost-FBC4/demo/JoinBoostDemo.ipynb)
+[Please Check out this notebook for Demo](https://colab.research.google.com/github/zachary62/JoinBoost/blob/main/demo/JoinBoostDemo.ipynb)
+
+For dev: https://gitpod.io/new#https://github.com/zachary62/JoinBoost
+
+## Docs
+
+Documentation is currently under development. To build docs locally, download [Sphinx](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html) and run
+```bash
+make html
+```
+in the folder `docs`. The docs will be generated in the folder `docs/build/html`.
 
 ## Reproducibility
 
 The technical report of JoinBoost could be found under /technical directory.
 
 We note that some optimizations discussed in the paper (e.g., inter-query parallelism, DP) are still under development in the main codes. To reproduce the experiment results from the paper, we include the prototype codes for JoinBoost under /proto folder, which includes all the optimizations. We also include Jupyter Notebook to help you use these codes to train models over Favorita.
```

### Comparing `joinboost-0.0.1521/src/test_model_basic.py` & `joinboost-0.0.1522/src/test_model_basic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,206 +1,271 @@
 import unittest
 import math
-import time
 import pandas as pd
 import numpy as np
 import duckdb
 import lightgbm
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import GradientBoostingRegressor
 from sklearn.metrics import mean_squared_error
 from joinboost.executor import DuckdbExecutor
 from joinboost.joingraph import JoinGraph
-from joinboost.app import DecisionTree,GradientBoosting,RandomForest
+from joinboost.app import DecisionTree, GradientBoosting, RandomForest
+
 
 class TestModel(unittest.TestCase):
-        
+
+    # TODO: some table have the same attribute name, making it hard to predict
+    def test_demo(self):
+        con = duckdb.connect(database=':memory:')
+        con.execute("CREATE TABLE customer AS SELECT * FROM '../data/demo/customer.csv'")
+        con.execute("CREATE TABLE lineorder AS SELECT * FROM '../data/demo/lineorder.csv'")
+        con.execute("CREATE TABLE date AS SELECT * FROM '../data/demo/date.csv'")
+        con.execute("CREATE TABLE part AS SELECT * FROM '../data/demo/part.csv'")
+        con.execute("CREATE TABLE supplier AS SELECT * FROM '../data/demo/supplier.csv'")
+        x = ["NAME", "ADDRESS", "CITY", "NAME", "MFGR", "CATEGORY", "BRAND1", "DATE", "DAYOFWEEK",
+             "MONTH", "YEAR", "YEARMONTH", "YEARMONTHNUM", "DAYNUMINWEEK", "NAME", "ADDRESS", "CITY", "NATION"]
+        y = "REVENUE"
+        # delete rows beyond 1000 in lineorder using duckdb
+        # con.execute("DELETE FROM lineorder WHERE rowid > 1000")
+
+        exe = DuckdbExecutor(con, debug=False)
+
+        dataset = JoinGraph(exe=exe)
+        dataset.add_relation('lineorder', [], y='REVENUE', relation_address='../data/demo/lineorder.csv')
+        dataset.add_relation('customer', ['NAME', 'ADDRESS', 'CITY'], relation_address='../data/demo/customer.csv')
+        dataset.add_relation('part', ['NAME', 'MFGR', 'CATEGORY', 'BRAND1'], relation_address='../data/demo/part.csv')
+        dataset.add_relation('date', ['DATE', 'DAYOFWEEK', 'MONTH', 'YEAR', 'YEARMONTH', 'YEARMONTHNUM', 'DAYNUMINWEEK'], relation_address='../data/demo/date.csv')
+        dataset.add_relation('supplier', ['NAME', 'ADDRESS', 'CITY', 'NATION'], relation_address='../data/demo/supplier.csv')
+        dataset.add_join("customer", "lineorder", ["CUSTKEY"], ["CUSTKEY"])
+        dataset.add_join("part", "lineorder", ["PARTKEY"], ["PARTKEY"])
+        dataset.add_join("date", "lineorder", ["DATEKEY"], ["ORDERDATE"])
+        dataset.add_join("supplier", "lineorder", ["SUPPKEY"], ["SUPPKEY"])
+
+        depth = 3
+        gb = DecisionTree(learning_rate=1, max_leaves=2 ** depth, max_depth=depth)
+
+        gb.fit(dataset)
+
+        for line in gb.model_def:
+            for subline in line:
+                print(subline)
+        # clf = DecisionTreeRegressor(max_depth=depth)
+        # clf = clf.fit(join[x], join[y])
+        # mse = mean_squared_error(join[y], clf.predict(join[x]))
+
+        # self.assertTrue(abs(gb.compute_rmse('test')[0] - math.sqrt(mse)) < 1e-3)
+
     def test_synthetic(self):
         join = pd.read_csv("../data/synthetic/RST.csv")
-        con = duckdb.connect(database=':memory:')
-        con.execute("CREATE TABLE R AS SELECT * FROM '../data/synthetic/R.csv'")
-        con.execute("CREATE TABLE S AS SELECT * FROM '../data/synthetic/S.csv'")
-        con.execute("CREATE TABLE T AS SELECT * FROM '../data/synthetic/T.csv'")
+        con = duckdb.connect(database=":memory:")
         con.execute("CREATE TABLE test AS SELECT * FROM '../data/synthetic/RST.csv'")
         x = ["A", "B", "D", "E", "F"]
         y = "H"
 
         exe = DuckdbExecutor(con, debug=False)
-    
+
         dataset = JoinGraph(exe=exe)
-        dataset.add_relation('R', ['B', 'D'], y = 'H')
-        dataset.add_relation('S', ['A', 'E'])
-        dataset.add_relation('T', ['F'])
+        dataset.add_relation('R', ['B', 'D'], y='H', relation_address='../data/synthetic/R.csv')
+        dataset.add_relation('S', ['A', 'E'], relation_address='../data/synthetic/S.csv')
+        dataset.add_relation('T', ['F'], relation_address='../data/synthetic/T.csv')
         dataset.add_join("R", "S", ["A"], ["A"])
         dataset.add_join("R", "T", ["B"], ["B"])
-        
+
         depth = 3
-        gb = DecisionTree(learning_rate=1, max_leaves=2 ** depth, max_depth=depth)
-        
+        gb = DecisionTree(learning_rate=1, max_leaves=2**depth, max_depth=depth)
+
         gb.fit(dataset)
-        
+
         clf = DecisionTreeRegressor(max_depth=depth)
         clf = clf.fit(join[x], join[y])
         mse = mean_squared_error(join[y], clf.predict(join[x]))
-        self.assertTrue(abs(gb.compute_rmse('test')[0] - math.sqrt(mse)) < 1e-3)
-    
+        self.assertTrue(abs(gb.compute_rmse("test")[0] - math.sqrt(mse)) < 1e-3)
+
     def test_favorita(self):
         con = duckdb.connect(database=':memory:')
-        con.execute("CREATE OR REPLACE TABLE holidays AS SELECT * FROM '../data/favorita/holidays.csv';")
-        con.execute("CREATE OR REPLACE TABLE oil AS SELECT * FROM '../data/favorita/oil.csv';")
-        con.execute("CREATE OR REPLACE TABLE transactions AS SELECT * FROM '../data/favorita/transactions.csv';")
-        con.execute("CREATE OR REPLACE TABLE stores AS SELECT * FROM '../data/favorita/stores.csv';")
-        con.execute("CREATE OR REPLACE TABLE items AS SELECT * FROM '../data/favorita/items.csv';")
-        con.execute("CREATE OR REPLACE TABLE sales AS SELECT * FROM '../data/favorita/sales_small.csv';")
         con.execute("CREATE OR REPLACE TABLE train AS SELECT * FROM '../data/favorita/train_small.csv';")
 
         y = "Y"
-        x = ["htype", "locale", "locale_name", "transferred","f2","dcoilwtico","f3","transactions",
-             "f5","city","state","stype","cluster","f4","family","class","perishable","f1"]
+        x = [
+            "htype",
+            "locale",
+            "locale_name",
+            "transferred",
+            "f2",
+            "dcoilwtico",
+            "f3",
+            "transactions",
+            "f5",
+            "city",
+            "state",
+            "stype",
+            "cluster",
+            "f4",
+            "family",
+            "class",
+            "perishable",
+            "f1",
+        ]
 
         exe = DuckdbExecutor(con, debug=False)
-    
+
         dataset = JoinGraph(exe=exe)
-        dataset.add_relation("sales", [], y = 'Y')
-        dataset.add_relation("holidays", ["htype", "locale", "locale_name", "transferred","f2"])
-        dataset.add_relation("oil", ["dcoilwtico","f3"])
-        dataset.add_relation("transactions", ["transactions","f5"])
-        dataset.add_relation("stores", ["city","state","stype","cluster","f4"])
-        dataset.add_relation("items", ["family","class","perishable","f1"])
+        dataset.add_relation("sales", [], y = 'Y', relation_address='../data/favorita/sales_small.csv')
+        dataset.add_relation("holidays", ["htype", "locale", "locale_name", "transferred","f2"], relation_address='../data/favorita/holidays.csv')
+        dataset.add_relation("oil", ["dcoilwtico","f3"], relation_address='../data/favorita/oil.csv')
+        dataset.add_relation("transactions", ["transactions","f5"], relation_address='../data/favorita/transactions.csv')
+        dataset.add_relation("stores", ["city","state","stype","cluster","f4"], relation_address='../data/favorita/stores.csv')
+        dataset.add_relation("items", ["family","class","perishable","f1"], relation_address='../data/favorita/items.csv')
         dataset.add_join("sales", "items", ["item_nbr"], ["item_nbr"])
         dataset.add_join("sales", "transactions", ["tid"], ["tid"])
         dataset.add_join("transactions", "stores", ["store_nbr"], ["store_nbr"])
         dataset.add_join("transactions", "holidays", ["date"], ["date"])
         dataset.add_join("holidays", "oil", ["date"], ["date"])
 
         depth = 3
-        reg = DecisionTree(learning_rate=1, max_leaves=2 ** depth, max_depth=depth)
+        reg = DecisionTree(learning_rate=1, max_leaves=2**depth, max_depth=depth)
 
         reg.fit(dataset)
 
-        data = pd.read_csv('../data/favorita/train_small.csv')
+        data = pd.read_csv("../data/favorita/train_small.csv")
         clf = DecisionTreeRegressor(max_depth=depth)
         clf = clf.fit(data[x], data[y])
         mse = mean_squared_error(data[y], clf.predict(data[x]))
-        self.assertTrue(abs(reg.compute_rmse('train')[0] - math.sqrt(mse)) < 1e-3)
-        
+        self.assertTrue(abs(reg.compute_rmse("train")[0] - math.sqrt(mse)) < 1e-3)
+
     def test_gradient_boosting(self):
         con = duckdb.connect(database=':memory:')
-        con.execute("CREATE OR REPLACE TABLE holidays AS SELECT * FROM '../data/favorita/holidays.csv';")
-        con.execute("CREATE OR REPLACE TABLE oil AS SELECT * FROM '../data/favorita/oil.csv';")
-        con.execute("CREATE OR REPLACE TABLE transactions AS SELECT * FROM '../data/favorita/transactions.csv';")
-        con.execute("CREATE OR REPLACE TABLE stores AS SELECT * FROM '../data/favorita/stores.csv';")
-        con.execute("CREATE OR REPLACE TABLE items AS SELECT * FROM '../data/favorita/items.csv';")
-        con.execute("CREATE OR REPLACE TABLE sales AS SELECT * FROM '../data/favorita/sales_small.csv';")
         con.execute("CREATE OR REPLACE TABLE train AS SELECT * FROM '../data/favorita/train_small.csv';")
 
         y = "Y"
-        x = ["htype", "locale", "locale_name", "transferred","f2","dcoilwtico","f3","transactions",
-             "f5","city","state","stype","cluster","f4","family","class","perishable","f1"]
+        x = [
+            "htype",
+            "locale",
+            "locale_name",
+            "transferred",
+            "f2",
+            "dcoilwtico",
+            "f3",
+            "transactions",
+            "f5",
+            "city",
+            "state",
+            "stype",
+            "cluster",
+            "f4",
+            "family",
+            "class",
+            "perishable",
+            "f1",
+        ]
 
         exe = DuckdbExecutor(con, debug=False)
         depth = 3
         iteration = 3
         dataset = JoinGraph(exe=exe)
-        dataset.add_relation("sales", [], y = 'Y')
-        dataset.add_relation("holidays", ["htype", "locale", "locale_name", "transferred","f2"])
-        dataset.add_relation("oil", ["dcoilwtico","f3"])
-        dataset.add_relation("transactions", ["transactions","f5"])
-        dataset.add_relation("stores", ["city","state","stype","cluster","f4"])
-        dataset.add_relation("items", ["family","class","perishable","f1"])
+        dataset.add_relation("sales", [], y = 'Y', relation_address='../data/favorita/sales_small.csv')
+        dataset.add_relation("holidays", ["htype", "locale", "locale_name", "transferred","f2"], relation_address='../data/favorita/holidays.csv')
+        dataset.add_relation("oil", ["dcoilwtico","f3"], relation_address='../data/favorita/oil.csv')
+        dataset.add_relation("transactions", ["transactions","f5"], relation_address='../data/favorita/transactions.csv')
+        dataset.add_relation("stores", ["city","state","stype","cluster","f4"], relation_address='../data/favorita/stores.csv')
+        dataset.add_relation("items", ["family","class","perishable","f1"], relation_address='../data/favorita/items.csv')
         dataset.add_join("sales", "items", ["item_nbr"], ["item_nbr"])
         dataset.add_join("sales", "transactions", ["tid"], ["tid"])
         dataset.add_join("transactions", "stores", ["store_nbr"], ["store_nbr"])
         dataset.add_join("transactions", "holidays", ["date"], ["date"])
         dataset.add_join("holidays", "oil", ["date"], ["date"])
 
-        reg = GradientBoosting(learning_rate=1, max_leaves=2 ** depth, max_depth=depth, iteration = iteration)
+        reg = GradientBoosting(
+            learning_rate=1, max_leaves=2**depth, max_depth=depth, iteration=iteration
+        )
 
         reg.fit(dataset)
-        reg_prediction = reg.predict(data='train', input_mode=1)
         
-        data = pd.read_csv('../data/favorita/train_small.csv')
-        clf = GradientBoostingRegressor(max_depth=depth,learning_rate=1, n_estimators=iteration)
+        dataset.set_target_relation("train")
+        reg_prediction = reg.predict(joingraph=dataset, input_mode="FULL_JOIN_JG")
+
+        data = pd.read_csv("../data/favorita/train_small.csv")
+        clf = GradientBoostingRegressor(
+            max_depth=depth, learning_rate=1, n_estimators=iteration
+        )
         clf = clf.fit(data[x], data[y])
         clf_prediction = clf.predict(data[x])
         mse = mean_squared_error(data[y], clf_prediction)
-        _reg_rmse = reg.compute_rmse('train')[0]
+        _reg_rmse = reg.compute_rmse("train")[0]
 
         self.assertTrue(abs(_reg_rmse - math.sqrt(mse)) < 1e-3)
         self.assertTrue(np.sum(np.abs(reg_prediction - clf_prediction)) < 1e-3)
-    
+
     def test_sample_syn(self):
         data = pd.read_csv("../data/synthetic/RST.csv")
         con = duckdb.connect(database=':memory:')
-        con.execute("CREATE TABLE R AS SELECT * FROM '../data/synthetic/R.csv'")
-        con.execute("CREATE TABLE S AS SELECT * FROM '../data/synthetic/S.csv'")
-        con.execute("CREATE TABLE T AS SELECT * FROM '../data/synthetic/T.csv'")
         con.execute("CREATE TABLE train AS SELECT * FROM '../data/synthetic/RST.csv'")
         x = ["A", "B", "D", "E", "F"]
         y = "H"
 
         exe = DuckdbExecutor(con, debug=False)
-    
+
         dataset = JoinGraph(exe=exe)
-        dataset.add_relation('R', ['B', 'D'], y = 'H')
-        dataset.add_relation('S', ['A', 'E'])
-        dataset.add_relation('T', ['F'])
+        dataset.add_relation('R', ['B', 'D'], y = 'H', relation_address='../data/synthetic/R.csv')
+        dataset.add_relation('S', ['A', 'E'], relation_address='../data/synthetic/S.csv')
+        dataset.add_relation('T', ['F'], relation_address='../data/synthetic/T.csv')
         dataset.add_join("R", "S", ["A"], ["A"])
         dataset.add_join("R", "T", ["B"], ["B"])
 
         depth = 2
-        reg = RandomForest(max_leaves=2 ** depth, 
-                           max_depth=depth, 
-                           subsample=0.5, 
-                           iteration = 2)
+        reg = RandomForest(
+            max_leaves=2**depth, max_depth=depth, subsample=0.5, iteration=2
+        )
 
         reg.fit(dataset)
 
         clf = DecisionTreeRegressor(max_depth=depth)
         clf = clf.fit(data[x], data[y])
         mse = mean_squared_error(data[y], clf.predict(data[x]))
         # the training data is sampled, but the accuracy should still be similar
-        print(reg.compute_rmse('train')[0])
+        print(reg.compute_rmse("train")[0])
         print(math.sqrt(mse))
-    
+
     def test_lightgbm_catigorial(self):
         R = pd.read_csv("../data/synthetic-very-small/R.csv")
-        con = duckdb.connect(database=':memory:')
+        con = duckdb.connect(database=":memory:")
         con.execute("CREATE TABLE R AS SELECT * FROM R")
         x = ["D"]
         y = "H"
 
         exe = DuckdbExecutor(con, debug=False)
 
         dataset = JoinGraph(exe=exe)
-        dataset.add_relation('R', categorical_feature=['D'], y = 'H')
+        dataset.add_relation('R', categorical_feature=['D'], y = 'H', relation_address='../data/synthetic-very-small/R.csv')
 
         iteration = 1
         depth = 1
 
-        reg = GradientBoosting(learning_rate=1, 
-                               max_depth=depth, 
-                               iteration = iteration)
+        reg = GradientBoosting(learning_rate=1, max_depth=depth, iteration=iteration)
 
         reg.fit(dataset)
 
-        clf = lightgbm.LGBMRegressor(learning_rate=1, 
-                                     max_depth=depth, 
-                                     min_child_samples=1, 
-                                     objective='RMSE', 
-                                     cat_l2=0, 
-                                     cat_smooth=0, 
-                                     deterministic=True,
-                                     max_bin=20000, 
-                                     min_data_in_bin=1, 
-                                     n_estimators=iteration, 
-                                     max_cat_threshold=10000, 
-                                     max_cat_to_onehot=1, 
-                                     min_data_per_group=1)
+        clf = lightgbm.LGBMRegressor(
+            learning_rate=1,
+            max_depth=depth,
+            min_child_samples=1,
+            objective="RMSE",
+            cat_l2=0,
+            cat_smooth=0,
+            deterministic=True,
+            max_bin=20000,
+            min_data_in_bin=1,
+            n_estimators=iteration,
+            max_cat_threshold=10000,
+            max_cat_to_onehot=1,
+            min_data_per_group=1,
+        )
 
         clf.fit(R[x], R[y], feature_name=x, categorical_feature=x)
         mse = mean_squared_error(R[y], clf.predict(R[x]))
-        
-        self.assertTrue(reg.compute_rmse('R')[0] < math.sqrt(mse))
 
-if __name__ == '__main__':
-    unittest.main()
+        self.assertTrue(reg.compute_rmse("R")[0] < math.sqrt(mse))
+
+
+if __name__ == "__main__":
+    unittest.main()
```


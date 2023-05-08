# Comparing `tmp/ai-privacy-toolkit-0.1.0.tar.gz` & `tmp/ai-privacy-toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/abigailt/Desktop/Projects/mlPrivacy Projects/ai-privacy-toolkit/dist/tmpjsdrspyf/ai-privacy-toolkit-0.1.0.tar", last modified: Mon May  2 13:12:09 2022, max compression
+gzip compressed data, was "ai-privacy-toolkit-0.2.0.tar", last modified: Mon May  8 09:54:03 2023, max compression
```

## Comparing `ai-privacy-toolkit-0.1.0.tar` & `ai-privacy-toolkit-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,53 @@
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.489664 ai-privacy-toolkit-0.1.0/
--rw-r--r--   0 abigailt   (501) staff       (20)     1088 2021-07-11 15:56:47.000000 ai-privacy-toolkit-0.1.0/LICENSE
--rw-r--r--   0 abigailt   (501) staff       (20)     2665 2022-05-02 13:12:09.489805 ai-privacy-toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 abigailt   (501) staff       (20)     2044 2022-01-12 14:58:32.000000 ai-privacy-toolkit-0.1.0/README.md
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.478495 ai-privacy-toolkit-0.1.0/ai_privacy_toolkit.egg-info/
--rw-r--r--   0 abigailt   (501) staff       (20)     2665 2022-05-02 13:12:09.000000 ai-privacy-toolkit-0.1.0/ai_privacy_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 abigailt   (501) staff       (20)      547 2022-05-02 13:12:09.000000 ai-privacy-toolkit-0.1.0/ai_privacy_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 abigailt   (501) staff       (20)        1 2022-05-02 13:12:09.000000 ai-privacy-toolkit-0.1.0/ai_privacy_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 abigailt   (501) staff       (20)        4 2022-05-02 13:12:09.000000 ai-privacy-toolkit-0.1.0/ai_privacy_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.478869 ai-privacy-toolkit-0.1.0/apt/
--rw-r--r--   0 abigailt   (501) staff       (20)      142 2022-05-02 08:46:44.000000 ai-privacy-toolkit-0.1.0/apt/__init__.py
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.481074 ai-privacy-toolkit-0.1.0/apt/anonymization/
--rw-r--r--   0 abigailt   (501) staff       (20)      911 2021-07-11 15:56:47.000000 ai-privacy-toolkit-0.1.0/apt/anonymization/__init__.py
--rw-r--r--   0 abigailt   (501) staff       (20)     9537 2022-05-02 08:46:44.000000 ai-privacy-toolkit-0.1.0/apt/anonymization/anonymizer.py
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.483008 ai-privacy-toolkit-0.1.0/apt/minimization/
--rw-r--r--   0 abigailt   (501) staff       (20)      857 2022-02-23 17:21:20.000000 ai-privacy-toolkit-0.1.0/apt/minimization/__init__.py
--rw-r--r--   0 abigailt   (501) staff       (20)    50575 2022-05-02 08:46:44.000000 ai-privacy-toolkit-0.1.0/apt/minimization/minimizer.py
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.485245 ai-privacy-toolkit-0.1.0/apt/utils/
--rw-r--r--   0 abigailt   (501) staff       (20)        0 2022-05-01 12:07:08.000000 ai-privacy-toolkit-0.1.0/apt/utils/__init__.py
--rw-r--r--   0 abigailt   (501) staff       (20)    13353 2022-05-02 08:46:44.000000 ai-privacy-toolkit-0.1.0/apt/utils/dataset_utils.py
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.486510 ai-privacy-toolkit-0.1.0/apt/utils/datasets/
--rw-r--r--   0 abigailt   (501) staff       (20)      282 2022-05-01 12:07:08.000000 ai-privacy-toolkit-0.1.0/apt/utils/datasets/__init__.py
--rw-r--r--   0 abigailt   (501) staff       (20)    13407 2022-05-02 12:36:38.000000 ai-privacy-toolkit-0.1.0/apt/utils/datasets/datasets.py
-drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2022-05-02 13:12:09.489030 ai-privacy-toolkit-0.1.0/apt/utils/models/
--rw-r--r--   0 abigailt   (501) staff       (20)      151 2022-05-01 12:07:08.000000 ai-privacy-toolkit-0.1.0/apt/utils/models/__init__.py
--rw-r--r--   0 abigailt   (501) staff       (20)     3954 2022-05-02 08:46:44.000000 ai-privacy-toolkit-0.1.0/apt/utils/models/model.py
--rw-r--r--   0 abigailt   (501) staff       (20)     5043 2022-05-02 08:46:44.000000 ai-privacy-toolkit-0.1.0/apt/utils/models/sklearn_model.py
--rw-r--r--   0 abigailt   (501) staff       (20)      103 2021-04-28 12:42:22.000000 ai-privacy-toolkit-0.1.0/pyproject.toml
--rw-r--r--   0 abigailt   (501) staff       (20)      693 2022-05-02 13:12:09.490526 ai-privacy-toolkit-0.1.0/setup.cfg
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.806525 ai-privacy-toolkit-0.2.0/
+-rw-r--r--   0 abigailt   (501) staff       (20)     1088 2021-07-11 15:56:47.000000 ai-privacy-toolkit-0.2.0/LICENSE
+-rw-r--r--   0 abigailt   (501) staff       (20)     3186 2023-05-08 09:54:03.806610 ai-privacy-toolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 abigailt   (501) staff       (20)     2601 2023-05-04 09:26:58.000000 ai-privacy-toolkit-0.2.0/README.md
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.799384 ai-privacy-toolkit-0.2.0/ai_privacy_toolkit.egg-info/
+-rw-r--r--   0 abigailt   (501) staff       (20)     3186 2023-05-08 09:54:03.000000 ai-privacy-toolkit-0.2.0/ai_privacy_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 abigailt   (501) staff       (20)     1295 2023-05-08 09:54:03.000000 ai-privacy-toolkit-0.2.0/ai_privacy_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 abigailt   (501) staff       (20)        1 2023-05-08 09:54:03.000000 ai-privacy-toolkit-0.2.0/ai_privacy_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 abigailt   (501) staff       (20)        4 2023-05-08 09:54:03.000000 ai-privacy-toolkit-0.2.0/ai_privacy_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.799522 ai-privacy-toolkit-0.2.0/apt/
+-rw-r--r--   0 abigailt   (501) staff       (20)      143 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/__init__.py
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.799939 ai-privacy-toolkit-0.2.0/apt/anonymization/
+-rw-r--r--   0 abigailt   (501) staff       (20)      911 2021-07-11 15:56:47.000000 ai-privacy-toolkit-0.2.0/apt/anonymization/__init__.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     9546 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/apt/anonymization/anonymizer.py
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.800350 ai-privacy-toolkit-0.2.0/apt/minimization/
+-rw-r--r--   0 abigailt   (501) staff       (20)      857 2022-02-23 17:21:20.000000 ai-privacy-toolkit-0.2.0/apt/minimization/__init__.py
+-rw-r--r--   0 abigailt   (501) staff       (20)    50612 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/apt/minimization/minimizer.py
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.800544 ai-privacy-toolkit-0.2.0/apt/risk/
+-rw-r--r--   0 abigailt   (501) staff       (20)        1 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/risk/__init__.py
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.802050 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/
+-rw-r--r--   0 abigailt   (501) staff       (20)      725 2023-04-23 10:55:07.000000 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/__init__.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     3201 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/attack_strategy_utils.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     4388 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/dataset_assessment_manager.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     5082 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/dataset_attack.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     9218 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/dataset_attack_membership_knn_probabilities.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     1000 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/dataset_attack_result.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     6997 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/risk/data_assessment/dataset_attack_whole_dataset_knn_distance.py
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.802354 ai-privacy-toolkit-0.2.0/apt/utils/
+-rw-r--r--   0 abigailt   (501) staff       (20)        0 2022-05-01 12:07:08.000000 ai-privacy-toolkit-0.2.0/apt/utils/__init__.py
+-rw-r--r--   0 abigailt   (501) staff       (20)    13151 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/apt/utils/dataset_utils.py
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.802789 ai-privacy-toolkit-0.2.0/apt/utils/datasets/
+-rw-r--r--   0 abigailt   (501) staff       (20)      306 2022-07-12 06:23:17.000000 ai-privacy-toolkit-0.2.0/apt/utils/datasets/__init__.py
+-rw-r--r--   0 abigailt   (501) staff       (20)    16598 2022-08-11 15:27:18.000000 ai-privacy-toolkit-0.2.0/apt/utils/datasets/datasets.py
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.804190 ai-privacy-toolkit-0.2.0/apt/utils/models/
+-rw-r--r--   0 abigailt   (501) staff       (20)      454 2022-08-11 15:27:18.000000 ai-privacy-toolkit-0.2.0/apt/utils/models/__init__.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     6653 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/utils/models/keras_model.py
+-rw-r--r--   0 abigailt   (501) staff       (20)    17670 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/apt/utils/models/model.py
+-rw-r--r--   0 abigailt   (501) staff       (20)    17713 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/utils/models/pytorch_model.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     5388 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/apt/utils/models/sklearn_model.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     3877 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/apt/utils/models/xgboost_model.py
+-rw-r--r--   0 abigailt   (501) staff       (20)      103 2021-04-28 12:42:22.000000 ai-privacy-toolkit-0.2.0/pyproject.toml
+-rw-r--r--   0 abigailt   (501) staff       (20)      758 2023-05-08 09:54:03.806957 ai-privacy-toolkit-0.2.0/setup.cfg
+drwxr-xr-x   0 abigailt   (501) staff       (20)        0 2023-05-08 09:54:03.806407 ai-privacy-toolkit-0.2.0/tests/
+-rw-r--r--   0 abigailt   (501) staff       (20)     5601 2021-12-22 13:45:20.000000 ai-privacy-toolkit-0.2.0/tests/testJupyter.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     5524 2021-12-22 14:19:35.000000 ai-privacy-toolkit-0.2.0/tests/testJupyter2.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     2359 2021-12-27 11:57:59.000000 ai-privacy-toolkit-0.2.0/tests/testJupyter3.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     5819 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/tests/test_anonymizer.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     7371 2023-04-23 10:55:07.000000 ai-privacy-toolkit-0.2.0/tests/test_data_assessment.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     4860 2023-04-23 10:55:07.000000 ai-privacy-toolkit-0.2.0/tests/test_data_assessment_short_test.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     1167 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/tests/test_datasets.py
+-rw-r--r--   0 abigailt   (501) staff       (20)    52095 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/tests/test_minimizer.py
+-rw-r--r--   0 abigailt   (501) staff       (20)    10798 2023-05-08 09:51:19.000000 ai-privacy-toolkit-0.2.0/tests/test_model.py
+-rw-r--r--   0 abigailt   (501) staff       (20)     3439 2022-12-25 13:14:22.000000 ai-privacy-toolkit-0.2.0/tests/test_pytorch.py
```

### Comparing `ai-privacy-toolkit-0.1.0/LICENSE` & `ai-privacy-toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-privacy-toolkit-0.1.0/PKG-INFO` & `ai-privacy-toolkit-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: ai-privacy-toolkit
-Version: 0.1.0
-Summary: A toolkit for tools and techniques related to the privacy and compliance of AI models.
-Home-page: https://github.com/IBM/ai-privacy-toolkit
-Author: Abigail Goldsteen
-Author-email: abigailt@il.ibm.com
-License: UNKNOWN
-Project-URL: Documentation, https://ai-privacy-toolkit.readthedocs.io/en/latest/
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ai-privacy-toolkit
 <p align="center">
   <img src="docs/images/logo with text.jpg?raw=true" width="467" title="ai-privacy-toolkit logo">
 </p>
 <br />
 
 A toolkit for tools and techniques related to the privacy and compliance of AI models.
@@ -29,29 +12,37 @@
 set out in data protection regulations such as GDPR, CCPA, etc. 
 
 The [**minimization**](apt/minimization/README.md) module contains methods to help adhere to the data 
 minimization principle in GDPR for ML models. It enables to reduce the amount of 
 personal data needed to perform predictions with a machine learning model, while still enabling the model
 to make accurate predictions. This is done by by removing or generalizing some of the input features.
 
+The [**dataset assessment**](apt/risk/data_assessment/README.md) module implements a tool for privacy assessment of
+synthetic datasets that are to be used in AI model training.
+
 Official ai-privacy-toolkit documentation: https://ai-privacy-toolkit.readthedocs.io/en/latest/
 
 Installation: pip install ai-privacy-toolkit
 
 For more information or help using or improving the toolkit, please contact Abigail Goldsteen at abigailt@il.ibm.com, 
 or join our Slack channel: https://aip360.mybluemix.net/community.
 
+We welcome new contributors! If you're interested, take a look at our [**contribution guidelines**](https://github.com/IBM/ai-privacy-toolkit/wiki/Contributing).
+
 **Related toolkits:**
 
 ai-minimization-toolkit - has been migrated into this toolkit.
 
 [differential-privacy-library](https://github.com/IBM/differential-privacy-library): A 
 general-purpose library for experimenting with, investigating and developing applications in, 
 differential privacy.
 
 [adversarial-robustness-toolbox](https://github.com/Trusted-AI/adversarial-robustness-toolbox):
 A Python library for Machine Learning Security. Includes an attack module called *inference* that contains privacy attacks on ML models 
 (membership inference, attribute inference, model inversion and database reconstruction) as well as a *privacy* metrics module that contains
 membership leakage metrics for ML models.
 
 
-
+Citation
+--------
+Abigail Goldsteen, Ola Saadi, Ron Shmelkin, Shlomit Shachor, Natalia Razinkov,
+"AI privacy toolkit", SoftwareX, Volume 22, 2023, 101352, ISSN 2352-7110, https://doi.org/10.1016/j.softx.2023.101352.
```

### Comparing `ai-privacy-toolkit-0.1.0/apt/anonymization/__init__.py` & `ai-privacy-toolkit-0.2.0/apt/anonymization/__init__.py`

 * *Files identical despite different names*

### Comparing `ai-privacy-toolkit-0.1.0/apt/anonymization/anonymizer.py` & `ai-privacy-toolkit-0.2.0/apt/anonymization/anonymizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         if dataset.get_samples().shape[1] != 0:
             self.features = [i for i in range(dataset.get_samples().shape[1])]
         else:
             raise ValueError('No data provided')
 
         if dataset.features_names is not None:
             self.features_names = dataset.features_names
-        else: # if no names provided, use numbers instead
+        else:  # if no names provided, use numbers instead
             self.features_names = self.features
 
         if not set(self.quasi_identifiers).issubset(set(self.features_names)):
             raise ValueError('Quasi identifiers should bs a subset of the supplied features or indexes in range of '
                              'the data columns')
         if self.categorical_features and not set(self.categorical_features).issubset(set(self.features_names)):
             raise ValueError('Categorical features should bs a subset of the supplied features or indexes in range of '
@@ -97,36 +97,36 @@
         else:
             x_prepared = x
         x_anonymizer_train = x_prepared
         if self.train_only_QI:
             # build DT just on QI features
             x_anonymizer_train = x_prepared[:, self.quasi_identifiers]
         if self.is_regression:
-            self.anonymizer = DecisionTreeRegressor(random_state=10, min_samples_split=2, min_samples_leaf=self.k)
+            self._anonymizer = DecisionTreeRegressor(random_state=10, min_samples_split=2, min_samples_leaf=self.k)
         else:
-            self.anonymizer = DecisionTreeClassifier(random_state=10, min_samples_split=2, min_samples_leaf=self.k)
+            self._anonymizer = DecisionTreeClassifier(random_state=10, min_samples_split=2, min_samples_leaf=self.k)
 
-        self.anonymizer.fit(x_anonymizer_train, y)
+        self._anonymizer.fit(x_anonymizer_train, y)
         cells_by_id = self._calculate_cells(x, x_anonymizer_train)
         return self._anonymize_data(x, x_anonymizer_train, cells_by_id)
 
     def _calculate_cells(self, x, x_anonymizer_train):
         # x is original data, x_anonymizer_train is only QIs + 1-hot encoded
         cells_by_id = {}
         leaves = []
-        for node, feature in enumerate(self.anonymizer.tree_.feature):
+        for node, feature in enumerate(self._anonymizer.tree_.feature):
             if feature == -2:  # leaf node
                 leaves.append(node)
-                hist = [int(i) for i in self.anonymizer.tree_.value[node][0]]
+                hist = [int(i) for i in self._anonymizer.tree_.value[node][0]]
                 # TODO we may change the method for choosing representative for cell
                 # label_hist = self.anonymizer.tree_.value[node][0]
                 # label = int(self.anonymizer.classes_[np.argmax(label_hist)])
                 cell = {'label': 1, 'hist': hist, 'id': int(node)}
                 cells_by_id[cell['id']] = cell
-        self.nodes = leaves
+        self._nodes = leaves
         self._find_representatives(x, x_anonymizer_train, cells_by_id.values())
         return cells_by_id
 
     def _find_representatives(self, x, x_anonymizer_train, cells):
         # x is original data, x_anonymizer_train is only QIs + 1-hot encoded
         node_ids = self._find_sample_nodes(x_anonymizer_train)
         for cell in cells:
@@ -149,16 +149,16 @@
                         dist = distance.euclidean(value, median)
                         if dist < min_dist:
                             min_dist = dist
                             min_value = value
                     cell['representative'][feature] = min_value
 
     def _find_sample_nodes(self, samples):
-        paths = self.anonymizer.decision_path(samples).toarray()
-        node_set = set(self.nodes)
+        paths = self._anonymizer.decision_path(samples).toarray()
+        node_set = set(self._nodes)
         return [(list(set([i for i, v in enumerate(p) if v == 1]) & node_set))[0] for p in paths]
 
     def _find_sample_cells(self, samples, cells_by_id):
         node_ids = self._find_sample_nodes(samples)
         return [cells_by_id[node_id] for node_id in node_ids]
 
     def _anonymize_data(self, x, x_anonymizer_train, cells_by_id):
```

### Comparing `ai-privacy-toolkit-0.1.0/apt/minimization/__init__.py` & `ai-privacy-toolkit-0.2.0/apt/minimization/__init__.py`

 * *Files identical despite different names*

### Comparing `ai-privacy-toolkit-0.1.0/apt/minimization/minimizer.py` & `ai-privacy-toolkit-0.2.0/apt/minimization/minimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import copy
 import sys
 from scipy.spatial import distance
 from sklearn.base import BaseEstimator, TransformerMixin, MetaEstimatorMixin
 from sklearn.compose import ColumnTransformer
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
-from sklearn.preprocessing import OneHotEncoder
-from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
+from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder
+from sklearn.utils.validation import check_is_fitted
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.model_selection import train_test_split
 
-from apt.utils.datasets import ArrayDataset, Data, DATA_PANDAS_NUMPY_TYPE
+from apt.utils.datasets import ArrayDataset, DATA_PANDAS_NUMPY_TYPE
 from apt.utils.models import Model, SklearnRegressor, ModelOutputType, SklearnClassifier
 
 
 class GeneralizeToRepresentative(BaseEstimator, MetaEstimatorMixin, TransformerMixin):
     """
     A transformer that generalizes data to representative points.
 
@@ -43,59 +43,70 @@
     :type target_accuracy: float, optional
     :param cells: The cells used to generalize records. Each cell must define a range or subset of categories for
                   each feature, as well as a representative value for each feature. This parameter should be used
                   when instantiating a transformer object without first fitting it.
     :type cells: list of objects, optional
     :param categorical_features: The list of categorical features (if supplied, these featurtes will be one-hot
                                  encoded before using them to train the decision tree model).
+    :param encoder: Optional encoder for encoding data before feeding it into the estimator (e.g., for categorical
+                    features)
+    :type encoder: sklearn OrdinalEncoder or OneHotEncoder
     :type categorical_features: list of strings, optional
     :param features_to_minimize: The features to be minimized.
     :type features_to_minimize: list of strings or int, optional
-    :param train_only_QI: Whether to train the tree just on the ``features_to_minimize`` or on all features. Default
-                          is only on ``features_to_minimize``.
-    :type train_only_QI: boolean, optional
+    :param train_only_features_to_minimize: Whether to train the tree just on the ``features_to_minimize`` or on all
+                                            features. Default is only on ``features_to_minimize``.
+    :type train_only_features_to_minimize: boolean, optional
     :param is_regression: Whether the model is a regression model or not (if False, assumes a classification model).
                           Default is False.
     :type is_regression: boolean, optional
     """
 
     def __init__(self, estimator: Union[BaseEstimator, Model] = None, target_accuracy: Optional[float] = 0.998,
                  cells: Optional[list] = None, categorical_features: Optional[Union[np.ndarray, list]] = None,
-                 features_to_minimize: Optional[Union[np.ndarray, list]] = None, train_only_QI: Optional[bool] = True,
+                 encoder: Optional[Union[OrdinalEncoder, OneHotEncoder]] = None,
+                 features_to_minimize: Optional[Union[np.ndarray, list]] = None,
+                 train_only_features_to_minimize: Optional[bool] = True,
                  is_regression: Optional[bool] = False):
-        if issubclass(estimator.__class__, Model):
-            self.estimator = estimator
-        else:
+
+        self.estimator = estimator
+        if estimator is not None and not issubclass(estimator.__class__, Model):
             if is_regression:
                 self.estimator = SklearnRegressor(estimator)
             else:
-                self.estimator = SklearnClassifier(estimator, ModelOutputType.CLASSIFIER_VECTOR)
+                self.estimator = SklearnClassifier(estimator, ModelOutputType.CLASSIFIER_PROBABILITIES)
         self.target_accuracy = target_accuracy
         self.cells = cells
         self.categorical_features = []
         if categorical_features:
             self.categorical_features = categorical_features
         self.features_to_minimize = features_to_minimize
-        self.train_only_QI = train_only_QI
+        self.train_only_features_to_minimize = train_only_features_to_minimize
         self.is_regression = is_regression
+        self.encoder = encoder
 
     def get_params(self, deep=True):
         """
         Get parameters
 
         :param deep: If True, will return the parameters for this estimator and contained
                      sub-objects that are estimators.
         :type deep: boolean, optional
         :return: Parameter names mapped to their values
         """
         ret = {}
         ret['target_accuracy'] = self.target_accuracy
+        ret['categorical_features'] = self.categorical_features
+        ret['features_to_minimize'] = self.features_to_minimize
+        ret['train_only_features_to_minimize'] = self.train_only_features_to_minimize
+        ret['is_regression'] = self.is_regression
         if deep:
             ret['cells'] = copy.deepcopy(self.cells)
             ret['estimator'] = self.estimator
+            ret['encoder'] = self.encoder
         else:
             ret['cells'] = copy.copy(self.cells)
         return ret
 
     def set_params(self, **params):
         """
         Set parameters
@@ -107,28 +118,45 @@
                       each feature, as well as a representative value for each feature. This parameter should be used
                       when instantiating a transformer object without first fitting it.
         :type cells: list of objects, optional
         :return: self
         """
         if 'target_accuracy' in params:
             self.target_accuracy = params['target_accuracy']
+        if 'categorical_features' in params:
+            self.categorical_features = params['categorical_features']
+        if 'features_to_minimize' in params:
+            self.features_to_minimize = params['features_to_minimize']
+        if 'train_only_features_to_minimize' in params:
+            self.train_only_features_to_minimize = params['train_only_features_to_minimize']
+        if 'is_regression' in params:
+            self.is_regression = params['is_regression']
         if 'cells' in params:
             self.cells = params['cells']
         return self
 
     @property
     def generalizations(self):
         """
         Return the generalizations derived from the model and test data.
 
         :return: generalizations object. Contains 3 sections: 'ranges' that contains ranges for numerical features,
                                  'categories' that contains sub-groups of categories for categorical features, and
                                  'untouched' that contains the features that could not be generalized.
         """
-        return self.generalizations_
+        return self._generalizations
+
+    @property
+    def ncp(self):
+        """
+        Return the NCP score of the generalizations.
+
+        :return: ncp score as float.
+        """
+        return self._ncp
 
     def fit_transform(self, X: Optional[DATA_PANDAS_NUMPY_TYPE] = None, y: Optional[DATA_PANDAS_NUMPY_TYPE] = None,
                       features_names: Optional[list] = None, dataset: Optional[ArrayDataset] = None):
         """
         Learns the generalizations based on training data, and applies them to the data.
 
         :param X: The training input samples.
@@ -168,202 +196,178 @@
         if X is not None and y is not None:
             if dataset is not None:
                 raise ValueError('Either X,y OR dataset need to be provided, not both')
             else:
                 dataset = ArrayDataset(X, y, features_names)
 
         if dataset and dataset.get_samples() is not None and dataset.get_labels() is not None:
-            self.n_features_ = dataset.get_samples().shape[1]
-
+            self._n_features = dataset.get_samples().shape[1]
         elif dataset and dataset.features_names:
-            self.n_features_ = len(dataset.features_names)
+            self._n_features = len(dataset.features_names)
         else:
-            self.n_features_ = 0
+            self._n_features = 0
 
         if dataset and dataset.features_names:
             self._features = dataset.features_names
         # if features is None, use numbers instead of names
-        elif self.n_features_ != 0:
-            self._features = [str(i) for i in range(self.n_features_)]
+        elif self._n_features != 0:
+            self._features = [str(i) for i in range(self._n_features)]
         else:
             self._features = None
 
-        if self.cells:
-            self.cells_ = self.cells
-        else:
-            self.cells_ = {}
-        self.categorical_values = {}
-
         # Going to fit
         # (currently not dealing with option to fit with only X and y and no estimator)
         if self.estimator and dataset and dataset.get_samples() is not None and dataset.get_labels() is not None:
             x = pd.DataFrame(dataset.get_samples(), columns=self._features)
             if not self.features_to_minimize:
                 self.features_to_minimize = self._features
             self.features_to_minimize = [str(i) for i in self.features_to_minimize]
             if not all(elem in self._features for elem in self.features_to_minimize):
                 raise ValueError('features to minimize should be a subset of features names')
             x_QI = x.loc[:, self.features_to_minimize]
 
             # divide dataset into train and test
             used_data = x
-            if self.train_only_QI:
+            if self.train_only_features_to_minimize:
                 used_data = x_QI
             if self.is_regression:
-                X_train, X_test, y_train, y_test = train_test_split(x, dataset.get_labels(), test_size=0.4, random_state=14)
+                X_train, X_test, y_train, y_test = train_test_split(x, dataset.get_labels(), test_size=0.4,
+                                                                    random_state=14)
             else:
-                X_train, X_test, y_train, y_test = train_test_split(x, dataset.get_labels(), stratify=dataset.get_labels(), test_size=0.4,
-                                                                    random_state=18)
+                try:
+                    X_train, X_test, y_train, y_test = train_test_split(x, dataset.get_labels(),
+                                                                        stratify=dataset.get_labels(), test_size=0.4,
+                                                                        random_state=18)
+                except ValueError:
+                    print('Could not stratify split due to uncommon class value, doing unstratified split instead')
+                    X_train, X_test, y_train, y_test = train_test_split(x, dataset.get_labels(), test_size=0.4,
+                                                                        random_state=18)
 
             X_train_QI = X_train.loc[:, self.features_to_minimize]
             X_test_QI = X_test.loc[:, self.features_to_minimize]
             used_X_train = X_train
-            if self.train_only_QI:
+            used_X_test = X_test
+            if self.train_only_features_to_minimize:
                 used_X_train = X_train_QI
+                used_X_test = X_test_QI
 
             # collect feature data (such as min, max)
             feature_data = {}
             for feature in self._features:
                 if feature not in feature_data.keys():
                     fd = {}
                     values = list(x.loc[:, feature])
                     if feature not in self.categorical_features:
                         fd['min'] = min(values)
                         fd['max'] = max(values)
                         fd['range'] = max(values) - min(values)
                     else:
-                        fd['range'] = len(values)
+                        fd['range'] = len(np.unique(values))
                     feature_data[feature] = fd
 
-            # prepare data for DT
-            categorical_features = [f for f in self._features if f in self.categorical_features and
-                                    f in self.features_to_minimize]
-
-            numeric_transformer = Pipeline(
-                steps=[('imputer', SimpleImputer(strategy='constant', fill_value=0))]
-            )
-
-            numeric_features = [f for f in self._features if f not in self.categorical_features and
-                                f in self.features_to_minimize]
-            categorical_transformer = OneHotEncoder(handle_unknown="ignore", sparse=False)
-
-            preprocessor_QI_features = ColumnTransformer(
-                transformers=[
-                    ("num", numeric_transformer, numeric_features),
-                    ("cat", categorical_transformer, categorical_features),
-                ]
-            )
-            preprocessor_QI_features.fit(x_QI)
-
-            # preprocessor to fit data that have features not included in QI (to get accuracy)
-            numeric_features = [f for f in self._features if f not in self.categorical_features]
-            numeric_transformer = Pipeline(
-                steps=[('imputer', SimpleImputer(strategy='constant', fill_value=0))]
-            )
-            categorical_transformer = OneHotEncoder(handle_unknown="ignore", sparse=False)
-            preprocessor = ColumnTransformer(
-                transformers=[
-                    ("num", numeric_transformer, numeric_features),
-                    ("cat", categorical_transformer, self.categorical_features),
-                ]
-            )
-            preprocessor.fit(x)
-            x_prepared = preprocessor.transform(X_train)
-            if self.train_only_QI:
-                x_prepared = preprocessor_QI_features.transform(X_train_QI)
+            # default encoder in case none provided
+            if self.encoder is None:
+                numeric_features = [f for f in self._features if f not in self.categorical_features]
+                numeric_transformer = Pipeline(
+                    steps=[('imputer', SimpleImputer(strategy='constant', fill_value=0))]
+                )
+                categorical_transformer = OneHotEncoder(handle_unknown="ignore", sparse=False)
+                self.encoder = ColumnTransformer(
+                    transformers=[
+                        ("num", numeric_transformer, numeric_features),
+                        ("cat", categorical_transformer, self.categorical_features),
+                    ]
+                )
+                self.encoder.fit(x)
 
-            self._preprocessor = preprocessor
+            self.cells = []
+            self._categorical_values = {}
 
-            self.cells_ = {}
             if self.is_regression:
-                self.dt_ = DecisionTreeRegressor(random_state=10, min_samples_split=2, min_samples_leaf=1)
+                self._dt = DecisionTreeRegressor(random_state=10, min_samples_split=2, min_samples_leaf=1)
             else:
-                self.dt_ = DecisionTreeClassifier(random_state=0, min_samples_split=2,
+                self._dt = DecisionTreeClassifier(random_state=0, min_samples_split=2,
                                                   min_samples_leaf=1)
-            self.dt_.fit(x_prepared, y_train)
-            self._modify_categorical_features(used_data)
 
-            x_prepared = pd.DataFrame(x_prepared, columns=self.categorical_data.columns)
+            # prepare data for DT
+            self._encode_categorical_features(used_data, save_mapping=True)
+            x_prepared = self._encode_categorical_features(used_X_train)
+            self._dt.fit(x_prepared, y_train)
+            x_prepared_test = self._encode_categorical_features(used_X_test)
 
             self._calculate_cells()
             self._modify_cells()
             # features that are not from QI should not be part of generalizations
             for feature in self._features:
                 if feature not in self.features_to_minimize:
-                    self._remove_feature_from_cells(self.cells_, self.cells_by_id_, feature)
+                    self._remove_feature_from_cells(self.cells, self._cells_by_id, feature)
 
             nodes = self._get_nodes_level(0)
             self._attach_cells_representatives(x_prepared, used_X_train, y_train, nodes)
 
-            # self.cells_ currently holds the generalization created from the tree leaves
+            # self._cells currently holds the generalization created from the tree leaves
             self._calculate_generalizations()
-
-            # apply generalizations to test data
-            x_prepared_test = preprocessor.transform(X_test)
-            if self.train_only_QI:
-                x_prepared_test = preprocessor_QI_features.transform(X_test_QI)
-
-            x_prepared_test = pd.DataFrame(x_prepared_test, index=X_test.index, columns=self.categorical_data.columns)
-
-            generalized = self._generalize(X_test, x_prepared_test, nodes, self.cells_, self.cells_by_id_)
+            generalized = self._generalize(X_test, x_prepared_test, nodes, self.cells, self._cells_by_id)
 
             # check accuracy
-            accuracy = self.estimator.score(ArrayDataset(preprocessor.transform(generalized), y_test))
+            accuracy = self.estimator.score(ArrayDataset(self.encoder.transform(generalized), y_test))
             print('Initial accuracy of model on generalized data, relative to original model predictions '
                   '(base generalization derived from tree, before improvements): %f' % accuracy)
 
             # if accuracy above threshold, improve generalization
             if accuracy > self.target_accuracy:
                 print('Improving generalizations')
                 level = 1
                 while accuracy > self.target_accuracy:
+                    cells_previous_iter = self.cells
+                    generalization_prev_iter = self._generalizations
+                    cells_by_id_prev = self._cells_by_id
+                    nodes = self._get_nodes_level(level)
+
                     try:
-                        cells_previous_iter = self.cells_
-                        generalization_prev_iter = self.generalizations_
-                        cells_by_id_prev = self.cells_by_id_
-                        nodes = self._get_nodes_level(level)
                         self._calculate_level_cells(level)
-                        self._attach_cells_representatives(x_prepared, used_X_train, y_train, nodes)
-
-                        self._calculate_generalizations()
-                        generalized = self._generalize(X_test, x_prepared_test, nodes, self.cells_,
-                                                       self.cells_by_id_)
-                        accuracy = self.estimator.score(ArrayDataset(preprocessor.transform(generalized), y_test))
-                        # if accuracy passed threshold roll back to previous iteration generalizations
-                        if accuracy < self.target_accuracy:
-                            self.cells_ = cells_previous_iter
-                            self.generalizations_ = generalization_prev_iter
-                            self.cells_by_id_ = cells_by_id_prev
-                            break
-                        else:
-                            print('Pruned tree to level: %d, new relative accuracy: %f' % (level, accuracy))
-                            level += 1
-                    except Exception as e:
+                    except TypeError as e:
                         print(e)
                         break
 
+                    self._attach_cells_representatives(x_prepared, used_X_train, y_train, nodes)
+
+                    self._calculate_generalizations()
+                    generalized = self._generalize(X_test, x_prepared_test, nodes, self.cells,
+                                                   self._cells_by_id)
+                    accuracy = self.estimator.score(ArrayDataset(self.encoder.transform(generalized), y_test))
+                    # if accuracy passed threshold roll back to previous iteration generalizations
+                    if accuracy < self.target_accuracy:
+                        self.cells = cells_previous_iter
+                        self._generalizations = generalization_prev_iter
+                        self._cells_by_id = cells_by_id_prev
+                        break
+                    else:
+                        print('Pruned tree to level: %d, new relative accuracy: %f' % (level, accuracy))
+                        level += 1
+
             # if accuracy below threshold, improve accuracy by removing features from generalization
             elif accuracy < self.target_accuracy:
                 print('Improving accuracy')
                 while accuracy < self.target_accuracy:
                     removed_feature = self._remove_feature_from_generalization(X_test, x_prepared_test,
                                                                                nodes, y_test,
                                                                                feature_data, accuracy)
                     if removed_feature is None:
                         break
 
                     self._calculate_generalizations()
-                    generalized = self._generalize(X_test, x_prepared_test, nodes, self.cells_, self.cells_by_id_)
-                    accuracy = self.estimator.score(ArrayDataset(preprocessor.transform(generalized), y_test))
+                    generalized = self._generalize(X_test, x_prepared_test, nodes, self.cells, self._cells_by_id)
+                    accuracy = self.estimator.score(ArrayDataset(self.encoder.transform(generalized), y_test))
                     print('Removed feature: %s, new relative accuracy: %f' % (removed_feature, accuracy))
 
-            # self.cells_ currently holds the chosen generalization based on target accuracy
+            # self._cells currently holds the chosen generalization based on target accuracy
 
             # calculate iLoss
-            self.ncp_ = self._calculate_ncp(X_test, self.generalizations_, feature_data)
+            self._ncp = self._calculate_ncp(X_test, self._generalizations, feature_data)
 
         # Return the transformer
         return self
 
     def transform(self, X: Optional[DATA_PANDAS_NUMPY_TYPE] = None, features_names: Optional[list] = None,
                   dataset: Optional[ArrayDataset] = None):
         """ Transforms data records to representative points.
@@ -394,53 +398,28 @@
         elif dataset is None:
             raise ValueError('Either X OR dataset need to be provided, not both')
         if dataset and dataset.features_names:
             self._features = dataset.features_names
         if dataset and dataset.get_samples() is not None:
             x = pd.DataFrame(dataset.get_samples(), columns=self._features)
 
-        if x.shape[1] != self.n_features_ and self.n_features_ != 0:
+        if x.shape[1] != self._n_features and self._n_features != 0:
             raise ValueError('Shape of input is different from what was seen'
                              'in `fit`')
 
         if not self._features:
             self._features = [i for i in range(x.shape[1])]
 
-        representatives = pd.DataFrame(columns=self._features)  # only columns
-        generalized = pd.DataFrame(x, columns=self._features, copy=True)  # original data
         mapped = np.zeros(x.shape[0])  # to mark records we already mapped
+        all_indexes = []
+        for i in range(len(self.cells)):
+            indexes = self._get_record_indexes_for_cell(x, self.cells[i], mapped)
+            all_indexes.append(indexes)
+        generalized = self._generalize_indexes(x, self.cells, all_indexes)
 
-        # iterate over cells (leaves in decision tree)
-        for i in range(len(self.cells_)):
-            # Copy the representatives from the cells into another data structure:
-            # iterate over features in test data
-            for feature in self._features:
-                # if feature has a representative value in the cell and should not
-                # be left untouched, take the representative value
-                if feature in self.cells_[i]['representative'] and \
-                        ('untouched' not in self.cells_[i]
-                         or feature not in self.cells_[i]['untouched']):
-                    representatives.loc[i, feature] = self.cells_[i]['representative'][feature]
-                # else, drop the feature (removes from representatives columns that
-                # do not have a representative value or should remain untouched)
-                elif feature in representatives.columns.tolist():
-                    representatives = representatives.drop(feature, axis=1)
-
-            # get the indexes of all records that map to this cell
-            indexes = self._get_record_indexes_for_cell(x, self.cells_[i], mapped)
-
-            # replace the values in the representative columns with the representative
-            # values (leaves others untouched)
-            if indexes and not representatives.columns.empty:
-                if len(indexes) > 1:
-                    replace = pd.concat([representatives.loc[i].to_frame().T] * len(indexes)).reset_index(drop=True)
-                else:
-                    replace = representatives.loc[i].to_frame().T.reset_index(drop=True)
-                replace.index = indexes
-                generalized.loc[indexes, representatives.columns] = replace
         if dataset and dataset.is_pandas:
             return generalized
         elif isinstance(X, pd.DataFrame):
             return generalized
         return generalized.to_numpy()
 
     def _get_record_indexes_for_cell(self, X, cell, mapped):
@@ -462,37 +441,44 @@
                 continue
             else:
                 raise TypeError("feature " + f + "not found in cell" + cell['id'])
         # Mark as mapped
         mapped.itemset(i, 1)
         return True
 
-    def _modify_categorical_features(self, X):
-        self.categorical_values = {}
-        self.oneHotVectorFeaturesToFeatures = {}
+    def _encode_categorical_features(self, X, save_mapping=False):
+        if save_mapping:
+            self._categorical_values = {}
+            self._one_hot_vector_features_to_features = {}
         features_to_remove = []
         used_features = self._features
-        if self.train_only_QI:
+        if self.train_only_features_to_minimize:
             used_features = self.features_to_minimize
         for feature in self.categorical_features:
             if feature in used_features:
                 try:
                     all_values = X.loc[:, feature]
                     values = list(all_values.unique())
-                    self.categorical_values[feature] = values
-                    X[feature] = pd.Categorical(X.loc[:, feature], categories=values, ordered=False)
+                    if save_mapping:
+                        self._categorical_values[feature] = values
+                    X[feature] = pd.Categorical(X.loc[:, feature], categories=self._categorical_values[feature],
+                                                ordered=False)
                     ohe = pd.get_dummies(X[feature], prefix=feature)
-                    for oneHotVectorFeature in ohe.columns:
-                        self.oneHotVectorFeaturesToFeatures[oneHotVectorFeature] = feature
+                    if save_mapping:
+                        for one_hot_vector_feature in ohe.columns:
+                            self._one_hot_vector_features_to_features[one_hot_vector_feature] = feature
                     X = pd.concat([X, ohe], axis=1)
                     features_to_remove.append(feature)
                 except KeyError:
                     print("feature " + feature + "not found in training data")
 
-        self.categorical_data = X.drop(features_to_remove, axis=1)
+        new_data = X.drop(features_to_remove, axis=1)
+        if save_mapping:
+            self._encoded_features = new_data.columns
+        return new_data
 
     def _cell_contains_numeric(self, f, range, x):
         i = self._features.index(f)
         # convert x to ndarray to allow indexing
         a = np.array(x)
         value = a.item(i)
         if range['start']:
@@ -509,69 +495,69 @@
         a = np.array(x)
         value = a.item(i)
         if value in range:
             return True
         return False
 
     def _calculate_cells(self):
-        self.cells_by_id_ = {}
-        self.cells_ = self._calculate_cells_recursive(0)
+        self._cells_by_id = {}
+        self.cells = self._calculate_cells_recursive(0)
 
     def _calculate_cells_recursive(self, node):
-        feature_index = self.dt_.tree_.feature[node]
+        feature_index = self._dt.tree_.feature[node]
         if feature_index == -2:
             # this is a leaf
             # if it is a regression problem we do not use label
             label = self._calculate_cell_label(node) if not self.is_regression else 1
-            hist = [int(i) for i in self.dt_.tree_.value[node][0]] if not self.is_regression else []
+            hist = [int(i) for i in self._dt.tree_.value[node][0]] if not self.is_regression else []
             cell = {'label': label, 'hist': hist, 'ranges': {}, 'id': int(node)}
             return [cell]
 
         cells = []
-        feature = self.categorical_data.columns[feature_index]
-        threshold = self.dt_.tree_.threshold[node]
-        left_child = self.dt_.tree_.children_left[node]
-        right_child = self.dt_.tree_.children_right[node]
+        feature = self._encoded_features[feature_index]
+        threshold = self._dt.tree_.threshold[node]
+        left_child = self._dt.tree_.children_left[node]
+        right_child = self._dt.tree_.children_right[node]
 
         left_child_cells = self._calculate_cells_recursive(left_child)
         for cell in left_child_cells:
             if feature not in cell['ranges'].keys():
                 cell['ranges'][feature] = {'start': None, 'end': None}
             if cell['ranges'][feature]['end'] is None:
                 cell['ranges'][feature]['end'] = threshold
             cells.append(cell)
-            self.cells_by_id_[cell['id']] = cell
+            self._cells_by_id[cell['id']] = cell
 
         right_child_cells = self._calculate_cells_recursive(right_child)
         for cell in right_child_cells:
             if feature not in cell['ranges'].keys():
                 cell['ranges'][feature] = {'start': None, 'end': None}
             if cell['ranges'][feature]['start'] is None:
                 cell['ranges'][feature]['start'] = threshold
             cells.append(cell)
-            self.cells_by_id_[cell['id']] = cell
+            self._cells_by_id[cell['id']] = cell
 
         return cells
 
     def _calculate_cell_label(self, node):
-        label_hist = self.dt_.tree_.value[node][0]
-        return int(self.dt_.classes_[np.argmax(label_hist)])
+        label_hist = self._dt.tree_.value[node][0]
+        return int(self._dt.classes_[np.argmax(label_hist)])
 
     def _modify_cells(self):
         cells = []
-        features = self.categorical_data.columns
-        for cell in self.cells_:
+        features = self._encoded_features
+        for cell in self.cells:
             new_cell = {'id': cell['id'], 'label': cell['label'], 'ranges': {}, 'categories': {}, 'hist': cell['hist'],
-                        'representative': None}
+                        'untouched': [], 'representative': None}
             for feature in features:
-                if feature in self.oneHotVectorFeaturesToFeatures.keys():
+                if feature in self._one_hot_vector_features_to_features.keys():
                     # feature is categorical and should be mapped
-                    categorical_feature = self.oneHotVectorFeaturesToFeatures[feature]
+                    categorical_feature = self._one_hot_vector_features_to_features[feature]
                     if categorical_feature not in new_cell['categories'].keys():
-                        new_cell['categories'][categorical_feature] = self.categorical_values[
+                        new_cell['categories'][categorical_feature] = self._categorical_values[
                             categorical_feature].copy()
                     if feature in cell['ranges'].keys():
                         categorical_value = feature[len(categorical_feature) + 1:]
                         if cell['ranges'][feature]['start'] is not None:
                             # categorical feature must have this value
                             new_cell['categories'][categorical_feature] = [categorical_value]
                         else:
@@ -580,72 +566,72 @@
                                 new_cell['categories'][categorical_feature].remove(categorical_value)
                 else:
                     if feature in cell['ranges'].keys():
                         new_cell['ranges'][feature] = cell['ranges'][feature]
                     else:
                         new_cell['ranges'][feature] = {'start': None, 'end': None}
             cells.append(new_cell)
-            self.cells_by_id_[new_cell['id']] = new_cell
-        self.cells_ = cells
+            self._cells_by_id[new_cell['id']] = new_cell
+        self.cells = cells
 
     def _calculate_level_cells(self, level):
-        if level < 0 or level > self.dt_.get_depth():
+        if level < 0 or level > self._dt.get_depth():
             raise TypeError("Illegal level %d' % level", level)
 
         if level > 0:
             new_cells = []
             new_cells_by_id = {}
             nodes = self._get_nodes_level(level)
             if nodes:
                 for node in nodes:
-                    if self.dt_.tree_.feature[node] == -2:  # leaf node
-                        new_cell = self.cells_by_id_[node]
+                    if self._dt.tree_.feature[node] == -2:  # leaf node
+                        new_cell = self._cells_by_id[node]
                     else:
-                        left_child = self.dt_.tree_.children_left[node]
-                        right_child = self.dt_.tree_.children_right[node]
-                        left_cell = self.cells_by_id_[left_child]
-                        right_cell = self.cells_by_id_[right_child]
+                        left_child = self._dt.tree_.children_left[node]
+                        right_child = self._dt.tree_.children_right[node]
+                        left_cell = self._cells_by_id[left_child]
+                        right_cell = self._cells_by_id[right_child]
                         new_cell = {'id': int(node), 'ranges': {}, 'categories': {}, 'untouched': [],
                                     'label': None, 'representative': None}
                         for feature in left_cell['ranges'].keys():
                             new_cell['ranges'][feature] = {}
                             new_cell['ranges'][feature]['start'] = left_cell['ranges'][feature]['start']
                             new_cell['ranges'][feature]['end'] = right_cell['ranges'][feature]['start']
                         for feature in left_cell['categories'].keys():
                             new_cell['categories'][feature] = \
-                                list(set(left_cell['categories'][feature]) |
-                                     set(right_cell['categories'][feature]))
+                                list(set(left_cell['categories'][feature])
+                                     | set(right_cell['categories'][feature]))
                         for feature in left_cell['untouched']:
                             if feature in right_cell['untouched']:
                                 new_cell['untouched'].append(feature)
                         self._calculate_level_cell_label(left_cell, right_cell, new_cell)
                     new_cells.append(new_cell)
                     new_cells_by_id[new_cell['id']] = new_cell
-                self.cells_ = new_cells
-                self.cells_by_id_ = new_cells_by_id
+                self.cells = new_cells
+                self._cells_by_id = new_cells_by_id
             # else: nothing to do, stay with previous cells
 
     def _calculate_level_cell_label(self, left_cell, right_cell, new_cell):
         new_cell['hist'] = [x + y for x, y in
                             zip(left_cell['hist'], right_cell['hist'])] if not self.is_regression else []
-        new_cell['label'] = int(self.dt_.classes_[np.argmax(new_cell['hist'])]) if not self.is_regression else 1
+        new_cell['label'] = int(self._dt.classes_[np.argmax(new_cell['hist'])]) if not self.is_regression else 1
 
     def _get_nodes_level(self, level):
         # level = distance from lowest leaf
-        node_depth = np.zeros(shape=self.dt_.tree_.node_count, dtype=np.int64)
-        is_leaves = np.zeros(shape=self.dt_.tree_.node_count, dtype=bool)
+        node_depth = np.zeros(shape=self._dt.tree_.node_count, dtype=np.int64)
+        is_leaves = np.zeros(shape=self._dt.tree_.node_count, dtype=bool)
         stack = [(0, -1)]  # seed is the root node id and its parent depth
         while len(stack) > 0:
             node_id, parent_depth = stack.pop()
             # depth = distance from root
             node_depth[node_id] = parent_depth + 1
 
-            if self.dt_.tree_.children_left[node_id] != self.dt_.tree_.children_right[node_id]:
-                stack.append((self.dt_.tree_.children_left[node_id], parent_depth + 1))
-                stack.append((self.dt_.tree_.children_right[node_id], parent_depth + 1))
+            if self._dt.tree_.children_left[node_id] != self._dt.tree_.children_right[node_id]:
+                stack.append((self._dt.tree_.children_left[node_id], parent_depth + 1))
+                stack.append((self._dt.tree_.children_right[node_id], parent_depth + 1))
             else:
                 is_leaves[node_id] = True
 
         # depth of entire tree
         max_depth = max(node_depth)
         # depth of current level
         depth = max_depth - level
@@ -656,15 +642,15 @@
         return [i for i, x in enumerate(node_depth) if x == depth or (x < depth and is_leaves[i])]
 
     def _attach_cells_representatives(self, prepared_data, originalTrainFeatures, labelFeature, level_nodes):
         # prepared data include one hot encoded categorical data,
         # if there is no categorical data prepared data is original data
         nodeIds = self._find_sample_nodes(prepared_data, level_nodes)
         labels_df = pd.DataFrame(labelFeature, columns=['label'])
-        for cell in self.cells_:
+        for cell in self.cells:
             cell['representative'] = {}
             # get all rows in cell
             indexes = [i for i, x in enumerate(nodeIds) if x == cell['id']]
             original_rows = originalTrainFeatures.iloc[indexes]
             sample_rows = prepared_data.iloc[indexes]
             sample_labels = labels_df.iloc[indexes]['label'].values.tolist()
             # get rows with matching label
@@ -691,42 +677,48 @@
             row = match_rows.iloc[min]
             for feature in cell['ranges'].keys():
                 cell['representative'][feature] = row[feature]
             for feature in cell['categories'].keys():
                 cell['representative'][feature] = row[feature]
 
     def _find_sample_nodes(self, samples, nodes):
-        paths = self.dt_.decision_path(samples).toarray()
+        paths = self._dt.decision_path(samples).toarray()
         nodeSet = set(nodes)
         return [(list(set([i for i, v in enumerate(p) if v == 1]) & nodeSet))[0] for p in paths]
 
     def _generalize(self, original_data, prepared_data, level_nodes, cells, cells_by_id):
+        mapping_to_cells = self._map_to_cells(prepared_data, level_nodes, cells_by_id)
+        all_indexes = []
+        for i in range(len(cells)):
+            # get the indexes of all records that map to this cell
+            indexes = [j for j in mapping_to_cells if mapping_to_cells[j]['id'] == cells[i]['id']]
+            all_indexes.append(indexes)
+        return self._generalize_indexes(original_data, cells, all_indexes)
+
+    def _generalize_indexes(self, original_data, cells, all_indexes):
         # prepared data include one hot encoded categorical data + QI
         representatives = pd.DataFrame(columns=self._features)  # empty except for columns
-        generalized = pd.DataFrame(prepared_data, columns=self.categorical_data.columns, copy=True)
         original_data_generalized = pd.DataFrame(original_data, columns=self._features, copy=True)
-        mapping_to_cells = self._map_to_cells(generalized, level_nodes, cells_by_id)
+
         # iterate over cells (leaves in decision tree)
         for i in range(len(cells)):
             # This code just copies the representatives from the cells into another data structure
             # iterate over features
             for feature in self._features:
                 # if feature has a representative value in the cell and should not be left untouched,
                 # take the representative value
-                if feature in cells[i]['representative'] and ('untouched' not in cells[i] or
-                                                              feature not in cells[i]['untouched']):
+                if feature in cells[i]['representative'] \
+                        and ('untouched' not in cells[i] or feature not in cells[i]['untouched']):
                     representatives.loc[i, feature] = cells[i]['representative'][feature]
                 # else, drop the feature (removes from representatives columns that do not have a
                 # representative value or should remain untouched)
                 elif feature in representatives.columns.tolist():
                     representatives = representatives.drop(feature, axis=1)
 
-            # get the indexes of all records that map to this cell
-            indexes = [j for j in mapping_to_cells if mapping_to_cells[j]['id'] == cells[i]['id']]
-
+            indexes = all_indexes[i]
             # replaces the values in the representative columns with the representative values
             # (leaves others untouched)
             if indexes and not representatives.columns.empty:
                 if len(indexes) > 1:
                     replace = pd.concat([representatives.loc[i].to_frame().T] * len(indexes)).reset_index(drop=True)
                 else:
                     replace = representatives.loc[i].to_frame().T.reset_index(drop=True)
@@ -751,43 +743,43 @@
                                             current_accuracy):
         # prepared data include one hot encoded categorical data,
         # if there is no categorical data prepared data is original data
         feature = self._get_feature_to_remove(original_data, prepared_data, nodes, labels, feature_data,
                                               current_accuracy)
         if feature is None:
             return None
-        GeneralizeToRepresentative._remove_feature_from_cells(self.cells_, self.cells_by_id_, feature)
+        GeneralizeToRepresentative._remove_feature_from_cells(self.cells, self._cells_by_id, feature)
         return feature
 
     def _get_feature_to_remove(self, original_data, prepared_data, nodes, labels, feature_data, current_accuracy):
         # prepared data include one hot encoded categorical data,
         # if there is no categorical data prepared data is original data
         # We want to remove features with low iLoss (NCP) and high accuracy gain
         # (after removing them)
-        ranges = self.generalizations_['ranges']
+        ranges = self._generalizations['ranges']
         range_counts = self._find_range_count(original_data, ranges)
         total = prepared_data.size
         range_min = sys.float_info.max
         remove_feature = None
         categories = self.generalizations['categories']
         category_counts = self._find_categories_count(original_data, categories)
 
         for feature in ranges.keys():
-            if feature not in self.generalizations_['untouched']:
+            if feature not in self._generalizations['untouched']:
                 feature_ncp = self._calc_ncp_numeric(ranges[feature],
                                                      range_counts[feature],
                                                      feature_data[feature],
                                                      total)
                 if feature_ncp > 0:
                     # divide by accuracy gain
-                    new_cells = copy.deepcopy(self.cells_)
-                    cells_by_id = copy.deepcopy(self.cells_by_id_)
+                    new_cells = copy.deepcopy(self.cells)
+                    cells_by_id = copy.deepcopy(self._cells_by_id)
                     GeneralizeToRepresentative._remove_feature_from_cells(new_cells, cells_by_id, feature)
                     generalized = self._generalize(original_data, prepared_data, nodes, new_cells, cells_by_id)
-                    accuracy_gain = self.estimator.score(ArrayDataset(self._preprocessor.transform(generalized),
+                    accuracy_gain = self.estimator.score(ArrayDataset(self.encoder.transform(generalized),
                                                                       labels)) - current_accuracy
                     if accuracy_gain < 0:
                         accuracy_gain = 0
                     if accuracy_gain != 0:
                         feature_ncp = feature_ncp / accuracy_gain
 
                 if feature_ncp < range_min:
@@ -798,39 +790,40 @@
             if feature not in self.generalizations['untouched']:
                 feature_ncp = self._calc_ncp_categorical(categories[feature],
                                                          category_counts[feature],
                                                          feature_data[feature],
                                                          total)
                 if feature_ncp > 0:
                     # divide by accuracy loss
-                    new_cells = copy.deepcopy(self.cells_)
-                    cells_by_id = copy.deepcopy(self.cells_by_id_)
+                    new_cells = copy.deepcopy(self.cells)
+                    cells_by_id = copy.deepcopy(self._cells_by_id)
                     GeneralizeToRepresentative._remove_feature_from_cells(new_cells, cells_by_id, feature)
                     generalized = self._generalize(original_data, prepared_data, nodes, new_cells, cells_by_id)
-                    accuracy_gain = self.estimator.score(ArrayDataset(self._preprocessor.transform(generalized),
+                    accuracy_gain = self.estimator.score(ArrayDataset(self.encoder.transform(generalized),
                                                                       labels)) - current_accuracy
 
                     if accuracy_gain < 0:
                         accuracy_gain = 0
                     if accuracy_gain != 0:
                         feature_ncp = feature_ncp / accuracy_gain
                 if feature_ncp < range_min:
                     range_min = feature_ncp
                     remove_feature = feature
 
         print('feature to remove: ' + (str(remove_feature) if remove_feature is not None else 'none'))
         return remove_feature
 
     def _calculate_generalizations(self):
-        self.generalizations_ = {'ranges': GeneralizeToRepresentative._calculate_ranges(self.cells_),
-                                 'categories': GeneralizeToRepresentative._calculate_categories(self.cells_),
-                                 'untouched': GeneralizeToRepresentative._calculate_untouched(self.cells_)}
+        self._generalizations = {'ranges': GeneralizeToRepresentative._calculate_ranges(self.cells),
+                                 'categories': GeneralizeToRepresentative._calculate_categories(self.cells),
+                                 'untouched': GeneralizeToRepresentative._calculate_untouched(self.cells)}
+        self._remove_categorical_untouched(self._generalizations)
 
     def _find_range_count(self, samples, ranges):
-        samples_df = pd.DataFrame(samples, columns=self.categorical_data.columns)
+        samples_df = pd.DataFrame(samples, columns=self._encoded_features)
         range_counts = {}
         last_value = None
         for r in ranges.keys():
             range_counts[r] = []
             # if empty list, all samples should be counted
             if not ranges[r]:
                 range_counts[r].append(samples_df.shape[0])
@@ -976,7 +969,21 @@
                 cell['untouched'] = []
             if feature in cell['ranges'].keys():
                 del cell['ranges'][feature]
             elif feature in cell['categories'].keys():
                 del cell['categories'][feature]
             cell['untouched'].append(feature)
             cells_by_id[cell['id']] = cell.copy()
+
+    @staticmethod
+    def _remove_categorical_untouched(generalizations):
+        to_remove = []
+        for feature in generalizations['categories'].keys():
+            category_sizes = [len(g) if len(g) > 1 else 0 for g in generalizations['categories'][feature]]
+            if sum(category_sizes) == 0:
+                if 'untouched' not in generalizations:
+                    generalizations['untouched'] = []
+                generalizations['untouched'].append(feature)
+                to_remove.append(feature)
+
+        for feature in to_remove:
+            del generalizations['categories'][feature]
```

### Comparing `ai-privacy-toolkit-0.1.0/apt/utils/dataset_utils.py` & `ai-privacy-toolkit-0.2.0/apt/utils/dataset_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sklearn.preprocessing
 import pandas as pd
 import ssl
 from os import path, mkdir
 from six.moves.urllib.request import urlretrieve
 
 
-def get_iris_dataset(test_set: float = 0.3):
+def get_iris_dataset_np(test_set: float = 0.3):
     """
     Loads the Iris dataset from scikit-learn.
 
     :param test_set: Proportion of the data to use as validation split (value between 0 and 1). Default is 0.3
     :type test_set: float
     :return: Entire dataset and labels as numpy arrays. Returned as a tuple (x_train, y_train), (x_test, y_test)
     """
@@ -20,20 +20,20 @@
 def _load_iris(test_set_size: float = 0.3):
     iris = datasets.load_iris()
     data = iris.data
     labels = iris.target
 
     # Split training and test sets
     x_train, x_test, y_train, y_test = model_selection.train_test_split(data, labels, test_size=test_set_size,
-                                                                                random_state=18, stratify=labels)
+                                                                        random_state=18, stratify=labels)
 
     return (x_train, y_train), (x_test, y_test)
 
 
-def get_diabetes_dataset(test_set: float = 0.3):
+def get_diabetes_dataset_np(test_set: float = 0.3):
     """
     Loads the Diabetes dataset from scikit-learn.
 
     :param test_set: Proportion of the data to use as validation split (value between 0 and 1). Default is 0.3
     :type test_set: float
     :return: Entire dataset and labels as numpy arrays. Returned as a tuple (x_train, y_train), (x_test, y_test)
     """
@@ -48,27 +48,27 @@
     # Split training and test sets
     x_train, x_test, y_train, y_test = model_selection.train_test_split(data, labels, test_size=test_set_size,
                                                                         random_state=18)
 
     return (x_train, y_train), (x_test, y_test)
 
 
-def get_german_credit_dataset(test_set: float = 0.3):
+def get_german_credit_dataset_pd(test_set: float = 0.3):
     """
-    Loads the UCI German credit dataset from `tests/datasets/german` or downloads it from
+    Loads the UCI German credit dataset from `datasets/german` or downloads it from
     https://archive.ics.uci.edu/ml/machine-learning-databases/statlog/german/ if necessary.
 
     :param test_set: Proportion of the data to use as validation split (value between 0 and 1). Default is 0.3
     :type test_set: float
     :return: Dataset and labels as pandas dataframes. Returned as a tuple (x_train, y_train), (x_test, y_test)
     """
 
     url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/statlog/german/german.data'
-    data_dir = '../datasets/german'
-    data_file = '../datasets/german/data'
+    data_dir = 'datasets/german'
+    data_file = 'datasets/german/data'
 
     if not path.exists(data_dir):
         mkdir(data_dir)
 
     ssl._create_default_https_context = ssl._create_unverified_context
     if not path.exists(data_file):
         urlretrieve(url, data_file)
@@ -90,17 +90,14 @@
         train = data.iloc[train_set]
         test = data.iloc[test_set]
     x_train = train.drop(["label"], axis=1)
     y_train = train.loc[:, "label"]
     x_test = test.drop(["label"], axis=1)
     y_test = test.loc[:, "label"]
 
-    categorical_features = ["Existing_checking_account", "Credit_history", "Purpose", "Savings_account",
-                            "Present_employment_since", "Personal_status_sex", "debtors", "Property",
-                            "Other_installment_plans", "Housing", "Job"]
     x_train.reset_index(drop=True, inplace=True)
     y_train.reset_index(drop=True, inplace=True)
     x_test.reset_index(drop=True, inplace=True)
     y_test.reset_index(drop=True, inplace=True)
 
     return (x_train, y_train), (x_test, y_test)
 
@@ -118,33 +115,38 @@
     def modify_Telephone(value):
         if value == 'A191':
             return 0
         elif value == 'A192':
             return 1
         else:
             raise Exception('Bad value')
+
+    def modify_label(value):
+        return value - 1
+
     data['Foreign_worker'] = data['Foreign_worker'].apply(modify_Foreign_worker)
     data['Telephone'] = data['Telephone'].apply(modify_Telephone)
+    data['label'] = data['label'].apply(modify_label)
 
 
-def get_adult_dataset():
+def get_adult_dataset_pd():
     """
-    Loads the UCI Adult dataset from `tests/datasets/adult` or downloads it from
+    Loads the UCI Adult dataset from `datasets/adult` or downloads it from
     https://archive.ics.uci.edu/ml/machine-learning-databases/adult/ if necessary.
 
     :return: Dataset and labels as pandas dataframes. Returned as a tuple (x_train, y_train), (x_test, y_test)
     """
     features = ['age', 'workclass', 'fnlwgt', 'education', 'education-num', 'marital-status', 'occupation',
                 'relationship', 'race', 'sex', 'capital-gain', 'capital-loss', 'hours-per-week', 'native-country',
                 'label']
     train_url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
     test_url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.test'
-    data_dir = '../datasets/adult'
-    train_file = '../datasets/adult/train'
-    test_file = '../datasets/adult/test'
+    data_dir = 'datasets/adult'
+    train_file = 'datasets/adult/train'
+    test_file = 'datasets/adult/test'
 
     if not path.exists(data_dir):
         mkdir(data_dir)
 
     ssl._create_default_https_context = ssl._create_unverified_context
     if not path.exists(train_file):
         urlretrieve(train_url, train_file)
@@ -224,17 +226,17 @@
             data[col] = data[col].fillna('NA')
         except KeyError:
             print('missing column ' + col)
 
     return data.drop(['fnlwgt', 'education'], axis=1)
 
 
-def get_nursery_dataset(raw: bool = True, test_set: float = 0.2, transform_social: bool = False):
+def get_nursery_dataset_pd(raw: bool = True, test_set: float = 0.2, transform_social: bool = False):
     """
-    Loads the UCI Nursery dataset from `tests/datasets/nursery` or downloads it from
+    Loads the UCI Nursery dataset from `datasets/nursery` or downloads it from
     https://archive.ics.uci.edu/ml/machine-learning-databases/nursery/ if necessary.
 
     :param raw: `True` if no preprocessing should be applied to the data. Otherwise, categorical data is one-hot
                 encoded and data is scaled using sklearn's StandardScaler.
     :type raw: boolean
     :param test_set: Proportion of the data to use as validation split. The value should be between 0 and 1. Default is
                      0.2
@@ -242,16 +244,16 @@
     :param transform_social: If `True`, transforms the social feature to be binary for the purpose of attribute
                              inference. This is done by assigning the original value 'problematic' the new value 1, and
                              the other original values are assigned the new value 0.
     :type transform_social: boolean
     :return: Dataset and labels as pandas dataframes. Returned as a tuple (x_train, y_train), (x_test, y_test)
     """
     url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/nursery/nursery.data'
-    data_dir = '../datasets/nursery'
-    data_file = '../datasets/nursery/data'
+    data_dir = 'datasets/nursery'
+    data_file = 'datasets/nursery/data'
 
     if not path.exists(data_dir):
         mkdir(data_dir)
 
     ssl._create_default_https_context = ssl._create_unverified_context
     if not path.exists(data_file):
         urlretrieve(url, data_file)
```

### Comparing `ai-privacy-toolkit-0.1.0/apt/utils/datasets/datasets.py` & `ai-privacy-toolkit-0.2.0/apt/utils/datasets/datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,102 +20,104 @@
 
 
 INPUT_DATA_ARRAY_TYPE = Union[np.ndarray, pd.DataFrame, List, Tensor]
 OUTPUT_DATA_ARRAY_TYPE = np.ndarray
 DATA_PANDAS_NUMPY_TYPE = Union[np.ndarray, pd.DataFrame]
 
 
+def array2numpy(arr: INPUT_DATA_ARRAY_TYPE) -> OUTPUT_DATA_ARRAY_TYPE:
+
+    """
+    converts from INPUT_DATA_ARRAY_TYPE to numpy array
+    """
+    if type(arr) == np.ndarray:
+        return arr
+    if type(arr) == pd.DataFrame or type(arr) == pd.Series:
+        return arr.to_numpy()
+    if isinstance(arr, list):
+        return np.array(arr)
+    if type(arr) == Tensor:
+        return arr.detach().cpu().numpy()
+
+    raise ValueError("Non supported type: ", type(arr).__name__)
+
+
+def array2torch_tensor(arr: INPUT_DATA_ARRAY_TYPE) -> Tensor:
+    """
+    converts from INPUT_DATA_ARRAY_TYPE to torch tensor array
+    """
+    if type(arr) == np.ndarray:
+        return torch.from_numpy(arr)
+    if type(arr) == pd.DataFrame or type(arr) == pd.Series:
+        return torch.from_numpy(arr.to_numpy())
+    if isinstance(arr, list):
+        return torch.tensor(arr)
+    if type(arr) == Tensor:
+        return arr
+
+    raise ValueError("Non supported type: ", type(arr).__name__)
+
+
 class Dataset(metaclass=ABCMeta):
     """Base Abstract Class for Dataset"""
 
     @abstractmethod
     def __init__(self, **kwargs):
         pass
 
     @abstractmethod
     def get_samples(self) -> Collection[Any]:
         """
         Return data samples
 
         :return: the data samples
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def get_labels(self) -> Collection[Any]:
         """
         Return labels
 
         :return: the labels
         """
-        pass
+        raise NotImplementedError
 
-    def _array2numpy(self, arr: INPUT_DATA_ARRAY_TYPE) -> OUTPUT_DATA_ARRAY_TYPE:
+    @abstractmethod
+    def get_predictions(self) -> OUTPUT_DATA_ARRAY_TYPE:
         """
-        Converts from INPUT_DATA_ARRAY_TYPE to numpy array
+        Get predictions
 
-        :param arr: the array to transform
-        :type arr: numpy array or pandas DataFrame or list or pytorch Tensor
-        :return: the array transformed into a numpy array
-        """
-        if type(arr) == np.ndarray:
-            return arr
-        if type(arr) == pd.DataFrame or type(arr) == pd.Series:
-            self.is_pandas = True
-            return arr.to_numpy()
-        if isinstance(arr, list):
-            return np.array(arr)
-        if type(arr) == Tensor:
-            return arr.detach().cpu().numpy()
-
-        raise ValueError('Non supported type: ', type(arr).__name__)
-
-    def _array2torch_tensor(self, arr: INPUT_DATA_ARRAY_TYPE) -> Tensor:
-        """
-        Converts from INPUT_DATA_ARRAY_TYPE to torch tensor array
-
-        :param arr: the array to transform
-        :type arr: numpy array or pandas DataFrame or list or pytorch Tensor
-        :return: the array transformed into a pytorch Tensor
-        """
-        if type(arr) == np.ndarray:
-            return torch.from_numpy(arr)
-        if type(arr) == pd.DataFrame or type(arr) == pd.Series:
-            self.is_pandas = True
-            return torch.from_numpy(arr.to_numpy())
-        if isinstance(arr, list):
-            return torch.tensor(arr)
-        if type(arr) == Tensor:
-            return arr
-
-        raise ValueError('Non supported type: ', type(arr).__name__)
+        :return: predictions as numpy array
+        """
+        raise NotImplementedError
 
 
 class StoredDataset(Dataset):
     """Abstract Class for a Dataset that can be downloaded from a URL and stored in a file"""
 
     @abstractmethod
     def load_from_file(self, path: str):
         """
         Load dataset from file
 
         :param path: the path to the file
         :type path: string
         :return: None
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def load(self, **kwargs):
         """
         Load dataset
 
         :return: None
         """
-        pass
+        raise NotImplementedError
 
     @staticmethod
     def download(url: str, dest_path: str, filename: str, unzip: Optional[bool] = False) -> None:
         """
         Download the dataset from URL
 
         :param url: dataset URL, the dataset will be requested from this URL
@@ -133,15 +135,15 @@
         if os.path.exists(file_path):
             logger.warning("Files already downloaded, skipping downloading")
 
         else:
             os.makedirs(dest_path, exist_ok=True)
             logger.info("Downloading the dataset...")
             urllib.request.urlretrieve(url, file_path)
-            logger.info('Dataset Downloaded')
+            logger.info("Dataset Downloaded")
 
         if unzip:
             StoredDataset.extract_archive(zip_path=file_path, dest_path=dest_path, remove_archive=False)
 
     @staticmethod
     def extract_archive(zip_path: str, dest_path: Optional[str] = None, remove_archive: Optional[bool] = False):
         """
@@ -192,15 +194,15 @@
             os.makedirs(os.path.dirname(dest_datafile), exist_ok=True)
 
         data = np.genfromtxt(datafile, delimiter=delimiter)
         if shuffle:
             logger.info("Shuffling data")
             np.random.shuffle(data)
 
-        debug_data = data[:int(len(data) * ratio)]
+        debug_data = data[: int(len(data) * ratio)]
         logger.info(f"Saving {ratio} of the data to {dest_datafile}")
         np.savetxt(dest_datafile, debug_data, delimiter=delimiter, fmt=fmt)
 
 
 class ArrayDataset(Dataset):
     """
     Dataset that is based on x and y arrays (e.g., numpy/pandas/list...)
@@ -211,25 +213,27 @@
     :type y: numpy array or pandas DataFrame or list or pytorch Tensor, optional
     :param feature_names: The feature names, in the order that they appear in the data
     :type feature_names: list of strings, optional
     """
 
     def __init__(self, x: INPUT_DATA_ARRAY_TYPE, y: Optional[INPUT_DATA_ARRAY_TYPE] = None,
                  features_names: Optional[list] = None, **kwargs):
-        self.is_pandas = False
+        self.is_pandas = self.is_pandas = type(x) == pd.DataFrame or type(x) == pd.Series
+
         self.features_names = features_names
-        self._y = self._array2numpy(y) if y is not None else None
-        self._x = self._array2numpy(x)
+        self._y = array2numpy(y) if y is not None else None
+        self._x = array2numpy(x)
+
         if self.is_pandas:
             if features_names and not np.array_equal(features_names, x.columns):
                 raise ValueError("The supplied features are not the same as in the data features")
             self.features_names = x.columns.to_list()
 
-        if y is not None and len(self._x) != len(self._y):
-            raise ValueError('Non equivalent lengths of x and y')
+        if self._y is not None and len(self._x) != len(self._y):
+            raise ValueError("Non equivalent lengths of x and y")
 
     def get_samples(self) -> OUTPUT_DATA_ARRAY_TYPE:
         """
         Get data samples
 
         :return: data samples as numpy array
         """
@@ -239,97 +243,172 @@
         """
         Get labels
 
         :return: labels as numpy array
         """
         return self._y
 
+    def get_predictions(self) -> OUTPUT_DATA_ARRAY_TYPE:
+        """
+        Get predictions
+
+        :return: predictions as numpy array
+        """
+        return None
+
+
+class DatasetWithPredictions(Dataset):
+    """
+    Dataset that is based on arrays (e.g., numpy/pandas/list...). Includes predictions from a model, and possibly also
+    features and true labels.
+
+    :param x: collection of data samples
+    :type x: numpy array or pandas DataFrame or list or pytorch Tensor
+    :param y: collection of labels
+    :type y: numpy array or pandas DataFrame or list or pytorch Tensor, optional
+    :param feature_names: The feature names, in the order that they appear in the data
+    :type feature_names: list of strings, optional
+    """
+
+    def __init__(self, pred: INPUT_DATA_ARRAY_TYPE, x: Optional[INPUT_DATA_ARRAY_TYPE] = None,
+                 y: Optional[INPUT_DATA_ARRAY_TYPE] = None, features_names: Optional[list] = None, **kwargs):
+        self.is_pandas = False
+        self.features_names = features_names
+        self._pred = array2numpy(pred)
+        self._y = array2numpy(y) if y is not None else None
+        self._x = array2numpy(x) if x is not None else None
+        if self.is_pandas and x is not None:
+            if features_names and not np.array_equal(features_names, x.columns):
+                raise ValueError("The supplied features are not the same as in the data features")
+            self.features_names = x.columns.to_list()
+
+        if self._y is not None and len(self._pred) != len(self._y):
+            raise ValueError('Non equivalent lengths of pred and y')
+
+        if self._x is not None and len(self._x) != len(self._pred):
+            raise ValueError('Non equivalent lengths of x and pred')
+
+    def get_samples(self) -> OUTPUT_DATA_ARRAY_TYPE:
+        """
+        Get data samples
+
+        :return: data samples as numpy array
+        """
+        return self._x
+
+    def get_labels(self) -> OUTPUT_DATA_ARRAY_TYPE:
+        """
+        Get labels
+
+        :return: labels as numpy array
+        """
+        return self._y
+
+    def get_predictions(self) -> OUTPUT_DATA_ARRAY_TYPE:
+        """
+        Get predictions
+
+        :return: predictions as numpy array
+        """
+        return self._pred
+
 
 class PytorchData(Dataset):
     """
     Dataset for pytorch models.
 
     :param x: collection of data samples
     :type x: numpy array or pandas DataFrame or list or pytorch Tensor
     :param y: collection of labels
     :type y: numpy array or pandas DataFrame or list or pytorch Tensor, optional
     """
     def __init__(self, x: INPUT_DATA_ARRAY_TYPE, y: Optional[INPUT_DATA_ARRAY_TYPE] = None, **kwargs):
-        self.is_pandas = False
-        self._y = self._array2torch_tensor(y) if y is not None else None
-        self._x = self._array2torch_tensor(x)
+        self._y = array2torch_tensor(y) if y is not None else None
+        self._x = array2torch_tensor(x)
+
+        self.is_pandas = type(x) == pd.DataFrame or type(x) == pd.Series
+
         if self.is_pandas:
             self.features_names = x.columns
 
-        if y is not None and len(self._x) != len(self._y):
-            raise ValueError('Non equivalent lengths of x and y')
+        if self._y is not None and len(self._x) != len(self._y):
+            raise ValueError("Non equivalent lengths of x and y")
 
         if self._y is not None:
             self.__getitem__ = self.get_item
         else:
             self.__getitem__ = self.get_sample_item
 
     def get_samples(self) -> OUTPUT_DATA_ARRAY_TYPE:
         """
         Get data samples.
 
         :return: samples as numpy array
         """
-        return self._array2numpy(self._x)
+        return array2numpy(self._x)
 
     def get_labels(self) -> OUTPUT_DATA_ARRAY_TYPE:
         """
         Get labels.
 
         :return: labels as numpy array
         """
-        return self._array2numpy(self._y) if self._y is not None else None
+        return array2numpy(self._y) if self._y is not None else None
+
+    def get_predictions(self) -> OUTPUT_DATA_ARRAY_TYPE:
+        """
+        Get predictions
+
+        :return: predictions as numpy array
+        """
+        return None
 
     def get_sample_item(self, idx: int) -> Tensor:
         """
         Get the sample according to the given index
 
         :param idx: the index of the sample to return
         :type idx: int
         :return: the sample as a pytorch Tensor
         """
-        return self.x[idx]
+        return self._x[idx]
 
     def get_item(self, idx: int) -> Tensor:
         """
         Get the sample and label according to the given index
 
         :param idx: the index of the sample to return
         :type idx: int
         :return: the sample and label as pytorch Tensors. Returned as a tuple (sample, label)
         """
-        sample, label = self.x[idx], self.y[idx]
+        sample, label = self._x[idx], self._y[idx]
         return sample, label
 
     def __len__(self):
-        return len(self.x)
+        return len(self._x)
 
 
 class DatasetFactory:
     """Factory class for dataset creation"""
+
     registry = {}
 
     @classmethod
     def register(cls, name: str) -> Callable:
         """
         Class method to register Dataset to the internal registry
 
         :param name: dataset name
         :type name: string
         :return: a Callable that returns the registered dataset class
         """
 
         def inner_wrapper(wrapped_class: Type[Dataset]) -> Any:
             if name in cls.registry:
-                logger.warning('Dataset %s already exists. Will replace it', name)
+                logger.warning("Dataset %s already exists. Will replace it", name)
             cls.registry[name] = wrapped_class
             return wrapped_class
 
         return inner_wrapper
 
     @classmethod
     def create_dataset(cls, name: str, **kwargs) -> Dataset:
@@ -343,15 +422,15 @@
         :param name: The name of the dataset to create.
         :type name: string
         :param kwargs: dataset parameters
         :type kwargs: keyword arguments as expected by the class
         :return: An instance of the dataset that is created.
         """
         if name not in cls.registry:
-            msg = f'Dataset {name} does not exist in the registry'
+            msg = f"Dataset {name} does not exist in the registry"
             logger.error(msg)
             raise ValueError(msg)
 
         exec_class = cls.registry[name]
         executor = exec_class(**kwargs)
         return executor
 
@@ -392,36 +471,64 @@
 
         :return: test 'Dataset`
         """
         return self.test
 
     def get_train_samples(self) -> Collection[Any]:
         """
-        Get train set samples
+        Get train set samples, or None if no training data provided
 
         :return: training samples
         """
+        if self.train is None:
+            return None
         return self.train.get_samples()
 
     def get_train_labels(self) -> Collection[Any]:
         """
-        Get train set labels
+        Get train set labels, or None if no training labels provided
 
         :return: training labels
         """
+        if self.train is None:
+            return None
         return self.train.get_labels()
 
+    def get_train_predictions(self) -> Collection[Any]:
+        """
+        Get train set predictions, or None if no training predictions provided
+
+        :return: training labels
+        """
+        if self.train is None:
+            return None
+        return self.train.get_predictions()
+
     def get_test_samples(self) -> Collection[Any]:
         """
         Get test set samples
 
-        :return: test samples
+        :return: test samples, or None if no test data provided
         """
+        if self.test is None:
+            return None
         return self.test.get_samples()
 
     def get_test_labels(self) -> Collection[Any]:
         """
         Get test set labels
 
-        :return: test labels
+        :return: test labels, or None if no test labels provided
         """
+        if self.test is None:
+            return None
         return self.test.get_labels()
+
+    def get_test_predictions(self) -> Collection[Any]:
+        """
+        Get test set predictions, or None if no test predictions provided
+
+        :return: test labels
+        """
+        if self.test is None:
+            return None
+        return self.test.get_predictions()
```

### Comparing `ai-privacy-toolkit-0.1.0/apt/utils/models/model.py` & `ai-privacy-toolkit-0.2.0/apt/utils/models/xgboost_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,86 @@
-from abc import ABCMeta, abstractmethod
-from typing import Any, Optional
-from enum import Enum, auto
+from typing import Optional, Tuple
 
+from apt.utils.models import Model, ModelOutputType, ScoringMethod, check_correct_model_output, is_one_hot
 from apt.utils.datasets import Dataset, OUTPUT_DATA_ARRAY_TYPE
 
+import numpy as np
 
-class ModelOutputType(Enum):
-    CLASSIFIER_VECTOR = auto()  # probabilities or logits
-    CLASSIFIER_SCALAR = auto()  # label only
-    REGRESSOR_SCALAR = auto()  # value
+from art.estimators.classification.xgboost import XGBoostClassifier as ArtXGBoostClassifier
 
 
-class Model(metaclass=ABCMeta):
+class XGBoostModel(Model):
     """
-    Abstract base class for ML model wrappers.
+    Wrapper class for xgboost models.
+    """
+
+
+class XGBoostClassifier(XGBoostModel):
+    """
+    Wrapper class for xgboost classification models.
 
-    :param model: The original model object (of the underlying ML framework)
-    :type model: framework-specific model object
-    :param output_type: The type of output the model yields (vector/label only for classifiers,
-                        value for regressors)
+    :param model: The original xgboost model object. Must be fit.
+    :type model: Booster or XGBClassifier object
+    :param output_type: The type of output the model yields (vector/label only)
     :type output_type: `ModelOutputType`
+    :param input_shape: Shape of input to the model.
+    :type input_shape: Tuple[int, ...]
+    :param nb_classes: Number of prediction classes of the model.
+    :type  nb_classes: int
     :param black_box_access: Boolean describing the type of deployment of the model (when in production).
                              Set to True if the model is only available via query (API) access, i.e.,
                              only the outputs of the model are exposed, and False if the model internals
                              are also available. Default is True.
     :type black_box_access: boolean, optional
     :param unlimited_queries: If black_box_access is True, this boolean indicates whether a user can perform
                               unlimited queries to the model API or whether there is a limit to the number of
                               queries that can be submitted. Default is True.
     :type unlimited_queries: boolean, optional
     """
-
-    def __init__(self, model: Any, output_type: ModelOutputType, black_box_access: Optional[bool] = True,
+    def __init__(self, model: "xgboost.XGBClassifier", output_type: ModelOutputType, input_shape: Tuple[int, ...],
+                 nb_classes: int, black_box_access: Optional[bool] = True,
                  unlimited_queries: Optional[bool] = True, **kwargs):
-        self._model = model
-        self._output_type = output_type
-        self._black_box_access = black_box_access
-        self._unlimited_queries = unlimited_queries
+        super().__init__(model, output_type, black_box_access, unlimited_queries, **kwargs)
+        self._art_model = ArtXGBoostClassifier(model, nb_features=input_shape[0], nb_classes=nb_classes)
+        self.nb_classes = nb_classes
 
-    @abstractmethod
     def fit(self, train_data: Dataset, **kwargs) -> None:
         """
         Fit the model using the training data.
 
-        :param train_data: Training data.
+        :param train_data: Training data. Labels are expected to either be one-hot encoded or a 1D-array of categorical
+                           labels (consecutive integers starting at 0).
         :type train_data: `Dataset`
+        :return: None
         """
-        raise NotImplementedError
+        self._art_model._model.fit(train_data.get_samples(), train_data.get_labels())
 
-    @abstractmethod
     def predict(self, x: Dataset, **kwargs) -> OUTPUT_DATA_ARRAY_TYPE:
         """
         Perform predictions using the model for input `x`.
 
         :param x: Input samples.
-        :type x: `np.ndarray` or `pandas.DataFrame`
-        :return: Predictions from the model as numpy array.
+        :type x: `Dataset`
+        :return: Predictions from the model as numpy array (class probabilities, if supported).
         """
-        raise NotImplementedError
+        predictions = self._art_model.predict(x.get_samples(), **kwargs)
+        check_correct_model_output(predictions, self.output_type)
+        return predictions
 
-    @abstractmethod
-    def score(self, test_data: Dataset, **kwargs):
+    def score(self, test_data: Dataset, scoring_method: Optional[ScoringMethod] = ScoringMethod.ACCURACY, **kwargs):
         """
         Score the model using test data.
 
         :param test_data: Test data.
         :type train_data: `Dataset`
         :return: the score as float (for classifiers, between 0 and 1)
         """
-        return NotImplementedError
-
-    @property
-    def model(self) -> Any:
-        """
-        Return the underlying model.
-
-        :return: The model.
-        """
-        return self._model
-
-    @property
-    def output_type(self) -> ModelOutputType:
-        """
-        Return the model's output type.
-
-        :return: The model's output type.
-        """
-        return self._output_type
-
-    @property
-    def black_box_access(self) -> bool:
-        """
-        Return whether the model is only available via query (API) access, i.e.,
-        only the outputs of the model are exposed, or if the model internals are also available.
-
-        :return: True if the model is only available via query (API) access, otherwise False.
-        """
-        return self._black_box_access
-
-    @property
-    def unlimited_queries(self) -> bool:
-        """
-        If black_box_access is True, return whether a user can perform unlimited queries to the model API
-        or whether there is a limit to the number of queries that can be submitted.
-
-        :return: True if a user can perform unlimited queries to the model API, otherwise False.
-        """
-        return self._unlimited_queries
+        y = test_data.get_labels()
+        predicted = self.predict(test_data)
+        if is_one_hot(predicted):
+            predicted = np.argmax(predicted, axis=1)
+        if is_one_hot(y):
+            y = np.argmax(y, axis=1)
+        if scoring_method == ScoringMethod.ACCURACY:
+            return np.count_nonzero(y == predicted) / predicted.shape[0]
+        else:
+            raise NotImplementedError
```

### Comparing `ai-privacy-toolkit-0.1.0/apt/utils/models/sklearn_model.py` & `ai-privacy-toolkit-0.2.0/apt/utils/models/sklearn_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Optional
 
-import numpy as np
-
-from sklearn.preprocessing import OneHotEncoder
 from sklearn.base import BaseEstimator
 
-from apt.utils.models import Model, ModelOutputType
+from apt.utils.models import Model, ModelOutputType, get_nb_classes, check_correct_model_output
 from apt.utils.datasets import Dataset, OUTPUT_DATA_ARRAY_TYPE
 
 from art.estimators.classification.scikitlearn import SklearnClassifier as ArtSklearnClassifier
 from art.estimators.regression.scikitlearn import ScikitlearnRegressor
+from art.utils import check_and_transform_label_format
 
 
 class SklearnModel(Model):
     """
     Wrapper class for scikitlearn models.
     """
     def score(self, test_data: Dataset, **kwargs):
@@ -50,31 +48,35 @@
         super().__init__(model, output_type, black_box_access, unlimited_queries, **kwargs)
         self._art_model = ArtSklearnClassifier(model)
 
     def fit(self, train_data: Dataset, **kwargs) -> None:
         """
         Fit the model using the training data.
 
-        :param train_data: Training data.
+        :param train_data: Training data. Labels are expected to either be one-hot encoded or a 1D-array of categorical
+                           labels (consecutive integers starting at 0).
         :type train_data: `Dataset`
         :return: None
         """
-        encoder = OneHotEncoder(sparse=False)
-        y_encoded = encoder.fit_transform(train_data.get_labels().reshape(-1, 1))
+        y = train_data.get_labels()
+        self.nb_classes = get_nb_classes(y)
+        y_encoded = check_and_transform_label_format(y, nb_classes=self.nb_classes)
         self._art_model.fit(train_data.get_samples(), y_encoded, **kwargs)
 
     def predict(self, x: Dataset, **kwargs) -> OUTPUT_DATA_ARRAY_TYPE:
         """
         Perform predictions using the model for input `x`.
 
         :param x: Input samples.
         :type x: `Dataset`
         :return: Predictions from the model as numpy array (class probabilities, if supported).
         """
-        return self._art_model.predict(x, **kwargs)
+        predictions = self._art_model.predict(x.get_samples(), **kwargs)
+        check_correct_model_output(predictions, self.output_type)
+        return predictions
 
 
 class SklearnRegressor(SklearnModel):
     """
     Wrapper class for scikitlearn regression models.
 
     :param model: The original sklearn model object.
@@ -108,8 +110,8 @@
         """
         Perform predictions using the model for input `x`.
 
         :param x: Input samples.
         :type x: `Dataset`
         :return: Predictions from the model as numpy array.
         """
-        return self._art_model.predict(x, **kwargs)
+        return self._art_model.predict(x.get_samples(), **kwargs)
```

### Comparing `ai-privacy-toolkit-0.1.0/setup.cfg` & `ai-privacy-toolkit-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ai-privacy-toolkit
-version = 0.1.0
+version = 0.2.0
 author = Abigail Goldsteen
 author_email = abigailt@il.ibm.com
 description = A toolkit for tools and techniques related to the privacy and compliance of AI models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/ai-privacy-toolkit
 project_urls = 
@@ -18,11 +18,15 @@
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
 exclude = 
 	tests
 
+[flake8]
+ignore = C901,W503
+per-file-ignores = __init__.py:F401
+
 [egg_info]
 tag_build = 
 tag_date = 0
```


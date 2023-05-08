# Comparing `tmp/weasel-classifier-0.1.4.tar.gz` & `tmp/weasel-classifier-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasel-classifier-0.1.4.tar", last modified: Thu Mar  9 08:21:20 2023, max compression
+gzip compressed data, was "weasel-classifier-0.1.5.tar", last modified: Mon May  8 20:29:53 2023, max compression
```

## Comparing `weasel-classifier-0.1.4.tar` & `weasel-classifier-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.983891 weasel-classifier-0.1.4/
--rw-r--r--   0 bzcschae   (501) staff       (20)    35149 2022-12-30 10:49:29.000000 weasel-classifier-0.1.4/LICENSE
--rw-r--r--   0 bzcschae   (501) staff       (20)    43953 2023-03-09 08:21:20.984108 weasel-classifier-0.1.4/PKG-INFO
--rw-r--r--   0 bzcschae   (501) staff       (20)     2249 2023-01-30 13:45:17.000000 weasel-classifier-0.1.4/README.md
--rw-r--r--   0 bzcschae   (501) staff       (20)     1643 2023-03-09 08:21:00.000000 weasel-classifier-0.1.4/pyproject.toml
--rw-r--r--   0 bzcschae   (501) staff       (20)       79 2023-03-09 08:21:20.984406 weasel-classifier-0.1.4/setup.cfg
--rw-r--r--   0 bzcschae   (501) staff       (20)     1476 2023-03-09 08:21:00.000000 weasel-classifier-0.1.4/setup.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.979532 weasel-classifier-0.1.4/weasel/
--rw-r--r--   0 bzcschae   (501) staff       (20)        0 2022-03-04 13:25:18.000000 weasel-classifier-0.1.4/weasel/__init__.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.979645 weasel-classifier-0.1.4/weasel/classification/
--rw-r--r--   0 bzcschae   (501) staff       (20)       24 2022-12-30 10:55:53.000000 weasel-classifier-0.1.4/weasel/classification/__init__.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.981757 weasel-classifier-0.1.4/weasel/classification/dictionary_based/
--rw-r--r--   0 bzcschae   (501) staff       (20)      496 2023-01-31 17:57:39.000000 weasel-classifier-0.1.4/weasel/classification/dictionary_based/__init__.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    25481 2023-01-31 17:58:41.000000 weasel-classifier-0.1.4/weasel/classification/dictionary_based/_boss.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    14481 2023-01-31 09:06:03.000000 weasel-classifier-0.1.4/weasel/classification/dictionary_based/_muse.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    12763 2023-03-09 08:21:00.000000 weasel-classifier-0.1.4/weasel/classification/dictionary_based/_muse_v2.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    12045 2023-03-09 08:21:00.000000 weasel-classifier-0.1.4/weasel/classification/dictionary_based/_weasel.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    13618 2023-03-09 08:21:00.000000 weasel-classifier-0.1.4/weasel/classification/dictionary_based/_weasel_v2.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.981931 weasel-classifier-0.1.4/weasel/transformations/
--rw-r--r--   0 bzcschae   (501) staff       (20)        0 2022-03-04 13:25:18.000000 weasel-classifier-0.1.4/weasel/transformations/__init__.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.982047 weasel-classifier-0.1.4/weasel/transformations/panel/
--rw-r--r--   0 bzcschae   (501) staff       (20)        0 2022-03-04 13:25:18.000000 weasel-classifier-0.1.4/weasel/transformations/panel/__init__.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.982475 weasel-classifier-0.1.4/weasel/transformations/panel/dictionary_based/
--rw-r--r--   0 bzcschae   (501) staff       (20)      155 2022-12-30 11:20:02.000000 weasel-classifier-0.1.4/weasel/transformations/panel/dictionary_based/__init__.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    42503 2023-01-31 21:12:48.000000 weasel-classifier-0.1.4/weasel/transformations/panel/dictionary_based/_sfa_dilation.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-03-09 08:21:20.983778 weasel-classifier-0.1.4/weasel_classifier.egg-info/
--rw-r--r--   0 bzcschae   (501) staff       (20)    43953 2023-03-09 08:21:20.000000 weasel-classifier-0.1.4/weasel_classifier.egg-info/PKG-INFO
--rw-r--r--   0 bzcschae   (501) staff       (20)      846 2023-03-09 08:21:20.000000 weasel-classifier-0.1.4/weasel_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 bzcschae   (501) staff       (20)        1 2023-03-09 08:21:20.000000 weasel-classifier-0.1.4/weasel_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 bzcschae   (501) staff       (20)        1 2023-01-30 07:46:56.000000 weasel-classifier-0.1.4/weasel_classifier.egg-info/not-zip-safe
--rw-r--r--   0 bzcschae   (501) staff       (20)      137 2023-03-09 08:21:20.000000 weasel-classifier-0.1.4/weasel_classifier.egg-info/requires.txt
--rw-r--r--   0 bzcschae   (501) staff       (20)        7 2023-03-09 08:21:20.000000 weasel-classifier-0.1.4/weasel_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.349147 weasel-classifier-0.1.5/
+-rw-r--r--   0 bzcschae   (501) staff       (20)    35149 2022-12-30 10:49:29.000000 weasel-classifier-0.1.5/LICENSE
+-rw-r--r--   0 bzcschae   (501) staff       (20)    43941 2023-05-08 20:29:53.349354 weasel-classifier-0.1.5/PKG-INFO
+-rw-r--r--   0 bzcschae   (501) staff       (20)     2237 2023-05-08 20:28:10.000000 weasel-classifier-0.1.5/README.md
+-rw-r--r--   0 bzcschae   (501) staff       (20)     1635 2023-05-08 20:29:50.000000 weasel-classifier-0.1.5/pyproject.toml
+-rw-r--r--   0 bzcschae   (501) staff       (20)       79 2023-05-08 20:29:53.349645 weasel-classifier-0.1.5/setup.cfg
+-rw-r--r--   0 bzcschae   (501) staff       (20)     1476 2023-03-09 08:21:00.000000 weasel-classifier-0.1.5/setup.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.344815 weasel-classifier-0.1.5/weasel/
+-rw-r--r--   0 bzcschae   (501) staff       (20)        0 2022-03-04 13:25:18.000000 weasel-classifier-0.1.5/weasel/__init__.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.344964 weasel-classifier-0.1.5/weasel/classification/
+-rw-r--r--   0 bzcschae   (501) staff       (20)       24 2022-12-30 10:55:53.000000 weasel-classifier-0.1.5/weasel/classification/__init__.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.346810 weasel-classifier-0.1.5/weasel/classification/dictionary_based/
+-rw-r--r--   0 bzcschae   (501) staff       (20)      496 2023-01-31 17:57:39.000000 weasel-classifier-0.1.5/weasel/classification/dictionary_based/__init__.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    25469 2023-05-08 20:26:56.000000 weasel-classifier-0.1.5/weasel/classification/dictionary_based/_boss.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    14475 2023-05-08 20:26:32.000000 weasel-classifier-0.1.5/weasel/classification/dictionary_based/_muse.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    12759 2023-05-08 20:26:38.000000 weasel-classifier-0.1.5/weasel/classification/dictionary_based/_muse_v2.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    12041 2023-05-08 20:26:08.000000 weasel-classifier-0.1.5/weasel/classification/dictionary_based/_weasel.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    13614 2023-05-08 20:25:56.000000 weasel-classifier-0.1.5/weasel/classification/dictionary_based/_weasel_v2.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.347061 weasel-classifier-0.1.5/weasel/transformations/
+-rw-r--r--   0 bzcschae   (501) staff       (20)        0 2022-03-04 13:25:18.000000 weasel-classifier-0.1.5/weasel/transformations/__init__.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.347195 weasel-classifier-0.1.5/weasel/transformations/panel/
+-rw-r--r--   0 bzcschae   (501) staff       (20)        0 2022-03-04 13:25:18.000000 weasel-classifier-0.1.5/weasel/transformations/panel/__init__.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.347607 weasel-classifier-0.1.5/weasel/transformations/panel/dictionary_based/
+-rw-r--r--   0 bzcschae   (501) staff       (20)      155 2022-12-30 11:20:02.000000 weasel-classifier-0.1.5/weasel/transformations/panel/dictionary_based/__init__.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    42499 2023-05-08 20:27:13.000000 weasel-classifier-0.1.5/weasel/transformations/panel/dictionary_based/_sfa_dilation.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-05-08 20:29:53.349038 weasel-classifier-0.1.5/weasel_classifier.egg-info/
+-rw-r--r--   0 bzcschae   (501) staff       (20)    43941 2023-05-08 20:29:53.000000 weasel-classifier-0.1.5/weasel_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 bzcschae   (501) staff       (20)      846 2023-05-08 20:29:53.000000 weasel-classifier-0.1.5/weasel_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 bzcschae   (501) staff       (20)        1 2023-05-08 20:29:53.000000 weasel-classifier-0.1.5/weasel_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 bzcschae   (501) staff       (20)        1 2023-01-30 07:46:56.000000 weasel-classifier-0.1.5/weasel_classifier.egg-info/not-zip-safe
+-rw-r--r--   0 bzcschae   (501) staff       (20)      129 2023-05-08 20:29:53.000000 weasel-classifier-0.1.5/weasel_classifier.egg-info/requires.txt
+-rw-r--r--   0 bzcschae   (501) staff       (20)        7 2023-05-08 20:29:53.000000 weasel-classifier-0.1.5/weasel_classifier.egg-info/top_level.txt
```

### Comparing `weasel-classifier-0.1.4/LICENSE` & `weasel-classifier-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `weasel-classifier-0.1.4/PKG-INFO` & `weasel-classifier-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel-classifier
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Random Dilated Dictionary Transform for Fast, Accurate and Constrained Memory Time Series Classification
 Home-page: https://github.com/patrickzib/dictionary
 Author: patrickzib
 Author-email: patrickzib <void@void.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -717,15 +717,15 @@
 ![UCR_runtime](https://user-images.githubusercontent.com/7783034/214376264-7961db3b-2f24-488f-abbc-d53433ffacbc.png)
 
 
 ## Installation
 
 ### Dependencies
 ```
-sktime >= 0.13,<=0.15
+aeon >= 0.1.0
 ```
 
 # Installation
 
 The easiest is to use pip to install weasel-classifier.
 
 ## a) Install using pip
@@ -746,18 +746,18 @@
 ```
 pip install .
 ```
 
 
 ### Train a WEASEL 2.0 classifier
 
-WEASEL v2 follows the sktime pipeline.
+WEASEL v2 follows the aeon pipeline.
 
 ```python
-from sktime.datasets import load_arrow_head
+from aeon.datasets import load_arrow_head
 from weasel.classification.dictionary_based import WEASEL_V2
 
 X_train, y_train = load_arrow_head(split="train", return_type="numpy3d")
 X_test, y_test = load_arrow_head(split="test", return_type="numpy3d")
 clf = WEASEL_V2(random_state=1379, n_jobs=4)
 clf.fit(X_train,y_train)
 clf.predict(X_test)
```

### Comparing `weasel-classifier-0.1.4/README.md` & `weasel-classifier-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ![UCR_runtime](https://user-images.githubusercontent.com/7783034/214376264-7961db3b-2f24-488f-abbc-d53433ffacbc.png)
 
 
 ## Installation
 
 ### Dependencies
 ```
-sktime >= 0.13,<=0.15
+aeon >= 0.1.0
 ```
 
 # Installation
 
 The easiest is to use pip to install weasel-classifier.
 
 ## a) Install using pip
@@ -44,18 +44,18 @@
 ```
 pip install .
 ```
 
 
 ### Train a WEASEL 2.0 classifier
 
-WEASEL v2 follows the sktime pipeline.
+WEASEL v2 follows the aeon pipeline.
 
 ```python
-from sktime.datasets import load_arrow_head
+from aeon.datasets import load_arrow_head
 from weasel.classification.dictionary_based import WEASEL_V2
 
 X_train, y_train = load_arrow_head(split="train", return_type="numpy3d")
 X_test, y_test = load_arrow_head(split="test", return_type="numpy3d")
 clf = WEASEL_V2(random_state=1379, n_jobs=4)
 clf.fit(X_train,y_train)
 clf.predict(X_test)
```

### Comparing `weasel-classifier-0.1.4/pyproject.toml` & `weasel-classifier-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "weasel-classifier"
 
-version = "0.1.4"
+version = "0.1.5"
 
 description = "A Random Dilated Dictionary Transform for Fast, Accurate and Constrained Memory Time Series Classification"
 readme = "README.md"
 authors = [
     {name = "patrickzib", email = "void@void.com"}
 ]
 keywords = [
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.7,<3.11"
 dependencies = [
     "joblib>=1.1.1",
-    "sktime>=0.15,<=0.16",
+    "aeon>=0.1.0",
     "numba>=0.55.1",
     "numpy>=1.21.0,<1.25",
     "pandas>=1.1.0,<1.6.0",
     "scikit-learn>=0.24.0,<1.3.0",
     "scipy<2.0.0,>=1.2.0",
 ]
```

### Comparing `weasel-classifier-0.1.4/setup.py` & `weasel-classifier-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `weasel-classifier-0.1.4/weasel/classification/dictionary_based/_boss.py` & `weasel-classifier-0.1.5/weasel/classification/dictionary_based/_boss.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from sklearn.metrics import pairwise
 from sklearn.utils import check_random_state, gen_even_slices
 from sklearn.utils.extmath import safe_sparse_dot
 from sklearn.utils.fixes import delayed
 from sklearn.utils.sparsefuncs_fast import csr_row_norms
 from sklearn.utils.validation import _num_samples
 
-from sktime.classification.base import BaseClassifier
-from sktime.utils.validation.panel import check_X_y
+from aeon.classification.base import BaseClassifier
+from aeon.utils.validation.panel import check_X_y
 
 from weasel.transformations.panel.dictionary_based import SFADilation
 
 
 class BOSSEnsemble(BaseClassifier):
     """Ensemble of Bag of Symbolic Fourier Approximation Symbols (BOSS).
 
@@ -113,16 +113,16 @@
     ----------
     .. [1] Patrick Schäfer, "The BOSS is concerned with time series classification
        in the presence of noise", Data Mining and Knowledge Discovery, 29(6): 2015
        https://link.springer.com/article/10.1007/s10618-014-0377-7
 
     Examples
     --------
-    >>> from sktime.classification.dictionary_based import BOSSEnsemble
-    >>> from sktime.datasets import load_unit_test
+    >>> from aeon.classification.dictionary_based import BOSSEnsemble
+    >>> from aeon.datasets import load_unit_test
     >>> X_train, y_train = load_unit_test(split="train", return_X_y=True)
     >>> X_test, y_test = load_unit_test(split="test", return_X_y=True)
     >>> clf = BOSSEnsemble(max_ensemble_size=3)
     >>> clf.fit(X_train, y_train)
     BOSSEnsemble(...)
     >>> y_pred = clf.predict(X_test)
     """
@@ -478,16 +478,16 @@
     ----------
     .. [1] Patrick Schäfer, "The BOSS is concerned with time series classification
        in the presence of noise", Data Mining and Knowledge Discovery, 29(6): 2015
        https://link.springer.com/article/10.1007/s10618-014-0377-7
 
     Examples
     --------
-    >>> from sktime.classification.dictionary_based import IndividualBOSS
-    >>> from sktime.datasets import load_unit_test
+    >>> from aeon.classification.dictionary_based import IndividualBOSS
+    >>> from aeon.datasets import load_unit_test
     >>> X_train, y_train = load_unit_test(split="train", return_X_y=True)
     >>> X_test, y_test = load_unit_test(split="test", return_X_y=True)
     >>> clf = IndividualBOSS()
     >>> clf.fit(X_train, y_train)
     IndividualBOSS(...)
     >>> y_pred = clf.predict(X_test)
     """
```

### Comparing `weasel-classifier-0.1.4/weasel/classification/dictionary_based/_muse.py` & `weasel-classifier-0.1.5/weasel/classification/dictionary_based/_muse.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import numpy as np
 from joblib import Parallel, delayed
 from scipy.sparse import hstack
 from sklearn.linear_model import LogisticRegression, RidgeClassifierCV
 from sklearn.utils import check_random_state
 
-from sktime.classification.base import BaseClassifier
+from aeon.classification.base import BaseClassifier
 from weasel.transformations.panel.dictionary_based import SFADilation
 
 
 class MUSE(BaseClassifier):
     """MUSE (MUltivariate Symbolic Extension).
 
     Also known as WEASLE-MUSE: implementation of multivariate version of WEASEL,
@@ -108,16 +108,16 @@
     - `Original Publication <https://github.com/patrickzib/SFA>`_.
     - `MUSE
         <https://github.com/uea-machine-learning/tsml/blob/master/src/main/java/tsml/
     classifiers/multivariate/WEASEL_MUSE.java>`_.
 
     Examples
     --------
-    >>> from sktime.classification.dictionary_based import MUSE
-    >>> from sktime.datasets import load_unit_test
+    >>> from aeon.classification.dictionary_based import MUSE
+    >>> from aeon.datasets import load_unit_test
     >>> X_train, y_train = load_unit_test(split="train", return_X_y=True)
     >>> X_test, y_test = load_unit_test(split="test", return_X_y=True)
     >>> clf = MUSE(window_inc=4, use_first_order_differences=False)
     >>> clf.fit(X_train, y_train)
     MUSE(...)
     >>> y_pred = clf.predict(X_test)
     """
```

### Comparing `weasel-classifier-0.1.4/weasel/classification/dictionary_based/_muse_v2.py` & `weasel-classifier-0.1.5/weasel/classification/dictionary_based/_muse_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import warnings
 
 import numpy as np
 from joblib import Parallel, delayed
 from scipy.sparse import hstack
 from sklearn.linear_model import RidgeClassifierCV
 from sklearn.utils import check_random_state
-from sktime.classification.base import BaseClassifier
+from aeon.classification.base import BaseClassifier
 
 from weasel.transformations.panel.dictionary_based import SFADilation
 
 
 class MUSE_V2(BaseClassifier):
     """MUSE (MUltivariate Symbolic Extension) v2.0.
 
@@ -85,15 +85,15 @@
 
     Notes
     -----
     
     Examples
     --------
     >>> from weasel.classification.dictionary_based import MUSE_V2
-    >>> from sktime.datasets import load_unit_test
+    >>> from aeon.datasets import load_unit_test
     >>> X_train, y_train = load_unit_test(split="train", return_X_y=True)
     >>> X_test, y_test = load_unit_test(split="test", return_X_y=True)
     >>> clf = MUSE_V2()
     >>> clf.fit(X_train, y_train)
     MUSE_V2(...)
     >>> y_pred = clf.predict(X_test)
     """
```

### Comparing `weasel-classifier-0.1.4/weasel/classification/dictionary_based/_weasel.py` & `weasel-classifier-0.1.5/weasel/classification/dictionary_based/_weasel.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,16 +110,16 @@
     For the Java version, see
     - `Original Publication <https://github.com/patrickzib/SFA>`_.
     - `TSML <https://github.com/uea-machine-learning/tsml/blob/master/src/main/java
     /tsml/classifiers/dictionary_based/WEASEL.java>`_.
 
     Examples
     --------
-    >>> from sktime.classification.dictionary_based import WEASEL
-    >>> from sktime.datasets import load_unit_test
+    >>> from aeon.classification.dictionary_based import WEASEL
+    >>> from aeon.datasets import load_unit_test
     >>> X_train, y_train = load_unit_test(split="train", return_X_y=True)
     >>> X_test, y_test = load_unit_test(split="test", return_X_y=True)
     >>> clf = WEASEL(window_inc=4)
     >>> clf.fit(X_train, y_train)
     WEASEL(...)
     >>> y_pred = clf.predict(X_test)
     """
```

### Comparing `weasel-classifier-0.1.4/weasel/classification/dictionary_based/_weasel_v2.py` & `weasel-classifier-0.1.5/weasel/classification/dictionary_based/_weasel_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __all__ = ["WEASEL_V2"]
 
 import numpy as np
 from joblib import Parallel, delayed
 from scipy.sparse import hstack
 from sklearn.linear_model import RidgeClassifierCV
 from sklearn.utils import check_random_state
-from sktime.classification.base import BaseClassifier
+from aeon.classification.base import BaseClassifier
 
 from weasel.transformations.panel.dictionary_based import SFADilation
 
 
 class WEASEL_V2(BaseClassifier):
     """Word Extraction for Time Series Classification (WEASEL) v2.0.
 
@@ -92,15 +92,15 @@
 
     Notes
     -----
     
     Examples
     --------
     >>> from weasel.classification.dictionary_based import WEASEL_V2
-    >>> from sktime.datasets import load_unit_test
+    >>> from aeon.datasets import load_unit_test
     >>> X_train, y_train = load_unit_test(split="train", return_X_y=True)
     >>> X_test, y_test = load_unit_test(split="test", return_X_y=True)
     >>> clf = WEASEL_V2()
     >>> clf.fit(X_train, y_train)
     WEASEL_V2(...)
     >>> y_pred = clf.predict(X_test)
     """
```

### Comparing `weasel-classifier-0.1.4/weasel/transformations/panel/dictionary_based/_sfa_dilation.py` & `weasel-classifier-0.1.5/weasel/transformations/panel/dictionary_based/_sfa_dilation.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 from numba.typed import Dict
 from scipy.sparse import csr_matrix, hstack
 from sklearn.feature_selection import chi2, f_classif
 from sklearn.preprocessing import KBinsDiscretizer
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.utils import check_random_state
 
-from sktime.transformations.base import BaseTransformer
-from sktime.utils.validation.panel import check_X
+from aeon.transformations.base import BaseTransformer
+from aeon.utils.validation.panel import check_X
 
 # The binning methods to use: equi-depth, equi-width, information gain or kmeans
 binning_methods = {"equi-depth", "equi-width", "information-gain", "kmeans", "quantile"}
 
 simplefilter(action="ignore", category=NumbaPendingDeprecationWarning)
 simplefilter(action="ignore", category=NumbaTypeSafetyWarning)
```

### Comparing `weasel-classifier-0.1.4/weasel_classifier.egg-info/PKG-INFO` & `weasel-classifier-0.1.5/weasel_classifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel-classifier
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Random Dilated Dictionary Transform for Fast, Accurate and Constrained Memory Time Series Classification
 Home-page: https://github.com/patrickzib/dictionary
 Author: patrickzib
 Author-email: patrickzib <void@void.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -717,15 +717,15 @@
 ![UCR_runtime](https://user-images.githubusercontent.com/7783034/214376264-7961db3b-2f24-488f-abbc-d53433ffacbc.png)
 
 
 ## Installation
 
 ### Dependencies
 ```
-sktime >= 0.13,<=0.15
+aeon >= 0.1.0
 ```
 
 # Installation
 
 The easiest is to use pip to install weasel-classifier.
 
 ## a) Install using pip
@@ -746,18 +746,18 @@
 ```
 pip install .
 ```
 
 
 ### Train a WEASEL 2.0 classifier
 
-WEASEL v2 follows the sktime pipeline.
+WEASEL v2 follows the aeon pipeline.
 
 ```python
-from sktime.datasets import load_arrow_head
+from aeon.datasets import load_arrow_head
 from weasel.classification.dictionary_based import WEASEL_V2
 
 X_train, y_train = load_arrow_head(split="train", return_type="numpy3d")
 X_test, y_test = load_arrow_head(split="test", return_type="numpy3d")
 clf = WEASEL_V2(random_state=1379, n_jobs=4)
 clf.fit(X_train,y_train)
 clf.predict(X_test)
```

### Comparing `weasel-classifier-0.1.4/weasel_classifier.egg-info/SOURCES.txt` & `weasel-classifier-0.1.5/weasel_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*


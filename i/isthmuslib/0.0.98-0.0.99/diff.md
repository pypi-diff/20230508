# Comparing `tmp/isthmuslib-0.0.98.tar.gz` & `tmp/isthmuslib-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isthmuslib-0.0.98.tar", last modified: Wed Feb  8 21:34:47 2023, max compression
+gzip compressed data, was "isthmuslib-0.0.99.tar", last modified: Tue Mar  7 23:28:18 2023, max compression
```

## Comparing `isthmuslib-0.0.98.tar` & `isthmuslib-0.0.99.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/
--rw-rw-r--   0 m         (1001) m         (1001)       79 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/AUTHORS.rst
--rw-rw-r--   0 m         (1001) m         (1001)     7504 2023-02-08 21:31:15.000000 isthmuslib-0.0.98/CHANGELOG.rst
--rw-rw-r--   0 m         (1001) m         (1001)     2422 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/CONTRIBUTING.rst
--rw-rw-r--   0 m         (1001) m         (1001)    43628 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/LICENSE
--rw-rw-r--   0 m         (1001) m         (1001)      333 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/MANIFEST.in
--rw-rw-r--   0 m         (1001) m         (1001)     3157 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/PKG-INFO
--rw-rw-r--   0 m         (1001) m         (1001)     9734 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/README.rst
-drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/ci/
--rwxrwxr-x   0 m         (1001) m         (1001)     2886 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/ci/bootstrap.py
--rw-rw-r--   0 m         (1001) m         (1001)       62 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/ci/requirements.txt
--rw-rw-r--   0 m         (1001) m         (1001)       50 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/pyproject.toml
--rw-rw-r--   0 m         (1001) m         (1001)      529 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/setup.cfg
--rwxrwxr-x   0 m         (1001) m         (1001)     2839 2023-02-08 21:34:20.000000 isthmuslib-0.0.98/setup.py
-drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/src/
-drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/src/isthmuslib/
--rw-rw-r--   0 m         (1001) m         (1001)      163 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/src/isthmuslib/__init__.py
--rw-rw-r--   0 m         (1001) m         (1001)      389 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/src/isthmuslib/__main__.py
--rw-rw-r--   0 m         (1001) m         (1001)      819 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/src/isthmuslib/cli.py
--rw-rw-r--   0 m         (1001) m         (1001)     3373 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/src/isthmuslib/config.py
--rw-rw-r--   0 m         (1001) m         (1001)     7699 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/src/isthmuslib/data_quality.py
--rw-rw-r--   0 m         (1001) m         (1001)    34538 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/src/isthmuslib/legacy.py
--rw-rw-r--   0 m         (1001) m         (1001)    28844 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/src/isthmuslib/logging.py
--rw-rw-r--   0 m         (1001) m         (1001)    32649 2023-02-01 22:19:40.000000 isthmuslib-0.0.98/src/isthmuslib/plotting.py
--rw-rw-r--   0 m         (1001) m         (1001)    38148 2023-02-08 20:45:30.000000 isthmuslib-0.0.98/src/isthmuslib/utils.py
--rw-rw-r--   0 m         (1001) m         (1001)    70540 2023-02-03 03:04:49.000000 isthmuslib-0.0.98/src/isthmuslib/vectors.py
-drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/src/isthmuslib.egg-info/
--rw-rw-r--   0 m         (1001) m         (1001)     3157 2023-02-08 21:34:47.000000 isthmuslib-0.0.98/src/isthmuslib.egg-info/PKG-INFO
--rw-rw-r--   0 m         (1001) m         (1001)      698 2023-02-08 21:34:47.000000 isthmuslib-0.0.98/src/isthmuslib.egg-info/SOURCES.txt
--rw-rw-r--   0 m         (1001) m         (1001)        1 2023-02-08 21:34:47.000000 isthmuslib-0.0.98/src/isthmuslib.egg-info/dependency_links.txt
--rw-rw-r--   0 m         (1001) m         (1001)       51 2023-02-08 21:34:47.000000 isthmuslib-0.0.98/src/isthmuslib.egg-info/entry_points.txt
--rw-rw-r--   0 m         (1001) m         (1001)        1 2023-02-08 21:31:55.000000 isthmuslib-0.0.98/src/isthmuslib.egg-info/not-zip-safe
--rw-rw-r--   0 m         (1001) m         (1001)      109 2023-02-08 21:34:47.000000 isthmuslib-0.0.98/src/isthmuslib.egg-info/requires.txt
--rw-rw-r--   0 m         (1001) m         (1001)       11 2023-02-08 21:34:47.000000 isthmuslib-0.0.98/src/isthmuslib.egg-info/top_level.txt
-drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-02-08 21:34:47.416286 isthmuslib-0.0.98/tests/
--rw-rw-r--   0 m         (1001) m         (1001)     8155 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/tests/test_utils.py
--rw-rw-r--   0 m         (1001) m         (1001)     1329 2022-12-17 22:09:46.000000 isthmuslib-0.0.98/tox.ini
+drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/
+-rw-rw-r--   0 m         (1001) m         (1001)       79 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/AUTHORS.rst
+-rw-rw-r--   0 m         (1001) m         (1001)     7714 2023-03-07 23:23:11.000000 isthmuslib-0.0.99/CHANGELOG.rst
+-rw-rw-r--   0 m         (1001) m         (1001)     2422 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/CONTRIBUTING.rst
+-rw-rw-r--   0 m         (1001) m         (1001)    43628 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/LICENSE
+-rw-rw-r--   0 m         (1001) m         (1001)      333 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/MANIFEST.in
+-rw-rw-r--   0 m         (1001) m         (1001)     3157 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/PKG-INFO
+-rw-rw-r--   0 m         (1001) m         (1001)     9734 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/README.rst
+drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/ci/
+-rwxrwxr-x   0 m         (1001) m         (1001)     2886 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/ci/bootstrap.py
+-rw-rw-r--   0 m         (1001) m         (1001)       62 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/ci/requirements.txt
+-rw-rw-r--   0 m         (1001) m         (1001)       50 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/pyproject.toml
+-rw-rw-r--   0 m         (1001) m         (1001)      529 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/setup.cfg
+-rwxrwxr-x   0 m         (1001) m         (1001)     2834 2023-03-07 23:20:33.000000 isthmuslib-0.0.99/setup.py
+drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/src/
+drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/src/isthmuslib/
+-rw-rw-r--   0 m         (1001) m         (1001)      163 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/src/isthmuslib/__init__.py
+-rw-rw-r--   0 m         (1001) m         (1001)      389 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/src/isthmuslib/__main__.py
+-rw-rw-r--   0 m         (1001) m         (1001)      819 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/src/isthmuslib/cli.py
+-rw-rw-r--   0 m         (1001) m         (1001)     3373 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/src/isthmuslib/config.py
+-rw-rw-r--   0 m         (1001) m         (1001)     7699 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/src/isthmuslib/data_quality.py
+-rw-rw-r--   0 m         (1001) m         (1001)    34538 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/src/isthmuslib/legacy.py
+-rw-rw-r--   0 m         (1001) m         (1001)    28844 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/src/isthmuslib/logging.py
+-rw-rw-r--   0 m         (1001) m         (1001)    32649 2023-02-01 22:19:40.000000 isthmuslib-0.0.99/src/isthmuslib/plotting.py
+-rw-rw-r--   0 m         (1001) m         (1001)    38148 2023-02-08 20:45:30.000000 isthmuslib-0.0.99/src/isthmuslib/utils.py
+-rw-rw-r--   0 m         (1001) m         (1001)    71125 2023-02-10 03:08:34.000000 isthmuslib-0.0.99/src/isthmuslib/vectors.py
+drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/src/isthmuslib.egg-info/
+-rw-rw-r--   0 m         (1001) m         (1001)     3157 2023-03-07 23:28:18.000000 isthmuslib-0.0.99/src/isthmuslib.egg-info/PKG-INFO
+-rw-rw-r--   0 m         (1001) m         (1001)      698 2023-03-07 23:28:18.000000 isthmuslib-0.0.99/src/isthmuslib.egg-info/SOURCES.txt
+-rw-rw-r--   0 m         (1001) m         (1001)        1 2023-03-07 23:28:18.000000 isthmuslib-0.0.99/src/isthmuslib.egg-info/dependency_links.txt
+-rw-rw-r--   0 m         (1001) m         (1001)       51 2023-03-07 23:28:18.000000 isthmuslib-0.0.99/src/isthmuslib.egg-info/entry_points.txt
+-rw-rw-r--   0 m         (1001) m         (1001)        1 2023-02-08 21:31:55.000000 isthmuslib-0.0.99/src/isthmuslib.egg-info/not-zip-safe
+-rw-rw-r--   0 m         (1001) m         (1001)       78 2023-03-07 23:28:18.000000 isthmuslib-0.0.99/src/isthmuslib.egg-info/requires.txt
+-rw-rw-r--   0 m         (1001) m         (1001)       11 2023-03-07 23:28:18.000000 isthmuslib-0.0.99/src/isthmuslib.egg-info/top_level.txt
+drwxrwxr-x   0 m         (1001) m         (1001)        0 2023-03-07 23:28:18.773590 isthmuslib-0.0.99/tests/
+-rw-rw-r--   0 m         (1001) m         (1001)     8155 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/tests/test_utils.py
+-rw-rw-r--   0 m         (1001) m         (1001)     1329 2022-12-17 22:09:46.000000 isthmuslib-0.0.99/tox.ini
```

### Comparing `isthmuslib-0.0.98/CHANGELOG.rst` & `isthmuslib-0.0.99/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -457,8 +457,14 @@
 -------------------
 
 * chore: distro stats in histogram watermark, and can mark mean & median on the plot
 
 0.0.98 (2022-02-08)
 -------------------
 
-* chore: more sophisticated utility controls
+* chore: more sophisticated utility controls
+
+0.0.99 (2022-03-07)
+-------------------
+
+* chore: deprecate some methods until their dependencies are python 3.11 compatible
+* chore: improve downsampling and resampling, including integration with some plots
```

### Comparing `isthmuslib-0.0.98/CONTRIBUTING.rst` & `isthmuslib-0.0.99/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/LICENSE` & `isthmuslib-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/PKG-INFO` & `isthmuslib-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isthmuslib
-Version: 0.0.98
+Version: 0.0.99
 Summary: Tooling for rapid data exploration, timeseries analysis, log extraction & visualization, etc
 Home-page: https://github.com/mitchellpkt/python-isthmuslib
 Author: Isthmus (Mitchell P. Krawiec-Thayer)
 Author-email: isthmuslib@mitchellpkt.com
 License: LGPL-3.0-only
 Project-URL: Changelog, https://github.com/mitchellpkt/python-isthmuslib/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/mitchellpkt/python-isthmuslib/issues
```

### Comparing `isthmuslib-0.0.98/README.rst` & `isthmuslib-0.0.99/README.rst`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/ci/bootstrap.py` & `isthmuslib-0.0.99/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/setup.cfg` & `isthmuslib-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/setup.py` & `isthmuslib-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 from setuptools import setup
 
 
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
+
 long_description_raw: str = "%s\n%s" % (
-        re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
-        re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
-    )
+    re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
+    re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
+)
 split_string: str = "Demo one-liners"
 
 setup(
     name="isthmuslib",
-    version="0.0.98",
+    version="0.0.99",
     license="LGPL-3.0-only",
     description="Tooling for rapid data exploration, timeseries analysis, log extraction & visualization, etc",
     long_description=long_description_raw.split(split_string)[0],
     author="Isthmus (Mitchell P. Krawiec-Thayer)",
     author_email="isthmuslib@mitchellpkt.com",
     url="https://github.com/mitchellpkt/python-isthmuslib",
     packages=find_packages("src"),
@@ -69,17 +70,17 @@
         "seaborn",
         "loguru",
         "pydantic",
         "statsmodels",
         "pytz",
         "pyarrow",
         "tqdm",
-        "scikit-learn",
-        "ipywidgets",
-        "stumpy",
+        # "scikit-learn",
+        # "ipywidgets",
+        # "stumpy",
     ],
     extras_require={},
     entry_points={
         "console_scripts": [
             "isthmuslib = isthmuslib.cli:main",
         ]
     },
```

### Comparing `isthmuslib-0.0.98/src/isthmuslib/cli.py` & `isthmuslib-0.0.99/src/isthmuslib/cli.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/src/isthmuslib/config.py` & `isthmuslib-0.0.99/src/isthmuslib/config.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/src/isthmuslib/data_quality.py` & `isthmuslib-0.0.99/src/isthmuslib/data_quality.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/src/isthmuslib/legacy.py` & `isthmuslib-0.0.99/src/isthmuslib/legacy.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/src/isthmuslib/logging.py` & `isthmuslib-0.0.99/src/isthmuslib/logging.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/src/isthmuslib/plotting.py` & `isthmuslib-0.0.99/src/isthmuslib/plotting.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/src/isthmuslib/utils.py` & `isthmuslib-0.0.99/src/isthmuslib/utils.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/src/isthmuslib/vectors.py` & `isthmuslib-0.0.99/src/isthmuslib/vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time as time
 from typing import List, Any, Tuple, Callable, Dict, Union, Iterable
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import stumpy
+
+# import stumpy
 from matplotlib.patches import Rectangle
 from .config import Style
 from .utils import (
     PickleUtils,
     Rosetta,
     make_dict,
     get_num_workers,
@@ -24,19 +25,19 @@
     visualize_surface,
     visualize_embedded_surface,
     visualize_hist2d,
     visualize_x_y_input_interpreter,
 )
 import pathlib
 from pydantic import BaseModel
-from sklearn.feature_selection import SelectKBest, chi2
 from tqdm.auto import tqdm
 
 # import matrixprofile
 import math
+import sys
 
 
 class SVD(BaseModel):
     u: Any
     s: Any
     vh: Any
 
@@ -376,41 +377,41 @@
             df_surface.loc[:, surface_axes_names[1]],
             c=df_surface.loc[:, z_axis_name].tolist(),
             xlabel=self.translate(surface_axes_names[0]),
             ylabel=self.translate(surface_axes_names[1]),
             colorbar_label=self.translate(z_axis_name),
         )
 
-    def feature_selection_univariate(
-        self,
-        target_feature_name: str,
-        input_feature_names: List[str] = None,
-        k_best: int = 3,
-        normalize: bool = True,
-        **kwargs,
-    ) -> any:
-        """Feature selection of k best using univariate methods.
-
-        :param target_feature_name: column name of the target feature
-        :param input_feature_names: column names of the input features
-        :param k_best: how many features to return
-        :param normalize: if True, scales input features to unit mean
-        :param kwargs: additional keyword arguments passed through to scikit-learn SelectKBest
-        :return: trimmed input feature data set
-        """
-        if not input_feature_names:
-            input_feature_names = [x for x in self.data.keys() if x != target_feature_name]
-        input_feature_data = self.data.loc[:, input_feature_names]
-        if normalize:
-            for fieldname in input_feature_data.keys():
-                std_dev: float = float(np.std(this_field_data := self.data.loc[:, fieldname]))
-                input_feature_data[fieldname] = [x / std_dev for x in this_field_data]
-
-        target_feature_data = self.data.loc[:, target_feature_name].to_numpy()
-        return SelectKBest(chi2, k=k_best).fit_transform(input_feature_data, target_feature_data, **kwargs)
+    # def feature_selection_univariate(
+    #     self,
+    #     target_feature_name: str,
+    #     input_feature_names: List[str] = None,
+    #     k_best: int = 3,
+    #     normalize: bool = True,
+    #     **kwargs,
+    # ) -> any:
+    #     """Feature selection of k best using univariate methods.
+    #
+    #     :param target_feature_name: column name of the target feature
+    #     :param input_feature_names: column names of the input features
+    #     :param k_best: how many features to return
+    #     :param normalize: if True, scales input features to unit mean
+    #     :param kwargs: additional keyword arguments passed through to scikit-learn SelectKBest
+    #     :return: trimmed input feature data set
+    #     """
+    #     if not input_feature_names:
+    #         input_feature_names = [x for x in self.data.keys() if x != target_feature_name]
+    #     input_feature_data = self.data.loc[:, input_feature_names]
+    #     if normalize:
+    #         for fieldname in input_feature_data.keys():
+    #             std_dev: float = float(np.std(this_field_data := self.data.loc[:, fieldname]))
+    #             input_feature_data[fieldname] = [x / std_dev for x in this_field_data]
+    #
+    #     target_feature_data = self.data.loc[:, target_feature_name].to_numpy()
+    #     return SelectKBest(chi2, k=k_best).fit_transform(input_feature_data, target_feature_data, **kwargs)
 
     def cast_to_numeric(
         self,
         columns: Union[List[str], str] = None,
         errors: str = "ignore",
         inplace: bool = True,
     ) -> Union[None, Any]:
@@ -550,28 +551,45 @@
         Very thin wrapper around stumpy's matrix profile method. NB: for use in MultiSet, user is responsible for order
 
         :param col_name: column name to profile
         :param window_size: sliding window size
         :param kwargs: keyword arguments for stumpy.stump()
         :return: numpy array with the profile
         """
+
+        if "stumpy" not in sys.modules:
+            try:
+                import stumpy
+            except ImportError as e:
+                raise ImportError(
+                    f"Could not import stumpy. Please install if compatible with your environment.\n{e}"
+                )
+
         return stumpy.stump(self.data.loc[:, col_name].tolist(), window_size, **kwargs)
 
     def stumpy_profile_univariate(
         self, col_name: str, window_size: int, annotate_motif: bool = True, **kwargs
     ) -> plt.Figure:
         """
         Plot of data & matrix profile (with optional annotation). NB: for use in MultiSet, user is responsible for order
 
         :param col_name: name of the column to plot
         :param window_size: sliding window size
         :param annotate_motif: whether to highlight the main motif and its nearest neighbor
         :param kwargs: keyword arguments for plots and stumpy.stump()
         :return: figure handle of the plot
         """
+        if "stumpy" not in sys.modules:
+            try:
+                import stumpy
+            except ImportError as e:
+                raise ImportError(
+                    f"Could not import stumpy. Please install if compatible with your environment.\n{e}"
+                )
+
         # Make the plot and profile
         figsize: Any = kwargs.pop("figsize", self.figsize)  # typically a 2-element tuple or list
         title: str = kwargs.pop("title", self.translate(self.name_root))
         profile: np.ndarray = self.calculate_stumpy_profile_univariate(col_name, window_size, **kwargs)
         minimum: float = float(np.nanmin(self.data.loc[:, col_name].tolist()))
         maximum: float = float(np.nanmax(self.data.loc[:, col_name].tolist()))
         fig, axs = plt.subplots(
```

### Comparing `isthmuslib-0.0.98/src/isthmuslib.egg-info/PKG-INFO` & `isthmuslib-0.0.99/src/isthmuslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isthmuslib
-Version: 0.0.98
+Version: 0.0.99
 Summary: Tooling for rapid data exploration, timeseries analysis, log extraction & visualization, etc
 Home-page: https://github.com/mitchellpkt/python-isthmuslib
 Author: Isthmus (Mitchell P. Krawiec-Thayer)
 Author-email: isthmuslib@mitchellpkt.com
 License: LGPL-3.0-only
 Project-URL: Changelog, https://github.com/mitchellpkt/python-isthmuslib/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/mitchellpkt/python-isthmuslib/issues
```

### Comparing `isthmuslib-0.0.98/src/isthmuslib.egg-info/SOURCES.txt` & `isthmuslib-0.0.99/src/isthmuslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/tests/test_utils.py` & `isthmuslib-0.0.99/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isthmuslib-0.0.98/tox.ini` & `isthmuslib-0.0.99/tox.ini`

 * *Files identical despite different names*


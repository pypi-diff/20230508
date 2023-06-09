# Comparing `tmp/read_rapidpe-0.2.0.tar.gz` & `tmp/read_rapidpe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_rapidpe-0.2.0.tar", max compression
+gzip compressed data, was "read_rapidpe-0.2.1.tar", max compression
```

## Comparing `read_rapidpe-0.2.0.tar` & `read_rapidpe-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.2.0/README.md
--rw-r--r--   0        0        0      627 2023-05-02 06:44:20.832113 read_rapidpe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      353 2023-04-16 13:12:20.078578 read_rapidpe-0.2.0/read_rapidpe/__init__.py
--rw-r--r--   0        0        0     8323 2023-05-01 03:22:06.667674 read_rapidpe-0.2.0/read_rapidpe/grid_point.py
--rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.2.0/read_rapidpe/p_astro.py
--rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.2.0/read_rapidpe/parser.py
--rw-r--r--   0        0        0     1474 2023-04-16 14:05:36.413685 read_rapidpe-0.2.0/read_rapidpe/plot.py
--rw-r--r--   0        0        0    20050 2023-05-02 05:41:52.815628 read_rapidpe-0.2.0/read_rapidpe/result.py
--rw-r--r--   0        0        0     2200 2022-11-25 08:05:18.514011 read_rapidpe-0.2.0/read_rapidpe/transform.py
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.2.1/README.md
+-rw-r--r--   0        0        0      627 2023-05-08 04:54:52.922664 read_rapidpe-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-04-16 13:12:20.078578 read_rapidpe-0.2.1/read_rapidpe/__init__.py
+-rw-r--r--   0        0        0     8684 2023-05-08 03:49:41.967860 read_rapidpe-0.2.1/read_rapidpe/grid_point.py
+-rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.2.1/read_rapidpe/p_astro.py
+-rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.2.1/read_rapidpe/parser.py
+-rw-r--r--   0        0        0     1474 2023-04-16 14:05:36.413685 read_rapidpe-0.2.1/read_rapidpe/plot.py
+-rw-r--r--   0        0        0    20331 2023-05-08 04:54:14.701270 read_rapidpe-0.2.1/read_rapidpe/result.py
+-rw-r--r--   0        0        0     2200 2022-11-25 08:05:18.514011 read_rapidpe-0.2.1/read_rapidpe/transform.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.2.1/PKG-INFO
```

### Comparing `read_rapidpe-0.2.0/README.md` & `read_rapidpe-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.2.0/pyproject.toml` & `read_rapidpe-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "read-rapidpe"
-version = "0.2.0"
+version = "0.2.1"
 description = "Read and analyse results generated by rapidpe-rift-pipe"
 authors = ["Cory Chu <cory@gwlab.page>"]
 readme = "README.md"
 packages = [{include = "read_rapidpe"}]
 homepage = "https://github.com/c0rychu/read-rapidpe"
 repository = "https://git.ligo.org/yu-kuang.chu/read-rapidpe"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.23.4"
-matplotlib = "^3.6.2"
-scipy = "^1.9.3"
+matplotlib = "^3.5.3"
+scipy = "^1.8.1"
 python-ligo-lw = "^1.8.3"
 joblib = "^1.2.0"
-lalsuite = "^7.14"
+lalsuite = "^7.11"
 h5py = "^3.8.0"
 pandas = "^2.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `read_rapidpe-0.2.0/read_rapidpe/grid_point.py` & `read_rapidpe-0.2.1/read_rapidpe/grid_point.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             self._set_intrinsic_table()
             self.extrinsic_table = {}
             self._set_extrinsic_table()
             self._fix_intrinsic_table_spin()  # a temporary solution
 
     def _set_intrinsic_table(self):
         # Maps are "rapidpe_name": "canonical_name"
+        # Ref: https://lscsoft.docs.ligo.org/pesummary/stable_docs/gw/parameters.html  # noqa E501
         intrinsic_parameter_map = {
                                     "mass1": "mass_1",
                                     "mass2": "mass_2",
                                     "spin1z": "spin_1z",
                                     "spin2z": "spin_2z",
                                     "snr": "marg_log_likelihood",
                                     "tau0": "tau0",
@@ -67,24 +68,27 @@
             self.intrinsic_table["spin_1z"] = \
                 self.extrinsic_table["spin_1z"][0:1]
             self.intrinsic_table["spin_2z"] = \
                 self.extrinsic_table["spin_2z"][0:1]
 
     def _set_extrinsic_table(self):
         # Maps are "rapidpe_name": "canonical_name"
+        # Ref: https://lscsoft.docs.ligo.org/pesummary/stable_docs/gw/parameters.html  # noqa E501
+        # sampling_function is the p_s in Eq.28 of https://arxiv.org/pdf/1502.04370.pdf  # noqa E501
         extrinsic_parameter_map = {
                                     "mass1": "mass_1",
                                     "mass2": "mass_2",
                                     "spin1z": "spin_1z",
                                     "spin2z": "spin_2z",
                                     "distance": "luminosity_distance",
                                     "latitude": "dec",
                                     "longitude": "ra",
                                     "inclination": "iota",
                                     "polarization": "psi",
+                                    "coa_phase": "coa_phase",
                                     "alpha1": "log_likelihood",
                                     "alpha2": "prior",
                                     "alpha3": "sampling_function",
                                 }
         self.extrinsic_table = {}
         for key in extrinsic_parameter_map:
             try:
```

### Comparing `read_rapidpe-0.2.0/read_rapidpe/p_astro.py` & `read_rapidpe-0.2.1/read_rapidpe/p_astro.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.2.0/read_rapidpe/parser.py` & `read_rapidpe-0.2.1/read_rapidpe/parser.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.2.0/read_rapidpe/plot.py` & `read_rapidpe-0.2.1/read_rapidpe/plot.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.2.0/read_rapidpe/result.py` & `read_rapidpe-0.2.1/read_rapidpe/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Read and parse RapidPE output result for post-processing.
 Author: Cory Chu <cory@gwlab.page>
 """
 
+from functools import cached_property
 from pathlib import Path
 from joblib import Parallel, delayed
 import re
 import numpy as np
 import h5py
 import pandas as pd
 from .grid_point import RapidPE_grid_point
@@ -93,14 +94,22 @@
             # self.mass_1 = result.mass_1
             # self.mass_2 = result.mass_2
             # self.spin_1z = result.spin_1z
             # self.spin_2z = result.spin_2z
             # self.marg_log_likelihood = result.marg_log_likelihood
             # ...
 
+    @cached_property
+    def extrinsic_samples(self):
+        """
+        Combine extrinsic samples to a single padas.DataFrame
+        """
+        return pd.concat(
+             [pd.DataFrame(gp.extrinsic_table) for gp in self.grid_points])
+
     def __copy__(self):
         return RapidPE_result(self)
 
     def copy(self):
         return self.__copy__()
 
     @classmethod
```

### Comparing `read_rapidpe-0.2.0/read_rapidpe/transform.py` & `read_rapidpe-0.2.1/read_rapidpe/transform.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.2.0/PKG-INFO` & `read_rapidpe-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: read-rapidpe
-Version: 0.2.0
+Version: 0.2.1
 Summary: Read and analyse results generated by rapidpe-rift-pipe
 Home-page: https://github.com/c0rychu/read-rapidpe
 Author: Cory Chu
 Author-email: cory@gwlab.page
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
-Requires-Dist: lalsuite (>=7.14,<8.0)
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
+Requires-Dist: lalsuite (>=7.11,<8.0)
+Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-ligo-lw (>=1.8.3,<2.0.0)
-Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Project-URL: Repository, https://git.ligo.org/yu-kuang.chu/read-rapidpe
 Description-Content-Type: text/markdown
 
 Read Rapid-PE
 ===
 
 This is a package to read Rapid-PE outputs.
```


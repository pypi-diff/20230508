# Comparing `tmp/PyExpUtils-andnp-3.4.0.tar.gz` & `tmp/PyExpUtils-andnp-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyExpUtils-andnp-3.4.0.tar", last modified: Fri Mar 10 22:09:08 2023, max compression
+gzip compressed data, was "PyExpUtils-andnp-4.0.0.tar", last modified: Mon May  8 20:25:25 2023, max compression
```

## Comparing `PyExpUtils-andnp-3.4.0.tar` & `PyExpUtils-andnp-4.0.0.tar`

### file list

```diff
@@ -1,68 +1,60 @@
--rw-r--r--   0        0        0     1011 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/FileSystemContext.py
--rw-r--r--   0        0        0      119 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/__init__.py
--rw-r--r--   0        0        0     1207 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/models/Config.py
--rw-r--r--   0        0        0     7915 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/models/ExperimentDescription.py
--rw-r--r--   0        0        0       87 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/py.typed
--rw-r--r--   0        0        0     4235 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/Collection.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/backends/__init__.py
--rw-r--r--   0        0        0     5485 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/backends/backend.py
--rw-r--r--   0        0        0     6430 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/backends/csv.py
--rw-r--r--   0        0        0     6186 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/backends/h5.py
--rw-r--r--   0        0        0     7798 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/backends/pandas.py
--rw-r--r--   0        0        0      510 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/indices.py
--rw-r--r--   0        0        0     7465 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/results.py
--rw-r--r--   0        0        0     1070 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/tools.py
--rw-r--r--   0        0        0    10026 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/results/voting.py
--rw-r--r--   0        0        0      815 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/runner/Args.py
--rw-r--r--   0        0        0     3225 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/runner/Slurm.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/runner/__init__.py
--rw-r--r--   0        0        0      742 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/runner/parallel.py
--rw-r--r--   0        0        0     2826 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/Collector.py
--rw-r--r--   0        0        0     3030 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/NestedDict.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/__init__.py
--rw-r--r--   0        0        0     3432 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/arrays.py
--rw-r--r--   0        0        0      403 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/asyncio.py
--rw-r--r--   0        0        0      595 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/cache.py
--rw-r--r--   0        0        0      325 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/cmdline.py
--rw-r--r--   0        0        0     1233 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/csv.py
--rw-r--r--   0        0        0     3547 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/dict.py
--rw-r--r--   0        0        0     1266 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/fp.py
--rw-r--r--   0        0        0      921 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/generator.py
--rw-r--r--   0        0        0      476 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/jit.py
--rw-r--r--   0        0        0     1218 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/path.py
--rw-r--r--   0        0        0     3454 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/permute.py
--rw-r--r--   0        0        0     1046 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/random.py
--rw-r--r--   0        0        0      278 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/str.py
--rw-r--r--   0        0        0      439 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/PyExpUtils/utils/types.py
--rw-r--r--   0        0        0    13379 2023-03-10 22:08:26.855147 PyExpUtils-andnp-3.4.0/README.md
--rw-r--r--   0        0        0     1036 2023-03-10 22:09:07.125573 PyExpUtils-andnp-3.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/__init__.py
--rw-r--r--   0        0        0      214 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/_utils/pandas.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/models/__init__.py
--rw-r--r--   0        0        0     5461 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/models/test_ExperimentDescription.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/__init__.py
--rw-r--r--   0        0        0     1827 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/test_Collection.py
--rw-r--r--   0        0        0     4784 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/test_h5.py
--rw-r--r--   0        0        0      898 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/test_indices.py
--rw-r--r--   0        0        0     9122 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/test_pandas.py
--rw-r--r--   0        0        0     4499 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/test_results.py
--rw-r--r--   0        0        0     2010 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/test_tools.py
--rw-r--r--   0        0        0     8723 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/results/test_voting.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/runner/__init__.py
--rw-r--r--   0        0        0      385 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/runner/test_parallel.py
--rw-r--r--   0        0        0      860 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/runner/test_slurm.py
--rw-r--r--   0        0        0     2278 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/test_FileSystemContext.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     3210 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_Collector.py
--rw-r--r--   0        0        0     4023 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_arrays.py
--rw-r--r--   0        0        0      881 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_cmdline.py
--rw-r--r--   0        0        0     1911 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_csv.py
--rw-r--r--   0        0        0     5882 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_dict.py
--rw-r--r--   0        0        0      586 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_generator.py
--rw-r--r--   0        0        0     1685 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_path.py
--rw-r--r--   0        0        0     3725 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_permute.py
--rw-r--r--   0        0        0     1591 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_random.py
--rw-r--r--   0        0        0      365 2023-03-10 22:08:26.859147 PyExpUtils-andnp-3.4.0/tests/utils/test_str.py
--rw-r--r--   0        0        0    13632 1970-01-01 00:00:00.000000 PyExpUtils-andnp-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1011 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/FileSystemContext.py
+-rw-r--r--   0        0        0      119 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/__init__.py
+-rw-r--r--   0        0        0     1207 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/models/Config.py
+-rw-r--r--   0        0        0     7915 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/models/ExperimentDescription.py
+-rw-r--r--   0        0        0       87 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/py.typed
+-rw-r--r--   0        0        0     3110 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/Collection.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/__init__.py
+-rw-r--r--   0        0        0      510 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/indices.py
+-rw-r--r--   0        0        0     7798 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/pandas.py
+-rw-r--r--   0        0        0     1070 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/tools.py
+-rw-r--r--   0        0        0     8921 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/voting.py
+-rw-r--r--   0        0        0     5211 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/Slurm.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/parallel.py
+-rw-r--r--   0        0        0     1450 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/utils.py
+-rw-r--r--   0        0        0     2826 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/Collector.py
+-rw-r--r--   0        0        0     3030 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/NestedDict.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/__init__.py
+-rw-r--r--   0        0        0     3432 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/arrays.py
+-rw-r--r--   0        0        0      403 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/asyncio.py
+-rw-r--r--   0        0        0      595 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/cache.py
+-rw-r--r--   0        0        0      368 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/cmdline.py
+-rw-r--r--   0        0        0     1233 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/csv.py
+-rw-r--r--   0        0        0     3547 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/dict.py
+-rw-r--r--   0        0        0     1266 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/fp.py
+-rw-r--r--   0        0        0      921 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/generator.py
+-rw-r--r--   0        0        0      476 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/jit.py
+-rw-r--r--   0        0        0     1218 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/path.py
+-rw-r--r--   0        0        0     3454 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/permute.py
+-rw-r--r--   0        0        0     1046 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/random.py
+-rw-r--r--   0        0        0      278 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/str.py
+-rw-r--r--   0        0        0      439 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/types.py
+-rw-r--r--   0        0        0     6884 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/README.md
+-rw-r--r--   0        0        0     1036 2023-05-08 20:25:24.334010 PyExpUtils-andnp-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/_utils/pandas.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/models/__init__.py
+-rw-r--r--   0        0        0     5461 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/models/test_ExperimentDescription.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/__init__.py
+-rw-r--r--   0        0        0      898 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_indices.py
+-rw-r--r--   0        0        0     9113 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_pandas.py
+-rw-r--r--   0        0        0     2010 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_tools.py
+-rw-r--r--   0        0        0     8723 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_voting.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/runner/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/runner/test_parallel.py
+-rw-r--r--   0        0        0      987 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/runner/test_slurm.py
+-rw-r--r--   0        0        0     2278 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/test_FileSystemContext.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3210 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_Collector.py
+-rw-r--r--   0        0        0     4023 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_arrays.py
+-rw-r--r--   0        0        0      881 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_cmdline.py
+-rw-r--r--   0        0        0     1911 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_csv.py
+-rw-r--r--   0        0        0     5882 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_dict.py
+-rw-r--r--   0        0        0      586 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_generator.py
+-rw-r--r--   0        0        0     1685 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_path.py
+-rw-r--r--   0        0        0     3725 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_permute.py
+-rw-r--r--   0        0        0     1591 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_random.py
+-rw-r--r--   0        0        0      365 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_str.py
+-rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 PyExpUtils-andnp-4.0.0/PKG-INFO
```

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/FileSystemContext.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/FileSystemContext.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/models/Config.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/models/Config.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/models/ExperimentDescription.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/models/ExperimentDescription.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/results/Collection.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/results/Collection.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from __future__ import annotations
 import os
 import glob
 import importlib
 import pandas as pd
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Type, overload
-from PyExpUtils.utils.dict import flatKeys, get
+from typing import Any, Callable, Dict, List, Optional, Type, overload
 from PyExpUtils.utils.NestedDict import NestedDict
 from PyExpUtils.utils.permute import set_at_path
 from PyExpUtils.models.ExperimentDescription import ExperimentDescription, loadExperiment
-from PyExpUtils.results.backends.pandas import loadResults
-from PyExpUtils.results.results import ResultList
+from PyExpUtils.results.pandas import loadResults
 
-RList = TypeVar('RList', bound=ResultList)
 class ResultCollection(NestedDict[str, pd.DataFrame]):
     def __init__(self, Model: Optional[Type[ExperimentDescription]] = None):
         super().__init__(depth=2)
 
         self._data: Dict[str, Dict[str, pd.DataFrame]] = {}
         self._Model = Model
 
@@ -49,45 +46,16 @@
             paths = exp_files[domain]
             for p in paths:
                 alg = p.split('/')[-1].replace('.json', '')
 
                 exp = loadExperiment(p, Model)
                 df = loadResults(exp, file)
 
-                out[domain, alg] = df
-
-        return out
-
-    @classmethod
-    def fromResults(cls, env_alg_result: NestedDict[str, RList]) -> ResultCollection:
-        out = cls()
-
-        for domain, alg in env_alg_result:
-            results = env_alg_result[domain, alg]
-            results = list(results)
-            exp = results[0].exp
-            idx = results[0].idx
-
-            params = exp.getPermutation(idx)['metaParameters']
-            keys = flatKeys(params)
-            header = sorted(keys)
-
-            # avoid having to construct a list by appending
-            def _rowBuilder():
-                for r in results:
-                    pvalues = [get(r.params, k) for k in header]
-                    for run, data in enumerate(r.load()):
-                        if not isinstance(data, list):
-                            data = [data]
-
-                        yield pvalues + [run] + list(data)
-
-            rows = list(_rowBuilder())
-
-            out[domain, alg] = pd.DataFrame(rows, columns=header + ['run', 'data'])
+                if df is not None:
+                    out[domain, alg] = df
 
         return out
 
 @overload
 def findExperiments(key: str, path: Optional[str] = None) -> Dict[str, Any]: ...
 @overload
 def findExperiments() -> List[str]: ...
```

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/results/backends/pandas.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/results/pandas.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/results/tools.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/results/tools.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/results/voting.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/results/voting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from PyExpUtils.utils.dict import pick
-from copy import deepcopy
 import numpy as np
-from PyExpUtils.models.ExperimentDescription import ExperimentDescription
-from PyExpUtils.results.results import ResultList, Reducer, whereParametersEqual
+from copy import deepcopy
 from PyExpUtils.utils.types import T
 from PyExpUtils.utils.jit import try2jit
 from typing import Dict, List, NamedTuple, Tuple, Union, cast
 
 Name = Union[int, str]
 
 class ScoredCandidate(NamedTuple):
@@ -18,40 +15,14 @@
     stderr: float
 
 class RankedCandidate(NamedTuple):
     name: Name
     rank: int
     score: float = 0
 
-def scoreMetaparameters(results: ResultList, exp: ExperimentDescription, reducer: Reducer = lambda x: float(np.mean(x))):
-    # gotta cache the results
-    all_results = list(results)
-
-    all_scores: List[ScoredCandidate] = []
-    for i in range(exp.numPermutations()):
-        params = pick(exp.getPermutation(i), exp.getKeys())
-        results = whereParametersEqual(all_results, params)
-        results = list(results)
-
-        # if data is missing, then mark the score as nan
-        # different ranking methods might handle these nans differently so defer to them
-        if len(results) == 0:
-            all_scores.append(ScoredCandidate(i, np.nan, np.nan))
-            continue
-
-        # there should only be one result
-        r = results[0]
-
-        point = reducer(r.mean())
-        stderr = reducer(r.stderr())
-
-        all_scores.append(ScoredCandidate(i, point, stderr))
-
-    return all_scores
-
 def confidenceInterval(scored: ScoredCandidate, c: float):
     lo = scored.score - c * scored.stderr
     hi = scored.score + c * scored.stderr
 
     return (lo, hi)
 
 def inRange(a: Tuple[float, float], b: Tuple[float, float]):
```

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/runner/parallel.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/runner/parallel.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/Collector.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/Collector.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/NestedDict.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/NestedDict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/arrays.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/cache.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/cache.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/csv.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/csv.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/dict.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/dict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/fp.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/fp.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/generator.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/generator.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/path.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/path.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/permute.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/permute.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/PyExpUtils/utils/random.py` & `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/random.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/pyproject.toml` & `PyExpUtils-andnp-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.4.0"
+version = "4.0.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -26,15 +26,15 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "PyExpUtils-andnp"
-version = "3.4.0"
+version = "4.0.0"
 description = "A small set of utilities for RL and ML experiments"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.52.0",
     "numpy>=1.21.5",
```

### Comparing `PyExpUtils-andnp-3.4.0/tests/models/test_ExperimentDescription.py` & `PyExpUtils-andnp-4.0.0/tests/models/test_ExperimentDescription.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/results/test_indices.py` & `PyExpUtils-andnp-4.0.0/tests/results/test_indices.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/results/test_pandas.py` & `PyExpUtils-andnp-4.0.0/tests/results/test_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 import shutil
 import os
-import PyExpUtils.results.backends.pandas as PDBackend
+import PyExpUtils.results.pandas as PDBackend
 from PyExpUtils.results.tools import collapseRuns
 from PyExpUtils.models.ExperimentDescription import ExperimentDescription
 import unittest
 import pandas as pd
 import numpy as np
 
 from PyExpUtils.utils.Collector import Collector
```

### Comparing `PyExpUtils-andnp-3.4.0/tests/results/test_tools.py` & `PyExpUtils-andnp-4.0.0/tests/results/test_tools.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/results/test_voting.py` & `PyExpUtils-andnp-4.0.0/tests/results/test_voting.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/runner/test_slurm.py` & `PyExpUtils-andnp-4.0.0/tests/runner/test_slurm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import unittest
-from PyExpUtils.runner.Slurm import Options
+from PyExpUtils.runner.Slurm import MultiNodeOptions, SingleNodeOptions, to_cmdline_flags
 
 class TestSlurm(unittest.TestCase):
     def test_Options(self):
-        opts = Options({
-            'account': 'def-whitem',
-            'time': '2:59:59',
-            'cores': 1,
-            'memPerCpu': '4G',
-            'sequential': 30,
-        })
+        opts = SingleNodeOptions(
+            account='def-whitem',
+            time='2:59:59',
+            cores=2,
+            mem_per_core=4,
+            sequential=30,
+        )
 
-        got = opts.cmdArgs()
-        expected = '--account=def-whitem --time=2:59:59 --ntasks=1 --mem-per-cpu=4G --output=$SCRATCH/job_output_%j.txt'
+        got = to_cmdline_flags(opts)
+        expected = '--account=def-whitem --mem-per-cpu=4096M --nodes=1 --ntasks=1 --ntasks-per-node=2 --output=$SCRATCH/job_output_%j.txt --time=2:59:59'
         self.assertEqual(got, expected)
 
-        opts = Options({
-            'account': 'def-whitem',
-            'time': '2:59:59',
-            'nodes': 1,
-            'coresPerNode': 40,
-        })
+        opts = MultiNodeOptions(
+            account='def-whitem',
+            time='2:59:59',
+            cores=8,
+            mem_per_core=4,
+            sequential=30,
+        )
 
-        got = opts.cmdArgs()
-        expected = '--account=def-whitem --time=2:59:59 --nodes=1 --ntasks-per-node=40 --output=$SCRATCH/job_output_%j.txt'
+        got = to_cmdline_flags(opts)
+        expected = '--account=def-whitem --cpus-per-task=1 --mem-per-cpu=4096M --ntasks=8 --output=$SCRATCH/job_output_%j.txt --time=2:59:59'
         self.assertEqual(got, expected)
```

### Comparing `PyExpUtils-andnp-3.4.0/tests/test_FileSystemContext.py` & `PyExpUtils-andnp-4.0.0/tests/test_FileSystemContext.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_Collector.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_Collector.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_arrays.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_arrays.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_cmdline.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_cmdline.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         pairs = [
             ('--test', 'a'),
             ('--trial', 'b'),
             ('--exam', 'c'),
         ]
 
         got = flagString(pairs)
-        expected = '--test=a --trial=b --exam=c'
+        expected = '--exam=c --test=a --trial=b'
 
         self.assertEqual(got, expected)
 
         # removes None entries
         pairs = [
             ('--test', 'a'),
             ('--exam', None),
@@ -29,10 +29,10 @@
         # can join arguments with arbitrary string
         pairs = [
             ('--test', 'a'),
             ('--exam', 'b'),
         ]
 
         got = flagString(pairs, ' ')
-        expected = '--test a --exam b'
+        expected = '--exam b --test a'
 
         self.assertEqual(got, expected)
```

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_csv.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_csv.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_dict.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_generator.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_generator.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_path.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_permute.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_permute.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-3.4.0/tests/utils/test_random.py` & `PyExpUtils-andnp-4.0.0/tests/utils/test_random.py`

 * *Files identical despite different names*


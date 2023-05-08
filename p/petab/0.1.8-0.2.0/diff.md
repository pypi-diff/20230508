# Comparing `tmp/petab-0.1.8.tar.gz` & `tmp/petab-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/petab-0.1.8.tar", last modified: Thu Jul 23 15:13:47 2020, max compression
+gzip compressed data, was "petab-0.2.0.tar", last modified: Mon May  8 15:43:50 2023, max compression
```

## Comparing `petab-0.1.8.tar` & `petab-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-23 15:13:47.000000 petab-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-23 15:13:47.000000 petab-0.1.8/petab/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-23 15:13:47.000000 petab-0.1.8/petab/visualize/
--rw-r--r--   0 runner    (1001) docker     (116)     6778 2020-07-23 15:13:35.000000 petab-0.1.8/petab/visualize/plotting_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    37339 2020-07-23 15:13:35.000000 petab-0.1.8/petab/visualize/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    10015 2020-07-23 15:13:35.000000 petab-0.1.8/petab/visualize/plot_data_and_simulation.py
--rw-r--r--   0 runner    (1001) docker     (116)      458 2020-07-23 15:13:35.000000 petab-0.1.8/petab/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3109 2020-07-23 15:13:35.000000 petab-0.1.8/petab/visualize/data_overview.py
--rw-r--r--   0 runner    (1001) docker     (116)    13297 2020-07-23 15:13:35.000000 petab-0.1.8/petab/sbml.py
--rw-r--r--   0 runner    (1001) docker     (116)     3915 2020-07-23 15:13:35.000000 petab-0.1.8/petab/C.py
--rw-r--r--   0 runner    (1001) docker     (116)     5072 2020-07-23 15:13:35.000000 petab-0.1.8/petab/observables.py
--rw-r--r--   0 runner    (1001) docker     (116)    30190 2020-07-23 15:13:35.000000 petab-0.1.8/petab/lint.py
--rw-r--r--   0 runner    (1001) docker     (116)    14667 2020-07-23 15:13:35.000000 petab-0.1.8/petab/core.py
--rw-r--r--   0 runner    (1001) docker     (116)     7068 2020-07-23 15:13:35.000000 petab-0.1.8/petab/yaml.py
--rw-r--r--   0 runner    (1001) docker     (116)       55 2020-07-23 15:13:35.000000 petab-0.1.8/petab/format_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     3466 2020-07-23 15:13:35.000000 petab-0.1.8/petab/sampling.py
--rw-r--r--   0 runner    (1001) docker     (116)    12741 2020-07-23 15:13:35.000000 petab-0.1.8/petab/calculate.py
--rw-r--r--   0 runner    (1001) docker     (116)    15373 2020-07-23 15:13:35.000000 petab-0.1.8/petab/parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    24306 2020-07-23 15:13:35.000000 petab-0.1.8/petab/problem.py
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-07-23 15:13:35.000000 petab-0.1.8/petab/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     2652 2020-07-23 15:13:35.000000 petab-0.1.8/petab/composite_problem.py
--rw-r--r--   0 runner    (1001) docker     (116)    10983 2020-07-23 15:13:35.000000 petab-0.1.8/petab/measurements.py
--rw-r--r--   0 runner    (1001) docker     (116)     3030 2020-07-23 15:13:35.000000 petab-0.1.8/petab/conditions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2020-07-23 15:13:35.000000 petab-0.1.8/petab/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6170 2020-07-23 15:13:35.000000 petab-0.1.8/petab/petablint.py
--rw-r--r--   0 runner    (1001) docker     (116)    23293 2020-07-23 15:13:35.000000 petab-0.1.8/petab/parameter_mapping.py
--rw-r--r--   0 runner    (1001) docker     (116)     2469 2020-07-23 15:13:35.000000 petab-0.1.8/petab/petab_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    11452 2020-07-23 15:13:47.000000 petab-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-23 15:13:47.000000 petab-0.1.8/petab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      742 2020-07-23 15:13:47.000000 petab-0.1.8/petab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)    11452 2020-07-23 15:13:46.000000 petab-0.1.8/petab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       52 2020-07-23 15:13:46.000000 petab-0.1.8/petab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      164 2020-07-23 15:13:46.000000 petab-0.1.8/petab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-23 15:13:46.000000 petab-0.1.8/petab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-07-23 15:13:46.000000 petab-0.1.8/petab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-07-23 15:13:35.000000 petab-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-23 15:13:47.000000 petab-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     9435 2020-07-23 15:13:35.000000 petab-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     2274 2020-07-23 15:13:35.000000 petab-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 15:43:41.000000 petab-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 15:43:41.000000 petab-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 15:43:50.778574 petab-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-08 15:43:41.000000 petab-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-08 15:43:41.000000 petab-0.2.0/petab/C.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-08 15:43:41.000000 petab-0.2.0/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-08 15:43:41.000000 petab-0.2.0/petab/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-08 15:43:41.000000 petab-0.2.0/petab/composite_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-08 15:43:41.000000 petab-0.2.0/petab/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-05-08 15:43:41.000000 petab-0.2.0/petab/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 15:43:41.000000 petab-0.2.0/petab/format_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38465 2023-05-08 15:43:41.000000 petab-0.2.0/petab/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-08 15:43:41.000000 petab-0.2.0/petab/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-08 15:43:41.000000 petab-0.2.0/petab/measurements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/pysb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/sbml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-08 15:43:41.000000 petab-0.2.0/petab/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-05-08 15:43:41.000000 petab-0.2.0/petab/parameter_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-05-08 15:43:41.000000 petab-0.2.0/petab/parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4855 2023-05-08 15:43:41.000000 petab-0.2.0/petab/petablint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33069 2023-05-08 15:43:41.000000 petab-0.2.0/petab/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-08 15:43:41.000000 petab-0.2.0/petab/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-08 15:43:41.000000 petab-0.2.0/petab/sbml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-08 15:43:41.000000 petab-0.2.0/petab/schemas/petab_schema.v1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-08 15:43:41.000000 petab-0.2.0/petab/schemas/petab_schema.v2.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-08 15:43:41.000000 petab-0.2.0/petab/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-08 15:43:41.000000 petab-0.2.0/petab/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 15:43:41.000000 petab-0.2.0/petab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/data_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plot_data_and_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plot_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/visualize/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/templates/mystyle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-08 15:43:41.000000 petab-0.2.0/petab/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 15:43:41.000000 petab-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:43:50.778574 petab-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-08 15:43:41.000000 petab-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `petab-0.1.8/petab/visualize/helper_functions.py` & `petab-0.2.0/petab/visualize/plotting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,909 +1,1004 @@
-"""
-This file should contain the functions, which PEtab internally needs for
-plotting, but which are not meant to be used by non-developers and should
-hence not be directly visible/usable when using `import petab.visualize`.
-"""
-
-import functools
+"""PEtab visualization data selection and visualization settings classes"""
 import warnings
-from numbers import Number
-
+from numbers import Number, Real
+from pathlib import Path
+from typing import Dict, List, Optional, Tuple, Union, Literal
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import petab
-import seaborn as sns
 
-from .plotting_config import plot_lowlevel
+from .helper_functions import (create_dataset_id_list_new,
+                               generate_dataset_id_col)
+from .. import conditions, core, measurements
 from ..C import *
+from ..problem import Problem
 
-from typing import Dict, List, Optional, Tuple, Union
-
-sns.set()
+__all__ = ['DataSeries', 'DataPlot', 'Subplot', 'Figure', 'DataProvider',
+           'VisSpecParser']
 
 # for typehints
 IdsList = List[str]
 NumList = List[int]
 
 
-def import_from_files(
-        data_file_path: str,
-        condition_file_path: str,
-        simulation_file_path: str,
-        dataset_id_list: List[IdsList],
-        sim_cond_id_list: List[IdsList],
-        sim_cond_num_list: List[NumList],
-        observable_id_list: List[IdsList],
-        observable_num_list: List[NumList],
-        plotted_noise: str,
-        visualization_file_path: str = None
-) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
-    """
-    Helper function for plotting data and simulations, which imports data
-    from PEtab files. If `visualization_file_path` is not provided, the
-    visualisation specification DataFrame will be generated automatically.
-
-    For documentation, see main function plot_data_and_simulation()
-
-    Returns:
-        A tuple of experimental data, experimental conditions,
-        visualization specification and simulation data DataFrames.
-    """
-
-    # import measurement data and experimental condition
-    exp_data = petab.get_measurement_df(data_file_path)
-    exp_conditions = petab.get_condition_df(condition_file_path)
-
-    # import visualization specification, if file was specified
-    if visualization_file_path:
-        vis_spec = petab.get_visualization_df(visualization_file_path)
-    else:
-        # create them based on simulation conditions
-        vis_spec, exp_data = get_default_vis_specs(exp_data,
-                                                   exp_conditions,
-                                                   dataset_id_list,
-                                                   sim_cond_id_list,
-                                                   sim_cond_num_list,
-                                                   observable_id_list,
-                                                   observable_num_list,
-                                                   plotted_noise)
-
-    # import simulation file, if file was specified
-    if simulation_file_path != '':
-        sim_data = petab.get_simulation_df(simulation_file_path)
-    else:
-        sim_data = None
-
-    return exp_data, exp_conditions, vis_spec, sim_data
-
-
-def check_vis_spec_consistency(
-        exp_data: pd.DataFrame,
-        dataset_id_list: Optional[List[IdsList]] = None,
-        sim_cond_id_list: Optional[List[IdsList]] = None,
-        sim_cond_num_list: Optional[List[NumList]] = None,
-        observable_id_list: Optional[List[IdsList]] = None,
-        observable_num_list: Optional[List[NumList]] = None) -> str:
-    """
-    Helper function for plotting data and simulations, which checks the
-    visualization setting, if no visualization specification file is provided.
+# also for type hints
+# TODO: split into dataplot and subplot level dicts?
+# TODO: add when only python>=3.8 is supported
+# class VisDict(TypedDict):
+#     PLOT_NAME: str
+#     PLOT_TYPE_SIMULATION: str
+#     PLOT_TYPE_DATA: str
+#     X_VALUES: str
+#     X_OFFSET: List[Number]
+#     X_LABEL: str
+#     X_SCALE: str
+#     Y_VALUES: List[str]
+#     Y_OFFSET: List[Number]
+#     Y_LABEL: str
+#     Y_SCALE: str
+#     LEGEND_ENTRY: List[Number]
+#     DATASET_ID: List[str]
+
+
+class DataSeries:
+    """
+    Data for one individual line
+    """
+    def __init__(self, conditions_: Optional[Union[np.ndarray, pd.Series]],
+                 data_to_plot: Optional[pd.DataFrame] = None):
+
+        self.data_to_plot = data_to_plot
+        self.data_to_plot.sort_index(inplace=True)
+
+        self.conditions = conditions_
+        self.inf_point = np.inf in self.conditions if \
+            self.conditions is not None else False
+        # sort index for the case that indices of conditions and
+        # measurements differ. if indep_var='time', conditions is a
+        # numpy array, if indep_var=observable it's a Series
+        if isinstance(self.conditions, np.ndarray):
+            self.conditions.sort()
+        elif isinstance(self.conditions, pd.Series):
+            self.conditions.sort_index(inplace=True)
+
+    def add_x_offset(self, offset) -> None:
+        """
+        Offset for the independent variable.
+
+        Parameters
+        ----------
+        offset:
+            Offset value.
+
+        """
+        if self.conditions is not None:
+            self.conditions += offset
+
+    def add_y_offset(self, offset):
+        self.data_to_plot['mean'] += offset
+        self.data_to_plot['repl'] += offset
+
+    def add_offsets(self, x_offset=0, y_offset=0) -> None:
+        """
+        Data offsets.
+
+        Parameters
+        ----------
+        x_offset:
+            Offset for the independent variable.
+        y_offset:
+            Offsets for the observable.
+        """
+        self.add_x_offset(x_offset)
+        self.add_y_offset(y_offset)
+
+
+class DataPlot:
+    """
+    Visualization specification of a plot of one data series, e.g. for
+    an individual line on a subplot.
+    """
+    def __init__(self,
+                 plot_settings: dict):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        plot_settings: A plot spec for one dataplot
+            (only VISUALIZATION_DF_SINGLE_PLOT_LEVEL_COLS)
+        """
+
+        for key, val in plot_settings.items():
+            setattr(self, key, val)
+
+        if DATASET_ID not in vars(self):
+            raise ValueError(f'{DATASET_ID} must be specified')
+        if X_VALUES not in vars(self):  # TODO: singular?
+            setattr(self, X_VALUES, TIME)
+        if X_OFFSET not in vars(self):
+            setattr(self, X_OFFSET, 0)
+        if Y_VALUES not in vars(self):
+            setattr(self, Y_VALUES, '')
+        if Y_OFFSET not in vars(self):
+            setattr(self, Y_OFFSET, 0.)
+        if LEGEND_ENTRY not in vars(self):
+            setattr(self, LEGEND_ENTRY, getattr(self, DATASET_ID))
+
+    @classmethod
+    def from_df(cls, plot_spec: pd.DataFrame):
+
+        vis_spec_dict = plot_spec.to_dict()
+
+        return cls(vis_spec_dict)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}({self.__dict__})"
+
+
+class Subplot:
+    """
+    Visualization specification of a subplot.
+    """
+    def __init__(self,
+                 plot_id: str,
+                 plot_settings: dict,
+                 dataplots: Optional[List[DataPlot]] = None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        plot_id:
+            Plot ID.
+        plot_settings:
+            Plot spec for a subplot (only VISUALIZATION_DF_SUBPLOT_LEVEL_COLS).
+        dataplots:
+            A list of data plots that should be plotted on one subplot.
+        """
+        # parameters of a specific subplot
+
+        setattr(self, PLOT_ID, plot_id)
+        for key, val in plot_settings.items():
+            setattr(self, key, val)
+
+        if PLOT_NAME not in vars(self):
+            setattr(self, PLOT_NAME, '')
+        if PLOT_TYPE_SIMULATION not in vars(self):
+            setattr(self, PLOT_TYPE_SIMULATION, LINE_PLOT)
+        if PLOT_TYPE_DATA not in vars(self):
+            setattr(self, PLOT_TYPE_DATA, MEAN_AND_SD)
+        if X_LABEL not in vars(self):
+            setattr(self, X_LABEL, TIME)  # TODO: getattr(self, X_VALUES)
+        if X_SCALE not in vars(self):
+            setattr(self, X_SCALE, LIN)
+        if Y_LABEL not in vars(self):
+            setattr(self, Y_LABEL, 'values')
+        if Y_SCALE not in vars(self):
+            setattr(self, Y_SCALE, LIN)
+
+        self.data_plots = dataplots if dataplots is not None else []
+        self.xlim = None
+        self.ylim = None
+
+    @classmethod
+    def from_df(cls, plot_id: str, vis_spec: pd.DataFrame,
+                dataplots: Optional[List[DataPlot]] = None):
+
+        vis_spec_dict = {}
+        for col in vis_spec:
+            if col in VISUALIZATION_DF_SUBPLOT_LEVEL_COLS:
+                entry = vis_spec.loc[:, col]
+                entry = np.unique(entry)
+                if entry.size > 1:
+                    warnings.warn(f'For {PLOT_ID} {plot_id} in column '
+                                  f'{col} contradictory settings ({entry})'
+                                  f'. Proceeding with first entry '
+                                  f'({entry[0]}).')
+                entry = entry[0]
+
+                # check if values are allowed
+                if col in [Y_SCALE, X_SCALE] and entry not in \
+                        OBSERVABLE_TRANSFORMATIONS:
+                    raise ValueError(f'{X_SCALE} and {Y_SCALE} have to be '
+                                     f'one of the following: '
+                                     + ', '.join(OBSERVABLE_TRANSFORMATIONS))
+                elif col == PLOT_TYPE_DATA and entry not in \
+                        PLOT_TYPES_DATA:
+                    raise ValueError(f'{PLOT_TYPE_DATA} has to be one of the '
+                                     f'following: '
+                                     + ', '.join(PLOT_TYPES_DATA))
+                elif col == PLOT_TYPE_SIMULATION and entry not in \
+                        PLOT_TYPES_SIMULATION:
+                    raise ValueError(f'{PLOT_TYPE_SIMULATION} has to be one of'
+                                     f' the following: '
+                                     + ', '.join(PLOT_TYPES_SIMULATION))
+
+                # append new entry to dict
+                vis_spec_dict[col] = entry
+            else:
+                warnings.warn(f'Column {col} cannot be used to specify subplot'
+                              f', only settings from the following columns can'
+                              f' be used:'
+                              + ', '.join(VISUALIZATION_DF_SUBPLOT_LEVEL_COLS))
+        return cls(plot_id, vis_spec_dict, dataplots)
+
+    def add_dataplot(self, dataplot: DataPlot) -> None:
+        """
+        Add data plot.
+
+        Parameters
+        ----------
+        dataplot:
+            Data plot visualization settings.
+
+        """
+        self.data_plots.append(dataplot)
+
+    def set_axes_limits(self,
+                        xlim: Optional[Tuple[Optional[Real],
+                                             Optional[Real]]] = None,
+                        ylim: Optional[Tuple[Optional[Real],
+                                             Optional[Real]]] = None):
+        """
+        Set axes limits for all subplots. If xlim or ylim or any of the tuple
+        items is None, corresponding limit is left unchanged.
+
+        Parameters
+        ----------
+        xlim:
+            X axis limits.
+        ylim:
+            Y axis limits.
+        """
+        self.xlim = xlim
+        self.ylim = ylim
+
+
+class Figure:
+    """
+    Visualization specification of a figure.
+
+    Contains information regarding how data should be visualized.
+    """
+    def __init__(self, subplots: Optional[List[Subplot]] = None,
+                 size: Tuple = (20, 15),
+                 title: Optional[Tuple] = None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        subplots: A list of visualization specifications for each subplot
+        size: Figure size
+        title: Figure title
+        """
+
+        # TODO: Isensee measurements table in doc/examples doesn't correspond
+        #       to documentation: observableTransformation and
+        #       noiseDistribution columns replicateId problem
+        # TODO: Should we put in the documentation which combination of fields
+        #  must be unique in the measurement table and add such check?
+        #  obs_id + sim_cond_id + preeq_cod_id (if exists) + time +
+        #  replicate_id (if exists)?
+        self.size = size
+        self.title = title
+        self.subplots = subplots if subplots is not None else []
+
+    @property
+    def num_subplots(self) -> int:
+        return len(self.subplots)
+
+    def add_subplot(self, subplot: Subplot) -> None:
+        """
+        Add subplot.
+
+        Parameters
+        ----------
+        subplot:
+            Subplot visualization settings.
+
+        """
+        self.subplots.append(subplot)
+
+    def set_axes_limits(self,
+                        xlim: Optional[Tuple[Optional[Real],
+                                             Optional[Real]]] = None,
+                        ylim: Optional[Tuple[Optional[Real],
+                                             Optional[Real]]] = None) -> None:
+        """
+        Set axes limits for all subplots. If xlim or ylim or any of the tuple
+        items is None, corresponding limit is left unchanged.
+
+        Parameters
+        ----------
+        xlim:
+            X axis limits.
+        ylim:
+            Y axis limits.
+        """
+
+        for subplot in self.subplots:
+            subplot.set_axes_limits(xlim, ylim)
+
+    def save_to_tsv(self, output_file_path: str = 'visuSpec.tsv') -> None:
+        """
+        Save full Visualization specification table.
+
+        Note that datasetId column in the resulting table might have been
+        generated even though datasetId column in Measurement table is missing
+        or is different. Please, correct it manually.
+
+        Parameters
+        ----------
+        output_file_path:
+            File path to which the generated visualization specification is
+            saved.
+        """
+        # TODO: what if datasetIds were generated?
+
+        warnings.warn(f'Note: please check that {DATASET_ID} column '
+                      f'corresponds to {DATASET_ID} column in Measurement '
+                      f'(Simulation) table.')
+
+        visu_dict = {}
+        for subplot in self.subplots:
+            subplot_level = {key: subplot.__dict__[key] for key in
+                             subplot.__dict__ if key in
+                             VISUALIZATION_DF_SUBPLOT_LEVEL_COLS}
+
+            for dataplot in subplot.data_plots:
+                dataset_level = {key: dataplot.__dict__[key] for key in
+                                 dataplot.__dict__ if key in
+                                 VISUALIZATION_DF_SINGLE_PLOT_LEVEL_COLS}
+                row = {**subplot_level, **dataset_level}
+                for key, value in row.items():
+                    if key in visu_dict:
+                        visu_dict[key].append(value)
+                    else:
+                        visu_dict[key] = [row[key]]
+        visu_df = pd.DataFrame.from_dict(visu_dict)
+        visu_df.to_csv(output_file_path, sep='\t', index=False)
+
+
+class DataProvider:
+    """
+    Handles data selection.
+    """
+    def __init__(self,
+                 exp_conditions: pd.DataFrame,
+                 measurements_data: Optional[pd.DataFrame] = None,
+                 simulations_data: Optional[pd.DataFrame] = None):
+        self.conditions_data = exp_conditions
+
+        if measurements_data is None and simulations_data is None:
+            raise TypeError('Not enough arguments. Either measurements_data '
+                            'or simulations_data should be provided.')
+        self.measurements_data = measurements_data
+        self.simulations_data = simulations_data
+
+    @staticmethod
+    def _matches_plot_spec(df: pd.DataFrame,
+                           plot_spec: 'DataPlot',
+                           dataset_id) -> pd.Series:
+        """
+        Construct an index for subsetting of the dataframe according to what
+        is specified in plot_spec.
+
+        Parameters
+        ----------
+            df:
+                A pandas data frame to subset, can be from measurement file or
+                simulation file.
+            plot_spec:
+                A visualization spec from the visualization file.
+
+        Returns
+        -------
+        Boolean series that can be used for subsetting of the passed
+        dataframe
+        """
+        subset = (
+            (df[DATASET_ID] == dataset_id)
+        )
+        if getattr(plot_spec, Y_VALUES) == '':
+            if len(df.loc[subset, OBSERVABLE_ID].unique()) > 1:
+                raise ValueError(
+                    f'{Y_VALUES} must be specified in visualization table if '
+                    f'multiple different observables are available.'
+                )
+        else:
+            subset &= (df[OBSERVABLE_ID] == getattr(plot_spec, Y_VALUES))
+        return subset
 
-    For documentation, see main function plot_data_and_simulation()
+    def _get_independent_var_values(self, data_df: pd.DataFrame,
+                                    dataplot: DataPlot
+                                    ) -> Tuple[np.ndarray, str, pd.Series]:
+        """
+        Get independent variable values.
+
+        Parameters
+        ----------
+        data_df:
+            A pandas data frame to subset, can be from measurement file or
+            simulation file.
+        dataplot:
+            Data plot visualization settings.
+
+        Returns
+        -------
+        col_name_unique:
+            A name of the column from Measurement (Simulation) table, which
+            specifies independent variable values (depends on the xValues entry
+            of visualization specification).
+            Possible values:
+
+            * TIME (independent variable values will be taken from the TIME
+              column of Measurement (Simulation) table)
+
+            * SIMULATION_CONDITION_ID (independent variable values will be
+              taken from one of the columns of Condition table)
+
+        uni_condition_id:
+            Time points
+            or
+            contains all unique condition IDs which should be
+            plotted together as one dataplot. Independent variable values will
+            be collected for these conditions
+        conditions_:
+            An independent variable values or None for the BarPlot case
+            possible values: time points, None, vales of independent variable
+            (Parameter or Species, specified in the xValues entry of
+            visualization specification) for each condition_id in
+            uni_condition_id
+
+        """
+
+        indep_var = getattr(dataplot, X_VALUES)
+
+        dataset_id = getattr(dataplot, DATASET_ID)
+
+        single_m_data = data_df[self._matches_plot_spec(
+            data_df, dataplot, dataset_id)]
+
+        # gather simulationConditionIds belonging to datasetId
+        uni_condition_id, uind = np.unique(
+            single_m_data[SIMULATION_CONDITION_ID],
+            return_index=True)
+        # keep the ordering which was given by user from top to bottom
+        # (avoid ordering by names '1','10','11','2',...)'
+        uni_condition_id = uni_condition_id[np.argsort(uind)]
+        col_name_unique = SIMULATION_CONDITION_ID
+
+        if indep_var == TIME:
+            # obtain unique observation times
+            uni_condition_id = single_m_data[TIME].unique()
+            col_name_unique = TIME
+            conditions_ = uni_condition_id
+        elif indep_var == 'condition':
+            conditions_ = None
+        else:
+            # indep_var = parameterOrStateId case ?
+            # extract conditions (plot input) from condition file
+            ind_cond = self.conditions_data.index.isin(uni_condition_id)
+            conditions_ = self.conditions_data[ind_cond][indep_var]
+
+        return uni_condition_id, col_name_unique, conditions_
+
+    def get_data_series(
+            self,
+            data_df: pd.DataFrame,
+            data_col: Literal['measurement', 'simulation'],
+            dataplot: DataPlot,
+            provided_noise: bool
+    ) -> DataSeries:
+        """
+        Get data to plot from measurement or simulation DataFrame.
+
+        Parameters
+        ----------
+        data_df: measurement or simulation DataFrame
+        data_col: data column, i.e. 'measurement' or 'simulation'
+        dataplot: visualization specification
+        provided_noise:
+            True if numeric values for the noise level are provided in the
+            data table
+
+        Returns
+        -------
+        Data to plot
+        """
+        uni_condition_id, col_name_unique, conditions_ = \
+            self._get_independent_var_values(data_df, dataplot)
+
+        dataset_id = getattr(dataplot, DATASET_ID)
+
+        # get data subset selected based on provided dataset_id
+        # and observable_ids
+        single_m_data = data_df[self._matches_plot_spec(
+            data_df, dataplot, dataset_id)]
+
+        # create empty dataframe for means and SDs
+        measurements_to_plot = pd.DataFrame(
+            columns=['mean', 'noise_model', 'sd', 'sem', 'repl'],
+            index=uni_condition_id
+        )
+
+        for var_cond_id in uni_condition_id:
+
+            subset = (single_m_data[col_name_unique] == var_cond_id)
+
+            # what has to be plotted is selected
+            data_measurements = single_m_data.loc[
+                subset,
+                data_col
+            ]
+
+            # TODO: all this rather inside DataSeries?
+            # process the data
+            measurements_to_plot.at[var_cond_id, 'mean'] = np.mean(
+                data_measurements)
+            measurements_to_plot.at[var_cond_id, 'sd'] = np.std(
+                data_measurements)
+
+            if provided_noise and np.any(subset):
+                if len(single_m_data.loc[
+                           subset, NOISE_PARAMETERS].unique()) > 1:
+                    raise NotImplementedError(
+                        f"Datapoints with inconsistent {NOISE_PARAMETERS} "
+                        f"is currently not implemented. Stopping.")
+                tmp_noise = \
+                    single_m_data.loc[subset, NOISE_PARAMETERS].values[0]
+                if isinstance(tmp_noise, str):
+                    raise NotImplementedError(
+                        "No numerical noise values provided in the "
+                        "measurement table. Stopping.")
+                if isinstance(tmp_noise, Number) or \
+                        tmp_noise.dtype == 'float64':
+                    measurements_to_plot.at[
+                        var_cond_id, 'noise_model'] = tmp_noise
+
+            # standard error of mean
+            measurements_to_plot.at[var_cond_id, 'sem'] = \
+                np.std(data_measurements) / np.sqrt(
+                    len(data_measurements))
+
+            # single replicates
+            measurements_to_plot.at[var_cond_id, 'repl'] = \
+                data_measurements.values
+
+        data_series = DataSeries(conditions_, measurements_to_plot)
+        data_series.add_offsets(dataplot.xOffset, dataplot.yOffset)
+        return data_series
+
+    def get_data_to_plot(self, dataplot: DataPlot, provided_noise: bool
+                         ) -> Tuple[DataSeries, DataSeries]:
+        """
+        Get data to plot.
+
+        Parameters
+        ----------
+        dataplot: visualization specification
+        provided_noise:
+            True if numeric values for the noise level are provided in the
+            measurement table
+
+        Returns
+        -----------
+        measurements_to_plot,
+        simulations_to_plot
+        """
+        measurements_to_plot = None
+        simulations_to_plot = None
+
+        if self.measurements_data is not None:
+            measurements_to_plot = self.get_data_series(self.measurements_data,
+                                                        MEASUREMENT,
+                                                        dataplot,
+                                                        provided_noise)
+
+        if self.simulations_data is not None:
+            simulations_to_plot = self.get_data_series(self.simulations_data,
+                                                       SIMULATION,
+                                                       dataplot,
+                                                       provided_noise)
+        return measurements_to_plot, simulations_to_plot
+
+
+class VisSpecParser:
+    """
+    Parser of visualization specification provided by user either in the form
+    of Visualization table or as a list of lists with datasets ids or
+    observable ids or condition ids. Figure instance is created containing
+    information regarding how data should be visualized. In addition to the
+    Figure instance, a DataProvider instance is created that will be
+    responsible for the data selection and manipulation.
+    """
+    def __init__(
+            self,
+            conditions_data: Union[str, Path, pd.DataFrame],
+            exp_data: Optional[Union[str, Path, pd.DataFrame]] = None,
+            sim_data: Optional[Union[str, Path, pd.DataFrame]] = None,
+    ):
+        if isinstance(conditions_data, (str, Path)):
+            conditions_data = conditions.get_condition_df(conditions_data)
+
+        # import from file in case experimental data is provided in file
+        if isinstance(exp_data, (str, Path)):
+            exp_data = measurements.get_measurement_df(exp_data)
+
+        if isinstance(sim_data, (str, Path)):
+            sim_data = core.get_simulation_df(sim_data)
+
+        if exp_data is None and sim_data is None:
+            raise TypeError('Not enough arguments. Either measurements_data '
+                            'or simulations_data should be provided.')
+
+        self.conditions_data = conditions_data
+        self.measurements_data = exp_data
+        self.simulations_data = sim_data
+
+    @classmethod
+    def from_problem(cls, petab_problem: Problem, sim_data):
+        return cls(petab_problem.condition_df,
+                   petab_problem.measurement_df,
+                   sim_data)
+
+    @property
+    def _data_df(self):
+        return self.measurements_data if self.measurements_data is not \
+            None else self.simulations_data
+
+    @staticmethod
+    def create_subplot(
+            plot_id: str,
+            subplot_vis_spec: pd.DataFrame
+    ) -> Subplot:
+        """
+        Create subplot.
+
+        Parameters
+        ----------
+        plot_id:
+            Plot id.
+        subplot_vis_spec:
+            A visualization specification DataFrame that contains specification
+            for the subplot and corresponding dataplots.
+
+        Returns
+        -------
+
+                Subplot
+        """
+        subplot_columns = [col for col in subplot_vis_spec.columns if col in
+                           VISUALIZATION_DF_SUBPLOT_LEVEL_COLS]
+        subplot = Subplot.from_df(plot_id,
+                                  subplot_vis_spec.loc[:, subplot_columns])
+
+        dataplot_cols = [col for col in subplot_vis_spec.columns if col in
+                         VISUALIZATION_DF_SINGLE_PLOT_LEVEL_COLS]
+        dataplot_spec = subplot_vis_spec.loc[:, dataplot_cols]
+
+        for _, row in dataplot_spec.iterrows():
+            data_plot = DataPlot.from_df(row)
+            subplot.add_dataplot(data_plot)
+
+        return subplot
+
+    def parse_from_vis_spec(
+            self,
+            vis_spec: Optional[Union[str, Path, pd.DataFrame]],
+    ) -> Tuple[Figure, DataProvider]:
+        """
+        Get visualization settings from a visualization specification.
+
+        Parameters
+        ----------
+        vis_spec:
+            Visualization specification DataFrame in the PEtab format
+            or a path to a visualization file.
+
+        Returns
+        -------
+
+        A figure template with visualization settings and a data provider
+        """
+        # import visualization specification, if file was specified
+        if isinstance(vis_spec, (str, Path)):
+            vis_spec = core.get_visualization_df(vis_spec)
+
+        if DATASET_ID not in vis_spec.columns:
+            self._add_dataset_id_col()
+            vis_spec = self._expand_vis_spec_settings(vis_spec)
+        else:
+            if self.measurements_data is not None \
+                    and DATASET_ID not in self.measurements_data:
+                raise ValueError(f"grouping by datasetId was requested, but "
+                                 f"{DATASET_ID} column is missing from "
+                                 f"measurement table")
+            if self.simulations_data is not None \
+                    and DATASET_ID not in self.simulations_data:
+                raise ValueError(f"grouping by datasetId was requested, but "
+                                 f"{DATASET_ID} column is missing from "
+                                 f"simulation table")
+
+        figure = Figure()
+
+        # get unique plotIDs preserving the order from the original vis spec
+        _, idx = np.unique(vis_spec[PLOT_ID], return_index=True)
+        plot_ids = vis_spec[PLOT_ID].iloc[np.sort(idx)]
+
+        # loop over unique plotIds
+        for plot_id in plot_ids:
+            # get indices for specific plotId
+            ind_plot = (vis_spec[PLOT_ID] == plot_id)
+
+            subplot = self.create_subplot(plot_id, vis_spec[ind_plot])
+            figure.add_subplot(subplot)
+
+        return figure, DataProvider(self.conditions_data,
+                                    self.measurements_data,
+                                    self.simulations_data)
+
+    def parse_from_id_list(self,
+                           ids_per_plot: Optional[List[IdsList]] = None,
+                           group_by: str = 'observable',
+                           plotted_noise: Optional[str] = MEAN_AND_SD
+                           ) -> Tuple[Figure, DataProvider]:
+        """
+        Get visualization settings from a list of ids and a grouping parameter.
+
+        Parameters
+        ----------
+        ids_per_plot:
+            A list of lists. Each sublist corresponds to a plot, each subplot
+            contains the Ids of datasets or observables or simulation
+            conditions for this plot.
+            e.g.
+
+            ::
+
+                dataset_ids_per_plot = [['dataset_1', 'dataset_2'],
+                                        ['dataset_1', 'dataset_4',
+                                         'dataset_5']]
+
+            or
+
+            ::
+
+                cond_id_list = [['model1_data1'],
+                                ['model1_data2', 'model1_data3'],
+                                ['model1_data4', 'model1_data5'],
+                                ['model1_data6']].
 
-    Returns:
         group_by:
-            Specifies the grouping of data to plot.
-    """
+            Grouping type. Possible values: 'dataset', 'observable',
+            'simulation'.
+        plotted_noise:
+            String indicating how noise should be visualized:
+            ['MeanAndSD' (default), 'MeanAndSEM', 'replicate', 'provided'].
+
+        Returns
+        -------
+        A figure template with visualization settings and a data provider
+
+        """
+
+        if ids_per_plot is None:
+            # this is the default case. If no grouping is specified,
+            # all observables are plotted. One observable per plot.
+            unique_obs_list = self._data_df[OBSERVABLE_ID].unique()
+            ids_per_plot = [[obs_id] for obs_id in unique_obs_list]
+
+        if group_by == 'dataset' and DATASET_ID not in self._data_df:
+            raise ValueError(f"grouping by datasetId was requested, but "
+                             f"{DATASET_ID} column is missing from data table")
 
-    # We have no vis_spec file. Check how data should be grouped
-    group_by = ''
-    if dataset_id_list is not None:
-        group_by += 'dataset'
-
-    # check whether grouping by simulation condition should be done
-    if sim_cond_id_list is not None and sim_cond_num_list is not None:
-        raise NotImplementedError(
-            "Either specify a list of simulation condition IDs or a list of "
-            "simulation condition numbers, but not both. Stopping.")
-    if sim_cond_id_list is not None or sim_cond_num_list is not None:
-        group_by += 'simulation'
-
-    # check whether grouping by observable should be done
-    if observable_id_list is not None and observable_num_list is not None:
-        raise NotImplementedError(
-            "Either specify a list of observable IDs or a list "
-            "of observable numbers, but not both. Stopping.")
-    if observable_id_list is not None or observable_num_list is not None:
-        group_by += 'observable'
-    # consistency check. Warn or error, if grouping not clear
-    if group_by == 'datasetsimulation':
-        warnings.warn("Found grouping by datasetId and simulation condition. "
-                      "Using datasetId, omitting simulation condition.")
-        group_by = 'dataset'
-
-    elif group_by == 'datasetobservable':
-        warnings.warn("Found grouping by datasetId and observable. "
-                      "Using datasetId, omitting observable.")
-        group_by = 'dataset'
-
-    elif group_by == 'datasetsimulationobservable':
-        warnings.warn("Found grouping by datasetId, simulation condition, and "
-                      "observable. Using datasetId, omitting simulation "
-                      "condition and observable.")
-        group_by = 'dataset'
-
-    elif group_by == 'simulationobservable':
-        raise NotImplementedError(
-            "Plotting without visualization specification file and datasetId "
-            "can be performed via grouping by simulation conditions OR "
-            "observables, but not both. Stopping.")
-    elif group_by in ['simulation', 'observable', 'dataset']:
-        pass
-    # if group_by is still empty (if visuSpec file is available but datasetId
-    # is not  available), default: observables
-    elif group_by == '':
-        group_by = 'observable'
-        warnings.warn('Default plotting: grouping by observable. If you want '
-                      'to specify another grouping option, please add '
-                      '\'datasetId\' columns.')
-    else:
-        raise NotImplementedError(
-            "No information provided, how to plot data. Stopping.")
-
-    if group_by != 'dataset':
-        # group plots not by dataset. Check, whether such a column would
-        # have been available (and give a warning, if so)
-        if 'datasetId' in exp_data.columns:
-            warnings.warn("DatasetIds would have been available, but other "
-                          "grouping was requested. Consider using datasetId.")
-    else:
-        if 'datasetId' not in exp_data.columns:
-            raise NotImplementedError(
-                "Data should be grouped by datasetId, but no datasetId is "
-                "given in the measurement file. Stopping.")
-
-    return group_by
-
-
-def create_dataset_id_list(
-        simcond_id_list: List[IdsList],
-        simcond_num_list: List[NumList],
-        observable_id_list: List[IdsList],
-        observable_num_list: List[NumList],
-        exp_data: pd.DataFrame,
-        exp_conditions: pd.DataFrame,
-        group_by: str) -> Tuple[pd.DataFrame, List[IdsList], Dict, Dict]:
-    """
-    Create dataset id list and corresponding plot legends.
-    Additionally, update/create DATASET_ID column of exp_data
-
-    Parameters:
-        group_by: defines  grouping of data to plot
-
-    Returns:
-        A tuple of experimental DataFrame, list of datasetIds and
-        dictionary of plot legends, corresponding to the datasetIds
-
-    For additional documentation, see main function plot_data_and_simulation()
-    """
-    # create a column of dummy datasetIDs and legend entries: preallocate
-    dataset_id_column = []
-    legend_dict = {}
-    yvalues_dict = {}
-
-    # loop over experimental data table, create datasetId for each entry
-    tmp_simcond = list(exp_data[SIMULATION_CONDITION_ID])
-    tmp_obs = list(exp_data[OBSERVABLE_ID])
-    for ind, cond_id in enumerate(tmp_simcond):
-        # create and add dummy datasetID
-        dataset_id = tmp_simcond[ind] + '_' + tmp_obs[ind]
-        dataset_id_column.append(dataset_id)
-
-        # create nicer legend entries from condition names instead of IDs
-        if dataset_id not in legend_dict.keys():
-            tmp = exp_conditions.loc[exp_conditions.index == cond_id]
-            if CONDITION_NAME not in tmp.columns or tmp[
-                    CONDITION_NAME].isna().any():
-                tmp.loc[:, CONDITION_NAME] = tmp.index.tolist()
-            legend_dict[dataset_id] = tmp[CONDITION_NAME][0] + ' - ' + \
-                tmp_obs[ind]
-            yvalues_dict[dataset_id] = tmp_obs[ind]
-
-    # add these column to the measurement table (possibly overwrite)
-    if DATASET_ID in exp_data.columns:
-        exp_data = exp_data.drop(DATASET_ID, axis=1)
-    exp_data.insert(loc=exp_data.columns.size, column=DATASET_ID,
-                    value=dataset_id_column)
-
-    # make dummy dataset names unique and iterable
-    unique_dataset_list = functools.reduce(
-        lambda tmp, x: tmp.append(x) or tmp if x not in tmp else tmp,
-        list(exp_data[DATASET_ID]), [])
-    unique_simcond_list = functools.reduce(
-        lambda tmp, x: tmp.append(x) or tmp if x not in tmp else tmp,
-        list(exp_data[SIMULATION_CONDITION_ID]), [])
-    unique_obs_list = functools.reduce(
-        lambda tmp, x: tmp.append(x) or tmp if x not in tmp else tmp,
-        list(exp_data[OBSERVABLE_ID]), [])
-
-    # we will need a dictionary for mapping simulation conditions
-    # /observables to datasets
-    ds_dict = {}
-    dataset_id_list = []
-    if group_by == 'simulation':
-        if simcond_id_list is None:
-            simcond_id_list = [[unique_simcond_list[i_cond] for i_cond in
-                                i_cond_list] for i_cond_list in
-                               simcond_num_list]
-        for simcond in unique_simcond_list:
-            # ds_dict[simcond] = [ds for ds in unique_dataset_list if ds[
-            #    0:len(simcond)+3] == simcond + ' - ']
-            # ds_dict[simcond] = [ds for ds in unique_dataset_list if ds[
-            #    0:len(simcond) + 3] == simcond + '_']
-            ds_dict[simcond] = [ds for ds in unique_dataset_list if ds[
-                0:len(simcond)] == simcond]
-        grouped_list = simcond_id_list
-
-    elif group_by == 'observable':
-        if not observable_id_list and not observable_num_list:
-            observable_id_list = [unique_obs_list]
-        if observable_id_list is None:
-            observable_id_list = [[unique_obs_list[i_obs] for i_obs in
-                                   i_obs_list] for i_obs_list in
-                                  observable_num_list]
-        for observable in unique_obs_list:
-            # ds_dict[observable] = [ds for ds in unique_dataset_list if ds[
-            #    -len(observable)-3:] == ' - ' + observable]
-            ds_dict[observable] = [ds for ds in unique_dataset_list if ds[
-                -len(observable) - 1:] == '_' + observable]
-        grouped_list = observable_id_list
-
-    else:
-        raise NotImplementedError(
-            "Very, very weird error. Should not have happened. Something "
-            "went wrong in how datasets should be grouped. Very weird...")
-
-    for sublist in grouped_list:
-        datasets_for_this_plot = [dset for sublist_entry in sublist
-                                  for dset in ds_dict[sublist_entry]]
-        dataset_id_list.append(datasets_for_this_plot)
-
-    return exp_data, dataset_id_list, legend_dict, yvalues_dict
-
-
-def create_figure(
-        uni_plot_ids: np.ndarray,
-        plots_to_file: bool) -> Tuple[plt.Figure,
-                                      Union[Dict[str, plt.Subplot],
-                                            'np.ndarray[plt.Subplot]']]:
-    """
-    Helper function for plotting data and simulations, open figure and axes
-
-    Parameters
-    ----------
-    uni_plot_ids:
-        Array with unique plot indices
-    plots_to_file:
-        Indicator if plots are saved to file
-
-    Returns
-    -------
-    fig: Figure object of the created plot.
-    ax: Axis object of the created plot.
-    """
-
-    # Set Options for plots
-    # possible options: see: plt.rcParams.keys()
-    plt.rcParams['font.size'] = 10
-    plt.rcParams['axes.titlesize'] = 10
-    plt.rcParams['figure.figsize'] = [20, 10]
-    plt.rcParams['errorbar.capsize'] = 2
-
-    # Set Colormap
-    sns.set(style="ticks", palette="colorblind")
-
-    # Check if plots are saved to file and return single subplot axis
-    if plots_to_file:
-        num_subplot = 1
-    else:
-        num_subplot = len(uni_plot_ids)
-
-    # compute, how many rows and columns we need for the subplots
-    num_row = int(np.round(np.sqrt(num_subplot)))
-    num_col = int(np.ceil(num_subplot / num_row))
-
-    fig, axes = plt.subplots(num_row, num_col, squeeze=False)
-
-    if not plots_to_file:
-        for ax in axes.flat[num_subplot:]:
-            ax.remove()
-
-        axes = dict(zip(uni_plot_ids, axes.flat))
-
-    return fig, axes
-
-
-def get_default_vis_specs(
-        exp_data: pd.DataFrame,
-        exp_conditions: pd.DataFrame,
-        dataset_id_list: Optional[List[IdsList]] = None,
-        sim_cond_id_list: Optional[List[IdsList]] = None,
-        sim_cond_num_list: Optional[List[NumList]] = None,
-        observable_id_list: Optional[List[IdsList]] = None,
-        observable_num_list: Optional[List[NumList]] = None,
-        plotted_noise: Optional[str] = MEAN_AND_SD
-) -> Tuple[pd.DataFrame, pd.DataFrame]:
-    """
-    Helper function for plotting data and simulations, which creates a
-    default visualization table and updates/creates DATASET_ID column of
-    exp_data
-
-    Returns:
-        A tuple of visualization specification DataFrame and experimental
-        DataFrame.
-
-    For documentation, see main function plot_data_and_simulation()
-    """
-    warnings.warn("This function will be removed in future releases. ",
-                  DeprecationWarning)
-
-    # check consistency of settings
-    group_by = check_vis_spec_consistency(
-        exp_data, dataset_id_list, sim_cond_id_list, sim_cond_num_list,
-        observable_id_list, observable_num_list)
-
-    if group_by != 'dataset':
-        # datasetId_list will be created (possibly overwriting previous list
-        #  - only in the local variable, not in the tsv-file)
-        exp_data, dataset_id_list, legend_dict, _ = \
-            create_dataset_id_list(sim_cond_id_list, sim_cond_num_list,
-                                   observable_id_list, observable_num_list,
-                                   exp_data, exp_conditions, group_by)
-
-    dataset_id_column = [i_dataset for sublist in dataset_id_list
-                         for i_dataset in sublist]
-    if group_by != 'dataset':
-        dataset_label_column = [legend_dict[i_dataset] for sublist in
-                                dataset_id_list for i_dataset in sublist]
-    else:
-        dataset_label_column = dataset_id_column
+        if group_by != 'dataset':
+            # datasetId_list will be created (possibly overwriting previous
+            # list - only in the local variable, not in the tsv-file)
+            self._add_dataset_id_col()
+
+        columns_dict = self._get_vis_spec_dependent_columns_dict(
+            group_by, ids_per_plot)
 
-    # get number of plots and create plotId-lists
-    plot_id_list = [f'plot{ind+1}' for ind, inner_list in enumerate(
-        dataset_id_list) for _ in inner_list]
-
-    # create dataframe
-    vis_spec = pd.DataFrame({PLOT_ID: plot_id_list,
-                             DATASET_ID: dataset_id_column,
-                             LEGEND_ENTRY: dataset_label_column})
-
-    # fill columns with default values
-    fill_vis_spec = ((2, Y_LABEL, 'value'),
-                     (2, Y_OFFSET, 0),
-                     (2, Y_VALUES, ''),
-                     (2, X_LABEL, 'time'),
-                     (2, X_OFFSET, 0),
-                     (2, X_VALUES, 'time'),
-                     (1, Y_SCALE, LIN),
-                     (1, X_SCALE, LIN),
-                     (0, PLOT_TYPE_DATA, plotted_noise),
-                     (0, PLOT_TYPE_SIMULATION, LINE_PLOT),
-                     (0, PLOT_NAME, ''))
-    for pos, col, val in fill_vis_spec:
-        vis_spec.insert(loc=pos, column=col, value=val)
-
-    return vis_spec, exp_data
-
-
-def get_vis_spec_dependent_columns_dict(
-        exp_data: pd.DataFrame,
-        exp_conditions: pd.DataFrame,
-        dataset_id_list: Optional[List[IdsList]] = None,
-        sim_cond_id_list: Optional[List[IdsList]] = None,
-        sim_cond_num_list: Optional[List[NumList]] = None,
-        observable_id_list: Optional[List[IdsList]] = None,
-        observable_num_list: Optional[List[NumList]] = None
-) -> Tuple[pd.DataFrame, Dict]:
-    """
-    Helper function for creating values for columns PLOT_ID, DATASET_ID,
-    LEGEND_ENTRY, Y_VALUES for visualization specification file.
-    DATASET_ID column of exp_data is updated accordingly.
-
-    Returns:
-        A tuple of experimental DataFrame and a dictionary with values for
-        columns PLOT_ID, DATASET_ID, LEGEND_ENTRY, Y_VALUES for visualization
-        specification file.
-    """
-
-    # check consistency of settings
-    group_by = check_vis_spec_consistency(
-        exp_data, dataset_id_list, sim_cond_id_list, sim_cond_num_list,
-        observable_id_list, observable_num_list)
-
-    if group_by != 'dataset':
-        # datasetId_list will be created (possibly overwriting previous list
-        #  - only in the local variable, not in the tsv-file)
-        exp_data, dataset_id_list, legend_dict, yvalues_dict = \
-            create_dataset_id_list(sim_cond_id_list, sim_cond_num_list,
-                                   observable_id_list, observable_num_list,
-                                   exp_data, exp_conditions, group_by)
+        columns_dict[PLOT_TYPE_DATA] = [plotted_noise]*len(
+            columns_dict[DATASET_ID])
 
-    dataset_id_column = [i_dataset for sublist in dataset_id_list
-                         for i_dataset in sublist]
+        vis_spec_df = pd.DataFrame(columns_dict)
+
+        return self.parse_from_vis_spec(vis_spec_df)
+
+    def _add_dataset_id_col(self) -> None:
+        """
+        Add dataset_id column to the measurement table and simulations table
+        (possibly overwrite).
+        """
+
+        if self.measurements_data is not None:
+            if DATASET_ID in self.measurements_data.columns:
+                self.measurements_data = self.measurements_data.drop(
+                    DATASET_ID, axis=1)
+            self.measurements_data.insert(
+                loc=self.measurements_data.columns.size,
+                column=DATASET_ID,
+                value=generate_dataset_id_col(self.measurements_data))
+
+        if self.simulations_data is not None:
+            if DATASET_ID in self.simulations_data.columns:
+                self.simulations_data = self.simulations_data.drop(DATASET_ID,
+                                                                   axis=1)
+            self.simulations_data.insert(
+                loc=self.simulations_data.columns.size,
+                column=DATASET_ID,
+                value=generate_dataset_id_col(self.simulations_data))
+
+    def _get_vis_spec_dependent_columns_dict(
+        self,
+        group_by: str,
+        id_list: Optional[List[IdsList]] = None
+    ) -> Dict:
+        """
+        Helper method for creating values for columns PLOT_ID, DATASET_ID,
+        LEGEND_ENTRY, Y_VALUES for visualization specification file.
 
-    if group_by != 'dataset':
-        dataset_label_column = [legend_dict[i_dataset] for sublist in
+        Parameters
+        ----------
+        group_by:
+            Grouping type.
+            Possible values: 'dataset', 'observable', 'simulation'.
+        id_list:
+            Grouping list. Each sublist corresponds to a subplot and
+            contains the Ids of datasets or observables or simulation
+            conditions for this subplot.
+
+        Returns
+        -------
+        A dictionary with values for columns PLOT_ID, DATASET_ID, \
+        LEGEND_ENTRY, Y_VALUES for visualization specification.
+        """
+
+        if group_by != 'dataset':
+            dataset_id_list = create_dataset_id_list_new(self._data_df,
+                                                         group_by, id_list)
+        else:
+            dataset_id_list = id_list
+
+        dataset_id_column = [i_dataset for sublist in dataset_id_list
+                             for i_dataset in sublist]
+
+        dataset_label_column = [self._create_legend(i_dataset) for sublist in
                                 dataset_id_list for i_dataset in sublist]
-        yvalues_column = [yvalues_dict[i_dataset] for sublist in
-                          dataset_id_list for i_dataset in sublist]
-    else:
-        dataset_label_column = dataset_id_column
-        yvalues_column = ['']*len(dataset_id_column)
-
-    # get number of plots and create plotId-lists
-    if group_by == 'observable':
-        obs_uni = list(np.unique(exp_data[OBSERVABLE_ID]))
-        # copy of dataset ids, for later replacing with plot ids
-        plot_id_column = dataset_id_column.copy()
-        for i_obs in range(0, len(obs_uni)):
-            # get dataset_ids which include observable name
-            matching = [s for s in dataset_id_column if obs_uni[i_obs] in s]
-            # replace the dataset ids with plot id with grouping of observables
-            for m_i in matching:
-                plot_id_column = [sub.replace(m_i, 'plot%s' % str(i_obs + 1))
-                                  for sub in plot_id_column]
-    else:
+
+        # such dataset ids were generated that each dataset_id always
+        # corresponds to one observable
+        yvalues_column = [self._data_df.loc[self._data_df[DATASET_ID] ==
+                                            dataset_id, OBSERVABLE_ID].iloc[0]
+                          for sublist in dataset_id_list for dataset_id in
+                          sublist]
+
         # get number of plots and create plotId-lists
         plot_id_column = ['plot%s' % str(ind + 1) for ind, inner_list in
                           enumerate(dataset_id_list) for _ in inner_list]
 
-    columns_dict = {PLOT_ID: plot_id_column,
-                    DATASET_ID: dataset_id_column,
-                    LEGEND_ENTRY: dataset_label_column,
-                    Y_VALUES: yvalues_column}
-    return exp_data, columns_dict
-
-
-def expand_vis_spec_settings(vis_spec, columns_dict):
-    """
-    only makes sense if DATASET_ID is not in vis_spec.columns?
-
-    Returns:
-        A visualization specification DataFrame
-    """
-    columns_to_expand = [PLOT_NAME, PLOT_TYPE_SIMULATION, PLOT_TYPE_DATA,
-                         X_VALUES, X_OFFSET, X_LABEL, X_SCALE, Y_OFFSET,
-                         Y_LABEL, Y_SCALE, LEGEND_ENTRY]
-
-    for column in vis_spec.columns:
-        if column in columns_to_expand:
-            column_entries = []
-            if Y_VALUES in vis_spec.columns:
-                for i, plot_id in enumerate(columns_dict[PLOT_ID]):
-                    select_conditions = (vis_spec[PLOT_ID] == plot_id) & (
-                        vis_spec[Y_VALUES] == columns_dict[Y_VALUES][i])
-                    column_entries.append(
-                        vis_spec[select_conditions].loc[:, column].values[0])
-            else:
-                # get unique plotIDs from visspecfile
-                vis_plotid_u = vis_spec[PLOT_ID].unique()
-                auto_plotid_u = list(set(columns_dict[PLOT_ID]))
-                # if number of plotIds does not coincide (autmatically
-                # generated plotIds according to observable grouping, vs
-                # plotIds specified in the visu_Spec)
-                if len(vis_plotid_u) is not len(auto_plotid_u):
-                    # which items are not in visu_plotId:
-                    del_plotid = \
-                        list(set(columns_dict[PLOT_ID]) - set(vis_plotid_u))
-                    # replace automatically generated plotIds with 'plot1' from
-                    # visu file
-                    for d_i in del_plotid:
-                        columns_dict[PLOT_ID] = [
-                            sub.replace(d_i, vis_plotid_u[0])
-                            for sub in columns_dict[PLOT_ID]]
-
-                for plot_id in columns_dict[PLOT_ID]:
-                    select_conditions = vis_spec[PLOT_ID] == plot_id
-                    column_entries.append(
-                        vis_spec[select_conditions].loc[:, column].values[0])
-            columns_dict[column] = column_entries
-    vis_spec = pd.DataFrame(columns_dict)
-    return vis_spec
-
-
-def create_or_update_vis_spec(
-        exp_data: pd.DataFrame,
-        exp_conditions: pd.DataFrame,
-        vis_spec: Optional[pd.DataFrame] = None,
-        dataset_id_list: Optional[List[IdsList]] = None,
-        sim_cond_id_list: Optional[List[IdsList]] = None,
-        sim_cond_num_list: Optional[List[NumList]] = None,
-        observable_id_list: Optional[List[IdsList]] = None,
-        observable_num_list: Optional[List[NumList]] = None,
-        plotted_noise: Optional[str] = MEAN_AND_SD):
-    """
-    Helper function for plotting data and simulations, which updates vis_spec
-    file if necessary or creates a default visualization table and
-    updates/creates DATASET_ID column of exp_data. As a result, a visualization
-    specification file exists with columns PLOT_ID, DATASET_ID, Y_VALUES and
-    LEGEND_ENTRY
-
-    Returns:
-        A tuple of visualization specification DataFrame and experimental
-        DataFrame.
-    """
-    if vis_spec is None:
-        # create dataframe
-        exp_data, columns_dict = \
-            get_vis_spec_dependent_columns_dict(exp_data,
-                                                exp_conditions,
-                                                dataset_id_list,
-                                                sim_cond_id_list,
-                                                sim_cond_num_list,
-                                                observable_id_list,
-                                                observable_num_list)
-        vis_spec = pd.DataFrame(columns_dict)
-    else:
-        # TODO: do validation issue #190
-        # so, plotid is definitely there
-        if DATASET_ID not in vis_spec.columns:
-            if Y_VALUES in vis_spec.columns:
-                plot_id_list = np.unique(vis_spec[PLOT_ID])
-
-                observable_id_list = [vis_spec[vis_spec[PLOT_ID] ==
-                                               plot_id].loc[:, Y_VALUES].values
-                                      for plot_id in plot_id_list]
-                exp_data, columns_dict = \
-                    get_vis_spec_dependent_columns_dict(
-                        exp_data,
-                        exp_conditions,
-                        observable_id_list=observable_id_list)
-            else:
-                # PLOT_ID is there, but NOT DATASET_ID and not Y_VALUES,
-                # but potentially some settings.
-                # TODO: multiple plotids with diff settings
-                exp_data, columns_dict = \
-                    get_vis_spec_dependent_columns_dict(
-                        exp_data,
-                        exp_conditions)
-            # get other settings that could have potentially been there
-            # and expand according to plot_id_column
-            vis_spec = expand_vis_spec_settings(vis_spec, columns_dict)
-
-        # if dataset_id is there, then nothing to expand?
-    vis_spec[PLOT_TYPE_DATA] = plotted_noise
-
-    # check columns, and add non-mandatory default columns
-    vis_spec = check_ex_visu_columns(vis_spec, exp_data, exp_conditions)
-    return exp_data, vis_spec
-
-
-def check_ex_visu_columns(vis_spec: pd.DataFrame,
-                          exp_data: pd.DataFrame,
-                          exp_conditions: pd.DataFrame) -> pd.DataFrame:
-    """
-    Check the columns in Visu_Spec file, if non-mandotory columns does not
-    exist, create default columns
-
-    Returns:
-        Updated visualization specification DataFrame
-    """
-    if PLOT_NAME not in vis_spec.columns:
-        vis_spec[PLOT_NAME] = ''
-    if PLOT_TYPE_SIMULATION not in vis_spec.columns:
-        vis_spec[PLOT_TYPE_SIMULATION] = LINE_PLOT
-    if PLOT_TYPE_DATA not in vis_spec.columns:
-        vis_spec[PLOT_TYPE_DATA] = MEAN_AND_SD
-    if X_VALUES not in vis_spec.columns:
-        # check if time is constant in expdata (if yes, plot dose response)
-        # otherwise plot time series
-        uni_time = pd.unique(exp_data[TIME])
-        if len(uni_time) > 1:
-            vis_spec[X_VALUES] = 'time'
-        elif len(uni_time) == 1:
-            if np.isin(exp_conditions.columns.values, 'conditionName').any():
-                conds = exp_conditions.columns.drop('conditionName')
-            else:
-                conds = exp_conditions.columns
-            # default: first dose-response condition (first from condition
-            # table) is plotted
-            # TODO: expand to automatic plotting of all conditions
-            vis_spec[X_VALUES] = conds[0]
-            vis_spec[X_LABEL] = conds[0]
-            warnings.warn(
-                '\n First dose-response condition is plotted. \n Check which '
-                'condition you want to plot \n and possibly enter it into the '
-                'column *xValues* \n in the visualization table.')
-        else:
-            raise NotImplementedError(
-                'Strange Error. There is no time defined in the measurement '
-                'table?')
-    if X_OFFSET not in vis_spec.columns:
-        vis_spec[X_OFFSET] = 0
-    if X_LABEL not in vis_spec.columns:
-        vis_spec[X_LABEL] = 'time'
-        vis_spec.loc[vis_spec[X_VALUES] != 'time', X_LABEL] = 'condition'
-    if X_SCALE not in vis_spec.columns:
-        vis_spec[X_SCALE] = LIN
-    if Y_VALUES not in vis_spec.columns:
-        vis_spec[Y_VALUES] = ''
-    if Y_OFFSET not in vis_spec.columns:
-        vis_spec[Y_OFFSET] = 0
-    if Y_LABEL not in vis_spec.columns:
-        vis_spec[Y_LABEL] = 'value'
-    if Y_SCALE not in vis_spec.columns:
-        vis_spec[Y_SCALE] = LIN
-    if LEGEND_ENTRY not in vis_spec.columns:
-        vis_spec[LEGEND_ENTRY] = vis_spec[DATASET_ID]
-
-    return vis_spec
-
-
-def check_ex_exp_columns(
-        exp_data: pd.DataFrame,
-        dataset_id_list: List[IdsList],
-        sim_cond_id_list: List[IdsList],
-        sim_cond_num_list: List[NumList],
-        observable_id_list: List[IdsList],
-        observable_num_list: List[NumList],
-        exp_conditions: pd.DataFrame,
-        sim: Optional[bool] = False
-) -> Tuple[pd.DataFrame, List[IdsList], Dict]:
-    """
-    Check the columns in measurement file, if non-mandotory columns does not
-    exist, create default columns
-
-    Returns:
-        A tuple of experimental DataFrame, list of datasetIds and
-        dictionary of plot legends, corresponding to the datasetIds
-    """
-    data_type = MEASUREMENT
-    if sim:
-        data_type = SIMULATION
-    # mandatory columns
-    if OBSERVABLE_ID not in exp_data.columns:
-        raise NotImplementedError(
-            f"Column \'observableId\' is missing in {data_type} file. ")
-    if SIMULATION_CONDITION_ID not in exp_data.columns:
-        raise NotImplementedError(
-            f"Column \'simulationConditionId\' is missing in {data_type} "
-            f"file. ")
-    if data_type not in exp_data.columns:
-        raise NotImplementedError(
-            f"Column \'{data_type}\' is missing in {data_type} "
-            f"file. ")
-    if TIME not in exp_data.columns:
-        raise NotImplementedError(
-            f"Column \'time\' is missing in {data_type} "
-            f"file. ")
-    # non-mandatory columns
-    if PREEQUILIBRATION_CONDITION_ID not in exp_data.columns:
-        exp_data.insert(loc=1, column=PREEQUILIBRATION_CONDITION_ID,
-                        value='')
-    if OBSERVABLE_PARAMETERS not in exp_data.columns:
-        exp_data.insert(loc=4, column=OBSERVABLE_PARAMETERS,
-                        value='')
-    if NOISE_PARAMETERS not in exp_data.columns:
-        exp_data.insert(loc=4, column=NOISE_PARAMETERS,
-                        value=0)
-    if REPLICATE_ID not in exp_data.columns:
-        exp_data.insert(loc=4, column=REPLICATE_ID,
-                        value='')
-    legend_dict = {}
-    if DATASET_ID not in exp_data.columns:
-        if dataset_id_list is not None:
-            exp_data.insert(loc=4, column=DATASET_ID,
-                            value=dataset_id_list)
+        return {
+            PLOT_ID: plot_id_column,
+            DATASET_ID: dataset_id_column,
+            LEGEND_ENTRY: dataset_label_column,
+            Y_VALUES: yvalues_column
+        }
+
+    def _create_legend(self, dataset_id: str) -> str:
+        """
+        Create a legend for the dataset ids.
+
+        Parameters
+        ----------
+        dataset_id:
+            Dataset id.
+
+        Returns
+        -------
+        A legend.
+        """
+        # relies on the fact that dataset ids were created based on cond_ids
+        # and obs_ids. Therefore, in the following query all pairs will be
+        # the same
+        cond_id, obs_id = self._data_df[self._data_df[DATASET_ID] ==
+                                        dataset_id][[SIMULATION_CONDITION_ID,
+                                                     OBSERVABLE_ID]].iloc[0, :]
+        tmp = self.conditions_data.loc[cond_id]
+        if CONDITION_NAME not in tmp.index or \
+                pd.isna(tmp[CONDITION_NAME]):
+            cond_name = cond_id
         else:
-            # datasetId_list will be created (possibly overwriting previous
-            # list - only in the local variable, not in the tsv-file)
-            # check consistency of settings
-            group_by = check_vis_spec_consistency(exp_data,
-                                                  dataset_id_list,
-                                                  sim_cond_id_list,
-                                                  sim_cond_num_list,
-                                                  observable_id_list,
-                                                  observable_num_list)
-            observable_id_list = \
-                [[el] for el in exp_data.observableId.unique()]
-
-            exp_data, dataset_id_list, legend_dict, _ = create_dataset_id_list(
-                sim_cond_id_list, sim_cond_num_list, observable_id_list,
-                observable_num_list, exp_data, exp_conditions, group_by)
-
-    return exp_data, dataset_id_list, legend_dict
-
-
-def handle_dataset_plot(plot_spec: pd.Series,
-                        ax: plt.Axes,
-                        exp_data: pd.DataFrame,
-                        exp_conditions: pd.DataFrame,
-                        sim_data: pd.DataFrame):
-    """
-    Handle dataset plot
-    """
-    # get datasetID and independent variable of first entry of plot1
-    dataset_id = plot_spec[DATASET_ID]
-    indep_var = plot_spec[X_VALUES]
-
-    # define index to reduce exp_data to data linked to datasetId
-    ind_dataset = exp_data[DATASET_ID] == dataset_id
-
-    # gather simulationConditionIds belonging to datasetId
-    uni_condition_id, uind = np.unique(
-        exp_data[ind_dataset][SIMULATION_CONDITION_ID],
-        return_index=True)
-    # keep the ordering which was given by user from top to bottom
-    # (avoid ordering by names '1','10','11','2',...)'
-    uni_condition_id = uni_condition_id[np.argsort(uind)]
-    col_name_unique = SIMULATION_CONDITION_ID
-
-    # Case separation of independent parameter: condition, time or custom
-    if indep_var == TIME:
-        # obtain unique observation times
-        uni_condition_id = np.unique(exp_data[ind_dataset][TIME])
-        col_name_unique = TIME
-        conditions = uni_condition_id
-    elif indep_var == 'condition':
-        conditions = None
-    else:
-        # extract conditions (plot input) from condition file
-        ind_cond = exp_conditions.index.isin(uni_condition_id)
-        conditions = exp_conditions[ind_cond][indep_var]
-
-    # retrieve measurements from dataframes
-    measurement_to_plot = get_data_to_plot(plot_spec, exp_data, sim_data,
-                                           uni_condition_id, col_name_unique)
-
-    # check, whether simulation should be plotted
-    plot_sim = sim_data is not None
-
-    # plot data
-    nan_set = all([np.isnan(val) for val in measurement_to_plot['mean']])
-    if not nan_set:
-        plot_lowlevel(plot_spec, ax, conditions, measurement_to_plot, plot_sim)
-
-    # Beautify plots
-    ax.set_xlabel(
-        plot_spec.xLabel)
-    ax.set_ylabel(
-        plot_spec.yLabel)
-
-
-def matches_plot_spec(df: pd.DataFrame,
-                      col_id: str,
-                      x_value: Union[float, str],
-                      plot_spec: pd.Series) -> pd.Series:
-    """
-    constructs an index for subsetting of the dataframe according to what is
-    specified in plot_spec.
-
-    Parameters:
-        df:
-            pandas data frame to subset, can be from measurement file or
-            simulation file
-        col_id:
-            name of the column that will be used for indexing in x variable
-        x_value:
-            subsetted x value
-        plot_spec:
-            visualization spec from the visualization file
-
-    Returns:
-        index:
-            Boolean series that can be used for subsetting of the passed
-            dataframe
-    """
-    subset = (
-        (df[col_id] == x_value) &
-        (df[DATASET_ID] == plot_spec[DATASET_ID])
-    )
-    if plot_spec[Y_VALUES] == '':
-        if len(df.loc[subset, OBSERVABLE_ID].unique()) > 1:
-            ValueError(
-                f'{Y_VALUES} must be specified in visualization table if '
-                f'multiple different observables are available.'
-            )
-    else:
-        subset &= (df[OBSERVABLE_ID] == plot_spec[Y_VALUES])
-    return subset
-
-
-def get_data_to_plot(plot_spec: pd.Series,
-                     m_data: pd.DataFrame,
-                     simulation_data: pd.DataFrame,
-                     condition_ids: np.ndarray,
-                     col_id: str,
-                     simulation_field: str = SIMULATION) -> pd.DataFrame:
-    """
-    Group the data, which should be plotted and return it as dataframe.
-
-    Parameters:
-        plot_spec:
-            information about contains defined data format (visualization file)
-        m_data:
-            contains defined data format (measurement file)
-        simulation_data:
-            contains defined data format (simulation file)
-        condition_ids:
-            contains all unique condition IDs which should be
-            plotted in one figure (can be found in measurementData file,
-            column simulationConditionId)
-        col_id:
-            the name of the column in visualization file, whose entries
-            should be unique (depends on condition in column
-            xValues)
-        simulation_field:
-            Column name in ``simulation_data`` that contains the actual
-            simulation result.
-
-    Returns:
-        data_to_plot:
-            Contains the data which should be plotted
-            (Mean and Std)
-    """
-
-    # create empty dataframe for means and SDs
-    data_to_plot = pd.DataFrame(
-        columns=['mean', 'noise_model', 'sd', 'sem', 'repl', 'sim'],
-        index=condition_ids
-    )
-
-    for var_cond_id in condition_ids:
-
-        # TODO (#117): Here not the case: So, if entries in measurement file:
-        #  preequCondId, time, observableParams, noiseParams,
-        #  are not the same, then  -> differ these data into
-        #  different groups!
-        # now: go in simulationConditionId, search group of unique
-        # simulationConditionId e.g. rows 0,6,12,18 share the same
-        # simulationCondId, then check if other column entries are the same
-        # (now: they are), then take intersection of rows 0,6,12,18 and checked
-        # other same columns (-> now: 0,6,12,18) and then go on with code.
-        # if there is at some point a difference in other columns, say e.g.
-        # row 12,18 have different noiseParams than rows 0,6, the actual code
-        # would take rows 0,6 and forget about rows 12,18
-
-        # compute mean and standard deviation across replicates
-        subset = matches_plot_spec(m_data, col_id, var_cond_id, plot_spec)
-        data_measurements = m_data.loc[
-            subset,
-            MEASUREMENT
-        ]
-
-        data_to_plot.at[var_cond_id, 'mean'] = np.mean(data_measurements)
-        data_to_plot.at[var_cond_id, 'sd'] = np.std(data_measurements)
-
-        if (plot_spec.plotTypeData == PROVIDED) & sum(subset):
-            if len(m_data.loc[subset, NOISE_PARAMETERS].unique()) > 1:
-                raise NotImplementedError(
-                    f"Datapoints with inconsistent {NOISE_PARAMETERS} is "
-                    f"currently not implemented. Stopping.")
-            tmp_noise = m_data.loc[subset, NOISE_PARAMETERS].values[0]
-            if isinstance(tmp_noise, str):
-                raise NotImplementedError(
-                    "No numerical noise values provided in the measurement "
-                    "table. Stopping.")
-            if isinstance(tmp_noise, Number) or tmp_noise.dtype == 'float64':
-                data_to_plot.at[var_cond_id, 'noise_model'] = tmp_noise
-
-        # standard error of mean
-        data_to_plot.at[var_cond_id, 'sem'] = \
-            np.std(data_measurements) / np.sqrt(len(data_measurements))
-
-        # single replicates
-        data_to_plot.at[var_cond_id, 'repl'] = \
-            data_measurements
-
-        if simulation_data is not None:
-            simulation_measurements = simulation_data.loc[
-                matches_plot_spec(simulation_data, col_id, var_cond_id,
-                                  plot_spec),
-                simulation_field
+            cond_name = tmp[CONDITION_NAME]
+        return f'{cond_name} - {obs_id}'
+
+    def _expand_vis_spec_settings(self, vis_spec: pd.DataFrame):
+        """
+        Expand visualization specification for the case when DATASET_ID is not
+        in vis_spec.columns.
+
+        Parameters
+        -------
+        vis_spec:
+            Visualization specification DataFrame in the PEtab format
+            or a path to a visualization file.
+
+        Returns
+        -------
+        A visualization specification DataFrame.
+        """
+        if DATASET_ID in vis_spec.columns:
+            raise ValueError(f"visualization specification expansion is "
+                             f"unnecessary if column {DATASET_ID} is present")
+
+        if vis_spec.empty:
+            # in case of empty spec all measurements corresponding to each
+            # observable will be plotted on a separate subplot
+            observable_ids = self._data_df[OBSERVABLE_ID].unique()
+
+            vis_spec_exp_rows = [
+                self._vis_spec_rows_for_obs(obs_id, {PLOT_ID: f'plot{idx}'})
+                for idx, obs_id in enumerate(observable_ids)
             ]
-            data_to_plot.at[var_cond_id, 'sim'] = np.mean(
-                simulation_measurements
-            )
+            return pd.concat(vis_spec_exp_rows, ignore_index=True)
+
+        vis_spec_exp_rows = []
+        for _, row in vis_spec.iterrows():
+            if Y_VALUES in row:
+                vis_spec_exp_rows.append(
+                    self._vis_spec_rows_for_obs(row[Y_VALUES], row.to_dict())
+                )
+            else:
+                observable_ids = self._data_df[OBSERVABLE_ID].unique()
 
-    return data_to_plot
+                for obs_id in observable_ids:
+                    vis_spec_exp_rows.append(
+                        self._vis_spec_rows_for_obs(obs_id, row.to_dict())
+                    )
+        return pd.concat(vis_spec_exp_rows, ignore_index=True)
+
+    def _vis_spec_rows_for_obs(self, obs_id: str, settings: dict
+                               ) -> pd.DataFrame:
+        """
+        Create vis_spec for one observable.
+
+        For each dataset_id corresponding to the observable with the specified
+        id create a vis_spec entry with provided settings.
+
+        Parameters
+        ----------
+        obs_id:
+            Observable ID.
+        settings:
+            Additional visualization settings. For each key that is a
+            valid visualization specification column name, the setting
+            will be added to the resulting visualization specification.
+
+        Returns
+        -------
+        A visualization specification DataFrame.
+        """
+        columns_to_expand = [PLOT_ID, PLOT_NAME, PLOT_TYPE_SIMULATION,
+                             PLOT_TYPE_DATA, X_VALUES, X_OFFSET, X_LABEL,
+                             X_SCALE, Y_OFFSET, Y_LABEL, Y_SCALE,
+                             LEGEND_ENTRY]
+
+        dataset_ids = self._data_df[
+            self._data_df[OBSERVABLE_ID] ==
+            obs_id][DATASET_ID].unique()
+        n_rows = len(dataset_ids)
+        columns_dict = {DATASET_ID: dataset_ids,
+                        Y_VALUES: [obs_id] * n_rows}
+
+        for column in settings:
+            if column in columns_to_expand:
+                columns_dict[column] = [settings[column]] * n_rows
+
+        if LEGEND_ENTRY not in columns_dict:
+            columns_dict[LEGEND_ENTRY] = \
+                [self._create_legend(dataset_id) for dataset_id
+                 in columns_dict[DATASET_ID]]
+        return pd.DataFrame(columns_dict)
```

### Comparing `petab-0.1.8/petab/observables.py` & `petab-0.2.0/petab/observables.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 """Functions for working with the PEtab observables table"""
 
-from _collections import OrderedDict
-from typing import Union, List
+import re
+from collections import OrderedDict
+from pathlib import Path
+from typing import List, Literal, Union
 
-import libsbml
 import pandas as pd
-import re
 import sympy as sp
+from sympy.abc import _clash
 
-from . import lint, core
+from . import core, lint
 from .C import *  # noqa: F403
+from .models import Model
+
+__all__ = [
+    'create_observable_df',
+    'get_formula_placeholders',
+    'get_observable_df',
+    'get_output_parameters',
+    'get_placeholders',
+    'write_observable_df'
+]
 
 
 def get_observable_df(
-        observable_file: Union[str, pd.DataFrame, None]
-) -> pd.DataFrame:
+        observable_file: Union[str, pd.DataFrame, Path, None]
+) -> Union[pd.DataFrame, None]:
     """
     Read the provided observable file into a ``pandas.Dataframe``.
 
     Arguments:
         observable_file: Name of the file to read from or pandas.Dataframe.
 
     Returns:
         Observable DataFrame
     """
     if observable_file is None:
         return observable_file
 
-    if isinstance(observable_file, str):
+    if isinstance(observable_file, (str, Path)):
         observable_file = pd.read_csv(observable_file, sep='\t',
                                       float_precision='round_trip')
 
     lint.assert_no_leading_trailing_whitespace(
         observable_file.columns.values, "observable")
 
     if not isinstance(observable_file.index, pd.RangeIndex):
@@ -42,66 +53,88 @@
     except KeyError:
         raise KeyError(
             f"Observable table missing mandatory field {OBSERVABLE_ID}.")
 
     return observable_file
 
 
-def write_observable_df(df: pd.DataFrame, filename: str) -> None:
+def write_observable_df(df: pd.DataFrame, filename: Union[str, Path]) -> None:
     """Write PEtab observable table
 
     Arguments:
         df: PEtab observable table
         filename: Destination file name
     """
-    with open(filename, 'w') as fh:
-        df.to_csv(fh, sep='\t', index=True)
+    df = get_observable_df(df)
+    df.to_csv(filename, sep='\t', index=True)
 
 
-def get_output_parameters(observable_df: pd.DataFrame,
-                          sbml_model: libsbml.Model) -> List[str]:
+def get_output_parameters(
+        observable_df: pd.DataFrame,
+        model: Model,
+        observables: bool = True,
+        noise: bool = True,
+        mapping_df: pd.DataFrame = None
+) -> List[str]:
     """Get output parameters
 
     Returns IDs of parameters used in observable and noise formulas that are
-    not defined in the SBML model.
+    not defined in the model.
 
     Arguments:
         observable_df: PEtab observable table
-        sbml_model: SBML model
+        model: The underlying model
+        observables: Include parameters from observableFormulas
+        noise: Include parameters from noiseFormulas
+        mapping_df: PEtab mapping table
 
     Returns:
         List of output parameter IDs
     """
-    formulas = list(observable_df[OBSERVABLE_FORMULA])
-    if NOISE_FORMULA in observable_df:
+    formulas = []
+    if observables:
+        formulas.extend(observable_df[OBSERVABLE_FORMULA])
+    if noise and NOISE_FORMULA in observable_df:
         formulas.extend(observable_df[NOISE_FORMULA])
     output_parameters = OrderedDict()
 
     for formula in formulas:
-        free_syms = sorted(sp.sympify(formula).free_symbols,
+        free_syms = sorted(sp.sympify(formula, locals=_clash).free_symbols,
                            key=lambda symbol: symbol.name)
         for free_sym in free_syms:
             sym = str(free_sym)
-            if sbml_model.getElementBySId(sym) is None and sym != 'time':
-                output_parameters[sym] = None
+            if model.symbol_allowed_in_observable_formula(sym):
+                continue
+
+            # does it mapping to a model entity?
+            if mapping_df is not None \
+                    and sym in mapping_df.index \
+                    and model.symbol_allowed_in_observable_formula(
+                    mapping_df.loc[sym, MODEL_ENTITY_ID]):
+                continue
+
+            output_parameters[sym] = None
 
     return list(output_parameters.keys())
 
 
-def get_formula_placeholders(formula_string: str, observable_id: str,
-                             override_type: str) -> List[str]:
+def get_formula_placeholders(
+        formula_string: str,
+        observable_id: str,
+        override_type: Literal['observable', 'noise'],
+) -> List[str]:
     """
     Get placeholder variables in noise or observable definition for the
     given observable ID.
 
     Arguments:
         formula_string: observable formula
         observable_id: ID of current observable
-        override_type: 'observable' or 'noise', depending on whether `formula`
-            is for observable or for noise model
+        override_type: ``'observable'`` or ``'noise'``, depending on whether
+            ``formula`` is for observable or for noise model
 
     Returns:
         List of placeholder parameter IDs in the order expected in the
         observableParameter column of the measurement table.
     """
     if not formula_string:
         return []
@@ -121,33 +154,47 @@
     if placeholder_set != set(placeholders):
         raise AssertionError("Non-consecutive numbering of placeholder "
                              f"parameter for {placeholder_set}")
 
     return placeholders
 
 
-def get_placeholders(observable_df: pd.DataFrame) -> List[str]:
+def get_placeholders(
+        observable_df: pd.DataFrame,
+        observables: bool = True,
+        noise: bool = True,
+) -> List[str]:
     """Get all placeholder parameters from observable table observableFormulas
     and noiseFormulas
 
     Arguments:
         observable_df: PEtab observable table
+        observables: Include parameters from observableFormulas
+        noise: Include parameters from noiseFormulas
 
     Returns:
         List of placeholder parameters from observable table observableFormulas
         and noiseFormulas.
     """
 
     # collect placeholder parameters overwritten by
     # {observable,noise}Parameters
+    placeholder_types = []
+    formula_columns = []
+    if observables:
+        placeholder_types.append('observable')
+        formula_columns.append(OBSERVABLE_FORMULA)
+    if noise:
+        placeholder_types.append('noise')
+        formula_columns.append(NOISE_FORMULA)
+
     placeholders = []
     for _, row in observable_df.iterrows():
         for placeholder_type, formula_column \
-                in zip(['observable', 'noise'],
-                       [OBSERVABLE_FORMULA, NOISE_FORMULA]):
+                in zip(placeholder_types, formula_columns):
             if formula_column not in row:
                 continue
 
             cur_placeholders = get_formula_placeholders(
                 row[formula_column], row.name, placeholder_type)
             placeholders.extend(cur_placeholders)
     return core.unique_preserve_order(placeholders)
@@ -156,10 +203,8 @@
 def create_observable_df() -> pd.DataFrame:
     """Create empty observable dataframe
 
     Returns:
         Created DataFrame
     """
 
-    df = pd.DataFrame(data={col: [] for col in OBSERVABLE_DF_COLS})
-
-    return df
+    return pd.DataFrame(data={col: [] for col in OBSERVABLE_DF_COLS})
```

### Comparing `petab-0.1.8/petab/lint.py` & `petab-0.2.0/petab/problem.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,855 +1,891 @@
-"""Integrity checks and tests for specific features used"""
+"""PEtab Problem class"""
+from __future__ import annotations
 
-import copy
-import logging
-import numbers
-import re
-from typing import Optional, Iterable
-from collections import Counter
+import os
+import tempfile
+from pathlib import Path, PurePosixPath
+from typing import Dict, Iterable, List, Optional, Union, TYPE_CHECKING
+from urllib.parse import unquote, urlparse, urlunparse
+from warnings import warn
 
-import libsbml
-import numpy as np
 import pandas as pd
-import sympy as sp
 
-import petab
-from . import (core, parameters, sbml, measurements)
+from . import (conditions, core, format_version, measurements, observables,
+               parameter_mapping, parameters, sampling, sbml, yaml, mapping)
 from .C import *  # noqa: F403
+from .models import MODEL_TYPE_SBML
+from .models.model import Model, model_factory
+from .models.sbml_model import SbmlModel
 
-logger = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    import libsbml
 
 
-def _check_df(df: pd.DataFrame, req_cols: Iterable, name: str) -> None:
-    """Check if given columns are present in DataFrame
+__all__ = ['Problem']
 
-    Arguments:
-        df: Dataframe to check
-        req_cols: Column names which have to be present
-        name: Name of the DataFrame to be included in error message
 
-    Raises:
-          AssertionError: if a column is missing
+class Problem:
     """
-    cols_set = df.columns.values
-    missing_cols = set(req_cols) - set(cols_set)
-    if missing_cols:
-        raise AssertionError(
-            f"DataFrame {name} requires the columns {missing_cols}.")
-
-
-def assert_no_leading_trailing_whitespace(
-        names_list: Iterable[str], name: str) -> None:
-    """Check that there is no trailing whitespace in elements of Iterable
-
-    Arguments:
-        names_list: strings to check for whitespace
-        name: name of `names_list` for error messages
+    PEtab parameter estimation problem as defined by
 
-    Raises:
-        AssertionError: if there is trailing whitespace
-    """
-    r = re.compile(r'(?:^\s)|(?:\s$)')
-    for i, x in enumerate(names_list):
-        if isinstance(x, str) and r.search(x):
-            raise AssertionError(f"Whitespace around {name}[{i}] = '{x}'.")
-
-
-def check_condition_df(
-        df: pd.DataFrame, sbml_model: Optional[libsbml.Model]) -> None:
-    """Run sanity checks on PEtab condition table
-
-    Arguments:
-        df: PEtab condition DataFrame
-        sbml_model: SBML Model for additional checking of parameter IDs
-
-    Raises:
-        AssertionError: in case of problems
-    """
-
-    # Check required columns are present
-    req_cols = []
-    _check_df(df, req_cols, "condition")
-
-    # Check for correct index
-    if not df.index.name == CONDITION_ID:
-        raise AssertionError(
-            f"Condition table has wrong index {df.index.name}."
-            f"expected {CONDITION_ID}.")
-
-    check_ids(df.index.values, kind='condition')
-
-    for column_name in req_cols:
-        if not np.issubdtype(df[column_name].dtype, np.number):
-            assert_no_leading_trailing_whitespace(
-                df[column_name].values, column_name)
-
-    if sbml_model is not None:
-        for column_name in df.columns:
-            if column_name != CONDITION_NAME \
-                    and sbml_model.getParameter(column_name) is None \
-                    and sbml_model.getSpecies(column_name) is None \
-                    and sbml_model.getCompartment(column_name) is None:
-                raise AssertionError(
-                    "Condition table contains column for unknown entity '"
-                    f"{column_name}'. Column names must match parameter, "
-                    "species or compartment IDs specified in the SBML model.")
-
-
-def check_measurement_df(df: pd.DataFrame,
-                         observable_df: Optional[pd.DataFrame] = None) -> None:
-    """Run sanity checks on PEtab measurement table
-
-    Arguments:
-        df: PEtab measurement DataFrame
-        observable_df: PEtab observable DataFrame for checking if measurements
-            are compatible with observable transformations.
-
-    Raises:
-        AssertionError, ValueError: in case of problems
-    """
+    - model
+    - condition table
+    - measurement table
+    - parameter table
+    - observables table
+    - mapping table
 
-    _check_df(df, MEASUREMENT_DF_REQUIRED_COLS, "measurement")
+    Optionally it may contain visualization tables.
 
-    for column_name in MEASUREMENT_DF_REQUIRED_COLS:
-        if not np.issubdtype(df[column_name].dtype, np.number):
-            assert_no_leading_trailing_whitespace(
-                df[column_name].values, column_name)
-
-    for column_name in MEASUREMENT_DF_OPTIONAL_COLS:
-        if column_name in df \
-                and not np.issubdtype(df[column_name].dtype, np.number):
-            assert_no_leading_trailing_whitespace(
-                df[column_name].values, column_name)
-
-    if observable_df is not None:
-        # Check all observables are defined
-        observables_defined = set(observable_df.index.values)
-        observables_used = set(df[OBSERVABLE_ID])
-        observables_undefined = observables_used - observables_defined
-        if observables_undefined:
-            raise ValueError(f"Observables {observables_undefined} used in "
-                             "measurement table but not defined in "
-                             "observables table.")
-
-        if OBSERVABLE_TRANSFORMATION in observable_df:
-            # Check for positivity of measurements in case of
-            #  log-transformation
-            assert_unique_observable_ids(observable_df)
-            # If the above is not checked, in the following loop
-            # trafo may become a pandas Series
-            for measurement, obs_id in zip(df[MEASUREMENT], df[OBSERVABLE_ID]):
-                trafo = observable_df.loc[obs_id, OBSERVABLE_TRANSFORMATION]
-                if measurement <= 0.0 and trafo in [LOG, LOG10]:
-                    raise ValueError('Measurements with observable '
-                                     f'transformation {trafo} must be '
-                                     f'positive, but {measurement} <= 0.')
-
-    if observable_df is not None:
-        assert_measured_observables_defined(df, observable_df)
-        measurements.assert_overrides_match_parameter_count(
-            df, observable_df)
-
-
-def check_parameter_df(
-        df: pd.DataFrame,
-        sbml_model: Optional[libsbml.Model] = None,
-        observable_df: Optional[pd.DataFrame] = None,
-        measurement_df: Optional[pd.DataFrame] = None,
-        condition_df: Optional[pd.DataFrame] = None) -> None:
-    """Run sanity checks on PEtab parameter table
-
-    Arguments:
-        df: PEtab condition DataFrame
-        sbml_model: SBML Model for additional checking of parameter IDs
-        observable_df: PEtab observable table for additional checks
-        measurement_df: PEtab measurement table for additional checks
-        condition_df: PEtab condition table for additional checks
-
-    Raises:
-        AssertionError: in case of problems
-    """
-
-    _check_df(df, PARAMETER_DF_REQUIRED_COLS[1:], "parameter")
-
-    if not df.index.name == PARAMETER_ID:
-        raise AssertionError(
-            f"Parameter table has wrong index {df.index.name}."
-            f"expected {PARAMETER_ID}.")
-
-    check_ids(df.index.values, kind='parameter')
-
-    for column_name in PARAMETER_DF_REQUIRED_COLS[1:]:  # 0 is PARAMETER_ID
-        if not np.issubdtype(df[column_name].dtype, np.number):
-            assert_no_leading_trailing_whitespace(
-                df[column_name].values, column_name)
-
-    # nominal value is generally optional, but required if any for any
-    #  parameter estimate != 1
-    non_estimated_par_ids = list(
-        df.index[(df[ESTIMATE] != 1) | (
-            pd.api.types.is_string_dtype(df[ESTIMATE])
-            and df[ESTIMATE] != '1')])
-    if non_estimated_par_ids:
-        if NOMINAL_VALUE not in df:
-            raise AssertionError("Parameter table contains parameters "
-                                 f"{non_estimated_par_ids} that are not "
-                                 "specified to be estimated, "
-                                 f"but column {NOMINAL_VALUE} is missing.")
-        try:
-            df.loc[non_estimated_par_ids, NOMINAL_VALUE].apply(float)
-        except ValueError:
-            raise AssertionError("Expected numeric values for "
-                                 f"`{NOMINAL_VALUE}` in parameter table for "
-                                 "all non-estimated parameters.")
-
-    assert_parameter_id_is_string(df)
-    assert_parameter_scale_is_valid(df)
-    assert_parameter_bounds_are_numeric(df)
-    assert_parameter_estimate_is_boolean(df)
-    assert_unique_parameter_ids(df)
-    check_parameter_bounds(df)
-    assert_parameter_prior_type_is_valid(df)
-
-    if sbml_model and measurement_df is not None \
-            and condition_df is not None:
-        assert_all_parameters_present_in_parameter_df(
-            df, sbml_model, observable_df, measurement_df, condition_df)
-
-
-def check_observable_df(observable_df: pd.DataFrame) -> None:
-    """Check validity of observable table
-
-    Arguments:
-        observable_df: PEtab observable DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-    """
-    _check_df(observable_df, OBSERVABLE_DF_REQUIRED_COLS[1:], "observable")
-
-    check_ids(observable_df.index.values, kind='observable')
-
-    for column_name in OBSERVABLE_DF_REQUIRED_COLS[1:]:
-        if not np.issubdtype(observable_df[column_name].dtype, np.number):
-            assert_no_leading_trailing_whitespace(
-                observable_df[column_name].values, column_name)
-
-    for column_name in OBSERVABLE_DF_OPTIONAL_COLS:
-        if column_name in observable_df \
-                and not np.issubdtype(observable_df[column_name].dtype,
-                                      np.number):
-            assert_no_leading_trailing_whitespace(
-                observable_df[column_name].values, column_name)
-
-    assert_noise_distributions_valid(observable_df)
-    assert_unique_observable_ids(observable_df)
-
-    # Check that formulas are parsable
-    for row in observable_df.itertuples():
-        obs = getattr(row, OBSERVABLE_FORMULA)
-        try:
-            sp.sympify(obs)
-        except sp.SympifyError as e:
-            raise AssertionError(f"Cannot parse expression '{obs}' "
-                                 f"for observable {row.Index}: {e}")
-
-        noise = getattr(row, NOISE_FORMULA)
-        try:
-            sp.sympify(noise)
-        except sp.SympifyError as e:
-            raise AssertionError(f"Cannot parse expression '{noise}' "
-                                 f"for noise model for observable "
-                                 f"{row.Index}: {e}")
-
-
-def assert_all_parameters_present_in_parameter_df(
-        parameter_df: pd.DataFrame,
-        sbml_model: libsbml.Model,
-        observable_df: pd.DataFrame,
-        measurement_df: pd.DataFrame,
-        condition_df: pd.DataFrame) -> None:
-    """Ensure all required parameters are contained in the parameter table
-    with no additional ones
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-        sbml_model: PEtab SBML Model
-        observable_df: PEtab observable table
-        measurement_df: PEtab measurement table
+    Attributes:
         condition_df: PEtab condition table
-
-    Raises:
-        AssertionError: in case of problems
-    """
-
-    required = parameters.get_required_parameters_for_parameter_table(
-        sbml_model=sbml_model, condition_df=condition_df,
-        observable_df=observable_df, measurement_df=measurement_df)
-
-    allowed = parameters.get_valid_parameters_for_parameter_table(
-        sbml_model=sbml_model, condition_df=condition_df,
-        observable_df=observable_df, measurement_df=measurement_df)
-
-    actual = set(parameter_df.index)
-
-    missing = required - actual
-    extraneous = actual - allowed
-
-    if missing:
-        raise AssertionError('Missing parameter(s) in parameter table: '
-                             + str(missing))
-
-    if extraneous:
-        raise AssertionError('Extraneous parameter(s) in parameter table: '
-                             + str(extraneous))
-
-
-def assert_measured_observables_defined(
-        measurement_df: pd.DataFrame,
-        observable_df: pd.DataFrame) -> None:
-    """Check if all observables in the measurement table have been defined in the
-    observable table
-
-    Arguments:
         measurement_df: PEtab measurement table
+        parameter_df: PEtab parameter table
         observable_df: PEtab observable table
+        visualization_df: PEtab visualization table
+        mapping_df: PEtab mapping table
+        model: The underlying model
+        sbml_reader: Stored to keep object alive (deprecated).
+        sbml_document: Stored to keep object alive (deprecated).
+        sbml_model: PEtab SBML model (deprecated)
+        extensions_config: Information on the extensions used
+    """
+
+    def __init__(
+            self,
+            sbml_model: libsbml.Model = None,
+            sbml_reader: libsbml.SBMLReader = None,
+            sbml_document: libsbml.SBMLDocument = None,
+            model: Model = None,
+            model_id: str = None,
+            condition_df: pd.DataFrame = None,
+            measurement_df: pd.DataFrame = None,
+            parameter_df: pd.DataFrame = None,
+            visualization_df: pd.DataFrame = None,
+            observable_df: pd.DataFrame = None,
+            mapping_df: pd.DataFrame = None,
+            extensions_config: Dict = None,
+    ):
+        self.condition_df: Optional[pd.DataFrame] = condition_df
+        self.measurement_df: Optional[pd.DataFrame] = measurement_df
+        self.parameter_df: Optional[pd.DataFrame] = parameter_df
+        self.visualization_df: Optional[pd.DataFrame] = visualization_df
+        self.observable_df: Optional[pd.DataFrame] = observable_df
+        self.mapping_df: Optional[pd.DataFrame] = mapping_df
+
+        if any((sbml_model, sbml_document, sbml_reader),):
+            warn("Passing `sbml_model`, `sbml_document`, or `sbml_reader` "
+                 "to petab.Problem is deprecated and will be removed in a "
+                 "future version. Use `model=petab.models.sbml_model."
+                 "SbmlModel(...)` instead.", DeprecationWarning, stacklevel=2)
+            if model:
+                raise ValueError("Must only provide one of (`sbml_model`, "
+                                 "`sbml_document`, `sbml_reader`) or `model`.")
+
+            model = SbmlModel(
+                sbml_model=sbml_model,
+                sbml_reader=sbml_reader,
+                sbml_document=sbml_document,
+                model_id=model_id
+            )
 
-    Raises:
-        AssertionError: in case of problems
-    """
-
-    used_observables = set(measurement_df[OBSERVABLE_ID].values)
-    defined_observables = set(observable_df.index.values)
-    undefined_observables = used_observables - defined_observables
-
-    if undefined_observables:
-        raise AssertionError(
-            "Undefined observables in measurement file: "
-            f"{undefined_observables}.")
-
-
-def condition_table_is_parameter_free(condition_df: pd.DataFrame) -> bool:
-    """Check if all entries in the condition table are numeric
-    (no parameter IDs)
-
-    Arguments:
-        condition_df: PEtab condition table
-
-    Returns:
-        True if there are no parameter overrides in the condition table,
-        False otherwise.
-    """
-
-    return len(petab.get_parametric_overrides(condition_df)) == 0
-
-
-def assert_parameter_id_is_string(parameter_df: pd.DataFrame) -> None:
-    """
-    Check if all entries in the parameterId column of the parameter table
-    are string and not empty.
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-    """
+        self.model: Optional[Model] = model
+        self.extensions_config = extensions_config or {}
 
-    for parameter_id in parameter_df:
-        if isinstance(parameter_id, str):
-            if parameter_id[0].isdigit():
-                raise AssertionError(
-                    f"{PARAMETER_ID} {parameter_id} starts with integer.")
+    def __getattr__(self, name):
+        # For backward-compatibility, allow access to SBML model related
+        #  attributes now stored in self.model
+        if name in {'sbml_model', 'sbml_reader', 'sbml_document'}:
+            return getattr(self.model, name) if self.model else None
+        raise AttributeError(f"'{self.__class__.__name__}' object has no "
+                             f"attribute '{name}'")
+
+    def __setattr__(self, name, value):
+        # For backward-compatibility, allow access to SBML model related
+        #  attributes now stored in self.model
+        if name in {'sbml_model', 'sbml_reader', 'sbml_document'}:
+            if self.model:
+                setattr(self.model, name, value)
+            else:
+                self.model = SbmlModel(**{name: value})
         else:
-            raise AssertionError(f"Empty {PARAMETER_ID} found.")
-
-
-def assert_unique_parameter_ids(parameter_df: pd.DataFrame) -> None:
-    """
-    Check if the parameterId column of the parameter table is unique.
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-    """
-    non_unique_ids = get_non_unique(parameter_df.index)
-    if len(non_unique_ids) > 0:
-        raise AssertionError(
-            f"Non-unique values found in the {PARAMETER_ID} column"
-            " of the parameter table: " + str(non_unique_ids))
-
-
-def assert_parameter_scale_is_valid(parameter_df: pd.DataFrame) -> None:
-    """
-    Check if all entries in the parameterScale column of the parameter table
-    are 'lin' for linear, 'log' for natural logarithm or 'log10' for base 10
-    logarithm.
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-    """
-    for parameter_scale in parameter_df[PARAMETER_SCALE]:
-        if parameter_scale not in [LIN, LOG, LOG10]:
-            raise AssertionError(f"Expected {LIN}, {LOG}, or {LOG10}, but "
-                                 f"got {parameter_scale}.")
-
-
-def assert_parameter_bounds_are_numeric(parameter_df: pd.DataFrame) -> None:
-    """
-    Check if all entries in the lowerBound and upperBound columns of the
-    parameter table are numeric.
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-    """
-    parameter_df[LOWER_BOUND].apply(float).all()
-    parameter_df[UPPER_BOUND].apply(float).all()
-
-
-def check_parameter_bounds(parameter_df: pd.DataFrame) -> None:
-    """
-    Check if all entries in the lowerBound are smaller than upperBound column
-    in the parameter table and that bounds are positive for parameterScale
-    log|log10.
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-
-    """
-    for _, row in parameter_df.iterrows():
-        if int(row[ESTIMATE]):
-            if not row[LOWER_BOUND] <= row[UPPER_BOUND]:
-                raise AssertionError(
-                    f"{LOWER_BOUND} greater than {UPPER_BOUND} for "
-                    f"{PARAMETER_ID} {row.name}.")
-            if (row[LOWER_BOUND] <= 0.0 or row[UPPER_BOUND] < 0.0) \
-                    and row[PARAMETER_SCALE] in [LOG, LOG10]:
-                raise AssertionError(
-                    f"Bounds for {row[PARAMETER_SCALE]} scaled parameter "
-                    f"{ row.name} must be positive.")
-
-
-def assert_parameter_prior_type_is_valid(
-        parameter_df: pd.DataFrame) -> None:
-    """Check that valid prior types have been selected
-
-    Arguments:
-        parameter_df: PEtab parameter table
-
-    Raises:
-        AssertionError in case of invalid prior
-    """
-    for col in [INITIALIZATION_PRIOR_TYPE, OBJECTIVE_PRIOR_TYPE]:
-        if col not in parameter_df.columns:
-            continue
-        for _, row in parameter_df.iterrows():
-            if row[col] not in PRIOR_TYPES and not core.is_empty(row[col]):
-                raise AssertionError(
-                    f"{col} must be one of {PRIOR_TYPES} but is "
-                    f"'{row[col]}'.")
+            super().__setattr__(name, value)
 
+    def __str__(self):
+        model = f"with model ({self.model})" if self.model else "without model"
+        conditions = f"{self.condition_df.shape[0]} conditions" \
+            if self.condition_df is not None else "without conditions table"
+
+        observables = f"{self.observable_df.shape[0]} observables" \
+            if self.observable_df is not None else "without observables table"
+
+        measurements = f"{self.measurement_df.shape[0]} measurements" \
+            if self.measurement_df is not None \
+            else "without measurements table"
+
+        if self.parameter_df is not None:
+            num_estimated_parameters = sum(self.parameter_df[ESTIMATE] == 1) \
+                if ESTIMATE in self.parameter_df \
+                else self.parameter_df.shape[0]
+            parameters = f"{num_estimated_parameters} estimated parameters"
+        else:
+            parameters = "without parameter_df table"
 
-def assert_parameter_prior_parameters_are_valid(
-        parameter_df: pd.DataFrame) -> None:
-    """Check that the prior parameters are valid.
-
-    Arguments:
-        parameter_df: PEtab parameter table
-
-    Raises:
-        AssertionError in case of invalide prior parameters
-    """
-    prior_type_cols = [INITIALIZATION_PRIOR_TYPE,
-                       OBJECTIVE_PRIOR_TYPE]
-    prior_par_cols = [INITIALIZATION_PRIOR_PARAMETERS,
-                      OBJECTIVE_PRIOR_PARAMETERS]
-
-    # perform test for both priors
-    for type_col, par_col in zip(prior_type_cols, prior_par_cols):
-        # iterate over rows
-        for _, row in parameter_df.iterrows():
-            # get type
-            if type_col not in row or core.is_empty(row[type_col]):
-                type_ = PARAMETER_SCALE_UNIFORM
+        return (
+            f"PEtab Problem {model}, {conditions}, {observables}, "
+            f"{measurements}, {parameters}"
+        )
+
+    @staticmethod
+    def from_files(
+            sbml_file: Union[str, Path] = None,
+            condition_file:
+            Union[str, Path, Iterable[Union[str, Path]]] = None,
+            measurement_file: Union[str, Path,
+                                    Iterable[Union[str, Path]]] = None,
+            parameter_file: Union[str, Path,
+                                  Iterable[Union[str, Path]]] = None,
+            visualization_files: Union[str, Path,
+                                       Iterable[Union[str, Path]]] = None,
+            observable_files: Union[str, Path,
+                                    Iterable[Union[str, Path]]] = None,
+            model_id: str = None,
+            extensions_config: Dict = None,
+    ) -> 'Problem':
+        """
+        Factory method to load model and tables from files.
+
+        Arguments:
+            sbml_file: PEtab SBML model
+            condition_file: PEtab condition table
+            measurement_file: PEtab measurement table
+            parameter_file: PEtab parameter table
+            visualization_files: PEtab visualization tables
+            observable_files: PEtab observables tables
+            model_id: PEtab ID of the model
+            extensions_config: Information on the extensions used
+        """
+        warn("petab.Problem.from_files is deprecated and will be removed in a "
+             "future version. Use `petab.Problem.from_yaml instead.",
+             DeprecationWarning, stacklevel=2)
+
+        model = model_factory(sbml_file, MODEL_TYPE_SBML, model_id=model_id) \
+            if sbml_file else None
+
+        condition_df = core.concat_tables(
+            condition_file, conditions.get_condition_df) \
+            if condition_file else None
+
+        # If there are multiple tables, we will merge them
+        measurement_df = core.concat_tables(
+            measurement_file, measurements.get_measurement_df) \
+            if measurement_file else None
+
+        parameter_df = parameters.get_parameter_df(parameter_file) \
+            if parameter_file else None
+
+        # If there are multiple tables, we will merge them
+        visualization_df = core.concat_tables(
+            visualization_files, core.get_visualization_df) \
+            if visualization_files else None
+
+        # If there are multiple tables, we will merge them
+        observable_df = core.concat_tables(
+            observable_files, observables.get_observable_df) \
+            if observable_files else None
+
+        return Problem(
+            model=model,
+            condition_df=condition_df,
+            measurement_df=measurement_df,
+            parameter_df=parameter_df,
+            observable_df=observable_df,
+            visualization_df=visualization_df,
+            extensions_config=extensions_config,
+        )
+
+    @staticmethod
+    def from_yaml(yaml_config: Union[Dict, Path, str]) -> 'Problem':
+        """
+        Factory method to load model and tables as specified by YAML file.
+
+        Arguments:
+            yaml_config: PEtab configuration as dictionary or YAML file name
+        """
+        if isinstance(yaml_config, Path):
+            yaml_config = str(yaml_config)
+
+        get_path = lambda filename: filename  # noqa: E731
+        if isinstance(yaml_config, str):
+            yaml_path = yaml_config
+            yaml_config = yaml.load_yaml(yaml_config)
+
+            # yaml_config may be path or URL
+            path_url = urlparse(yaml_path)
+            if not path_url.scheme or \
+                    (path_url.scheme != 'file' and not path_url.netloc):
+                # a regular file path string
+                path_prefix = Path(yaml_path).parent
+                get_path = lambda filename: \
+                    path_prefix / filename  # noqa: E731
             else:
-                type_ = row[type_col]
-            # get parameters
-            pars_str = row.get(par_col, '')
-            with_default_parameters = [PARAMETER_SCALE_UNIFORM]
-            # check if parameters are empty
-            if core.is_empty(pars_str):
-                if type_ not in with_default_parameters:
-                    raise AssertionError(
-                        f"An empty {par_col} is only permitted with "
-                        f"{type_col} in {with_default_parameters}.")
-                # empty parameters fine
-                continue
-            # parse parameters
-            try:
-                pars = tuple([float(val) for val in pars_str.split(';')])
-            except ValueError:
-                raise AssertionError(
-                    f"Could not parse prior parameters '{pars_str}'.")
-            # all distributions take 2 parameters
-            if len(pars) != 2:
-                raise AssertionError(
-                    f"The prior parameters '{pars}' do not contain the "
-                    "expected number of entries (currently 'par1;par2' "
-                    "for all prior types).")
-
-
-def assert_parameter_estimate_is_boolean(parameter_df: pd.DataFrame) -> None:
-    """
-    Check if all entries in the estimate column of the parameter table are
-    0 or 1.
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-    """
-    for estimate in parameter_df[ESTIMATE]:
-        if int(estimate) not in [True, False]:
-            raise AssertionError(
-                f"Expected 0 or 1 but got {estimate} in {ESTIMATE} column.")
-
-
-def measurement_table_has_timepoint_specific_mappings(
-        measurement_df: pd.DataFrame) -> bool:
-    """
-    Are there time-point or replicate specific parameter assignments in the
-    measurement table.
-
-    Arguments:
-        measurement_df: PEtab measurement table
-
-    Returns:
-        True if there are time-point or replicate specific parameter
-        assignments in the measurement table, False otherwise.
-    """
-    # since we edit it, copy it first
-    measurement_df = copy.deepcopy(measurement_df)
-
-    if NOISE_PARAMETERS not in measurement_df:
-        measurement_df[NOISE_PARAMETERS] = np.nan
-
-    measurement_df.loc[
-        measurement_df.noiseParameters.apply(isinstance, args=(
-            numbers.Number,)), NOISE_PARAMETERS] = np.nan
-
-    grouping_cols = core.get_notnull_columns(
-        measurement_df,
-        [OBSERVABLE_ID,
-         SIMULATION_CONDITION_ID,
-         PREEQUILIBRATION_CONDITION_ID,
-         OBSERVABLE_PARAMETERS,
-         NOISE_PARAMETERS,
-         ])
-    grouped_df = measurement_df.fillna('').groupby(grouping_cols).size()\
-        .reset_index()
-
-    grouping_cols = core.get_notnull_columns(
-        grouped_df,
-        [OBSERVABLE_ID,
-         SIMULATION_CONDITION_ID,
-         PREEQUILIBRATION_CONDITION_ID])
-    grouped_df2 = grouped_df.groupby(grouping_cols).size().reset_index()
-
-    if len(grouped_df.index) != len(grouped_df2.index):
-        logger.warning("Measurement table has timepoint-specific "
-                       f"mappings:\n{grouped_df}")
-        return True
-    return False
-
-
-def measurement_table_has_observable_parameter_numeric_overrides(
-        measurement_df: pd.DataFrame) -> bool:
-    """Are there any numbers to override observable parameters?
-
-    Arguments:
-        measurement_df: PEtab measurement table
-
-    Returns:
-        True if there any numbers to override observable parameters,
-        False otherwise.
-    """
-    if OBSERVABLE_PARAMETERS not in measurement_df:
-        return False
-
-    for _, row in measurement_df.iterrows():
-        for override in measurements.split_parameter_replacement_list(
-                row.get(OBSERVABLE_PARAMETERS, None)):
-            if isinstance(override, numbers.Number):
-                return True
-
-    return False
-
-
-def assert_noise_distributions_valid(observable_df: pd.DataFrame) -> None:
-    """
-    Ensure that noise distributions and transformations for observables are
-    valid.
-
-    Arguments:
-        observable_df: PEtab observable table
-
-    Raises:
-        AssertionError: in case of problems
-    """
-    if OBSERVABLE_TRANSFORMATION in observable_df:
-        # check for valid values
-        for trafo in observable_df[OBSERVABLE_TRANSFORMATION]:
-            if trafo not in ['', *OBSERVABLE_TRANSFORMATIONS] \
-                    and not (isinstance(trafo, numbers.Number)
-                             and np.isnan(trafo)):
-                raise ValueError(
-                    f"Unrecognized observable transformation in observable "
-                    f"table: {trafo}.")
-
-    if NOISE_DISTRIBUTION in observable_df:
-        for distr in observable_df[NOISE_DISTRIBUTION]:
-            if distr not in ['', *NOISE_MODELS] \
-                    and not (isinstance(distr, numbers.Number)
-                             and np.isnan(distr)):
-                raise ValueError(
-                    f"Unrecognized noise distribution in observable "
-                    f"table: {distr}.")
-
-
-def assert_unique_observable_ids(observable_df: pd.DataFrame) -> None:
-    """
-    Check if the observableId column of the observable table is unique.
-
-    Arguments:
-        observable_df: PEtab observable DataFrame
-
-    Raises:
-        AssertionError: in case of problems
-    """
-    non_unique_ids = get_non_unique(observable_df.index)
-    if len(non_unique_ids) > 0:
-        raise AssertionError(
-            f"Non-unique values found in the {OBSERVABLE_ID} column"
-            " of the observable table: " + str(non_unique_ids))
-
-
-def get_non_unique(values):
-    counter = Counter(values)
-    return [value for (value, count) in counter.items() if count > 1]
-
-
-def lint_problem(problem: 'petab.Problem') -> bool:
-    """Run PEtab validation on problem
-
-    Arguments:
-        problem: PEtab problem to check
-
-    Returns:
-        True is errors occurred, False otherwise
-    """
-    # pylint: disable=too-many-statements
-    errors_occurred = False
-
-    # Run checks on individual files
-    if problem.sbml_model is not None:
-        logger.info("Checking SBML model...")
-        errors_occurred |= not sbml.is_sbml_consistent(
-            problem.sbml_model.getSBMLDocument())
-        sbml.log_sbml_errors(problem.sbml_model.getSBMLDocument())
-    else:
-        logger.warning("SBML model not available. Skipping.")
-
-    if problem.measurement_df is not None:
-        logger.info("Checking measurement table...")
-        try:
-            check_measurement_df(problem.measurement_df, problem.observable_df)
-
-            if problem.condition_df is not None:
-                assert_measurement_conditions_present_in_condition_table(
-                    problem.measurement_df, problem.condition_df
+                # a URL
+                # extract parent path from
+                url_path = unquote(urlparse(yaml_path).path)
+                parent_path = str(PurePosixPath(url_path).parent)
+                path_prefix = urlunparse(
+                    (path_url.scheme, path_url.netloc, parent_path,
+                     path_url.params, path_url.query, path_url.fragment)
                 )
-        except AssertionError as e:
-            logger.error(e)
-            errors_occurred = True
-    else:
-        logger.warning("Measurement table not available. Skipping.")
-
-    if problem.condition_df is not None:
-        logger.info("Checking condition table...")
-        try:
-            check_condition_df(problem.condition_df, problem.sbml_model)
-        except AssertionError as e:
-            logger.error(e)
-            errors_occurred = True
-    else:
-        logger.warning("Condition table not available. Skipping.")
-
-    if problem.observable_df is not None:
-        logger.info("Checking observable table...")
-        try:
-            check_observable_df(problem.observable_df)
-        except AssertionError as e:
-            logger.error(e)
-            errors_occurred = True
-        if problem.sbml_model is not None:
-            for obs_id in problem.observable_df.index:
-                if problem.sbml_model.getElementBySId(obs_id):
-                    logger.error(f"Observable ID {obs_id} shadows model "
-                                 "entity.")
-                    errors_occurred = True
-    else:
-        logger.warning("Observable table not available. Skipping.")
-
-    if problem.parameter_df is not None:
-        logger.info("Checking parameter table...")
-        try:
-            check_parameter_df(problem.parameter_df, problem.sbml_model,
-                               problem.observable_df,
-                               problem.measurement_df, problem.condition_df)
-        except AssertionError as e:
-            logger.error(e)
-            errors_occurred = True
-    else:
-        logger.warning("Parameter table not available. Skipping.")
-
-    if problem.sbml_model is not None and problem.condition_df is not None \
-            and problem.parameter_df is not None:
+                # need "/" on windows, not "\"
+                get_path = lambda filename: \
+                    f"{path_prefix}/{filename}"  # noqa: E731
+
+        if yaml.is_composite_problem(yaml_config):
+            raise ValueError('petab.Problem.from_yaml() can only be used for '
+                             'yaml files comprising a single model. '
+                             'Consider using '
+                             'petab.CompositeProblem.from_yaml() instead.')
+
+        if yaml_config[FORMAT_VERSION] not in {"1", 1, "1.0.0", "2.0.0"}:
+            raise ValueError("Provided PEtab files are of unsupported version "
+                             f"{yaml_config[FORMAT_VERSION]}. Expected "
+                             f"{format_version.__format_version__}.")
+        if yaml_config[FORMAT_VERSION] == "2.0.0":
+            warn("Support for PEtab2.0 is experimental!")
+
+        problem0 = yaml_config['problems'][0]
+
+        if isinstance(yaml_config[PARAMETER_FILE], list):
+            parameter_df = parameters.get_parameter_df([
+                get_path(f)
+                for f in yaml_config[PARAMETER_FILE]
+            ])
+        else:
+            parameter_df = parameters.get_parameter_df(
+                get_path(yaml_config[PARAMETER_FILE])) \
+                if yaml_config[PARAMETER_FILE] else None
+
+        if yaml_config[FORMAT_VERSION] in [1, "1", "1.0.0"]:
+            if len(problem0[SBML_FILES]) > 1:
+                # TODO https://github.com/PEtab-dev/libpetab-python/issues/6
+                raise NotImplementedError(
+                    'Support for multiple models is not yet implemented.')
+
+            model = model_factory(get_path(problem0[SBML_FILES][0]),
+                                  MODEL_TYPE_SBML, model_id=None) \
+                if problem0[SBML_FILES] else None
+        else:
+            if len(problem0[MODEL_FILES]) > 1:
+                # TODO https://github.com/PEtab-dev/libpetab-python/issues/6
+                raise NotImplementedError(
+                    'Support for multiple models is not yet implemented.')
+            if not problem0[MODEL_FILES]:
+                model = None
+            else:
+                model_id, model_info = \
+                    next(iter(problem0[MODEL_FILES].items()))
+                model = model_factory(get_path(model_info[MODEL_LOCATION]),
+                                      model_info[MODEL_LANGUAGE],
+                                      model_id=model_id)
+
+        measurement_files = [
+            get_path(f) for f in problem0.get(MEASUREMENT_FILES, [])]
+        # If there are multiple tables, we will merge them
+        measurement_df = core.concat_tables(
+            measurement_files, measurements.get_measurement_df) \
+            if measurement_files else None
+
+        condition_files = [
+            get_path(f) for f in problem0.get(CONDITION_FILES, [])]
+        # If there are multiple tables, we will merge them
+        condition_df = core.concat_tables(
+            condition_files, conditions.get_condition_df) \
+            if condition_files else None
+
+        visualization_files = [
+            get_path(f) for f in problem0.get(VISUALIZATION_FILES, [])]
+        # If there are multiple tables, we will merge them
+        visualization_df = core.concat_tables(
+            visualization_files, core.get_visualization_df) \
+            if visualization_files else None
+
+        observable_files = [
+            get_path(f) for f in problem0.get(OBSERVABLE_FILES, [])]
+        # If there are multiple tables, we will merge them
+        observable_df = core.concat_tables(
+            observable_files, observables.get_observable_df) \
+            if observable_files else None
+
+        mapping_files = [
+            get_path(f) for f in problem0.get(MAPPING_FILES, [])]
+        # If there are multiple tables, we will merge them
+        mapping_df = core.concat_tables(
+            mapping_files, mapping.get_mapping_df) \
+            if mapping_files else None
+
+        return Problem(
+            condition_df=condition_df,
+            measurement_df=measurement_df,
+            parameter_df=parameter_df,
+            observable_df=observable_df,
+            model=model,
+            visualization_df=visualization_df,
+            mapping_df=mapping_df,
+            extensions_config=yaml_config.get(EXTENSIONS, {})
+        )
+
+    @staticmethod
+    def from_combine(filename: Union[Path, str]) -> 'Problem':
+        """Read PEtab COMBINE archive (http://co.mbine.org/documents/archive).
+
+        See also :py:func:`petab.create_combine_archive`.
+
+        Arguments:
+            filename: Path to the PEtab-COMBINE archive
+
+        Returns:
+            A :py:class:`petab.Problem` instance.
+        """
+        # function-level import, because module-level import interfered with
+        # other SWIG interfaces
         try:
-            assert_model_parameters_in_condition_or_parameter_table(
-                problem.sbml_model,
-                problem.condition_df,
-                problem.parameter_df
-            )
-        except AssertionError as e:
-            logger.error(e)
-            errors_occurred = True
-
-    if errors_occurred:
-        logger.error('Not OK')
-    elif problem.measurement_df is None or problem.condition_df is None \
-            or problem.sbml_model is None or problem.parameter_df is None \
-            or problem.observable_df is None:
-        logger.warning('Not all files of the PEtab problem definition could '
-                       'be checked.')
-    else:
-        logger.info('OK')
-
-    return errors_occurred
-
-
-def assert_model_parameters_in_condition_or_parameter_table(
-        sbml_model: libsbml.Model,
-        condition_df: pd.DataFrame,
-        parameter_df: pd.DataFrame) -> None:
-    """Model parameters that are targets of AssignmentRule must not be present
-    in parameter table or in condition table columns. Other parameters must
-    only be present in either in parameter table or condition table columns.
-    Check that.
-
-    Arguments:
-        parameter_df: PEtab parameter DataFrame
-        sbml_model: PEtab SBML Model
-        condition_df: PEtab condition table
-
-    Raises:
-        AssertionError: in case of problems
-    """
-
-    for parameter in sbml_model.getListOfParameters():
-        parameter_id = parameter.getId()
-
-        if parameter_id.startswith('observableParameter'):
-            continue
-        if parameter_id.startswith('noiseParameter'):
-            continue
-
-        is_assignee = \
-            sbml_model.getAssignmentRuleByVariable(parameter_id) is not None
-        in_parameter_df = parameter_id in parameter_df.index
-        in_condition_df = parameter_id in condition_df.columns
-
-        if is_assignee and (in_parameter_df or in_condition_df):
-            raise AssertionError(f"Model parameter '{parameter_id}' is target "
-                                 "of AssignmentRule, and thus, must not be "
-                                 "present in condition table or in parameter "
-                                 "table.")
-
-        if in_parameter_df and in_condition_df:
-            raise AssertionError(f"Model parameter '{parameter_id}' present "
-                                 "in both condition table and parameter "
-                                 "table.")
-
-
-def assert_measurement_conditions_present_in_condition_table(
-        measurement_df: pd.DataFrame, condition_df: pd.DataFrame) -> None:
-    """Ensure that all entries from measurement_df.simulationConditionId and
-    measurement_df.preequilibrationConditionId are present in
-    condition_df.index.
+            import libcombine
+        except ImportError as e:
+            raise ImportError(
+                "To use PEtab's COMBINE functionality, libcombine "
+                "(python-libcombine) must be installed.") from e
+
+        archive = libcombine.CombineArchive()
+        if archive.initializeFromArchive(str(filename)) is None:
+            print(f"Invalid Combine Archive: {filename}")
+            return None
+
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            archive.extractTo(tmpdirname)
+            problem = Problem.from_yaml(
+                os.path.join(tmpdirname,
+                             archive.getMasterFile().getLocation()))
+        archive.cleanUp()
+
+        return problem
+
+    def to_files_generic(
+        self,
+        prefix_path: Union[str, Path],
+    ) -> str:
+        """Save a PEtab problem to generic file names.
+
+        The PEtab problem YAML file is always created. PEtab data files are
+        only created if the PEtab problem contains corresponding data (e.g. a
+        PEtab visualization TSV file is only created if the PEtab problem has
+        one).
+
+        Arguments:
+            prefix_path:
+                Specify a prefix to all paths, to avoid specifying the
+                prefix for all paths individually. NB: the prefix is added to
+                paths before ``relative_paths`` is handled downstream in
+                :func:`petab.yaml.create_problem_yaml`.
+
+        Returns:
+            The path to the PEtab problem YAML file.
+        """
+        prefix_path = Path(prefix_path)
+
+        # Generate generic filenames for data tables in the PEtab problem that
+        # contain data.
+        filenames = {}
+        for table_name in [
+            'condition',
+            'measurement',
+            'parameter',
+            'observable',
+            'visualization',
+            'mapping',
+        ]:
+            if getattr(self, f'{table_name}_df') is not None:
+                filenames[f'{table_name}_file'] = f'{table_name}s.tsv'
+
+        if self.model:
+            if not isinstance(self.model, SbmlModel):
+                raise NotImplementedError("Saving non-SBML models is "
+                                          "currently not supported.")
+            filenames['sbml_file'] = 'model.xml'
+
+        filenames['yaml_file'] = 'problem.yaml'
+
+        self.to_files(**filenames, prefix_path=prefix_path)
+
+        if prefix_path is None:
+            return filenames['yaml_file']
+        return str(prefix_path / filenames['yaml_file'])
+
+    def to_files(
+            self,
+            sbml_file: Union[None, str, Path] = None,
+            condition_file: Union[None, str, Path] = None,
+            measurement_file: Union[None, str, Path] = None,
+            parameter_file: Union[None, str, Path] = None,
+            visualization_file: Union[None, str, Path] = None,
+            observable_file: Union[None, str, Path] = None,
+            yaml_file: Union[None, str, Path] = None,
+            prefix_path: Union[None, str, Path] = None,
+            relative_paths: bool = True,
+            model_file: Union[None, str, Path] = None,
+            mapping_file: Union[None, str, Path] = None,
+    ) -> None:
+        """
+        Write PEtab tables to files for this problem
+
+        Writes PEtab files for those entities for which a destination was
+        passed.
+
+        NOTE: If this instance was created from multiple measurement or
+        visualization tables, they will be merged and written to a single file.
+
+        Arguments:
+            sbml_file: SBML model destination (deprecated)
+            model_file: Model destination
+            condition_file: Condition table destination
+            measurement_file: Measurement table destination
+            parameter_file: Parameter table destination
+            visualization_file: Visualization table destination
+            observable_file: Observables table destination
+            mapping_file: Mapping table destination
+            yaml_file: YAML file destination
+            prefix_path:
+                Specify a prefix to all paths, to avoid specifying the
+                prefix for all paths individually. NB: the prefix is added to
+                paths before ``relative_paths`` is handled.
+            relative_paths:
+                whether all paths in the YAML file should be
+                relative to the location of the YAML file. If ``False``, then
+                paths are left unchanged.
+
+        Raises:
+            ValueError:
+                If a destination was provided for a non-existing entity.
+        """
+        if sbml_file:
+            warn("The `sbml_file` argument is deprecated and will be "
+                 "removed in a future version. Use `model_file` instead.",
+                 DeprecationWarning, stacklevel=2)
+
+            if model_file:
+                raise ValueError("Must provide either `sbml_file` or "
+                                 "`model_file` argument, but not both.")
+
+            model_file = sbml_file
+
+        if prefix_path is not None:
+            prefix_path = Path(prefix_path)
+
+            def add_prefix(path0: Union[None, str, Path]) -> str:
+                return path0 if path0 is None else str(prefix_path / path0)
+
+            model_file = add_prefix(model_file)
+            condition_file = add_prefix(condition_file)
+            measurement_file = add_prefix(measurement_file)
+            parameter_file = add_prefix(parameter_file)
+            observable_file = add_prefix(observable_file)
+            visualization_file = add_prefix(visualization_file)
+            mapping_file = add_prefix(mapping_file)
+            yaml_file = add_prefix(yaml_file)
+
+        if model_file:
+            self.model.to_file(model_file)
+
+        def error(name: str) -> ValueError:
+            return ValueError(f"Unable to save non-existent {name} table")
+
+        if condition_file:
+            if self.condition_df is not None:
+                conditions.write_condition_df(self.condition_df,
+                                              condition_file)
+            else:
+                raise error("condition")
 
-    Arguments:
-        measurement_df: PEtab measurement table
-        condition_df: PEtab condition table
+        if measurement_file:
+            if self.measurement_df is not None:
+                measurements.write_measurement_df(self.measurement_df,
+                                                  measurement_file)
+            else:
+                raise error("measurement")
 
-    Raises:
-        AssertionError: in case of problems
-    """
+        if parameter_file:
+            if self.parameter_df is not None:
+                parameters.write_parameter_df(self.parameter_df,
+                                              parameter_file)
+            else:
+                raise error("parameter")
 
-    used_conditions = set(measurement_df[SIMULATION_CONDITION_ID].values)
-    if PREEQUILIBRATION_CONDITION_ID in measurement_df:
-        used_conditions |= \
-            set(measurement_df[PREEQUILIBRATION_CONDITION_ID].dropna().values)
-    available_conditions = set(condition_df.index.values)
-    missing_conditions = used_conditions - available_conditions
-
-    if missing_conditions:
-        raise AssertionError("Measurement table references conditions that "
-                             "are not specified in the condition table: "
-                             + str(missing_conditions))
-
-
-def is_valid_identifier(x: str) -> bool:
-    """Check whether `x` is a valid identifier
-
-    Check whether `x` is a valid identifier for conditions, parameters,
-    observables... . Identifiers may contain upper and lower case letters,
-    digits and underscores, but must not start with a digit.
+        if observable_file:
+            if self.observable_df is not None:
+                observables.write_observable_df(self.observable_df,
+                                                observable_file)
+            else:
+                raise error("observable")
 
-    Arguments:
-        x: string to check
+        if visualization_file:
+            if self.visualization_df is not None:
+                core.write_visualization_df(self.visualization_df,
+                                            visualization_file)
+            else:
+                raise error("visualization")
 
-    Returns:
-        ``True`` if valid, ``False`` otherwise
-    """
+        if mapping_file:
+            if self.mapping_df is not None:
+                mapping.write_mapping_df(self.mapping_df, mapping_file)
+            else:
+                raise error("mapping")
 
-    return re.match(r'^[a-zA-Z_]\w*$', x) is not None
+        if yaml_file:
+            yaml.create_problem_yaml(
+                sbml_files=sbml_file,
+                condition_files=condition_file,
+                measurement_files=measurement_file,
+                parameter_file=parameter_file,
+                observable_files=observable_file,
+                yaml_file=yaml_file,
+                visualization_files=visualization_file,
+                relative_paths=relative_paths,
+                mapping_files=mapping_file,
+            )
 
+    def get_optimization_parameters(self):
+        """
+        Return list of optimization parameter IDs.
+
+        See :py:func:`petab.parameters.get_optimization_parameters`.
+        """
+        return parameters.get_optimization_parameters(self.parameter_df)
+
+    def get_optimization_parameter_scales(self):
+        """
+        Return list of optimization parameter scaling strings.
+
+        See :py:func:`petab.parameters.get_optimization_parameters`.
+        """
+        return parameters.get_optimization_parameter_scaling(self.parameter_df)
+
+    def get_model_parameters(self):
+        """See :py:func:`petab.sbml.get_model_parameters`"""
+        warn("petab.Problem.get_model_parameters is deprecated and will be "
+             "removed in a future version.",
+             DeprecationWarning, stacklevel=2)
+
+        return sbml.get_model_parameters(self.sbml_model)
+
+    def get_observable_ids(self):
+        """
+        Returns dictionary of observable ids.
+        """
+        return list(self.observable_df.index)
+
+    def _apply_mask(self, v: List, free: bool = True, fixed: bool = True):
+        """Apply mask of only free or only fixed values.
+
+        Parameters
+        ----------
+        v:
+            The full vector the mask is to be applied to.
+        free:
+            Whether to return free parameters, i.e. parameters to estimate.
+        fixed:
+            Whether to return fixed parameters, i.e. parameters not to
+            estimate.
+
+        Returns
+        -------
+        The reduced vector with applied mask.
+        """
+        if not free and not fixed:
+            return []
+        if not free:
+            return [v[ix] for ix in self.x_fixed_indices]
+        if not fixed:
+            return [v[ix] for ix in self.x_free_indices]
+        return v
+
+    def get_x_ids(self, free: bool = True, fixed: bool = True):
+        """Generic function to get parameter ids.
+
+        Parameters
+        ----------
+        free:
+            Whether to return free parameters, i.e. parameters to estimate.
+        fixed:
+            Whether to return fixed parameters, i.e. parameters not to
+            estimate.
+
+        Returns
+        -------
+        The parameter IDs.
+        """
+        v = list(self.parameter_df.index.values)
+        return self._apply_mask(v, free=free, fixed=fixed)
+
+    @property
+    def x_ids(self) -> List[str]:
+        """Parameter table parameter IDs"""
+        return self.get_x_ids()
+
+    @property
+    def x_free_ids(self) -> List[str]:
+        """Parameter table parameter IDs, for free parameters."""
+        return self.get_x_ids(fixed=False)
+
+    @property
+    def x_fixed_ids(self) -> List[str]:
+        """Parameter table parameter IDs, for fixed parameters."""
+        return self.get_x_ids(free=False)
+
+    def get_x_nominal(self, free: bool = True, fixed: bool = True,
+                      scaled: bool = False):
+        """Generic function to get parameter nominal values.
+
+        Parameters
+        ----------
+        free:
+            Whether to return free parameters, i.e. parameters to estimate.
+        fixed:
+            Whether to return fixed parameters, i.e. parameters not to
+            estimate.
+        scaled:
+            Whether to scale the values according to the parameter scale,
+            or return them on linear scale.
+
+        Returns
+        -------
+        The parameter nominal values.
+        """
+        v = list(self.parameter_df[NOMINAL_VALUE])
+        if scaled:
+            v = list(parameters.map_scale(
+                v, self.parameter_df[PARAMETER_SCALE]))
+        return self._apply_mask(v, free=free, fixed=fixed)
+
+    @property
+    def x_nominal(self) -> List:
+        """Parameter table nominal values"""
+        return self.get_x_nominal()
+
+    @property
+    def x_nominal_free(self) -> List:
+        """Parameter table nominal values, for free parameters."""
+        return self.get_x_nominal(fixed=False)
+
+    @property
+    def x_nominal_fixed(self) -> List:
+        """Parameter table nominal values, for fixed parameters."""
+        return self.get_x_nominal(free=False)
+
+    @property
+    def x_nominal_scaled(self) -> List:
+        """Parameter table nominal values with applied parameter scaling"""
+        return self.get_x_nominal(scaled=True)
+
+    @property
+    def x_nominal_free_scaled(self) -> List:
+        """Parameter table nominal values with applied parameter scaling,
+        for free parameters."""
+        return self.get_x_nominal(fixed=False, scaled=True)
+
+    @property
+    def x_nominal_fixed_scaled(self) -> List:
+        """Parameter table nominal values with applied parameter scaling,
+        for fixed parameters."""
+        return self.get_x_nominal(free=False, scaled=True)
+
+    def get_lb(self, free: bool = True, fixed: bool = True,
+               scaled: bool = False):
+        """Generic function to get lower parameter bounds.
+
+        Parameters
+        ----------
+        free:
+            Whether to return free parameters, i.e. parameters to estimate.
+        fixed:
+            Whether to return fixed parameters, i.e. parameters not to
+            estimate.
+        scaled:
+            Whether to scale the values according to the parameter scale,
+            or return them on linear scale.
+
+        Returns
+        -------
+        The lower parameter bounds.
+        """
+        v = list(self.parameter_df[LOWER_BOUND])
+        if scaled:
+            v = list(parameters.map_scale(
+                v, self.parameter_df[PARAMETER_SCALE]))
+        return self._apply_mask(v, free=free, fixed=fixed)
+
+    @property
+    def lb(self) -> List:
+        """Parameter table lower bounds."""
+        return self.get_lb()
+
+    @property
+    def lb_scaled(self) -> List:
+        """Parameter table lower bounds with applied parameter scaling"""
+        return self.get_lb(scaled=True)
+
+    def get_ub(self, free: bool = True, fixed: bool = True,
+               scaled: bool = False):
+        """Generic function to get upper parameter bounds.
+
+        Parameters
+        ----------
+        free:
+            Whether to return free parameters, i.e. parameters to estimate.
+        fixed:
+            Whether to return fixed parameters, i.e. parameters not to
+            estimate.
+        scaled:
+            Whether to scale the values according to the parameter scale,
+            or return them on linear scale.
+
+        Returns
+        -------
+        The upper parameter bounds.
+        """
+        v = list(self.parameter_df[UPPER_BOUND])
+        if scaled:
+            v = list(parameters.map_scale(
+                v, self.parameter_df[PARAMETER_SCALE]))
+        return self._apply_mask(v, free=free, fixed=fixed)
+
+    @property
+    def ub(self) -> List:
+        """Parameter table upper bounds"""
+        return self.get_ub()
+
+    @property
+    def ub_scaled(self) -> List:
+        """Parameter table upper bounds with applied parameter scaling"""
+        return self.get_ub(scaled=True)
+
+    @property
+    def x_free_indices(self) -> List[int]:
+        """Parameter table estimated parameter indices."""
+        estimated = list(self.parameter_df[ESTIMATE])
+        return [j for j, val in enumerate(estimated) if val != 0]
+
+    @property
+    def x_fixed_indices(self) -> List[int]:
+        """Parameter table non-estimated parameter indices."""
+        estimated = list(self.parameter_df[ESTIMATE])
+        return [j for j, val in enumerate(estimated) if val == 0]
+
+    def get_simulation_conditions_from_measurement_df(self):
+        """See petab.get_simulation_conditions"""
+        return measurements.get_simulation_conditions(self.measurement_df)
+
+    def get_optimization_to_simulation_parameter_mapping(
+            self, **kwargs
+    ):
+        """
+        See
+        :py:func:`petab.parameter_mapping.get_optimization_to_simulation_parameter_mapping`,
+        to which all keyword arguments are forwarded.
+        """
+        return parameter_mapping \
+            .get_optimization_to_simulation_parameter_mapping(
+                condition_df=self.condition_df,
+                measurement_df=self.measurement_df,
+                parameter_df=self.parameter_df,
+                observable_df=self.observable_df,
+                model=self.model,
+                **kwargs
+            )
 
-def check_ids(ids: Iterable[str], kind: str = '') -> None:
-    """Check IDs are valid
+    def create_parameter_df(self, *args, **kwargs):
+        """Create a new PEtab parameter table
 
-    Arguments:
-        ids: Iterable of IDs to check
-        kind: Kind of IDs, for more informative error message
+        See :py:func:`create_parameter_df`.
+        """
+        return parameters.create_parameter_df(
+            model=self.model,
+            condition_df=self.condition_df,
+            observable_df=self.observable_df,
+            measurement_df=self.measurement_df,
+            mapping_df=self.mapping_df,
+            *args, **kwargs)
+
+    def sample_parameter_startpoints(self, n_starts: int = 100):
+        """Create 2D array with starting points for optimization
+
+        See :py:func:`petab.sample_parameter_startpoints`.
+        """
+        return sampling.sample_parameter_startpoints(
+            self.parameter_df, n_starts=n_starts)
+
+    def sample_parameter_startpoints_dict(
+            self,
+            n_starts: int = 100
+    ) -> List[Dict[str, float]]:
+        """Create dictionaries with starting points for optimization
+
+        See also :py:func:`petab.sample_parameter_startpoints`.
+
+        Returns:
+            A list of dictionaries with parameter IDs mapping to samples
+            parameter values.
+        """
+        return [
+            dict(zip(self.x_free_ids, parameter_values))
+            for parameter_values in self.sample_parameter_startpoints(
+                n_starts=n_starts
+            )
+        ]
 
-    Raises:
-        ValueError - in case of invalid IDs
-    """
-    invalids = []
-    for _id in ids:
-        if not is_valid_identifier(_id):
-            invalids.append(_id)
+    def unscale_parameters(
+        self,
+        x_dict: Dict[str, float],
+    ) -> Dict[str, float]:
+        """Unscale parameter values.
+
+        Parameters
+        ----------
+        x_dict:
+            Keys are parameter IDs in the PEtab problem, values are scaled
+            parameter values.
+
+        Returns
+        -------
+        The unscaled parameter values.
+        """
+        return {
+            parameter_id: parameters.unscale(
+                parameter_value,
+                self.parameter_df[PARAMETER_SCALE][parameter_id],
+            )
+            for parameter_id, parameter_value in x_dict.items()
+        }
 
-    if invalids:
-        raise ValueError(f"Invalid {kind} ID(s): {invalids}")
+    def scale_parameters(
+        self,
+        x_dict: Dict[str, float],
+    ) -> Dict[str, float]:
+        """Scale parameter values.
+
+        Parameters
+        ----------
+        x_dict:
+            Keys are parameter IDs in the PEtab problem, values are unscaled
+            parameter values.
+
+        Returns
+        -------
+        The scaled parameter values.
+        """
+        return {
+            parameter_id: parameters.scale(
+                parameter_value,
+                self.parameter_df[PARAMETER_SCALE][parameter_id],
+            )
+            for parameter_id, parameter_value in x_dict.items()
+        }
```

### Comparing `petab-0.1.8/petab/core.py` & `petab-0.2.0/petab/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,94 @@
 """PEtab core functions (or functions that don't fit anywhere else)"""
-
+from pathlib import Path
 import logging
 import os
-from typing import Iterable, Optional, Callable, Union, Any, Sequence, List
+import re
+from typing import (
+    Iterable, Optional, Callable, Union, Any, Sequence, List, Dict,
+)
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 
 from . import yaml
 from .C import *  # noqa: F403
 
 logger = logging.getLogger(__name__)
+__all__ = ['get_simulation_df', 'write_simulation_df', 'get_visualization_df',
+           'write_visualization_df', 'get_notnull_columns',
+           'flatten_timepoint_specific_output_overrides',
+           'concat_tables', 'to_float_if_float', 'is_empty',
+           'create_combine_archive', 'unique_preserve_order',
+           'unflatten_simulation_df']
+
+POSSIBLE_GROUPVARS_FLATTENED_PROBLEM = [
+    OBSERVABLE_ID,
+    OBSERVABLE_PARAMETERS,
+    NOISE_PARAMETERS,
+    SIMULATION_CONDITION_ID,
+    PREEQUILIBRATION_CONDITION_ID,
+]
 
 
-def get_simulation_df(simulation_file: str) -> pd.DataFrame:
+def get_simulation_df(simulation_file: Union[str, Path]) -> pd.DataFrame:
     """Read PEtab simulation table
 
     Arguments:
         simulation_file: URL or filename of PEtab simulation table
 
     Returns:
         Simulation DataFrame
     """
     return pd.read_csv(simulation_file, sep="\t", index_col=None,
                        float_precision='round_trip')
 
 
-def write_simulation_df(df: pd.DataFrame, filename: str) -> None:
+def write_simulation_df(df: pd.DataFrame, filename: Union[str, Path]) -> None:
     """Write PEtab simulation table
 
     Arguments:
         df: PEtab simulation table
         filename: Destination file name
     """
-    with open(filename, 'w') as fh:
-        df.to_csv(fh, sep='\t', index=False)
+    df.to_csv(filename, sep='\t', index=False)
 
 
-def get_visualization_df(visualization_file: str) -> pd.DataFrame:
+def get_visualization_df(visualization_file: Union[str, Path]) -> pd.DataFrame:
     """Read PEtab visualization table
 
     Arguments:
         visualization_file: URL or filename of PEtab visualization table
 
     Returns:
         Visualization DataFrame
     """
     try:
+        types = {PLOT_NAME: str}
         vis_spec = pd.read_csv(visualization_file, sep="\t", index_col=None,
+                               converters=types,
                                float_precision='round_trip')
     except pd.errors.EmptyDataError:
         warn("Visualization table is empty. Defaults will be used. "
              "Refer to the documentation for details.")
         vis_spec = pd.DataFrame()
     return vis_spec
 
 
-def write_visualization_df(df: pd.DataFrame, filename: str) -> None:
+def write_visualization_df(
+        df: pd.DataFrame, filename: Union[str, Path]
+) -> None:
     """Write PEtab visualization table
 
     Arguments:
         df: PEtab visualization table
         filename: Destination file name
     """
-    with open(filename, 'w') as fh:
-        df.to_csv(fh, sep='\t', index=False)
+    df.to_csv(filename, sep='\t', index=False)
 
 
 def get_notnull_columns(df: pd.DataFrame, candidates: Iterable):
     """
     Return list of ``df``-columns in ``candidates`` which are not all null/nan.
 
     The output can e.g. be used as input for ``pandas.DataFrame.groupby``.
@@ -80,177 +99,200 @@
         candidates:
             Columns of ``df`` to consider
     """
     return [col for col in candidates
             if col in df and not np.all(df[col].isnull())]
 
 
-def get_observable_id(parameter_id: str) -> str:
-    """Get PEtab observable ID from PEtab-style sigma or observable
-    `AssignmentRule`-target ``parameter_id``.
-
-    e.g. for 'observable_obs1' -> 'obs1', for 'sigma_obs1' -> 'obs1'
+def get_observable_replacement_id(groupvars, groupvar) -> str:
+    """Get the replacement ID for an observable.
 
     Arguments:
-        parameter_id: Some parameter ID
+        groupvars:
+            The columns of a PEtab measurement table that should be unique
+            between observables in a flattened PEtab problem.
+        groupvar:
+            A specific grouping of `groupvars`.
 
     Returns:
-        Observable ID
+        The observable replacement ID.
     """
-    warn("This function will be removed in future releases.",
-         DeprecationWarning)
+    replacement_id = ''
+    for field in POSSIBLE_GROUPVARS_FLATTENED_PROBLEM:
+        if field in groupvars:
+            val = str(groupvar[groupvars.index(field)])\
+                .replace(PARAMETER_SEPARATOR, '_').replace('.', '_')
+            if replacement_id == '':
+                replacement_id = val
+            elif val != '':
+                replacement_id += f'__{val}'
+    return replacement_id
+
+
+def get_hyperparameter_replacement_id(
+        hyperparameter_type,
+        observable_replacement_id,
+):
+    """Get the full ID for a replaced hyperparameter.
+
+    Arguments:
+        hyperparameter_type:
+            The type of hyperparameter, e.g. `noiseParameter`.
+        observable_replacement_id:
+            The observable replacement ID, e.g. the output of
+            `get_observable_replacement_id`.
 
-    if parameter_id.startswith(r'observable_'):
-        return parameter_id[len('observable_'):]
+    Returns:
+        The hyperparameter replacement ID, with a field that will be replaced
+        by the first matched substring in a regex substitution.
+    """
+    return f'{hyperparameter_type}\\1_{observable_replacement_id}'
 
-    if parameter_id.startswith(r'sigma_'):
-        return parameter_id[len('sigma_'):]
 
-    raise ValueError('Cannot extract observable id from: ' + parameter_id)
+def get_flattened_id_mappings(
+    petab_problem: 'petab.problem.Problem',
+) -> Dict[str, Dict[str, str]]:
+    """Get mapping from unflattened to flattened observable IDs.
+
+    Arguments:
+        petab_problem:
+            The unflattened PEtab problem.
+
+    Returns:
+        A dictionary of dictionaries. Each inner dictionary is a mapping
+        from original ID to flattened ID. Each outer dictionary is the mapping
+        for either: observable IDs; noise parameter IDs; or, observable
+        parameter IDs.
+    """
+    groupvars = get_notnull_columns(petab_problem.measurement_df,
+                                    POSSIBLE_GROUPVARS_FLATTENED_PROBLEM)
+    mappings = {
+        OBSERVABLE_ID: {},
+        NOISE_PARAMETERS: {},
+        OBSERVABLE_PARAMETERS: {},
+    }
+    for groupvar, measurements in \
+            petab_problem.measurement_df.groupby(groupvars, dropna=False):
+        observable_id = groupvar[groupvars.index(OBSERVABLE_ID)]
+        observable_replacement_id = \
+            get_observable_replacement_id(groupvars, groupvar)
+
+        logger.debug(f'Creating synthetic observable {observable_id}')
+        if observable_replacement_id in petab_problem.observable_df.index:
+            raise RuntimeError('could not create synthetic observables '
+                               f'since {observable_replacement_id} was '
+                               'already present in observable table')
+
+        mappings[OBSERVABLE_ID][observable_replacement_id] = observable_id
+
+        for field, hyperparameter_type, target in [
+            (NOISE_PARAMETERS, 'noiseParameter', NOISE_FORMULA),
+            (OBSERVABLE_PARAMETERS, 'observableParameter', OBSERVABLE_FORMULA)
+        ]:
+            if field in measurements:
+                mappings[field][get_hyperparameter_replacement_id(
+                    hyperparameter_type=hyperparameter_type,
+                    observable_replacement_id=observable_replacement_id,
+                )] = fr'{hyperparameter_type}([0-9]+)_{observable_id}'
+    return mappings
 
 
 def flatten_timepoint_specific_output_overrides(
-        petab_problem: 'petab.problem.Problem') -> None:
+        petab_problem: 'petab.problem.Problem',
+) -> None:
     """Flatten timepoint-specific output parameter overrides.
 
     If the PEtab problem definition has timepoint-specific
     `observableParameters` or `noiseParameters` for the same observable,
     replace those by replicating the respective observable.
 
     This is a helper function for some tools which may not support such
     timepoint-specific mappings. The observable table and measurement table
     are modified in place.
 
     Arguments:
         petab_problem:
             PEtab problem to work on
     """
-    measurement_df = petab_problem.measurement_df
+    new_measurement_dfs = []
+    new_observable_dfs = []
+    groupvars = get_notnull_columns(petab_problem.measurement_df,
+                                    POSSIBLE_GROUPVARS_FLATTENED_PROBLEM)
+
+    mappings = get_flattened_id_mappings(petab_problem)
+
+    for groupvar, measurements in \
+            petab_problem.measurement_df.groupby(groupvars, dropna=False):
+        obs_id = groupvar[groupvars.index(OBSERVABLE_ID)]
+        observable_replacement_id = \
+            get_observable_replacement_id(groupvars, groupvar)
+
+        observable = petab_problem.observable_df.loc[obs_id].copy()
+        observable.name = observable_replacement_id
+        for field, hyperparameter_type, target in [
+            (NOISE_PARAMETERS, 'noiseParameter', NOISE_FORMULA),
+            (OBSERVABLE_PARAMETERS, 'observableParameter', OBSERVABLE_FORMULA)
+        ]:
+            if field in measurements:
+                hyperparameter_replacement_id = \
+                    get_hyperparameter_replacement_id(
+                        hyperparameter_type=hyperparameter_type,
+                        observable_replacement_id=observable_replacement_id,
+                    )
+                hyperparameter_id = \
+                    mappings[field][hyperparameter_replacement_id]
+                observable[target] = re.sub(
+                    hyperparameter_id,
+                    hyperparameter_replacement_id,
+                    observable[target],
+                )
 
-    # remember if columns exist
-    has_obs_par = OBSERVABLE_PARAMETERS in measurement_df
-    has_noise_par = NOISE_PARAMETERS in measurement_df
-    has_preeq = PREEQUILIBRATION_CONDITION_ID in measurement_df
-
-    # fill in optional columns to avoid special cases later
-    if not has_obs_par \
-            or np.all(measurement_df[OBSERVABLE_PARAMETERS].isnull()):
-        measurement_df[OBSERVABLE_PARAMETERS] = ''
-    if not has_noise_par \
-            or np.all(measurement_df[NOISE_PARAMETERS].isnull()):
-        measurement_df[NOISE_PARAMETERS] = ''
-    if not has_preeq \
-            or np.all(measurement_df[PREEQUILIBRATION_CONDITION_ID].isnull()):
-        measurement_df[PREEQUILIBRATION_CONDITION_ID] = ''
-    # convert to str row by row
-    for irow, row in measurement_df.iterrows():
-        if is_empty(row[OBSERVABLE_PARAMETERS]):
-            measurement_df.at[irow, OBSERVABLE_PARAMETERS] = ''
-        if is_empty(row[NOISE_PARAMETERS]):
-            measurement_df.at[irow, NOISE_PARAMETERS] = ''
-        if is_empty(row[PREEQUILIBRATION_CONDITION_ID]):
-            measurement_df.at[irow, PREEQUILIBRATION_CONDITION_ID] = ''
-
-    # Create empty df -> to be filled with replicate-specific observables
-    df_new = pd.DataFrame()
-
-    # Get observableId, preequilibrationConditionId
-    # and simulationConditionId columns in measurement df
-    cols = get_notnull_columns(
-        measurement_df,
-        [OBSERVABLE_ID, PREEQUILIBRATION_CONDITION_ID,
-         SIMULATION_CONDITION_ID]
-    )
-    df = measurement_df[cols]
+        measurements[OBSERVABLE_ID] = observable_replacement_id
+        new_measurement_dfs.append(measurements)
+        new_observable_dfs.append(observable)
+
+    petab_problem.observable_df = pd.concat(new_observable_dfs, axis=1).T
+    petab_problem.observable_df.index.name = OBSERVABLE_ID
+    petab_problem.measurement_df = pd.concat(new_measurement_dfs)
 
-    # Get unique combinations of observableId, preequilibrationConditionId
-    # and simulationConditionId
-    df_unique_values = df.drop_duplicates()
-
-    # replaced observables: new ID => old ID
-    replacements = dict()
-
-    # Loop over each unique combination
-    for irow in df_unique_values.index:
-        df = measurement_df.loc[
-            (measurement_df[OBSERVABLE_ID] ==
-             df_unique_values.loc[irow, OBSERVABLE_ID])
-            & (measurement_df[PREEQUILIBRATION_CONDITION_ID] ==
-               df_unique_values.loc[irow, PREEQUILIBRATION_CONDITION_ID])
-            & (measurement_df[SIMULATION_CONDITION_ID] ==
-               df_unique_values.loc[irow, SIMULATION_CONDITION_ID])
-            ]
-
-        # Get list of unique observable parameters
-        unique_sc = df[OBSERVABLE_PARAMETERS].unique()
-        # Get list of unique noise parameters
-        unique_noise = df[NOISE_PARAMETERS].unique()
-
-        # Loop
-        for i_noise, cur_noise in enumerate(unique_noise):
-            for i_sc, cur_sc in enumerate(unique_sc):
-                # Find the position of all instances of cur_noise
-                # and unique_sc[j] in their corresponding column
-                # (full-string matches are denoted by zero)
-                idxs = (
-                    df[NOISE_PARAMETERS].astype(str).str.find(cur_noise) +
-                    df[OBSERVABLE_PARAMETERS].astype(str).str.find(cur_sc)
-                )
-                tmp_ = df.loc[idxs == 0, OBSERVABLE_ID]
-                # Create replicate-specific observable name
-                tmp = tmp_ + "_" + str(i_noise + i_sc + 1)
-                # Check if replicate-specific observable name already exists
-                # in df. If true, rename replicate-specific observable
-                counter = 2
-                while (df[OBSERVABLE_ID].str.find(
-                        tmp.to_string()
-                ) == 0).any():
-                    tmp = tmp_ + counter * "_" + str(i_noise + i_sc + 1)
-                    counter += 1
-                if not tmp_.empty and not tmp_.empty:
-                    replacements[tmp.values[0]] = tmp_.values[0]
-                df.loc[idxs == 0, OBSERVABLE_ID] = tmp
-                # Append the result in a new df
-                df_new = df_new.append(df.loc[idxs == 0])
-                # Restore the observable name in the original df
-                # (for continuation of the loop)
-                df.loc[idxs == 0, OBSERVABLE_ID] = tmp
-
-    # remove previously non-existent columns again
-    if not has_obs_par:
-        df_new.drop(columns=OBSERVABLE_PARAMETERS, inplace=True)
-    if not has_noise_par:
-        df_new.drop(columns=NOISE_PARAMETERS, inplace=True)
-    if not has_preeq:
-        df_new.drop(columns=PREEQUILIBRATION_CONDITION_ID, inplace=True)
-
-    # Update/Redefine measurement df with replicate-specific observables
-    petab_problem.measurement_df = df_new
-
-    observable_df = petab_problem.observable_df
-
-    # Update observables table
-    for replacement, replacee in replacements.items():
-        new_obs = observable_df.loc[replacee].copy()
-        new_obs.name = replacement
-        new_obs[OBSERVABLE_FORMULA] = new_obs[OBSERVABLE_FORMULA].replace(
-            replacee, replacement)
-        new_obs[NOISE_FORMULA] = new_obs[NOISE_FORMULA].replace(
-            replacee, replacement)
-        observable_df = observable_df.append(
-            new_obs
-        )
 
-    petab_problem.observable_df = observable_df
-    petab_problem.observable_df.drop(index=set(replacements.values()),
-                                     inplace=True)
+def unflatten_simulation_df(
+    simulation_df: pd.DataFrame,
+    petab_problem: 'petab.problem.Problem',
+) -> None:
+    """Unflatten simulations from a flattened PEtab problem.
+
+    A flattened PEtab problem is the output of applying
+    :func:`flatten_timepoint_specific_output_overrides` to a PEtab problem.
+
+    Arguments:
+        simulation_df:
+            The simulation dataframe. A dataframe in the same format as a PEtab
+            measurements table, but with the ``measurement`` column switched
+            with a ``simulation`` column.
+        petab_problem:
+            The unflattened PEtab problem.
+
+    Returns:
+        The simulation dataframe for the unflattened PEtab problem.
+    """
+    mappings = get_flattened_id_mappings(petab_problem)
+    original_observable_ids = (
+        simulation_df[OBSERVABLE_ID]
+        .replace(mappings[OBSERVABLE_ID])
+    )
+    unflattened_simulation_df = simulation_df.assign(**{
+        OBSERVABLE_ID: original_observable_ids,
+    })
+    return unflattened_simulation_df
 
 
 def concat_tables(
-        tables: Union[str, pd.DataFrame, Iterable[Union[pd.DataFrame, str]]],
+        tables: Union[str, Path, pd.DataFrame,
+                      Iterable[Union[pd.DataFrame, str, Path]]],
         file_parser: Optional[Callable] = None
 ) -> pd.DataFrame:
     """Concatenate DataFrames provided as DataFrames or filenames, and a parser
 
     Arguments:
         tables:
             Iterable of tables to join, as DataFrame or filename.
@@ -261,25 +303,25 @@
     Returns:
         The concatenated DataFrames
     """
 
     if isinstance(tables, pd.DataFrame):
         return tables
 
-    if isinstance(tables, str):
+    if isinstance(tables, (str, Path)):
         return file_parser(tables)
 
     df = pd.DataFrame()
 
     for tmp_df in tables:
         # load from file, if necessary
-        if isinstance(tmp_df, str):
+        if isinstance(tmp_df, (str, Path)):
             tmp_df = file_parser(tmp_df)
 
-        df = df.append(tmp_df, sort=False,
+        df = pd.concat([df, tmp_df], sort=False,
                        ignore_index=isinstance(tmp_df.index, pd.RangeIndex))
 
     return df
 
 
 def to_float_if_float(x: Any) -> Any:
     """Return input as float if possible, otherwise return as is
@@ -300,38 +342,40 @@
 def is_empty(val) -> bool:
     """Check if the value `val`, e.g. a table entry, is empty.
 
     Arguments:
         val: The value to check.
 
     Returns:
-        empty: Whether the field is to be considered empty.
+        Whether the field is to be considered empty.
     """
     return val == '' or pd.isnull(val)
 
 
 def create_combine_archive(
-        yaml_file: str, filename: str,
+        yaml_file: Union[str, Path],
+        filename: Union[str, Path],
         family_name: Optional[str] = None,
         given_name: Optional[str] = None,
         email: Optional[str] = None,
         organization: Optional[str] = None,
 ) -> None:
-    """Create COMBINE archive (http://co.mbine.org/documents/archive) based
+    """Create COMBINE archive (https://co.mbine.org/documents/archive) based
     on PEtab YAML file.
 
     Arguments:
         yaml_file: Path to PEtab YAML file
+        filename: Destination file name
         family_name: Family name of archive creator
         given_name: Given name of archive creator
         email: E-mail address of archive creator
         organization: Organization of archive creator
     """
 
-    path_prefix = os.path.dirname(yaml_file)
+    path_prefix = os.path.dirname(str(yaml_file))
     yaml_config = yaml.load_yaml(yaml_file)
 
     # function-level import, because module-level import interfered with
     # other SWIG interfaces
     try:
         import libcombine
     except ImportError:
@@ -348,17 +392,17 @@
             libcombine.OmexDescription.getCurrentDateAndTime())
         archive.addMetadata(location, omex_description)
 
     archive = libcombine.CombineArchive()
 
     # Add PEtab files and metadata
     archive.addFile(
-        yaml_file,
+        str(yaml_file),
         os.path.basename(yaml_file),
-        libcombine.KnownFormats.lookupFormat("yaml"),
+        "http://identifiers.org/combine.specifications/petab.version-1",
         True
     )
     _add_file_metadata(location=os.path.basename(yaml_file),
                        description="PEtab YAML file")
 
     # Add parameter file(s) that describe a single parameter table.
     # Works for a single file name, or a list of file names.
@@ -416,22 +460,23 @@
     if email:
         creator.setEmail(email)
     if organization:
         creator.setOrganization(organization)
     description.addCreator(creator)
 
     archive.addMetadata(".", description)
-    archive.writeToFile(filename)
+    archive.writeToFile(str(filename))
 
 
 def unique_preserve_order(seq: Sequence) -> List:
     """Return a list of unique elements in Sequence, keeping only the first
     occurrence of each element
 
-    seq: Sequence to prune
+    Parameters:
+        seq: Sequence to prune
 
     Returns:
         List of unique elements in ``seq``
     """
     seen = set()
     seen_add = seen.add
     return [x for x in seq if not (x in seen or seen_add(x))]
```

### Comparing `petab-0.1.8/petab/sampling.py` & `petab-0.2.0/petab/sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 import pandas as pd
 
 from typing import Tuple
 
 from . import parameters
 from .C import *  # noqa: F403
 
+__all__ = ['sample_from_prior', 'sample_parameter_startpoints']
 
-def sample_from_prior(prior: Tuple[str, list, str, list],
-                      n_starts: int) -> np.array:
+
+def sample_from_prior(
+        prior: Tuple[str, list, str, list],
+        n_starts: int
+) -> np.array:
     """Creates samples for one parameter based on prior
 
     Arguments:
-        prior: A tuple as obtained from ``petab.parameter.get_priors_from_df``
+        prior: A tuple as obtained from
+            :func:`petab.parameter.get_priors_from_df`
         n_starts: Number of samples
 
     Returns:
         Array with sampled values
     """
-
     # unpack info
     p_type, p_params, scaling, bounds = prior
 
     # define a function to rescale the sampled points to parameter scale
     def scale(x):
         if scaling == LIN:
             return x
@@ -34,16 +38,15 @@
             return np.log10(x)
         raise NotImplementedError(
             f"Parameter priors on the parameter scale {scaling} are "
             "currently not implemented.")
 
     def clip_to_bounds(x: np.array):
         """Clip values in array x to bounds"""
-        x = np.maximum(np.minimum(scale(bounds[1]), x), scale(bounds[0]))
-        return x
+        return np.maximum(np.minimum(scale(bounds[1]), x), scale(bounds[0]))
 
     # define lambda functions for each parameter
     if p_type == UNIFORM:
         sp = scale((p_params[1] - p_params[0]) * np.random.random((
             n_starts,)) + p_params[0])
 
     elif p_type == PARAMETER_SCALE_UNIFORM:
@@ -77,23 +80,25 @@
     else:
         raise NotImplementedError(
             f"Parameter priors of type {prior[0]} are not implemented.")
 
     return clip_to_bounds(sp)
 
 
-def sample_parameter_startpoints(parameter_df: pd.DataFrame,
-                                 n_starts: int = 100,
-                                 seed: int = None) -> np.array:
-    """Create numpy.array with starting points for an optimization
+def sample_parameter_startpoints(
+        parameter_df: pd.DataFrame,
+        n_starts: int = 100,
+        seed: int = None,
+) -> np.array:
+    """Create :class:`numpy.array` with starting points for an optimization
 
     Arguments:
         parameter_df: PEtab parameter DataFrame
         n_starts: Number of points to be sampled
-        seed: Random number generator seed (see numpy.random.seed)
+        seed: Random number generator seed (see :func:`numpy.random.seed`)
 
     Returns:
         Array of sampled starting points with dimensions
         n_startpoints x n_optimization_parameters
     """
     if seed is not None:
         np.random.seed(seed)
```

### Comparing `petab-0.1.8/petab/calculate.py` & `petab-0.2.0/petab/calculate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """Functions performing various calculations."""
 
+import numbers
+from functools import reduce
+from typing import Dict, List, Union
+
 import numpy as np
 import pandas as pd
-from functools import reduce
-from typing import List, Union
 import sympy
-import numbers
+from sympy.abc import _clash
 
-from .C import *
 import petab
+from .C import *
+
+__all__ = ['calculate_residuals', 'calculate_residuals_for_table',
+           'get_symbolic_noise_formulas', 'evaluate_noise_formula',
+           'calculate_chi2', 'calculate_chi2_for_table_from_residuals',
+           'calculate_llh', 'calculate_llh_for_table', 'calculate_single_llh']
 
 
 def calculate_residuals(
         measurement_dfs: Union[List[pd.DataFrame], pd.DataFrame],
         simulation_dfs: Union[List[pd.DataFrame], pd.DataFrame],
         observable_dfs: Union[List[pd.DataFrame], pd.DataFrame],
         parameter_dfs: Union[List[pd.DataFrame], pd.DataFrame],
@@ -33,17 +40,16 @@
         normalize:
             Whether to normalize residuals by the noise standard deviation
             terms.
         scale:
             Whether to calculate residuals of scaled values.
 
     Returns:
-        residual_dfs:
-            Data frames in the same structure as `measurement_dfs`
-            with a field `residual` instead of measurement.
+        List of DataFrames in the same structure as `measurement_dfs`
+        with a field `residual` instead of measurement.
     """
     # convenience
     if isinstance(measurement_dfs, pd.DataFrame):
         measurement_dfs = [measurement_dfs]
     if isinstance(simulation_dfs, pd.DataFrame):
         simulation_dfs = [simulation_dfs]
     if isinstance(observable_dfs, pd.DataFrame):
@@ -68,15 +74,15 @@
         observable_df: pd.DataFrame,
         parameter_df: pd.DataFrame,
         normalize: bool = True,
         scale: bool = True
 ) -> pd.DataFrame:
     """
     Calculate residuals for a single measurement table.
-    For the argumenets, see `calculate_residuals`.
+    For the arguments, see `calculate_residuals`.
     """
     # create residual df as copy of measurement df, change column
     residual_df = measurement_df.copy(deep=True).rename(
         columns={MEASUREMENT: RESIDUAL})
 
     # matching columns
     compared_cols = set(MEASUREMENT_DF_COLS)
@@ -113,62 +119,64 @@
         residual /= noise_value
 
         # fill in value
         residual_df.loc[irow, RESIDUAL] = residual
     return residual_df
 
 
-def get_symbolic_noise_formulas(observable_df) -> dict:
+def get_symbolic_noise_formulas(observable_df) -> Dict[str, sympy.Expr]:
     """Sympify noise formulas.
 
     Arguments:
-        obervable_df: The observable table.
+        observable_df: The observable table.
 
     Returns:
-        noise_formulas: Dictionary of {observable_id}: {noise_formula}.
+        Dictionary of {observable_id}: {noise_formula}.
     """
     noise_formulas = {}
     # iterate over observables
     for row in observable_df.itertuples():
         observable_id = row.Index
         if NOISE_FORMULA not in observable_df.columns:
             noise_formula = None
         else:
-            noise_formula = sympy.sympify(row.noiseFormula)
+            noise_formula = sympy.sympify(row.noiseFormula, locals=_clash)
         noise_formulas[observable_id] = noise_formula
     return noise_formulas
 
 
 def evaluate_noise_formula(
         measurement: pd.Series,
-        noise_formulas: dict,
+        noise_formulas: Dict[str, sympy.Expr],
         parameter_df: pd.DataFrame,
-        simulation: float) -> float:
+        simulation: numbers.Number,
+) -> float:
     """Fill in parameters for `measurement` and evaluate noise_formula.
 
     Arguments:
         measurement: A measurement table row.
         noise_formulas: The noise formulas as computed by
             `get_symbolic_noise_formulas`.
         parameter_df: The parameter table.
         simulation: The simulation corresponding to the measurement, scaled.
 
     Returns:
-        noise_value: The noise value.
+        The noise value.
     """
     # the observable id
     observable_id = measurement[OBSERVABLE_ID]
 
     # extract measurement specific overrides
     observable_parameter_overrides = petab.split_parameter_replacement_list(
         measurement.get(NOISE_PARAMETERS, None))
-    overrides = {}
     # fill in measurement specific parameters
-    for i_obs_par, obs_par in enumerate(observable_parameter_overrides):
-        overrides[f"noiseParameter{i_obs_par+1}_{observable_id}"] = obs_par
+    overrides = {
+        f"noiseParameter{i_obs_par + 1}_{observable_id}": obs_par
+        for i_obs_par, obs_par in enumerate(observable_parameter_overrides)
+    }
 
     # fill in observables
     overrides[observable_id] = simulation
 
     # fill in general parameters
     for row in parameter_df.itertuples():
         overrides[row.Index] = row.nominalValue
@@ -182,18 +190,20 @@
     # replace parameters by values in formula
     noise_formula = noise_formulas[observable_id]
     noise_value = noise_formula.subs(overrides)
 
     # conversion is possible if all parameters are replaced
     try:
         noise_value = float(noise_value)
-    except TypeError:
-        raise TypeError(
+    except TypeError as e:
+        raise ValueError(
             f"Cannot replace all parameters in noise formula {noise_value} "
-            f"for observable {observable_id}.")
+            f"for observable {observable_id}. "
+            f"Missing {noise_formula.free_symbols}. Note that model states "
+            "are currently not supported.") from e
     return noise_value
 
 
 def calculate_chi2(
         measurement_dfs: Union[List[pd.DataFrame], pd.DataFrame],
         simulation_dfs: Union[List[pd.DataFrame], pd.DataFrame],
         observable_dfs: Union[List[pd.DataFrame], pd.DataFrame],
@@ -215,27 +225,27 @@
         normalize:
             Whether to normalize residuals by the noise standard deviation
             terms.
         scale:
             Whether to calculate residuals of scaled values.
 
     Returns:
-        chi2: The aggregated chi2 value.
+        The aggregated chi2 value.
     """
     residual_dfs = calculate_residuals(
         measurement_dfs, simulation_dfs, observable_dfs, parameter_dfs,
         normalize, scale)
     chi2s = [calculate_chi2_for_table_from_residuals(df)
              for df in residual_dfs]
-    chi2 = sum(chi2s)
-    return chi2
+    return sum(chi2s)
 
 
 def calculate_chi2_for_table_from_residuals(
-        residual_df: pd.DataFrame) -> float:
+        residual_df: pd.DataFrame,
+) -> float:
     """Compute chi2 value for a single residual table."""
     return (np.array(residual_df[RESIDUAL])**2).sum()
 
 
 def calculate_llh(
         measurement_dfs: Union[List[pd.DataFrame], pd.DataFrame],
         simulation_dfs: Union[List[pd.DataFrame], pd.DataFrame],
@@ -251,15 +261,15 @@
             Simulation tables corresponding to the measurement tables.
         observable_dfs:
             The problem observable tables.
         parameter_dfs:
             The problem parameter tables.
 
     Returns:
-        llh: The log-likelihood.
+        The log-likelihood.
     """
     # convenience
     if isinstance(measurement_dfs, pd.DataFrame):
         measurement_dfs = [measurement_dfs]
     if isinstance(simulation_dfs, pd.DataFrame):
         simulation_dfs = [simulation_dfs]
     if isinstance(observable_dfs, pd.DataFrame):
@@ -270,16 +280,15 @@
     # iterate over data frames
     llhs = []
     for (measurement_df, simulation_df, observable_df, parameter_df) in zip(
             measurement_dfs, simulation_dfs, observable_dfs, parameter_dfs):
         _llh = calculate_llh_for_table(
             measurement_df, simulation_df, observable_df, parameter_df)
         llhs.append(_llh)
-    llh = sum(llhs)
-    return llh
+    return sum(llhs)
 
 
 def calculate_llh_for_table(
         measurement_df: pd.DataFrame,
         simulation_df: pd.DataFrame,
         observable_df: pd.DataFrame,
         parameter_df: pd.DataFrame) -> float:
@@ -318,16 +327,15 @@
 
         # get noise distribution
         noise_distribution = observable.get(NOISE_DISTRIBUTION, NORMAL)
 
         llh = calculate_single_llh(
             measurement, simulation, scale, noise_distribution, noise_value)
         llhs.append(llh)
-    llh = sum(llhs)
-    return llh
+    return sum(llhs)
 
 
 def calculate_single_llh(
         measurement: float,
         simulation: float,
         scale: str,
         noise_distribution: str,
@@ -339,15 +347,15 @@
         simulation: The simulated value.
         scale: The scale on which the noise model is to be applied.
         noise_distribution: The noise distribution.
         noise_value: The considered noise models possess a single noise
             parameter, e.g. the normal standard deviation.
 
     Returns:
-        llh: The computed likelihood for the given values.
+        The computed likelihood for the given values.
     """
     # short-hand
     m, s, sigma = measurement, simulation, noise_value
     pi, log, log10 = np.pi, np.log, np.log10
 
     # go over the possible cases
     if noise_distribution == NORMAL and scale == LIN:
@@ -359,9 +367,12 @@
             0.5*((log10(s)-log10(m))/sigma)**2
     elif noise_distribution == LAPLACE and scale == LIN:
         nllh = log(2*sigma) + abs((s-m)/sigma)
     elif noise_distribution == LAPLACE and scale == LOG:
         nllh = log(2*sigma*m) + abs((log(s)-log(m))/sigma)
     elif noise_distribution == LAPLACE and scale == LOG10:
         nllh = log(2*sigma*m*log(10)) + abs((log10(s)-log10(m))/sigma)
-    llh = - nllh
-    return llh
+    else:
+        raise NotImplementedError(
+            "Unsupported combination of noise_distribution and scale "
+            f"specified: {noise_distribution}, {scale}.")
+    return -nllh
```

### Comparing `petab-0.1.8/petab/parameters.py` & `petab-0.2.0/petab/parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,112 @@
 """Functions operating on the PEtab parameter table"""
 
 import numbers
-import pandas as pd
-import numpy as np
+import warnings
 from collections import OrderedDict
-from typing import Iterable, Set, List, Tuple, Dict, Union
+from pathlib import Path
+from typing import (
+    Dict, Iterable, List, Set, Tuple, Union, Optional, Literal, Sequence
+)
 
 import libsbml
+import numpy as np
+import pandas as pd
 
-from . import lint, core, measurements, conditions, observables
+from . import conditions, core, lint, measurements, observables
 from .C import *  # noqa: F403
+from .models import Model
+
+__all__ = ['create_parameter_df',
+           'get_optimization_parameter_scaling',
+           'get_optimization_parameters',
+           'get_parameter_df',
+           'get_priors_from_df',
+           'get_valid_parameters_for_parameter_table',
+           'map_scale',
+           'map_unscale',
+           'normalize_parameter_df',
+           'scale',
+           'unscale',
+           'write_parameter_df']
+
+PARAMETER_SCALE_ARGS = Literal['', 'lin', 'log', 'log10']
 
 
 def get_parameter_df(
-        parameter_file: Union[str, List[str], pd.DataFrame, None]
-) -> pd.DataFrame:
+        parameter_file: Union[str, Path, pd.DataFrame,
+                              Iterable[Union[str, Path, pd.DataFrame]], None]
+) -> Union[pd.DataFrame, None]:
     """
     Read the provided parameter file into a ``pandas.Dataframe``.
 
     Arguments:
-        parameter_file: Name of the file to read from or pandas.Dataframe.
+        parameter_file: Name of the file to read from or pandas.Dataframe,
+        or an Iterable.
 
     Returns:
-        Parameter DataFrame
+        Parameter ``DataFrame``, or ``None`` if ``None`` was passed.
     """
     if parameter_file is None:
-        return parameter_file
-
-    parameter_df = None
-
+        return None
     if isinstance(parameter_file, pd.DataFrame):
         parameter_df = parameter_file
-
-    if isinstance(parameter_file, str):
+    elif isinstance(parameter_file, (str, Path)):
         parameter_df = pd.read_csv(parameter_file, sep='\t',
                                    float_precision='round_trip')
+    elif isinstance(parameter_file, Iterable):
+        dfs = [get_parameter_df(x) for x in parameter_file if x]
 
-    if isinstance(parameter_file, list):
-        parameter_df = pd.concat([pd.read_csv(subset_file, sep='\t',
-                                              float_precision='round_trip')
-                                  for subset_file in parameter_file])
-        # Remove identical parameter definitions
-        parameter_df.drop_duplicates(inplace=True, ignore_index=True)
+        if not dfs:
+            return None
+
+        parameter_df = pd.concat(dfs)
         # Check for contradicting parameter definitions
-        parameter_duplicates = set(parameter_df[PARAMETER_ID].loc[
-            parameter_df[PARAMETER_ID].duplicated()])
-        if parameter_duplicates:
-            raise ValueError(
-                f'The values of {PARAMETER_ID} must be unique or'
-                ' identical between all parameter subset files. The'
-                ' following duplicates were found:\n'
-                f'{parameter_duplicates}'
-            )
+        _check_for_contradicting_parameter_definitions(parameter_df)
+
+        return parameter_df
 
     lint.assert_no_leading_trailing_whitespace(
         parameter_df.columns.values, "parameter")
 
     if not isinstance(parameter_df.index, pd.RangeIndex):
         parameter_df.reset_index(inplace=True)
 
     try:
         parameter_df.set_index([PARAMETER_ID], inplace=True)
-    except KeyError:
+    except KeyError as e:
         raise KeyError(
-            f"Parameter table missing mandatory field {PARAMETER_ID}.")
+            f"Parameter table missing mandatory field {PARAMETER_ID}.") from e
+    _check_for_contradicting_parameter_definitions(parameter_df)
 
     return parameter_df
 
 
-def write_parameter_df(df: pd.DataFrame, filename: str) -> None:
+def _check_for_contradicting_parameter_definitions(parameter_df: pd.DataFrame):
+    """
+    Raises a ValueError for non-unique parameter IDs
+    """
+    parameter_duplicates = set(parameter_df.index.values[
+                                    parameter_df.index.duplicated()])
+    if parameter_duplicates:
+        raise ValueError(
+            f'The values of `{PARAMETER_ID}` must be unique. The '
+            f'following duplicates were found:\n{parameter_duplicates}'
+        )
+
+
+def write_parameter_df(df: pd.DataFrame, filename: Union[str, Path]) -> None:
     """Write PEtab parameter table
 
     Arguments:
         df: PEtab parameter table
         filename: Destination file name
     """
-    with open(filename, 'w') as fh:
-        df.to_csv(fh, sep='\t', index=True)
+    df = get_parameter_df(df)
+    df.to_csv(filename, sep='\t', index=True)
 
 
 def get_optimization_parameters(parameter_df: pd.DataFrame) -> List[str]:
     """
     Get list of optimization parameter IDs from parameter table.
 
     Arguments:
@@ -105,52 +131,70 @@
         Dictionary with optimization parameter IDs mapped to parameter scaling
         strings.
     """
     estimated_df = parameter_df.loc[parameter_df[ESTIMATE] == 1]
     return dict(zip(estimated_df.index, estimated_df[PARAMETER_SCALE]))
 
 
-def create_parameter_df(sbml_model: libsbml.Model,
-                        condition_df: pd.DataFrame,
-                        observable_df: pd.DataFrame,
-                        measurement_df: pd.DataFrame,
-                        include_optional: bool = False,
-                        parameter_scale: str = LOG10,
-                        lower_bound: Iterable = None,
-                        upper_bound: Iterable = None) -> pd.DataFrame:
+def create_parameter_df(
+        sbml_model: Optional[libsbml.Model] = None,
+        condition_df: Optional[pd.DataFrame] = None,
+        observable_df: Optional[pd.DataFrame] = None,
+        measurement_df: Optional[pd.DataFrame] = None,
+        model: Optional[Model] = None,
+        include_optional: bool = False,
+        parameter_scale: str = LOG10,
+        lower_bound: Iterable = None,
+        upper_bound: Iterable = None,
+        mapping_df: Optional[pd.DataFrame] = None,
+) -> pd.DataFrame:
     """Create a new PEtab parameter table
 
     All table entries can be provided as string or list-like with length
     matching the number of parameters
 
     Arguments:
-        sbml_model: SBML Model
+        sbml_model: SBML Model (deprecated, mutually exclusive with ``model``)
+        model: PEtab model (mutually exclusive with ``sbml_model``)
         condition_df: PEtab condition DataFrame
+        observable_df: PEtab observable DataFrame
         measurement_df: PEtab measurement DataFrame
         include_optional: By default this only returns parameters that are
-            required to be present in the parameter table. If set to True,
+            required to be present in the parameter table. If set to ``True``,
             this returns all parameters that are allowed to be present in the
             parameter table (i.e. also including parameters specified in the
-            SBML model).
+            model).
         parameter_scale: parameter scaling
         lower_bound: lower bound for parameter value
         upper_bound: upper bound for parameter value
+        mapping_df: PEtab mapping DataFrame
 
     Returns:
         The created parameter DataFrame
     """
-
+    if sbml_model:
+        warnings.warn("Passing a model via the `sbml_model` argument is "
+                      "deprecated, use `model=petab.models.sbml_model."
+                      "SbmlModel(...)` instead.", DeprecationWarning,
+                      stacklevel=2)
+        from petab.models.sbml_model import SbmlModel
+        if model:
+            raise ValueError("Arguments `model` and `sbml_model` are "
+                             "mutually exclusive.")
+        model = SbmlModel(sbml_model=sbml_model)
     if include_optional:
         parameter_ids = list(get_valid_parameters_for_parameter_table(
-            sbml_model=sbml_model, condition_df=condition_df,
+            model=model, condition_df=condition_df,
             observable_df=observable_df, measurement_df=measurement_df))
     else:
         parameter_ids = list(get_required_parameters_for_parameter_table(
-            sbml_model=sbml_model, condition_df=condition_df,
-            observable_df=observable_df, measurement_df=measurement_df))
+            model=model, condition_df=condition_df,
+            observable_df=observable_df, measurement_df=measurement_df,
+            mapping_df=mapping_df
+        ))
 
     df = pd.DataFrame(
         data={
             PARAMETER_ID: parameter_ids,
             PARAMETER_NAME: parameter_ids,
             PARAMETER_SCALE: parameter_scale,
             LOWER_BOUND: lower_bound,
@@ -160,48 +204,49 @@
             INITIALIZATION_PRIOR_TYPE: '',
             INITIALIZATION_PRIOR_PARAMETERS: '',
             OBJECTIVE_PRIOR_TYPE: '',
             OBJECTIVE_PRIOR_PARAMETERS: '',
         })
     df.set_index([PARAMETER_ID], inplace=True)
 
-    # For SBML model parameters, set nominal values as defined in the model
+    # For model parameters, set nominal values as defined in the model
     for parameter_id in df.index:
         try:
-            parameter = sbml_model.getParameter(parameter_id)
-            if parameter:
-                df.loc[parameter_id, NOMINAL_VALUE] = parameter.getValue()
+            df.loc[parameter_id, NOMINAL_VALUE] = \
+                model.get_parameter_value(parameter_id)
         except ValueError:
             # parameter was introduced as condition-specific override and
             # is potentially not present in the model
             pass
     return df
 
 
 def get_required_parameters_for_parameter_table(
-        sbml_model: libsbml.Model,
+        model: Model,
         condition_df: pd.DataFrame,
         observable_df: pd.DataFrame,
-        measurement_df: pd.DataFrame) -> Set[str]:
+        measurement_df: pd.DataFrame,
+        mapping_df: pd.DataFrame = None
+) -> Set[str]:
     """
     Get set of parameters which need to go into the parameter table
 
     Arguments:
-        sbml_model: PEtab SBML model
+        model: PEtab model
         condition_df: PEtab condition table
         observable_df: PEtab observable table
         measurement_df: PEtab measurement table
+        mapping_df: PEtab mapping table
 
     Returns:
         Set of parameter IDs which PEtab requires to be present in the
         parameter table. That is all {observable,noise}Parameters from the
         measurement table as well as all parametric condition table overrides
-        that are not defined in the SBML model.
+        that are not defined in the model.
     """
-
     # use ordered dict as proxy for ordered set
     parameter_ids = OrderedDict()
 
     # Add parameters from measurement table, unless they are fixed parameters
     def append_overrides(overrides):
         for p in overrides:
             if isinstance(p, str) and p not in condition_df.columns:
@@ -211,112 +256,135 @@
         # we trust that the number of overrides matches
         append_overrides(measurements.split_parameter_replacement_list(
             row.get(OBSERVABLE_PARAMETERS, None)))
         append_overrides(measurements.split_parameter_replacement_list(
             row.get(NOISE_PARAMETERS, None)))
 
     # Add output parameters except for placeholders
-    output_parameters = observables.get_output_parameters(
-        observable_df, sbml_model)
-    placeholders = observables.get_placeholders(observable_df)
-    for p in output_parameters:
-        if p not in placeholders and sbml_model.getParameter(p) is None:
-            parameter_ids[p] = None
+    for kwargs in [dict(observables=True, noise=False),
+                   dict(observables=False, noise=True)]:
+        output_parameters = observables.get_output_parameters(
+            observable_df, model, mapping_df=mapping_df, **kwargs)
+        placeholders = observables.get_placeholders(
+            observable_df, **kwargs)
+        for p in output_parameters:
+            if p not in placeholders:
+                parameter_ids[p] = None
 
     # Add condition table parametric overrides unless already defined in the
-    # SBML model
+    #  model
     for p in conditions.get_parametric_overrides(condition_df):
-        if sbml_model.getParameter(p) is None:
+        if not model.has_entity_with_id(p):
             parameter_ids[p] = None
 
+    # remove parameters that occur in the condition table and are overridden
+    #  for ALL conditions
+    for p in condition_df.columns[~condition_df.isnull().any()]:
+        try:
+            del parameter_ids[p]
+        except KeyError:
+            pass
     return parameter_ids.keys()
 
 
 def get_valid_parameters_for_parameter_table(
-        sbml_model: libsbml.Model,
+        model: Model,
         condition_df: pd.DataFrame,
         observable_df: pd.DataFrame,
-        measurement_df: pd.DataFrame) -> Set[str]:
+        measurement_df: pd.DataFrame,
+        mapping_df: pd.DataFrame = None,
+) -> Set[str]:
     """
     Get set of parameters which may be present inside the parameter table
 
     Arguments:
-        sbml_model: PEtab SBML model
+        model: PEtab model
         condition_df: PEtab condition table
         observable_df: PEtab observable table
         measurement_df: PEtab measurement table
+        mapping_df: PEtab mapping table for additional checks
 
     Returns:
         Set of parameter IDs which PEtab allows to be present in the
         parameter table.
     """
-
-    # - grab all model parameters
+    # - grab all allowed model parameters
+    # - grab corresponding names from mapping table
     # - grab all output parameters defined in {observable,noise}Formula
     # - grab all parameters from measurement table
     # - grab all parametric overrides from condition table
     # - remove parameters for which condition table columns exist
-    # - remove observables assigment targets
-    # - remove sigma assignment targets
     # - remove placeholder parameters
     #   (only partial overrides are not supported)
 
-    placeholders = set(observables.get_placeholders(observable_df))
-
-    # exclude rule targets
-    assignment_targets = {ar.getVariable()
-                          for ar in sbml_model.getListOfRules()}
-
     # must not go into parameter table
     blackset = set()
-    # collect assignment targets
-    blackset |= placeholders
-    blackset |= assignment_targets
-    blackset |= set(condition_df.columns.values) - {CONDITION_NAME}
 
-    # use ordered dict as proxy for ordered set
-    parameter_ids = OrderedDict.fromkeys(
-        p.getId() for p in sbml_model.getListOfParameters()
-        if p.getId() not in blackset)
+    if observable_df is not None:
+        placeholders = set(observables.get_placeholders(observable_df))
 
-    # add output parameters from observables table
-    output_parameters = observables.get_output_parameters(
-        observable_df, sbml_model)
-    for p in output_parameters:
-        if p not in blackset:
-            parameter_ids[p] = None
+        # collect assignment targets
+        blackset |= placeholders
+
+    if condition_df is not None:
+        blackset |= set(condition_df.columns.values) - {CONDITION_NAME}
+
+    # don't use sets here, to have deterministic ordering,
+    #  e.g. for creating parameter tables
+    parameter_ids = OrderedDict.fromkeys(
+        p for p in model.get_valid_parameters_for_parameter_table()
+        if p not in blackset
+    )
+
+    if mapping_df is not None:
+        for from_id, to_id in zip(mapping_df.index.values,
+                                  mapping_df[MODEL_ENTITY_ID]):
+            if to_id in parameter_ids.keys():
+                parameter_ids[from_id] = None
+
+    if observable_df is not None:
+        # add output parameters from observables table
+        output_parameters = observables.get_output_parameters(
+            observable_df=observable_df, model=model)
+        for p in output_parameters:
+            if p not in blackset:
+                parameter_ids[p] = None
 
     # Append parameters from measurement table, unless they occur as condition
     # table columns
     def append_overrides(overrides):
         for p in overrides:
             if isinstance(p, str) and p not in blackset:
                 parameter_ids[p] = None
 
-    for _, row in measurement_df.iterrows():
-        # we trust that the number of overrides matches
-        append_overrides(measurements.split_parameter_replacement_list(
-            row.get(OBSERVABLE_PARAMETERS, None)))
-        append_overrides(measurements.split_parameter_replacement_list(
-            row.get(NOISE_PARAMETERS, None)))
+    if measurement_df is not None:
+        for _, row in measurement_df.iterrows():
+            # we trust that the number of overrides matches
+            append_overrides(measurements.split_parameter_replacement_list(
+                row.get(OBSERVABLE_PARAMETERS, None)))
+            append_overrides(measurements.split_parameter_replacement_list(
+                row.get(NOISE_PARAMETERS, None)))
 
     # Append parameter overrides from condition table
-    for p in conditions.get_parametric_overrides(condition_df):
-        parameter_ids[p] = None
+    if condition_df is not None:
+        for p in conditions.get_parametric_overrides(condition_df):
+            parameter_ids[p] = None
 
     return parameter_ids.keys()
 
 
-def get_priors_from_df(parameter_df: pd.DataFrame,
-                       mode: str) -> List[Tuple]:
+def get_priors_from_df(
+        parameter_df: pd.DataFrame,
+        mode: Literal['initialization', 'objective'],
+) -> List[Tuple]:
     """Create list with information about the parameter priors
 
     Arguments:
         parameter_df: PEtab parameter table
-        mode: 'initialization' or 'objective'
+        mode: ``'initialization'`` or ``'objective'``
 
     Returns:
         List with prior information.
     """
 
     # get types and parameters of priors from dataframe
     par_to_estimate = parameter_df.loc[parameter_df[ESTIMATE] == 1]
@@ -329,83 +397,123 @@
             prior_type = PARAMETER_SCALE_UNIFORM
 
         # retrieve info about parameters of priors, make it a tuple of floats
         pars_str = str(row.get(f'{mode}PriorParameters', ''))
         if core.is_empty(pars_str):
             lb, ub = map_scale([row[LOWER_BOUND], row[UPPER_BOUND]],
                                [row[PARAMETER_SCALE]] * 2)
-            pars_str = f'{lb};{ub}'
-        prior_pars = tuple([float(entry) for entry in pars_str.split(';')])
+            pars_str = f'{lb}{PARAMETER_SEPARATOR}{ub}'
+        prior_pars = tuple(
+            float(entry) for entry in pars_str.split(PARAMETER_SEPARATOR)
+        )
 
         # add parameter scale and bounds, as this may be needed
         par_scale = row[PARAMETER_SCALE]
         par_bounds = (row[LOWER_BOUND], row[UPPER_BOUND])
 
         # if no prior is specified, we assume a non-informative (uniform) one
         if prior_type == 'nan':
             prior_type = PARAMETER_SCALE_UNIFORM
-            prior_pars = (row[LOWER_BOUND], row[UPPER_BOUND])
+            prior_pars = (scale(row[LOWER_BOUND], par_scale),
+                          scale(row[UPPER_BOUND], par_scale))
 
         prior_list.append((prior_type, prior_pars, par_scale, par_bounds))
 
     return prior_list
 
 
-def scale(parameter: numbers.Number, scale_str: 'str') -> numbers.Number:
-    """Scale parameter according to scale_str
+def scale(
+        parameter: numbers.Number,
+        scale_str: PARAMETER_SCALE_ARGS,
+) -> numbers.Number:
+    """Scale parameter according to ``scale_str``.
 
     Arguments:
         parameter:
             Parameter to be scaled.
         scale_str:
-            One of 'lin' (synonymous with ''), 'log', 'log10'.
+            One of ``'lin'`` (synonymous with ``''``), ``'log'``, ``'log10'``.
 
     Returns:
-        parameter:
-            The scaled parameter.
+        The scaled parameter.
     """
-
     if scale_str == LIN or not scale_str:
         return parameter
     if scale_str == LOG:
         return np.log(parameter)
     if scale_str == LOG10:
         return np.log10(parameter)
-    raise ValueError("Invalid parameter scaling: " + scale_str)
+    raise ValueError(f"Invalid parameter scaling: {scale_str}")
 
 
-def unscale(parameter: numbers.Number, scale_str: 'str') -> numbers.Number:
-    """Unscale parameter according to scale_str
+def unscale(
+        parameter: numbers.Number,
+        scale_str: PARAMETER_SCALE_ARGS,
+) -> numbers.Number:
+    """Unscale parameter according to ``scale_str``.
 
     Arguments:
         parameter:
             Parameter to be unscaled.
         scale_str:
-            One of 'lin' (synonymous with ''), 'log', 'log10'.
+            One of ``'lin'`` (synonymous with ``''``), ``'log'``, ``'log10'``.
 
     Returns:
-        parameter:
-            The unscaled parameter.
+        The unscaled parameter.
     """
-
     if scale_str == LIN or not scale_str:
         return parameter
     if scale_str == LOG:
         return np.exp(parameter)
     if scale_str == LOG10:
         return 10**parameter
-    raise ValueError("Invalid parameter scaling: " + scale_str)
+    raise ValueError(f"Invalid parameter scaling: {scale_str}")
 
 
-def map_scale(parameters: Iterable[numbers.Number],
-              scale_strs: Iterable[str]) -> Iterable[numbers.Number]:
-    """As scale(), but for Iterables"""
+def map_scale(
+    parameters: Sequence[numbers.Number],
+    scale_strs: Union[Iterable[PARAMETER_SCALE_ARGS], PARAMETER_SCALE_ARGS],
+) -> Iterable[numbers.Number]:
+    """Scale the parameters, i.e. as :func:`scale`, but for Sequences.
+
+    Arguments:
+        parameters:
+            Parameters to be scaled.
+        scale_strs:
+            Scales to apply. Broadcast if a single string.
+
+    Returns:
+        The scaled parameters.
+    """
+    if isinstance(scale_strs, str):
+        scale_strs = [scale_strs] * len(parameters)
     return map(lambda x: scale(x[0], x[1]), zip(parameters, scale_strs))
 
 
+def map_unscale(
+    parameters: Sequence[numbers.Number],
+    scale_strs: Union[Iterable[PARAMETER_SCALE_ARGS], PARAMETER_SCALE_ARGS],
+) -> Iterable[numbers.Number]:
+    """Unscale the parameters, i.e. as :func:`unscale`, but for Sequences.
+
+    Arguments:
+        parameters:
+            Parameters to be unscaled.
+        scale_strs:
+            Scales that the parameters are currently on.
+            Broadcast if a single string.
+
+    Returns:
+        The unscaled parameters.
+    """
+    if isinstance(scale_strs, str):
+        scale_strs = [scale_strs] * len(parameters)
+    return map(lambda x: unscale(x[0], x[1]), zip(parameters, scale_strs))
+
+
 def normalize_parameter_df(parameter_df: pd.DataFrame) -> pd.DataFrame:
     """Add missing columns and fill in default values."""
     df = parameter_df.copy(deep=True)
 
     if PARAMETER_NAME not in df:
         df[PARAMETER_NAME] = df.reset_index()[PARAMETER_ID]
 
@@ -425,10 +533,10 @@
         if prior_par_col not in df:
             df[prior_par_col] = None
         for irow, row in df.iterrows():
             if core.is_empty(row[prior_par_col]) \
                     and row[prior_type_col] == PARAMETER_SCALE_UNIFORM:
                 lb, ub = map_scale([row[LOWER_BOUND], row[UPPER_BOUND]],
                                    [row[PARAMETER_SCALE]] * 2)
-                df.loc[irow, prior_par_col] = f'{lb};{ub}'
+                df.loc[irow, prior_par_col] = f'{lb}{PARAMETER_SEPARATOR}{ub}'
 
     return df
```

### Comparing `petab-0.1.8/petab/composite_problem.py` & `petab-0.2.0/petab/composite_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 import pandas as pd
 
 from . import parameters
 from . import problem
 from . import yaml
 from .C import *  # noqa: F403
 
+__all__ = ['CompositeProblem']
+
 
 class CompositeProblem:
     """Representation of a PEtab problem consisting of multiple models
 
     Attributes:
         problems:
-            List ``petab.Problems``
+            List of :py:class:`petab.Problem` s
         parameter_df:
             PEtab parameter DataFrame
     """
 
     def __init__(
             self,
             parameter_df: pd.DataFrame = None,
```

### Comparing `petab-0.1.8/petab/measurements.py` & `petab-0.2.0/petab/measurements.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,68 @@
 """Functions operating on the PEtab measurement table"""
 # noqa: F405
 
-
 import itertools
+import math
 import numbers
-from typing import List, Union, Dict
-from warnings import warn
+from pathlib import Path
+from typing import Dict, List, Union
 
 import numpy as np
 import pandas as pd
 
-from . import (lint, core, observables)
+from . import (core, lint, observables)
 from .C import *  # noqa: F403
 
+__all__ = ['assert_overrides_match_parameter_count',
+           'create_measurement_df',
+           'get_measurement_df',
+           'get_measurement_parameter_ids',
+           'get_rows_for_condition',
+           'get_simulation_conditions',
+           'measurements_have_replicates',
+           'measurement_is_at_steady_state',
+           'split_parameter_replacement_list',
+           'write_measurement_df']
+
 
 def get_measurement_df(
-        measurement_file: Union[None, str, pd.DataFrame]
+        measurement_file: Union[None, str, Path, pd.DataFrame]
 ) -> pd.DataFrame:
     """
     Read the provided measurement file into a ``pandas.Dataframe``.
 
     Arguments:
         measurement_file: Name of file to read from or pandas.Dataframe
 
     Returns:
         Measurement DataFrame
     """
     if measurement_file is None:
         return measurement_file
 
-    if isinstance(measurement_file, str):
+    if isinstance(measurement_file, (str, Path)):
         measurement_file = pd.read_csv(measurement_file, sep='\t',
                                        float_precision='round_trip')
 
     lint.assert_no_leading_trailing_whitespace(
         measurement_file.columns.values, MEASUREMENT)
 
     return measurement_file
 
 
-def write_measurement_df(df: pd.DataFrame, filename: str) -> None:
+def write_measurement_df(df: pd.DataFrame, filename: Union[str, Path]) -> None:
     """Write PEtab measurement table
 
     Arguments:
         df: PEtab measurement table
         filename: Destination file name
     """
-    with open(filename, 'w') as fh:
-        df.to_csv(fh, sep='\t', index=False)
-
-
-def get_noise_distributions(measurement_df: pd.DataFrame) -> dict:
-    """
-    Returns dictionary of cost definitions per observable, if specified.
-
-    Looks through all parameters satisfying `sbml_parameter_is_cost` and
-    return as dictionary.
-
-    Parameters:
-        measurement_df: PEtab measurement table
-
-    Returns:
-        Dictionary with `observableId` => `cost definition`
-    """
-    warn("This function will be removed in future releases.",
-         DeprecationWarning)
-
-    lint.assert_noise_distributions_valid(measurement_df)
-
-    # read noise distributions from measurement file
-    grouping_cols = core.get_notnull_columns(
-        measurement_df, [OBSERVABLE_ID, OBSERVABLE_TRANSFORMATION,
-                         NOISE_DISTRIBUTION])
-
-    observables = measurement_df.fillna('').groupby(grouping_cols).size()\
-        .reset_index()
-    noise_distrs = {}
-    for _, row in observables.iterrows():
-        # prefix id to get observable id
-        id_ = 'observable_' + row.observableId
-
-        # extract observable transformation and noise distribution,
-        # use lin+normal as default if none provided
-        obs_trafo = row.observableTransformation \
-            if OBSERVABLE_TRANSFORMATION in row \
-            and row.observableTransformation \
-            else LIN
-        noise_distr = row.noiseDistribution \
-            if NOISE_DISTRIBUTION in row \
-            and row.noiseDistribution \
-            else NORMAL
-        # add to noise distributions
-        noise_distrs[id_] = {
-            OBSERVABLE_TRANSFORMATION: obs_trafo,
-            NOISE_DISTRIBUTION: noise_distr}
-
-    return noise_distrs
+    df = get_measurement_df(df)
+    df.to_csv(filename, sep='\t', index=False)
 
 
 def get_simulation_conditions(measurement_df: pd.DataFrame) -> pd.DataFrame:
     """
     Create a table of separate simulation conditions. A simulation condition
     is a specific combination of simulationConditionId and
     preequilibrationConditionId.
@@ -109,14 +72,16 @@
 
     Returns:
         Dataframe with columns 'simulationConditionId' and
         'preequilibrationConditionId'. All-null columns will be omitted.
         Missing 'preequilibrationConditionId's will be set to '' (empty
         string).
     """
+    if measurement_df.empty:
+        return pd.DataFrame(data={SIMULATION_CONDITION_ID: []})
     # find columns to group by (i.e. if not all nans).
     # can be improved by checking for identical condition vectors
     grouping_cols = core.get_notnull_columns(
         measurement_df,
         [SIMULATION_CONDITION_ID, PREEQUILIBRATION_CONDITION_ID])
 
     # group by cols and return dataframe containing each combination
@@ -143,15 +108,15 @@
         condition:
             DataFrame with single row (or Series) and columns
             'preequilibrationConditionId' and 'simulationConditionId'.
             Or dictionary with those keys.
 
     Returns:
         The subselection of rows in ``measurement_df`` for the condition
-    ``condition``.
+        ``condition``.
     """
     # filter rows for condition
     row_filter = 1
     # check for equality in all grouping cols
     if PREEQUILIBRATION_CONDITION_ID in condition:
         row_filter = (measurement_df[PREEQUILIBRATION_CONDITION_ID]
                       .fillna('') ==
@@ -186,61 +151,73 @@
     return core.unique_preserve_order(
         get_unique_parameters(measurement_df[OBSERVABLE_PARAMETERS])
         + get_unique_parameters(measurement_df[NOISE_PARAMETERS]))
 
 
 def split_parameter_replacement_list(
         list_string: Union[str, numbers.Number],
-        delim: str = ';') -> List[Union[str, float]]:
+        delim: str = PARAMETER_SEPARATOR) -> List[Union[str, numbers.Number]]:
     """
     Split values in observableParameters and noiseParameters in measurement
     table.
 
     Arguments:
         list_string: delim-separated stringified list
         delim: delimiter
 
     Returns:
-         List of split values. Numeric values converted to float.
+         List of split values. Numeric values may be converted to `float`,
+         and parameter IDs are kept as strings.
     """
-    if list_string is None:
+    if list_string is None or list_string == '':
         return []
 
     if isinstance(list_string, numbers.Number):
         # Empty cells in pandas might be turned into nan
         # We might want to allow nan as replacement...
         if np.isnan(list_string):
             return []
         return [list_string]
 
-    result = [x.strip() for x in list_string.split(delim) if len(x.strip())]
-    return [core.to_float_if_float(x) for x in result]
+    result = [x.strip() for x in list_string.split(delim)]
+
+    def convert_and_check(x):
+        x = core.to_float_if_float(x)
+        if isinstance(x, float):
+            return x
+        if lint.is_valid_identifier(x):
+            return x
+
+        raise ValueError(
+            f"The value '{x}' in the parameter replacement list "
+            f"'{list_string}' is neither a number, nor a valid parameter ID."
+        )
+
+    return list(map(convert_and_check, result))
 
 
 def create_measurement_df() -> pd.DataFrame:
     """Create empty measurement dataframe
 
     Returns:
         Created DataFrame
     """
 
-    df = pd.DataFrame(data={
+    return pd.DataFrame(data={
         OBSERVABLE_ID: [],
         PREEQUILIBRATION_CONDITION_ID: [],
         SIMULATION_CONDITION_ID: [],
         MEASUREMENT: [],
         TIME: [],
         OBSERVABLE_PARAMETERS: [],
         NOISE_PARAMETERS: [],
         DATASET_ID: [],
         REPLICATE_ID: []
     })
 
-    return df
-
 
 def measurements_have_replicates(measurement_df: pd.DataFrame) -> bool:
     """Tests whether the measurements come with replicates
 
     Arguments:
         measurement_df: Measurement table
 
@@ -253,23 +230,23 @@
          PREEQUILIBRATION_CONDITION_ID, TIME])
     return np.any(
         measurement_df.fillna('').groupby(grouping_cols).size().values - 1)
 
 
 def assert_overrides_match_parameter_count(
         measurement_df: pd.DataFrame,
-        observable_df: pd.DataFrame) -> None:
+        observable_df: pd.DataFrame
+) -> None:
     """Ensure that number of parameters in the observable definition matches
     the number of overrides in ``measurement_df``
 
     Arguments:
         measurement_df: PEtab measurement table
         observable_df: PEtab observable table
     """
-
     # sympify only once and save number of parameters
     observable_parameters_count = {
         obs_id: len(observables.get_formula_placeholders(
             formula, obs_id, 'observable'))
         for obs_id, formula in zip(observable_df.index.values,
                                    observable_df[OBSERVABLE_FORMULA])}
     noise_parameters_count = {
@@ -278,43 +255,57 @@
         for obs_id, formula in zip(observable_df.index.values,
                                    observable_df[NOISE_FORMULA])}
 
     for _, row in measurement_df.iterrows():
         # check observable parameters
         try:
             expected = observable_parameters_count[row[OBSERVABLE_ID]]
-        except KeyError:
+        except KeyError as e:
             raise ValueError(
                 f"Observable {row[OBSERVABLE_ID]} used in measurement table "
-                f"is not defined.")
+                f"is not defined.") from e
+
         actual = len(split_parameter_replacement_list(
             row.get(OBSERVABLE_PARAMETERS, None)))
         # No overrides are also allowed
-        if actual not in [0, expected]:
+        if actual != expected:
             formula = observable_df.loc[row[OBSERVABLE_ID], OBSERVABLE_FORMULA]
             raise AssertionError(
                 f'Mismatch of observable parameter overrides for '
                 f'{row[OBSERVABLE_ID]} ({formula})'
                 f'in:\n{row}\n'
-                f'Expected 0 or {expected} but got {actual}')
+                f'Expected {expected} but got {actual}')
 
         # check noise parameters
         replacements = split_parameter_replacement_list(
             row.get(NOISE_PARAMETERS, None))
         try:
             expected = noise_parameters_count[row[OBSERVABLE_ID]]
 
             # No overrides are also allowed
-            if not (len(replacements) == 0 or len(replacements) == expected):
+            if len(replacements) != expected:
                 raise AssertionError(
                     f'Mismatch of noise parameter overrides in:\n{row}\n'
-                    f'Expected 0 or {expected} but got {actual}')
+                    f'Expected {expected} but got {len(replacements)}')
         except KeyError:
             # no overrides defined, but a numerical sigma can be provided
             # anyways
-            if not len(replacements) == 1 \
+            if len(replacements) != 1 \
                     or not isinstance(replacements[0], numbers.Number):
                 raise AssertionError(
                     f'No placeholders have been specified in the noise model '
                     f'for observable {row[OBSERVABLE_ID]}, but parameter ID '
                     'or multiple overrides were specified in the '
                     'noiseParameters column.')
+
+
+def measurement_is_at_steady_state(time: float) -> bool:
+    """Check whether a measurement is at steady state.
+
+    Arguments:
+        time:
+            The time.
+
+    Returns:
+        Whether the measurement is at steady state.
+    """
+    return math.isinf(time)
```

### Comparing `petab-0.1.8/petab/conditions.py` & `petab-0.2.0/petab/conditions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Functions operating on the PEtab condition table"""
 
-from typing import Iterable, Optional, List, Union
+from pathlib import Path
+from typing import Iterable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-from . import lint, core
+from . import core, lint
 from .C import *
 
+__all__ = ['get_condition_df', 'write_condition_df', 'create_condition_df',
+           'get_parametric_overrides']
+
 
 def get_condition_df(
-        condition_file: Union[str, pd.DataFrame, None]
+        condition_file: Union[str, pd.DataFrame, Path, None]
 ) -> pd.DataFrame:
     """Read the provided condition file into a ``pandas.Dataframe``
 
     Conditions are rows, parameters are columns, conditionId is index.
 
     Arguments:
         condition_file: File name of PEtab condition file or pandas.Dataframe
     """
     if condition_file is None:
         return condition_file
 
-    if isinstance(condition_file, str):
+    if isinstance(condition_file, (str, Path)):
         condition_file = pd.read_csv(condition_file, sep='\t',
                                      float_precision='round_trip')
 
     lint.assert_no_leading_trailing_whitespace(
         condition_file.columns.values, "condition")
 
     if not isinstance(condition_file.index, pd.RangeIndex):
@@ -37,36 +41,36 @@
     except KeyError:
         raise KeyError(
             f'Condition table missing mandatory field {CONDITION_ID}.')
 
     return condition_file
 
 
-def write_condition_df(df: pd.DataFrame, filename: str) -> None:
+def write_condition_df(df: pd.DataFrame, filename: Union[str, Path]) -> None:
     """Write PEtab condition table
 
     Arguments:
         df: PEtab condition table
         filename: Destination file name
     """
-    with open(filename, 'w') as fh:
-        df.to_csv(fh, sep='\t', index=True)
+    df = get_condition_df(df)
+    df.to_csv(filename, sep='\t', index=True)
 
 
 def create_condition_df(parameter_ids: Iterable[str],
                         condition_ids: Optional[Iterable[str]] = None
                         ) -> pd.DataFrame:
     """Create empty condition DataFrame
 
     Arguments:
         parameter_ids: the columns
         condition_ids: the rows
     Returns:
-        A ``pandas.DataFrame`` with empty given rows and columns and all nan
-        values
+        A :py:class:`pandas.DataFrame` with empty given rows and columns and
+        all nan values
     """
 
     condition_ids = [] if condition_ids is None else list(condition_ids)
 
     data = {CONDITION_ID: condition_ids}
     df = pd.DataFrame(data)
 
@@ -85,22 +89,19 @@
 
     Arguments:
         condition_df: PEtab condition table
 
     Returns:
         List of parameter IDs that are mapped in a condition-specific way
     """
-    constant_parameters = list(
-        set(condition_df.columns.values.tolist()) - {CONDITION_ID,
-                                                     CONDITION_NAME})
+    constant_parameters = (set(condition_df.columns.values.tolist())
+                           - {CONDITION_ID, CONDITION_NAME})
     result = []
 
     for column in constant_parameters:
         if np.issubdtype(condition_df[column].dtype, np.number):
             continue
 
         floatified = condition_df.loc[:, column].apply(core.to_float_if_float)
 
-        for x in floatified:
-            if not isinstance(x, float):
-                result.append(x)
+        result.extend(x for x in floatified if not isinstance(x, float))
     return result
```

### Comparing `petab-0.1.8/petab/__init__.py` & `petab-0.2.0/petab/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-"""PEtab global
+"""
+PEtab global
+============
 
 Attributes:
     ENV_NUM_THREADS:
         Name of environment variable to set number of threads or processes
         PEtab should use for operations that can be performed in parallel.
         By default, all operations are performed sequentially.
 """
 
 ENV_NUM_THREADS = "PETAB_NUM_THREADS"
 
+from .C import *  # noqa: F403, F401, E402
 from .calculate import *  # noqa: F403, F401, E402
 from .composite_problem import *  # noqa: F403, F401, E402
 from .conditions import *  # noqa: F403, F401, E402
 from .core import *  # noqa: F403, F401, E402
 from .lint import *  # noqa: F403, F401, E402
 from .measurements import *  # noqa: F403, F401, E402
 from .observables import *  # noqa: F403, F401, E402
 from .parameter_mapping import *  # noqa: F403, F401, E402
 from .parameters import *  # noqa: F403, F401, E402
 from .problem import *  # noqa: F403, F401, E402
 from .sampling import *  # noqa: F403, F401, E402
 from .sbml import *  # noqa: F403, F401, E402
+from .simulate import *  # noqa: F403, F401, E402
 from .yaml import *  # noqa: F403, F401, E402
 from .version import __version__  # noqa: F401, E402
 from .format_version import __format_version__  # noqa: F401, E402
+from .mapping import *  # noqa: F403, F401, E402
```

### Comparing `petab-0.1.8/petab/petablint.py` & `petab-0.2.0/petab/petablint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 """Command line tool to check for correct format"""
 
 import argparse
 import logging
-import os
 import sys
 
 import petab
 from colorama import (init as init_colorama, Fore)
 
 logger = logging.getLogger(__name__)
 
@@ -29,15 +28,14 @@
         result = logging.Formatter.format(self, record)
         self._style._fmt = format_orig
         return result
 
 
 def parse_cli_args():
     """Parse command line arguments"""
-
     parser = argparse.ArgumentParser(
         description='Check if a set of files adheres to the PEtab format.')
 
     # General options:
     parser.add_argument('-v', '--verbose', dest='verbose', action='store_true',
                         help='More verbose output')
 
@@ -48,64 +46,30 @@
                         help='Observable table')
     parser.add_argument('-m', '--measurements', dest='measurement_file_name',
                         help='Measurement table')
     parser.add_argument('-c', '--conditions', dest='condition_file_name',
                         help='Conditions table')
     parser.add_argument('-p', '--parameters', dest='parameter_file_name',
                         help='Parameter table')
+    parser.add_argument('--vis', '--visualizations',
+                        dest='visualization_file_name',
+                        help='Visualization table')
 
     group = parser.add_mutually_exclusive_group()
     group.add_argument('-y', '--yaml', dest='yaml_file_name',
                        help='PEtab YAML problem filename')
 
-    # or with model name, following default naming
-    group.add_argument('-n', '--model-name', dest='model_name',
-                       help='Model name where all files are in the working '
-                            'directory and follow PEtab naming convention. '
-                            'Specifying -[smcp] will override defaults')
-    parser.add_argument('-d', '--directory', dest='directory',
-                        default=os.getcwd())
     args = parser.parse_args()
 
-    if args.model_name:
-        if not args.sbml_file_name:
-            args.sbml_file_name = petab.get_default_sbml_file_name(
-                args.model_name,
-                folder=args.directory,
-            )
-        if not args.measurement_file_name:
-            args.measurement_file_name = \
-                petab.get_default_measurement_file_name(
-                    args.model_name,
-                    folder=args.directory,
-                )
-        if not args.condition_file_name:
-            args.condition_file_name = petab.get_default_condition_file_name(
-                args.model_name,
-                folder=args.directory,
-            )
-        if not args.parameter_file_name:
-            args.parameter_file_name = petab.get_default_parameter_file_name(
-                args.model_name,
-                folder=args.directory,
-            )
-
     if (args.yaml_file_name
             and any((args.sbml_file_name, args.condition_file_name,
                      args.measurement_file_name, args.parameter_file_name))):
         parser.error('When providing a yaml file, no other files may '
                      'be specified.')
 
-    if (not args.model_name
-            and not any([args.sbml_file_name, args.condition_file_name,
-                         args.measurement_file_name, args.parameter_file_name,
-                         args.observable_file_name, args.yaml_file_name])):
-        parser.error('Neither model name nor any filename specified. '
-                     'What shall I do?')
-
     return args
 
 
 def main():
     """Run PEtab validator"""
     args = parse_cli_args()
     init_colorama(autoreset=True)
@@ -144,22 +108,26 @@
             logger.debug(f'\tCondition table: {args.condition_file_name}')
         if args.observable_file_name:
             logger.debug(f'\tObservable table: {args.observable_file_name}')
         if args.measurement_file_name:
             logger.debug(f'\tMeasurement table: {args.measurement_file_name}')
         if args.parameter_file_name:
             logger.debug(f'\tParameter table: {args.parameter_file_name}')
+        if args.visualization_file_name:
+            logger.debug('\tVisualization table: '
+                         f'{args.visualization_file_name}')
 
         try:
             problem = petab.Problem.from_files(
                 sbml_file=args.sbml_file_name,
                 condition_file=args.condition_file_name,
                 measurement_file=args.measurement_file_name,
                 parameter_file=args.parameter_file_name,
-                observable_files=args.observable_file_name
+                observable_files=args.observable_file_name,
+                visualization_files=args.visualization_file_name,
             )
         except FileNotFoundError as e:
             logger.error(e)
             sys.exit(1)
 
     ret = petab.lint.lint_problem(problem)
     sys.exit(ret)
```

### Comparing `petab-0.1.8/petab/parameter_mapping.py` & `petab-0.2.0/petab/parameter_mapping.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 """Functions related to mapping parameter from model to parameter estimation
 problem"""
 
 import logging
 import numbers
 import os
 import re
-from typing import Tuple, Dict, Union, Any, List, Optional, Iterable
+import warnings
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, Literal
 
 import libsbml
 import numpy as np
 import pandas as pd
 
-from . import lint, measurements, sbml, core, observables, parameters
-from . import ENV_NUM_THREADS
+from . import ENV_NUM_THREADS, core, lint, measurements, observables, \
+    parameters
 from .C import *  # noqa: F403
-
+from .models import Model
+from .mapping import resolve_mapping
 
 logger = logging.getLogger(__name__)
+__all__ = ['get_optimization_to_simulation_parameter_mapping',
+           'get_parameter_mapping_for_condition',
+           'handle_missing_overrides',
+           'merge_preeq_and_sim_pars',
+           'merge_preeq_and_sim_pars_condition',
+           'ParMappingDict', 'ParMappingDictTuple',
+           'ScaleMappingDict', 'ScaleMappingDictTuple',
+           'ParMappingDictQuadruple']
+
 
 # Parameter mapping for condition
 ParMappingDict = Dict[str, Union[str, numbers.Number]]
 # Parameter mapping for combination of preequilibration and simulation
 # condition
 ParMappingDictTuple = Tuple[ParMappingDict, ParMappingDict]
 # Same for scale mapping
@@ -33,230 +44,318 @@
 
 
 def get_optimization_to_simulation_parameter_mapping(
         condition_df: pd.DataFrame,
         measurement_df: pd.DataFrame,
         parameter_df: Optional[pd.DataFrame] = None,
         observable_df: Optional[pd.DataFrame] = None,
+        mapping_df: Optional[pd.DataFrame] = None,
         sbml_model: libsbml.Model = None,
         simulation_conditions: Optional[pd.DataFrame] = None,
         warn_unmapped: Optional[bool] = True,
         scaled_parameters: bool = False,
         fill_fixed_parameters: bool = True,
+        allow_timepoint_specific_numeric_noise_parameters: bool = False,
+        model: Model = None,
 ) -> List[ParMappingDictQuadruple]:
     """
-    Create list of mapping dicts from PEtab-problem to SBML parameters.
+    Create list of mapping dicts from PEtab-problem to model parameters.
 
     Mapping can be performed in parallel. The number of threads is controlled
-    by the environment variable with the name of petab.ENV_NUM_THREADS.
+    by the environment variable with the name of
+    :py:data:`petab.ENV_NUM_THREADS`.
 
     Parameters:
         condition_df, measurement_df, parameter_df, observable_df:
             The dataframes in the PEtab format.
         sbml_model:
-            The sbml model with observables and noise specified according to
-            the PEtab format.
+            The SBML model (deprecated)
+        model:
+            The model.
         simulation_conditions:
             Table of simulation conditions as created by
             ``petab.get_simulation_conditions``.
         warn_unmapped:
             If ``True``, log warning regarding unmapped parameters
         scaled_parameters:
             Whether parameter values should be scaled.
         fill_fixed_parameters:
             Whether to fill in nominal values for fixed parameters
             (estimate=0 in parameters table).
+        allow_timepoint_specific_numeric_noise_parameters:
+            Mapping of timepoint-specific parameters overrides is generally
+            not supported. If this option is set to True, this function will
+            not fail in case of timepoint-specific fixed noise parameters,
+            if the noise formula consists only of one single parameter.
+            It is expected that the respective mapping is performed elsewhere.
+            The value mapped to the respective parameter here is undefined.
 
     Returns:
         Parameter value and parameter scale mapping for all conditions.
 
         The length of the returned array is the number of unique combinations
-        of ``simulationConditionId``s and ``preequilibrationConditionId``s from
-        the measurement table. Each entry is a tuple of four dicts of length
-        equal to the number of model parameters.
+        of ``simulationConditionId`` s and ``preequilibrationConditionId`` s
+        from the measurement table. Each entry is a tuple of four dicts of
+        length equal to the number of model parameters.
         The first two dicts map simulation parameter IDs to optimization
         parameter IDs or values (where values are fixed) for preequilibration
         and simulation condition, respectively.
         The last two dicts map simulation parameter IDs to the parameter scale
         of the respective parameter, again for preequilibration and simulation
         condition.
         If no preequilibration condition is defined, the respective dicts will
         be empty. ``NaN`` is used where no mapping exists.
     """
+    if sbml_model:
+        warnings.warn("Passing a model via the `sbml_model` argument is "
+                      "deprecated, use `model=petab.models.sbml_model."
+                      "SbmlModel(...)` instead.", DeprecationWarning,
+                      stacklevel=2)
+        from petab.models.sbml_model import SbmlModel
+        if model:
+            raise ValueError("Arguments `model` and `sbml_model` are "
+                             "mutually exclusive.")
+        model = SbmlModel(sbml_model=sbml_model)
 
     # Ensure inputs are okay
-    _perform_mapping_checks(measurement_df)
+    _perform_mapping_checks(
+        measurement_df,
+        allow_timepoint_specific_numeric_noise_parameters=  # noqa: E251,E501
+        allow_timepoint_specific_numeric_noise_parameters)
 
     if simulation_conditions is None:
         simulation_conditions = measurements.get_simulation_conditions(
             measurement_df)
 
-    simulation_parameters = sbml.get_model_parameters(sbml_model,
-                                                      with_values=True)
-    # Add output parameters that are not already defined in the SBML model
+    simulation_parameters = dict(model.get_free_parameter_ids_with_values())
+    # Add output parameters that are not already defined in the model
     if observable_df is not None:
         output_parameters = observables.get_output_parameters(
-            observable_df=observable_df, sbml_model=sbml_model)
+            observable_df=observable_df, model=model, mapping_df=mapping_df
+        )
         for par_id in output_parameters:
             simulation_parameters[par_id] = np.nan
 
     num_threads = int(os.environ.get(ENV_NUM_THREADS, 1))
 
     # If sequential execution is requested, let's not create any
     # thread-allocation overhead
     if num_threads == 1:
         mapping = map(
             _map_condition,
             _map_condition_arg_packer(
                 simulation_conditions, measurement_df, condition_df,
-                parameter_df, sbml_model, simulation_parameters, warn_unmapped,
-                scaled_parameters, fill_fixed_parameters))
+                parameter_df, mapping_df,
+                model, simulation_parameters, warn_unmapped, scaled_parameters,
+                fill_fixed_parameters,
+                allow_timepoint_specific_numeric_noise_parameters))
         return list(mapping)
 
     # Run multi-threaded
     from concurrent.futures import ThreadPoolExecutor
     with ThreadPoolExecutor(max_workers=num_threads) as executor:
         mapping = executor.map(
             _map_condition,
             _map_condition_arg_packer(
                 simulation_conditions, measurement_df, condition_df,
-                parameter_df, sbml_model, simulation_parameters, warn_unmapped,
-                scaled_parameters, fill_fixed_parameters))
+                parameter_df, mapping_df, model, simulation_parameters,
+                warn_unmapped, scaled_parameters, fill_fixed_parameters,
+                allow_timepoint_specific_numeric_noise_parameters))
     return list(mapping)
 
 
-def _map_condition_arg_packer(simulation_conditions, measurement_df,
-                              condition_df, parameter_df, sbml_model,
-                              simulation_parameters, warn_unmapped,
-                              scaled_parameters, fill_fixed_parameters):
+def _map_condition_arg_packer(
+        simulation_conditions,
+        measurement_df,
+        condition_df,
+        parameter_df,
+        mapping_df,
+        model,
+        simulation_parameters,
+        warn_unmapped,
+        scaled_parameters,
+        fill_fixed_parameters,
+        allow_timepoint_specific_numeric_noise_parameters
+):
     """Helper function to pack extra arguments for _map_condition"""
     for _, condition in simulation_conditions.iterrows():
-        yield(condition, measurement_df, condition_df, parameter_df,
-              sbml_model, simulation_parameters, warn_unmapped,
-              scaled_parameters, fill_fixed_parameters)
+        yield (
+            condition, measurement_df, condition_df, parameter_df, mapping_df,
+            model, simulation_parameters, warn_unmapped, scaled_parameters,
+            fill_fixed_parameters,
+            allow_timepoint_specific_numeric_noise_parameters
+        )
 
 
 def _map_condition(packed_args):
     """Helper function for parallel condition mapping.
 
-    For arguments see get_optimization_to_simulation_parameter_mapping"""
+    For arguments see
+    :py:func:`get_optimization_to_simulation_parameter_mapping`.
+    """
 
-    (condition, measurement_df, condition_df, parameter_df, sbml_model,
+    (condition, measurement_df, condition_df, parameter_df, mapping_df, model,
      simulation_parameters, warn_unmapped, scaled_parameters,
-     fill_fixed_parameters) = packed_args
+     fill_fixed_parameters,
+     allow_timepoint_specific_numeric_noise_parameters) = packed_args
 
-    cur_measurement_df = measurements.get_rows_for_condition(
-        measurement_df, condition)
+    cur_measurement_df = None
+    # Get the condition specific measurements for the current condition, but
+    # only if relevant for parameter mapping
+    if (OBSERVABLE_PARAMETERS in measurement_df
+        and measurement_df[OBSERVABLE_PARAMETERS].notna().any()) \
+        or (NOISE_PARAMETERS in measurement_df
+            and measurement_df[NOISE_PARAMETERS].notna().any()):
+        cur_measurement_df = measurements.get_rows_for_condition(
+            measurement_df, condition)
 
     if PREEQUILIBRATION_CONDITION_ID not in condition \
             or not isinstance(condition[PREEQUILIBRATION_CONDITION_ID], str) \
             or not condition[PREEQUILIBRATION_CONDITION_ID]:
         par_map_preeq = {}
         scale_map_preeq = {}
     else:
         par_map_preeq, scale_map_preeq = get_parameter_mapping_for_condition(
             condition_id=condition[PREEQUILIBRATION_CONDITION_ID],
             is_preeq=True,
             cur_measurement_df=cur_measurement_df,
-            sbml_model=sbml_model,
+            model=model,
             condition_df=condition_df,
             parameter_df=parameter_df,
+            mapping_df=mapping_df,
             simulation_parameters=simulation_parameters,
             warn_unmapped=warn_unmapped,
             scaled_parameters=scaled_parameters,
             fill_fixed_parameters=fill_fixed_parameters,
+            allow_timepoint_specific_numeric_noise_parameters=  # noqa: E251,E501
+            allow_timepoint_specific_numeric_noise_parameters
         )
 
     par_map_sim, scale_map_sim = get_parameter_mapping_for_condition(
         condition_id=condition[SIMULATION_CONDITION_ID],
         is_preeq=False,
         cur_measurement_df=cur_measurement_df,
-        sbml_model=sbml_model,
+        model=model,
         condition_df=condition_df,
         parameter_df=parameter_df,
+        mapping_df=mapping_df,
         simulation_parameters=simulation_parameters,
         warn_unmapped=warn_unmapped,
         scaled_parameters=scaled_parameters,
         fill_fixed_parameters=fill_fixed_parameters,
+        allow_timepoint_specific_numeric_noise_parameters=  # noqa: E251,E501
+        allow_timepoint_specific_numeric_noise_parameters
     )
 
     return par_map_preeq, par_map_sim, scale_map_preeq, scale_map_sim
 
 
 def get_parameter_mapping_for_condition(
         condition_id: str,
         is_preeq: bool,
-        cur_measurement_df: pd.DataFrame,
-        sbml_model: libsbml.Model,
-        condition_df: pd.DataFrame,
+        cur_measurement_df: Optional[pd.DataFrame],
+        sbml_model: libsbml.Model = None,
+        condition_df: pd.DataFrame = None,
         parameter_df: pd.DataFrame = None,
+        mapping_df: Optional[pd.DataFrame] = None,
         simulation_parameters: Optional[Dict[str, str]] = None,
         warn_unmapped: bool = True,
         scaled_parameters: bool = False,
         fill_fixed_parameters: bool = True,
+        allow_timepoint_specific_numeric_noise_parameters: bool = False,
+        model: Model = None,
 ) -> Tuple[ParMappingDict, ScaleMappingDict]:
     """
     Create dictionary of parameter value and parameter scale mappings from
     PEtab-problem to SBML parameters for the given condition.
 
     Parameters:
         condition_id:
             Condition ID for which to perform mapping
         is_preeq:
             If ``True``, output parameters will not be mapped
         cur_measurement_df:
-            Measurement sub-table for current condition
+            Measurement sub-table for current condition, can be ``None`` if
+            not relevant for parameter mapping
         condition_df:
             PEtab condition DataFrame
         parameter_df:
             PEtab parameter DataFrame
+        mapping_df:
+            PEtab mapping DataFrame
         sbml_model:
-            The sbml model with observables and noise specified according to
-            the PEtab format used to retrieve simulation parameter IDs.
+            The SBML model (deprecated)
+        model:
+            The model.
         simulation_parameters:
             Model simulation parameter IDs mapped to parameter values (output
             of ``petab.sbml.get_model_parameters(.., with_values=True)``).
             Optional, saves time if precomputed.
         warn_unmapped:
             If ``True``, log warning regarding unmapped parameters
+        scaled_parameters:
+            Whether parameter values should be scaled.
         fill_fixed_parameters:
             Whether to fill in nominal values for fixed parameters
             (estimate=0 in parameters table).
+        allow_timepoint_specific_numeric_noise_parameters:
+            Mapping of timepoint-specific parameters overrides is generally
+            not supported. If this option is set to True, this function will
+            not fail in case of timepoint-specific fixed noise parameters,
+            if the noise formula consists only of one single parameter.
+            It is expected that the respective mapping is performed elsewhere.
+            The value mapped to the respective parameter here is undefined.
 
     Returns:
         Tuple of two dictionaries. First dictionary mapping model parameter IDs
         to mapped parameters IDs to be estimated or to filled-in values in case
         of non-estimated parameters.
         Second dictionary mapping model parameter IDs to their scale.
-        NaN is used where no mapping exists.
+        ``NaN`` is used where no mapping exists.
     """
-    _perform_mapping_checks(cur_measurement_df)
+    if sbml_model:
+        warnings.warn("Passing a model via the `sbml_model` argument is "
+                      "deprecated, use `model=petab.models.sbml_model."
+                      "SbmlModel(...)` instead.", DeprecationWarning,
+                      stacklevel=2)
+        from petab.models.sbml_model import SbmlModel
+        if model:
+            raise ValueError("Arguments `model` and `sbml_model` are "
+                             "mutually exclusive.")
+        model = SbmlModel(sbml_model=sbml_model)
+
+    if cur_measurement_df is not None:
+        _perform_mapping_checks(
+            cur_measurement_df,
+            allow_timepoint_specific_numeric_noise_parameters=  # noqa: E251,E501
+            allow_timepoint_specific_numeric_noise_parameters)
 
     if simulation_parameters is None:
-        simulation_parameters = sbml.get_model_parameters(sbml_model,
-                                                          with_values=True)
+        simulation_parameters = dict(
+            model.get_free_parameter_ids_with_values())
 
     # NOTE: order matters here - the former is overwritten by the latter:
-    #  SBML model < condition table < measurement < table parameter table
+    #  model < condition table < measurement < table parameter table
 
     # initialize mapping dicts
     # for the case of matching simulation and optimization parameter vector
     par_mapping = simulation_parameters.copy()
     scale_mapping = {par_id: LIN for par_id in par_mapping.keys()}
     _output_parameters_to_nan(par_mapping)
 
     # not strictly necessary for preequilibration, be we do it to have
     # same length of parameter vectors
-    _apply_output_parameter_overrides(par_mapping, cur_measurement_df)
+    if cur_measurement_df is not None:
+        _apply_output_parameter_overrides(par_mapping, cur_measurement_df)
 
     if not is_preeq:
         handle_missing_overrides(par_mapping, warn=warn_unmapped)
 
     _apply_condition_parameters(par_mapping, scale_mapping, condition_id,
-                                condition_df, sbml_model)
+                                condition_df, model, mapping_df)
     _apply_parameter_table(par_mapping, scale_mapping,
                            parameter_df, scaled_parameters,
                            fill_fixed_parameters)
 
     return par_mapping, scale_mapping
 
 
@@ -271,23 +370,24 @@
 
         if matches:
             mapping[key] = np.nan
 
 
 def _apply_output_parameter_overrides(
         mapping: ParMappingDict,
-        cur_measurement_df: pd.DataFrame) -> None:
+        cur_measurement_df: pd.DataFrame
+) -> None:
     """
     Apply output parameter overrides to the parameter mapping dict for a given
     condition as defined in the measurement table (``observableParameter``,
     ``noiseParameters``).
 
     Arguments:
         mapping: parameter mapping dict as obtained from
-            ``get_parameter_mapping_for_condition``
+            :py:func:`get_parameter_mapping_for_condition`.
         cur_measurement_df:
             Subset of the measurement table for the current condition
     """
     for _, row in cur_measurement_df.iterrows():
         # we trust that the number of overrides matches (see above)
         overrides = measurements.split_parameter_replacement_list(
             row.get(OBSERVABLE_PARAMETERS, None))
@@ -299,82 +399,95 @@
         _apply_overrides_for_observable(mapping, row[OBSERVABLE_ID], 'noise',
                                         overrides)
 
 
 def _apply_overrides_for_observable(
         mapping: ParMappingDict,
         observable_id: str,
-        override_type: str,
-        overrides: List[str]) -> None:
+        override_type: Literal['observable', 'noise'],
+        overrides: List[str],
+) -> None:
     """
     Apply parameter-overrides for observables and noises to mapping
     matrix.
 
     Arguments:
         mapping: mapping dict to which to apply overrides
         observable_id: observable ID
-        override_type: 'observable' or 'noise'
+        override_type: ``'observable'`` or ``'noise'``
         overrides: list of overrides for noise or observable parameters
     """
     for i, override in enumerate(overrides):
         overridee_id = f'{override_type}Parameter{i+1}_{observable_id}'
-        try:
-            mapping[overridee_id] = override
-        except KeyError as e:
-            raise TypeError(f'Cannot override {override_type} parameter '
-                            f'{overridee_id} for observable {observable_id}.'
-                            f'Ensure there exists an {override_type} '
-                            'definition containing the correct number of '
-                            'placeholder parameters.') from e
+        mapping[overridee_id] = override
 
 
-def _apply_condition_parameters(par_mapping: ParMappingDict,
-                                scale_mapping: ScaleMappingDict,
-                                condition_id: str,
-                                condition_df: pd.DataFrame,
-                                sbml_model: libsbml.Model) -> None:
+def _apply_condition_parameters(
+        par_mapping: ParMappingDict,
+        scale_mapping: ScaleMappingDict,
+        condition_id: str,
+        condition_df: pd.DataFrame,
+        model: Model,
+        mapping_df: Optional[pd.DataFrame] = None,
+) -> None:
     """Replace parameter IDs in parameter mapping dictionary by condition
     table parameter values (in-place).
 
     Arguments:
-        par_mapping: see get_parameter_mapping_for_condition
+        par_mapping: see :py:func:`get_parameter_mapping_for_condition`
         condition_id: ID of condition to work on
         condition_df: PEtab condition table
     """
     for overridee_id in condition_df.columns:
         if overridee_id == CONDITION_NAME:
             continue
 
-        # Species and compartments are handled elsewhere
-        if sbml_model.getSpecies(overridee_id) is not None:
-            continue
-        if sbml_model.getCompartment(overridee_id) is not None:
+        overridee_id = resolve_mapping(mapping_df, overridee_id)
+
+        # Species, compartments, and rule targets are handled elsewhere
+        if model.is_state_variable(overridee_id):
             continue
 
         par_mapping[overridee_id] = core.to_float_if_float(
             condition_df.loc[condition_id, overridee_id])
+
+        if isinstance(par_mapping[overridee_id], numbers.Number) \
+                and np.isnan(par_mapping[overridee_id]):
+            # NaN in the condition table for an entity without time derivative
+            #  indicates that the model value should be used
+            try:
+                par_mapping[overridee_id] = \
+                    model.get_parameter_value(overridee_id)
+            except ValueError as e:
+                raise NotImplementedError(
+                    "Not sure how to handle NaN in condition table for "
+                    f"{overridee_id}."
+                ) from e
+
         scale_mapping[overridee_id] = LIN
 
 
-def _apply_parameter_table(par_mapping: ParMappingDict,
-                           scale_mapping: ScaleMappingDict,
-                           parameter_df: Optional[pd.DataFrame] = None,
-                           scaled_parameters: bool = False,
-                           fill_fixed_parameters: bool = True,
-                           ) -> None:
+def _apply_parameter_table(
+        par_mapping: ParMappingDict,
+        scale_mapping: ScaleMappingDict,
+        parameter_df: Optional[pd.DataFrame] = None,
+        scaled_parameters: bool = False,
+        fill_fixed_parameters: bool = True,
+) -> None:
     """Replace parameters from parameter table in mapping list for a given
     condition and set the corresponding scale.
 
     Replace non-estimated parameters by ``nominalValues``
     (un-scaled / lin-scaled), replace estimated parameters by the respective
     ID.
 
     Arguments:
         par_mapping:
-            mapping dict obtained from ``get_parameter_mapping_for_condition``
+            mapping dict obtained from
+            :py:func:`get_parameter_mapping_for_condition`
         parameter_df:
             PEtab parameter table
     """
 
     if parameter_df is None:
         return
 
@@ -422,38 +535,46 @@
                 else:
                     scale = LIN
                 par_mapping[problem_par] = val
 
             scale_mapping[problem_par] = scale
 
 
-def _perform_mapping_checks(measurement_df: pd.DataFrame) -> None:
+def _perform_mapping_checks(
+        measurement_df: pd.DataFrame,
+        allow_timepoint_specific_numeric_noise_parameters: bool = False
+) -> None:
     """Check for PEtab features which we can't account for during parameter
     mapping."""
 
-    if lint.measurement_table_has_timepoint_specific_mappings(measurement_df):
+    if lint.measurement_table_has_timepoint_specific_mappings(
+            measurement_df,
+            allow_scalar_numeric_noise_parameters=  # noqa: E251,E501
+            allow_timepoint_specific_numeric_noise_parameters):
         # we could allow that for floats, since they don't matter in this
         # function and would be simply ignored
         raise ValueError(
             "Timepoint-specific parameter overrides currently unsupported.")
 
 
-def handle_missing_overrides(mapping_par_opt_to_par_sim: ParMappingDict,
-                             warn: bool = True,
-                             condition_id: str = None) -> None:
+def handle_missing_overrides(
+        mapping_par_opt_to_par_sim: ParMappingDict,
+        warn: bool = True,
+        condition_id: str = None,
+) -> None:
     """
     Find all observable parameters and noise parameters that were not mapped
     and set their mapping to np.nan.
 
-    Assumes that parameters matching "(noise|observable)Parameter[0-9]+_" were
-    all supposed to be overwritten.
+    Assumes that parameters matching the regular expression
+    ``(noise|observable)Parameter[0-9]+_`` were all supposed to be overwritten.
 
     Parameters:
         mapping_par_opt_to_par_sim:
-            Output of get_parameter_mapping_for_condition
+            Output of :py:func:`get_parameter_mapping_for_condition`
         warn:
             If True, log warning regarding unmapped parameters
         condition_id:
             Optional condition ID for more informative output
     """
     _missed_vals = []
     rex = re.compile("^(noise|observable)Parameter[0-9]+_")
@@ -475,31 +596,32 @@
 
 
 def merge_preeq_and_sim_pars_condition(
         condition_map_preeq: ParMappingDict,
         condition_map_sim: ParMappingDict,
         condition_scale_map_preeq: ScaleMappingDict,
         condition_scale_map_sim: ScaleMappingDict,
-        condition: Any) -> None:
+        condition: Any,
+) -> None:
     """Merge preequilibration and simulation parameters and scales for a single
     condition while checking for compatibility.
 
     This function is meant for the case where we cannot have different
     parameters (and scales) for preequilibration and simulation. Therefore,
     merge both and ensure matching scales and parameters.
-    ``condition_map_sim`` and ``condition_scale_map_sim`` will ne modified in
+    ``condition_map_sim`` and ``condition_scale_map_sim`` will be modified in
     place.
 
     Arguments:
         condition_map_preeq, condition_map_sim:
             Parameter mapping as obtained from
-            `get_parameter_mapping_for_condition`
+            :py:func:`get_parameter_mapping_for_condition`
         condition_scale_map_preeq, condition_scale_map_sim:
             Parameter scale mapping as obtained from
-            `get_get_scale_mapping_for_condition`
+            :py:func:`get_parameter_mapping_for_condition`
         condition: Condition identifier for more informative error messages
     """
     if not condition_map_preeq:
         # nothing to do
         return
 
     all_par_ids = set(condition_map_sim.keys()) \
@@ -560,17 +682,18 @@
 ) -> Tuple[List[ParMappingDictTuple], List[ScaleMappingDictTuple]]:
     """Merge preequilibration and simulation parameters and scales for a list
     of conditions while checking for compatibility.
 
     Parameters:
         parameter_mappings:
             As returned by
-            petab.get_optimization_to_simulation_parameter_mapping
+            :py:func:`petab.get_optimization_to_simulation_parameter_mapping`.
         scale_mappings:
-            As returned by petab.get_optimization_to_simulation_scale_mapping.
+            As returned by
+            :py:func:`petab.get_optimization_to_simulation_parameter_mapping`.
 
     Returns:
         The parameter and scale simulation mappings, modified and checked.
     """
     parameter_mapping = []
     scale_mapping = []
     for ic, ((map_preeq, map_sim), (scale_map_preeq, scale_map_sim)) in \
```

### Comparing `petab-0.1.8/petab/petab_schema.yaml` & `petab-0.2.0/petab/schemas/petab_schema.v1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `petab-0.1.8/setup.py` & `petab-0.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,106 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 import sys
 import os
 import re
 
 
 def read(fname):
     """Read a file."""
     return open(fname).read()
 
 
 def absolute_links(txt):
     """Replace relative petab github links by absolute links."""
-    raw_base = "(https://raw.githubusercontent.com/petab-dev/petab/master/"
-    embedded_base = "(https://github.com/petab-dev/petab/tree/master/"
+
+    raw_base = \
+        "(https://raw.githubusercontent.com/petab-dev/libpetab-python/master/"
+    embedded_base = \
+        "(https://github.com/petab-dev/libpetab-python/tree/master/"
     # iterate over links
-    for var in re.findall(r'\[.*?\]\((?!http).*?\)', txt):
-        if re.match(r'.*?.(png|svg)\)', var):
+    for var in re.findall(r"\[.*?\]\((?!http).*?\)", txt):
+        if re.match(r".*?.(png|svg)\)", var):
             # link to raw file
             rep = var.replace("(", raw_base)
         else:
             # link to github embedded file
             rep = var.replace("(", embedded_base)
         txt = txt.replace(var, rep)
     return txt
 
 
-# Python version check. We need >= 3.6 due to e.g. f-strings
-if sys.version_info < (3, 6):
-    sys.exit('PEtab requires at least Python version 3.6')
+# Python version check
+if sys.version_info < (3, 9, 0):
+    sys.exit("PEtab requires at least Python version 3.9")
 
 # read version from file
-version_file = os.path.join('petab', 'version.py')
+__version__ = ""
+version_file = os.path.join("petab", "version.py")
+# sets __version__
 exec(read(version_file))  # pylint: disable=W0122 # nosec
 
 ENTRY_POINTS = {
-    'console_scripts': [
-        'petablint = petab.petablint:main',
+    "console_scripts": [
+        "petablint = petab.petablint:main",
+        "petab_visualize = petab.visualize.cli:_petab_visualize_main",
     ]
 }
 
 # project metadata
 # noinspection PyUnresolvedReferences
-setup(name='petab',
-      version=__version__,  # noqa: F821
-      description='Parameter estimation tabular data',
-      long_description=absolute_links(read('README.md')),
-      long_description_content_type="text/markdown",
-      author='The PEtab developers',
-      author_email='daniel.weindl@helmholtz-muenchen.de',
-      url='https://github.com/PEtab-dev/PEtab',
-      packages=find_packages(exclude=['doc*', 'test*']),
-      install_requires=['numpy>=1.15.1',
-                        'pandas>=1.0.1',
-                        'matplotlib>=2.2.3',
-                        'python-libsbml>=5.17.0',
-                        'sympy',
-                        'colorama',
-                        'seaborn',
-                        'pyyaml',
-                        'jsonschema',
-                        ],
-      include_package_data=True,
-      tests_require=['flake8', 'pytest', 'python-libcombine'],
-      python_requires='>=3.6',
-      entry_points=ENTRY_POINTS,
-      extras_require={'reports': ['Jinja2'],
-                      'combine': ['python-libcombine>=0.2.6']},
-      )
+setup(
+    name="petab",
+    version=__version__,
+    description="Parameter estimation tabular data",
+    long_description=absolute_links(read("README.md")),
+    long_description_content_type="text/markdown",
+    author="The PEtab developers",
+    author_email="daniel.weindl@helmholtz-muenchen.de",
+    url="https://github.com/PEtab-dev/libpetab-python",
+    packages=find_namespace_packages(exclude=["doc*", "test*"]),
+    install_requires=[
+        "numpy>=1.15.1",
+        "pandas>=1.2.0",
+        "python-libsbml>=5.17.0",
+        "sympy",
+        "colorama",
+        "pyyaml",
+        "jsonschema",
+    ],
+    include_package_data=True,
+    python_requires=">=3.9.0",
+    entry_points=ENTRY_POINTS,
+    extras_require={
+        "tests": [
+            "pytest",
+            "pytest-cov",
+            "simplesbml",
+            "scipy",
+            "pysb",
+        ],
+        "quality": [
+            "flake8>=3.8.3",
+        ],
+        "reports": [
+            # https://github.com/spatialaudio/nbsphinx/issues/641
+            "Jinja2==3.0.3",
+        ],
+        "combine": [
+            "python-libcombine>=0.2.6",
+        ],
+        "doc": [
+            "sphinx>=3.5.3, !=5.1.0",
+            "sphinxcontrib-napoleon>=0.7",
+            "sphinx-markdown-tables>=0.0.15",
+            "sphinx-rtd-theme>=0.5.1",
+            "m2r2",
+            "myst-nb>=0.14.0",
+            # https://github.com/spatialaudio/nbsphinx/issues/687#issuecomment-1339271312
+            "ipython>=7.21.0, !=8.7.0",
+        ],
+        "vis": [
+            "matplotlib>=3.6.0",
+            "seaborn",
+            "scipy"
+        ]
+    },
+)
```


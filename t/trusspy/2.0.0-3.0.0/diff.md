# Comparing `tmp/trusspy-2.0.0.tar.gz` & `tmp/trusspy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trusspy-2.0.0.tar", last modified: Wed May  3 21:47:15 2023, max compression
+gzip compressed data, was "trusspy-3.0.0.tar", last modified: Mon May  8 17:49:35 2023, max compression
```

## Comparing `trusspy-2.0.0.tar` & `trusspy-3.0.0.tar`

### file list

```diff
@@ -1,63 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.733802 trusspy-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    33206 2023-05-03 21:47:06.000000 trusspy-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43830 2023-05-03 21:47:15.733802 trusspy-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-03 21:47:06.000000 trusspy-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 21:47:06.000000 trusspy-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:47:15.733802 trusspy-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.725802 trusspy-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.725802 trusspy-2.0.0/src/trusspy/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.729802 trusspy-2.0.0/src/trusspy/core/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/core/boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/core/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/core/external_force.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/core/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.729802 trusspy-2.0.0/src/trusspy/elements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/elements/element_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.729802 trusspy-2.0.0/src/trusspy/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/handlers/handler_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/handlers/handler_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/handlers/handler_extforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/handlers/handler_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/handlers/handler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/handlers/handler_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.729802 trusspy-2.0.0/src/trusspy/materials/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/materials/material_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    24697 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.729802 trusspy-2.0.0/src/trusspy/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/solvers/tpsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/solvers/zerosearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.729802 trusspy-2.0.0/src/trusspy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/tools/helper_functions2.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/tools/movie_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-03 21:47:06.000000 trusspy-2.0.0/src/trusspy/tools/plot_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.729802 trusspy-2.0.0/src/trusspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43830 2023-05-03 21:47:15.000000 trusspy-2.0.0/src/trusspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-03 21:47:15.000000 trusspy-2.0.0/src/trusspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:47:15.000000 trusspy-2.0.0/src/trusspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 21:47:15.000000 trusspy-2.0.0/src/trusspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 21:47:15.000000 trusspy-2.0.0/src/trusspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:47:15.733802 trusspy-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e101_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e102_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e102_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e103_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e10x_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e10xx_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e201_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e202_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_e302_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_eADV_A_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_eNTA_A_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_eNTA_A_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_eNTA_A_model_python2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_eNTA_X_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-03 21:47:06.000000 trusspy-2.0.0/tests/test_stiffness_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.658940 trusspy-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    33206 2023-05-08 17:49:26.000000 trusspy-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43778 2023-05-08 17:49:35.658940 trusspy-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-08 17:49:26.000000 trusspy-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 17:49:26.000000 trusspy-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:49:35.658940 trusspy-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.654940 trusspy-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.654940 trusspy-3.0.0/src/trusspy/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.654940 trusspy-3.0.0/src/trusspy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/core/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/core/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/core/external_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/core/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.654940 trusspy-3.0.0/src/trusspy/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/elements/element_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.654940 trusspy-3.0.0/src/trusspy/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/handlers/handler_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/handlers/handler_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/handlers/handler_extforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/handlers/handler_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/handlers/handler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/handlers/handler_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.658940 trusspy-3.0.0/src/trusspy/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/materials/material_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.658940 trusspy-3.0.0/src/trusspy/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/solvers/tpsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/solvers/zerosearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.658940 trusspy-3.0.0/src/trusspy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/tools/helper_functions2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/tools/movie_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-08 17:49:26.000000 trusspy-3.0.0/src/trusspy/tools/plot_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.654940 trusspy-3.0.0/src/trusspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43778 2023-05-08 17:49:35.000000 trusspy-3.0.0/src/trusspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 17:49:35.000000 trusspy-3.0.0/src/trusspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:49:35.000000 trusspy-3.0.0/src/trusspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 17:49:35.000000 trusspy-3.0.0/src/trusspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 17:49:35.000000 trusspy-3.0.0/src/trusspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:49:35.658940 trusspy-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_e102_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_e103_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_e10x_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_e10xx_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_eADV_A_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_eNTA_A_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_eNTA_A_model_python2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-08 17:49:26.000000 trusspy-3.0.0/tests/test_stiffness_function.py
```

### Comparing `trusspy-2.0.0/LICENSE` & `trusspy-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/PKG-INFO` & `trusspy-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trusspy
-Version: 2.0.0
+Version: 3.0.0
 Summary: Truss Solver for Python
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -666,17 +666,17 @@
 License-File: LICENSE
 
 <p align="center">
   <a href="https://trusspy.readthedocs.io"><img src="https://raw.githubusercontent.com/adtzlr/trusspy/main/docs/_static/logo.png" height="80px"/></a>
   <p align="center">Truss Solver for Python.</p>
 </p>
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101_nb_interactive.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101%2Fe101.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101/e101.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
-**TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. Input files may be written in Excel or directly in Python. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
+**TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
    
 Official Documentation: http://trusspy.readthedocs.io/
 
 # Installation
 Use `pip` to install TrussPy
 
 ```
@@ -709,21 +709,21 @@
 with M.ExtForces as MF:
     MF.add_force(2, (1, 0, 0))
 
 # build model, run, show results
 M.build()
 M.run()
 
-# plot results
-M.plot_model()
-M.plot_show()
+# plot results of last increment
+M.plot_model(inc=-1, contour="force")
 ```
 	
 # Online Notebook
-Try TrussPy without installation in an [Interactive Online Notebook](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb).
+Try TrussPy without installation in an [Interactive Online Notebook](
+https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101/e101.ipynb).
 
 # Changelog
 All notable changes to this project will be documented in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 # License
 TrussPy - Truss Solver for Python (C) 2023 Andreas Dutzler, Graz (Austria).
```

### Comparing `trusspy-2.0.0/README.md` & `trusspy-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <p align="center">
   <a href="https://trusspy.readthedocs.io"><img src="https://raw.githubusercontent.com/adtzlr/trusspy/main/docs/_static/logo.png" height="80px"/></a>
   <p align="center">Truss Solver for Python.</p>
 </p>
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101_nb_interactive.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101%2Fe101.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101/e101.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
-**TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. Input files may be written in Excel or directly in Python. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
+**TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
    
 Official Documentation: http://trusspy.readthedocs.io/
 
 # Installation
 Use `pip` to install TrussPy
 
 ```
@@ -42,21 +42,21 @@
 with M.ExtForces as MF:
     MF.add_force(2, (1, 0, 0))
 
 # build model, run, show results
 M.build()
 M.run()
 
-# plot results
-M.plot_model()
-M.plot_show()
+# plot results of last increment
+M.plot_model(inc=-1, contour="force")
 ```
 	
 # Online Notebook
-Try TrussPy without installation in an [Interactive Online Notebook](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb).
+Try TrussPy without installation in an [Interactive Online Notebook](
+https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101/e101.ipynb).
 
 # Changelog
 All notable changes to this project will be documented in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 # License
 TrussPy - Truss Solver for Python (C) 2023 Andreas Dutzler, Graz (Austria).
```

#### html2text {}

```diff
@@ -1,50 +1,49 @@
  [https://raw.githubusercontent.com/adtzlr/trusspy/main/docs/_static/logo.png]
                            Truss Solver for Python.
 [![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https:/
 /pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/
-main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb) [Open_In_Colab] [!
+main?labpath=docs%2Fexamples%2Fe101%2Fe101.ipynb) [Open_In_Colab] [!
 [Documentation Status](https://readthedocs.org/projects/trusspy/badge/
 ?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [!
 [License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https:/
 /www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://
 img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-
 0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/
 badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI]
 (https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/
 145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-
 black) **TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is
 capable of material and geometric nonlinearities. It uses an object-oriented
 approach to structure the code in meaningful classes, attributes and methods.
 TrussPy contains both multistep functionality (multiple loadcase analysis with
 sequenced external forces) and an adaptive method to control incremental
-stepwidths. Input files may be written in Excel or directly in Python. A simple
-post-processing inside TrussPy is directly available via Matplotlib. Model
-Plots whether in undeformed or deformed configuration with optional contour
-plots on element forces are easy to show. They may also be generated for a
-series of increments and saved as a GIF Movie. Last but not least History
-(a.k.a. x-y) Plots for a series of increments or Path Plots along a given node
-path may be generated for nodal properties (displacements, forces) or global
-quantities like the Load-Proportionality-Factor (LPF). Official Documentation:
-http://trusspy.readthedocs.io/ # Installation Use `pip` to install TrussPy ```
-pip install trusspy ``` # Example ```python import trusspy as tp M = tp.Model()
-# create nodes with M.Nodes as MN: MN.add_node(1, (0, 0, 0)) MN.add_node(2, (1,
-0, 0)) # create element with M.Elements as ME: ME.add_element(1, [1, 2])
-ME.assign_material("all", [1]) ME.assign_geometry("all", [1]) # create
-displacement (U) boundary conditions with M.Boundaries as MB: MB.add_bound_U(1,
-(0, 0, 0)) MB.add_bound_U(2, (1, 0, 0)) # create external forces with
-M.ExtForces as MF: MF.add_force(2, (1, 0, 0)) # build model, run, show results
-M.build() M.run() # plot results M.plot_model() M.plot_show() ``` # Online
-Notebook Try TrussPy without installation in an [Interactive Online Notebook]
-(https://mybinder.org/v2/gh/adtzlr/trusspy/
-main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb). # Changelog All
-notable changes to this project will be documented in [this file]
-(CHANGELOG.md). The format is based on [Keep a Changelog](https://
-keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
+stepwidths. A simple post-processing inside TrussPy is directly available via
+Matplotlib. Model Plots whether in undeformed or deformed configuration with
+optional contour plots on element forces are easy to show. They may also be
+generated for a series of increments and saved as a GIF Movie. Last but not
+least History (a.k.a. x-y) Plots for a series of increments or Path Plots along
+a given node path may be generated for nodal properties (displacements, forces)
+or global quantities like the Load-Proportionality-Factor (LPF). Official
+Documentation: http://trusspy.readthedocs.io/ # Installation Use `pip` to
+install TrussPy ``` pip install trusspy ``` # Example ```python import trusspy
+as tp M = tp.Model() # create nodes with M.Nodes as MN: MN.add_node(1, (0, 0,
+0)) MN.add_node(2, (1, 0, 0)) # create element with M.Elements as ME:
+ME.add_element(1, [1, 2]) ME.assign_material("all", [1]) ME.assign_geometry
+("all", [1]) # create displacement (U) boundary conditions with M.Boundaries as
+MB: MB.add_bound_U(1, (0, 0, 0)) MB.add_bound_U(2, (1, 0, 0)) # create external
+forces with M.ExtForces as MF: MF.add_force(2, (1, 0, 0)) # build model, run,
+show results M.build() M.run() # plot results of last increment M.plot_model
+(inc=-1, contour="force") ``` # Online Notebook Try TrussPy without
+installation in an [Interactive Online Notebook]( https://
+colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101/
+e101.ipynb). # Changelog All notable changes to this project will be documented
+in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https:/
+/keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). # License TrussPy - Truss
 Solver for Python (C) 2023 Andreas Dutzler, Graz (Austria). This program is
 free software: you can redistribute it and/or modify it under the terms of the
 GNU General Public License as published by the Free Software Foundation, either
 version 3 of the License, or (at your option) any later version. This program
 is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
```

### Comparing `trusspy-2.0.0/pyproject.toml` & `trusspy-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -42,19 +42,17 @@
 ]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
   "numpy",
   "scipy",
   "matplotlib",
-  "pandas",
-  "openpyxl",
   "imageio",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "trusspy.__about__.__version__"}
 
 [project.urls]
 Homepage = "https://trusspy.readthedocs.io/en/latest"
 Code = "https://github.com/adtzlr/trusspy"
-Issues = "https://github.com/adtzlr/trusspy/issues"
+Issues = "https://github.com/adtzlr/trusspy/issues"
```

### Comparing `trusspy-2.0.0/src/trusspy/core/analysis.py` & `trusspy-3.0.0/src/trusspy/core/analysis.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/core/boundary.py` & `trusspy-3.0.0/src/trusspy/core/boundary.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/core/element.py` & `trusspy-3.0.0/src/trusspy/core/element.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/core/external_force.py` & `trusspy-3.0.0/src/trusspy/core/external_force.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/core/node.py` & `trusspy-3.0.0/src/trusspy/core/node.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/elements/element_definition.py` & `trusspy-3.0.0/src/trusspy/elements/element_definition.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/handlers/handler_boundary.py` & `trusspy-3.0.0/src/trusspy/handlers/handler_boundary.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,24 +66,14 @@
         for n in fix_nodes:
             B = BoundaryU(n, (1, 1, 1))
             self.add_bound_U(B)
         indices = np.argsort(self.Unodes)
         self.Unodes = self.Unodes.take(indices)
         self.Uvalues = self.Uvalues.take(indices, axis=0)
 
-    def add_bound_U_matrix(self, UM):
-        # add matrix of displacement boundaries from input file
-        if self.Unodes is None:
-            self.Unodes = np.array(UM[:, 0])
-            self.Uvalues = np.array(UM[:, 1:4])
-        else:
-            self.Unodes = np.append(self.Unodes, UM[:, 0])
-            self.Uvalues = np.vstack((self.Uvalues, UM[:, 1:4]))
-        self.Uvalues[np.isnan(self.Uvalues)] = 0
-
     def add_bound_T(self, B):
         # add thermal boundary
         if self.Tnodes is None:
             self.Tnodes = np.array([B.node])
             self.Tvalues = np.array(B.value)
         else:
             self.Tnodes = np.append(self.Tnodes, B.node)
```

### Comparing `trusspy-2.0.0/src/trusspy/handlers/handler_element.py` & `trusspy-3.0.0/src/trusspy/handlers/handler_element.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,25 +107,14 @@
         self.geometric_properties = np.delete(self.geometric_properties, idx, axis=0)
 
     def add_elements(self, EE):
         "add several elements from element list to ElementManager"
         for E in EE:
             self.add_element(E)
 
-    def add_element_matrix(self, EM, MM, GM, TM):
-        # EM Element Matrix Data
-        # TM Thermal Matrix Data
-        if self.labels is None:
-            self.labels = np.array(EM[:, 0])
-            self.elem_type = np.array(EM[:, 1])
-            self.mat_type = np.array(MM[:, 1])
-            self.conns = np.array(EM[:, 2:4])
-            self.material_properties = np.vstack((MM[:, 2:12].T, TM[:, 1])).T
-            self.geometric_properties = GM[:, 1].reshape(len(GM), 1)
-
     def get_nodes(self, label):
         "choose element label and return connected end node"
         return self.conns[np.where(self.labels == label)][0]
 
     def NE(self, label):
         "choose element label and return connected end node"
         return self.conns[np.where(self.labels == label)][0, -1]
```

### Comparing `trusspy-2.0.0/src/trusspy/handlers/handler_extforce.py` & `trusspy-3.0.0/src/trusspy/handlers/handler_extforce.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,23 +39,14 @@
         self.nodes = np.delete(self.nodes, idx, axis=0)
         self.forces = np.delete(self.forces, idx, axis=0)
 
     def add_forces(self, FF):
         for F in FF:
             self.add_force(F)
 
-    def add_force_matrix(self, FM):
-        if self.nodes is None:
-            self.nodes = np.array(FM[:, 0])
-            self.forces = np.array(FM[:, 1 : 1 + 5 * 3])
-        else:
-            self.nodes = np.append(self.nodes, FM[:, 0])
-            self.forces = np.vstack((self.forces, FM[:, 1 : 1 + 5 * 3]))
-        self.forces[np.isnan(self.forces)] = 0
-
     def fix_forces(self, nodelist):
         # check for missing external forces --> set them all to zero
 
         # are nodelist entries in force-nodes?
         mask = np.isin(nodelist, self.nodes, invert=True)
         fix_nodes = nodelist[mask]  # nodes to fix
         comp = self.forces.shape[1]
```

### Comparing `trusspy-2.0.0/src/trusspy/handlers/handler_node.py` & `trusspy-3.0.0/src/trusspy/handlers/handler_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,19 +40,11 @@
         self.labels = np.delete(self.labels, idx, axis=0)
         self.coords = np.delete(self.coords, idx, axis=0)
 
     def add_nodes(self, NN):
         for N in NN:
             self.add_node(N)
 
-    def add_node_matrix(self, NM):
-        if self.labels is None:
-            self.labels = np.array(NM[:, 0])
-            self.coords = np.array(NM[:, 1:4])
-        else:
-            self.labels = np.append(self.labels, NM[:, 0])
-            self.coords = np.vstack((self.coords, NM[:, 1:4]))
-
     def fix_nodes(self):
         indices = np.argsort(self.labels)
         self.labels = self.labels.take(indices)
         self.coords = self.coords.take(indices, axis=0)
```

### Comparing `trusspy-2.0.0/src/trusspy/handlers/handler_settings.py` & `trusspy-3.0.0/src/trusspy/handlers/handler_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,9 +41,7 @@
         self.j0 = None
         self.j_pre = True
         self.j_fixed = False
 
         self.nstatev = 0
 
         self.nsteps = 1
-
-        self.logpdf = False
```

### Comparing `trusspy-2.0.0/src/trusspy/materials/material_definition.py` & `trusspy-3.0.0/src/trusspy/materials/material_definition.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/model.py` & `trusspy-3.0.0/src/trusspy/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import copy
 import sys
 import time
 from subprocess import run as sp_run
 
 import numpy as np
-import pandas as pd
 
 from .__about__ import __version__
 from .core import Analysis
 from .elements import truss
 from .handlers import (
     BoundaryHandler,
     ElementHandler,
@@ -41,16 +40,14 @@
 class Model:
     """Model Class with Nodes, Elements, Boundaries, etc.
 
     Attributes
     ----------
     stdout : sys.stdout
         get current stdout
-    file : None or str
-        name of input file (default is None)
     log : int
         Level of collecting logging informations during analysis.
         Higher numbers will collect more informations (default is 2).
     logfile : boolean
         flag for logfile creation (default is True)
     Nodes : NodeHandler
         Handles all nodes inside the model
@@ -66,15 +63,15 @@
         Handles all result data inside the model.
         A collection of all converged analysis solutions.
     Settings : SettingsHandler
         Handles all model parameters inside the model
 
     """
 
-    def __init__(self, file=None, log=2, logfile=False, logfile_name="analysis"):
+    def __init__(self, log=2, logfile=False, logfile_name="analysis"):
         """Init Model class with Nodes, Elements, Boundaries, etc. with default values.
         If an input file is specified, collect all data and create the model.
 
         Parameters
         ----------
         file : None or str, optional
             Name of input file (default is None).
@@ -85,23 +82,16 @@
             flag for logfile creation (default is True)
         logfile_name : str, optional
             The name of the log file (default is "analysis").
 
         """
 
         self.stdout = sys.stdout
-        self.file = file
         self.logfile = logfile
-
-        if self.file is not None:
-            # extract base name of input file without file extension and use it as
-            # log file name
-            self.logfile_name = ".".join(self.file.split(".")[:-1])
-        else:
-            self.logfile_name = logfile_name
+        self.logfile_name = logfile_name
 
         if self.logfile:
             sys.stdout = open(self.logfile_name + ".md", "w")
 
         if log > 1:
             if self.logfile:
                 print("```")
@@ -122,83 +112,21 @@
 
 Dutzler Andreas, Graz University of Technology, 2023
         """
             )
         if self.logfile:
             print("```")
 
-        if log > 1:
-            print("")
-        if log > 1:
-            print("# Initialize Model")
-        if log > 1:
-            print("* loading Managers\n")
-
         self.Nodes = NodeHandler()
         self.Elements = ElementHandler()
         self.Boundaries = BoundaryHandler()
         self.ExtForces = ExternalForceHandler()
         self.Settings = SettingsHandler()
-
         self.Settings.log = log
 
-        if log > 1:
-            print("    - finished.\n")
-
-        if file is not None:
-            if log > 1:
-                print('* loading INPUT-File: "' + file + '"\n')
-            Nodes = (
-                pd.read_excel(file, sheet_name="Nodes", skiprows=2)
-                .values[:, :4]
-                .astype(float)
-            )
-            Elements = (
-                pd.read_excel(file, sheet_name="Elements", skiprows=2)
-                .values[:, :10]
-                .astype(float)
-            )
-            Material = (
-                pd.read_excel(file, sheet_name="Material", skiprows=2)
-                .values[:, :10]
-                .astype(float)
-            )
-            Geometry = (
-                pd.read_excel(file, sheet_name="Geometry", skiprows=2)
-                .values[:, :10]
-                .astype(float)
-            )
-            ExtForces = (
-                pd.read_excel(file, sheet_name="ExternalForces", skiprows=2)
-                .values[:, : 1 + 5 * 3]
-                .astype(float)
-            )
-            Boundary_U = (
-                pd.read_excel(file, sheet_name="BoundaryU", skiprows=2)
-                .values[:, :4]
-                .astype(float)
-            )
-            Boundary_T = (
-                pd.read_excel(file, sheet_name="BoundaryT", skiprows=2)
-                .values[:, :2]
-                .astype(float)
-            )
-            if log > 1:
-                print("    - successful.\n")
-
-            if log > 1:
-                print("* Converting Data...\n")
-            self.Nodes.add_node_matrix(Nodes)
-            self.Elements.add_element_matrix(Elements, Material, Geometry, Boundary_T)
-            self.ExtForces.add_force_matrix(ExtForces)
-            self.Boundaries.add_bound_U_matrix(Boundary_U)
-
-            if log > 1:
-                print("    - Import finished.\n")
-
     def build(self):
         "Build Model (r,U,K,...) with Model data and dimensions."
 
         self.Results = ResultHandler()
         self.Analysis = Analysis()
 
         self.clock0_build = time.perf_counter()
@@ -236,37 +164,40 @@
         self.nproDOF1 = self.nproDOF.flatten()[np.where(self.nproBC.flatten() == 1)]
         self.ndof0 = len(self.nproDOF0)
         self.ndof1 = len(self.nproDOF1)
 
         if self.Settings.log > 1:
             print("")
             print("# Model Summary")
-
-            print('    Analysis Dimension      "ndim":', self.Settings.ndim)
-            print('    Number of Nodes       "nnodes":', self.nnodes)
-            print('    Number of Elements    "nelems":', self.nelems)
+            print('Analysis Dimension      "ndim":', self.Settings.ndim)
+            print('Number of Nodes       "nnodes":', self.nnodes)
+            print('Number of Elements    "nelems":', self.nelems)
             print(" ")
-            print('    System DOF              "ndof":', self.ndof)
-            print('    active DOF             "ndof1":', self.ndof1)
-            print('    locked DOF             "ndof2":', self.ndof0)
+            print('System DOF              "ndof":', self.ndof)
+            print('active DOF             "ndof1":', self.ndof1)
+            print('locked DOF             "ndof2":', self.ndof0)
             print(" ")
-            print('    active DOF          "nproDOF1":', self.nproDOF1)
-            print('    fixed  DOF          "nproDOF0":', self.nproDOF0)
+            print('active DOF          "nproDOF1":', self.nproDOF1)
+            print('fixed  DOF          "nproDOF0":', self.nproDOF0)
 
-        # init results, add empty increment
-        self.Results.add_increment()
         self.Analysis.build(
             self.nnodes,
             self.nelems,
             self.ndim,
             self.nproDOF0,
             self.nproDOF1,
             self.Settings.nstatev,
         )
-        self.Results.R[-1] = copy.deepcopy(self.Analysis)
+
+        # init results, add empty increment
+        self.Results.add_increment(
+            analysis=self.Analysis,
+            extforces=self.ExtForces,
+            lpf=0,
+        )
 
         self.clock1_build = time.perf_counter()
         self.time1_build = time.process_time()
 
     def run(self):
         """Run job."""
 
@@ -366,14 +297,17 @@
         self.clock0_run = time.perf_counter()
         self.time0_run = time.process_time()
 
         # reduced modified displacement vector to active DOF and LPF
         self.Analysis.Vred = np.append(self.Analysis.Ured, 0)
         self.Analysis.lpf = 0
 
+        # duplicate first increment to get right indices
+        self.Results.duplicate_first_increment()
+
         for step in range(self.Settings.nsteps):
             # maximum number of increment and maximum value per step
             if type(self.Settings.incs) == tuple:
                 incs = self.Settings.incs[step]
             else:
                 incs = self.Settings.incs
             if type(self.Settings.xlimit[0]) == tuple:
@@ -471,17 +405,14 @@
                 self.Analysis.lpf = 0.0
             else:
                 self.Results.remove_last_increment()
 
             if self.Settings.log > 0:
                 print("\nEnd of Step", step + 1)
 
-        # duplicate first increment to get right indices
-        self.Results.duplicate_first_increment()
-
         time_dclock_run = time.perf_counter() - self.clock0_run
         time_dtime_run = time.process_time() - self.time0_run
         time_dclock_build = self.clock1_build - self.clock0_build
         time_dtime_build = self.time1_build - self.time0_build
         if self.Settings.log > 1:
             print(r"\pagebreak")
             print(" ")
@@ -504,36 +435,14 @@
             )
             print(
                 '    total wall time "run":   {:10.3f} seconds\n'.format(time_dtime_run)
             )
 
         if self.logfile:
             sys.stdout = self.stdout
-            if self.Settings.logpdf:
-                sp_run(
-                    [
-                        "pandoc",
-                        self.logfile_name + ".md",
-                        "-t",
-                        "latex",
-                        "-o",
-                        self.logfile_name + ".pdf",
-                    ]
-                )
-                sp_run(
-                    [
-                        "pandoc",
-                        self.logfile_name + ".md",
-                        "-t",
-                        "html",
-                        "-s",
-                        "-o",
-                        self.logfile_name + ".html",
-                    ]
-                )
 
     def stiffness(self, Ured, analysis=None):
         """Method for evaluating the stiffness matrix. It re-shapes the stiffness matrix
         to ``K(nnodes,nnodes,ndim,ndim) --> K(nnodes*ndim,nnodes*nim)`` and returns a
         view on the reduced (active part of the) matrix
         ``K(nnodes*ndim,nnodes*nim)[active DOF rows][:,active DOF columns]``.
         """
@@ -716,21 +625,20 @@
             incs,
             **kwargs,
         )
 
     def plot_history(
         self,
         nodes=[1, 1],
-        increments=None,
         X="Displacement X",
         Y="LPF",
         fig=None,
         ax=None,
     ):
-        fig, ax = p_history(self, nodes, increments, X, Y, fig, ax)
+        fig, ax = p_history(self, nodes, X, Y, fig, ax)
         return fig, ax
 
     def plot_path(
         self, nodepath=[1], increment=-1, Y="Displacement X", fig=None, ax=None
     ):
         fig, ax = p_path(self, nodepath, increment, Y, fig, ax)
         return fig, ax
```

### Comparing `trusspy-2.0.0/src/trusspy/solvers/tpsolver.py` & `trusspy-3.0.0/src/trusspy/solvers/tpsolver.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/solvers/zerosearch.py` & `trusspy-3.0.0/src/trusspy/solvers/zerosearch.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/tools/helper_functions2.py` & `trusspy-3.0.0/src/trusspy/tools/helper_functions2.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/tools/movie_generator.py` & `trusspy-3.0.0/src/trusspy/tools/movie_generator.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/src/trusspy/tools/plot_utilities.py` & `trusspy-3.0.0/src/trusspy/tools/plot_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,21 +41,25 @@
     inc=-1,
     step=1,
 ):
     con = None
     plt.figure()
     fig, ax = None, None
 
+    if inc < 0:
+        inc = len(self.Results.R) + inc
+
     if inc == 0:
         lpf = 1.0
+        force_label = r"$[F_0]$"
+        contour = None
         title = "UNDEFORMED"
     else:
-        if inc < 0:
-            inc = len(self.Results.R) + inc
         lpf = self.Results.R[inc].lpf
+        force_label = r"$\lambda \cdot [F_0]$"
         title = f"INCREMENT: {inc}"
 
     if contour == "stretch":
         if cbar_limits == "auto":
             contour_lim = [
                 1 - max(abs(self.Results.R[inc].stretch[:, 0] - 1)),
                 1 + max(abs(self.Results.R[inc].stretch[:, 0] - 1)),
@@ -87,15 +91,17 @@
         elif contour[0] == "force":
             con_data = self.Results.R[inc].element_force[:, 0]
         elif contour[0] == "stress":
             con_data = self.Results.R[inc].element_stress[:, 0]
         con = contour[0], con_data, contour[1]
 
     textstr = (
-        r"$\mathbf{Plot}$ $\mathbf{Scale}$ $[F_0] =$ "
+        r"$\mathbf{Plot}$ $\mathbf{Scale}$ "
+        + force_label
+        + " ="
         + "{:2.1g} ".format(force_scale)
         + r"$\cdot [L]$"
     )
     f0_const = self.Results.R[inc].ExtForces.forces_const
     step = self.Results.R[inc].step
     fig, ax = plot_force(
         f0_const + lpf * self.ExtForces.forces[:, 3 * (step - 1) : 3 * step],
@@ -115,15 +121,15 @@
         size=nodesize,
     )
     fig, ax = plot_elems(
         self.Elements.conns,
         self.Nodes.coords + self.Results.R[inc].U,
         fig,
         ax,
-        color="C0",
+        color="C7",
         view=view,
         contour=con,
         lim_scale=lim_scale,
     )
 
     # these are matplotlib.patch.Patch properties
     props = dict(boxstyle="round", facecolor="C2", alpha=0.25)
@@ -175,24 +181,15 @@
     force_scale=0.5,
     nodesize=10,
     cbar_limits="auto",
     incs="all",
     **kwargs,
 ):
     if incs == "all":
-        if self.Settings.nsteps > 1:
-            b = 0
-            for s in range(self.Settings.nsteps):
-                b += self.Settings.incs[s]
-        else:
-            if type(self.Settings.incs) == tuple:
-                b = self.Settings.incs[0]
-            else:
-                b = self.Settings.incs
-        incs = range(0, b)
+        incs = range(1, len(self.Results.R))
 
     if os.path.isdir("figures/"):
         shutil.rmtree("figures/")
     os.mkdir("figures/")
     os.mkdir("figures/png/")
 
     for i in incs:
@@ -224,22 +221,20 @@
             stv_index = int(Y[-1]) - 1
             y = R.state_v[np.where(self.Nodes.labels == node)][0][stv_index]
         xx.append(x)
         yy.append(y)
 
     if fig is None:
         fig, ax = plt.subplots()
-    plot_pth(nodepath, yy, increment, Y, fig, ax)
+    fig, ax = plot_pth(nodepath, yy, increment, Y, fig, ax)
 
     return fig, ax
 
 
-def p_history(
-    self, nodes=[1, 1], increments=None, X="Displacement X", Y="LPF", fig=None, ax=None
-):
+def p_history(self, nodes=[1, 1], X="Displacement X", Y="LPF", fig=None, ax=None):
     # loop over increments
     xx = [0]
     yy = [0]
     dir_dict = {"X": 0, "Y": 1, "Z": 2}
 
     x, y = np.nan, np.nan
     for R in self.Results.R:
@@ -268,14 +263,14 @@
     if "Increments" in X:
         xx = np.arange(1 + len(self.Results.R), dtype=int)
     if "Increments" in Y:
         yy = np.arange(1 + len(self.Results.R))
 
     if fig is None:
         fig, ax = plt.subplots()
-    plot_hist(xx, yy, nodes[0], X, Y, fig, ax)
+    fig, ax = plot_hist(xx, yy, nodes[0], X, Y, fig, ax)
 
     return fig, ax
 
 
 def p_show(self):
     plt.show()
```

### Comparing `trusspy-2.0.0/src/trusspy.egg-info/PKG-INFO` & `trusspy-3.0.0/src/trusspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trusspy
-Version: 2.0.0
+Version: 3.0.0
 Summary: Truss Solver for Python
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -666,17 +666,17 @@
 License-File: LICENSE
 
 <p align="center">
   <a href="https://trusspy.readthedocs.io"><img src="https://raw.githubusercontent.com/adtzlr/trusspy/main/docs/_static/logo.png" height="80px"/></a>
   <p align="center">Truss Solver for Python.</p>
 </p>
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101_nb_interactive.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101%2Fe101.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101/e101.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
-**TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. Input files may be written in Excel or directly in Python. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
+**TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
    
 Official Documentation: http://trusspy.readthedocs.io/
 
 # Installation
 Use `pip` to install TrussPy
 
 ```
@@ -709,21 +709,21 @@
 with M.ExtForces as MF:
     MF.add_force(2, (1, 0, 0))
 
 # build model, run, show results
 M.build()
 M.run()
 
-# plot results
-M.plot_model()
-M.plot_show()
+# plot results of last increment
+M.plot_model(inc=-1, contour="force")
 ```
 	
 # Online Notebook
-Try TrussPy without installation in an [Interactive Online Notebook](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb).
+Try TrussPy without installation in an [Interactive Online Notebook](
+https://colab.research.google.com/github/adtzlr/trusspy/blob/main/docs/examples/e101/e101.ipynb).
 
 # Changelog
 All notable changes to this project will be documented in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 # License
 TrussPy - Truss Solver for Python (C) 2023 Andreas Dutzler, Graz (Austria).
```

### Comparing `trusspy-2.0.0/src/trusspy.egg-info/SOURCES.txt` & `trusspy-3.0.0/src/trusspy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -29,22 +29,15 @@
 src/trusspy/solvers/__init__.py
 src/trusspy/solvers/tpsolver.py
 src/trusspy/solvers/zerosearch.py
 src/trusspy/tools/__init__.py
 src/trusspy/tools/helper_functions2.py
 src/trusspy/tools/movie_generator.py
 src/trusspy/tools/plot_utilities.py
-tests/test_e101_model.py
-tests/test_e102_model.py
 tests/test_e102_model_python.py
 tests/test_e103_model_python.py
 tests/test_e10x_model.py
 tests/test_e10xx_model.py
-tests/test_e201_model.py
-tests/test_e202_model.py
-tests/test_e302_model.py
 tests/test_eADV_A_model_python.py
-tests/test_eNTA_A_model.py
 tests/test_eNTA_A_model_python.py
 tests/test_eNTA_A_model_python2.py
-tests/test_eNTA_X_model.py
 tests/test_stiffness_function.py
```

### Comparing `trusspy-2.0.0/tests/test_e102_model_python.py` & `trusspy-3.0.0/tests/test_e102_model_python.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/tests/test_e103_model_python.py` & `trusspy-3.0.0/tests/test_e103_model_python.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/tests/test_e10x_model.py` & `trusspy-3.0.0/tests/test_e10x_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/tests/test_e10xx_model.py` & `trusspy-3.0.0/tests/test_e10xx_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/tests/test_eADV_A_model_python.py` & `trusspy-3.0.0/tests/test_eADV_A_model_python.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/tests/test_eNTA_A_model_python.py` & `trusspy-3.0.0/tests/test_eNTA_A_model_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     M.run()
 
     ## model plot: undeformed and deformed configuration for last increment
     fig, ax = M.plot_model(
         view="3d",
         contour="force",
         lim_scale=(-3, 2, 0, 5, -1, 4),
-        force_scale=5.0,
+        force_scale=2.0,
         inc=0,
     )
     fig.savefig("model_undeformed_inc0_3d.pdf")
     fig.savefig("model_undeformed_inc0_3d.png")
 
     fig, ax = M.plot_model(
         view="xz",
@@ -142,26 +142,26 @@
         # lim_scale=1.2,
         force_scale=500.0,
         inc=pinc,
     )
     fig.savefig("model_contour-force_inc40_3d.pdf")
     fig.savefig("model_contour-force_inc40_3d.png")
 
-    M.plot_movie(
-        view="3d",
-        contour="force",
-        lim_scale=(-3, 2, 0, 5, -2, 3),  # 3D
-        # lim_scale=-5, #XZ
-        # lim_scale=(-4,4,-2,6), #XY
-        # lim_scale=(-2,6,-2,6), #YZ
-        cbar_limits=[-0.3, 0.3],
-        force_scale=50.0,
-        incs=range(0, M.Settings.incs, 1),
-    )
-    #
+    # M.plot_movie(
+    #     view="3d",
+    #     contour="force",
+    #     lim_scale=(-3, 2, 0, 5, -2, 3),  # 3D
+    #     # lim_scale=-5, #XZ
+    #     # lim_scale=(-4,4,-2,6), #XY
+    #     # lim_scale=(-2,6,-2,6), #YZ
+    #     cbar_limits=[-0.3, 0.3],
+    #     force_scale=50.0,
+    #     incs=range(0, M.Settings.incs, 1),
+    # )
+
     ## history plot
     Disp = "Displacement X"
     fig, ax = M.plot_history(nodes=[4, 4], X=Disp, Y="LPF")
     fig, ax = M.plot_history(nodes=[5, 5], X=Disp, Y="LPF", fig=fig, ax=ax)
     fig.savefig("history_node45_Disp" + Disp[-1] + "-LPF.pdf")
     fig.savefig("history_node45_Disp" + Disp[-1] + "-LPF.png")
```

### Comparing `trusspy-2.0.0/tests/test_eNTA_A_model_python2.py` & `trusspy-3.0.0/tests/test_eNTA_A_model_python2.py`

 * *Files identical despite different names*

### Comparing `trusspy-2.0.0/tests/test_stiffness_function.py` & `trusspy-3.0.0/tests/test_stiffness_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     M = create_model()
     M.Elements.assign_geometries("all", list_of_areas)
 
     M.build()
     M.run()
 
-    R0 = M.Results.R[0]
+    R0 = M.Results.R[1]
     # return K (full system), Kred (only active DOF)
     # or Kmod (see Documentation)
     return R0.Kred
 
 
 def test_stiffness_function():
     list_of_areas = [2, 3]
```


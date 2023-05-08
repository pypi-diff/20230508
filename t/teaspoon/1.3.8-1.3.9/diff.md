# Comparing `tmp/teaspoon-1.3.8.tar.gz` & `tmp/teaspoon-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teaspoon-1.3.8.tar", last modified: Mon Feb 27 14:26:47 2023, max compression
+gzip compressed data, was "teaspoon-1.3.9.tar", last modified: Mon May  8 16:20:10 2023, max compression
```

## Comparing `teaspoon-1.3.8.tar` & `teaspoon-1.3.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.621937 teaspoon-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35142 2023-02-27 14:22:40.000000 teaspoon-1.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-02-27 14:26:47.621937 teaspoon-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-02-27 14:22:40.000000 teaspoon-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-27 14:22:42.000000 teaspoon-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-27 14:26:47.621937 teaspoon-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-27 14:22:42.000000 teaspoon-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.609936 teaspoon-1.3.8/teaspoon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.613937 teaspoon-1.3.8/teaspoon/teaspoon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.613937 teaspoon-1.3.8/teaspoon/teaspoon/ML/
--rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/ML/Base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28553 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/ML/PD_Classification.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/ML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40345 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/ML/feature_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.613937 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.617937 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37504 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    23405 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/PointCloud.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/MakeData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.617937 teaspoon-1.3.8/teaspoon/teaspoon/SP/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/adaptivePart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.617937 teaspoon-1.3.8/teaspoon/teaspoon/SP/information/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/information/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/information/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/texture_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/SP/tsa_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.617937 teaspoon-1.3.8/teaspoon/teaspoon/TDA/
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/BuZZ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/Distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/Draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/PHN.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/Persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/SLSP.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/SLSP_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/TGZZ.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/TDA/c_profile_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.621937 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/FNN_n.py
--rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/MI_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/MsPE.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/PAMI_delay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-02-27 14:22:42.000000 teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/delay_LMS.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.613937 teaspoon-1.3.8/teaspoon/teaspoon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-02-27 14:26:47.000000 teaspoon-1.3.8/teaspoon/teaspoon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-02-27 14:26:47.000000 teaspoon-1.3.8/teaspoon/teaspoon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-27 14:26:47.000000 teaspoon-1.3.8/teaspoon/teaspoon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-27 14:26:47.000000 teaspoon-1.3.8/teaspoon/teaspoon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-27 14:26:47.000000 teaspoon-1.3.8/teaspoon/teaspoon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:26:47.621937 teaspoon-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_MakeData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_OrdinalPartition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_PointSummariesPHN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_SLSP.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_parameterSelection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_signalProcessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-02-27 14:22:42.000000 teaspoon-1.3.8/tests/test_texture_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.558263 teaspoon-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35142 2023-05-08 16:16:45.000000 teaspoon-1.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-08 16:20:10.558263 teaspoon-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-08 16:16:45.000000 teaspoon-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-08 16:16:46.000000 teaspoon-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-08 16:20:10.558263 teaspoon-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 16:16:46.000000 teaspoon-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.546263 teaspoon-1.3.9/teaspoon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.550263 teaspoon-1.3.9/teaspoon/teaspoon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.550263 teaspoon-1.3.9/teaspoon/teaspoon/ML/
+-rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/ML/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28553 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/ML/PD_Classification.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/ML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40345 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/ML/feature_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.550263 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.554263 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37504 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23405 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/PointCloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/MakeData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.554263 teaspoon-1.3.9/teaspoon/teaspoon/SP/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/adaptivePart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.554263 teaspoon-1.3.9/teaspoon/teaspoon/SP/information/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/information/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/information/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/texture_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/SP/tsa_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.558263 teaspoon-1.3.9/teaspoon/teaspoon/TDA/
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/BuZZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/Distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/Draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/PHN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/Persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/SLSP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/SLSP_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/TGZZ.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/TDA/c_profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.558263 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/FNN_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/MI_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/MsPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/PAMI_delay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-08 16:16:46.000000 teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/delay_LMS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.550263 teaspoon-1.3.9/teaspoon/teaspoon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-08 16:20:10.000000 teaspoon-1.3.9/teaspoon/teaspoon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-08 16:20:10.000000 teaspoon-1.3.9/teaspoon/teaspoon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 16:20:10.000000 teaspoon-1.3.9/teaspoon/teaspoon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 16:20:10.000000 teaspoon-1.3.9/teaspoon/teaspoon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:20:10.000000 teaspoon-1.3.9/teaspoon/teaspoon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:10.558263 teaspoon-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_MakeData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_OrdinalPartition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_PointSummariesPHN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_SLSP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_parameterSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_signalProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-08 16:16:46.000000 teaspoon-1.3.9/tests/test_texture_analysis.py
```

### Comparing `teaspoon-1.3.8/LICENSE.txt` & `teaspoon-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/PKG-INFO` & `teaspoon-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaspoon
-Version: 1.3.8
+Version: 1.3.9
 Summary: A Topological Signal Processing Package
 Author-email: Elizabeth Munch <muncheli@msu.edu>
 Project-URL: repository, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: homepage, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: documentation, https://teaspoontda.github.io/teaspoon/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `teaspoon-1.3.8/README.md` & `teaspoon-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/pyproject.toml` & `teaspoon-1.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build]
 
 [project]
 name = "teaspoon"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
   { name="Elizabeth Munch", email="muncheli@msu.edu" },
 ]
 description = "A Topological Signal Processing Package"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -17,15 +17,15 @@
 dependencies = ["cycler==0.11.0",
                 "fonttools==4.34.4",
                 "joblib==1.2.0",
                 "kiwisolver==1.4.4",
                 "matplotlib==3.5.2",
                 "networkx==2.8.5",
                 "numpy==1.23.1",
-                "packaging==21.3",
+                "packaging==23.1",
                 "Pillow==9.3.0",
                 "POT==0.8.2",
                 "pyentrp==0.7.1",
                 "pyparsing==3.0.9",
                 "python-dateutil==2.8.2",
                 "scikit-learn==1.1.1",
                 "scipy==1.8.1",
```

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/ML/Base.py` & `teaspoon-1.3.9/teaspoon/teaspoon/ML/Base.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/ML/PD_Classification.py` & `teaspoon-1.3.9/teaspoon/teaspoon/ML/PD_Classification.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/ML/feature_functions.py` & `teaspoon-1.3.9/teaspoon/teaspoon/ML/feature_functions.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/maps.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/maps.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/MakeData/PointCloud.py` & `teaspoon-1.3.9/teaspoon/teaspoon/MakeData/PointCloud.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/SP/adaptivePart.py` & `teaspoon-1.3.9/teaspoon/teaspoon/SP/adaptivePart.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/SP/information/entropy.py` & `teaspoon-1.3.9/teaspoon/teaspoon/SP/information/entropy.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/SP/network.py` & `teaspoon-1.3.9/teaspoon/teaspoon/SP/network.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/SP/network_tools.py` & `teaspoon-1.3.9/teaspoon/teaspoon/SP/network_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/SP/texture_analysis.py` & `teaspoon-1.3.9/teaspoon/teaspoon/SP/texture_analysis.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/SP/tsa_tools.py` & `teaspoon-1.3.9/teaspoon/teaspoon/SP/tsa_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/BuZZ.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/BuZZ.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/Distance.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/Distance.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/Draw.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/Draw.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/PHN.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/PHN.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/Persistence.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/Persistence.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/SLSP.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/SLSP.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/SLSP_tools.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/SLSP_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/TDA/TGZZ.py` & `teaspoon-1.3.9/teaspoon/teaspoon/TDA/TGZZ.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/FNN_n.py` & `teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/FNN_n.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/MI_delay.py` & `teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/MI_delay.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/MsPE.py` & `teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/MsPE.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/PAMI_delay.py` & `teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/PAMI_delay.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/autocorrelation.py` & `teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon/parameter_selection/delay_LMS.py` & `teaspoon-1.3.9/teaspoon/teaspoon/parameter_selection/delay_LMS.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon.egg-info/PKG-INFO` & `teaspoon-1.3.9/teaspoon/teaspoon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaspoon
-Version: 1.3.8
+Version: 1.3.9
 Summary: A Topological Signal Processing Package
 Author-email: Elizabeth Munch <muncheli@msu.edu>
 Project-URL: repository, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: homepage, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: documentation, https://teaspoontda.github.io/teaspoon/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `teaspoon-1.3.8/teaspoon/teaspoon.egg-info/SOURCES.txt` & `teaspoon-1.3.9/teaspoon/teaspoon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_MakeData.py` & `teaspoon-1.3.9/tests/test_MakeData.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_OrdinalPartition.py` & `teaspoon-1.3.9/tests/test_OrdinalPartition.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_PointSummariesPHN.py` & `teaspoon-1.3.9/tests/test_PointSummariesPHN.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_SLSP.py` & `teaspoon-1.3.9/tests/test_SLSP.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_basics.py` & `teaspoon-1.3.9/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_classification.py` & `teaspoon-1.3.9/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_parameterSelection.py` & `teaspoon-1.3.9/tests/test_parameterSelection.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_signalProcessing.py` & `teaspoon-1.3.9/tests/test_signalProcessing.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.3.8/tests/test_texture_analysis.py` & `teaspoon-1.3.9/tests/test_texture_analysis.py`

 * *Files identical despite different names*

